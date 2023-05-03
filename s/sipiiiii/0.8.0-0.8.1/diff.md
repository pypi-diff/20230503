# Comparing `tmp/sipiiiii-0.8.0.tar.gz` & `tmp/sipiiiii-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sipiiiii-0.8.0.tar", last modified: Wed May  3 12:12:07 2023, max compression
+gzip compressed data, was "sipiiiii-0.8.1.tar", last modified: Wed May  3 12:19:46 2023, max compression
```

## Comparing `sipiiiii-0.8.0.tar` & `sipiiiii-0.8.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:12:07.867752 sipiiiii-0.8.0/
--rw-r--r--   0 j0hn       (501) staff       (20)       18 2023-05-03 12:00:50.000000 sipiiiii-0.8.0/MANIFEST.in
--rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-03 12:12:07.867111 sipiiiii-0.8.0/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)     3326 2023-05-02 13:20:44.000000 sipiiiii-0.8.0/README.md
--rw-r--r--   0 j0hn       (501) staff       (20)      625 2023-05-03 12:11:51.000000 sipiiiii-0.8.0/pyproject.toml
--rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-03 12:12:07.868046 sipiiiii-0.8.0/setup.cfg
--rw-r--r--   0 j0hn       (501) staff       (20)     3488 2023-05-03 12:11:39.000000 sipiiiii-0.8.0/setup.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:12:07.812604 sipiiiii-0.8.0/sipiiiii/
--rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-0.8.0/sipiiiii/__init__.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:12:07.832404 sipiiiii-0.8.0/sipiiiii/app/
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-0.8.0/sipiiiii/app/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)    10722 2023-05-03 10:00:47.000000 sipiiiii-0.8.0/sipiiiii/app/core.py
--rw-r--r--   0 j0hn       (501) staff       (20)    22498 2023-05-03 12:11:45.000000 sipiiiii-0.8.0/sipiiiii/app/new_app.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:12:07.838898 sipiiiii-0.8.0/sipiiiii/app/utils/
--rw-r--r--   0 j0hn       (501) staff       (20)     7845 2023-05-03 09:19:05.000000 sipiiiii-0.8.0/sipiiiii/app/utils/HttpSDK.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:12:07.848156 sipiiiii-0.8.0/sipiiiii/app/utils/PPI/
--rw-rw-r--   0 j0hn       (501) staff       (20)      174 2018-04-19 14:27:03.000000 sipiiiii-0.8.0/sipiiiii/app/utils/PPI/__init__.py
--rw-rw-r--   0 j0hn       (501) staff       (20)      524 2018-04-19 14:27:03.000000 sipiiiii-0.8.0/sipiiiii/app/utils/PPI/generator_factory.py
--rw-rw-r--   0 j0hn       (501) staff       (20)     6829 2023-04-10 15:58:16.000000 sipiiiii-0.8.0/sipiiiii/app/utils/PPI/prog_class.py
--rw-rw-r--   0 j0hn       (501) staff       (20)     3470 2018-04-19 14:27:03.000000 sipiiiii-0.8.0/sipiiiii/app/utils/PPI/progbar.py
--rw-rw-r--   0 j0hn       (501) staff       (20)     2460 2018-04-19 14:27:03.000000 sipiiiii-0.8.0/sipiiiii/app/utils/PPI/progpercent.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1695 2023-05-03 09:56:22.000000 sipiiiii-0.8.0/sipiiiii/app/utils/Tools.py
--rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-0.8.0/sipiiiii/app/utils/ZipFileTool.py
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-0.8.0/sipiiiii/app/utils/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)      138 2023-05-03 08:02:36.000000 sipiiiii-0.8.0/sipiiiii/app/utils/config.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-0.8.0/sipiiiii/app/utils/formatConversion.py
--rw-r--r--   0 j0hn       (501) staff       (20)     8501 2023-05-03 09:49:18.000000 sipiiiii-0.8.0/sipiiiii/main.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:12:07.829616 sipiiiii-0.8.0/sipiiiii.egg-info/
--rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-03 12:12:07.000000 sipiiiii-0.8.0/sipiiiii.egg-info/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)      863 2023-05-03 12:12:07.000000 sipiiiii-0.8.0/sipiiiii.egg-info/SOURCES.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-03 12:12:07.000000 sipiiiii-0.8.0/sipiiiii.egg-info/dependency_links.txt
--rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-03 12:12:07.000000 sipiiiii-0.8.0/sipiiiii.egg-info/entry_points.txt
--rw-r--r--   0 j0hn       (501) staff       (20)       97 2023-05-03 12:12:07.000000 sipiiiii-0.8.0/sipiiiii.egg-info/requires.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-03 12:12:07.000000 sipiiiii-0.8.0/sipiiiii.egg-info/top_level.txt
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:12:07.865811 sipiiiii-0.8.0/template/
--rw-r--r--   0 j0hn       (501) staff       (20)      366 2023-04-18 15:46:14.000000 sipiiiii-0.8.0/template/python_fastapi.j2
--rw-r--r--   0 j0hn       (501) staff       (20)      371 2023-04-18 15:46:06.000000 sipiiiii-0.8.0/template/python_flask.j2
--rw-r--r--   0 j0hn       (501) staff       (20)     1505 2023-05-01 16:17:11.000000 sipiiiii-0.8.0/template/python_openai.j2
--rw-r--r--   0 j0hn       (501) staff       (20)      793 2023-05-01 16:06:19.000000 sipiiiii-0.8.0/template/template_openai.yaml
--rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-01 16:06:57.000000 sipiiiii-0.8.0/template/template_other.yaml
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:19:46.355208 sipiiiii-0.8.1/
+-rw-r--r--   0 j0hn       (501) staff       (20)       18 2023-05-03 12:00:50.000000 sipiiiii-0.8.1/MANIFEST.in
+-rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-03 12:19:46.353900 sipiiiii-0.8.1/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)     3326 2023-05-02 13:20:44.000000 sipiiiii-0.8.1/README.md
+-rw-r--r--   0 j0hn       (501) staff       (20)      625 2023-05-03 12:19:12.000000 sipiiiii-0.8.1/pyproject.toml
+-rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-03 12:19:46.359083 sipiiiii-0.8.1/setup.cfg
+-rw-r--r--   0 j0hn       (501) staff       (20)     3488 2023-05-03 12:19:23.000000 sipiiiii-0.8.1/setup.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:19:46.306683 sipiiiii-0.8.1/sipiiiii/
+-rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-0.8.1/sipiiiii/__init__.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:19:46.324145 sipiiiii-0.8.1/sipiiiii/app/
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-0.8.1/sipiiiii/app/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    10722 2023-05-03 10:00:47.000000 sipiiiii-0.8.1/sipiiiii/app/core.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    22498 2023-05-03 12:19:06.000000 sipiiiii-0.8.1/sipiiiii/app/new_app.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:19:46.333365 sipiiiii-0.8.1/sipiiiii/app/utils/
+-rw-r--r--   0 j0hn       (501) staff       (20)     7845 2023-05-03 09:19:05.000000 sipiiiii-0.8.1/sipiiiii/app/utils/HttpSDK.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:19:46.342508 sipiiiii-0.8.1/sipiiiii/app/utils/PPI/
+-rw-rw-r--   0 j0hn       (501) staff       (20)      174 2018-04-19 14:27:03.000000 sipiiiii-0.8.1/sipiiiii/app/utils/PPI/__init__.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)      524 2018-04-19 14:27:03.000000 sipiiiii-0.8.1/sipiiiii/app/utils/PPI/generator_factory.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)     6829 2023-04-10 15:58:16.000000 sipiiiii-0.8.1/sipiiiii/app/utils/PPI/prog_class.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)     3470 2018-04-19 14:27:03.000000 sipiiiii-0.8.1/sipiiiii/app/utils/PPI/progbar.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)     2460 2018-04-19 14:27:03.000000 sipiiiii-0.8.1/sipiiiii/app/utils/PPI/progpercent.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1695 2023-05-03 12:17:12.000000 sipiiiii-0.8.1/sipiiiii/app/utils/Tools.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-0.8.1/sipiiiii/app/utils/ZipFileTool.py
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-0.8.1/sipiiiii/app/utils/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      138 2023-05-03 08:02:36.000000 sipiiiii-0.8.1/sipiiiii/app/utils/config.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-0.8.1/sipiiiii/app/utils/formatConversion.py
+-rw-r--r--   0 j0hn       (501) staff       (20)       17 2023-05-03 12:18:49.000000 sipiiiii-0.8.1/sipiiiii/app/version.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     8501 2023-05-03 12:18:55.000000 sipiiiii-0.8.1/sipiiiii/main.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:19:46.316481 sipiiiii-0.8.1/sipiiiii.egg-info/
+-rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-03 12:19:45.000000 sipiiiii-0.8.1/sipiiiii.egg-info/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)      887 2023-05-03 12:19:46.000000 sipiiiii-0.8.1/sipiiiii.egg-info/SOURCES.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-03 12:19:45.000000 sipiiiii-0.8.1/sipiiiii.egg-info/dependency_links.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-03 12:19:45.000000 sipiiiii-0.8.1/sipiiiii.egg-info/entry_points.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)       97 2023-05-03 12:19:45.000000 sipiiiii-0.8.1/sipiiiii.egg-info/requires.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-03 12:19:45.000000 sipiiiii-0.8.1/sipiiiii.egg-info/top_level.txt
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:19:46.352294 sipiiiii-0.8.1/template/
+-rw-r--r--   0 j0hn       (501) staff       (20)      366 2023-04-18 15:46:14.000000 sipiiiii-0.8.1/template/python_fastapi.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      371 2023-04-18 15:46:06.000000 sipiiiii-0.8.1/template/python_flask.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)     1505 2023-05-01 16:17:11.000000 sipiiiii-0.8.1/template/python_openai.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      793 2023-05-01 16:06:19.000000 sipiiiii-0.8.1/template/template_openai.yaml
+-rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-01 16:06:57.000000 sipiiiii-0.8.1/template/template_other.yaml
```

### Comparing `sipiiiii-0.8.0/PKG-INFO` & `sipiiiii-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 0.8.0
+Version: 0.8.1
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sipiiiii-0.8.0/README.md` & `sipiiiii-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.0/pyproject.toml` & `sipiiiii-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sipiiiii"
-version = "0.8.0"
+version = "0.8.1"
 authors = [
   { name="DeplRun", email="sipiiiii@example.com" },
 ]
 description = "sipiiiii定位为简单易用的云应用托管平台"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `sipiiiii-0.8.0/setup.py` & `sipiiiii-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     print(msg)
     sys.exit(1)
 
 setuptools.setup(
     # 包的分发名称，使用字母、数字、_、-
     name="sipiiiii",
     # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
-    version="0.8.0",
+    version="0.8.1",
     # 作者名
     author="sipiiiii@admin",
     # 作者邮箱
     author_email="j0hn.wahahaha@gmail.com",
     # 包的简介描述
     description="depl sipiiiii, App Development Framework",
     # 包的详细介绍(一般通过加载README.md)
```

