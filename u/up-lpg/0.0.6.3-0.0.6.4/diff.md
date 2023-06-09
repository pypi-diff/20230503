# Comparing `tmp/up_lpg-0.0.6.3-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/up_lpg-0.0.6.4-pp39-pypy39_pp73-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 1190327 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       36 b- defN 23-Apr-21 16:03 up_lpg/__init__.py
--rw-rw-rw-  2.0 fat     9730 b- defN 23-Apr-21 16:03 up_lpg/lpg_planner.py
--rw-rw-rw-  2.0 fat  3881596 b- defN 23-Apr-21 16:03 up_lpg/winlpg.exe
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Apr-21 16:11 up_lpg-0.0.6.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      336 b- defN 23-Apr-21 16:11 up_lpg-0.0.6.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 23-Apr-21 16:11 up_lpg-0.0.6.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-21 16:11 up_lpg-0.0.6.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      619 b- defN 23-Apr-21 16:11 up_lpg-0.0.6.3.dist-info/RECORD
-8 files, 3903989 bytes uncompressed, 1189257 bytes compressed:  69.6%
+Zip file size: 1190490 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat       36 b- defN 23-May-03 12:54 up_lpg/__init__.py
+-rw-rw-rw-  2.0 fat    10761 b- defN 23-May-03 12:54 up_lpg/lpg_planner.py
+-rw-rw-rw-  2.0 fat  3881596 b- defN 23-May-03 12:54 up_lpg/winlpg.exe
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-May-03 13:03 up_lpg-0.0.6.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      336 b- defN 23-May-03 13:03 up_lpg-0.0.6.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      107 b- defN 23-May-03 13:03 up_lpg-0.0.6.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-May-03 13:03 up_lpg-0.0.6.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      620 b- defN 23-May-03 13:03 up_lpg-0.0.6.4.dist-info/RECORD
+8 files, 3905021 bytes uncompressed, 1189420 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: up_lpg/lpg_planner.py
 Comment: 
 
 Filename: up_lpg/winlpg.exe
 Comment: 
 
-Filename: up_lpg-0.0.6.3.dist-info/LICENSE
+Filename: up_lpg-0.0.6.4.dist-info/LICENSE
 Comment: 
 
-Filename: up_lpg-0.0.6.3.dist-info/METADATA
+Filename: up_lpg-0.0.6.4.dist-info/METADATA
 Comment: 
 
-Filename: up_lpg-0.0.6.3.dist-info/WHEEL
+Filename: up_lpg-0.0.6.4.dist-info/WHEEL
 Comment: 
 
-Filename: up_lpg-0.0.6.3.dist-info/top_level.txt
+Filename: up_lpg-0.0.6.4.dist-info/top_level.txt
 Comment: 
 
-Filename: up_lpg-0.0.6.3.dist-info/RECORD
+Filename: up_lpg-0.0.6.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## up_lpg/lpg_planner.py

