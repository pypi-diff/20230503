# Comparing `tmp/sipiiiii-0.7.8.tar.gz` & `tmp/sipiiiii-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sipiiiii-0.7.8.tar", last modified: Wed May  3 11:40:39 2023, max compression
+gzip compressed data, was "sipiiiii-0.7.9.tar", last modified: Wed May  3 12:03:20 2023, max compression
```

## Comparing `sipiiiii-0.7.8.tar` & `sipiiiii-0.7.9.tar`

### file list

```diff
@@ -1,33 +1,40 @@
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 11:40:39.503566 sipiiiii-0.7.8/
--rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-03 11:40:39.502709 sipiiiii-0.7.8/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)     3326 2023-05-02 13:20:44.000000 sipiiiii-0.7.8/README.md
--rw-r--r--   0 j0hn       (501) staff       (20)      633 2023-05-03 11:40:10.000000 sipiiiii-0.7.8/pyproject.toml
--rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-03 11:40:39.504558 sipiiiii-0.7.8/setup.cfg
--rw-r--r--   0 j0hn       (501) staff       (20)     3170 2023-05-03 11:39:48.000000 sipiiiii-0.7.8/setup.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 11:40:39.465397 sipiiiii-0.7.8/sipiiiii/
--rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-0.7.8/sipiiiii/__init__.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 11:40:39.476136 sipiiiii-0.7.8/sipiiiii/app/
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-0.7.8/sipiiiii/app/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)    10722 2023-05-03 10:00:47.000000 sipiiiii-0.7.8/sipiiiii/app/core.py
--rw-r--r--   0 j0hn       (501) staff       (20)    22498 2023-05-03 11:40:17.000000 sipiiiii-0.7.8/sipiiiii/app/new_app.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 11:40:39.486426 sipiiiii-0.7.8/sipiiiii/app/utils/
--rw-r--r--   0 j0hn       (501) staff       (20)     7845 2023-05-03 09:19:05.000000 sipiiiii-0.7.8/sipiiiii/app/utils/HttpSDK.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 11:40:39.500315 sipiiiii-0.7.8/sipiiiii/app/utils/PPI/
--rw-rw-r--   0 j0hn       (501) staff       (20)      174 2018-04-19 14:27:03.000000 sipiiiii-0.7.8/sipiiiii/app/utils/PPI/__init__.py
--rw-rw-r--   0 j0hn       (501) staff       (20)      524 2018-04-19 14:27:03.000000 sipiiiii-0.7.8/sipiiiii/app/utils/PPI/generator_factory.py
--rw-rw-r--   0 j0hn       (501) staff       (20)     6829 2023-04-10 15:58:16.000000 sipiiiii-0.7.8/sipiiiii/app/utils/PPI/prog_class.py
--rw-rw-r--   0 j0hn       (501) staff       (20)     3470 2018-04-19 14:27:03.000000 sipiiiii-0.7.8/sipiiiii/app/utils/PPI/progbar.py
--rw-rw-r--   0 j0hn       (501) staff       (20)     2460 2018-04-19 14:27:03.000000 sipiiiii-0.7.8/sipiiiii/app/utils/PPI/progpercent.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1695 2023-05-03 09:56:22.000000 sipiiiii-0.7.8/sipiiiii/app/utils/Tools.py
--rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-0.7.8/sipiiiii/app/utils/ZipFileTool.py
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-0.7.8/sipiiiii/app/utils/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)      138 2023-05-03 08:02:36.000000 sipiiiii-0.7.8/sipiiiii/app/utils/config.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-0.7.8/sipiiiii/app/utils/formatConversion.py
--rw-r--r--   0 j0hn       (501) staff       (20)     8501 2023-05-03 09:49:18.000000 sipiiiii-0.7.8/sipiiiii/main.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 11:40:39.471699 sipiiiii-0.7.8/sipiiiii.egg-info/
--rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-03 11:40:39.000000 sipiiiii-0.7.8/sipiiiii.egg-info/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)      714 2023-05-03 11:40:39.000000 sipiiiii-0.7.8/sipiiiii.egg-info/SOURCES.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-03 11:40:39.000000 sipiiiii-0.7.8/sipiiiii.egg-info/dependency_links.txt
--rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-03 11:40:39.000000 sipiiiii-0.7.8/sipiiiii.egg-info/entry_points.txt
--rw-r--r--   0 j0hn       (501) staff       (20)      102 2023-05-03 11:40:39.000000 sipiiiii-0.7.8/sipiiiii.egg-info/requires.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-03 11:40:39.000000 sipiiiii-0.7.8/sipiiiii.egg-info/top_level.txt
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:03:20.605194 sipiiiii-0.7.9/
+-rw-r--r--   0 j0hn       (501) staff       (20)       18 2023-05-03 12:00:50.000000 sipiiiii-0.7.9/MANIFEST.in
+-rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-03 12:03:20.604435 sipiiiii-0.7.9/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)     3326 2023-05-02 13:20:44.000000 sipiiiii-0.7.9/README.md
+-rw-r--r--   0 j0hn       (501) staff       (20)      625 2023-05-03 12:02:43.000000 sipiiiii-0.7.9/pyproject.toml
+-rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-03 12:03:20.605545 sipiiiii-0.7.9/setup.cfg
+-rw-r--r--   0 j0hn       (501) staff       (20)     3470 2023-05-03 12:02:55.000000 sipiiiii-0.7.9/setup.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:03:20.566091 sipiiiii-0.7.9/sipiiiii/
+-rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-0.7.9/sipiiiii/__init__.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:03:20.582557 sipiiiii-0.7.9/sipiiiii/app/
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-0.7.9/sipiiiii/app/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    10722 2023-05-03 10:00:47.000000 sipiiiii-0.7.9/sipiiiii/app/core.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    22498 2023-05-03 12:03:06.000000 sipiiiii-0.7.9/sipiiiii/app/new_app.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:03:20.590955 sipiiiii-0.7.9/sipiiiii/app/utils/
+-rw-r--r--   0 j0hn       (501) staff       (20)     7845 2023-05-03 09:19:05.000000 sipiiiii-0.7.9/sipiiiii/app/utils/HttpSDK.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:03:20.596697 sipiiiii-0.7.9/sipiiiii/app/utils/PPI/
+-rw-rw-r--   0 j0hn       (501) staff       (20)      174 2018-04-19 14:27:03.000000 sipiiiii-0.7.9/sipiiiii/app/utils/PPI/__init__.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)      524 2018-04-19 14:27:03.000000 sipiiiii-0.7.9/sipiiiii/app/utils/PPI/generator_factory.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)     6829 2023-04-10 15:58:16.000000 sipiiiii-0.7.9/sipiiiii/app/utils/PPI/prog_class.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)     3470 2018-04-19 14:27:03.000000 sipiiiii-0.7.9/sipiiiii/app/utils/PPI/progbar.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)     2460 2018-04-19 14:27:03.000000 sipiiiii-0.7.9/sipiiiii/app/utils/PPI/progpercent.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1695 2023-05-03 09:56:22.000000 sipiiiii-0.7.9/sipiiiii/app/utils/Tools.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-0.7.9/sipiiiii/app/utils/ZipFileTool.py
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-0.7.9/sipiiiii/app/utils/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      138 2023-05-03 08:02:36.000000 sipiiiii-0.7.9/sipiiiii/app/utils/config.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-0.7.9/sipiiiii/app/utils/formatConversion.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     8501 2023-05-03 09:49:18.000000 sipiiiii-0.7.9/sipiiiii/main.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:03:20.578656 sipiiiii-0.7.9/sipiiiii.egg-info/
+-rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-03 12:03:20.000000 sipiiiii-0.7.9/sipiiiii.egg-info/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)      863 2023-05-03 12:03:20.000000 sipiiiii-0.7.9/sipiiiii.egg-info/SOURCES.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-03 12:03:20.000000 sipiiiii-0.7.9/sipiiiii.egg-info/dependency_links.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-03 12:03:20.000000 sipiiiii-0.7.9/sipiiiii.egg-info/entry_points.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)       97 2023-05-03 12:03:20.000000 sipiiiii-0.7.9/sipiiiii.egg-info/requires.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-03 12:03:20.000000 sipiiiii-0.7.9/sipiiiii.egg-info/top_level.txt
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:03:20.603191 sipiiiii-0.7.9/template/
+-rw-r--r--   0 j0hn       (501) staff       (20)      366 2023-04-18 15:46:14.000000 sipiiiii-0.7.9/template/python_fastapi.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      371 2023-04-18 15:46:06.000000 sipiiiii-0.7.9/template/python_flask.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)     1505 2023-05-01 16:17:11.000000 sipiiiii-0.7.9/template/python_openai.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      793 2023-05-01 16:06:19.000000 sipiiiii-0.7.9/template/template_openai.yaml
+-rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-01 16:06:57.000000 sipiiiii-0.7.9/template/template_other.yaml
```

### Comparing `sipiiiii-0.7.8/PKG-INFO` & `sipiiiii-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 0.7.8
+Version: 0.7.9
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sipiiiii-0.7.8/README.md` & `sipiiiii-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.8/pyproject.toml` & `sipiiiii-0.7.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sipiiiii"
-version = "0.7.8"
+version = "0.7.9"
 authors = [
   { name="DeplRun", email="sipiiiii@example.com" },
 ]
 description = "sipiiiii定位为简单易用的云应用托管平台"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -14,11 +14,11 @@
 ]
 dependencies = [
   'httpx', 
   'prettytable==3.7.0', 
   'jinja2', 
   'requests', 
   'requests_toolbelt', 
-  'xmltodict', 'validators', 'pathlib', 'jsonpath', 'yaml']
+  'xmltodict', 'validators', 'pathlib', 'jsonpath']
 [project.urls]
 "Homepage" = "http://www.depl.run/"
 "Bug Tracker" = "http://www.depl.run/"
