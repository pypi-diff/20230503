# Comparing `tmp/openhab_pythonrule_engine-1.1.8.tar.gz` & `tmp/openhab_pythonrule_engine-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openhab_pythonrule_engine-1.1.8.tar", last modified: Fri Feb 25 06:21:37 2022, max compression
+gzip compressed data, was "dist/openhab_pythonrule_engine-1.1.9.tar", last modified: Sat Mar 26 20:57:32 2022, max compression
```

## Comparing `openhab_pythonrule_engine-1.1.8.tar` & `openhab_pythonrule_engine-1.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 06:21:37.000000 openhab_pythonrule_engine-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     4719 2022-02-25 06:21:37.000000 openhab_pythonrule_engine-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3596 2022-02-25 06:21:23.000000 openhab_pythonrule_engine-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 06:21:37.000000 openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine/
--rw-r--r--   0 runner    (1001) docker     (121)     3327 2022-02-25 06:21:23.000000 openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5443 2022-02-25 06:21:23.000000 openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine/app.py
--rw-r--r--   0 runner    (1001) docker     (121)      537 2022-02-25 06:21:23.000000 openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     3195 2022-02-25 06:21:23.000000 openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine/condition.py
--rw-r--r--   0 runner    (1001) docker     (121)     2108 2022-02-25 06:21:23.000000 openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine/eventbus_consumer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1712 2022-02-25 06:21:23.000000 openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine/invoke.py
--rw-r--r--   0 runner    (1001) docker     (121)    11212 2022-02-25 06:21:23.000000 openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine/item_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)    13614 2022-02-25 06:21:23.000000 openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine/rule_engine.py
--rw-r--r--   0 runner    (1001) docker     (121)     3031 2022-02-25 06:21:23.000000 openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine/rule_engine_webthing.py
--rw-r--r--   0 runner    (1001) docker     (121)     5118 2022-02-25 06:21:23.000000 openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 06:21:37.000000 openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4719 2022-02-25 06:21:36.000000 openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-02-25 06:21:37.000000 openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-25 06:21:36.000000 openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-02-25 06:21:36.000000 openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-02-25 06:21:36.000000 openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-02-25 06:21:36.000000 openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-25 06:21:37.000000 openhab_pythonrule_engine-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1414 2022-02-25 06:21:23.000000 openhab_pythonrule_engine-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 20:57:32.000000 openhab_pythonrule_engine-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     4719 2022-03-26 20:57:32.000000 openhab_pythonrule_engine-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3596 2022-03-26 20:57:22.000000 openhab_pythonrule_engine-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 20:57:32.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/
+-rw-r--r--   0 runner    (1001) docker     (121)     3327 2022-03-26 20:57:22.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5443 2022-03-26 20:57:22.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)      537 2022-03-26 20:57:22.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3195 2022-03-26 20:57:22.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/condition.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2108 2022-03-26 20:57:22.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/eventbus_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1712 2022-03-26 20:57:22.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11429 2022-03-26 20:57:22.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/item_registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13613 2022-03-26 20:57:22.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/rule_engine.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3031 2022-03-26 20:57:22.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/rule_engine_webthing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5118 2022-03-26 20:57:22.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 20:57:32.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4719 2022-03-26 20:57:31.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      713 2022-03-26 20:57:31.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-26 20:57:31.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-03-26 20:57:31.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2022-03-26 20:57:31.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-03-26 20:57:31.000000 openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-26 20:57:32.000000 openhab_pythonrule_engine-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1414 2022-03-26 20:57:22.000000 openhab_pythonrule_engine-1.1.9/setup.py
```

### Comparing `openhab_pythonrule_engine-1.1.8/PKG-INFO` & `openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openhab_pythonrule_engine
-Version: 1.1.8
+Name: openhab-pythonrule-engine
+Version: 1.1.9
 Summary: Openhab python rule engine
 Home-page: https://github.com/grro/openhab_pythonrule_engine
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # OpenHAB python rule engine
         A python 3.x rule engine for OpenHAB. This rule engine allows defining rule by using python 3.x.
