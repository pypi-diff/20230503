# Comparing `tmp/sipiiiii-0.8.2.tar.gz` & `tmp/sipiiiii-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sipiiiii-0.8.2.tar", last modified: Wed May  3 12:21:48 2023, max compression
+gzip compressed data, was "sipiiiii-0.8.3.tar", last modified: Wed May  3 12:42:02 2023, max compression
```

## Comparing `sipiiiii-0.8.2.tar` & `sipiiiii-0.8.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:21:48.935665 sipiiiii-0.8.2/
--rw-r--r--   0 j0hn       (501) staff       (20)       18 2023-05-03 12:00:50.000000 sipiiiii-0.8.2/MANIFEST.in
--rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-03 12:21:48.934922 sipiiiii-0.8.2/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)     3326 2023-05-02 13:20:44.000000 sipiiiii-0.8.2/README.md
--rw-r--r--   0 j0hn       (501) staff       (20)      634 2023-05-03 12:21:28.000000 sipiiiii-0.8.2/pyproject.toml
--rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-03 12:21:48.936163 sipiiiii-0.8.2/setup.cfg
--rw-r--r--   0 j0hn       (501) staff       (20)     3506 2023-05-03 12:21:28.000000 sipiiiii-0.8.2/setup.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:21:48.892941 sipiiiii-0.8.2/sipiiiii/
--rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-0.8.2/sipiiiii/__init__.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:21:48.910593 sipiiiii-0.8.2/sipiiiii/app/
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-0.8.2/sipiiiii/app/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)    10722 2023-05-03 10:00:47.000000 sipiiiii-0.8.2/sipiiiii/app/core.py
--rw-r--r--   0 j0hn       (501) staff       (20)    22498 2023-05-03 12:21:28.000000 sipiiiii-0.8.2/sipiiiii/app/new_app.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:21:48.921251 sipiiiii-0.8.2/sipiiiii/app/utils/
--rw-r--r--   0 j0hn       (501) staff       (20)     7845 2023-05-03 09:19:05.000000 sipiiiii-0.8.2/sipiiiii/app/utils/HttpSDK.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:21:48.928554 sipiiiii-0.8.2/sipiiiii/app/utils/PPI/
--rw-rw-r--   0 j0hn       (501) staff       (20)      174 2018-04-19 14:27:03.000000 sipiiiii-0.8.2/sipiiiii/app/utils/PPI/__init__.py
--rw-rw-r--   0 j0hn       (501) staff       (20)      524 2018-04-19 14:27:03.000000 sipiiiii-0.8.2/sipiiiii/app/utils/PPI/generator_factory.py
--rw-rw-r--   0 j0hn       (501) staff       (20)     6829 2023-04-10 15:58:16.000000 sipiiiii-0.8.2/sipiiiii/app/utils/PPI/prog_class.py
--rw-rw-r--   0 j0hn       (501) staff       (20)     3470 2018-04-19 14:27:03.000000 sipiiiii-0.8.2/sipiiiii/app/utils/PPI/progbar.py
--rw-rw-r--   0 j0hn       (501) staff       (20)     2460 2018-04-19 14:27:03.000000 sipiiiii-0.8.2/sipiiiii/app/utils/PPI/progpercent.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1695 2023-05-03 12:17:12.000000 sipiiiii-0.8.2/sipiiiii/app/utils/Tools.py
--rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-0.8.2/sipiiiii/app/utils/ZipFileTool.py
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-0.8.2/sipiiiii/app/utils/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)      138 2023-05-03 08:02:36.000000 sipiiiii-0.8.2/sipiiiii/app/utils/config.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-0.8.2/sipiiiii/app/utils/formatConversion.py
--rw-r--r--   0 j0hn       (501) staff       (20)       17 2023-05-03 12:21:28.000000 sipiiiii-0.8.2/sipiiiii/app/version.py
--rw-r--r--   0 j0hn       (501) staff       (20)     8501 2023-05-03 12:18:55.000000 sipiiiii-0.8.2/sipiiiii/main.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:21:48.899743 sipiiiii-0.8.2/sipiiiii.egg-info/
--rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-03 12:21:48.000000 sipiiiii-0.8.2/sipiiiii.egg-info/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)      887 2023-05-03 12:21:48.000000 sipiiiii-0.8.2/sipiiiii.egg-info/SOURCES.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-03 12:21:48.000000 sipiiiii-0.8.2/sipiiiii.egg-info/dependency_links.txt
--rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-03 12:21:48.000000 sipiiiii-0.8.2/sipiiiii.egg-info/entry_points.txt
--rw-r--r--   0 j0hn       (501) staff       (20)      104 2023-05-03 12:21:48.000000 sipiiiii-0.8.2/sipiiiii.egg-info/requires.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-03 12:21:48.000000 sipiiiii-0.8.2/sipiiiii.egg-info/top_level.txt
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:21:48.933847 sipiiiii-0.8.2/template/
--rw-r--r--   0 j0hn       (501) staff       (20)      366 2023-04-18 15:46:14.000000 sipiiiii-0.8.2/template/python_fastapi.j2
--rw-r--r--   0 j0hn       (501) staff       (20)      371 2023-04-18 15:46:06.000000 sipiiiii-0.8.2/template/python_flask.j2
--rw-r--r--   0 j0hn       (501) staff       (20)     1505 2023-05-01 16:17:11.000000 sipiiiii-0.8.2/template/python_openai.j2
--rw-r--r--   0 j0hn       (501) staff       (20)      793 2023-05-01 16:06:19.000000 sipiiiii-0.8.2/template/template_openai.yaml
--rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-01 16:06:57.000000 sipiiiii-0.8.2/template/template_other.yaml
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:42:02.896291 sipiiiii-0.8.3/
+-rw-r--r--   0 j0hn       (501) staff       (20)       18 2023-05-03 12:00:50.000000 sipiiiii-0.8.3/MANIFEST.in
+-rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-03 12:42:02.895703 sipiiiii-0.8.3/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)     3326 2023-05-02 13:20:44.000000 sipiiiii-0.8.3/README.md
+-rw-r--r--   0 j0hn       (501) staff       (20)      634 2023-05-03 12:41:46.000000 sipiiiii-0.8.3/pyproject.toml
+-rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-03 12:42:02.896473 sipiiiii-0.8.3/setup.cfg
+-rw-r--r--   0 j0hn       (501) staff       (20)     3401 2023-05-03 12:41:47.000000 sipiiiii-0.8.3/setup.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:42:02.868928 sipiiiii-0.8.3/sipiiiii/
+-rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-0.8.3/sipiiiii/__init__.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:42:02.878425 sipiiiii-0.8.3/sipiiiii/app/
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-0.8.3/sipiiiii/app/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    10751 2023-05-03 12:36:45.000000 sipiiiii-0.8.3/sipiiiii/app/core.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    22498 2023-05-03 12:41:46.000000 sipiiiii-0.8.3/sipiiiii/app/new_app.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:42:02.885104 sipiiiii-0.8.3/sipiiiii/app/utils/
+-rw-r--r--   0 j0hn       (501) staff       (20)     7845 2023-05-03 09:19:05.000000 sipiiiii-0.8.3/sipiiiii/app/utils/HttpSDK.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:42:02.890159 sipiiiii-0.8.3/sipiiiii/app/utils/PPI/
+-rw-rw-r--   0 j0hn       (501) staff       (20)      174 2018-04-19 14:27:03.000000 sipiiiii-0.8.3/sipiiiii/app/utils/PPI/__init__.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)      524 2018-04-19 14:27:03.000000 sipiiiii-0.8.3/sipiiiii/app/utils/PPI/generator_factory.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)     6829 2023-04-10 15:58:16.000000 sipiiiii-0.8.3/sipiiiii/app/utils/PPI/prog_class.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)     3470 2018-04-19 14:27:03.000000 sipiiiii-0.8.3/sipiiiii/app/utils/PPI/progbar.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)     2460 2018-04-19 14:27:03.000000 sipiiiii-0.8.3/sipiiiii/app/utils/PPI/progpercent.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1695 2023-05-03 12:17:12.000000 sipiiiii-0.8.3/sipiiiii/app/utils/Tools.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-0.8.3/sipiiiii/app/utils/ZipFileTool.py
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-0.8.3/sipiiiii/app/utils/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      138 2023-05-03 08:02:36.000000 sipiiiii-0.8.3/sipiiiii/app/utils/config.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-0.8.3/sipiiiii/app/utils/formatConversion.py
+-rw-r--r--   0 j0hn       (501) staff       (20)       17 2023-05-03 12:41:46.000000 sipiiiii-0.8.3/sipiiiii/app/version.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     8501 2023-05-03 12:18:55.000000 sipiiiii-0.8.3/sipiiiii/main.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:42:02.874513 sipiiiii-0.8.3/sipiiiii.egg-info/
+-rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-03 12:42:02.000000 sipiiiii-0.8.3/sipiiiii.egg-info/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)      887 2023-05-03 12:42:02.000000 sipiiiii-0.8.3/sipiiiii.egg-info/SOURCES.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-03 12:42:02.000000 sipiiiii-0.8.3/sipiiiii.egg-info/dependency_links.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-03 12:42:02.000000 sipiiiii-0.8.3/sipiiiii.egg-info/entry_points.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)      104 2023-05-03 12:42:02.000000 sipiiiii-0.8.3/sipiiiii.egg-info/requires.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-03 12:42:02.000000 sipiiiii-0.8.3/sipiiiii.egg-info/top_level.txt
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:42:02.894864 sipiiiii-0.8.3/template/
+-rw-r--r--   0 j0hn       (501) staff       (20)      366 2023-04-18 15:46:14.000000 sipiiiii-0.8.3/template/python_fastapi.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      371 2023-04-18 15:46:06.000000 sipiiiii-0.8.3/template/python_flask.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)     1505 2023-05-01 16:17:11.000000 sipiiiii-0.8.3/template/python_openai.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      793 2023-05-01 16:06:19.000000 sipiiiii-0.8.3/template/template_openai.yaml
+-rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-01 16:06:57.000000 sipiiiii-0.8.3/template/template_other.yaml
```

### Comparing `sipiiiii-0.8.2/PKG-INFO` & `sipiiiii-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 0.8.2
+Version: 0.8.3
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sipiiiii-0.8.2/README.md` & `sipiiiii-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.2/pyproject.toml` & `sipiiiii-0.8.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sipiiiii"
-version = "0.8.2"
+version = "0.8.3"
 authors = [
   { name="DeplRun", email="sipiiiii@example.com" },
 ]
 description = "sipiiiii定位为简单易用的云应用托管平台"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `sipiiiii-0.8.2/setup.py` & `sipiiiii-0.8.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,15 @@
 from pathlib import Path
 
 # from version import version
 # from initsipiiiii import init_framework
 
 
 def get_current_path():
-    _path = '~'
-    if os.name == 'nt':
-        _path = R"${TEMP}"
-    home_dir = os.path.expanduser(_path)
-    aiapi_dir = os.path.join(home_dir, ".aiapi")
+    aiapi_dir = os.path.join(Path.home(), ".aiapi")
     if os.path.exists(aiapi_dir):
         return aiapi_dir
     else:
         path = Path(f"{aiapi_dir}")
         path.mkdir(parents=True, exist_ok=True)
         return aiapi_dir
 
@@ -68,15 +64,15 @@
     print(msg)
     sys.exit(1)
 
 setuptools.setup(
     # 包的分发名称，使用字母、数字、_、-
     name="sipiiiii",
     # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
-    version="0.8.2",
+    version="0.8.3",
     # 作者名
     author="sipiiiii@admin",
     # 作者邮箱
     author_email="j0hn.wahahaha@gmail.com",
     # 包的简介描述
     description="depl sipiiiii, App Development Framework",
     # 包的详细介绍(一般通过加载README.md)
```

