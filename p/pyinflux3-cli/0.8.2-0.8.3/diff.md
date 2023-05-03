# Comparing `tmp/pyinflux3-cli-0.8.2.tar.gz` & `tmp/pyinflux3-cli-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinflux3-cli-0.8.2.tar", last modified: Mon Apr 17 16:12:39 2023, max compression
+gzip compressed data, was "pyinflux3-cli-0.8.3.tar", last modified: Wed May  3 14:06:58 2023, max compression
```

## Comparing `pyinflux3-cli-0.8.2.tar` & `pyinflux3-cli-0.8.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:12:39.189639 pyinflux3-cli-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-17 16:12:39.189639 pyinflux3-cli-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-17 16:12:31.000000 pyinflux3-cli-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:12:39.189639 pyinflux3-cli-0.8.2/influxdb_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:12:31.000000 pyinflux3-cli-0.8.2/influxdb_cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7626 2023-04-17 16:12:31.000000 pyinflux3-cli-0.8.2/influxdb_cli/influx3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:12:39.189639 pyinflux3-cli-0.8.2/pyinflux3_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-17 16:12:39.000000 pyinflux3-cli-0.8.2/pyinflux3_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-17 16:12:39.000000 pyinflux3-cli-0.8.2/pyinflux3_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 16:12:39.000000 pyinflux3-cli-0.8.2/pyinflux3_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-17 16:12:39.000000 pyinflux3-cli-0.8.2/pyinflux3_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-17 16:12:39.000000 pyinflux3-cli-0.8.2/pyinflux3_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-17 16:12:39.000000 pyinflux3-cli-0.8.2/pyinflux3_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-17 16:12:31.000000 pyinflux3-cli-0.8.2/setup-cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 16:12:39.189639 pyinflux3-cli-0.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:06:58.796858 pyinflux3-cli-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-03 14:06:58.796858 pyinflux3-cli-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-03 14:06:52.000000 pyinflux3-cli-0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:06:58.796858 pyinflux3-cli-0.8.3/influxdb_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:06:52.000000 pyinflux3-cli-0.8.3/influxdb_cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7626 2023-05-03 14:06:52.000000 pyinflux3-cli-0.8.3/influxdb_cli/influx3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:06:58.796858 pyinflux3-cli-0.8.3/pyinflux3_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-03 14:06:58.000000 pyinflux3-cli-0.8.3/pyinflux3_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-03 14:06:58.000000 pyinflux3-cli-0.8.3/pyinflux3_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 14:06:58.000000 pyinflux3-cli-0.8.3/pyinflux3_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 14:06:58.000000 pyinflux3-cli-0.8.3/pyinflux3_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-03 14:06:58.000000 pyinflux3-cli-0.8.3/pyinflux3_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 14:06:58.000000 pyinflux3-cli-0.8.3/pyinflux3_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-03 14:06:52.000000 pyinflux3-cli-0.8.3/setup-cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 14:06:58.796858 pyinflux3-cli-0.8.3/setup.cfg
```

### Comparing `pyinflux3-cli-0.8.2/PKG-INFO` & `pyinflux3-cli-0.8.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3-cli
-Version: 0.8.2
+Version: 0.8.3
 Summary: Community Python client for InfluxDB IOx (CLI)
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -97,7 +97,20 @@
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

### Comparing `pyinflux3-cli-0.8.2/README.md` & `pyinflux3-cli-0.8.3/README.md`

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

### Comparing `pyinflux3-cli-0.8.2/influxdb_cli/influx3.py` & `pyinflux3-cli-0.8.3/influxdb_cli/influx3.py`

 * *Files identical despite different names*

### Comparing `pyinflux3-cli-0.8.2/pyinflux3_cli.egg-info/PKG-INFO` & `pyinflux3-cli-0.8.3/pyinflux3_cli.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3-cli
-Version: 0.8.2
+Version: 0.8.3
 Summary: Community Python client for InfluxDB IOx (CLI)
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -97,7 +97,20 @@
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

### Comparing `pyinflux3-cli-0.8.2/setup-cli.py` & `pyinflux3-cli-0.8.3/setup-cli.py`

 * *Files identical despite different names*

