# Comparing `tmp/jaaql-monitor-1.2.25.tar.gz` & `tmp/jaaql-monitor-1.2.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.25.tar", last modified: Wed May  3 01:57:22 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.26.tar", last modified: Wed May  3 02:11:08 2023, max compression
```

## Comparing `jaaql-monitor-1.2.25.tar` & `jaaql-monitor-1.2.26.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 01:57:22.014507 jaaql-monitor-1.2.25/
--rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.25/LICENSE.txt
--rw-rw-rw-   0        0        0     1475 2023-05-03 01:57:22.013507 jaaql-monitor-1.2.25/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.25/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 01:57:22.006505 jaaql-monitor-1.2.25/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-05-03 01:57:21.000000 jaaql-monitor-1.2.25/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-03 01:57:21.000000 jaaql-monitor-1.2.25/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 01:57:21.000000 jaaql-monitor-1.2.25/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-03 01:57:21.000000 jaaql-monitor-1.2.25/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-03 01:57:21.000000 jaaql-monitor-1.2.25/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-03 01:57:22.011508 jaaql-monitor-1.2.25/monitor/
--rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.25/monitor/__init__.py
--rw-rw-rw-   0        0        0    23725 2023-05-03 01:57:01.000000 jaaql-monitor-1.2.25/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-05-03 01:57:07.000000 jaaql-monitor-1.2.25/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-05-03 01:57:22.014507 jaaql-monitor-1.2.25/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.25/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 02:11:08.867667 jaaql-monitor-1.2.26/
+-rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.26/LICENSE.txt
+-rw-rw-rw-   0        0        0     1475 2023-05-03 02:11:08.866668 jaaql-monitor-1.2.26/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.26/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 02:11:08.854667 jaaql-monitor-1.2.26/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1475 2023-05-03 02:11:08.000000 jaaql-monitor-1.2.26/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-03 02:11:08.000000 jaaql-monitor-1.2.26/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 02:11:08.000000 jaaql-monitor-1.2.26/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-03 02:11:08.000000 jaaql-monitor-1.2.26/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-03 02:11:08.000000 jaaql-monitor-1.2.26/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 02:11:08.864668 jaaql-monitor-1.2.26/monitor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.26/monitor/__init__.py
+-rw-rw-rw-   0        0        0    23648 2023-05-03 02:10:51.000000 jaaql-monitor-1.2.26/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-05-03 02:10:52.000000 jaaql-monitor-1.2.26/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-03 02:11:08.867667 jaaql-monitor-1.2.26/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.26/setup.py
```

### Comparing `jaaql-monitor-1.2.25/LICENSE.txt` & `jaaql-monitor-1.2.26/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.25/PKG-INFO` & `jaaql-monitor-1.2.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.25
+Version: 1.2.26
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.25/README.md` & `jaaql-monitor-1.2.26/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.25/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.26/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.25
+Version: 1.2.26
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.25/monitor/main.py` & `jaaql-monitor-1.2.26/monitor/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,16 +154,14 @@
                 conn.oauth_token = {HEADER__security_bypass: conn.password.split(MARKER__bypass)[1]}
             elif conn.password.startswith(MARKER__jaaql_bypass):
                 conn.oauth_token = {HEADER__security_bypass_jaaql: conn.password.split(MARKER__jaaql_bypass)[1]}
             else:
                 self._fetch_oauth_token_for_current_connection()
 
         start_time = datetime.now()
-        print("Accessing URL")
-        print(conn.get_http_url() + endpoint)
         res = requests.request(method, conn.get_http_url() + endpoint, json=send_json, headers=conn.oauth_token)
 
         if res.status_code == 401:
             self.log("Refreshing oauth token")
             self._fetch_oauth_token_for_current_connection()
             start_time = datetime.now()
             res = requests.request(method, conn.get_http_url() + endpoint, json=send_json, headers=conn.oauth_token)
```

### Comparing `jaaql-monitor-1.2.25/setup.py` & `jaaql-monitor-1.2.26/setup.py`

 * *Files identical despite different names*

