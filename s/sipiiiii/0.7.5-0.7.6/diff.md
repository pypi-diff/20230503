# Comparing `tmp/sipiiiii-0.7.5.tar.gz` & `tmp/sipiiiii-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sipiiiii-0.7.5.tar", last modified: Wed May  3 10:07:26 2023, max compression
+gzip compressed data, was "sipiiiii-0.7.6.tar", last modified: Wed May  3 10:15:46 2023, max compression
```

## Comparing `sipiiiii-0.7.5.tar` & `sipiiiii-0.7.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 10:07:26.926427 sipiiiii-0.7.5/
--rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-03 10:07:26.925765 sipiiiii-0.7.5/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)     3326 2023-05-02 13:20:44.000000 sipiiiii-0.7.5/README.md
--rw-r--r--   0 j0hn       (501) staff       (20)      468 2023-05-03 10:05:31.000000 sipiiiii-0.7.5/pyproject.toml
--rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-03 10:07:26.926781 sipiiiii-0.7.5/setup.cfg
--rw-r--r--   0 j0hn       (501) staff       (20)     1839 2023-05-03 10:04:56.000000 sipiiiii-0.7.5/setup.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 10:07:26.903745 sipiiiii-0.7.5/sipiiiii/
--rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-0.7.5/sipiiiii/__init__.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 10:07:26.912421 sipiiiii-0.7.5/sipiiiii/app/
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-0.7.5/sipiiiii/app/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)    10722 2023-05-03 10:00:47.000000 sipiiiii-0.7.5/sipiiiii/app/core.py
--rw-r--r--   0 j0hn       (501) staff       (20)    22517 2023-05-03 10:05:09.000000 sipiiiii-0.7.5/sipiiiii/app/new_app.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 10:07:26.918609 sipiiiii-0.7.5/sipiiiii/app/utils/
--rw-r--r--   0 j0hn       (501) staff       (20)     7845 2023-05-03 09:19:05.000000 sipiiiii-0.7.5/sipiiiii/app/utils/HttpSDK.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 10:07:26.924531 sipiiiii-0.7.5/sipiiiii/app/utils/PPI/
--rw-rw-r--   0 j0hn       (501) staff       (20)      174 2018-04-19 14:27:03.000000 sipiiiii-0.7.5/sipiiiii/app/utils/PPI/__init__.py
--rw-rw-r--   0 j0hn       (501) staff       (20)      524 2018-04-19 14:27:03.000000 sipiiiii-0.7.5/sipiiiii/app/utils/PPI/generator_factory.py
--rw-rw-r--   0 j0hn       (501) staff       (20)     6829 2023-04-10 15:58:16.000000 sipiiiii-0.7.5/sipiiiii/app/utils/PPI/prog_class.py
--rw-rw-r--   0 j0hn       (501) staff       (20)     3470 2018-04-19 14:27:03.000000 sipiiiii-0.7.5/sipiiiii/app/utils/PPI/progbar.py
--rw-rw-r--   0 j0hn       (501) staff       (20)     2460 2018-04-19 14:27:03.000000 sipiiiii-0.7.5/sipiiiii/app/utils/PPI/progpercent.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1695 2023-05-03 09:56:22.000000 sipiiiii-0.7.5/sipiiiii/app/utils/Tools.py
--rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-0.7.5/sipiiiii/app/utils/ZipFileTool.py
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-0.7.5/sipiiiii/app/utils/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)      138 2023-05-03 08:02:36.000000 sipiiiii-0.7.5/sipiiiii/app/utils/config.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-0.7.5/sipiiiii/app/utils/formatConversion.py
--rw-r--r--   0 j0hn       (501) staff       (20)       15 2023-05-03 10:05:02.000000 sipiiiii-0.7.5/sipiiiii/app/version.py
--rw-r--r--   0 j0hn       (501) staff       (20)     8501 2023-05-03 09:49:18.000000 sipiiiii-0.7.5/sipiiiii/main.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 10:07:26.908619 sipiiiii-0.7.5/sipiiiii.egg-info/
--rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-03 10:07:26.000000 sipiiiii-0.7.5/sipiiiii.egg-info/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)      738 2023-05-03 10:07:26.000000 sipiiiii-0.7.5/sipiiiii.egg-info/SOURCES.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-03 10:07:26.000000 sipiiiii-0.7.5/sipiiiii.egg-info/dependency_links.txt
--rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-03 10:07:26.000000 sipiiiii-0.7.5/sipiiiii.egg-info/entry_points.txt
--rw-r--r--   0 j0hn       (501) staff       (20)      102 2023-05-03 10:07:26.000000 sipiiiii-0.7.5/sipiiiii.egg-info/requires.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-03 10:07:26.000000 sipiiiii-0.7.5/sipiiiii.egg-info/top_level.txt
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 10:15:46.444973 sipiiiii-0.7.6/
+-rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-03 10:15:46.444309 sipiiiii-0.7.6/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)     3326 2023-05-02 13:20:44.000000 sipiiiii-0.7.6/README.md
+-rw-r--r--   0 j0hn       (501) staff       (20)      468 2023-05-03 10:15:06.000000 sipiiiii-0.7.6/pyproject.toml
+-rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-03 10:15:46.445237 sipiiiii-0.7.6/setup.cfg
+-rw-r--r--   0 j0hn       (501) staff       (20)     1839 2023-05-03 10:15:00.000000 sipiiiii-0.7.6/setup.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 10:15:46.413945 sipiiiii-0.7.6/sipiiiii/
+-rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-0.7.6/sipiiiii/__init__.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 10:15:46.430357 sipiiiii-0.7.6/sipiiiii/app/
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-0.7.6/sipiiiii/app/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    10722 2023-05-03 10:00:47.000000 sipiiiii-0.7.6/sipiiiii/app/core.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    22517 2023-05-03 10:15:23.000000 sipiiiii-0.7.6/sipiiiii/app/new_app.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 10:15:46.437212 sipiiiii-0.7.6/sipiiiii/app/utils/
+-rw-r--r--   0 j0hn       (501) staff       (20)     7845 2023-05-03 09:19:05.000000 sipiiiii-0.7.6/sipiiiii/app/utils/HttpSDK.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 10:15:46.443360 sipiiiii-0.7.6/sipiiiii/app/utils/PPI/
+-rw-rw-r--   0 j0hn       (501) staff       (20)      174 2018-04-19 14:27:03.000000 sipiiiii-0.7.6/sipiiiii/app/utils/PPI/__init__.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)      524 2018-04-19 14:27:03.000000 sipiiiii-0.7.6/sipiiiii/app/utils/PPI/generator_factory.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)     6829 2023-04-10 15:58:16.000000 sipiiiii-0.7.6/sipiiiii/app/utils/PPI/prog_class.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)     3470 2018-04-19 14:27:03.000000 sipiiiii-0.7.6/sipiiiii/app/utils/PPI/progbar.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)     2460 2018-04-19 14:27:03.000000 sipiiiii-0.7.6/sipiiiii/app/utils/PPI/progpercent.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1695 2023-05-03 09:56:22.000000 sipiiiii-0.7.6/sipiiiii/app/utils/Tools.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-0.7.6/sipiiiii/app/utils/ZipFileTool.py
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-0.7.6/sipiiiii/app/utils/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      138 2023-05-03 08:02:36.000000 sipiiiii-0.7.6/sipiiiii/app/utils/config.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-0.7.6/sipiiiii/app/utils/formatConversion.py
+-rw-r--r--   0 j0hn       (501) staff       (20)       15 2023-05-03 10:15:10.000000 sipiiiii-0.7.6/sipiiiii/app/version.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     8501 2023-05-03 09:49:18.000000 sipiiiii-0.7.6/sipiiiii/main.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 10:15:46.424301 sipiiiii-0.7.6/sipiiiii.egg-info/
+-rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-03 10:15:46.000000 sipiiiii-0.7.6/sipiiiii.egg-info/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)      738 2023-05-03 10:15:46.000000 sipiiiii-0.7.6/sipiiiii.egg-info/SOURCES.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-03 10:15:46.000000 sipiiiii-0.7.6/sipiiiii.egg-info/dependency_links.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-03 10:15:46.000000 sipiiiii-0.7.6/sipiiiii.egg-info/entry_points.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)      102 2023-05-03 10:15:46.000000 sipiiiii-0.7.6/sipiiiii.egg-info/requires.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-03 10:15:46.000000 sipiiiii-0.7.6/sipiiiii.egg-info/top_level.txt
```

### Comparing `sipiiiii-0.7.5/PKG-INFO` & `sipiiiii-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 0.7.5
+Version: 0.7.6
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sipiiiii-0.7.5/README.md` & `sipiiiii-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.5/setup.py` & `sipiiiii-0.7.6/setup.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -27,28 +27,28 @@
     # 包的详细介绍(一般通过加载README.md)
     long_description=long_description,
     # 和上条命令配合使用，声明加载的是markdown文件
     long_description_content_type="text/markdown",
     # 项目开源地址
     url="http://www.depl.run/",
     # 如果项目由多个文件组成，我们可以使用find_packages()自动发现所有包和子包，而不是手动列出每个包，在这种情况下，包列表将是example_pkg
