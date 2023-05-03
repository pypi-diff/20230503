# Comparing `tmp/custom_rails-0.0.7.tar.gz` & `tmp/custom_rails-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_rails-0.0.7.tar", last modified: Wed May  3 19:39:18 2023, max compression
+gzip compressed data, was "custom_rails-0.0.8.tar", last modified: Wed May  3 19:41:12 2023, max compression
```

## Comparing `custom_rails-0.0.7.tar` & `custom_rails-0.0.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 patcasrares   (501) staff       (20)        0 2023-05-03 19:39:18.106587 custom_rails-0.0.7/
--rw-r--r--   0 patcasrares   (501) staff       (20)      412 2023-05-03 19:39:18.106199 custom_rails-0.0.7/PKG-INFO
--rw-r--r--   0 patcasrares   (501) staff       (20)     7315 2023-04-30 14:20:14.000000 custom_rails-0.0.7/README.md
-drwxr-xr-x   0 patcasrares   (501) staff       (20)        0 2023-05-03 19:39:18.104451 custom_rails-0.0.7/custom_rails/
--rw-r--r--   0 patcasrares   (501) staff       (20)      630 2023-05-03 19:38:12.000000 custom_rails-0.0.7/custom_rails/__init__.py
--rw-r--r--   0 patcasrares   (501) staff       (20)      593 2023-04-17 15:43:26.000000 custom_rails-0.0.7/custom_rails/__main__.py
--rw-r--r--   0 patcasrares   (501) staff       (20)     2071 2023-04-17 00:54:40.000000 custom_rails-0.0.7/custom_rails/app.py
--rw-r--r--   0 patcasrares   (501) staff       (20)      546 2023-05-03 19:25:42.000000 custom_rails-0.0.7/custom_rails/cli.py
--rw-r--r--   0 patcasrares   (501) staff       (20)     4380 2023-04-30 14:20:14.000000 custom_rails-0.0.7/custom_rails/db.py
--rw-r--r--   0 patcasrares   (501) staff       (20)     1588 2023-04-30 14:20:14.000000 custom_rails-0.0.7/custom_rails/db_static.py
--rw-r--r--   0 patcasrares   (501) staff       (20)      115 2023-04-30 14:20:14.000000 custom_rails-0.0.7/custom_rails/db_static_model.py
--rw-r--r--   0 patcasrares   (501) staff       (20)     2898 2023-04-30 14:20:14.000000 custom_rails-0.0.7/custom_rails/request.py
--rw-r--r--   0 patcasrares   (501) staff       (20)     3945 2023-04-17 10:27:34.000000 custom_rails-0.0.7/custom_rails/response.py
--rw-r--r--   0 patcasrares   (501) staff       (20)     1213 2023-04-16 21:05:11.000000 custom_rails-0.0.7/custom_rails/router.py
--rw-r--r--   0 patcasrares   (501) staff       (20)     3566 2023-04-30 14:20:14.000000 custom_rails-0.0.7/custom_rails/start_rails_app.py
--rw-r--r--   0 patcasrares   (501) staff       (20)      339 2023-04-17 11:04:26.000000 custom_rails-0.0.7/custom_rails/template_gen.py
-drwxr-xr-x   0 patcasrares   (501) staff       (20)        0 2023-05-03 19:39:18.105312 custom_rails-0.0.7/custom_rails/templates/
--rw-r--r--   0 patcasrares   (501) staff       (20)      115 2023-04-17 11:06:26.000000 custom_rails-0.0.7/custom_rails/templates/config.ini
--rw-r--r--   0 patcasrares   (501) staff       (20)      349 2023-04-30 14:20:14.000000 custom_rails-0.0.7/custom_rails/templates/main_app.py
-drwxr-xr-x   0 patcasrares   (501) staff       (20)        0 2023-05-03 19:39:18.105087 custom_rails-0.0.7/custom_rails.egg-info/
--rw-r--r--   0 patcasrares   (501) staff       (20)      412 2023-05-03 19:39:18.000000 custom_rails-0.0.7/custom_rails.egg-info/PKG-INFO
--rw-r--r--   0 patcasrares   (501) staff       (20)      681 2023-05-03 19:39:18.000000 custom_rails-0.0.7/custom_rails.egg-info/SOURCES.txt
--rw-r--r--   0 patcasrares   (501) staff       (20)        1 2023-05-03 19:39:18.000000 custom_rails-0.0.7/custom_rails.egg-info/dependency_links.txt
--rw-r--r--   0 patcasrares   (501) staff       (20)       55 2023-05-03 19:39:18.000000 custom_rails-0.0.7/custom_rails.egg-info/entry_points.txt
--rw-r--r--   0 patcasrares   (501) staff       (20)       13 2023-05-03 19:39:18.000000 custom_rails-0.0.7/custom_rails.egg-info/top_level.txt
--rw-r--r--   0 patcasrares   (501) staff       (20)       38 2023-05-03 19:39:18.106684 custom_rails-0.0.7/setup.cfg
--rw-r--r--   0 patcasrares   (501) staff       (20)      689 2023-05-03 19:39:04.000000 custom_rails-0.0.7/setup.py
-drwxr-xr-x   0 patcasrares   (501) staff       (20)        0 2023-05-03 19:39:18.106005 custom_rails-0.0.7/test/
--rw-r--r--   0 patcasrares   (501) staff       (20)      123 2023-04-16 21:05:11.000000 custom_rails-0.0.7/test/__init__.py
--rw-r--r--   0 patcasrares   (501) staff       (20)     1192 2023-04-16 23:12:40.000000 custom_rails-0.0.7/test/test_app.py
--rw-r--r--   0 patcasrares   (501) staff       (20)     1256 2023-04-16 23:12:41.000000 custom_rails-0.0.7/test/test_request.py
--rw-r--r--   0 patcasrares   (501) staff       (20)      881 2023-04-16 23:12:42.000000 custom_rails-0.0.7/test/test_response.py
--rw-r--r--   0 patcasrares   (501) staff       (20)      843 2023-04-16 23:12:43.000000 custom_rails-0.0.7/test/test_router.py
--rw-r--r--   0 patcasrares   (501) staff       (20)     3333 2023-04-30 14:20:14.000000 custom_rails-0.0.7/test/utils.py
+drwxr-xr-x   0 patcasrares   (501) staff       (20)        0 2023-05-03 19:41:12.006764 custom_rails-0.0.8/
+-rw-r--r--   0 patcasrares   (501) staff       (20)      412 2023-05-03 19:41:12.006601 custom_rails-0.0.8/PKG-INFO
+-rw-r--r--   0 patcasrares   (501) staff       (20)     7315 2023-04-30 14:20:14.000000 custom_rails-0.0.8/README.md
+drwxr-xr-x   0 patcasrares   (501) staff       (20)        0 2023-05-03 19:41:12.004841 custom_rails-0.0.8/custom_rails/
+-rw-r--r--   0 patcasrares   (501) staff       (20)      646 2023-05-03 19:41:03.000000 custom_rails-0.0.8/custom_rails/__init__.py
+-rw-r--r--   0 patcasrares   (501) staff       (20)      593 2023-04-17 15:43:26.000000 custom_rails-0.0.8/custom_rails/__main__.py
+-rw-r--r--   0 patcasrares   (501) staff       (20)     2071 2023-04-17 00:54:40.000000 custom_rails-0.0.8/custom_rails/app.py
+-rw-r--r--   0 patcasrares   (501) staff       (20)      546 2023-05-03 19:25:42.000000 custom_rails-0.0.8/custom_rails/cli.py
+-rw-r--r--   0 patcasrares   (501) staff       (20)     4380 2023-04-30 14:20:14.000000 custom_rails-0.0.8/custom_rails/db.py
+-rw-r--r--   0 patcasrares   (501) staff       (20)     1588 2023-04-30 14:20:14.000000 custom_rails-0.0.8/custom_rails/db_static.py
+-rw-r--r--   0 patcasrares   (501) staff       (20)      115 2023-04-30 14:20:14.000000 custom_rails-0.0.8/custom_rails/db_static_model.py
+-rw-r--r--   0 patcasrares   (501) staff       (20)     2898 2023-04-30 14:20:14.000000 custom_rails-0.0.8/custom_rails/request.py
+-rw-r--r--   0 patcasrares   (501) staff       (20)     3945 2023-04-17 10:27:34.000000 custom_rails-0.0.8/custom_rails/response.py
+-rw-r--r--   0 patcasrares   (501) staff       (20)     1213 2023-04-16 21:05:11.000000 custom_rails-0.0.8/custom_rails/router.py
+-rw-r--r--   0 patcasrares   (501) staff       (20)     3566 2023-04-30 14:20:14.000000 custom_rails-0.0.8/custom_rails/start_rails_app.py
+-rw-r--r--   0 patcasrares   (501) staff       (20)      339 2023-04-17 11:04:26.000000 custom_rails-0.0.8/custom_rails/template_gen.py
+drwxr-xr-x   0 patcasrares   (501) staff       (20)        0 2023-05-03 19:41:12.005677 custom_rails-0.0.8/custom_rails/templates/
+-rw-r--r--   0 patcasrares   (501) staff       (20)      115 2023-04-17 11:06:26.000000 custom_rails-0.0.8/custom_rails/templates/config.ini
+-rw-r--r--   0 patcasrares   (501) staff       (20)      349 2023-04-30 14:20:14.000000 custom_rails-0.0.8/custom_rails/templates/main_app.py
+drwxr-xr-x   0 patcasrares   (501) staff       (20)        0 2023-05-03 19:41:12.005462 custom_rails-0.0.8/custom_rails.egg-info/
+-rw-r--r--   0 patcasrares   (501) staff       (20)      412 2023-05-03 19:41:11.000000 custom_rails-0.0.8/custom_rails.egg-info/PKG-INFO
+-rw-r--r--   0 patcasrares   (501) staff       (20)      681 2023-05-03 19:41:11.000000 custom_rails-0.0.8/custom_rails.egg-info/SOURCES.txt
+-rw-r--r--   0 patcasrares   (501) staff       (20)        1 2023-05-03 19:41:11.000000 custom_rails-0.0.8/custom_rails.egg-info/dependency_links.txt
+-rw-r--r--   0 patcasrares   (501) staff       (20)       55 2023-05-03 19:41:11.000000 custom_rails-0.0.8/custom_rails.egg-info/entry_points.txt
+-rw-r--r--   0 patcasrares   (501) staff       (20)       13 2023-05-03 19:41:11.000000 custom_rails-0.0.8/custom_rails.egg-info/top_level.txt
+-rw-r--r--   0 patcasrares   (501) staff       (20)       38 2023-05-03 19:41:12.006805 custom_rails-0.0.8/setup.cfg
+-rw-r--r--   0 patcasrares   (501) staff       (20)      689 2023-05-03 19:41:08.000000 custom_rails-0.0.8/setup.py
+drwxr-xr-x   0 patcasrares   (501) staff       (20)        0 2023-05-03 19:41:12.006396 custom_rails-0.0.8/test/
+-rw-r--r--   0 patcasrares   (501) staff       (20)      123 2023-04-16 21:05:11.000000 custom_rails-0.0.8/test/__init__.py
+-rw-r--r--   0 patcasrares   (501) staff       (20)     1192 2023-04-16 23:12:40.000000 custom_rails-0.0.8/test/test_app.py
+-rw-r--r--   0 patcasrares   (501) staff       (20)     1256 2023-04-16 23:12:41.000000 custom_rails-0.0.8/test/test_request.py
+-rw-r--r--   0 patcasrares   (501) staff       (20)      881 2023-04-16 23:12:42.000000 custom_rails-0.0.8/test/test_response.py
+-rw-r--r--   0 patcasrares   (501) staff       (20)      843 2023-04-16 23:12:43.000000 custom_rails-0.0.8/test/test_router.py
+-rw-r--r--   0 patcasrares   (501) staff       (20)     3333 2023-04-30 14:20:14.000000 custom_rails-0.0.8/test/utils.py
```

### Comparing `custom_rails-0.0.7/README.md` & `custom_rails-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `custom_rails-0.0.7/custom_rails/__init__.py` & `custom_rails-0.0.8/custom_rails/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import shutil
 from pkg_resources import resource_filename
 
 def copy_folder_contents(src_folder):
     for item in os.listdir(src_folder):
-        src = os.path.join(src_folder, item)
+        src = resource_filename("custom_rails", "templates")
         dest_folder = os.getcwd()
         dest = os.path.join(dest_folder, item)
         if os.path.isdir(src):
             shutil.copytree(src, dest, dirs_exist_ok=True)
         else:
             shutil.copy(src, dest)
```