```

### Comparing `openhab_pythonrule_engine-1.1.8/README.md` & `openhab_pythonrule_engine-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine/__init__.py` & `openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine/app.py` & `openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/app.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine/cache.py` & `openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/cache.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine/condition.py` & `openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/condition.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine/eventbus_consumer.py` & `openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/eventbus_consumer.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine/invoke.py` & `openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/invoke.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine/item_registry.py` & `openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/item_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,16 +226,18 @@
         try:
             response = requests.get(uri, headers={"Accept": "application/json"}, auth = self.credentials)
             if response.status_code == 200:
                 data = response.json()
                 return to_item(data)
             elif response.status_code == 404:
                 raise Exception("item " +   uri + " not exists " + response.text)
+            elif response.status_code == 401:
+                raise Exception("auth error. user=" + self.credentials.username)
             else:
-                raise Exception("could not read item state " +   uri +  " got error " + response.text)
+                raise Exception("could not read item state " +  uri +  " got error " + response.text)
         except Exception as e:
             logging.warning("error occurred by calling " + uri, e)
 
     def has_item(self, item_name: str) -> bool:
         if item_name is None:
             return False
         else:
@@ -248,14 +250,16 @@
         uri = self.openhab_uri+ "rest/items/" + item_name
         try:
             response = requests.post(uri, data=value, headers={"Content-type": "text/plain"}, auth = self.credentials)
             if response.status_code == 200:
                 return
             elif response.status_code == 404:
                 raise Exception("item " +   uri + " not exists " + response.text)
+            elif response.status_code == 401:
+                raise Exception("auth error. user=" + self.credentials.username)
             else:
                 raise Exception("could not update item state " +   uri +  " got error " + response.text)
         except Exception as e:
             logging.warning("error occurred by performing put on " + uri, e)
 
     def get_item_metadata(self, item_name: str) -> Optional[Item]:
         items_meta_data = self.get_items(use_cache=True)
@@ -291,15 +295,15 @@
             return dflt
         else:
             return state.get_state_as_text()
 
     def get_state_as_datetime(self, item_name: str, datetime_string: str="1970-01-01") -> datetime:
         state = self.get_item(item_name)
         if state is None or state.value is None:
-            return datetime.fromtimestamp(parser.parse(datetime_string).timestamp())
+            return parser.parse(datetime_string)
         else:
             return state.get_state_as_datetime()
 
 
     def set_state(self, item_name: str, new_state, reason: str = "", log_level: int = INFO) -> bool:
         if new_state is None:
             logging.warning("try to set " + item_name + " = None. ignoring it")
```

### Comparing `openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine/rule_engine.py` & `openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/rule_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,9 +346,9 @@
                 rule.add_trigger(ManualTrigger(func))
                 for trigger in triggers:
                     if trigger.name == rule.name:
                         rule.add_trigger(trigger)
                 rules.add(rule)
         return sorted(list(rules))
 
-#RuleEngine.start_singleton("http://192.168.1.27:8080", "C:\\workspace\\test", "xxx", "secret")
+#RuleEngine.start_singleton("http://192.168.1.27:8080", "C:\\workspace\\test", "test", "test")
 #sleep(10000)
```

### Comparing `openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine/rule_engine_webthing.py` & `openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/rule_engine_webthing.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine/trigger.py` & `openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine/trigger.py`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine.egg-info/PKG-INFO` & `openhab_pythonrule_engine-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openhab-pythonrule-engine
-Version: 1.1.8
+Name: openhab_pythonrule_engine
+Version: 1.1.9
 Summary: Openhab python rule engine
 Home-page: https://github.com/grro/openhab_pythonrule_engine
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # OpenHAB python rule engine
         A python 3.x rule engine for OpenHAB. This rule engine allows defining rule by using python 3.x.
```

### Comparing `openhab_pythonrule_engine-1.1.8/openhab_pythonrule_engine.egg-info/SOURCES.txt` & `openhab_pythonrule_engine-1.1.9/openhab_pythonrule_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openhab_pythonrule_engine-1.1.8/setup.py` & `openhab_pythonrule_engine-1.1.9/setup.py`

 * *Files identical despite different names*

