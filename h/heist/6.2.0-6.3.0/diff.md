# Comparing `tmp/heist-6.2.0.tar.gz` & `tmp/heist-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heist-6.2.0.tar", last modified: Wed Jul 13 14:40:59 2022, max compression
+gzip compressed data, was "heist-6.3.0.tar", last modified: Wed May  3 18:22:30 2023, max compression
```

## Comparing `heist-6.2.0.tar` & `heist-6.3.0.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:40:59.820250 heist-6.2.0/
--rw-rw-rw-   0 root         (0) root         (0)    11357 2022-07-13 14:40:48.000000 heist-6.2.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       43 2022-07-13 14:40:48.000000 heist-6.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2804 2022-07-13 14:40:59.820250 heist-6.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2331 2022-07-13 14:40:48.000000 heist-6.2.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:40:59.809249 heist-6.2.0/heist/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:40:59.802249 heist-6.2.0/heist/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:40:59.811249 heist-6.2.0/heist/acct/artifact/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-13 14:40:48.000000 heist-6.2.0/heist/acct/artifact/jfrog.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:40:59.811249 heist-6.2.0/heist/acct/recursive_contracts/
--rw-rw-rw-   0 root         (0) root         (0)       99 2022-07-13 14:40:48.000000 heist-6.2.0/heist/acct/recursive_contracts/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:40:59.803249 heist-6.2.0/heist/acct/tunnel/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:40:59.813249 heist-6.2.0/heist/acct/tunnel/ssh/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-13 14:40:48.000000 heist-6.2.0/heist/acct/tunnel/ssh/gssapi.py
--rw-rw-rw-   0 root         (0) root         (0)        9 2022-07-13 14:40:48.000000 heist-6.2.0/heist/acct/tunnel/ssh/pam.py
--rw-rw-rw-   0 root         (0) root         (0)      199 2022-07-13 14:40:48.000000 heist-6.2.0/heist/acct/tunnel/ssh/password.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-13 14:40:48.000000 heist-6.2.0/heist/acct/tunnel/ssh/public_key.py
--rw-rw-rw-   0 root         (0) root         (0)        9 2022-07-13 14:40:48.000000 heist-6.2.0/heist/acct/tunnel/ssh/secure_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:40:59.813249 heist-6.2.0/heist/artifact/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:40:59.814250 heist-6.2.0/heist/artifact/contracts/
--rw-rw-rw-   0 root         (0) root         (0)      573 2022-07-13 14:40:48.000000 heist-6.2.0/heist/artifact/contracts/init.py
--rw-rw-rw-   0 root         (0) root         (0)     4870 2022-07-13 14:40:48.000000 heist-6.2.0/heist/artifact/init.py
--rw-rw-rw-   0 root         (0) root         (0)     4820 2022-07-13 14:40:48.000000 heist-6.2.0/heist/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:40:59.814250 heist-6.2.0/heist/heist/
--rw-rw-rw-   0 root         (0) root         (0)     6663 2022-07-13 14:40:48.000000 heist-6.2.0/heist/heist/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:40:59.815250 heist-6.2.0/heist/heist/recursive_contracts/
--rw-rw-rw-   0 root         (0) root         (0)      786 2022-07-13 14:40:48.000000 heist-6.2.0/heist/heist/recursive_contracts/init.py
--rw-rw-rw-   0 root         (0) root         (0)      292 2022-07-13 14:40:48.000000 heist-6.2.0/heist/heist/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:40:59.816250 heist-6.2.0/heist/roster/
--rw-rw-rw-   0 root         (0) root         (0)     2221 2022-07-13 14:40:48.000000 heist-6.2.0/heist/roster/clustershell.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:40:59.817250 heist-6.2.0/heist/roster/contracts/
--rw-rw-rw-   0 root         (0) root         (0)      276 2022-07-13 14:40:48.000000 heist-6.2.0/heist/roster/contracts/init.py
--rw-rw-rw-   0 root         (0) root         (0)      333 2022-07-13 14:40:48.000000 heist-6.2.0/heist/roster/fernet.py
--rw-rw-rw-   0 root         (0) root         (0)      676 2022-07-13 14:40:48.000000 heist-6.2.0/heist/roster/flat.py
--rw-rw-rw-   0 root         (0) root         (0)     1866 2022-07-13 14:40:48.000000 heist-6.2.0/heist/roster/init.py
--rw-rw-rw-   0 root         (0) root         (0)     1951 2022-07-13 14:40:48.000000 heist-6.2.0/heist/roster/scan.py
--rw-rw-rw-   0 root         (0) root         (0)      118 2022-07-13 14:40:48.000000 heist-6.2.0/heist/scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:40:59.818250 heist-6.2.0/heist/service/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:40:59.818250 heist-6.2.0/heist/service/contracts/
--rw-rw-rw-   0 root         (0) root         (0)     1001 2022-07-13 14:40:48.000000 heist-6.2.0/heist/service/contracts/init.py
--rw-rw-rw-   0 root         (0) root         (0)     2701 2022-07-13 14:40:48.000000 heist-6.2.0/heist/service/init.py
--rw-rw-rw-   0 root         (0) root         (0)     1530 2022-07-13 14:40:48.000000 heist-6.2.0/heist/service/raw.py
--rw-rw-rw-   0 root         (0) root         (0)     1706 2022-07-13 14:40:48.000000 heist-6.2.0/heist/service/systemd.py
--rw-rw-rw-   0 root         (0) root         (0)     1973 2022-07-13 14:40:48.000000 heist-6.2.0/heist/service/win_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:40:59.819250 heist-6.2.0/heist/tool/
--rw-rw-rw-   0 root         (0) root         (0)     3049 2022-07-13 14:40:48.000000 heist-6.2.0/heist/tool/path.py
--rw-rw-rw-   0 root         (0) root         (0)     1034 2022-07-13 14:40:48.000000 heist-6.2.0/heist/tool/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:40:59.819250 heist-6.2.0/heist/tunnel/
--rw-rw-rw-   0 root         (0) root         (0)     7688 2022-07-13 14:40:48.000000 heist-6.2.0/heist/tunnel/asyncssh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:40:59.820250 heist-6.2.0/heist/tunnel/contracts/
--rw-rw-rw-   0 root         (0) root         (0)      410 2022-07-13 14:40:48.000000 heist-6.2.0/heist/tunnel/contracts/init.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2022-07-13 14:40:48.000000 heist-6.2.0/heist/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-13 14:40:59.811249 heist-6.2.0/heist.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2804 2022-07-13 14:40:59.000000 heist-6.2.0/heist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1041 2022-07-13 14:40:59.000000 heist-6.2.0/heist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-13 14:40:59.000000 heist-6.2.0/heist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       47 2022-07-13 14:40:59.000000 heist-6.2.0/heist.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       92 2022-07-13 14:40:59.000000 heist-6.2.0/heist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-07-13 14:40:59.000000 heist-6.2.0/heist.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      686 2022-07-13 14:40:48.000000 heist-6.2.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      129 2022-07-13 14:40:48.000000 heist-6.2.0/requirements-test.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-13 14:40:59.821250 heist-6.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2031 2022-07-13 14:40:48.000000 heist-6.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.896367 heist-6.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2023-05-03 18:22:18.000000 heist-6.3.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-05-03 18:22:18.000000 heist-6.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2804 2023-05-03 18:22:30.894534 heist-6.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2331 2023-05-03 18:22:18.000000 heist-6.3.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.885367 heist-6.3.0/heist/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.878033 heist-6.3.0/heist/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.886283 heist-6.3.0/heist/acct/artifact/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 18:22:18.000000 heist-6.3.0/heist/acct/artifact/jfrog.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.887200 heist-6.3.0/heist/acct/recursive_contracts/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-05-03 18:22:18.000000 heist-6.3.0/heist/acct/recursive_contracts/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.878950 heist-6.3.0/heist/acct/tunnel/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.888117 heist-6.3.0/heist/acct/tunnel/ssh/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 18:22:18.000000 heist-6.3.0/heist/acct/tunnel/ssh/gssapi.py
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-05-03 18:22:18.000000 heist-6.3.0/heist/acct/tunnel/ssh/pam.py
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-05-03 18:22:18.000000 heist-6.3.0/heist/acct/tunnel/ssh/password.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 18:22:18.000000 heist-6.3.0/heist/acct/tunnel/ssh/public_key.py
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-05-03 18:22:18.000000 heist-6.3.0/heist/acct/tunnel/ssh/secure_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.888117 heist-6.3.0/heist/artifact/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.889034 heist-6.3.0/heist/artifact/contracts/
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-05-03 18:22:18.000000 heist-6.3.0/heist/artifact/contracts/init.py
+-rw-rw-rw-   0 root         (0) root         (0)    15694 2023-05-03 18:22:18.000000 heist-6.3.0/heist/artifact/init.py
+-rw-rw-rw-   0 root         (0) root         (0)     5158 2023-05-03 18:22:18.000000 heist-6.3.0/heist/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.889034 heist-6.3.0/heist/heist/
+-rw-rw-rw-   0 root         (0) root         (0)     8876 2023-05-03 18:22:18.000000 heist-6.3.0/heist/heist/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.889950 heist-6.3.0/heist/heist/recursive_contracts/
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-05-03 18:22:18.000000 heist-6.3.0/heist/heist/recursive_contracts/init.py
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-05-03 18:22:18.000000 heist-6.3.0/heist/heist/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.890867 heist-6.3.0/heist/roster/
+-rw-rw-rw-   0 root         (0) root         (0)     2221 2023-05-03 18:22:18.000000 heist-6.3.0/heist/roster/clustershell.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.891784 heist-6.3.0/heist/roster/contracts/
+-rw-rw-rw-   0 root         (0) root         (0)      276 2023-05-03 18:22:18.000000 heist-6.3.0/heist/roster/contracts/init.py
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-05-03 18:22:18.000000 heist-6.3.0/heist/roster/fernet.py
+-rw-rw-rw-   0 root         (0) root         (0)      676 2023-05-03 18:22:18.000000 heist-6.3.0/heist/roster/flat.py
+-rw-rw-rw-   0 root         (0) root         (0)     1866 2023-05-03 18:22:18.000000 heist-6.3.0/heist/roster/init.py
+-rw-rw-rw-   0 root         (0) root         (0)     1951 2023-05-03 18:22:18.000000 heist-6.3.0/heist/roster/scan.py
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-05-03 18:22:18.000000 heist-6.3.0/heist/scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.892701 heist-6.3.0/heist/service/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.892701 heist-6.3.0/heist/service/contracts/
+-rw-rw-rw-   0 root         (0) root         (0)     1100 2023-05-03 18:22:18.000000 heist-6.3.0/heist/service/contracts/init.py
+-rw-rw-rw-   0 root         (0) root         (0)     3290 2023-05-03 18:22:18.000000 heist-6.3.0/heist/service/init.py
+-rw-rw-rw-   0 root         (0) root         (0)     3236 2023-05-03 18:22:18.000000 heist-6.3.0/heist/service/raw.py
+-rw-rw-rw-   0 root         (0) root         (0)     2013 2023-05-03 18:22:18.000000 heist-6.3.0/heist/service/systemd.py
+-rw-rw-rw-   0 root         (0) root         (0)     2308 2023-05-03 18:22:18.000000 heist-6.3.0/heist/service/win_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.893617 heist-6.3.0/heist/tool/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-05-03 18:22:18.000000 heist-6.3.0/heist/tool/artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)     3064 2023-05-03 18:22:18.000000 heist-6.3.0/heist/tool/path.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-05-03 18:22:18.000000 heist-6.3.0/heist/tool/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.894534 heist-6.3.0/heist/tunnel/
+-rw-rw-rw-   0 root         (0) root         (0)     7861 2023-05-03 18:22:18.000000 heist-6.3.0/heist/tunnel/asyncssh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.894534 heist-6.3.0/heist/tunnel/contracts/
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-05-03 18:22:18.000000 heist-6.3.0/heist/tunnel/contracts/init.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-03 18:22:18.000000 heist-6.3.0/heist/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 18:22:30.886283 heist-6.3.0/heist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2804 2023-05-03 18:22:30.000000 heist-6.3.0/heist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-05-03 18:22:30.000000 heist-6.3.0/heist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 18:22:30.000000 heist-6.3.0/heist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-03 18:22:30.000000 heist-6.3.0/heist.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2023-05-03 18:22:30.000000 heist-6.3.0/heist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-03 18:22:30.000000 heist-6.3.0/heist.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      686 2023-05-03 18:22:18.000000 heist-6.3.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-05-03 18:22:18.000000 heist-6.3.0/requirements-test.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 18:22:30.896367 heist-6.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2023-05-03 18:22:18.000000 heist-6.3.0/setup.py
```

### Comparing `heist-6.2.0/LICENSE` & `heist-6.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heist-6.2.0/PKG-INFO` & `heist-6.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heist
-Version: 6.2.0
+Version: 6.3.0
 Summary: Ephemeral software tunneling and delivery system
 Home-page: UNKNOWN
 Author: 
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `heist-6.2.0/README.rst` & `heist-6.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `heist-6.2.0/heist/conf.py` & `heist-6.3.0/heist/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,21 @@
     "roster_data": {"subcommands": ["_global_"]},
     "checkin_time": {"subcommands": ["_global_"]},
     "dynamic_upgrade": {"subcommands": ["_global_"]},
     "renderer": {"subcommands": ["_global_"]},
     "target": {"options": ["--tgt", "-t"], "subcommands": ["_global_"]},
     "artifact_version": {"options": ["-a, --artifact"], "subcommands": ["_global_"]},
     "service_plugin": {"options": ["-s", "--service"], "subcommands": ["_global_"]},
