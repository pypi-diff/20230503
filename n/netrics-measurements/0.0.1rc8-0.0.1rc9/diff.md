# Comparing `tmp/netrics_measurements-0.0.1rc8.tar.gz` & `tmp/netrics_measurements-0.0.1rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netrics_measurements-0.0.1rc8.tar", max compression
+gzip compressed data, was "netrics_measurements-0.0.1rc9.tar", max compression
```

## Comparing `netrics_measurements-0.0.1rc8.tar` & `netrics_measurements-0.0.1rc9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1362 2023-04-12 18:18:47.149885 netrics_measurements-0.0.1rc8/pyproject.toml
--rw-r--r--   0        0        0       62 2023-01-25 22:59:21.061389 netrics_measurements-0.0.1rc8/src/netrics/__init__.py
--rw-r--r--   0        0        0     1232 2023-02-15 20:41:58.536404 netrics_measurements-0.0.1rc8/src/netrics/__main__.py
--rw-r--r--   0        0        0      199 2023-01-25 22:59:21.061389 netrics_measurements-0.0.1rc8/src/netrics/cli/include/banner/doom
--rw-r--r--   0        0        0        0 2023-02-28 18:00:07.862862 netrics_measurements-0.0.1rc8/src/netrics/conf/include/defaults.yaml
--rw-r--r--   0        0        0     1549 2023-04-12 18:16:17.266926 netrics_measurements-0.0.1rc8/src/netrics/conf/include/measurements.yaml
--rw-r--r--   0        0        0        0 2023-01-17 22:42:48.980256 netrics_measurements-0.0.1rc8/src/netrics/measurement/__init__.py
--rw-r--r--   0        0        0      202 2023-03-08 19:45:00.221723 netrics_measurements-0.0.1rc8/src/netrics/measurement/common/__init__.py
--rw-r--r--   0        0        0      243 2023-03-02 20:41:16.518278 netrics_measurements-0.0.1rc8/src/netrics/measurement/common/connectivity/__init__.py
--rw-r--r--   0        0        0     2643 2023-01-25 22:59:21.061389 netrics_measurements-0.0.1rc8/src/netrics/measurement/common/connectivity/command.py
--rw-r--r--   0        0        0     7857 2023-04-05 20:20:57.974126 netrics_measurements-0.0.1rc8/src/netrics/measurement/common/connectivity/decorator.py
--rw-r--r--   0        0        0       93 2023-03-08 19:45:00.221723 netrics_measurements-0.0.1rc8/src/netrics/measurement/common/connectivity/default.py
--rw-r--r--   0        0        0     1093 2023-03-02 20:41:16.518278 netrics_measurements-0.0.1rc8/src/netrics/measurement/common/connectivity/output.py
--rw-r--r--   0        0        0     2004 2023-02-28 21:19:35.997221 netrics_measurements-0.0.1rc8/src/netrics/measurement/common/dns.py
--rw-r--r--   0        0        0     1357 2023-04-12 18:16:17.266926 netrics_measurements-0.0.1rc8/src/netrics/measurement/common/executable.py
--rw-r--r--   0        0        0     6548 2023-04-12 18:16:17.266926 netrics_measurements-0.0.1rc8/src/netrics/measurement/dev.py
--rw-r--r--   0        0        0     4898 2023-04-05 20:22:22.737595 netrics_measurements-0.0.1rc8/src/netrics/measurement/dns_latency.py
--rw-r--r--   0        0        0     6333 2023-04-05 20:22:22.737595 netrics_measurements-0.0.1rc8/src/netrics/measurement/hops.py
--rw-r--r--   0        0        0     4936 2023-04-05 20:22:22.737595 netrics_measurements-0.0.1rc8/src/netrics/measurement/hops_traceroute.py
--rw-r--r--   0        0        0     2010 2023-04-05 20:22:22.737595 netrics_measurements-0.0.1rc8/src/netrics/measurement/ip.py
--rw-r--r--   0        0        0     7509 2023-03-08 19:45:00.221723 netrics_measurements-0.0.1rc8/src/netrics/measurement/lml.py
--rw-r--r--   0        0        0     9766 2023-03-08 19:45:00.221723 netrics_measurements-0.0.1rc8/src/netrics/measurement/lml_traceroute.py
--rw-r--r--   0        0        0       63 2023-01-17 22:42:48.980256 netrics_measurements-0.0.1rc8/src/netrics/measurement/ndt7.py
--rw-r--r--   0        0        0      212 2023-01-17 22:42:48.980256 netrics_measurements-0.0.1rc8/src/netrics/measurement/ookla.py
--rw-r--r--   0        0        0     4743 2023-04-05 20:22:22.737595 netrics_measurements-0.0.1rc8/src/netrics/measurement/ping.py
--rw-r--r--   0        0        0      158 2023-04-12 18:16:17.266926 netrics_measurements-0.0.1rc8/src/netrics/task/__init__.py
--rw-r--r--   0        0        0     1513 2023-02-28 21:19:35.997221 netrics_measurements-0.0.1rc8/src/netrics/task/param.py
--rw-r--r--   0        0        0      650 2023-02-28 21:19:35.997221 netrics_measurements-0.0.1rc8/src/netrics/task/result.py
--rw-r--r--   0        0        0     6629 2023-04-05 20:22:22.737595 netrics_measurements-0.0.1rc8/src/netrics/task/schema.py
--rw-r--r--   0        0        0      184 2023-01-25 22:59:21.061389 netrics_measurements-0.0.1rc8/src/netrics/task/sysexit.py
--rw-r--r--   0        0        0        0 2023-02-28 21:19:35.997221 netrics_measurements-0.0.1rc8/src/netrics/util/__init__.py
--rw-r--r--   0        0        0      991 2023-04-05 20:22:22.737595 netrics_measurements-0.0.1rc8/src/netrics/util/iterutils.py
--rw-r--r--   0        0        0     1835 2023-04-05 20:22:22.737595 netrics_measurements-0.0.1rc8/src/netrics/util/lazy_validation.py
--rw-r--r--   0        0        0      960 2023-04-05 20:22:22.737595 netrics_measurements-0.0.1rc8/src/netrics/util/procutils.py
--rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 netrics_measurements-0.0.1rc8/PKG-INFO
+-rw-r--r--   0        0        0     1362 2023-04-20 17:00:10.816850 netrics_measurements-0.0.1rc9/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-04-13 16:37:58.704133 netrics_measurements-0.0.1rc9/src/netrics/__init__.py
+-rw-r--r--   0        0        0     1232 2023-04-13 16:37:58.704133 netrics_measurements-0.0.1rc9/src/netrics/__main__.py
+-rw-r--r--   0        0        0      199 2023-04-13 16:37:58.704133 netrics_measurements-0.0.1rc9/src/netrics/cli/include/banner/doom
+-rw-r--r--   0        0        0        0 2023-04-13 16:37:58.704133 netrics_measurements-0.0.1rc9/src/netrics/conf/include/defaults.yaml
+-rw-r--r--   0        0        0     1549 2023-04-20 16:48:07.813378 netrics_measurements-0.0.1rc9/src/netrics/conf/include/measurements.yaml
+-rw-r--r--   0        0        0        0 2023-01-17 22:42:48.980256 netrics_measurements-0.0.1rc9/src/netrics/measurement/__init__.py
+-rw-r--r--   0        0        0      202 2023-04-13 16:37:58.704133 netrics_measurements-0.0.1rc9/src/netrics/measurement/common/__init__.py
+-rw-r--r--   0        0        0      243 2023-04-13 16:37:58.704133 netrics_measurements-0.0.1rc9/src/netrics/measurement/common/connectivity/__init__.py
+-rw-r--r--   0        0        0     2643 2023-04-13 16:37:58.704133 netrics_measurements-0.0.1rc9/src/netrics/measurement/common/connectivity/command.py
+-rw-r--r--   0        0        0     7857 2023-04-13 16:37:58.704133 netrics_measurements-0.0.1rc9/src/netrics/measurement/common/connectivity/decorator.py
+-rw-r--r--   0        0        0       93 2023-04-13 16:37:58.704133 netrics_measurements-0.0.1rc9/src/netrics/measurement/common/connectivity/default.py
+-rw-r--r--   0        0        0     1093 2023-04-13 16:37:58.704133 netrics_measurements-0.0.1rc9/src/netrics/measurement/common/connectivity/output.py
+-rw-r--r--   0        0        0     2004 2023-04-13 16:37:58.704133 netrics_measurements-0.0.1rc9/src/netrics/measurement/common/dns.py
+-rw-r--r--   0        0        0     1357 2023-04-13 16:37:58.704133 netrics_measurements-0.0.1rc9/src/netrics/measurement/common/executable.py
+-rw-r--r--   0        0        0     6548 2023-04-13 16:37:58.704133 netrics_measurements-0.0.1rc9/src/netrics/measurement/dev.py
+-rw-r--r--   0        0        0     4898 2023-04-13 16:37:58.704133 netrics_measurements-0.0.1rc9/src/netrics/measurement/dns_latency.py
+-rw-r--r--   0        0        0     6333 2023-04-13 16:37:58.704133 netrics_measurements-0.0.1rc9/src/netrics/measurement/hops.py
+-rw-r--r--   0        0        0     4936 2023-04-13 16:37:58.704133 netrics_measurements-0.0.1rc9/src/netrics/measurement/hops_traceroute.py
+-rw-r--r--   0        0        0     2010 2023-04-13 16:37:58.704133 netrics_measurements-0.0.1rc9/src/netrics/measurement/ip.py
+-rw-r--r--   0        0        0     7509 2023-04-13 16:37:58.704133 netrics_measurements-0.0.1rc9/src/netrics/measurement/lml.py
+-rw-r--r--   0        0        0     9766 2023-04-20 16:48:07.813378 netrics_measurements-0.0.1rc9/src/netrics/measurement/lml_traceroute.py
+-rw-r--r--   0        0        0       63 2023-01-17 22:42:48.980256 netrics_measurements-0.0.1rc9/src/netrics/measurement/ndt7.py
+-rw-r--r--   0        0        0      212 2023-04-20 16:49:21.432917 netrics_measurements-0.0.1rc9/src/netrics/measurement/ookla.py
+-rw-r--r--   0        0        0     4743 2023-04-20 16:48:07.813378 netrics_measurements-0.0.1rc9/src/netrics/measurement/ping.py
+-rw-r--r--   0        0        0      158 2023-04-13 16:37:58.704133 netrics_measurements-0.0.1rc9/src/netrics/task/__init__.py
+-rw-r--r--   0        0        0     1513 2023-04-13 16:37:58.704133 netrics_measurements-0.0.1rc9/src/netrics/task/param.py
+-rw-r--r--   0        0        0      678 2023-04-20 16:56:20.310295 netrics_measurements-0.0.1rc9/src/netrics/task/result.py
+-rw-r--r--   0        0        0     6629 2023-04-20 16:48:07.813378 netrics_measurements-0.0.1rc9/src/netrics/task/schema.py
+-rw-r--r--   0        0        0      184 2023-04-20 16:48:07.813378 netrics_measurements-0.0.1rc9/src/netrics/task/sysexit.py
+-rw-r--r--   0        0        0        0 2023-04-13 16:37:58.708133 netrics_measurements-0.0.1rc9/src/netrics/util/__init__.py
+-rw-r--r--   0        0        0      991 2023-04-13 16:37:58.708133 netrics_measurements-0.0.1rc9/src/netrics/util/iterutils.py
+-rw-r--r--   0        0        0     1835 2023-04-13 16:37:58.708133 netrics_measurements-0.0.1rc9/src/netrics/util/lazy_validation.py
+-rw-r--r--   0        0        0      960 2023-04-13 16:37:58.708133 netrics_measurements-0.0.1rc9/src/netrics/util/procutils.py
+-rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 netrics_measurements-0.0.1rc9/PKG-INFO
```

### Comparing `netrics_measurements-0.0.1rc8/pyproject.toml` & `netrics_measurements-0.0.1rc9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "netrics-measurements"
-version = "0.0.1-rc.8"
+version = "0.0.1-rc.9"
 description = "The extensible network measurements framework"
 license = "MIT"
 authors = [
   "Jesse London <jesselondon@gmail.com>",
   "Kyle MacMillan <macmillan@uchicago.edu>",
 ]
 packages = [{include = "netrics", from = "src"}]
