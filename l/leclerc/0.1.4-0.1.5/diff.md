# Comparing `tmp/leclerc-0.1.4.tar.gz` & `tmp/leclerc-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leclerc-0.1.4.tar", last modified: Wed May  3 04:24:45 2023, max compression
+gzip compressed data, was "leclerc-0.1.5.tar", last modified: Wed May  3 04:32:41 2023, max compression
```

## Comparing `leclerc-0.1.4.tar` & `leclerc-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 hoshang    (501) staff       (20)        0 2023-05-03 04:24:45.249616 leclerc-0.1.4/
--rw-r--r--   0 hoshang    (501) staff       (20)     2056 2023-05-03 04:24:45.249378 leclerc-0.1.4/PKG-INFO
--rw-r--r--   0 hoshang    (501) staff       (20)     1523 2023-03-06 04:34:34.000000 leclerc-0.1.4/README
-drwxr-xr-x   0 hoshang    (501) staff       (20)        0 2023-05-03 04:24:45.248055 leclerc-0.1.4/leclerc/
--rw-r--r--   0 hoshang    (501) staff       (20)       22 2023-05-03 04:23:55.000000 leclerc-0.1.4/leclerc/__init__.py
--rw-r--r--   0 hoshang    (501) staff       (20)     3310 2023-05-03 02:33:49.000000 leclerc-0.1.4/leclerc/monte_databricks.py
--rw-r--r--   0 hoshang    (501) staff       (20)     3175 2023-05-03 02:22:46.000000 leclerc-0.1.4/leclerc/montecarlinator.py
--rw-r--r--   0 hoshang    (501) staff       (20)     3485 2023-02-28 11:51:15.000000 leclerc-0.1.4/leclerc/pert.py
-drwxr-xr-x   0 hoshang    (501) staff       (20)        0 2023-05-03 04:24:45.249056 leclerc-0.1.4/leclerc.egg-info/
--rw-r--r--   0 hoshang    (501) staff       (20)     2056 2023-05-03 04:24:45.000000 leclerc-0.1.4/leclerc.egg-info/PKG-INFO
--rw-r--r--   0 hoshang    (501) staff       (20)      230 2023-05-03 04:24:45.000000 leclerc-0.1.4/leclerc.egg-info/SOURCES.txt
--rw-r--r--   0 hoshang    (501) staff       (20)        1 2023-05-03 04:24:45.000000 leclerc-0.1.4/leclerc.egg-info/dependency_links.txt
--rw-r--r--   0 hoshang    (501) staff       (20)        8 2023-05-03 04:24:45.000000 leclerc-0.1.4/leclerc.egg-info/top_level.txt
--rw-r--r--   0 hoshang    (501) staff       (20)       38 2023-05-03 04:24:45.249692 leclerc-0.1.4/setup.cfg
--rw-r--r--   0 hoshang    (501) staff       (20)      792 2023-05-03 04:23:45.000000 leclerc-0.1.4/setup.py
+drwxr-xr-x   0 hoshang    (501) staff       (20)        0 2023-05-03 04:32:41.686853 leclerc-0.1.5/
+-rw-r--r--   0 hoshang    (501) staff       (20)     2056 2023-05-03 04:32:41.686612 leclerc-0.1.5/PKG-INFO
+-rw-r--r--   0 hoshang    (501) staff       (20)     1523 2023-03-06 04:34:34.000000 leclerc-0.1.5/README
+drwxr-xr-x   0 hoshang    (501) staff       (20)        0 2023-05-03 04:32:41.685065 leclerc-0.1.5/leclerc/
+-rw-r--r--   0 hoshang    (501) staff       (20)       22 2023-05-03 04:32:14.000000 leclerc-0.1.5/leclerc/__init__.py
+-rw-r--r--   0 hoshang    (501) staff       (20)     3238 2023-05-03 04:31:40.000000 leclerc-0.1.5/leclerc/monte_databricks.py
+-rw-r--r--   0 hoshang    (501) staff       (20)     3175 2023-05-03 02:22:46.000000 leclerc-0.1.5/leclerc/montecarlinator.py
+-rw-r--r--   0 hoshang    (501) staff       (20)     3485 2023-02-28 11:51:15.000000 leclerc-0.1.5/leclerc/pert.py
+drwxr-xr-x   0 hoshang    (501) staff       (20)        0 2023-05-03 04:32:41.686258 leclerc-0.1.5/leclerc.egg-info/
+-rw-r--r--   0 hoshang    (501) staff       (20)     2056 2023-05-03 04:32:41.000000 leclerc-0.1.5/leclerc.egg-info/PKG-INFO
+-rw-r--r--   0 hoshang    (501) staff       (20)      230 2023-05-03 04:32:41.000000 leclerc-0.1.5/leclerc.egg-info/SOURCES.txt
+-rw-r--r--   0 hoshang    (501) staff       (20)        1 2023-05-03 04:32:41.000000 leclerc-0.1.5/leclerc.egg-info/dependency_links.txt
+-rw-r--r--   0 hoshang    (501) staff       (20)        8 2023-05-03 04:32:41.000000 leclerc-0.1.5/leclerc.egg-info/top_level.txt
+-rw-r--r--   0 hoshang    (501) staff       (20)       38 2023-05-03 04:32:41.686932 leclerc-0.1.5/setup.cfg
+-rw-r--r--   0 hoshang    (501) staff       (20)      792 2023-05-03 04:32:35.000000 leclerc-0.1.5/setup.py
```

### Comparing `leclerc-0.1.4/PKG-INFO` & `leclerc-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leclerc
-Version: 0.1.4
+Version: 0.1.5
 Summary: Leclerc conducts a montecarlo analysis on a range of function files that involve formula derivation
 Home-page: https://pypi.org/project/leclerc/
 Author: Luke Marhsall and Hoshang Mehta
 Author-email: luke.marshall@suncable.energy
 License: Open Source
 Keywords: Montecarlo,levelised cost
 Platform: UNKNOWN
