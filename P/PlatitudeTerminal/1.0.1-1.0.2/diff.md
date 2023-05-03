# Comparing `tmp/PlatitudeTerminal-1.0.1.tar.gz` & `tmp/PlatitudeTerminal-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlatitudeTerminal-1.0.1.tar", last modified: Tue May  2 19:34:42 2023, max compression
+gzip compressed data, was "PlatitudeTerminal-1.0.2.tar", last modified: Wed May  3 04:06:02 2023, max compression
```

## Comparing `PlatitudeTerminal-1.0.1.tar` & `PlatitudeTerminal-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-02 19:34:42.968804 PlatitudeTerminal-1.0.1/
--rw-r--r--   0 louis      (501) staff       (20)     2273 2023-05-02 19:34:42.968854 PlatitudeTerminal-1.0.1/PKG-INFO
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-02 19:34:42.967003 PlatitudeTerminal-1.0.1/PlatitudeTerminal.egg-info/
--rw-r--r--   0 louis      (501) staff       (20)     2273 2023-05-02 19:34:42.000000 PlatitudeTerminal-1.0.1/PlatitudeTerminal.egg-info/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)      457 2023-05-02 19:34:42.000000 PlatitudeTerminal-1.0.1/PlatitudeTerminal.egg-info/SOURCES.txt
--rw-r--r--   0 louis      (501) staff       (20)        1 2023-05-02 19:34:42.000000 PlatitudeTerminal-1.0.1/PlatitudeTerminal.egg-info/dependency_links.txt
--rw-r--r--   0 louis      (501) staff       (20)       43 2023-05-02 19:34:42.000000 PlatitudeTerminal-1.0.1/PlatitudeTerminal.egg-info/entry_points.txt
--rw-r--r--   0 louis      (501) staff       (20)      144 2023-05-02 19:34:42.000000 PlatitudeTerminal-1.0.1/PlatitudeTerminal.egg-info/requires.txt
--rw-r--r--   0 louis      (501) staff       (20)       10 2023-05-02 19:34:42.000000 PlatitudeTerminal-1.0.1/PlatitudeTerminal.egg-info/top_level.txt
--rw-r--r--   0 louis      (501) staff       (20)     2079 2023-05-02 17:40:54.000000 PlatitudeTerminal-1.0.1/README.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-02 19:34:42.968603 PlatitudeTerminal-1.0.1/peregrine/
--rw-r--r--   0 louis      (501) staff       (20)        0 2023-04-17 02:58:31.000000 PlatitudeTerminal-1.0.1/peregrine/__init__.py
--rw-r--r--   0 louis      (501) staff       (20)    29618 2023-05-02 19:21:46.000000 PlatitudeTerminal-1.0.1/peregrine/cli.py
--rw-r--r--   0 louis      (501) staff       (20)     3098 2023-04-23 07:52:41.000000 PlatitudeTerminal-1.0.1/peregrine/client.py
--rw-r--r--   0 louis      (501) staff       (20)      980 2023-04-22 18:06:19.000000 PlatitudeTerminal-1.0.1/peregrine/colorutils.py
--rw-r--r--   0 louis      (501) staff       (20)      246 2023-04-22 22:46:59.000000 PlatitudeTerminal-1.0.1/peregrine/errors.py
--rw-r--r--   0 louis      (501) staff       (20)       21 2023-05-02 19:33:47.000000 PlatitudeTerminal-1.0.1/peregrine/install.py
--rw-r--r--   0 louis      (501) staff       (20)       87 2023-03-30 08:54:25.000000 PlatitudeTerminal-1.0.1/peregrine/main.py
--rw-r--r--   0 louis      (501) staff       (20)     2838 2023-05-02 19:16:55.000000 PlatitudeTerminal-1.0.1/peregrine/stateutils.py
--rw-r--r--   0 louis      (501) staff       (20)      510 2023-05-02 06:21:17.000000 PlatitudeTerminal-1.0.1/pyproject.toml
--rw-r--r--   0 louis      (501) staff       (20)      277 2023-05-02 19:34:42.969053 PlatitudeTerminal-1.0.1/setup.cfg
--rw-r--r--   0 louis      (501) staff       (20)       37 2023-04-18 06:28:45.000000 PlatitudeTerminal-1.0.1/setup.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-03 04:06:02.574087 PlatitudeTerminal-1.0.2/
+-rw-r--r--   0 louis      (501) staff       (20)     2273 2023-05-03 04:06:02.574142 PlatitudeTerminal-1.0.2/PKG-INFO
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-03 04:06:02.572099 PlatitudeTerminal-1.0.2/PlatitudeTerminal.egg-info/
+-rw-r--r--   0 louis      (501) staff       (20)     2273 2023-05-03 04:06:02.000000 PlatitudeTerminal-1.0.2/PlatitudeTerminal.egg-info/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)      457 2023-05-03 04:06:02.000000 PlatitudeTerminal-1.0.2/PlatitudeTerminal.egg-info/SOURCES.txt
+-rw-r--r--   0 louis      (501) staff       (20)        1 2023-05-03 04:06:02.000000 PlatitudeTerminal-1.0.2/PlatitudeTerminal.egg-info/dependency_links.txt
+-rw-r--r--   0 louis      (501) staff       (20)       43 2023-05-03 04:06:02.000000 PlatitudeTerminal-1.0.2/PlatitudeTerminal.egg-info/entry_points.txt
+-rw-r--r--   0 louis      (501) staff       (20)      154 2023-05-03 04:06:02.000000 PlatitudeTerminal-1.0.2/PlatitudeTerminal.egg-info/requires.txt
+-rw-r--r--   0 louis      (501) staff       (20)       10 2023-05-03 04:06:02.000000 PlatitudeTerminal-1.0.2/PlatitudeTerminal.egg-info/top_level.txt
+-rw-r--r--   0 louis      (501) staff       (20)     2079 2023-05-02 17:40:54.000000 PlatitudeTerminal-1.0.2/README.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-03 04:06:02.573873 PlatitudeTerminal-1.0.2/peregrine/
+-rw-r--r--   0 louis      (501) staff       (20)        0 2023-04-17 02:58:31.000000 PlatitudeTerminal-1.0.2/peregrine/__init__.py
+-rw-r--r--   0 louis      (501) staff       (20)    29668 2023-05-03 04:00:43.000000 PlatitudeTerminal-1.0.2/peregrine/cli.py
+-rw-r--r--   0 louis      (501) staff       (20)     3098 2023-04-23 07:52:41.000000 PlatitudeTerminal-1.0.2/peregrine/client.py
+-rw-r--r--   0 louis      (501) staff       (20)      980 2023-04-22 18:06:19.000000 PlatitudeTerminal-1.0.2/peregrine/colorutils.py
+-rw-r--r--   0 louis      (501) staff       (20)      246 2023-04-22 22:46:59.000000 PlatitudeTerminal-1.0.2/peregrine/errors.py
+-rw-r--r--   0 louis      (501) staff       (20)       21 2023-05-03 03:58:08.000000 PlatitudeTerminal-1.0.2/peregrine/install.py
+-rw-r--r--   0 louis      (501) staff       (20)       87 2023-03-30 08:54:25.000000 PlatitudeTerminal-1.0.2/peregrine/main.py
+-rw-r--r--   0 louis      (501) staff       (20)     2838 2023-05-02 19:16:55.000000 PlatitudeTerminal-1.0.2/peregrine/stateutils.py
+-rw-r--r--   0 louis      (501) staff       (20)      527 2023-05-03 03:52:08.000000 PlatitudeTerminal-1.0.2/pyproject.toml
+-rw-r--r--   0 louis      (501) staff       (20)      277 2023-05-03 04:06:02.574570 PlatitudeTerminal-1.0.2/setup.cfg
+-rw-r--r--   0 louis      (501) staff       (20)       37 2023-04-18 06:28:45.000000 PlatitudeTerminal-1.0.2/setup.py
```

### Comparing `PlatitudeTerminal-1.0.1/PKG-INFO` & `PlatitudeTerminal-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlatitudeTerminal
-Version: 1.0.1
+Version: 1.0.2
 Summary: "Natural language command line queries."
 Author: Louis Smidt
 Requires-Python: >3.8
 Description-Content-Type: text/markdown
 
 # Platitude Terminal
 ## by Platitude.ai
