# Comparing `tmp/guify-0.2.7.tar.gz` & `tmp/guify-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guify-0.2.7.tar", last modified: Wed May  3 10:17:20 2023, max compression
+gzip compressed data, was "guify-0.2.8.tar", last modified: Wed May  3 18:18:18 2023, max compression
```

## Comparing `guify-0.2.7.tar` & `guify-0.2.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:17:20.538101 guify-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-03 10:15:47.000000 guify-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-03 10:15:47.000000 guify-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-05-03 10:17:20.538101 guify-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-03 10:15:47.000000 guify-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:17:20.530101 guify-0.2.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-05-03 10:15:47.000000 guify-0.2.7/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-03 10:15:47.000000 guify-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-03 10:17:20.538101 guify-0.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:17:20.530101 guify-0.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:17:20.534101 guify-0.2.7/src/guify/
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-03 10:15:47.000000 guify-0.2.7/src/guify/App.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-03 10:15:47.000000 guify-0.2.7/src/guify/BaseTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-03 10:15:47.000000 guify-0.2.7/src/guify/ConfigTab.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-03 10:15:47.000000 guify-0.2.7/src/guify/Monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-03 10:15:47.000000 guify-0.2.7/src/guify/TestPool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-05-03 10:15:47.000000 guify-0.2.7/src/guify/TestWorker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-03 10:15:47.000000 guify-0.2.7/src/guify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-03 10:15:47.000000 guify-0.2.7/src/guify/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-03 10:15:47.000000 guify-0.2.7/src/guify/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:17:20.538101 guify-0.2.7/src/guify/web/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-03 10:17:12.000000 guify-0.2.7/src/guify/web/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-05-03 10:16:55.000000 guify-0.2.7/src/guify/web/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-03 10:17:12.000000 guify-0.2.7/src/guify/web/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-03 10:16:55.000000 guify-0.2.7/src/guify/web/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:17:20.530101 guify-0.2.7/src/guify/web/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:17:20.538101 guify-0.2.7/src/guify/web/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   144117 2023-05-03 10:17:12.000000 guify-0.2.7/src/guify/web/static/css/main.c779b13f.css
--rw-r--r--   0 runner    (1001) docker     (123)   481735 2023-05-03 10:17:12.000000 guify-0.2.7/src/guify/web/static/css/main.c779b13f.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:17:20.538101 guify-0.2.7/src/guify/web/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   207756 2023-05-03 10:17:12.000000 guify-0.2.7/src/guify/web/static/js/main.bf3c494e.js
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-03 10:17:12.000000 guify-0.2.7/src/guify/web/static/js/main.bf3c494e.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   660732 2023-05-03 10:17:12.000000 guify-0.2.7/src/guify/web/static/js/main.bf3c494e.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:17:20.534101 guify-0.2.7/src/guify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-05-03 10:17:20.000000 guify-0.2.7/src/guify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-03 10:17:20.000000 guify-0.2.7/src/guify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 10:17:20.000000 guify-0.2.7/src/guify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-03 10:17:20.000000 guify-0.2.7/src/guify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 10:17:20.000000 guify-0.2.7/src/guify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:18:18.935901 guify-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-03 18:17:05.000000 guify-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-03 18:17:05.000000 guify-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-03 18:18:18.935901 guify-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-03 18:17:05.000000 guify-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:18:18.931901 guify-0.2.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-03 18:17:05.000000 guify-0.2.8/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-03 18:17:05.000000 guify-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-03 18:18:18.935901 guify-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:18:18.931901 guify-0.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:18:18.931901 guify-0.2.8/src/guify/
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-03 18:17:05.000000 guify-0.2.8/src/guify/App.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-03 18:17:05.000000 guify-0.2.8/src/guify/BaseTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-03 18:17:05.000000 guify-0.2.8/src/guify/ConfigTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-03 18:17:05.000000 guify-0.2.8/src/guify/Monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-03 18:17:05.000000 guify-0.2.8/src/guify/TestPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-05-03 18:17:05.000000 guify-0.2.8/src/guify/TestWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-03 18:17:05.000000 guify-0.2.8/src/guify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-03 18:17:05.000000 guify-0.2.8/src/guify/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-03 18:17:05.000000 guify-0.2.8/src/guify/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:18:18.935901 guify-0.2.8/src/guify/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-03 18:18:11.000000 guify-0.2.8/src/guify/web/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-05-03 18:17:59.000000 guify-0.2.8/src/guify/web/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-03 18:18:12.000000 guify-0.2.8/src/guify/web/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-03 18:17:59.000000 guify-0.2.8/src/guify/web/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:18:18.931901 guify-0.2.8/src/guify/web/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:18:18.935901 guify-0.2.8/src/guify/web/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   144117 2023-05-03 18:18:11.000000 guify-0.2.8/src/guify/web/static/css/main.c779b13f.css
+-rw-r--r--   0 runner    (1001) docker     (123)   481735 2023-05-03 18:18:11.000000 guify-0.2.8/src/guify/web/static/css/main.c779b13f.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:18:18.935901 guify-0.2.8/src/guify/web/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   207756 2023-05-03 18:18:11.000000 guify-0.2.8/src/guify/web/static/js/main.bf3c494e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-03 18:18:11.000000 guify-0.2.8/src/guify/web/static/js/main.bf3c494e.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   660732 2023-05-03 18:18:11.000000 guify-0.2.8/src/guify/web/static/js/main.bf3c494e.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:18:18.935901 guify-0.2.8/src/guify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-03 18:18:18.000000 guify-0.2.8/src/guify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-03 18:18:18.000000 guify-0.2.8/src/guify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 18:18:18.000000 guify-0.2.8/src/guify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-03 18:18:18.000000 guify-0.2.8/src/guify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 18:18:18.000000 guify-0.2.8/src/guify.egg-info/top_level.txt
```

### Comparing `guify-0.2.7/LICENSE` & `guify-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `guify-0.2.7/PKG-INFO` & `guify-0.2.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guify
-Version: 0.2.7
+Version: 0.2.8
 Summary: A tool that will GUI-ify your functions
 Author: Michael Druyan
 Author-email: michael@druyan.net
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -23,39 +23,39 @@
 ```
 
 ```py
 # main.py
 import GUIfy from guify
 
 # Instantiate the app, variables are optional.
-# app_name is the title of the app shown on the top, equivalent to <title /> tag in HTML
-# report_dir is the directory where reports will be stored
-# report_prefix is the prefix of the report, if none, it will be 'report'
-# if set to 'serial_number', this will be requested in the gui.
-app = GUIfy(app_name='GUIfy', port=8080, report_dir=None, report_prefix=None) # default app_name is 'GUIfy'
+# - app_name is the title of the app shown on the top, equivalent to <title /> tag in HTML
+# - report_dir is the directory where reports will be stored if none reports are disabled.
+# - report_prefix // the name of the variable to take the prefix from, default is "report_*.txt"
+# - redirect_stdout // if True, will redirect stdout to the monitor, default is True
+app = GUIfy(app_name='GUIfy', port=8080, report_dir=None, report_prefix=None, redirect_stdout=True) # default app_name is 'GUIfy'
 
 # Register the function "test_1"
 # All variables are optional
 # name - the name of the "test" in the gui
 # priority - Sets the order of the tests, priority 0 will run before priority 1
 # description - the small text description under the test's name in the gui.
 @app.register(name='Test 1', priority=0, description='This is a test')
 # Define the test, each argument that "test_1"
 # requires will be automatically prompted for in the gui.
 # no arg will be requested twice.
 def test_1(example_arg):
     # app.monitor object represents the textarea on the right-hand side of the gui
-    # app.monitor.clear_text() - sets the text to empty string
-    app.monitor.clear_text()
+    # app.monitor.flush() - sets the text to empty string
+    app.monitor.flush()
 
     # app.monitor.set_text(text) - sets the text to whatever is passed to it
-    app.monitor.set_text('This is a test\n')
+    app.monitor.write('This is a test\n')
 
-    # app.monitor.append_text(text) - appends whatever passed to it to the textarea
-    app.monitor.append_text('This is a test2\n')
+    # print function will also print to the monitor
+    print('This is a test2\n')
 
     # app.prompt_user(prompt) - pops up a modal in the gui and asks user to click OK or cancel.
     # app.prompt_user will return True if user clicked OK and False if user clicked cancel
     result = app.prompt_user('This is a prompt') # True if user clicked OK, False if user clicked Cancel
 
     # app.config get something from config tab, acts similar to configparser
     # config stored in config.ini in the current working directory.
@@ -66,15 +66,15 @@
     # if function returns False then test considered as Failed
     return True
 
 
 # this test will be registered after test_1, because its priority arg is higher.
 @app.register(name='Test 2', priority=1, description='This is the second test.')
 def test_2(example_arg, second_arg):
-    app.monitor.clear_text()
+    app.monitor.flush()
 
 
 
 
 app.run()
 
 ```
