# Comparing `tmp/leclerc-0.1.1.tar.gz` & `tmp/leclerc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leclerc-0.1.1.tar", last modified: Wed May  3 02:26:01 2023, max compression
+gzip compressed data, was "leclerc-0.1.2.tar", last modified: Wed May  3 02:39:36 2023, max compression
```

## Comparing `leclerc-0.1.1.tar` & `leclerc-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 hoshang    (501) staff       (20)        0 2023-05-03 02:26:01.107084 leclerc-0.1.1/
--rw-r--r--   0 hoshang    (501) staff       (20)     2055 2023-05-03 02:26:01.106707 leclerc-0.1.1/PKG-INFO
--rw-r--r--   0 hoshang    (501) staff       (20)     1523 2023-03-06 04:34:34.000000 leclerc-0.1.1/README
-drwxr-xr-x   0 hoshang    (501) staff       (20)        0 2023-05-03 02:26:01.104049 leclerc-0.1.1/leclerc/
--rw-r--r--   0 hoshang    (501) staff       (20)       22 2023-02-28 11:47:07.000000 leclerc-0.1.1/leclerc/__init__.py
--rw-r--r--   0 hoshang    (501) staff       (20)     3310 2023-05-03 02:23:05.000000 leclerc-0.1.1/leclerc/monte_databricks.py
--rw-r--r--   0 hoshang    (501) staff       (20)     3175 2023-05-03 02:22:46.000000 leclerc-0.1.1/leclerc/montecarlinator.py
--rw-r--r--   0 hoshang    (501) staff       (20)     3485 2023-02-28 11:51:15.000000 leclerc-0.1.1/leclerc/pert.py
-drwxr-xr-x   0 hoshang    (501) staff       (20)        0 2023-05-03 02:26:01.106205 leclerc-0.1.1/leclerc.egg-info/
--rw-r--r--   0 hoshang    (501) staff       (20)     2055 2023-05-03 02:26:01.000000 leclerc-0.1.1/leclerc.egg-info/PKG-INFO
--rw-r--r--   0 hoshang    (501) staff       (20)      245 2023-05-03 02:26:01.000000 leclerc-0.1.1/leclerc.egg-info/SOURCES.txt
--rw-r--r--   0 hoshang    (501) staff       (20)        1 2023-05-03 02:26:01.000000 leclerc-0.1.1/leclerc.egg-info/dependency_links.txt
--rw-r--r--   0 hoshang    (501) staff       (20)        8 2023-05-03 02:26:01.000000 leclerc-0.1.1/leclerc.egg-info/top_level.txt
--rw-r--r--   0 hoshang    (501) staff       (20)      402 2023-03-06 04:35:27.000000 leclerc-0.1.1/pyproject.toml
--rw-r--r--   0 hoshang    (501) staff       (20)       38 2023-05-03 02:26:01.107200 leclerc-0.1.1/setup.cfg
--rw-r--r--   0 hoshang    (501) staff       (20)      791 2023-05-03 02:25:43.000000 leclerc-0.1.1/setup.py
+drwxr-xr-x   0 hoshang    (501) staff       (20)        0 2023-05-03 02:39:36.569463 leclerc-0.1.2/
+-rw-r--r--   0 hoshang    (501) staff       (20)     2056 2023-05-03 02:39:36.568941 leclerc-0.1.2/PKG-INFO
+-rw-r--r--   0 hoshang    (501) staff       (20)     1523 2023-03-06 04:34:34.000000 leclerc-0.1.2/README
+drwxr-xr-x   0 hoshang    (501) staff       (20)        0 2023-05-03 02:39:36.565337 leclerc-0.1.2/leclerc/
+-rw-r--r--   0 hoshang    (501) staff       (20)       22 2023-05-03 02:39:24.000000 leclerc-0.1.2/leclerc/__init__.py
+-rw-r--r--   0 hoshang    (501) staff       (20)     3310 2023-05-03 02:33:49.000000 leclerc-0.1.2/leclerc/monte_databricks.py
+-rw-r--r--   0 hoshang    (501) staff       (20)     3175 2023-05-03 02:22:46.000000 leclerc-0.1.2/leclerc/montecarlinator.py
+-rw-r--r--   0 hoshang    (501) staff       (20)     3485 2023-02-28 11:51:15.000000 leclerc-0.1.2/leclerc/pert.py
+drwxr-xr-x   0 hoshang    (501) staff       (20)        0 2023-05-03 02:39:36.568248 leclerc-0.1.2/leclerc.egg-info/
+-rw-r--r--   0 hoshang    (501) staff       (20)     2056 2023-05-03 02:39:36.000000 leclerc-0.1.2/leclerc.egg-info/PKG-INFO
+-rw-r--r--   0 hoshang    (501) staff       (20)      245 2023-05-03 02:39:36.000000 leclerc-0.1.2/leclerc.egg-info/SOURCES.txt
+-rw-r--r--   0 hoshang    (501) staff       (20)        1 2023-05-03 02:39:36.000000 leclerc-0.1.2/leclerc.egg-info/dependency_links.txt
+-rw-r--r--   0 hoshang    (501) staff       (20)        8 2023-05-03 02:39:36.000000 leclerc-0.1.2/leclerc.egg-info/top_level.txt
+-rw-r--r--   0 hoshang    (501) staff       (20)      402 2023-03-06 04:35:27.000000 leclerc-0.1.2/pyproject.toml
+-rw-r--r--   0 hoshang    (501) staff       (20)       38 2023-05-03 02:39:36.569608 leclerc-0.1.2/setup.cfg
+-rw-r--r--   0 hoshang    (501) staff       (20)      792 2023-05-03 02:39:29.000000 leclerc-0.1.2/setup.py
```

### Comparing `leclerc-0.1.1/PKG-INFO` & `leclerc-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: leclerc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Leclerc conducts a montecarlo analysis on a range of function files that involve formula derivation
 Home-page: https://pypi.org/project/leclerc/
 Author: Luke Marhsall and Hoshang Mehta