```

### Comparing `PlatitudeTerminal-1.0.1/PlatitudeTerminal.egg-info/PKG-INFO` & `PlatitudeTerminal-1.0.2/PlatitudeTerminal.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlatitudeTerminal
-Version: 1.0.1
+Version: 1.0.2
 Summary: "Natural language command line queries."
 Author: Louis Smidt
 Requires-Python: >3.8
 Description-Content-Type: text/markdown
 
 # Platitude Terminal
 ## by Platitude.ai
```

### Comparing `PlatitudeTerminal-1.0.1/README.md` & `PlatitudeTerminal-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `PlatitudeTerminal-1.0.1/peregrine/cli.py` & `PlatitudeTerminal-1.0.2/peregrine/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import typer
 import fcntl, termios, sys
 from halo import Halo
 import requests
 import pyrebase
+from packaging import version as vers
 import json, time, jwt
 from peregrine import stateutils, client, install, errors, colorutils
 
 
 # Use your Firebase project configuration
 firebase_config = {
   "apiKey": "AIzaSyCqZOXQZZ6q1WPzIPIE7anvi3-Hfjuuzh8",
@@ -464,25 +465,25 @@
 
 @app.command()
 def version(verbose = True):
 
     try:
         (your_v, latest_v, minimum_v) = fetchVersions()
     
-        verboseEcho(f"Your installed Platitude.ai version: {float(your_v)}", verbose)
+        verboseEcho(f"Currently installed version: {your_v}", verbose)
         
-        if your_v < minimum_v:
+        if vers.parse(your_v) < vers.parse(minimum_v):
             verboseEcho(f"Currently installed version: {your_v} is older than minimum version: {minimum_v}. You'll need to update before you can use Platitude.ai. Please run: `pip install --upgrade PlatitudeTerminal` to get the latest features.", verbose) 
             
             print_branch = typer.prompt("Copy command? [y / N]", type=str)
             if print_branch == 'y':
                 writeToTerminal("pip install --upgrade PlatitudeTerminal")
             raise errors.PeregrineVersionOutOfDateError(f"Your version: {your_v}, minnimum version: {minimum_v}, latest version: {latest_v}.")
         
-        elif your_v < latest_v:
+        elif vers.parse(your_v) < vers.parse(latest_v):
             verboseEcho("A new version is available to install! Run: `pip install --upgrade PlatitudeTerminal` to upgrade to get the latest features.", verbose)
             
         else:
 
             verboseEcho(f"Latest Version: {latest_v}", verbose)
             verboseEcho(f"Minimum Version: {minimum_v}", verbose)
 
@@ -511,15 +512,15 @@
         latest_v = response_json['latest']
         minimum_v = response_json['minimum']
 
     except Exception as e:
         raise errors.PeregrineConnectionError(f"Versions Failed to connect to server. Check your internet connection. Error {e}")
 
     else:
-        return (float(your_v), float(latest_v), float(minimum_v))
+        return (your_v, latest_v, minimum_v)
 
 
 def fetchUsage(uid, idT):
         auth_headers = {'Authorization': f'Bearer {idT}', 'Content-Type': 'application/json'}
         body = {'uid': uid }
 
         try:
```

### Comparing `PlatitudeTerminal-1.0.1/peregrine/client.py` & `PlatitudeTerminal-1.0.2/peregrine/client.py`

 * *Files identical despite different names*

### Comparing `PlatitudeTerminal-1.0.1/peregrine/colorutils.py` & `PlatitudeTerminal-1.0.2/peregrine/colorutils.py`

 * *Files identical despite different names*

### Comparing `PlatitudeTerminal-1.0.1/peregrine/stateutils.py` & `PlatitudeTerminal-1.0.2/peregrine/stateutils.py`

 * *Files identical despite different names*