@@ -82,16 +82,16 @@
 ---
 
 ### Monitor object
 
 app.monitor is the monitor object representing the preview window on right hand side of the GUI,
 
 - set_text(text: str) -> None // will set the text in the monitor to whatever passed in "text" argument
-- append_text(text: str) -> None // will append the next to the monitor
-- clear_text(text: str) -> None // will clear all text in the monitor
+- write(text: str) -> None // will append the next to the monitor, print() also works
+- flush(text: str) -> None // will clear all text in the monitor
 
 ---
 
 ## Config tab
 
 "app.config" is an object representing the config tab.
 All configurations are stored in config.ini.
@@ -123,9 +123,8 @@
 ## Building
 
 Theoretically its possible to build an executable with eel using the following:
 
 ```bash
 py -m eel index.py build --onefile --noconsole --name <whatever_u_want> --icon=public/favicon.ico
 ```
-
-Please not that this hasn't been tested yet.
+Please note that eel build hasn't been tested yet.
```

### Comparing `guify-0.2.7/README.md` & `guify-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `guify-0.2.7/docs/README.md` & `guify-0.2.8/docs/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -13,39 +13,39 @@
 ```
 
 ```py
 # main.py
 import GUIfy from guify
 
 # Instantiate the app, variables are optional.
-# app_name is the title of the app shown on the top, equivalent to <title /> tag in HTML
-# report_dir is the directory where reports will be stored
-# report_prefix is the prefix of the report, if none, it will be 'report'
-# if set to 'serial_number', this will be requested in the gui.
-app = GUIfy(app_name='GUIfy', port=8080, report_dir=None, report_prefix=None) # default app_name is 'GUIfy'
+# - app_name is the title of the app shown on the top, equivalent to <title /> tag in HTML
+# - report_dir is the directory where reports will be stored if none reports are disabled.
+# - report_prefix // the name of the variable to take the prefix from, default is "report_*.txt"
+# - redirect_stdout // if True, will redirect stdout to the monitor, default is True
+app = GUIfy(app_name='GUIfy', port=8080, report_dir=None, report_prefix=None, redirect_stdout=True) # default app_name is 'GUIfy'
 
 # Register the function "test_1"
 # All variables are optional
 # name - the name of the "test" in the gui
 # priority - Sets the order of the tests, priority 0 will run before priority 1
 # description - the small text description under the test's name in the gui.
 @app.register(name='Test 1', priority=0, description='This is a test')
 # Define the test, each argument that "test_1"
 # requires will be automatically prompted for in the gui.
 # no arg will be requested twice.
 def test_1(example_arg):
     # app.monitor object represents the textarea on the right-hand side of the gui
-    # app.monitor.clear_text() - sets the text to empty string
-    app.monitor.clear_text()
+    # app.monitor.flush() - sets the text to empty string
+    app.monitor.flush()
 
     # app.monitor.set_text(text) - sets the text to whatever is passed to it
-    app.monitor.set_text('This is a test\n')
+    app.monitor.write('This is a test\n')
 
-    # app.monitor.append_text(text) - appends whatever passed to it to the textarea
-    app.monitor.append_text('This is a test2\n')
+    # print function will also print to the monitor
+    print('This is a test2\n')
 
     # app.prompt_user(prompt) - pops up a modal in the gui and asks user to click OK or cancel.
     # app.prompt_user will return True if user clicked OK and False if user clicked cancel
     result = app.prompt_user('This is a prompt') # True if user clicked OK, False if user clicked Cancel
 
     # app.config get something from config tab, acts similar to configparser
     # config stored in config.ini in the current working directory.
@@ -56,15 +56,15 @@
     # if function returns False then test considered as Failed
     return True
 
 
 # this test will be registered after test_1, because its priority arg is higher.
 @app.register(name='Test 2', priority=1, description='This is the second test.')
 def test_2(example_arg, second_arg):
-    app.monitor.clear_text()
+    app.monitor.flush()
 
 
 
 
 app.run()
 
 ```