-Author-email: luke.marshal@suncable.energy
+Author-email: luke.marshall@suncable.energy
 License: Open Source
 Keywords: Montecarlo,levelised cost
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
```

### Comparing `leclerc-0.1.1/README` & `leclerc-0.1.2/README`

 * *Files identical despite different names*

### Comparing `leclerc-0.1.1/leclerc/monte_databricks.py` & `leclerc-0.1.2/leclerc/monte_databricks.py`

 * *Files identical despite different names*

### Comparing `leclerc-0.1.1/leclerc/montecarlinator.py` & `leclerc-0.1.2/leclerc/montecarlinator.py`

 * *Files identical despite different names*

### Comparing `leclerc-0.1.1/leclerc/pert.py` & `leclerc-0.1.2/leclerc/pert.py`

 * *Files identical despite different names*

### Comparing `leclerc-0.1.1/leclerc.egg-info/PKG-INFO` & `leclerc-0.1.2/leclerc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: leclerc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Leclerc conducts a montecarlo analysis on a range of function files that involve formula derivation
 Home-page: https://pypi.org/project/leclerc/
 Author: Luke Marhsall and Hoshang Mehta
-Author-email: luke.marshal@suncable.energy
+Author-email: luke.marshall@suncable.energy
 License: Open Source
 Keywords: Montecarlo,levelised cost
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
```

### Comparing `leclerc-0.1.1/setup.py` & `leclerc-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from setuptools import setup
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "leclerc",
-    version = "0.1.1",
+    version = "0.1.2",
     author = "Luke Marhsall and Hoshang Mehta",
-    author_email = "luke.marshal@suncable.energy",
+    author_email = "luke.marshall@suncable.energy",
     description = ("Leclerc conducts a montecarlo analysis on a range of function files that involve formula derivation"),
     license = "Open Source",
     keywords = "Montecarlo, levelised cost",
     url = "https://pypi.org/project/leclerc/",
     packages=['leclerc'],
         long_description_content_type="text/markdown",
     long_description=read('README'),
```