-    packages=setuptools.find_packages(),
     install_requires=[
         'httpx',
         'prettytable',
         'jinja2',
         'requests',
         'yaml',
         'shutil',
         'requests_toolbelt',
         'xmltodict',
         'validators',
         'pathlib',
         'jsonpath'
     ],
+    packages=setuptools.find_packages(),
     entry_points={
         'console_scripts': [
             'sipiiiii = sipiiiii.main:main'
         ]
     },
     # 关于包的其他元数据(metadata)
     classifiers=[
```

### Comparing `sipiiiii-0.7.5/sipiiiii/app/core.py` & `sipiiiii-0.7.6/sipiiiii/app/core.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.5/sipiiiii/app/new_app.py` & `sipiiiii-0.7.6/sipiiiii/app/new_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -641,15 +641,15 @@
         table.add_row((app['AppName'], app['AppCnName'], app['Domain'],
                       app['ServerStatus'], app['AppStast'], app['CreateTime']))
 
     return True, table
 
 
 def get_cli_server_version():
-    return "0.7.5"
+    return "0.7.6"
 
 
 def update_template():
     pass
 
 
 def activate_account():
```

### Comparing `sipiiiii-0.7.5/sipiiiii/app/utils/HttpSDK.py` & `sipiiiii-0.7.6/sipiiiii/app/utils/HttpSDK.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.5/sipiiiii/app/utils/PPI/generator_factory.py` & `sipiiiii-0.7.6/sipiiiii/app/utils/PPI/generator_factory.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.5/sipiiiii/app/utils/PPI/prog_class.py` & `sipiiiii-0.7.6/sipiiiii/app/utils/PPI/prog_class.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.5/sipiiiii/app/utils/PPI/progbar.py` & `sipiiiii-0.7.6/sipiiiii/app/utils/PPI/progbar.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.5/sipiiiii/app/utils/PPI/progpercent.py` & `sipiiiii-0.7.6/sipiiiii/app/utils/PPI/progpercent.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.5/sipiiiii/app/utils/Tools.py` & `sipiiiii-0.7.6/sipiiiii/app/utils/Tools.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.5/sipiiiii/app/utils/ZipFileTool.py` & `sipiiiii-0.7.6/sipiiiii/app/utils/ZipFileTool.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.5/sipiiiii/app/utils/formatConversion.py` & `sipiiiii-0.7.6/sipiiiii/app/utils/formatConversion.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.5/sipiiiii/main.py` & `sipiiiii-0.7.6/sipiiiii/main.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.5/sipiiiii.egg-info/PKG-INFO` & `sipiiiii-0.7.6/sipiiiii.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 0.7.5
+Version: 0.7.6
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sipiiiii-0.7.5/sipiiiii.egg-info/SOURCES.txt` & `sipiiiii-0.7.6/sipiiiii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