@@ -72,16 +72,16 @@
 ---
 
 ### Monitor object
 
 app.monitor is the monitor object representing the preview window on right hand side of the GUI,
 
 - set_text(text: str) -> None // will set the text in the monitor to whatever passed in "text" argument
-- append_text(text: str) -> None // will append the next to the monitor
-- clear_text(text: str) -> None // will clear all text in the monitor
+- write(text: str) -> None // will append the next to the monitor, print() also works
+- flush(text: str) -> None // will clear all text in the monitor
 
 ---
 
 ## Config tab
 
 "app.config" is an object representing the config tab.
 All configurations are stored in config.ini.
@@ -113,9 +113,8 @@
 ## Building
 
 Theoretically its possible to build an executable with eel using the following:
 
 ```bash
 py -m eel index.py build --onefile --noconsole --name <whatever_u_want> --icon=public/favicon.ico
 ```
-
-Please not that this hasn't been tested yet.
+Please note that eel build hasn't been tested yet.
```

### Comparing `guify-0.2.7/setup.cfg` & `guify-0.2.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = guify
-version = 0.2.7
+version = 0.2.8
 author = Michael Druyan
 author_email = michael@druyan.net
 description = A tool that will GUI-ify your functions
 long_description = file: docs/README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `guify-0.2.7/src/guify/App.py` & `guify-0.2.8/src/guify/App.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,32 +6,36 @@
 import sys
 import eel
 from pymsgbox import alert
 
 log = logging.getLogger("\tindex.py")
 worker = TestWorker()
 
+
 class GUIfy:
     # report_dir is the directory of the reports
-    
+
     # report_prefix is the prefix of the report file
     # report_prefix can be set to one of the arguments
     # that is required by registered functions. For example:
     # if a registered function requires argument name and age
     # then report_prefix can be set to 'name' or 'age'.
-    def __init__(self, app_name='GUIfy', port=8080, report_dir=None, report_prefix=None):
+    def __init__(self, app_name='GUIfy', port=8080, report_dir=None, report_prefix=None, redirect_stdout=True):
         self._port = port
         self._app_name = app_name
         eel.expose(self.app_name)
         worker._report_dir = report_dir
         worker._report_prefix = report_prefix
         self.worker = worker
         self.monitor = self.worker.monitor
         self.config = self.worker.config_tab
 
+        if redirect_stdout:
+            sys.stdout = self.monitor
+
     def app_name(self):
         return self._app_name
 
     def register(self, priority: int = None, name: str = None, description: str = None):
         def decorator(func):
             self.worker.pool.add(func, name,
                                  priority, description)
```