```

### Comparing `netrics_measurements-0.0.1rc8/src/netrics/__main__.py` & `netrics_measurements-0.0.1rc9/src/netrics/__main__.py`

 * *Files identical despite different names*

### Comparing `netrics_measurements-0.0.1rc8/src/netrics/conf/include/measurements.yaml` & `netrics_measurements-0.0.1rc9/src/netrics/conf/include/measurements.yaml`

 * *Files identical despite different names*

### Comparing `netrics_measurements-0.0.1rc8/src/netrics/measurement/common/connectivity/command.py` & `netrics_measurements-0.0.1rc9/src/netrics/measurement/common/connectivity/command.py`

 * *Files identical despite different names*

### Comparing `netrics_measurements-0.0.1rc8/src/netrics/measurement/common/connectivity/decorator.py` & `netrics_measurements-0.0.1rc9/src/netrics/measurement/common/connectivity/decorator.py`

 * *Files identical despite different names*

### Comparing `netrics_measurements-0.0.1rc8/src/netrics/measurement/common/connectivity/output.py` & `netrics_measurements-0.0.1rc9/src/netrics/measurement/common/connectivity/output.py`

 * *Files identical despite different names*

### Comparing `netrics_measurements-0.0.1rc8/src/netrics/measurement/common/dns.py` & `netrics_measurements-0.0.1rc9/src/netrics/measurement/common/dns.py`

 * *Files identical despite different names*

### Comparing `netrics_measurements-0.0.1rc8/src/netrics/measurement/common/executable.py` & `netrics_measurements-0.0.1rc9/src/netrics/measurement/common/executable.py`

 * *Files identical despite different names*

### Comparing `netrics_measurements-0.0.1rc8/src/netrics/measurement/dev.py` & `netrics_measurements-0.0.1rc9/src/netrics/measurement/dev.py`

 * *Files identical despite different names*

### Comparing `netrics_measurements-0.0.1rc8/src/netrics/measurement/dns_latency.py` & `netrics_measurements-0.0.1rc9/src/netrics/measurement/dns_latency.py`

 * *Files identical despite different names*

### Comparing `netrics_measurements-0.0.1rc8/src/netrics/measurement/hops.py` & `netrics_measurements-0.0.1rc9/src/netrics/measurement/hops.py`

 * *Files identical despite different names*

### Comparing `netrics_measurements-0.0.1rc8/src/netrics/measurement/hops_traceroute.py` & `netrics_measurements-0.0.1rc9/src/netrics/measurement/hops_traceroute.py`

 * *Files identical despite different names*

### Comparing `netrics_measurements-0.0.1rc8/src/netrics/measurement/ip.py` & `netrics_measurements-0.0.1rc9/src/netrics/measurement/ip.py`

 * *Files identical despite different names*

### Comparing `netrics_measurements-0.0.1rc8/src/netrics/measurement/lml.py` & `netrics_measurements-0.0.1rc9/src/netrics/measurement/lml.py`

 * *Files identical despite different names*

### Comparing `netrics_measurements-0.0.1rc8/src/netrics/measurement/lml_traceroute.py` & `netrics_measurements-0.0.1rc9/src/netrics/measurement/lml_traceroute.py`

 * *Files identical despite different names*

### Comparing `netrics_measurements-0.0.1rc8/src/netrics/measurement/ping.py` & `netrics_measurements-0.0.1rc9/src/netrics/measurement/ping.py`

 * *Files identical despite different names*

### Comparing `netrics_measurements-0.0.1rc8/src/netrics/task/param.py` & `netrics_measurements-0.0.1rc9/src/netrics/task/param.py`

 * *Files identical despite different names*

### Comparing `netrics_measurements-0.0.1rc8/src/netrics/task/result.py` & `netrics_measurements-0.0.1rc9/src/netrics/task/result.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,11 +17,12 @@
         results = {label: results}
 
     if annotate:
         results = {
             'Measurements': results,
             'Meta': {
                 'Time': time.time(),
+                'Id': None,
             },
         }
 
     return fate.task.result.write(results, **kwargs)
```

### Comparing `netrics_measurements-0.0.1rc8/src/netrics/task/schema.py` & `netrics_measurements-0.0.1rc9/src/netrics/task/schema.py`

 * *Files identical despite different names*

### Comparing `netrics_measurements-0.0.1rc8/src/netrics/util/iterutils.py` & `netrics_measurements-0.0.1rc9/src/netrics/util/iterutils.py`

 * *Files identical despite different names*

### Comparing `netrics_measurements-0.0.1rc8/src/netrics/util/lazy_validation.py` & `netrics_measurements-0.0.1rc9/src/netrics/util/lazy_validation.py`

 * *Files identical despite different names*

### Comparing `netrics_measurements-0.0.1rc8/src/netrics/util/procutils.py` & `netrics_measurements-0.0.1rc9/src/netrics/util/procutils.py`

 * *Files identical despite different names*

### Comparing `netrics_measurements-0.0.1rc8/PKG-INFO` & `netrics_measurements-0.0.1rc9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netrics-measurements
-Version: 0.0.1rc8
+Version: 0.0.1rc9
 Summary: The extensible network measurements framework
 License: MIT
 Author: Jesse London
 Author-email: jesselondon@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