### Comparing `sipiiiii-0.8.0/sipiiiii/app/core.py` & `sipiiiii-0.8.1/sipiiiii/app/core.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.0/sipiiiii/app/new_app.py` & `sipiiiii-0.8.1/sipiiiii/app/new_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -642,15 +642,15 @@
         table.add_row((app['AppName'], app['AppCnName'], app['Domain'],
                       app['ServerStatus'], app['AppStast'], app['CreateTime']))
 
     return True, table
 
 
 def get_cli_server_version():
-    return "0.8.0"
+    return "0.8.1"
 
 
 def update_template():
     pass
 
 
 def activate_account():
```

### Comparing `sipiiiii-0.8.0/sipiiiii/app/utils/HttpSDK.py` & `sipiiiii-0.8.1/sipiiiii/app/utils/HttpSDK.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.0/sipiiiii/app/utils/PPI/generator_factory.py` & `sipiiiii-0.8.1/sipiiiii/app/utils/PPI/generator_factory.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.0/sipiiiii/app/utils/PPI/prog_class.py` & `sipiiiii-0.8.1/sipiiiii/app/utils/PPI/prog_class.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.0/sipiiiii/app/utils/PPI/progbar.py` & `sipiiiii-0.8.1/sipiiiii/app/utils/PPI/progbar.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.0/sipiiiii/app/utils/PPI/progpercent.py` & `sipiiiii-0.8.1/sipiiiii/app/utils/PPI/progpercent.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.0/sipiiiii/app/utils/Tools.py` & `sipiiiii-0.8.1/sipiiiii/app/utils/Tools.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.0/sipiiiii/app/utils/ZipFileTool.py` & `sipiiiii-0.8.1/sipiiiii/app/utils/ZipFileTool.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.0/sipiiiii/app/utils/formatConversion.py` & `sipiiiii-0.8.1/sipiiiii/app/utils/formatConversion.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.0/sipiiiii/main.py` & `sipiiiii-0.8.1/sipiiiii/main.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.0/sipiiiii.egg-info/PKG-INFO` & `sipiiiii-0.8.1/sipiiiii.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 0.8.0
+Version: 0.8.1
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sipiiiii-0.8.0/sipiiiii.egg-info/SOURCES.txt` & `sipiiiii-0.8.1/sipiiiii.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 sipiiiii.egg-info/dependency_links.txt
 sipiiiii.egg-info/entry_points.txt
 sipiiiii.egg-info/requires.txt
 sipiiiii.egg-info/top_level.txt
 sipiiiii/app/__init__.py
 sipiiiii/app/core.py
 sipiiiii/app/new_app.py
+sipiiiii/app/version.py
 sipiiiii/app/utils/HttpSDK.py
 sipiiiii/app/utils/Tools.py
 sipiiiii/app/utils/ZipFileTool.py
 sipiiiii/app/utils/__init__.py
 sipiiiii/app/utils/config.py
 sipiiiii/app/utils/formatConversion.py
 sipiiiii/app/utils/PPI/__init__.py
```

### Comparing `sipiiiii-0.8.0/template/python_openai.j2` & `sipiiiii-0.8.1/template/python_openai.j2`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.0/template/template_openai.yaml` & `sipiiiii-0.8.1/template/template_openai.yaml`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.0/template/template_other.yaml` & `sipiiiii-0.8.1/template/template_other.yaml`

 * *Files identical despite different names*