### Comparing `guify-0.2.7/src/guify/BaseTest.py` & `guify-0.2.8/src/guify/BaseTest.py`

 * *Files identical despite different names*

### Comparing `guify-0.2.7/src/guify/ConfigTab.py` & `guify-0.2.8/src/guify/ConfigTab.py`

 * *Files identical despite different names*

### Comparing `guify-0.2.7/src/guify/TestPool.py` & `guify-0.2.8/src/guify/TestPool.py`

 * *Files identical despite different names*

### Comparing `guify-0.2.7/src/guify/TestWorker.py` & `guify-0.2.8/src/guify/TestWorker.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .TestPool import TestPool
 from .BaseTest import BaseTest
 from threading import Thread, Event, Lock
 import logging
 from .constants import OK, CANCEL, WAITING_FOR_RUN, RUNNING_TEST, PENDING_USER_INPUT, DONE
 from .Monitor import Monitor
 from .ConfigTab import ConfigTab
+import traceback
 
 CFG_FILE_NAME = 'settings.ini'
 DEFAULT_REPORTS_FOLDER_NAME = 'reports'
 
 log = logging.getLogger("\tTestWorker")
 
 
@@ -73,15 +74,15 @@
         # returns the path to the reports folder
         # if no path is set, returns the default path
         # default path is 'reports' folder in the current working directory
         # path is set in settings.ini
         if self._report_dir is None:
             log.debug("No report directory set, report generation is off")
             return None