### Comparing `custom_rails-0.0.7/custom_rails/__main__.py` & `custom_rails-0.0.8/custom_rails/__main__.py`

 * *Files identical despite different names*

### Comparing `custom_rails-0.0.7/custom_rails/app.py` & `custom_rails-0.0.8/custom_rails/app.py`

 * *Files identical despite different names*

### Comparing `custom_rails-0.0.7/custom_rails/cli.py` & `custom_rails-0.0.8/custom_rails/cli.py`

 * *Files identical despite different names*

### Comparing `custom_rails-0.0.7/custom_rails/db.py` & `custom_rails-0.0.8/custom_rails/db.py`

 * *Files identical despite different names*

### Comparing `custom_rails-0.0.7/custom_rails/db_static.py` & `custom_rails-0.0.8/custom_rails/db_static.py`

 * *Files identical despite different names*

### Comparing `custom_rails-0.0.7/custom_rails/request.py` & `custom_rails-0.0.8/custom_rails/request.py`

 * *Files identical despite different names*

### Comparing `custom_rails-0.0.7/custom_rails/response.py` & `custom_rails-0.0.8/custom_rails/response.py`

 * *Files identical despite different names*

### Comparing `custom_rails-0.0.7/custom_rails/router.py` & `custom_rails-0.0.8/custom_rails/router.py`

 * *Files identical despite different names*