### Comparing `sipiiiii-0.8.2/sipiiiii/app/core.py` & `sipiiiii-0.8.3/sipiiiii/app/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,19 +308,19 @@
 
     # if openapi_json == {}:
     #     code_yaml = read_app_yaml(directory_path)
 
     # print(f"code_yaml: {openapi_yaml}")
 
     # current_path = get_current_path()
-
+    print(directory_path)
     env = Environment(loader=FileSystemLoader(f"{directory_path}"))
     # template.j2
-    if app_type != "openai":
-        app_type = "other"
+    # if app_type != "openai":
+    #     app_type = "other"
     j2_file = f"{code_type}_{app_type}"
     template = env.get_template(f'{j2_file}.j2')
     output = template.render(paths=openapi_yaml['paths'])
     _fix = fix.get(code_type, None)
     if _fix is None:
         return False
     # Write the output to a Python file
```

### Comparing `sipiiiii-0.8.2/sipiiiii/app/new_app.py` & `sipiiiii-0.8.3/sipiiiii/app/new_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -642,15 +642,15 @@
         table.add_row((app['AppName'], app['AppCnName'], app['Domain'],
                       app['ServerStatus'], app['AppStast'], app['CreateTime']))
 
     return True, table
 
 
 def get_cli_server_version():
-    return "0.8.2"
+    return "0.8.3"
 
 
 def update_template():
     pass
 
 
 def activate_account():