```

### Comparing `leclerc-0.1.4/README` & `leclerc-0.1.5/README`

 * *Files identical despite different names*

### Comparing `leclerc-0.1.4/leclerc/monte_databricks.py` & `leclerc-0.1.5/leclerc/monte_databricks.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,11 +86,9 @@
 		results = []
 		for i in range(N):
 			new_args = [d[i][0] for d in dists]
 			result = func(*new_args)
 			results.append(result)
 		create_histogram(calculation, name, results)
 		show(gridplot([plots], toolbar_location="below"))
-		for plot in results:
-			html = file_html(plot, CDN, "my plot1")
-			displayHTML(html)
+		return plots
 	return wrapper_pert_monte_carlo
```

### Comparing `leclerc-0.1.4/leclerc/montecarlinator.py` & `leclerc-0.1.5/leclerc/montecarlinator.py`

 * *Files identical despite different names*

### Comparing `leclerc-0.1.4/leclerc/pert.py` & `leclerc-0.1.5/leclerc/pert.py`

 * *Files identical despite different names*

### Comparing `leclerc-0.1.4/leclerc.egg-info/PKG-INFO` & `leclerc-0.1.5/leclerc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leclerc
-Version: 0.1.4
+Version: 0.1.5
 Summary: Leclerc conducts a montecarlo analysis on a range of function files that involve formula derivation
 Home-page: https://pypi.org/project/leclerc/
 Author: Luke Marhsall and Hoshang Mehta
 Author-email: luke.marshall@suncable.energy
 License: Open Source
 Keywords: Montecarlo,levelised cost
 Platform: UNKNOWN
```

### Comparing `leclerc-0.1.4/setup.py` & `leclerc-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "leclerc",
-    version = "0.1.4",
+    version = "0.1.5",
     author = "Luke Marhsall and Hoshang Mehta",
     author_email = "luke.marshall@suncable.energy",
     description = ("Leclerc conducts a montecarlo analysis on a range of function files that involve formula derivation"),
     license = "Open Source",
     keywords = "Montecarlo, levelised cost",
     url = "https://pypi.org/project/leclerc/",
     packages=['leclerc'],
```

