# Comparing `tmp/pyinflux3-0.8.2.tar.gz` & `tmp/pyinflux3-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinflux3-0.8.2.tar", last modified: Mon Apr 17 16:12:35 2023, max compression
+gzip compressed data, was "pyinflux3-0.8.3.tar", last modified: Wed May  3 14:06:51 2023, max compression
```

## Comparing `pyinflux3-0.8.2.tar` & `pyinflux3-0.8.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:12:35.945612 pyinflux3-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-04-17 16:12:35.945612 pyinflux3-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-17 16:12:29.000000 pyinflux3-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:12:35.945612 pyinflux3-0.8.2/influxdb_client_3/
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-04-17 16:12:29.000000 pyinflux3-0.8.2/influxdb_client_3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:12:35.945612 pyinflux3-0.8.2/pyinflux3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-04-17 16:12:35.000000 pyinflux3-0.8.2/pyinflux3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-17 16:12:35.000000 pyinflux3-0.8.2/pyinflux3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 16:12:35.000000 pyinflux3-0.8.2/pyinflux3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-17 16:12:35.000000 pyinflux3-0.8.2/pyinflux3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 16:12:35.000000 pyinflux3-0.8.2/pyinflux3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-17 16:12:29.000000 pyinflux3-0.8.2/setup-client.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 16:12:35.945612 pyinflux3-0.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:06:51.899442 pyinflux3-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-03 14:06:51.899442 pyinflux3-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-03 14:06:45.000000 pyinflux3-0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:06:51.899442 pyinflux3-0.8.3/influxdb_client_3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-03 14:06:45.000000 pyinflux3-0.8.3/influxdb_client_3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:06:51.899442 pyinflux3-0.8.3/pyinflux3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-03 14:06:51.000000 pyinflux3-0.8.3/pyinflux3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-03 14:06:51.000000 pyinflux3-0.8.3/pyinflux3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 14:06:51.000000 pyinflux3-0.8.3/pyinflux3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-03 14:06:51.000000 pyinflux3-0.8.3/pyinflux3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-03 14:06:51.000000 pyinflux3-0.8.3/pyinflux3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-03 14:06:45.000000 pyinflux3-0.8.3/setup-client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 14:06:51.899442 pyinflux3-0.8.3/setup.cfg
```

### Comparing `pyinflux3-0.8.2/PKG-INFO` & `pyinflux3-0.8.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.8.2
+Version: 0.8.3
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -98,7 +98,20 @@
 influx3 write_csv --file ./Examples/example.csv --measurement table2 --time Date --tags host,region
 ```
 
 
 # Client library
 This project also includes a new client library that strives for utter simplicity. It includes 3 functions, a constuctor, write(), and read().
 
+# Contribution
+If you are working on a new feature for either the CLI or the Client Libary please make sure you test both for breaking changes. This can currently be achived using the following method:
+```bash
+python3 -m venv .venv
+source .venv/bin/activate
+chmod +x ./test/test-package.sh 
+./test/test-package.sh 
+```
+Any time you make changes in your code and want to retest just run the script again:
+```
+./test/test-package.sh 
+```
+
```

### Comparing `pyinflux3-0.8.2/README.md` & `pyinflux3-0.8.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -79,7 +79,20 @@
 influx3 write_csv --file ./Examples/example.csv --measurement table2 --time Date --tags host,region
 ```
 
 
 # Client library
 This project also includes a new client library that strives for utter simplicity. It includes 3 functions, a constuctor, write(), and read().
 
+# Contribution
+If you are working on a new feature for either the CLI or the Client Libary please make sure you test both for breaking changes. This can currently be achived using the following method:
+```bash
+python3 -m venv .venv
+source .venv/bin/activate
+chmod +x ./test/test-package.sh 
+./test/test-package.sh 
+```
+Any time you make changes in your code and want to retest just run the script again:
+```
+./test/test-package.sh 
+```
+
```

### Comparing `pyinflux3-0.8.2/influxdb_client_3/__init__.py` & `pyinflux3-0.8.3/influxdb_client_3/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinflux3-0.8.2/pyinflux3.egg-info/PKG-INFO` & `pyinflux3-0.8.3/pyinflux3.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3
-Version: 0.8.2
+Version: 0.8.3
 Summary: Community Python client for InfluxDB IOx
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -98,7 +98,20 @@
 influx3 write_csv --file ./Examples/example.csv --measurement table2 --time Date --tags host,region
 ```
 
 
 # Client library
 This project also includes a new client library that strives for utter simplicity. It includes 3 functions, a constuctor, write(), and read().
 
+# Contribution
+If you are working on a new feature for either the CLI or the Client Libary please make sure you test both for breaking changes. This can currently be achived using the following method:
+```bash
+python3 -m venv .venv
+source .venv/bin/activate
+chmod +x ./test/test-package.sh 
+./test/test-package.sh 
+```
+Any time you make changes in your code and want to retest just run the script again:
+```
+./test/test-package.sh 
+```
+
```

### Comparing `pyinflux3-0.8.2/setup-client.py` & `pyinflux3-0.8.3/setup-client.py`

 * *Files identical despite different names*

