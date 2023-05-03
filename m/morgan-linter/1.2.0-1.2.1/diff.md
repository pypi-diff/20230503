# Comparing `tmp/morgan_linter-1.2.0.tar.gz` & `tmp/morgan_linter-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morgan_linter-1.2.0.tar", max compression
+gzip compressed data, was "morgan_linter-1.2.1.tar", max compression
```

## Comparing `morgan_linter-1.2.0.tar` & `morgan_linter-1.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2022-11-12 04:07:08.230015 morgan_linter-1.2.0/LICENSE
--rw-r--r--   0        0        0       82 2022-11-11 19:34:46.478633 morgan_linter-1.2.0/README.md
--rw-r--r--   0        0        0     1052 2022-11-12 04:52:18.755529 morgan_linter-1.2.0/morgan_linter/__init__.py
--rw-r--r--   0        0        0       23 2022-11-12 04:46:33.506832 morgan_linter-1.2.0/morgan_linter/__main__.py
--rw-r--r--   0        0        0     3595 2022-11-11 19:15:23.226035 morgan_linter-1.2.0/morgan_linter/base_linter.py
--rw-r--r--   0        0        0     1096 2022-11-12 04:51:02.677813 morgan_linter-1.2.0/morgan_linter/custom_linter.py
--rw-r--r--   0        0        0     8511 2022-12-28 22:13:40.170560 morgan_linter-1.2.0/morgan_linter/google_checks.py
--rw-r--r--   0        0        0     2356 2022-11-10 16:48:40.351547 morgan_linter-1.2.0/morgan_linter/utils.py
--rw-r--r--   0        0        0      474 2023-05-02 20:13:43.487655 morgan_linter-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 morgan_linter-1.2.0/setup.py
--rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 morgan_linter-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-11-12 04:07:08.230015 morgan_linter-1.2.1/LICENSE
+-rw-r--r--   0        0        0       82 2022-11-11 19:34:46.478633 morgan_linter-1.2.1/README.md
+-rw-r--r--   0        0        0     1052 2022-11-12 04:52:18.755529 morgan_linter-1.2.1/morgan_linter/__init__.py
+-rw-r--r--   0        0        0       23 2022-11-12 04:46:33.506832 morgan_linter-1.2.1/morgan_linter/__main__.py
+-rw-r--r--   0        0        0     3595 2022-11-11 19:15:23.226035 morgan_linter-1.2.1/morgan_linter/base_linter.py
+-rw-r--r--   0        0        0     1096 2022-11-12 04:51:02.677813 morgan_linter-1.2.1/morgan_linter/custom_linter.py
+-rw-r--r--   0        0        0     8513 2023-05-03 20:08:15.335065 morgan_linter-1.2.1/morgan_linter/google_checks.py
+-rw-r--r--   0        0        0     2356 2022-11-10 16:48:40.351547 morgan_linter-1.2.1/morgan_linter/utils.py
+-rw-r--r--   0        0        0      474 2023-05-03 20:10:00.540312 morgan_linter-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 morgan_linter-1.2.1/setup.py
+-rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 morgan_linter-1.2.1/PKG-INFO
```

### Comparing `morgan_linter-1.2.0/LICENSE` & `morgan_linter-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `morgan_linter-1.2.0/morgan_linter/__init__.py` & `morgan_linter-1.2.1/morgan_linter/__init__.py`

 * *Files identical despite different names*

### Comparing `morgan_linter-1.2.0/morgan_linter/base_linter.py` & `morgan_linter-1.2.1/morgan_linter/base_linter.py`

 * *Files identical despite different names*

### Comparing `morgan_linter-1.2.0/morgan_linter/custom_linter.py` & `morgan_linter-1.2.1/morgan_linter/custom_linter.py`

 * *Files identical despite different names*

### Comparing `morgan_linter-1.2.0/morgan_linter/google_checks.py` & `morgan_linter-1.2.1/morgan_linter/google_checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,16 +168,16 @@
         """
         The function checks if the documentation about the arguments is up to date.
         
         Args:
           
           - node (ast): the node of the function
         """
-        import pdb
-        pdb.set_trace()
+        #import pdb
+        #pdb.set_trace()
         is_args_section = self._check_section(section = "Args:")
         is_return_section = self._check_section(section = "Returns:")
 
         if is_args_section:            
             args_section = self._get_args_section(is_return_section = is_return_section)
                                     
             #Check if the documentation about the arguments is up to date
```

### Comparing `morgan_linter-1.2.0/morgan_linter/utils.py` & `morgan_linter-1.2.1/morgan_linter/utils.py`

 * *Files identical despite different names*

### Comparing `morgan_linter-1.2.0/setup.py` & `morgan_linter-1.2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 entry_points = \
 {'console_scripts': ['morgan = morgan_linter:cli']}
 
 setup_kwargs = {
     'name': 'morgan-linter',
-    'version': '1.2.0',
+    'version': '1.2.1',
     'description': 'Linter to validate google docstrings',
     'long_description': '# morgan-linter\nLinter to verify the google docstrings format in a python project\n',
     'author': 'Edwar Girón',
     'author_email': 'contactoedwargiron@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `morgan_linter-1.2.0/PKG-INFO` & `morgan_linter-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morgan-linter
-Version: 1.2.0
+Version: 1.2.1
 Summary: Linter to validate google docstrings
 Author: Edwar Girón
 Author-email: contactoedwargiron@gmail.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