```

### Comparing `sipiiiii-0.8.2/sipiiiii/app/utils/HttpSDK.py` & `sipiiiii-0.8.3/sipiiiii/app/utils/HttpSDK.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.2/sipiiiii/app/utils/PPI/generator_factory.py` & `sipiiiii-0.8.3/sipiiiii/app/utils/PPI/generator_factory.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.2/sipiiiii/app/utils/PPI/prog_class.py` & `sipiiiii-0.8.3/sipiiiii/app/utils/PPI/prog_class.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.2/sipiiiii/app/utils/PPI/progbar.py` & `sipiiiii-0.8.3/sipiiiii/app/utils/PPI/progbar.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.2/sipiiiii/app/utils/PPI/progpercent.py` & `sipiiiii-0.8.3/sipiiiii/app/utils/PPI/progpercent.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.2/sipiiiii/app/utils/Tools.py` & `sipiiiii-0.8.3/sipiiiii/app/utils/Tools.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.2/sipiiiii/app/utils/ZipFileTool.py` & `sipiiiii-0.8.3/sipiiiii/app/utils/ZipFileTool.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.2/sipiiiii/app/utils/formatConversion.py` & `sipiiiii-0.8.3/sipiiiii/app/utils/formatConversion.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.2/sipiiiii/main.py` & `sipiiiii-0.8.3/sipiiiii/main.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.2/sipiiiii.egg-info/PKG-INFO` & `sipiiiii-0.8.3/sipiiiii.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 0.8.2
+Version: 0.8.3
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sipiiiii-0.8.2/sipiiiii.egg-info/SOURCES.txt` & `sipiiiii-0.8.3/sipiiiii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.2/template/python_openai.j2` & `sipiiiii-0.8.3/template/python_openai.j2`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.2/template/template_openai.yaml` & `sipiiiii-0.8.3/template/template_openai.yaml`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.2/template/template_other.yaml` & `sipiiiii-0.8.3/template/template_other.yaml`

 * *Files identical despite different names*