```

### Comparing `sipiiiii-0.7.8/setup.py` & `sipiiiii-0.7.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,17 +24,24 @@
 
 
 def init_framework():
     aiapi_dir = get_current_path()
 
     # Replace 'template/template.yaml' with the path to the file you want to copy
     # src_file = f'sipiiiii{os.sep}template/template.yaml'
-    src_dir = os.path.join("sipiiiii", "template")
+    # try:
+    src_dir = os.path.join(os.getcwd(), "template")
+    # src_dir = os.path.join('sipiiiii', "template")
+    try:
+        template_files = os.listdir(src_dir)
+    except Exception as e:
+        print(e)
+        src_dir = os.path.join(os.getcwd(), "sipiiiii", "template")
+        template_files = os.listdir(src_dir)
 
-    template_files = os.listdir(src_dir)
     for tFIle in template_files:
         src_file = os.path.join(src_dir, tFIle)
 
         # Use Path().resolve() to get the absolute path of the source file
         src_path = Path(src_file).resolve()
 
         # Use Path().joinpath() to get the destination path
@@ -61,40 +68,41 @@
     print(msg)
     sys.exit(1)
 
 setuptools.setup(
     # 包的分发名称，使用字母、数字、_、-
     name="sipiiiii",
     # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
-    version="0.7.8",
+    version="0.7.9",
     # 作者名
     author="sipiiiii@admin",
     # 作者邮箱
     author_email="j0hn.wahahaha@gmail.com",
     # 包的简介描述
     description="depl sipiiiii, App Development Framework",
     # 包的详细介绍(一般通过加载README.md)
     long_description=long_description,
     # 和上条命令配合使用，声明加载的是markdown文件
     long_description_content_type="text/markdown",
     # 项目开源地址
     url="http://www.depl.run/",
     # 如果项目由多个文件组成，我们可以使用find_packages()自动发现所有包和子包，而不是手动列出每个包，在这种情况下，包列表将是example_pkg
     packages=setuptools.find_packages(),
+    package_data={'template': ['*.j2', '*.yaml']},
+    nclude_package_data=True,
     install_requires=[
         'httpx',
         'prettytable==3.7.0',
         'jinja2',
         'requests',
         'requests_toolbelt',
         'xmltodict',
         'validators',
         'pathlib',
-        'jsonpath',
-        'yaml'
+        'jsonpath'
     ],
     entry_points={
         'console_scripts': [
             'sipiiiii = sipiiiii.main:main'
         ]
     },
     # 关于包的其他元数据(metadata)
```

### Comparing `sipiiiii-0.7.8/sipiiiii/app/core.py` & `sipiiiii-0.7.9/sipiiiii/app/core.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.8/sipiiiii/app/new_app.py` & `sipiiiii-0.7.9/sipiiiii/app/new_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -642,15 +642,15 @@
         table.add_row((app['AppName'], app['AppCnName'], app['Domain'],
                       app['ServerStatus'], app['AppStast'], app['CreateTime']))
 
     return True, table
 
 
 def get_cli_server_version():
-    return "0.7.8"
+    return "0.7.9"
 
 
 def update_template():
     pass
 
 
 def activate_account():
```

### Comparing `sipiiiii-0.7.8/sipiiiii/app/utils/HttpSDK.py` & `sipiiiii-0.7.9/sipiiiii/app/utils/HttpSDK.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.8/sipiiiii/app/utils/PPI/generator_factory.py` & `sipiiiii-0.7.9/sipiiiii/app/utils/PPI/generator_factory.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.8/sipiiiii/app/utils/PPI/prog_class.py` & `sipiiiii-0.7.9/sipiiiii/app/utils/PPI/prog_class.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.8/sipiiiii/app/utils/PPI/progbar.py` & `sipiiiii-0.7.9/sipiiiii/app/utils/PPI/progbar.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.8/sipiiiii/app/utils/PPI/progpercent.py` & `sipiiiii-0.7.9/sipiiiii/app/utils/PPI/progpercent.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.8/sipiiiii/app/utils/Tools.py` & `sipiiiii-0.7.9/sipiiiii/app/utils/Tools.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.8/sipiiiii/app/utils/ZipFileTool.py` & `sipiiiii-0.7.9/sipiiiii/app/utils/ZipFileTool.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.8/sipiiiii/app/utils/formatConversion.py` & `sipiiiii-0.7.9/sipiiiii/app/utils/formatConversion.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.8/sipiiiii/main.py` & `sipiiiii-0.7.9/sipiiiii/main.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.8/sipiiiii.egg-info/PKG-INFO` & `sipiiiii-0.7.9/sipiiiii.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 0.7.8
+Version: 0.7.9
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
```

