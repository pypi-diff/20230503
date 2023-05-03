# Comparing `tmp/classconfig-1.0.1.tar.gz` & `tmp/classconfig-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classconfig-1.0.1.tar", last modified: Thu Apr 27 11:57:19 2023, max compression
+gzip compressed data, was "classconfig-1.0.2.tar", last modified: Wed May  3 08:15:34 2023, max compression
```

## Comparing `classconfig-1.0.1.tar` & `classconfig-1.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2023-04-27 11:57:19.942717 classconfig-1.0.1/
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     1211 2022-05-31 11:17:31.000000 classconfig-1.0.1/LICENSE
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       24 2023-04-27 11:55:37.000000 classconfig-1.0.1/MANIFEST.in
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     3770 2023-04-27 11:57:19.942717 classconfig-1.0.1/PKG-INFO
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     3320 2023-04-27 10:43:07.000000 classconfig-1.0.1/README.md
-drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2023-04-27 11:57:19.938717 classconfig-1.0.1/classconfig/
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)      111 2023-04-26 13:54:46.000000 classconfig-1.0.1/classconfig/__init__.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2845 2023-04-26 14:19:24.000000 classconfig-1.0.1/classconfig/base.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2527 2023-04-26 13:46:41.000000 classconfig-1.0.1/classconfig/classes.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)    38514 2023-04-27 11:23:27.000000 classconfig-1.0.1/classconfig/configurable.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     7128 2023-04-27 11:23:40.000000 classconfig-1.0.1/classconfig/transforms.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     9236 2023-04-27 10:56:32.000000 classconfig-1.0.1/classconfig/validators.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)      382 2023-04-26 15:16:39.000000 classconfig-1.0.1/classconfig/yaml.py
-drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2023-04-27 11:57:19.942717 classconfig-1.0.1/classconfig.egg-info/
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     3770 2023-04-27 11:57:19.000000 classconfig-1.0.1/classconfig.egg-info/PKG-INFO
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)      516 2023-04-27 11:57:19.000000 classconfig-1.0.1/classconfig.egg-info/SOURCES.txt
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)        1 2023-04-27 11:57:19.000000 classconfig-1.0.1/classconfig.egg-info/dependency_links.txt
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       21 2023-04-27 11:57:19.000000 classconfig-1.0.1/classconfig.egg-info/requires.txt
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       12 2023-04-27 11:57:19.000000 classconfig-1.0.1/classconfig.egg-info/top_level.txt
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       20 2023-04-26 13:45:04.000000 classconfig-1.0.1/requirements.txt
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       38 2023-04-27 11:57:19.942717 classconfig-1.0.1/setup.cfg
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     1115 2023-04-27 11:57:03.000000 classconfig-1.0.1/setup.py
-drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2023-04-27 11:57:19.942717 classconfig-1.0.1/tests/
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2626 2023-04-27 11:14:46.000000 classconfig-1.0.1/tests/test_classes.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)    23630 2023-04-26 15:10:49.000000 classconfig-1.0.1/tests/test_configurable.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     1948 2023-04-27 10:43:21.000000 classconfig-1.0.1/tests/test_readme.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2521 2023-04-27 11:32:32.000000 classconfig-1.0.1/tests/test_transforms.py
--rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     5872 2023-04-27 11:12:58.000000 classconfig-1.0.1/tests/test_validators.py
+drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2023-05-03 08:15:34.227396 classconfig-1.0.2/
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     1211 2022-05-31 11:17:31.000000 classconfig-1.0.2/LICENSE
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       24 2023-04-27 11:55:37.000000 classconfig-1.0.2/MANIFEST.in
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     3770 2023-05-03 08:15:34.227396 classconfig-1.0.2/PKG-INFO
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     3320 2023-04-27 10:43:07.000000 classconfig-1.0.2/README.md
+drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2023-05-03 08:15:34.223396 classconfig-1.0.2/classconfig/
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)      111 2023-04-26 13:54:46.000000 classconfig-1.0.2/classconfig/__init__.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2845 2023-04-26 14:19:24.000000 classconfig-1.0.2/classconfig/base.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2527 2023-04-26 13:46:41.000000 classconfig-1.0.2/classconfig/classes.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)    38658 2023-05-03 08:13:31.000000 classconfig-1.0.2/classconfig/configurable.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     7128 2023-04-27 11:23:40.000000 classconfig-1.0.2/classconfig/transforms.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     9236 2023-04-27 10:56:32.000000 classconfig-1.0.2/classconfig/validators.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)      382 2023-04-26 15:16:39.000000 classconfig-1.0.2/classconfig/yaml.py
+drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2023-05-03 08:15:34.227396 classconfig-1.0.2/classconfig.egg-info/
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     3770 2023-05-03 08:15:34.000000 classconfig-1.0.2/classconfig.egg-info/PKG-INFO
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)      516 2023-05-03 08:15:34.000000 classconfig-1.0.2/classconfig.egg-info/SOURCES.txt
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)        1 2023-05-03 08:15:34.000000 classconfig-1.0.2/classconfig.egg-info/dependency_links.txt
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       21 2023-05-03 08:15:34.000000 classconfig-1.0.2/classconfig.egg-info/requires.txt
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       12 2023-05-03 08:15:34.000000 classconfig-1.0.2/classconfig.egg-info/top_level.txt
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       20 2023-04-26 13:45:04.000000 classconfig-1.0.2/requirements.txt
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)       38 2023-05-03 08:15:34.227396 classconfig-1.0.2/setup.cfg
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     1115 2023-05-03 08:15:02.000000 classconfig-1.0.2/setup.py
+drwxrwxr-x   0 windionleaf  (1000) windionleaf  (1000)        0 2023-05-03 08:15:34.227396 classconfig-1.0.2/tests/
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2626 2023-04-27 11:14:46.000000 classconfig-1.0.2/tests/test_classes.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)    23630 2023-04-26 15:10:49.000000 classconfig-1.0.2/tests/test_configurable.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     1948 2023-04-27 10:43:21.000000 classconfig-1.0.2/tests/test_readme.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     2521 2023-04-27 11:32:32.000000 classconfig-1.0.2/tests/test_transforms.py
+-rw-rw-r--   0 windionleaf  (1000) windionleaf  (1000)     5872 2023-04-27 11:12:58.000000 classconfig-1.0.2/tests/test_validators.py
```

### Comparing `classconfig-1.0.1/LICENSE` & `classconfig-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.1/PKG-INFO` & `classconfig-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classconfig
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package for creating configuration files automatically and loading objects from those configuration files.
 Home-page: https://github.com/mdocekal/classconfig
 Author: Martin Dočekal
 Keywords: configuration,auto config,config,configurable,configurable class,configurable object,configurable attribute
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `classconfig-1.0.1/README.md` & `classconfig-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.1/classconfig/base.py` & `classconfig-1.0.2/classconfig/base.py`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.1/classconfig/classes.py` & `classconfig-1.0.2/classconfig/classes.py`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.1/classconfig/configurable.py` & `classconfig-1.0.2/classconfig/configurable.py`

 * *Files 0% similar despite different names*

