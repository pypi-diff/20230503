# Comparing `tmp/ts_app-0.9.0.tar.gz` & `tmp/ts_app-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ts_app-0.9.0.tar", last modified: Fri Aug 26 19:43:03 2022, max compression
+gzip compressed data, was "ts_app-0.9.1.tar", last modified: Wed May  3 12:50:13 2023, max compression
```

## Comparing `ts_app-0.9.0.tar` & `ts_app-0.9.1.tar`

### file list

```diff
@@ -1,38 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 19:43:03.119545 ts_app-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-08-26 19:42:51.000000 ts_app-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-26 19:42:51.000000 ts_app-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2470 2022-08-26 19:43:03.119545 ts_app-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-08-26 19:42:51.000000 ts_app-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-08-26 19:42:51.000000 ts_app-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-08-26 19:43:03.119545 ts_app-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 19:43:03.115544 ts_app-0.9.0/ts_app/
--rw-r--r--   0 runner    (1001) docker     (121)     1808 2022-08-26 19:42:51.000000 ts_app-0.9.0/ts_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-08-26 19:42:51.000000 ts_app-0.9.0/ts_app/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 19:43:03.119545 ts_app-0.9.0/ts_app/assets/
--rw-r--r--   0 runner    (1001) docker     (121)    49449 2022-08-26 19:42:51.000000 ts_app-0.9.0/ts_app/assets/background_large.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    36861 2022-08-26 19:42:51.000000 ts_app-0.9.0/ts_app/assets/background_small.jpg
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-08-26 19:42:51.000000 ts_app-0.9.0/ts_app/assets/dashboard_style.css
--rw-r--r--   0 runner    (1001) docker     (121)     3626 2022-08-26 19:42:51.000000 ts_app-0.9.0/ts_app/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)     2056 2022-08-26 19:42:51.000000 ts_app-0.9.0/ts_app/assets/glossary.json
--rw-r--r--   0 runner    (1001) docker     (121)    15266 2022-08-26 19:42:51.000000 ts_app-0.9.0/ts_app/assets/ts.svg
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-08-26 19:42:51.000000 ts_app-0.9.0/ts_app/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 19:43:03.119545 ts_app-0.9.0/ts_app/components/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-26 19:42:51.000000 ts_app-0.9.0/ts_app/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6404 2022-08-26 19:42:51.000000 ts_app-0.9.0/ts_app/components/modelling.py
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-08-26 19:42:51.000000 ts_app-0.9.0/ts_app/dash_app.py
--rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-08-26 19:42:51.000000 ts_app-0.9.0/ts_app/file_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 19:43:03.119545 ts_app-0.9.0/ts_app/pages/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-26 19:42:51.000000 ts_app-0.9.0/ts_app/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-08-26 19:42:51.000000 ts_app-0.9.0/ts_app/pages/glossary.py
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-08-26 19:42:51.000000 ts_app-0.9.0/ts_app/pages/home_page.py
--rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-08-26 19:42:51.000000 ts_app-0.9.0/ts_app/pages/sample.py
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 19:42:51.000000 ts_app-0.9.0/ts_app/pages/upload.py
--rw-r--r--   0 runner    (1001) docker     (121)     3681 2022-08-26 19:42:51.000000 ts_app-0.9.0/ts_app/plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)     1980 2022-08-26 19:42:51.000000 ts_app-0.9.0/ts_app/ts_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 19:43:03.115544 ts_app-0.9.0/ts_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2470 2022-08-26 19:43:03.000000 ts_app-0.9.0/ts_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-08-26 19:43:03.000000 ts_app-0.9.0/ts_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 19:43:03.000000 ts_app-0.9.0/ts_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-08-26 19:43:03.000000 ts_app-0.9.0/ts_app.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-08-26 19:43:03.000000 ts_app-0.9.0/ts_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-26 19:43:03.000000 ts_app-0.9.0/ts_app.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:50:13.499126 ts_app-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-03 12:49:59.000000 ts_app-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 12:49:59.000000 ts_app-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-03 12:50:13.499126 ts_app-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-03 12:49:59.000000 ts_app-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-03 12:49:59.000000 ts_app-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-03 12:50:13.499126 ts_app-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:50:13.491126 ts_app-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-03 12:49:59.000000 ts_app-0.9.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-03 12:49:59.000000 ts_app-0.9.1/tests/test_ts_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-03 12:49:59.000000 ts_app-0.9.1/tests/test_upload_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:50:13.495126 ts_app-0.9.1/ts_app/
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-03 12:49:59.000000 ts_app-0.9.1/ts_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-03 12:49:59.000000 ts_app-0.9.1/ts_app/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:50:13.499126 ts_app-0.9.1/ts_app/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    49449 2023-05-03 12:49:59.000000 ts_app-0.9.1/ts_app/assets/background_large.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    36861 2023-05-03 12:49:59.000000 ts_app-0.9.1/ts_app/assets/background_small.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-03 12:49:59.000000 ts_app-0.9.1/ts_app/assets/dashboard_style.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-03 12:49:59.000000 ts_app-0.9.1/ts_app/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-03 12:49:59.000000 ts_app-0.9.1/ts_app/assets/glossary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15266 2023-05-03 12:49:59.000000 ts_app-0.9.1/ts_app/assets/ts.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-03 12:49:59.000000 ts_app-0.9.1/ts_app/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:50:13.499126 ts_app-0.9.1/ts_app/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 12:49:59.000000 ts_app-0.9.1/ts_app/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-05-03 12:49:59.000000 ts_app-0.9.1/ts_app/components/modelling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-03 12:49:59.000000 ts_app-0.9.1/ts_app/dash_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-03 12:49:59.000000 ts_app-0.9.1/ts_app/file_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:50:13.499126 ts_app-0.9.1/ts_app/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 12:49:59.000000 ts_app-0.9.1/ts_app/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-03 12:49:59.000000 ts_app-0.9.1/ts_app/pages/glossary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-03 12:49:59.000000 ts_app-0.9.1/ts_app/pages/home_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-03 12:49:59.000000 ts_app-0.9.1/ts_app/pages/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-03 12:49:59.000000 ts_app-0.9.1/ts_app/pages/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-03 12:49:59.000000 ts_app-0.9.1/ts_app/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-03 12:49:59.000000 ts_app-0.9.1/ts_app/ts_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:50:13.495126 ts_app-0.9.1/ts_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-03 12:50:13.000000 ts_app-0.9.1/ts_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-03 12:50:13.000000 ts_app-0.9.1/ts_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:50:13.000000 ts_app-0.9.1/ts_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-03 12:50:13.000000 ts_app-0.9.1/ts_app.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-03 12:50:13.000000 ts_app-0.9.1/ts_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 12:50:13.000000 ts_app-0.9.1/ts_app.egg-info/top_level.txt
```

### Comparing `ts_app-0.9.0/LICENSE` & `ts_app-0.9.1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 Abwao
+Copyright (c) 2020 - 2023 Abwao
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ts_app-0.9.0/PKG-INFO` & `ts_app-0.9.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts_app
-Version: 0.9.0
+Version: 0.9.1
 Summary: A simple dashboard application for interactively fitting ARIMA models.
 Home-page: https://github.com/Tim-Abwao/time-series-app
 Author: Abwao
 Author-email: abwaomusungu@gmail.com
 License: MIT
 Keywords: time_series dashboard ARIMA
 Classifier: Development Status :: 4 - Beta
