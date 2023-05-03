# Comparing `tmp/rungalileo-tidecv-0.0.3.tar.gz` & `tmp/rungalileo-tidecv-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rungalileo-tidecv-0.0.3.tar", last modified: Thu Apr 13 16:50:35 2023, max compression
+gzip compressed data, was "rungalileo-tidecv-0.0.4.tar", last modified: Wed May  3 16:30:01 2023, max compression
```

## Comparing `rungalileo-tidecv-0.0.3.tar` & `rungalileo-tidecv-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 benepstein   (501) staff       (20)        0 2023-04-13 16:50:35.556410 rungalileo-tidecv-0.0.3/
--rw-r--r--   0 benepstein   (501) staff       (20)     1055 2023-04-05 13:21:58.000000 rungalileo-tidecv-0.0.3/LICENSE
--rw-r--r--   0 benepstein   (501) staff       (20)     3971 2023-04-13 16:50:35.556048 rungalileo-tidecv-0.0.3/PKG-INFO
--rw-r--r--   0 benepstein   (501) staff       (20)     3431 2023-04-05 13:21:58.000000 rungalileo-tidecv-0.0.3/README.md
-drwxr-xr-x   0 benepstein   (501) staff       (20)        0 2023-04-13 16:50:35.544806 rungalileo-tidecv-0.0.3/rungalileo_tidecv.egg-info/
--rw-r--r--   0 benepstein   (501) staff       (20)     3971 2023-04-13 16:50:35.000000 rungalileo-tidecv-0.0.3/rungalileo_tidecv.egg-info/PKG-INFO
--rw-r--r--   0 benepstein   (501) staff       (20)      434 2023-04-13 16:50:35.000000 rungalileo-tidecv-0.0.3/rungalileo_tidecv.egg-info/SOURCES.txt
--rw-r--r--   0 benepstein   (501) staff       (20)        1 2023-04-13 16:50:35.000000 rungalileo-tidecv-0.0.3/rungalileo_tidecv.egg-info/dependency_links.txt
--rw-r--r--   0 benepstein   (501) staff       (20)       33 2023-04-13 16:50:35.000000 rungalileo-tidecv-0.0.3/rungalileo_tidecv.egg-info/requires.txt
--rw-r--r--   0 benepstein   (501) staff       (20)        7 2023-04-13 16:50:35.000000 rungalileo-tidecv-0.0.3/rungalileo_tidecv.egg-info/top_level.txt
--rw-r--r--   0 benepstein   (501) staff       (20)       38 2023-04-13 16:50:35.556575 rungalileo-tidecv-0.0.3/setup.cfg
--rw-r--r--   0 benepstein   (501) staff       (20)     1214 2023-04-13 15:04:15.000000 rungalileo-tidecv-0.0.3/setup.py
-drwxr-xr-x   0 benepstein   (501) staff       (20)        0 2023-04-13 16:50:35.551152 rungalileo-tidecv-0.0.3/tidecv/
--rw-r--r--   0 benepstein   (501) staff       (20)      103 2023-04-13 14:59:03.000000 rungalileo-tidecv-0.0.3/tidecv/__init__.py
--rw-r--r--   0 benepstein   (501) staff       (20)    10968 2023-04-05 13:33:47.000000 rungalileo-tidecv-0.0.3/tidecv/ap.py
--rw-r--r--   0 benepstein   (501) staff       (20)     4733 2023-04-13 14:56:12.000000 rungalileo-tidecv-0.0.3/tidecv/data.py
--rw-r--r--   0 benepstein   (501) staff       (20)    11375 2023-04-05 13:33:47.000000 rungalileo-tidecv-0.0.3/tidecv/datasets.py
-drwxr-xr-x   0 benepstein   (501) staff       (20)        0 2023-04-13 16:50:35.554985 rungalileo-tidecv-0.0.3/tidecv/errors/
--rw-r--r--   0 benepstein   (501) staff       (20)     2927 2023-04-05 13:33:29.000000 rungalileo-tidecv-0.0.3/tidecv/errors/error.py
--rw-r--r--   0 benepstein   (501) staff       (20)     3081 2023-04-13 16:36:57.000000 rungalileo-tidecv-0.0.3/tidecv/errors/main_errors.py
--rw-r--r--   0 benepstein   (501) staff       (20)     1329 2023-04-05 13:21:58.000000 rungalileo-tidecv-0.0.3/tidecv/errors/qualifiers.py
--rw-r--r--   0 benepstein   (501) staff       (20)     3010 2023-04-05 13:33:47.000000 rungalileo-tidecv-0.0.3/tidecv/functions.py
--rw-r--r--   0 benepstein   (501) staff       (20)     1116 2023-04-05 13:21:58.000000 rungalileo-tidecv-0.0.3/tidecv/plotting.py
--rw-r--r--   0 benepstein   (501) staff       (20)    27034 2023-04-13 16:36:57.000000 rungalileo-tidecv-0.0.3/tidecv/quantify.py
+drwxr-xr-x   0 benepstein   (501) staff       (20)        0 2023-05-03 16:30:01.252567 rungalileo-tidecv-0.0.4/
+-rw-r--r--   0 benepstein   (501) staff       (20)     1055 2023-04-05 13:21:58.000000 rungalileo-tidecv-0.0.4/LICENSE
+-rw-r--r--   0 benepstein   (501) staff       (20)     3971 2023-05-03 16:30:01.252232 rungalileo-tidecv-0.0.4/PKG-INFO
+-rw-r--r--   0 benepstein   (501) staff       (20)     3431 2023-04-05 13:21:58.000000 rungalileo-tidecv-0.0.4/README.md
+drwxr-xr-x   0 benepstein   (501) staff       (20)        0 2023-05-03 16:30:01.242320 rungalileo-tidecv-0.0.4/rungalileo_tidecv.egg-info/
+-rw-r--r--   0 benepstein   (501) staff       (20)     3971 2023-05-03 16:30:01.000000 rungalileo-tidecv-0.0.4/rungalileo_tidecv.egg-info/PKG-INFO
+-rw-r--r--   0 benepstein   (501) staff       (20)      434 2023-05-03 16:30:01.000000 rungalileo-tidecv-0.0.4/rungalileo_tidecv.egg-info/SOURCES.txt
+-rw-r--r--   0 benepstein   (501) staff       (20)        1 2023-05-03 16:30:01.000000 rungalileo-tidecv-0.0.4/rungalileo_tidecv.egg-info/dependency_links.txt
+-rw-r--r--   0 benepstein   (501) staff       (20)       33 2023-05-03 16:30:01.000000 rungalileo-tidecv-0.0.4/rungalileo_tidecv.egg-info/requires.txt
+-rw-r--r--   0 benepstein   (501) staff       (20)        7 2023-05-03 16:30:01.000000 rungalileo-tidecv-0.0.4/rungalileo_tidecv.egg-info/top_level.txt
+-rw-r--r--   0 benepstein   (501) staff       (20)       38 2023-05-03 16:30:01.252698 rungalileo-tidecv-0.0.4/setup.cfg
+-rw-r--r--   0 benepstein   (501) staff       (20)     1214 2023-05-03 16:28:29.000000 rungalileo-tidecv-0.0.4/setup.py
+drwxr-xr-x   0 benepstein   (501) staff       (20)        0 2023-05-03 16:30:01.248431 rungalileo-tidecv-0.0.4/tidecv/
+-rw-r--r--   0 benepstein   (501) staff       (20)      103 2023-05-03 16:28:43.000000 rungalileo-tidecv-0.0.4/tidecv/__init__.py
+-rw-r--r--   0 benepstein   (501) staff       (20)    11096 2023-05-03 16:29:39.000000 rungalileo-tidecv-0.0.4/tidecv/ap.py
+-rw-r--r--   0 benepstein   (501) staff       (20)     4733 2023-04-13 14:56:12.000000 rungalileo-tidecv-0.0.4/tidecv/data.py
+-rw-r--r--   0 benepstein   (501) staff       (20)    11375 2023-04-05 13:33:47.000000 rungalileo-tidecv-0.0.4/tidecv/datasets.py
+drwxr-xr-x   0 benepstein   (501) staff       (20)        0 2023-05-03 16:30:01.251300 rungalileo-tidecv-0.0.4/tidecv/errors/
+-rw-r--r--   0 benepstein   (501) staff       (20)     2927 2023-04-05 13:33:29.000000 rungalileo-tidecv-0.0.4/tidecv/errors/error.py
+-rw-r--r--   0 benepstein   (501) staff       (20)     3081 2023-04-13 16:36:57.000000 rungalileo-tidecv-0.0.4/tidecv/errors/main_errors.py
+-rw-r--r--   0 benepstein   (501) staff       (20)     1329 2023-04-05 13:21:58.000000 rungalileo-tidecv-0.0.4/tidecv/errors/qualifiers.py
+-rw-r--r--   0 benepstein   (501) staff       (20)     3010 2023-04-05 13:33:47.000000 rungalileo-tidecv-0.0.4/tidecv/functions.py
+-rw-r--r--   0 benepstein   (501) staff       (20)     1116 2023-04-05 13:21:58.000000 rungalileo-tidecv-0.0.4/tidecv/plotting.py
+-rw-r--r--   0 benepstein   (501) staff       (20)    27034 2023-04-13 16:36:57.000000 rungalileo-tidecv-0.0.4/tidecv/quantify.py
```

### Comparing `rungalileo-tidecv-0.0.3/LICENSE` & `rungalileo-tidecv-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.3/PKG-INFO` & `rungalileo-tidecv-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rungalileo-tidecv
-Version: 0.0.3
+Version: 0.0.4
 Summary: A General Toolbox for Identifying ObjectDetection Errors
 Home-page: https://github.com/rungalileo/tide
 Author: Galileo
 Author-email: galileo@rungalileo.io
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rungalileo-tidecv-0.0.3/README.md` & `rungalileo-tidecv-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.3/rungalileo_tidecv.egg-info/PKG-INFO` & `rungalileo-tidecv-0.0.4/rungalileo_tidecv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rungalileo-tidecv
-Version: 0.0.3
+Version: 0.0.4
 Summary: A General Toolbox for Identifying ObjectDetection Errors
 Home-page: https://github.com/rungalileo/tide
 Author: Galileo
 Author-email: galileo@rungalileo.io
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rungalileo-tidecv-0.0.3/setup.py` & `rungalileo-tidecv-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.3/tidecv/ap.py` & `rungalileo-tidecv-0.0.4/tidecv/ap.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,14 +144,17 @@
         self.objs[class_].push_false_negative(id)
 
     def add_gt_positives(self, class_: int, num_positives: int):
         self.objs[class_].add_gt_positives(num_positives)
 
     def get_mAP(self) -> float:
         aps = [x.get_ap() for x in self.objs.values() if not x.is_empty()]