-        
+
         if os.path.isabs(self._report_dir):
             retval = self._report_dir
         else:
             retval = os.path.join(os.getcwd(), self._report_dir)
 
         self._create_report_folder(retval)
         return retval
@@ -96,25 +97,28 @@
         else:
             self._prompt = 'pass'
 
         self._save_report(report)
         self._wait_for_unpause()
         self._state = WAITING_FOR_RUN
         self.currently_running = None
-
+        self.pause.clear()
+        self._halt.clear()
         log.debug('"Restarting" thread')
         super().__init__(name='TestWorker')
+        self._lock.release()
 
     def set_prompt(self, message):
         self.pause.set()
         self._state = PENDING_USER_INPUT
         self._prompt = message
         return self._wait_for_response()
 
     def stop(self):
+        self.pause.clear()
         self._halt.set()
         self._lock.acquire()
         self.currently_running = None
 
     def answer_prompt(self, response):
         assert response in [
             OK, CANCEL], f"Gotten response other than '{OK}' or '{CANCEL}'"
@@ -156,18 +160,18 @@
 
             log.info(
                 f"Test: {test._name}\t Status:{'Pass' if result else 'Fail'}")
 
             return result
 
         except Exception as exc:
-            exc_str = f"Exception: {exc} in {test._name}"
-            log.error(exc_str)
 
-            self.stop()
+            exc_str = f"{exc.__class__.__name__}: {exc} in {test._name}"
+            log.error(exc_str)
+            print(traceback.format_exc())
 
             self.set_prompt(exc_str)
             return False
 
     def _save_report(self, report: dict):
         log.debug("Saving report")
         reports_path = self._get_reports_path()
@@ -221,25 +225,25 @@
 
         super().start()
 
     def _get_initial_report(self):
         return {key: None for key in self.queue}
 
     def run(self):
-        self.monitor.clear_text()
+        self.monitor.flush()
         self._halt.clear()
         report = self._get_initial_report()
         log.info("Starting Worker Thread")
         for test in self.pool:
             if self._halt.is_set():
                 break
             # Skip this iteration if test is not meant to run
             if test._name in self.queue:
                 self.queue.remove(test._name)
                 status = self._run_test(test)
 
                 report[test._name] = status
                 if status is False:
-                    self._halt.set()
+                    self.stop()
                     break
 
         self.finish_job(report)
```

### Comparing `guify-0.2.7/src/guify/__init__.py` & `guify-0.2.8/src/guify/__init__.py`

 * *Files identical despite different names*

### Comparing `guify-0.2.7/src/guify/web/favicon.ico` & `guify-0.2.8/src/guify/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `guify-0.2.7/src/guify/web/index.html` & `guify-0.2.8/src/guify/web/index.html`

 * *Files identical despite different names*

### Comparing `guify-0.2.7/src/guify/web/static/css/main.c779b13f.css` & `guify-0.2.8/src/guify/web/static/css/main.c779b13f.css`

 * *Files identical despite different names*

### Comparing `guify-0.2.7/src/guify/web/static/css/main.c779b13f.css.map` & `guify-0.2.8/src/guify/web/static/css/main.c779b13f.css.map`

 * *Files identical despite different names*

### Comparing `guify-0.2.7/src/guify/web/static/js/main.bf3c494e.js` & `guify-0.2.8/src/guify/web/static/js/main.bf3c494e.js`

 * *Files identical despite different names*

### Comparing `guify-0.2.7/src/guify/web/static/js/main.bf3c494e.js.LICENSE.txt` & `guify-0.2.8/src/guify/web/static/js/main.bf3c494e.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `guify-0.2.7/src/guify/web/static/js/main.bf3c494e.js.map` & `guify-0.2.8/src/guify/web/static/js/main.bf3c494e.js.map`

 * *Files identical despite different names*