### Comparing `custom_rails-0.0.7/custom_rails/start_rails_app.py` & `custom_rails-0.0.8/custom_rails/start_rails_app.py`

 * *Files identical despite different names*

### Comparing `custom_rails-0.0.7/custom_rails.egg-info/SOURCES.txt` & `custom_rails-0.0.8/custom_rails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `custom_rails-0.0.7/setup.py` & `custom_rails-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="custom_rails",
     keywords=["wsgi", "framework", ],
-    version="0.0.7",
+    version="0.0.8",
     maintainer="Patcas Rares",
     package_data={"custom_rails": ["templates/*"]},
     description="An educational wsgi based python web framework",
     packages=["custom_rails"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
```

### Comparing `custom_rails-0.0.7/test/test_app.py` & `custom_rails-0.0.8/test/test_app.py`

 * *Files identical despite different names*

### Comparing `custom_rails-0.0.7/test/test_request.py` & `custom_rails-0.0.8/test/test_request.py`

 * *Files identical despite different names*

### Comparing `custom_rails-0.0.7/test/test_response.py` & `custom_rails-0.0.8/test/test_response.py`

 * *Files identical despite different names*

### Comparing `custom_rails-0.0.7/test/test_router.py` & `custom_rails-0.0.8/test/test_router.py`

 * *Files identical despite different names*

### Comparing `custom_rails-0.0.7/test/utils.py` & `custom_rails-0.0.8/test/utils.py`

 * *Files identical despite different names*

