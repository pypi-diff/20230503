# Comparing `tmp/utilspggmdatalab-0.4.tar.gz` & `tmp/utilspggmdatalab-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilspggmdatalab-0.4.tar", last modified: Tue May  2 16:06:50 2023, max compression
+gzip compressed data, was "utilspggmdatalab-0.5.tar", last modified: Wed May  3 14:03:39 2023, max compression
```

## Comparing `utilspggmdatalab-0.4.tar` & `utilspggmdatalab-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 16:06:50.850913 utilspggmdatalab-0.4/
--rw-rw-rw-   0        0        0      811 2023-05-02 16:06:50.849912 utilspggmdatalab-0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-02 10:39:07.000000 utilspggmdatalab-0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-02 16:06:50.850913 utilspggmdatalab-0.4/setup.cfg
--rw-rw-rw-   0        0        0     1608 2023-05-02 16:04:47.000000 utilspggmdatalab-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:06:50.793909 utilspggmdatalab-0.4/utilspggmdatalab/
--rw-rw-rw-   0        0        0       31 2023-05-02 14:49:48.000000 utilspggmdatalab-0.4/utilspggmdatalab/__init__.py
--rw-rw-rw-   0        0        0     8105 2023-05-02 10:39:42.000000 utilspggmdatalab-0.4/utilspggmdatalab/utilspggmdatalab.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:06:50.848912 utilspggmdatalab-0.4/utilspggmdatalab.egg-info/
--rw-rw-rw-   0        0        0      811 2023-05-02 16:06:50.000000 utilspggmdatalab-0.4/utilspggmdatalab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-05-02 16:06:50.000000 utilspggmdatalab-0.4/utilspggmdatalab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 16:06:50.000000 utilspggmdatalab-0.4/utilspggmdatalab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      279 2023-05-02 16:06:50.000000 utilspggmdatalab-0.4/utilspggmdatalab.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-02 16:06:50.000000 utilspggmdatalab-0.4/utilspggmdatalab.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 14:03:39.326758 utilspggmdatalab-0.5/
+-rw-rw-rw-   0        0        0      861 2023-05-03 14:03:39.324758 utilspggmdatalab-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:39:07.000000 utilspggmdatalab-0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-03 14:03:39.326758 utilspggmdatalab-0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1176 2023-05-03 13:45:54.000000 utilspggmdatalab-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:03:39.309463 utilspggmdatalab-0.5/utilspggmdatalab/
+-rw-rw-rw-   0        0        0       31 2023-05-02 14:49:48.000000 utilspggmdatalab-0.5/utilspggmdatalab/__init__.py
+-rw-rw-rw-   0        0        0     8105 2023-05-02 10:39:42.000000 utilspggmdatalab-0.5/utilspggmdatalab/utilspggmdatalab.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:03:39.322760 utilspggmdatalab-0.5/utilspggmdatalab.egg-info/
+-rw-rw-rw-   0        0        0      861 2023-05-03 14:03:39.000000 utilspggmdatalab-0.5/utilspggmdatalab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-05-03 14:03:39.000000 utilspggmdatalab-0.5/utilspggmdatalab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 14:03:39.000000 utilspggmdatalab-0.5/utilspggmdatalab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-05-03 14:03:39.000000 utilspggmdatalab-0.5/utilspggmdatalab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-03 14:03:39.000000 utilspggmdatalab-0.5/utilspggmdatalab.egg-info/top_level.txt
```

### Comparing `utilspggmdatalab-0.4/PKG-INFO` & `utilspggmdatalab-0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: utilspggmdatalab
-Version: 0.4
+Version: 0.5
 Summary: A toolkit module for the Mimir app created in Innovation Data Lab
 Home-page: https://github.com/PGGM-Innovatie/utilspggmdatalab
 Author: Dominique Stoverink
 Author-email: dominique.stoverink@pggm.nl
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+
+UNKNOWN
+
```

### Comparing `utilspggmdatalab-0.4/utilspggmdatalab/utilspggmdatalab.py` & `utilspggmdatalab-0.5/utilspggmdatalab/utilspggmdatalab.py`

 * *Files identical despite different names*

### Comparing `utilspggmdatalab-0.4/utilspggmdatalab.egg-info/PKG-INFO` & `utilspggmdatalab-0.5/utilspggmdatalab.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: utilspggmdatalab
-Version: 0.4
+Version: 0.5
 Summary: A toolkit module for the Mimir app created in Innovation Data Lab
 Home-page: https://github.com/PGGM-Innovatie/utilspggmdatalab
 Author: Dominique Stoverink
 Author-email: dominique.stoverink@pggm.nl
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+
+UNKNOWN
+
```