+        # If there are no objects (no golds, no preds), then it's a perfect run
+        if not aps:
+            return 100.0
         return sum(aps) / len(aps)
 
     def get_gt_positives(self) -> dict:
         return {k: v.num_gt_positives for k, v in self.objs.items()}
 
     def get_pr_curve(self, cat_id: int = None) -> tuple:
         if cat_id is None:
```

### Comparing `rungalileo-tidecv-0.0.3/tidecv/data.py` & `rungalileo-tidecv-0.0.4/tidecv/data.py`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.3/tidecv/datasets.py` & `rungalileo-tidecv-0.0.4/tidecv/datasets.py`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.3/tidecv/errors/error.py` & `rungalileo-tidecv-0.0.4/tidecv/errors/error.py`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.3/tidecv/errors/main_errors.py` & `rungalileo-tidecv-0.0.4/tidecv/errors/main_errors.py`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.3/tidecv/errors/qualifiers.py` & `rungalileo-tidecv-0.0.4/tidecv/errors/qualifiers.py`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.3/tidecv/functions.py` & `rungalileo-tidecv-0.0.4/tidecv/functions.py`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.3/tidecv/plotting.py` & `rungalileo-tidecv-0.0.4/tidecv/plotting.py`

 * *Files identical despite different names*

### Comparing `rungalileo-tidecv-0.0.3/tidecv/quantify.py` & `rungalileo-tidecv-0.0.4/tidecv/quantify.py`

 * *Files identical despite different names*