### Comparing `guify-0.2.7/src/guify.egg-info/PKG-INFO` & `guify-0.2.8/src/guify.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guify
-Version: 0.2.7
+Version: 0.2.8
 Summary: A tool that will GUI-ify your functions
 Author: Michael Druyan
 Author-email: michael@druyan.net
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -23,39 +23,39 @@
 ```
 
 ```py
 # main.py
 import GUIfy from guify
 
 # Instantiate the app, variables are optional.
-# app_name is the title of the app shown on the top, equivalent to <title /> tag in HTML
-# report_dir is the directory where reports will be stored
-# report_prefix is the prefix of the report, if none, it will be 'report'
-# if set to 'serial_number', this will be requested in the gui.
-app = GUIfy(app_name='GUIfy', port=8080, report_dir=None, report_prefix=None) # default app_name is 'GUIfy'
+# - app_name is the title of the app shown on the top, equivalent to <title /> tag in HTML
+# - report_dir is the directory where reports will be stored if none reports are disabled.
+# - report_prefix // the name of the variable to take the prefix from, default is "report_*.txt"
+# - redirect_stdout // if True, will redirect stdout to the monitor, default is True
+app = GUIfy(app_name='GUIfy', port=8080, report_dir=None, report_prefix=None, redirect_stdout=True) # default app_name is 'GUIfy'
 
 # Register the function "test_1"
 # All variables are optional
 # name - the name of the "test" in the gui
 # priority - Sets the order of the tests, priority 0 will run before priority 1
 # description - the small text description under the test's name in the gui.
 @app.register(name='Test 1', priority=0, description='This is a test')
 # Define the test, each argument that "test_1"
 # requires will be automatically prompted for in the gui.
 # no arg will be requested twice.
 def test_1(example_arg):
     # app.monitor object represents the textarea on the right-hand side of the gui
-    # app.monitor.clear_text() - sets the text to empty string
-    app.monitor.clear_text()
+    # app.monitor.flush() - sets the text to empty string
+    app.monitor.flush()
 
     # app.monitor.set_text(text) - sets the text to whatever is passed to it
-    app.monitor.set_text('This is a test\n')
+    app.monitor.write('This is a test\n')
 
-    # app.monitor.append_text(text) - appends whatever passed to it to the textarea
-    app.monitor.append_text('This is a test2\n')
+    # print function will also print to the monitor
+    print('This is a test2\n')
 
     # app.prompt_user(prompt) - pops up a modal in the gui and asks user to click OK or cancel.
     # app.prompt_user will return True if user clicked OK and False if user clicked cancel
     result = app.prompt_user('This is a prompt') # True if user clicked OK, False if user clicked Cancel
 
     # app.config get something from config tab, acts similar to configparser
     # config stored in config.ini in the current working directory.
@@ -66,15 +66,15 @@
     # if function returns False then test considered as Failed
     return True
 
 
 # this test will be registered after test_1, because its priority arg is higher.
 @app.register(name='Test 2', priority=1, description='This is the second test.')
 def test_2(example_arg, second_arg):
-    app.monitor.clear_text()
+    app.monitor.flush()
 
 
 
 
 app.run()
 
 ```
@@ -82,16 +82,16 @@
 ---
 
 ### Monitor object
 
 app.monitor is the monitor object representing the preview window on right hand side of the GUI,
 
 - set_text(text: str) -> None // will set the text in the monitor to whatever passed in "text" argument
-- append_text(text: str) -> None // will append the next to the monitor
-- clear_text(text: str) -> None // will clear all text in the monitor
+- write(text: str) -> None // will append the next to the monitor, print() also works
+- flush(text: str) -> None // will clear all text in the monitor
 
 ---
 
 ## Config tab
 
 "app.config" is an object representing the config tab.
 All configurations are stored in config.ini.
@@ -123,9 +123,8 @@
 ## Building
 
 Theoretically its possible to build an executable with eel using the following:
 
 ```bash
 py -m eel index.py build --onefile --noconsole --name <whatever_u_want> --icon=public/favicon.ico
 ```
-
-Please not that this hasn't been tested yet.
+Please note that eel build hasn't been tested yet.
```

### Comparing `guify-0.2.7/src/guify.egg-info/SOURCES.txt` & `guify-0.2.8/src/guify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `guify-0.2.7/src/guify.egg-info/requires.txt` & `guify-0.2.8/src/guify.egg-info/requires.txt`

 * *Files identical despite different names*