@@ -20,32 +20,28 @@
 
 A dashboard application to help learn a little about, and apply *[Time Series][wiki_time_series] analysis* & *forecasting* concepts.
 
 You can create a sample, or upload a file, and interactively fit a time series model on it.
 
 The dashboard is built with [Dash][dash], and the time series models are fitted using [Statsmodels][statsmodels].
 
-You can [try it out here][live-link].
+You can [try it out here][live-link], courtesy of [Render][render].
 
-[![screencast of the app](https://raw.githubusercontent.com/Tim-Abwao/time-series-app/master/screencast.gif)][live-link]
+>**NOTE:** Free-hosted apps on *Render* might take a while to load since they are shut down when not in use.
+
+![screencast of the app](https://raw.githubusercontent.com/Tim-Abwao/time-series-app/master/screencast.gif)
 
 ## Installation
 
-The easiest way to install the app is from [PyPI][pypi]:
+The easiest way to get the app is from [PyPI][pypi]:
 
 ```bash
 pip install ts-app
 ```
 
-You could also install it directly from the **GitHub** repository:
-
-```bash
-pip install https://github.com/tim-abwao/time-series-app/archive/main.tar.gz
-```
-
 ## Basic Usage
 
 The command `ts_app` launches the app:
 
 ```bash
 $ ts_app -h
 usage: ts_app [-h] [-p PORT] [--host HOST] [--no-browser]
@@ -65,11 +61,12 @@
 >>> import ts_app
 >>> ts_app.run_app()
 ```
 
 Afterwards, press `CTRL` + `C` to stop the server.
 
 [wiki_time_series]: https://en.wikipedia.org/wiki/Time_series
-[live-link]: https://time-series-app.herokuapp.com
+[live-link]: https://time-series-app.onrender.com
 [dash]: https://dash.plotly.com/
+[render]: https://render.com/
 [statsmodels]: https://www.statsmodels.org/stable/index.html
 [pypi]:  https://pypi.org/project/ts-app/
```

### Comparing `ts_app-0.9.0/README.md` & `ts_app-0.9.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -5,32 +5,28 @@
 
 A dashboard application to help learn a little about, and apply *[Time Series][wiki_time_series] analysis* & *forecasting* concepts.
 
 You can create a sample, or upload a file, and interactively fit a time series model on it.
 
 The dashboard is built with [Dash][dash], and the time series models are fitted using [Statsmodels][statsmodels].
 
-You can [try it out here][live-link].
+You can [try it out here][live-link], courtesy of [Render][render].
 
-[![screencast of the app](https://raw.githubusercontent.com/Tim-Abwao/time-series-app/master/screencast.gif)][live-link]
+>**NOTE:** Free-hosted apps on *Render* might take a while to load since they are shut down when not in use.
+
+![screencast of the app](https://raw.githubusercontent.com/Tim-Abwao/time-series-app/master/screencast.gif)
 
 ## Installation
 
-The easiest way to install the app is from [PyPI][pypi]:
+The easiest way to get the app is from [PyPI][pypi]:
 
 ```bash
 pip install ts-app
 ```
 
-You could also install it directly from the **GitHub** repository:
-
-```bash
-pip install https://github.com/tim-abwao/time-series-app/archive/main.tar.gz
-```
-
 ## Basic Usage
 
 The command `ts_app` launches the app:
 
 ```bash
 $ ts_app -h
 usage: ts_app [-h] [-p PORT] [--host HOST] [--no-browser]
@@ -50,11 +46,12 @@
 >>> import ts_app
 >>> ts_app.run_app()
 ```
 
 Afterwards, press `CTRL` + `C` to stop the server.
 
 [wiki_time_series]: https://en.wikipedia.org/wiki/Time_series
-[live-link]: https://time-series-app.herokuapp.com
+[live-link]: https://time-series-app.onrender.com
 [dash]: https://dash.plotly.com/
+[render]: https://render.com/
 [statsmodels]: https://www.statsmodels.org/stable/index.html
 [pypi]:  https://pypi.org/project/ts-app/
```

### Comparing `ts_app-0.9.0/setup.cfg` & `ts_app-0.9.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 license = MIT
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python :: 3.9
 
 [options]
 install_requires = 
-	dash>=2.6.1
-	openpyxl>=3.0.10
-	statsmodels>=0.13.2
+	dash>=2.9.3
+	openpyxl>=3.1.2
+	statsmodels>=0.13.5
 	waitress>=2.1.2
 include_package_data = True
 packages = find:
 python_requires = >=3.8
 
 [options.entry_points]
 console_scripts =
```

### Comparing `ts_app-0.9.0/ts_app/__init__.py` & `ts_app-0.9.1/ts_app/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import webbrowser
 
 import waitress
 
 from ts_app.cli import process_cli_args
 from ts_app.dash_app import app
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 logging.basicConfig(level="INFO")
 
 # Suppress benign queue warnings
 logging.getLogger("waitress.queue").setLevel("ERROR")
```

### Comparing `ts_app-0.9.0/ts_app/assets/background_large.jpg` & `ts_app-0.9.1/ts_app/assets/background_large.jpg`

 * *Files identical despite different names*

### Comparing `ts_app-0.9.0/ts_app/assets/background_small.jpg` & `ts_app-0.9.1/ts_app/assets/background_small.jpg`

 * *Files identical despite different names*

### Comparing `ts_app-0.9.0/ts_app/assets/dashboard_style.css` & `ts_app-0.9.1/ts_app/assets/dashboard_style.css`

 * *Files identical despite different names*

### Comparing `ts_app-0.9.0/ts_app/assets/favicon.ico` & `ts_app-0.9.1/ts_app/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `ts_app-0.9.0/ts_app/assets/glossary.json` & `ts_app-0.9.1/ts_app/assets/glossary.json`

 * *Files identical despite different names*

### Comparing `ts_app-0.9.0/ts_app/assets/ts.svg` & `ts_app-0.9.1/ts_app/assets/ts.svg`

 * *Files identical despite different names*

### Comparing `ts_app-0.9.0/ts_app/cli.py` & `ts_app-0.9.1/ts_app/cli.py`

 * *Files identical despite different names*

### Comparing `ts_app-0.9.0/ts_app/components/modelling.py` & `ts_app-0.9.1/ts_app/components/modelling.py`

 * *Files identical despite different names*

### Comparing `ts_app-0.9.0/ts_app/file_upload.py` & `ts_app-0.9.1/ts_app/file_upload.py`

 * *Files identical despite different names*

### Comparing `ts_app-0.9.0/ts_app/pages/glossary.py` & `ts_app-0.9.1/ts_app/pages/glossary.py`

 * *Files identical despite different names*

### Comparing `ts_app-0.9.0/ts_app/pages/home_page.py` & `ts_app-0.9.1/ts_app/pages/home_page.py`

 * *Files identical despite different names*

### Comparing `ts_app-0.9.0/ts_app/pages/sample.py` & `ts_app-0.9.1/ts_app/pages/sample.py`

 * *Files identical despite different names*

### Comparing `ts_app-0.9.0/ts_app/pages/upload.py` & `ts_app-0.9.1/ts_app/pages/upload.py`

 * *Files identical despite different names*

### Comparing `ts_app-0.9.0/ts_app/plotting.py` & `ts_app-0.9.1/ts_app/plotting.py`

 * *Files identical despite different names*

### Comparing `ts_app-0.9.0/ts_app/ts_functions.py` & `ts_app-0.9.1/ts_app/ts_functions.py`

 * *Files identical despite different names*

### Comparing `ts_app-0.9.0/ts_app.egg-info/PKG-INFO` & `ts_app-0.9.1/ts_app.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-app
-Version: 0.9.0
+Version: 0.9.1
 Summary: A simple dashboard application for interactively fitting ARIMA models.
 Home-page: https://github.com/Tim-Abwao/time-series-app
 Author: Abwao
 Author-email: abwaomusungu@gmail.com
 License: MIT
 Keywords: time_series dashboard ARIMA
 Classifier: Development Status :: 4 - Beta
@@ -20,32 +20,28 @@
 
 A dashboard application to help learn a little about, and apply *[Time Series][wiki_time_series] analysis* & *forecasting* concepts.
 
 You can create a sample, or upload a file, and interactively fit a time series model on it.
 
 The dashboard is built with [Dash][dash], and the time series models are fitted using [Statsmodels][statsmodels].
 
-You can [try it out here][live-link].
+You can [try it out here][live-link], courtesy of [Render][render].
 
-[![screencast of the app](https://raw.githubusercontent.com/Tim-Abwao/time-series-app/master/screencast.gif)][live-link]
+>**NOTE:** Free-hosted apps on *Render* might take a while to load since they are shut down when not in use.
+
+![screencast of the app](https://raw.githubusercontent.com/Tim-Abwao/time-series-app/master/screencast.gif)
 
 ## Installation
 
-The easiest way to install the app is from [PyPI][pypi]:
+The easiest way to get the app is from [PyPI][pypi]:
 
 ```bash
 pip install ts-app
 ```
 
-You could also install it directly from the **GitHub** repository:
-
-```bash
-pip install https://github.com/tim-abwao/time-series-app/archive/main.tar.gz
-```
-
 ## Basic Usage
 
 The command `ts_app` launches the app:
 
 ```bash
 $ ts_app -h
 usage: ts_app [-h] [-p PORT] [--host HOST] [--no-browser]
@@ -65,11 +61,12 @@
 >>> import ts_app
 >>> ts_app.run_app()
 ```
 
 Afterwards, press `CTRL` + `C` to stop the server.
 
 [wiki_time_series]: https://en.wikipedia.org/wiki/Time_series
-[live-link]: https://time-series-app.herokuapp.com
+[live-link]: https://time-series-app.onrender.com
 [dash]: https://dash.plotly.com/
+[render]: https://render.com/
 [statsmodels]: https://www.statsmodels.org/stable/index.html
 [pypi]:  https://pypi.org/project/ts-app/
```