```diff
@@ -607,32 +607,34 @@
         if res is None:
             return for_update
 
         res.update(for_update)
 
         return res
 
-    def load(self, path_to: Optional[str] = None) -> LoadedConfig[str, Any]:
+    def load(self, path_to: Optional[str] = None, use_program_arguments: bool = True) -> LoadedConfig[str, Any]:
         """
         Loads configuration from file and arguments.
 
         :param path_to: Path to YAML file with configuration.
          if None, then it is loaded from default path
 
          if default path is None, then it tries to load confiuration from default values
+        :param use_program_arguments: true uses program arguments
         :return: loaded configuration
         """
         path_to = path_to if path_to is not None else self.path_to
 
         if path_to is None:
             return self.load_itself()
         
         with open(path_to, "r") as f:
             conf_dict = YAML().load(f)
-            conf_dict.update(self.get_values_from_arguments())
+            if use_program_arguments:
+                conf_dict.update(self.get_values_from_arguments())
             return self.trans_and_val(conf_dict, path_to)
 
     def load_itself(self) -> LoadedConfig[str, Any]:
         """
         Loads configuration from default.
 
         :return: loaded configuration
```

### Comparing `classconfig-1.0.1/classconfig/transforms.py` & `classconfig-1.0.2/classconfig/transforms.py`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.1/classconfig/validators.py` & `classconfig-1.0.2/classconfig/validators.py`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.1/classconfig.egg-info/PKG-INFO` & `classconfig-1.0.2/classconfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classconfig
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package for creating configuration files automatically and loading objects from those configuration files.
 Home-page: https://github.com/mdocekal/classconfig
 Author: Martin Dočekal
 Keywords: configuration,auto config,config,configurable,configurable class,configurable object,configurable attribute
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `classconfig-1.0.1/classconfig.egg-info/SOURCES.txt` & `classconfig-1.0.2/classconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.1/setup.py` & `classconfig-1.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 with open("requirements.txt") as f:
     REQUIREMENTS = [line.strip() for line in f if is_requirement(line)]
 
 
 setup_args = dict(
     name='classconfig',
-    version='1.0.1',
+    version='1.0.2',
     description='Package for creating configuration files automatically and loading objects from those configuration files.',
     long_description_content_type="text/markdown",
     long_description=README,
     packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
     author='Martin Dočekal',
     keywords=['configuration', 'auto config', 'config', 'configurable', 'configurable class', 'configurable object',
               'configurable attribute'],
```

### Comparing `classconfig-1.0.1/tests/test_classes.py` & `classconfig-1.0.2/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.1/tests/test_configurable.py` & `classconfig-1.0.2/tests/test_configurable.py`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.1/tests/test_readme.py` & `classconfig-1.0.2/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.1/tests/test_transforms.py` & `classconfig-1.0.2/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `classconfig-1.0.1/tests/test_validators.py` & `classconfig-1.0.2/tests/test_validators.py`

 * *Files identical despite different names*

