# Comparing `tmp/jaaql-monitor-1.2.23.tar.gz` & `tmp/jaaql-monitor-1.2.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.23.tar", last modified: Wed May  3 01:47:38 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.24.tar", last modified: Wed May  3 01:48:00 2023, max compression
```

## Comparing `jaaql-monitor-1.2.23.tar` & `jaaql-monitor-1.2.24.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 01:47:38.809816 jaaql-monitor-1.2.23/
--rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.23/LICENSE.txt
--rw-rw-rw-   0        0        0     1475 2023-05-03 01:47:38.809816 jaaql-monitor-1.2.23/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.23/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 01:47:38.806816 jaaql-monitor-1.2.23/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-05-03 01:47:38.000000 jaaql-monitor-1.2.23/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-03 01:47:38.000000 jaaql-monitor-1.2.23/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 01:47:38.000000 jaaql-monitor-1.2.23/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-03 01:47:38.000000 jaaql-monitor-1.2.23/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-03 01:47:38.000000 jaaql-monitor-1.2.23/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-03 01:47:38.808817 jaaql-monitor-1.2.23/monitor/
--rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.23/monitor/__init__.py
--rw-rw-rw-   0        0        0    23648 2023-05-03 01:47:37.000000 jaaql-monitor-1.2.23/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-05-03 01:47:25.000000 jaaql-monitor-1.2.23/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-05-03 01:47:38.810818 jaaql-monitor-1.2.23/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.23/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:00.982908 jaaql-monitor-1.2.24/
+-rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.24/LICENSE.txt
+-rw-rw-rw-   0        0        0     1475 2023-05-03 01:48:00.982908 jaaql-monitor-1.2.24/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.24/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:00.977905 jaaql-monitor-1.2.24/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1475 2023-05-03 01:48:00.000000 jaaql-monitor-1.2.24/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-03 01:48:00.000000 jaaql-monitor-1.2.24/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 01:48:00.000000 jaaql-monitor-1.2.24/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-03 01:48:00.000000 jaaql-monitor-1.2.24/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-03 01:48:00.000000 jaaql-monitor-1.2.24/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 01:48:00.981905 jaaql-monitor-1.2.24/monitor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.24/monitor/__init__.py
+-rw-rw-rw-   0        0        0    23648 2023-05-03 01:47:37.000000 jaaql-monitor-1.2.24/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-05-03 01:47:45.000000 jaaql-monitor-1.2.24/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-03 01:48:00.983908 jaaql-monitor-1.2.24/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.24/setup.py
```

### Comparing `jaaql-monitor-1.2.23/LICENSE.txt` & `jaaql-monitor-1.2.24/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.23/PKG-INFO` & `jaaql-monitor-1.2.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.23
+Version: 1.2.24
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.23/README.md` & `jaaql-monitor-1.2.24/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.23/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.24/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.23
+Version: 1.2.24
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.23/monitor/main.py` & `jaaql-monitor-1.2.24/monitor/main.py`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.23/setup.py` & `jaaql-monitor-1.2.24/setup.py`

 * *Files identical despite different names*