+    "manage_service": {"options": ["--service-status"], "subcommands": ["_global_"]},
     "auto_service": {"subcommands": ["_global_"]},
+    "clean": {
+        "options": ["--clean"],
+        "action": "store_true",
+        "subcommands": ["_global_"],
+    },
     "noclean": {
         "options": ["--noclean"],
         "action": "store_true",
         "subcommands": ["_global_"],
     },
     # ACCT options
     "acct_file": {"source": "acct", "os": "ACCT_FILE", "subcommands": ["_global_"]},
@@ -102,15 +108,15 @@
     "artifact_version": {
         "default": "",
         "help": "Version of the artifact to use for heist",
     },
     "roster_defaults": {
         "default": {},
         "type": dict,
-        "help": "Defaults options to use for all rosters. CLI options will"
+        "help": "Default options to use for all rosters. CLI options will"
         "override these defaults",
     },
     "service_plugin": {
         "default": "raw",
         "help": "The type of service to use when managing the artifacts service status",
     },
     "auto_service": {
@@ -119,14 +125,18 @@
         "help": "Auto detect the service manager to use on start up of service.",
     },
     "noclean": {
         "default": False,
         "action": "store_true",
         "help": "Whether to clean the deployed artifact and configurations",
     },
+    "run_dir_root": {
+        "default": False,
+        "help": "Directory location on remote system for root deployment",
+    },
 }
 SUBCOMMANDS = {
     # The manager determines how you want to create the tunnels and if you want to deploy
     # ephemeral agents to the remote systems
     "test": {x: "" for x in ("help", "desc")}
 }
 DYNE = {
```

### Comparing `heist-6.2.0/heist/heist/init.py` & `heist-6.3.0/heist/heist/init.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 The entry point for Heist, this is where config loading and the project
 spine is set up
 """
 import asyncio
 import ipaddress
 import pathlib
 import socket
+import subprocess
 import sys
 from typing import Any
 
 from dict_tools.data import NamespaceDict
 
 
 def __init__(hub):
@@ -23,20 +24,26 @@
     hub.pop.sub.load_subdirs(hub.service, recurse=True)
 
 
 def cli(hub):
     """
     Load the cli as the first thing we do to account for pluggable OS dependent systems.
     """
-    hub.pop.config.load(["heist", "acct"], cli="heist")
+    hub.pop.config.load(["heist", "acct", "rend"], cli="heist")
     hub.heist.init.env()
 
     # Create a path on host system to cache downloads
     # This location is where grains and salt binary will be downloaded to
-    pathlib.Path(hub.OPT.heist.artifacts_dir).mkdir(parents=True, exist_ok=True)
+    pathlib.Path(hub.OPT.heist.artifacts_dir).mkdir(0o700, parents=True, exist_ok=True)
+    if sys.platform.startswith("win"):
+        subprocess.run(["icacls", hub.OPT.heist.artifacts_dir, "inheritance:d"])
+        subprocess.run(
+            ["icacls", hub.OPT.heist.artifacts_dir, "/remove", "Users", "/T"]
+        )
+        subprocess.run(["icacls", hub.OPT.heist.artifacts_dir, "/GRANT:R", "Users:(R)"])
 
     # If we are on windows, create a separate loop so we can handle the
     # keyboard interrupt. due to issues with current asyncio, windows, and
     # python together, we cannot support signals natively when running from
     # windows. therefore, we must diverge code here
     if "win" in sys.platform:
         hub.pop.loop.create()
@@ -53,31 +60,51 @@
 
 def env(hub):
     """
     Translate the config into the needed vars on the hub.
     :param hub:
     :return:
     """
-    hub.heist.OS_DEFAULTS = {
-        "linux": {
-            "os_path": "/var/tmp/heist",
-            "user": "root",
-            "run_dir_root": "/var/",
-        },
-        "windows": {
-            "os_path": "C:\\Windows\\temp\\heist",
-            "user": "Administrator",
-            "run_dir_root": "C:\\Windows\\temp\\",
-        },
-        "default": {
-            "os_path": "/var/tmp/heist",
-            "user": "root",
-            "run_dir_root": "/var/",
-        },
-    }
+    if hub.OPT["heist"].run_dir_root:
+        run_dir_root = hub.OPT["heist"].run_dir_root
+        hub.heist.OS_DEFAULTS = {
+            "linux": {
+                "os_path": "/var/tmp/heist",
+                "user": "root",
+                "run_dir_root": run_dir_root,
+            },
+            "windows": {
+                "os_path": "C:\\Windows\\temp\\heist",
+                "user": "Administrator",
+                "run_dir_root": run_dir_root,
+            },
+            "default": {
+                "os_path": "/var/tmp/heist",
+                "user": "root",
+                "run_dir_root": run_dir_root,
+            },
+        }
+    else:
+        hub.heist.OS_DEFAULTS = {
+            "linux": {
+                "os_path": "/var/tmp/heist",
+                "user": "root",
+                "run_dir_root": "/var/tmp/",
+            },
+            "windows": {
+                "os_path": "C:\\Windows\\temp\\heist",
+                "user": "Administrator",
+                "run_dir_root": "C:\\Windows\\temp\\",
+            },
+            "default": {
+                "os_path": "/var/tmp/heist",
+                "user": "root",
+                "run_dir_root": "/var/tmp/",
+            },
+        }
 
 
 def default(hub, target_os: str, key: str) -> Any:
     os_defaults = hub.heist.OS_DEFAULTS.get(target_os)
     if not os_defaults:
         value = None
         hub.log.error(f"OS '{target_os}' not defined in hub.heist.OS_DEFAULTS")
@@ -103,14 +130,16 @@
         hub.pop.loop.start(
             hub.heist.init.run_remotes(
                 hub.SUBPARSER,
                 artifact_version=hub.OPT.heist.artifact_version,
                 roster_file=hub.OPT.heist.roster_file,
                 roster=hub.OPT.heist.roster,
                 roster_data=hub.OPT.heist.roster_data,
+                manage_service=hub.OPT.heist.manage_service,
+                clean=hub.OPT.heist.clean,
             ),
             sigint=hub.heist.init.clean,
             sigterm=hub.heist.init.clean,
         )
     except asyncio.CancelledError:
         hub.log.debug("Cancelled remaining running asyncio tasks")
     finally:
@@ -127,24 +156,45 @@
 
     await hub.heist.init.run_remotes(
         hub.SUBPARSER,
         artifact_version=hub.OPT.heist.artifact_version,
         roster_file=hub.OPT.heist.roster_file,
         roster=hub.OPT.heist.roster,
         roster_data=hub.OPT.heist.roster_data,
+        manage_service=hub.OPT.heist.manage_service,
+        clean=hub.OPT.heist.clean,
     )
 
 
+def display_output(hub, out):
+    """
+    print results to the screen
+    for the user
+    """
+    lines = []
+    for target in out:
+        for key, value in target.items():
+            if target["retvalue"] == 0:
+                # print green
+                lines.append(f"\033[92m {key}: {value}\033[00m\n")
+            else:
+                # print red
+                lines.append(f"\033[91m {key}: {value}\033[00m\n")
+    print("".join(lines))
+
+
 async def run_remotes(
     hub,
     manager: str,
     artifact_version=None,
     roster_file: str = "",
     roster: str = None,
     roster_data=None,
+    manage_service=None,
+    clean=False,
     **kwargs,
 ):
     """
     Configs, rosters and targets have been loaded, time to execute the
     remote system calls
     """
     try:
@@ -158,21 +208,32 @@
     for k, v in raw_remotes.items():
         remotes[k] = NamespaceDict(v)
     if not remotes:
         return False
 
     hub.log.debug(f"Heist manager is '{manager}'")
 
+    if manage_service:
+        valid_opts = ["start", "restart", "stop", "enable", "disable", "status"]
+        if manage_service not in valid_opts:
+            hub.log.error(f"The service cannot be managed with {manage_service}")
+            hub.log.error(f"Please use one of {valid_opts}")
+            return False
     ret = hub.heist[manager].run(
         remotes,
         artifact_version=artifact_version,
+        manage_service=manage_service,
+        clean=clean,
         **kwargs,
     )
     if asyncio.iscoroutine(ret):
-        await ret
+        _ret = await ret
+
+    hub.heist.init.display_output(out=_ret)
+    return _ret
 
 
 async def clean(hub, signal: int = None):
     """
     Clean up the connections
     """
     if signal:
```

### Comparing `heist-6.2.0/heist/heist/recursive_contracts/init.py` & `heist-6.3.0/heist/heist/recursive_contracts/init.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 DEFAULT_TUNNEL = "asyncssh"
 
 
 async def sig_run(
     hub,
     remotes: Dict[str, Dict[str, str]],
     artifact_version,
+    manage_service,
     roster_file: str,
     roster: str,
     **kwargs
 ):
     ...
 
 
@@ -30,9 +31,10 @@
         validate_remotes[id_] = _validate_remote(remote)
 
     kwargs.pop("remotes")
     return await ctx.func(
         kwargs.pop("hub"),
         remotes=validate_remotes,
         artifact_version=kwargs["artifact_version"],
+        manage_service=kwargs["manage_service"],
         **kwargs["kwargs"]
     )
```

### Comparing `heist-6.2.0/heist/roster/clustershell.py` & `heist-6.3.0/heist/roster/clustershell.py`

 * *Files identical despite different names*

### Comparing `heist-6.2.0/heist/roster/flat.py` & `heist-6.3.0/heist/roster/flat.py`

 * *Files identical despite different names*

### Comparing `heist-6.2.0/heist/roster/init.py` & `heist-6.3.0/heist/roster/init.py`

 * *Files identical despite different names*

### Comparing `heist-6.2.0/heist/roster/scan.py` & `heist-6.3.0/heist/roster/scan.py`

 * *Files identical despite different names*

### Comparing `heist-6.2.0/heist/service/contracts/init.py` & `heist-6.3.0/heist/service/contracts/init.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,30 +2,34 @@
     ...
 
 
 def sig_enable(hub, tunnel_plugin, target_name, service):
     ...
 
 
-def sig_start(hub, tunnel_plugin, target_name, service, **kwargs):
+def sig_start(hub, target_name, tunnel_plugin, service, **kwargs):
     ...
 
 
-def sig_stop(hub, tunnel_plugin, target_name, service):
+def sig_stop(hub, target_name, tunnel_plugin, service, target_os):
     ...
 
 
-def sig_restart(hub, tunnel_plugin, target_name, service):
+def sig_restart(hub, target_name, tunnel_plugin, service, **kwargs):
     ...
 
 
 def sig_clean(hub, target_name, tunnel_plugin, service):
     ...
 
 
+def sig_status(hub, target_name, tunnel_plugin, service, **kwargs):
+    ...
+
+
 def pre(hub, ctx):
     kwargs = ctx.get_arguments()
     if ctx.func.__name__ in ["clean", "get_service_plugin", "valid_service_names"]:
         return True
     service_name = kwargs.get("service")
     if ctx.func.__name__ in ["service_conf_path", "clean", "conf_path"]:
         service_name = kwargs.get("service_name")
```

### Comparing `heist-6.2.0/heist/service/init.py` & `heist-6.3.0/heist/service/init.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,28 +7,32 @@
 async def enable(hub, tunnel_plugin, target_name, service):
     await hub.service[hub.OPT.heist.service_plugin].enable(
         tunnel_plugin, target_name, service
     )
 
 
 async def start(hub, tunnel_plugin, target_name, service, **kwargs):
-    await hub.service[hub.OPT.heist.service_plugin].start(
+    return await hub.service[hub.OPT.heist.service_plugin].start(
         tunnel_plugin, target_name, service, **kwargs
     )
 
 
-async def stop(hub, tunnel_plugin, target_name, service):
-    await hub.service[hub.OPT.heist.service_plugin].stop(
-        tunnel_plugin, target_name, service
+async def stop(hub, tunnel_plugin, target_name, service, target_os="linux"):
+    return await hub.service[hub.OPT.heist.service_plugin].stop(
+        tunnel_plugin,
+        target_name,
+        service,
+        target_os=target_os,
     )
 
 
-async def restart(hub, tunnel_plugin, target_name, service):
-    await hub.service[hub.OPT.heist.service_plugin].restart(
-        tunnel_plugin, target_name, service
+async def restart(hub, target_name, tunnel_plugin, service, **kwargs):
+    hub.log.debug(f"Restarting the service {service}")
+    return await hub.service[hub.OPT.heist.service_plugin].restart(
+        target_name, tunnel_plugin, service, **kwargs
     )
 
 
 def get_service_plugin(hub, remote=None, grains=None):
     """
     Return the serivce manager plugin that should be used.
     """
@@ -60,24 +64,43 @@
         service_plugin = hub.service.init.get_service_plugin()
     conf_path = hub.service[service_plugin].conf_path(service_name)
     if not conf_path:
         return ""
     return conf_path
 
 
-async def clean(hub, target_name, tunnel_plugin, service_name, service_plugin):
+async def clean(
+    hub,
+    target_name,
+    tunnel_plugin,
+    service_name,
+    service_plugin=None,
+    target_os="linux",
+):
+    if not service_plugin:
+        service_plugin = hub.heist.CONS[target_name]["service_plugin"]
     # stop service
-    await hub.service[hub.heist.CONS[target_name]["service_plugin"]].stop(
-        tunnel_plugin, target_name, service_name
+    await hub.service[service_plugin].stop(
+        target_name, tunnel_plugin, service_name, target_os=target_os
     )
 
     service_conf = hub.service.init.service_conf_path(service_name)
     if service_conf:
         ret = await hub.tunnel[tunnel_plugin].cmd(target_name, f"[ -f {service_conf} ]")
         if ret.returncode == 0:
             await hub.tunnel[tunnel_plugin].cmd(target_name, f"rm -f {service_conf}")
         else:
             hub.log.error(
                 f"The conf file {service_conf} does not exist. Will not attempt to remove"
             )
 
     await hub.service[service_plugin].clean(target_name, tunnel_plugin, service_name)
+
+
+async def status(hub, target_name, tunnel_plugin, service, target_os="linux"):
+    """
+    Check the status of the service and return if it's
+    running or not.
+    """
+    return await hub.service[hub.OPT.heist.service_plugin].status(
+        target_name, tunnel_plugin, service
+    )
```

### Comparing `heist-6.2.0/heist/service/raw.py` & `heist-6.3.0/heist/service/systemd.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,69 @@
-async def disable(hub, tunnel_plugin, target_name, service):
-    pass
-
-
-async def enable(hub, tunnel_plugin, target_name, service):
-    pass
+import os
 
 
-async def start(
-    hub, tunnel_plugin, target_name, service, run_cmd=None, target_os="linux", **kwargs
-):
-    """
-    Start the service in the background
-    """
-    cmd = [f"{run_cmd}"]
+async def disable(hub, tunnel_plugin, target_name, service):
     ret = await hub.tunnel[tunnel_plugin].cmd(
-        target_name, " ".join(cmd), background=True, target_os=target_os
+        target_name, f"systemctl disable {service}"
     )
-    if ret.returncode != 0:
+    if ret.exit_status != 0:
         hub.log.error(ret.stderr)
         return False
     return True
 
 
-async def stop(hub, tunnel_plugin, target_name, service):
-    """
-    Stop the service
-    """
-    # TODO: Need to figure out how to get target_os here
-    target_os, _ = await hub.tool.system.os_arch(target_name, tunnel_plugin)
-    if target_os == "windows":
-        kill_cmd = (
-            "Stop-Process -Name salt -ErrorAction SilentlyContinue; "
-            "If ($?) { exit 0 } else { exit 1 }"
-        )
-    else:
-        kill_cmd = f"pkill -f {service}"
-    hub.log.debug(f"Attempting to kill {service} with: {kill_cmd}")
+async def enable(hub, tunnel_plugin, target_name, service):
     ret = await hub.tunnel[tunnel_plugin].cmd(
-        target_name, kill_cmd, target_os=target_os
+        target_name, f"systemctl enable {service}"
     )
     if ret.exit_status != 0:
         hub.log.error(ret.stderr)
         return False
-    hub.log.info(f"Successfully killed {service}")
     return True
 
 
-async def restart(hub, tunnel_plugin, target_name, service):
-    pass
+async def start(hub, target_name, tunnel_plugin, service, block=True, **kwargs):
+    cmd = [f"systemctl start {service}"]
+    if not block:
+        cmd.append("--no-block")
+    ret = await hub.tunnel[tunnel_plugin].cmd(target_name, " ".join(cmd))
+    if ret.exit_status != 0:
+        hub.log.error(ret.stderr)
+        return False
+    return True
+
+
+async def stop(hub, target_name, tunnel_plugin, service, target_os="linux"):
+    ret = await hub.tunnel[tunnel_plugin].cmd(target_name, f"systemctl stop {service}")
+    if ret.exit_status != 0:
+        hub.log.error(ret.stderr)
+        return False
+    return True
+
+
+async def restart(hub, target_name, tunnel_plugin, service):
+    ret = await hub.tunnel[tunnel_plugin].cmd(
+        target_name, f"systemctl restart {service}"
+    )
+    if ret.exit_status != 0:
+        hub.log.error(ret.stderr)
+        return False
+    return True
 
 
 def conf_path(hub, service_name):
-    pass
+    return hub.tool.path.path_convert(
+        "linux", "/etc", ["systemd", "system", f"{service_name}.service"]
+    )
 
 
 async def clean(hub, target_name, tunnel_plugin, service):
-    pass
+    await hub.tunnel[tunnel_plugin].cmd(target_name, f"systemctl daemon-reload")
+
+
+async def status(hub, target_name, tunnel_plugin, service, **kwargs):
+    cmd = [f"systemctl status {service}"]
+    ret = await hub.tunnel[tunnel_plugin].cmd(target_name, " ".join(cmd))
+    if ret.exit_status != 0:
+        hub.log.error(ret.stderr)
+        return False
+    return True
```

### Comparing `heist-6.2.0/heist/service/systemd.py` & `heist-6.3.0/heist/service/win_service.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,83 @@
-import os
-
-
 async def disable(hub, tunnel_plugin, target_name, service):
     ret = await hub.tunnel[tunnel_plugin].cmd(
-        target_name, f"systemctl disable {service}"
+        target_name,
+        f"Set-Service -Name {service} -StartupType Disabled; "
+        f"If ($?) {{ exit 0 }} else {{ exit 1 }}",
     )
     if ret.exit_status != 0:
         hub.log.error(ret.stderr)
         return False
     return True
 
 
 async def enable(hub, tunnel_plugin, target_name, service):
     ret = await hub.tunnel[tunnel_plugin].cmd(
-        target_name, f"systemctl enable {service}"
+        target_name,
+        f"Set-Service -Name {service} -StartupType Automatic; "
+        f"If ($?) {{ exit 0 }} else {{ exit 1 }}",
     )
     if ret.exit_status != 0:
         hub.log.error(ret.stderr)
         return False
     return True
 
 
-async def start(hub, tunnel_plugin, target_name, service, block=True, **kwargs):
-    cmd = [f"systemctl start {service}"]
-    if not block:
-        cmd.append("--no-block")
-    ret = await hub.tunnel[tunnel_plugin].cmd(target_name, " ".join(cmd))
+async def start(hub, target_name, tunnel_plugin, service, **kwargs):
+    ret = await hub.tunnel[tunnel_plugin].cmd(
+        target_name,
+        f"Start-Service -Name {service}; If ($?) {{ exit 0 }} else {{ exit 1 }}",
+    )
     if ret.exit_status != 0:
         hub.log.error(ret.stderr)
         return False
     return True
 
 
-async def stop(hub, tunnel_plugin, target_name, service):
-    ret = await hub.tunnel[tunnel_plugin].cmd(target_name, f"systemctl stop {service}")
+async def stop(hub, target_name, tunnel_plugin, service):
+    ret = await hub.tunnel[tunnel_plugin].cmd(
+        target_name,
+        f"Stop-Service -Name {service}; If ($?) {{ exit 0 }} else {{ exit 1 }}",
+    )
     if ret.exit_status != 0:
         hub.log.error(ret.stderr)
         return False
     return True
 
 
-async def restart(hub, tunnel_plugin, target_name, service):
+async def restart(hub, target_name, tunnel_plugin, service):
     ret = await hub.tunnel[tunnel_plugin].cmd(
-        target_name, f"systemctl restart {service}"
+        target_name,
+        f"Restart-Service -Name {service}; If ($?) {{ exit 0 }} else {{ exit 1 }}",
     )
     if ret.exit_status != 0:
         hub.log.error(ret.stderr)
         return False
     return True
 
 
 def conf_path(hub, service_name):
-    return hub.tool.path.path_convert(
-        "linux", "/etc", ["systemd", "system", f"{service_name}.service"]
-    )
+    pass
 
 
 async def clean(hub, target_name, tunnel_plugin, service):
-    await hub.tunnel[tunnel_plugin].cmd(target_name, f"systemctl daemon-reload")
+    ret = await hub.tunnel[tunnel_plugin].cmd(
+        target_name, f"cmd /c sc delete {service}"
+    )
+    if ret.exit_status != 0:
+        hub.log.error(ret.stderr)
+        return False
+    return True
+
+
+async def status(hub, target_name, tunnel_plugin, service, **kwargs):
+    """
+    Get status of a service on windows
+    """
+    ret = await hub.tunnel[tunnel_plugin].cmd(
+        target_name,
+        f"Get-Service {service}",
+    )
+    if ret.exit_status != 0:
+        hub.log.error(ret.stderr)
+        return False
+    return True
```

### Comparing `heist-6.2.0/heist/tool/path.py` & `heist-6.3.0/heist/tool/path.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Path operations for heist
 """
 import os
+import pathlib
 import sys
 from pathlib import Path
 from pathlib import PurePosixPath
 from pathlib import PureWindowsPath
 
 
 def path_convert(hub, target_system, entry_path, ext_path):
```

### Comparing `heist-6.2.0/heist/tool/system.py` & `heist-6.3.0/heist/tool/system.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from typing import Tuple
 
 
 async def os_arch(hub, target_name: str, tunnel_plugin: str) -> Tuple[str, str]:
     """
     Query the system for the OS and architecture type
     """
-    DELIM = "|"
+    DELIM = "'|'"
     ret = await hub.tunnel[tunnel_plugin].cmd(
-        target_name, f'echo "$OSTYPE{DELIM}$MACHTYPE{DELIM}$env:PROCESSOR_ARCHITECTURE"'
+        target_name,
+        f'echo "$OSTYPE{DELIM}$MACHTYPE{DELIM}$env:PROCESSOR_ARCHITECTURE"'
+        # target_name, f'echo "$OSTYPE|$MACHTYPE|$env:PROCESSOR_ARCHITECTURE"'
     )
     assert not ret.returncode, ret.stderr
-    kernel, arch, winarch = ret.stdout.lower().split(DELIM, maxsplit=2)
+    kernel, arch, winarch = ret.stdout.lower().split("|", maxsplit=2)
 
     # Set the architecture bit
     if "64" in winarch or "64" in arch:
         os_arch = "amd64"
     else:
         os_arch = "i386"
```

### Comparing `heist-6.2.0/heist/tunnel/asyncssh.py` & `heist-6.3.0/heist/tunnel/asyncssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,33 +131,38 @@
     sudo_password = re.compile(r"(?:.*)[Pp]assword(?: for .*)?:", re.M)
     con: asyncssh.SSHClientConnection = hub.tunnel.asyncssh.CONS[name]["con"]
     if target_os == "windows":
         win_background_cmd = command
         arg_list = win_background_cmd.split()
         win_background_cmd = arg_list.pop(0)
         arg_list = " ".join(arg_list)
-        win_background_cmd = "; ".join(
-            [
-                f'$action = New-ScheduledTaskAction -Execute "{win_background_cmd}" '
-                f'-Argument "{arg_list}"',
-                "$trigger = New-ScheduledTaskTrigger -Once -At 00:00",
-                "$principal = New-ScheduledTaskPrincipal "
-                '-UserId "$env:USERNAME" '
-                '-LogonType "S4U" '
-                "-RunLevel Highest",
-                "Register-ScheduledTask -Action $action "
-                "-Trigger $trigger "
-                "-Principal $principal "
-                "-TaskName heist-background "
-                "-Description 'Run background process' "
-                "-Force",
-                "Start-ScheduledTask -TaskName heist-background",
-                "Unregister-ScheduledTask -TaskName heist-background "
-                "-Confirm:$false",
-            ]
+        win_background_cmd = (
+            "powershell -command "
+            + '"'
+            + "; ".join(
+                [
+                    f"$action = New-ScheduledTaskAction -Execute '{win_background_cmd}' "
+                    f"-Argument '{arg_list}'",
+                    "$trigger = New-ScheduledTaskTrigger -Once -At 00:00",
+                    "$principal = New-ScheduledTaskPrincipal "
+                    '-UserId "$env:USERNAME" '
+                    '-LogonType "S4U" '
+                    "-RunLevel Highest",
+                    "Register-ScheduledTask -Action $action "
+                    "-Trigger $trigger "
+                    "-Principal $principal "
+                    "-TaskName heist-background "
+                    "-Description 'Run background process' "
+                    "-Force",
+                    "Start-ScheduledTask -TaskName heist-background",
+                    "Unregister-ScheduledTask -TaskName heist-background "
+                    "-Confirm:$false",
+                ]
+            )
+            + '"'
         )
 
     result = {}
     if hub.tunnel.asyncssh.CONS[name].get("tty"):
         kwargs["term_type"] = (
             hub.tunnel.asyncssh.CONS[name].get("term_type") or "xterm-color"
         )
```

### Comparing `heist-6.2.0/heist.egg-info/PKG-INFO` & `heist-6.3.0/heist.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heist
-Version: 6.2.0
+Version: 6.3.0
 Summary: Ephemeral software tunneling and delivery system
 Home-page: UNKNOWN
 Author: 
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `heist-6.2.0/heist.egg-info/SOURCES.txt` & `heist-6.3.0/heist.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -32,11 +32,12 @@
 heist/roster/scan.py
 heist/roster/contracts/init.py
 heist/service/init.py
 heist/service/raw.py
 heist/service/systemd.py
 heist/service/win_service.py
 heist/service/contracts/init.py
+heist/tool/artifacts.py
 heist/tool/path.py
 heist/tool/system.py
 heist/tunnel/asyncssh.py
 heist/tunnel/contracts/init.py
```

### Comparing `heist-6.2.0/pyproject.toml` & `heist-6.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `heist-6.2.0/setup.py` & `heist-6.3.0/setup.py`

 * *Files identical despite different names*