```diff
@@ -52,31 +52,43 @@
                 'up.model.Object',
                 'up.model.Parameter',
                 'up.model.Variable',
             ],
         ],) -> 'up.plans.Plan':
         '''Takes a problem and a filename and returns the plan parsed from the file.'''
         actions = []
+        tt = False
+        if 'CONTINUOUS_TIME' in problem.kind.features:
+            tt = True
         with open(plan_filename) as plan:
             for line in plan.readlines():
                 if re.match(r'^\s*(;.*)?$', line):
                     continue
                 res = re.match(r'^[\d.]+:\s*\(\s*([\w?-]+)((\s+[\w?-]+)*)\s*\)\s*\[.*\]$', line.lower().split(' ;;')[0])
                 if res:
                     action = get_item_named(res.group(1))
                     parameters = []
                     for p in res.group(2).split():
                         p_correct = get_item_named(p)
                         parameters.append(problem.environment.expression_manager.ObjectExp(p_correct))
-                    actions.append(up.plans.ActionInstance(action, tuple(parameters)))
+                    if tt:
+                        start = re.match(r'^([\d.]+):', line).group(1)
+                        dur = re.match(r'^[\d.]+:\s*\(\s*[\w?-]+((\s+[\w?-]+)*)\s*\)\s*\[([\d.]+)\]$', line).group(3)                                                                                               
+                        actions.append((start,up.plans.ActionInstance(action, tuple(parameters)),dur))
+                    else:
+                        actions.append(up.plans.ActionInstance(action, tuple(parameters)))
                 elif re.match(r'no solution', line):
                     return None
                 else:
                     raise UPException('Error parsing plan generated by ' + self.__class__.__name__)
-        return up.plans.SequentialPlan(actions)
+                
+        if tt:
+            return up.plans.TimeTriggeredPlan(actions)
+        else:
+            return up.plans.SequentialPlan(actions)
 
     def _result_status(
         self,
         problem: 'up.model.Problem',
         plan: Optional['up.plan.Plan'],
         retval: int = 0,
         log_messages: Optional[List['LogMessage']] = None,
@@ -98,17 +110,21 @@
         supported_kind.set_typing('FLAT_TYPING')  # type: ignore
         supported_kind.set_typing('HIERARCHICAL_TYPING')  # type: ignore
         supported_kind.set_fluents_type('NUMERIC_FLUENTS')  # type: ignore
         supported_kind.set_conditions_kind('EQUALITIES')  # type: ignore
         supported_kind.set_numbers('DISCRETE_NUMBERS')  # type: ignore
         supported_kind.set_effects_kind('INCREASE_EFFECTS')  # type: ignore
         supported_kind.set_effects_kind('DECREASE_EFFECTS')  # type: ignore
+        supported_kind.set_effects_kind('STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS')  # type: ignore
+        supported_kind.set_effects_kind('FLUENTS_IN_NUMERIC_ASSIGNMENTS')  # type: ignore
         supported_kind.set_time('CONTINUOUS_TIME')  # type: ignore
         supported_kind.set_quality_metrics('PLAN_LENGTH') # type: ignore
         supported_kind.set_expression_duration('STATIC_FLUENTS_IN_DURATIONS')  # type: ignore
+        supported_kind.set_actions_cost_kind('STATIC_FLUENTS_IN_ACTIONS_COST')  # type: ignore
+        supported_kind.set_actions_cost_kind('FLUENTS_IN_ACTIONS_COST')  # type: ignore
         return supported_kind
 
     @staticmethod
     def supports(problem_kind: 'ProblemKind') -> bool:
         return problem_kind <= LPGEngine.supported_kind()
 
     @staticmethod
```

## Comparing `up_lpg-0.0.6.3.dist-info/LICENSE` & `up_lpg-0.0.6.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `up_lpg-0.0.6.3.dist-info/RECORD` & `up_lpg-0.0.6.4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 up_lpg/__init__.py,sha256=cD1uY16onwsxHOEI1I-lmF6WlYtDKB8YOie6BNUZji0,36
-up_lpg/lpg_planner.py,sha256=VMScu5mMTLilyGRqJQjX4JFZmREHnppxSXE_K-Av4uI,9730
+up_lpg/lpg_planner.py,sha256=TwnTTRPMehwz7fItTlonTt9VLhrR6YRJgxyQE-QFs7o,10761
 up_lpg/winlpg.exe,sha256=Ut1frT86CopooTsvbc20MyQGGUrmRtWnVLObmzp4v4w,3881596
-up_lpg-0.0.6.3.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-up_lpg-0.0.6.3.dist-info/METADATA,sha256=zm3sgRHE1DxL6tfpIgwsRVTEnvtl351j_vVaTLngyZU,336
-up_lpg-0.0.6.3.dist-info/WHEEL,sha256=kbzA5tyEuvWcVsltnhCG02Vwq0RkG0K4o74bVDVA1mQ,107
-up_lpg-0.0.6.3.dist-info/top_level.txt,sha256=p4RjFqpyQ96YXeEcg2Qtkfgt61fd_rOwRCePcthjdUk,7
-up_lpg-0.0.6.3.dist-info/RECORD,,
+up_lpg-0.0.6.4.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+up_lpg-0.0.6.4.dist-info/METADATA,sha256=zMbClZdz8mu0KRQQy5-jH_MNuekepqpe21De9tDTh9s,336
+up_lpg-0.0.6.4.dist-info/WHEEL,sha256=kbzA5tyEuvWcVsltnhCG02Vwq0RkG0K4o74bVDVA1mQ,107
+up_lpg-0.0.6.4.dist-info/top_level.txt,sha256=p4RjFqpyQ96YXeEcg2Qtkfgt61fd_rOwRCePcthjdUk,7
+up_lpg-0.0.6.4.dist-info/RECORD,,
```

