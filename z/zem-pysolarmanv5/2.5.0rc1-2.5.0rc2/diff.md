# Comparing `tmp/zem-pysolarmanv5-2.5.0rc1.tar.gz` & `tmp/zem-pysolarmanv5-2.5.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zem-pysolarmanv5-2.5.0rc1.tar", last modified: Wed May  3 21:03:32 2023, max compression
+gzip compressed data, was "zem-pysolarmanv5-2.5.0rc2.tar", last modified: Wed May  3 21:55:17 2023, max compression
```

## Comparing `zem-pysolarmanv5-2.5.0rc1.tar` & `zem-pysolarmanv5-2.5.0rc2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 21:03:32.454043 zem-pysolarmanv5-2.5.0rc1/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1083 2023-03-17 18:38:26.000000 zem-pysolarmanv5-2.5.0rc1/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4065 2023-05-03 21:03:32.454043 zem-pysolarmanv5-2.5.0rc1/PKG-INFO
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3251 2023-05-02 20:38:45.000000 zem-pysolarmanv5-2.5.0rc1/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1032 2023-05-03 21:03:21.000000 zem-pysolarmanv5-2.5.0rc1/pyproject.toml
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 21:03:32.454043 zem-pysolarmanv5-2.5.0rc1/pysolarmanv5/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      339 2023-03-22 17:00:26.000000 zem-pysolarmanv5-2.5.0rc1/pysolarmanv5/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    25142 2023-05-02 20:38:45.000000 zem-pysolarmanv5-2.5.0rc1/pysolarmanv5/pysolarmanv5.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    16912 2023-04-02 12:12:49.000000 zem-pysolarmanv5-2.5.0rc1/pysolarmanv5/pysolarmanv5_async.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-03 21:03:32.454043 zem-pysolarmanv5-2.5.0rc1/setup.cfg
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 21:03:32.454043 zem-pysolarmanv5-2.5.0rc1/zem_pysolarmanv5.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4065 2023-05-03 21:03:32.000000 zem-pysolarmanv5-2.5.0rc1/zem_pysolarmanv5.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      330 2023-05-03 21:03:32.000000 zem-pysolarmanv5-2.5.0rc1/zem_pysolarmanv5.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-03 21:03:32.000000 zem-pysolarmanv5-2.5.0rc1/zem_pysolarmanv5.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-05-03 21:03:32.000000 zem-pysolarmanv5-2.5.0rc1/zem_pysolarmanv5.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       13 2023-05-03 21:03:32.000000 zem-pysolarmanv5-2.5.0rc1/zem_pysolarmanv5.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 21:55:17.405710 zem-pysolarmanv5-2.5.0rc2/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1083 2023-03-17 18:38:26.000000 zem-pysolarmanv5-2.5.0rc2/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4229 2023-05-03 21:55:17.405710 zem-pysolarmanv5-2.5.0rc2/PKG-INFO
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3415 2023-05-03 21:07:15.000000 zem-pysolarmanv5-2.5.0rc2/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1032 2023-05-03 21:53:47.000000 zem-pysolarmanv5-2.5.0rc2/pyproject.toml
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 21:55:17.405710 zem-pysolarmanv5-2.5.0rc2/pysolarmanv5/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      339 2023-03-22 17:00:26.000000 zem-pysolarmanv5-2.5.0rc2/pysolarmanv5/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    25142 2023-05-03 21:52:45.000000 zem-pysolarmanv5-2.5.0rc2/pysolarmanv5/pysolarmanv5.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    16874 2023-05-03 21:53:15.000000 zem-pysolarmanv5-2.5.0rc2/pysolarmanv5/pysolarmanv5_async.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-03 21:55:17.405710 zem-pysolarmanv5-2.5.0rc2/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 21:55:17.405710 zem-pysolarmanv5-2.5.0rc2/zem_pysolarmanv5.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4229 2023-05-03 21:55:17.000000 zem-pysolarmanv5-2.5.0rc2/zem_pysolarmanv5.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      330 2023-05-03 21:55:17.000000 zem-pysolarmanv5-2.5.0rc2/zem_pysolarmanv5.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-03 21:55:17.000000 zem-pysolarmanv5-2.5.0rc2/zem_pysolarmanv5.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-05-03 21:55:17.000000 zem-pysolarmanv5-2.5.0rc2/zem_pysolarmanv5.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       13 2023-05-03 21:55:17.000000 zem-pysolarmanv5-2.5.0rc2/zem_pysolarmanv5.egg-info/top_level.txt
```

### Comparing `zem-pysolarmanv5-2.5.0rc1/LICENSE` & `zem-pysolarmanv5-2.5.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `zem-pysolarmanv5-2.5.0rc1/PKG-INFO` & `zem-pysolarmanv5-2.5.0rc2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zem-pysolarmanv5
-Version: 2.5.0rc1
+Version: 2.5.0rc2
 Summary: A Python library for interacting with Solarman (IGEN-Tech) v5 based Solar Data Loggers
 Author-email: Jonathan McCrohan <jmccrohan@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/jmccrohan/pysolarmanv5
 Project-URL: repository, https://github.com/jmccrohan/pysolarmanv5
 Project-URL: documentation, https://pysolarmanv5.readthedocs.io/
 Project-URL: changelog, https://pysolarmanv5.readthedocs.io/en/latest/changelog.html
@@ -13,14 +13,16 @@
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
+*Note:* This project is a placeholder for unreleased versions of the upstream project. Please see https://pypi.org/project/pysolarmanv5/ for the upstream project.
+
 # pysolarmanv5
 
 This is a Python module to interact with Solarman (IGEN-Tech) v5 based solar
 inverter data loggers. Modbus RTU frames can be encapsulated in the proprietary
 Solarman v5 protocol and requests sent to the data logger on port tcp/8899.
 
 This module aims to simplify the Solarman v5 protocol, exposing interfaces
```

