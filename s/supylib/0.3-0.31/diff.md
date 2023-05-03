# Comparing `tmp/supylib-0.3.tar.gz` & `tmp/supylib-0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ak/projects/supylib/dist/tmph3vqsvnl/supylib-0.3.tar", last modified: Wed May  3 16:52:39 2023, max compression
+gzip compressed data, was "/home/ak/projects/supylib/dist/tmp66_2pt52/supylib-0.31.tar", last modified: Wed May  3 17:06:52 2023, max compression
```

## Comparing `supylib-0.3.tar` & `supylib-0.31.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 ak        (1000) ak        (1000)        0 2023-05-03 16:52:39.000000 supylib-0.3/
--rw-rw-r--   0 ak        (1000) ak        (1000)     1118 2022-03-09 09:38:11.000000 supylib-0.3/LICENSE
--rw-r--r--   0 ak        (1000) ak        (1000)     1210 2023-05-03 15:06:47.000000 supylib-0.3/README.md
-drwxrwxr-x   0 ak        (1000) ak        (1000)        0 2023-05-03 16:52:39.000000 supylib-0.3/python/
-drwxrwxr-x   0 ak        (1000) ak        (1000)        0 2023-05-03 16:52:39.000000 supylib-0.3/python/supylib.egg-info/
--rw-rw-r--   0 ak        (1000) ak        (1000)        5 2023-05-03 16:52:39.000000 supylib-0.3/python/supylib.egg-info/top_level.txt
--rw-rw-r--   0 ak        (1000) ak        (1000)        1 2023-05-03 16:52:39.000000 supylib-0.3/python/supylib.egg-info/dependency_links.txt
--rw-rw-r--   0 ak        (1000) ak        (1000)      671 2023-05-03 16:52:39.000000 supylib-0.3/python/supylib.egg-info/SOURCES.txt
--rw-rw-r--   0 ak        (1000) ak        (1000)     1823 2023-05-03 16:52:39.000000 supylib-0.3/python/supylib.egg-info/PKG-INFO
-drwxrwxr-x   0 ak        (1000) ak        (1000)        0 2023-05-03 16:52:39.000000 supylib-0.3/python/supy/
--rw-r--r--   0 ak        (1000) ak        (1000)    12807 2019-02-28 09:55:09.000000 supylib-0.3/python/supy/forms.py
--rw-rw-r--   0 ak        (1000) ak        (1000)   170861 2023-05-03 16:18:00.000000 supylib-0.3/python/supy/signal.py
--rw-r--r--   0 ak        (1000) ak        (1000)     6868 2022-09-08 14:57:35.000000 supylib-0.3/python/supy/guimaker3.py
--rw-r--r--   0 ak        (1000) ak        (1000)    40317 2022-03-09 08:59:15.000000 supylib-0.3/python/supy/sqltableeditor.py
--rw-r--r--   0 ak        (1000) ak        (1000)     7965 2022-03-09 08:57:33.000000 supylib-0.3/python/supy/multibase.py
--rw-r--r--   0 ak        (1000) ak        (1000)     6871 2019-02-28 09:56:23.000000 supylib-0.3/python/supy/guimaker.py
--rw-r--r--   0 ak        (1000) ak        (1000)    17745 2022-03-09 08:58:19.000000 supylib-0.3/python/supy/sqldatabase_inputmask.py
--rw-r--r--   0 ak        (1000) ak        (1000)    20272 2022-03-09 08:54:20.000000 supylib-0.3/python/supy/database_inputmask3.py
--rw-r--r--   0 ak        (1000) ak        (1000)    20266 2022-03-09 08:55:21.000000 supylib-0.3/python/supy/database_inputmask.py
--rw-r--r--   0 ak        (1000) ak        (1000)    19500 2022-03-09 08:55:47.000000 supylib-0.3/python/supy/database.py
--rw-r--r--   0 ak        (1000) ak        (1000)    31946 2022-03-09 09:01:33.000000 supylib-0.3/python/supy/widgets.py
--rw-r--r--   0 ak        (1000) ak        (1000)     5419 2022-03-09 08:57:58.000000 supylib-0.3/python/supy/serialize.py
--rw-r--r--   0 ak        (1000) ak        (1000)   106175 2022-03-09 09:00:49.000000 supylib-0.3/python/supy/sqlforms.py
--rw-r--r--   0 ak        (1000) ak        (1000)    42485 2022-03-09 08:56:45.000000 supylib-0.3/python/supy/forms3.py
--rw-rw-r--   0 ak        (1000) ak        (1000)       22 2022-11-02 18:18:03.000000 supylib-0.3/python/supy/__init__.py
--rw-r--r--   0 ak        (1000) ak        (1000)    30059 2022-03-09 08:58:51.000000 supylib-0.3/python/supy/sqldatabase.py
--rw-r--r--   0 ak        (1000) ak        (1000)     5226 2022-03-09 09:01:13.000000 supylib-0.3/python/supy/utilities.py
--rw-r--r--   0 ak        (1000) ak        (1000)    76826 2023-04-14 09:28:16.000000 supylib-0.3/python/supy/computervision.py
--rw-rw-r--   0 ak        (1000) ak        (1000)      707 2023-05-03 16:52:39.000000 supylib-0.3/setup.cfg
--rw-rw-r--   0 ak        (1000) ak        (1000)      104 2022-03-09 09:36:04.000000 supylib-0.3/pyproject.toml
--rw-rw-r--   0 ak        (1000) ak        (1000)     1823 2023-05-03 16:52:39.000000 supylib-0.3/PKG-INFO
+drwxrwxr-x   0 ak        (1000) ak        (1000)        0 2023-05-03 17:06:52.000000 supylib-0.31/
+-rw-rw-r--   0 ak        (1000) ak        (1000)     1118 2022-03-09 09:38:11.000000 supylib-0.31/LICENSE
+-rw-r--r--   0 ak        (1000) ak        (1000)     1211 2023-05-03 17:05:22.000000 supylib-0.31/README.md
+drwxrwxr-x   0 ak        (1000) ak        (1000)        0 2023-05-03 17:06:52.000000 supylib-0.31/python/
+drwxrwxr-x   0 ak        (1000) ak        (1000)        0 2023-05-03 17:06:52.000000 supylib-0.31/python/supylib.egg-info/
+-rw-rw-r--   0 ak        (1000) ak        (1000)        5 2023-05-03 17:06:52.000000 supylib-0.31/python/supylib.egg-info/top_level.txt
+-rw-rw-r--   0 ak        (1000) ak        (1000)        1 2023-05-03 17:06:52.000000 supylib-0.31/python/supylib.egg-info/dependency_links.txt
+-rw-rw-r--   0 ak        (1000) ak        (1000)      671 2023-05-03 17:06:52.000000 supylib-0.31/python/supylib.egg-info/SOURCES.txt
+-rw-rw-r--   0 ak        (1000) ak        (1000)     1825 2023-05-03 17:06:52.000000 supylib-0.31/python/supylib.egg-info/PKG-INFO
+drwxrwxr-x   0 ak        (1000) ak        (1000)        0 2023-05-03 17:06:52.000000 supylib-0.31/python/supy/
+-rw-r--r--   0 ak        (1000) ak        (1000)    12807 2019-02-28 09:55:09.000000 supylib-0.31/python/supy/forms.py
+-rw-rw-r--   0 ak        (1000) ak        (1000)   170861 2023-05-03 16:18:00.000000 supylib-0.31/python/supy/signal.py
+-rw-r--r--   0 ak        (1000) ak        (1000)     6868 2022-09-08 14:57:35.000000 supylib-0.31/python/supy/guimaker3.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    40317 2022-03-09 08:59:15.000000 supylib-0.31/python/supy/sqltableeditor.py
+-rw-r--r--   0 ak        (1000) ak        (1000)     7965 2022-03-09 08:57:33.000000 supylib-0.31/python/supy/multibase.py
+-rw-r--r--   0 ak        (1000) ak        (1000)     6871 2019-02-28 09:56:23.000000 supylib-0.31/python/supy/guimaker.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    17745 2022-03-09 08:58:19.000000 supylib-0.31/python/supy/sqldatabase_inputmask.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    20272 2022-03-09 08:54:20.000000 supylib-0.31/python/supy/database_inputmask3.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    20266 2022-03-09 08:55:21.000000 supylib-0.31/python/supy/database_inputmask.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    19500 2022-03-09 08:55:47.000000 supylib-0.31/python/supy/database.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    31946 2022-03-09 09:01:33.000000 supylib-0.31/python/supy/widgets.py
+-rw-r--r--   0 ak        (1000) ak        (1000)     5419 2022-03-09 08:57:58.000000 supylib-0.31/python/supy/serialize.py
+-rw-r--r--   0 ak        (1000) ak        (1000)   106175 2022-03-09 09:00:49.000000 supylib-0.31/python/supy/sqlforms.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    42485 2022-03-09 08:56:45.000000 supylib-0.31/python/supy/forms3.py
+-rw-rw-r--   0 ak        (1000) ak        (1000)       22 2023-05-03 17:03:01.000000 supylib-0.31/python/supy/__init__.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    30059 2022-03-09 08:58:51.000000 supylib-0.31/python/supy/sqldatabase.py
+-rw-r--r--   0 ak        (1000) ak        (1000)     5226 2022-03-09 09:01:13.000000 supylib-0.31/python/supy/utilities.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    76826 2023-04-14 09:28:16.000000 supylib-0.31/python/supy/computervision.py
+-rw-rw-r--   0 ak        (1000) ak        (1000)      708 2023-05-03 17:06:52.000000 supylib-0.31/setup.cfg
+-rw-rw-r--   0 ak        (1000) ak        (1000)      104 2022-03-09 09:36:04.000000 supylib-0.31/pyproject.toml
+-rw-rw-r--   0 ak        (1000) ak        (1000)     1825 2023-05-03 17:06:52.000000 supylib-0.31/PKG-INFO
```

### Comparing `supylib-0.3/LICENSE` & `supylib-0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `supylib-0.3/README.md` & `supylib-0.31/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-supylib 0.3
+supylib 0.31
 -------------------------
 Eine Python-basierte Utility-Bibliothek für Datenbanken, Computer Vision, Signalverarbeitung und Machine Learning
 (c) Andreas Knoblauch, HS Albstadt-Sigmaringen, 2015-2023
 
 Aktivierung/Sichtbarkeit
 -------------------------
 Der folgende Shell-Befehl macht das suplib/python Verzeichnis global sichtbar,
```

### Comparing `supylib-0.3/python/supylib.egg-info/SOURCES.txt` & `supylib-0.31/python/supylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `supylib-0.3/python/supylib.egg-info/PKG-INFO` & `supylib-0.31/python/supylib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: supylib
-Version: 0.3
+Version: 0.31
 Summary: A Python-based utility library for databases, computer vision, signal processing, and machine learning
 Home-page: https://github.com/aknoblauch/supylib
 Author: Andreas Knoblauch
 Author-email: knoblauch@hs-albsig.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/aknoblauch/supylib/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-supylib 0.3
+supylib 0.31
 -------------------------
 Eine Python-basierte Utility-Bibliothek für Datenbanken, Computer Vision, Signalverarbeitung und Machine Learning
 (c) Andreas Knoblauch, HS Albstadt-Sigmaringen, 2015-2023
 
 Aktivierung/Sichtbarkeit
 -------------------------
 Der folgende Shell-Befehl macht das suplib/python Verzeichnis global sichtbar,
```

### Comparing `supylib-0.3/python/supy/forms.py` & `supylib-0.31/python/supy/forms.py`

 * *Files identical despite different names*

### Comparing `supylib-0.3/python/supy/signal.py` & `supylib-0.31/python/supy/signal.py`

 * *Files identical despite different names*

### Comparing `supylib-0.3/python/supy/guimaker3.py` & `supylib-0.31/python/supy/guimaker3.py`

 * *Files identical despite different names*

### Comparing `supylib-0.3/python/supy/sqltableeditor.py` & `supylib-0.31/python/supy/sqltableeditor.py`

 * *Files identical despite different names*

### Comparing `supylib-0.3/python/supy/multibase.py` & `supylib-0.31/python/supy/multibase.py`

 * *Files identical despite different names*

### Comparing `supylib-0.3/python/supy/guimaker.py` & `supylib-0.31/python/supy/guimaker.py`

 * *Files identical despite different names*

### Comparing `supylib-0.3/python/supy/sqldatabase_inputmask.py` & `supylib-0.31/python/supy/sqldatabase_inputmask.py`

 * *Files identical despite different names*

### Comparing `supylib-0.3/python/supy/database_inputmask3.py` & `supylib-0.31/python/supy/database_inputmask3.py`

 * *Files identical despite different names*

### Comparing `supylib-0.3/python/supy/database_inputmask.py` & `supylib-0.31/python/supy/database_inputmask.py`

 * *Files identical despite different names*

### Comparing `supylib-0.3/python/supy/database.py` & `supylib-0.31/python/supy/database.py`

 * *Files identical despite different names*

### Comparing `supylib-0.3/python/supy/widgets.py` & `supylib-0.31/python/supy/widgets.py`

 * *Files identical despite different names*

### Comparing `supylib-0.3/python/supy/serialize.py` & `supylib-0.31/python/supy/serialize.py`

 * *Files identical despite different names*

### Comparing `supylib-0.3/python/supy/sqlforms.py` & `supylib-0.31/python/supy/sqlforms.py`

 * *Files identical despite different names*

### Comparing `supylib-0.3/python/supy/forms3.py` & `supylib-0.31/python/supy/forms3.py`

 * *Files identical despite different names*

### Comparing `supylib-0.3/python/supy/sqldatabase.py` & `supylib-0.31/python/supy/sqldatabase.py`

 * *Files identical despite different names*

### Comparing `supylib-0.3/python/supy/utilities.py` & `supylib-0.31/python/supy/utilities.py`

 * *Files identical despite different names*

### Comparing `supylib-0.3/python/supy/computervision.py` & `supylib-0.31/python/supy/computervision.py`

 * *Files identical despite different names*

### Comparing `supylib-0.3/setup.cfg` & `supylib-0.31/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = supylib
-version = 0.3
+version = 0.31
 author = Andreas Knoblauch
 author_email = knoblauch@hs-albsig.de
 description = A Python-based utility library for databases, computer vision, signal processing, and machine learning
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/aknoblauch/supylib
 project_urls =
```

### Comparing `supylib-0.3/PKG-INFO` & `supylib-0.31/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: supylib
-Version: 0.3
+Version: 0.31
 Summary: A Python-based utility library for databases, computer vision, signal processing, and machine learning
 Home-page: https://github.com/aknoblauch/supylib
 Author: Andreas Knoblauch
 Author-email: knoblauch@hs-albsig.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/aknoblauch/supylib/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-supylib 0.3
+supylib 0.31
 -------------------------
 Eine Python-basierte Utility-Bibliothek für Datenbanken, Computer Vision, Signalverarbeitung und Machine Learning
 (c) Andreas Knoblauch, HS Albstadt-Sigmaringen, 2015-2023
 
 Aktivierung/Sichtbarkeit
 -------------------------
 Der folgende Shell-Befehl macht das suplib/python Verzeichnis global sichtbar,
```