### Comparing `zem-pysolarmanv5-2.5.0rc1/README.md` & `zem-pysolarmanv5-2.5.0rc2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+*Note:* This project is a placeholder for unreleased versions of the upstream project. Please see https://pypi.org/project/pysolarmanv5/ for the upstream project.
+
 # pysolarmanv5
 
 This is a Python module to interact with Solarman (IGEN-Tech) v5 based solar
 inverter data loggers. Modbus RTU frames can be encapsulated in the proprietary
 Solarman v5 protocol and requests sent to the data logger on port tcp/8899.
 
 This module aims to simplify the Solarman v5 protocol, exposing interfaces
```

### Comparing `zem-pysolarmanv5-2.5.0rc1/pyproject.toml` & `zem-pysolarmanv5-2.5.0rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "zem-pysolarmanv5"
-version = "2.5.0.rc1"
+version = "2.5.0.rc2"
 description = "A Python library for interacting with Solarman (IGEN-Tech) v5 based Solar Data Loggers"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 authors = [{name = "Jonathan McCrohan", email = "jmccrohan@gmail.com"}]
 keywords = ["solarman", "igen-tech", "modbus", "solar", "inverter", "solarmanv5"]
 classifiers = [
```

### Comparing `zem-pysolarmanv5-2.5.0rc1/pysolarmanv5/pysolarmanv5.py` & `zem-pysolarmanv5-2.5.0rc2/pysolarmanv5/pysolarmanv5.py`

 * *Files identical despite different names*

### Comparing `zem-pysolarmanv5-2.5.0rc1/pysolarmanv5/pysolarmanv5_async.py` & `zem-pysolarmanv5-2.5.0rc2/pysolarmanv5/pysolarmanv5_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 
     See :doc:`examples` directory for further examples.
 
     """
 
     def __init__(self, address, serial, **kwargs):
         """Constructor"""
-        kwargs.update({'socket': ''})
         super(PySolarmanV5Async, self).__init__(address, serial, **kwargs)
         self._needs_reconnect = kwargs.get("auto_reconnect", False)
         """ Auto-reconnect feature """
         self.reader: asyncio.StreamReader = None  # noqa
         self.writer: asyncio.StreamWriter = None  # noqa
         self.data_queue = asyncio.Queue(maxsize=1)
         self.data_wanted_ev = Event()
```

### Comparing `zem-pysolarmanv5-2.5.0rc1/zem_pysolarmanv5.egg-info/PKG-INFO` & `zem-pysolarmanv5-2.5.0rc2/zem_pysolarmanv5.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zem-pysolarmanv5
-Version: 2.5.0rc1
+Version: 2.5.0rc2
 Summary: A Python library for interacting with Solarman (IGEN-Tech) v5 based Solar Data Loggers
 Author-email: Jonathan McCrohan <jmccrohan@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/jmccrohan/pysolarmanv5
 Project-URL: repository, https://github.com/jmccrohan/pysolarmanv5
 Project-URL: documentation, https://pysolarmanv5.readthedocs.io/
 Project-URL: changelog, https://pysolarmanv5.readthedocs.io/en/latest/changelog.html
@@ -13,14 +13,16 @@
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
+*Note:* This project is a placeholder for unreleased versions of the upstream project. Please see https://pypi.org/project/pysolarmanv5/ for the upstream project.
+
 # pysolarmanv5
 
 This is a Python module to interact with Solarman (IGEN-Tech) v5 based solar
 inverter data loggers. Modbus RTU frames can be encapsulated in the proprietary
 Solarman v5 protocol and requests sent to the data logger on port tcp/8899.
 
 This module aims to simplify the Solarman v5 protocol, exposing interfaces
```

