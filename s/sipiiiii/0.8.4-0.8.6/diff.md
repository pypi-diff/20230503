# Comparing `tmp/sipiiiii-0.8.4.tar.gz` & `tmp/sipiiiii-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sipiiiii-0.8.4.tar", last modified: Wed May  3 12:49:10 2023, max compression
+gzip compressed data, was "sipiiiii-0.8.6.tar", last modified: Wed May  3 13:34:58 2023, max compression
```

## Comparing `sipiiiii-0.8.4.tar` & `sipiiiii-0.8.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:49:10.836391 sipiiiii-0.8.4/
--rw-r--r--   0 j0hn       (501) staff       (20)       18 2023-05-03 12:00:50.000000 sipiiiii-0.8.4/MANIFEST.in
--rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-03 12:49:10.835783 sipiiiii-0.8.4/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)     3326 2023-05-02 13:20:44.000000 sipiiiii-0.8.4/README.md
--rw-r--r--   0 j0hn       (501) staff       (20)      634 2023-05-03 12:48:51.000000 sipiiiii-0.8.4/pyproject.toml
--rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-03 12:49:10.836574 sipiiiii-0.8.4/setup.cfg
--rw-r--r--   0 j0hn       (501) staff       (20)     3401 2023-05-03 12:48:51.000000 sipiiiii-0.8.4/setup.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:49:10.791375 sipiiiii-0.8.4/sipiiiii/
--rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-0.8.4/sipiiiii/__init__.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:49:10.803313 sipiiiii-0.8.4/sipiiiii/app/
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-0.8.4/sipiiiii/app/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)    10751 2023-05-03 12:36:45.000000 sipiiiii-0.8.4/sipiiiii/app/core.py
--rw-r--r--   0 j0hn       (501) staff       (20)    22498 2023-05-03 12:48:51.000000 sipiiiii-0.8.4/sipiiiii/app/new_app.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:49:10.822655 sipiiiii-0.8.4/sipiiiii/app/utils/
--rw-r--r--   0 j0hn       (501) staff       (20)     7845 2023-05-03 09:19:05.000000 sipiiiii-0.8.4/sipiiiii/app/utils/HttpSDK.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:49:10.829665 sipiiiii-0.8.4/sipiiiii/app/utils/PPI/
--rw-rw-r--   0 j0hn       (501) staff       (20)      174 2018-04-19 14:27:03.000000 sipiiiii-0.8.4/sipiiiii/app/utils/PPI/__init__.py
--rw-rw-r--   0 j0hn       (501) staff       (20)      524 2018-04-19 14:27:03.000000 sipiiiii-0.8.4/sipiiiii/app/utils/PPI/generator_factory.py
--rw-rw-r--   0 j0hn       (501) staff       (20)     6829 2023-04-10 15:58:16.000000 sipiiiii-0.8.4/sipiiiii/app/utils/PPI/prog_class.py
--rw-rw-r--   0 j0hn       (501) staff       (20)     3470 2018-04-19 14:27:03.000000 sipiiiii-0.8.4/sipiiiii/app/utils/PPI/progbar.py
--rw-rw-r--   0 j0hn       (501) staff       (20)     2460 2018-04-19 14:27:03.000000 sipiiiii-0.8.4/sipiiiii/app/utils/PPI/progpercent.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1590 2023-05-03 12:48:37.000000 sipiiiii-0.8.4/sipiiiii/app/utils/Tools.py
--rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-0.8.4/sipiiiii/app/utils/ZipFileTool.py
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-0.8.4/sipiiiii/app/utils/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)      138 2023-05-03 08:02:36.000000 sipiiiii-0.8.4/sipiiiii/app/utils/config.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-0.8.4/sipiiiii/app/utils/formatConversion.py
--rw-r--r--   0 j0hn       (501) staff       (20)       17 2023-05-03 12:48:51.000000 sipiiiii-0.8.4/sipiiiii/app/version.py
--rw-r--r--   0 j0hn       (501) staff       (20)     8501 2023-05-03 12:18:55.000000 sipiiiii-0.8.4/sipiiiii/main.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:49:10.798433 sipiiiii-0.8.4/sipiiiii.egg-info/
--rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-03 12:49:10.000000 sipiiiii-0.8.4/sipiiiii.egg-info/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)      887 2023-05-03 12:49:10.000000 sipiiiii-0.8.4/sipiiiii.egg-info/SOURCES.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-03 12:49:10.000000 sipiiiii-0.8.4/sipiiiii.egg-info/dependency_links.txt
--rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-03 12:49:10.000000 sipiiiii-0.8.4/sipiiiii.egg-info/entry_points.txt
--rw-r--r--   0 j0hn       (501) staff       (20)      104 2023-05-03 12:49:10.000000 sipiiiii-0.8.4/sipiiiii.egg-info/requires.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-03 12:49:10.000000 sipiiiii-0.8.4/sipiiiii.egg-info/top_level.txt
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 12:49:10.834625 sipiiiii-0.8.4/template/
--rw-r--r--   0 j0hn       (501) staff       (20)      366 2023-04-18 15:46:14.000000 sipiiiii-0.8.4/template/python_fastapi.j2
--rw-r--r--   0 j0hn       (501) staff       (20)      371 2023-04-18 15:46:06.000000 sipiiiii-0.8.4/template/python_flask.j2
--rw-r--r--   0 j0hn       (501) staff       (20)     1505 2023-05-01 16:17:11.000000 sipiiiii-0.8.4/template/python_openai.j2
--rw-r--r--   0 j0hn       (501) staff       (20)      793 2023-05-01 16:06:19.000000 sipiiiii-0.8.4/template/template_openai.yaml
--rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-01 16:06:57.000000 sipiiiii-0.8.4/template/template_other.yaml
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 13:34:58.722109 sipiiiii-0.8.6/
+-rw-r--r--   0 j0hn       (501) staff       (20)       18 2023-05-03 12:00:50.000000 sipiiiii-0.8.6/MANIFEST.in
+-rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-03 13:34:58.721438 sipiiiii-0.8.6/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)     3326 2023-05-02 13:20:44.000000 sipiiiii-0.8.6/README.md
+-rw-r--r--   0 j0hn       (501) staff       (20)      634 2023-05-03 13:25:35.000000 sipiiiii-0.8.6/pyproject.toml
+-rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-03 13:34:58.722332 sipiiiii-0.8.6/setup.cfg
+-rw-r--r--   0 j0hn       (501) staff       (20)     3401 2023-05-03 13:25:35.000000 sipiiiii-0.8.6/setup.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 13:34:58.674990 sipiiiii-0.8.6/sipiiiii/
+-rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-0.8.6/sipiiiii/__init__.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 13:34:58.687572 sipiiiii-0.8.6/sipiiiii/app/
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-0.8.6/sipiiiii/app/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    10430 2023-05-03 13:32:57.000000 sipiiiii-0.8.6/sipiiiii/app/core.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    22667 2023-05-03 13:29:55.000000 sipiiiii-0.8.6/sipiiiii/app/new_app.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 13:34:58.702240 sipiiiii-0.8.6/sipiiiii/app/utils/
+-rw-r--r--   0 j0hn       (501) staff       (20)     7845 2023-05-03 09:19:05.000000 sipiiiii-0.8.6/sipiiiii/app/utils/HttpSDK.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 13:34:58.713683 sipiiiii-0.8.6/sipiiiii/app/utils/PPI/
+-rw-rw-r--   0 j0hn       (501) staff       (20)      174 2018-04-19 14:27:03.000000 sipiiiii-0.8.6/sipiiiii/app/utils/PPI/__init__.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)      524 2018-04-19 14:27:03.000000 sipiiiii-0.8.6/sipiiiii/app/utils/PPI/generator_factory.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)     6829 2023-04-10 15:58:16.000000 sipiiiii-0.8.6/sipiiiii/app/utils/PPI/prog_class.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)     3470 2018-04-19 14:27:03.000000 sipiiiii-0.8.6/sipiiiii/app/utils/PPI/progbar.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)     2460 2018-04-19 14:27:03.000000 sipiiiii-0.8.6/sipiiiii/app/utils/PPI/progpercent.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1598 2023-05-03 13:30:01.000000 sipiiiii-0.8.6/sipiiiii/app/utils/Tools.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-0.8.6/sipiiiii/app/utils/ZipFileTool.py
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-0.8.6/sipiiiii/app/utils/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      138 2023-05-03 08:02:36.000000 sipiiiii-0.8.6/sipiiiii/app/utils/config.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-0.8.6/sipiiiii/app/utils/formatConversion.py
+-rw-r--r--   0 j0hn       (501) staff       (20)       17 2023-05-03 13:25:35.000000 sipiiiii-0.8.6/sipiiiii/app/version.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     8501 2023-05-03 12:18:55.000000 sipiiiii-0.8.6/sipiiiii/main.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 13:34:58.683323 sipiiiii-0.8.6/sipiiiii.egg-info/
+-rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-03 13:34:58.000000 sipiiiii-0.8.6/sipiiiii.egg-info/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)      887 2023-05-03 13:34:58.000000 sipiiiii-0.8.6/sipiiiii.egg-info/SOURCES.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-03 13:34:58.000000 sipiiiii-0.8.6/sipiiiii.egg-info/dependency_links.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-03 13:34:58.000000 sipiiiii-0.8.6/sipiiiii.egg-info/entry_points.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)      104 2023-05-03 13:34:58.000000 sipiiiii-0.8.6/sipiiiii.egg-info/requires.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-03 13:34:58.000000 sipiiiii-0.8.6/sipiiiii.egg-info/top_level.txt
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 13:34:58.720305 sipiiiii-0.8.6/template/
+-rw-r--r--   0 j0hn       (501) staff       (20)      366 2023-04-18 15:46:14.000000 sipiiiii-0.8.6/template/python_fastapi.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      371 2023-04-18 15:46:06.000000 sipiiiii-0.8.6/template/python_flask.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)     1505 2023-05-01 16:17:11.000000 sipiiiii-0.8.6/template/python_openai.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      795 2023-05-03 13:15:30.000000 sipiiiii-0.8.6/template/template_openai.yaml
+-rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-01 16:06:57.000000 sipiiiii-0.8.6/template/template_other.yaml
```

### Comparing `sipiiiii-0.8.4/PKG-INFO` & `sipiiiii-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 0.8.4
+Version: 0.8.6
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sipiiiii-0.8.4/README.md` & `sipiiiii-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.4/pyproject.toml` & `sipiiiii-0.8.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sipiiiii"
-version = "0.8.4"
+version = "0.8.6"
 authors = [
   { name="DeplRun", email="sipiiiii@example.com" },
 ]
 description = "sipiiiii定位为简单易用的云应用托管平台"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `sipiiiii-0.8.4/setup.py` & `sipiiiii-0.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     print(msg)
     sys.exit(1)
 
 setuptools.setup(
     # 包的分发名称，使用字母、数字、_、-
     name="sipiiiii",
     # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
-    version="0.8.4",
+    version="0.8.6",
     # 作者名
     author="sipiiiii@admin",
     # 作者邮箱
     author_email="j0hn.wahahaha@gmail.com",
     # 包的简介描述
     description="depl sipiiiii, App Development Framework",
     # 包的详细介绍(一般通过加载README.md)
```

### Comparing `sipiiiii-0.8.4/sipiiiii/app/core.py` & `sipiiiii-0.8.6/sipiiiii/app/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,56 +267,44 @@
         return False, "应用配置文件错误!"
 
     if not os.path.exists(directory_path):
         return False, f"{directory_path} 目录没有找到."
 
     # ai-plugin.json
     if app_type == "openai":
-        app_type = "ai-plugin.json"
+        app_type = "ai-plugin"
     else:
-        app_type = "config.json"
+        app_type = "config"
 
     plugin_json_file_path = os.path.join(directory_path, f"{app_type}.json")
     # plugin_json_data = "\n".join(plugin_json_file_path)
     with open(plugin_json_file_path, encoding="utf-8", mode="w") as f:
         json.dump(plugin_json, f, indent=2)
 
     return True, plugin_json_file_path
 
 
 def create_app_yaml(directory_path, openapi_yaml, app_type):
     if not os.path.exists(directory_path):
         return False, f"{directory_path} 目录不存在"
 
-    openapi_yaml_file_path = os.path.join(directory_path, f"{app_type}.yaml")
-    if app_type is None:
-        openapi_yaml_file_path = os.path.join(directory_path, f"aiapi.yaml")
+    # openapi_yaml_file_path = os.path.join(directory_path, f"{app_type}.yaml")
+    # if app_type is None:
+    openapi_yaml_file_path = os.path.join(directory_path, "aiapi.yaml")
     # openapi.yaml
     # openapi_yaml_file_path = os.path.join(directory_path, f"{app_type}.yaml")
 
     # plugin_json_data = "\n".join(plugin_json_file_path)
     with open(openapi_yaml_file_path, encoding="utf-8", mode="w") as f:
         yaml.dump(openapi_yaml, stream=f, allow_unicode=True)
 
     return True, openapi_yaml_file_path
 
 
 def create_framework_code(directory_path, app_path, openapi_yaml, code_type, app_type):
-    # if type(openapi_json) != dict:
-    #     return False, "openapi_json error!"
-
-    # code_yaml = openapi_json.copy()
-
-    # if openapi_json == {}:
-    #     code_yaml = read_app_yaml(directory_path)
-
-    # print(f"code_yaml: {openapi_yaml}")
-
-    # current_path = get_current_path()
-    print(directory_path)
     env = Environment(loader=FileSystemLoader(f"{directory_path}"))
     # template.j2
     # if app_type != "openai":
     #     app_type = "other"
     j2_file = f"{code_type}_{app_type}"
     template = env.get_template(f'{j2_file}.j2')
     output = template.render(paths=openapi_yaml['paths'])
@@ -325,7 +313,8 @@
         return False
     # Write the output to a Python file
     app_file = os.path.join(app_path, f"app.{_fix}")
     with open(app_file, 'w', encoding="utf-8") as f:
         f.write(output)
 
     return True
+
```

### Comparing `sipiiiii-0.8.4/sipiiiii/app/new_app.py` & `sipiiiii-0.8.6/sipiiiii/app/new_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 from pathlib import Path
 from shutil import copyfile
 
 from .core import CreateAppTypeClass, yaml_app_info, ExecAppClass, get_app_code_type, get_app_name
 
-from .utils.PPI import ProgPercent
+# from .utils.PPI import ProgPercent
 from .utils.ZipFileTool import zip_folder
 from .utils.HttpSDK import https_get, https_post, https_file
 from .utils.Tools import get_outside_ip, is_encomm_char, write_new_yaml, get_current_path
 from .utils.config import app_all_types, server_host, fix
 
 
 def process_update_outside_ip(domain, _token):
@@ -64,36 +64,41 @@
     while True:
         is_ai_create = input("是否使用向导创建应用(y/n):")
         is_ai_create = is_ai_create.lower()
 
         if is_ai_create == "y":
             app_name = input("请输入应用名:")
             if app_name == "":
-                return False, "项目名不能为空", ""
+                print("项目名不能为空")
+                continue
             if not is_encomm_char(app_name):
-                return False, "项目名必须是英文", ""
+                print("项目名必须是英文")
+                continue
 
             app_desc = input("请输入应用说明:")
             app_version = input("请输入应用版本(不输入默认 v1.0):")
             if app_version == "":
                 app_version = "v1.0"
             print(f"项目名: {app_name}, 项目说明: {app_desc}, 项目版本: {app_version}")
+
             status, yaml_data = create_yaml(
                 app_name, app_version, app_desc)
             if not status:
                 print(yaml_data)
+                continue
 
             with open(f"{os.getcwd()}{os.sep}aiapi.yaml", "w", encoding="utf-8") as f:
                 f.write(yaml_data)
 
             status, msg, app_name = create_app(
                 f"{os.getcwd()}{os.sep}aiapi.yaml")
             if status:
-                write_new_yaml(f"{msg}{os.sep}aiapi.yaml")
-
+                write_new_yaml(
+                    f"{os.getcwd()}{os.sep}{app_name}{os.sep}aiapi.yaml")
+            
             os.remove(f"{os.getcwd()}{os.sep}aiapi.yaml")
             return status, msg, app_name
         elif is_ai_create == "n":
             status, msg, app_name = create_app(None)
             # if status:
             #     write_new_yaml(f"{msg}{os.sep}aiapi.yaml")
             break
@@ -433,30 +438,30 @@
 
     # return True, "ok"
 
     status, info_json, _ = get_app_info(filename)
     if not status:
         return False, "部署成功，状态获取失败"
 
-    bar = ProgPercent(50, monitor=True)
+    # bar = ProgPercent(50, monitor=True)
     print("正在远程部署...\r\n")
     while True:
         status, info_json, _ = get_app_info(filename)
         if not status:
-            bar.update(50)
+            # bar.update(50)
             return False, "\r\n部署成功，状态获取失败"
         if info_json['ServerStatus'] == "close" or info_json['ServerStatus'] == "exited":
-            bar.update(50)
+            # bar.update(50)
             return True, f"\r\n应用程序部署出错，日志: \r\n{info_json['Log']}"
 
         if info_json['ServerStatus'] == "created" or info_json['ServerStatus'] == "running":
-            bar.update(50)
+            # bar.update(50)
             return True, f"\r\n部署成功, \r\n域名: {info_json['Domain']}"
 
-    return True, response.data
+    # return True, response.data
 
 
 def login(email, password):
     url = f"{server_host}/system/openapi/users/login"
     headers = {
         "Content-type": "application/json"
     }
@@ -478,42 +483,42 @@
     status, tally = get_tally()
     if status:
         return True, f"登录成功, 登录有效期3天, 剩余积分: {tally}"
 
     return False, "登录成功, 登录有效期3天, 获取积分失败."
 
 
-def init_framework():
-    aiapi_dir = get_current_path()
+# def init_framework():
+#     aiapi_dir = get_current_path()
 
-    # Replace 'template/template.yaml' with the path to the file you want to copy
-    # src_file = f'sipiiiii{os.sep}template/template.yaml'
-    src_dir = os.path.join("sipiiiii", "template")
-
-    template_files = os.listdir(src_dir)
-    for tFIle in template_files:
-        src_file = os.path.join(src_dir, tFIle)
-
-        # Use Path().resolve() to get the absolute path of the source file
-        src_path = Path(src_file).resolve()
-
-        # Use Path().joinpath() to get the destination path
-        dest_path = Path(aiapi_dir).joinpath(tFIle)
-        # Use Path().replace() to copy the file
-        try:
-            copyfile(src_path, dest_path)
-        except Exception as e:
-            print(str(e))
-            continue
-
-        # Check if the file was copied successfully
-        if not dest_path.exists():
-            continue
+#     # Replace 'template/template.yaml' with the path to the file you want to copy
+#     # src_file = f'sipiiiii{os.sep}template/template.yaml'
+#     src_dir = os.path.join("sipiiiii", "template")
+
+#     template_files = os.listdir(src_dir)
+#     for tFIle in template_files:
+#         src_file = os.path.join(src_dir, tFIle)
+
+#         # Use Path().resolve() to get the absolute path of the source file
+#         src_path = Path(src_file).resolve()
+
+#         # Use Path().joinpath() to get the destination path
+#         dest_path = Path(aiapi_dir).joinpath(tFIle)
+#         # Use Path().replace() to copy the file
+#         try:
+#             copyfile(src_path, dest_path)
+#         except Exception as e:
+#             print(str(e))
+#             continue
+
+#         # Check if the file was copied successfully
+#         if not dest_path.exists():
+#             continue
 
-    return True, "初始化成功"
+#     return True, "初始化成功"
 
 
 def get_tally():
     status, _token = get_token()
     if not status:
         return False, _token
 
@@ -642,15 +647,15 @@
         table.add_row((app['AppName'], app['AppCnName'], app['Domain'],
                       app['ServerStatus'], app['AppStast'], app['CreateTime']))
 
     return True, table
 
 
 def get_cli_server_version():
-    return "0.8.4"
+    return "0.8.6"
 
 
 def update_template():
     pass
 
 
 def activate_account():
```

### Comparing `sipiiiii-0.8.4/sipiiiii/app/utils/HttpSDK.py` & `sipiiiii-0.8.6/sipiiiii/app/utils/HttpSDK.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.4/sipiiiii/app/utils/PPI/generator_factory.py` & `sipiiiii-0.8.6/sipiiiii/app/utils/PPI/generator_factory.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.4/sipiiiii/app/utils/PPI/prog_class.py` & `sipiiiii-0.8.6/sipiiiii/app/utils/PPI/prog_class.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.4/sipiiiii/app/utils/PPI/progbar.py` & `sipiiiii-0.8.6/sipiiiii/app/utils/PPI/progbar.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.4/sipiiiii/app/utils/PPI/progpercent.py` & `sipiiiii-0.8.6/sipiiiii/app/utils/PPI/progpercent.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.4/sipiiiii/app/utils/Tools.py` & `sipiiiii-0.8.6/sipiiiii/app/utils/Tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,11 +51,11 @@
         openapi_yaml = f.read()
     openapi_yaml = yaml.safe_load(openapi_yaml)
     openapi_yaml['openapi'] = "3.0.1"
     del openapi_yaml['swagger']
     with open(f"{os.getcwd()}{os.sep}aiapi.yaml", "w", encoding="utf") as f:
         yaml.dump(openapi_yaml, stream=f, allow_unicode=True)
 
-    try:
-        os.remove(yaml_file)
-    except Exception as _:
-        pass
+    # try:
+    #     os.remove(yaml_file)
+    # except Exception as _:
+    #     pass
```

### Comparing `sipiiiii-0.8.4/sipiiiii/app/utils/ZipFileTool.py` & `sipiiiii-0.8.6/sipiiiii/app/utils/ZipFileTool.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.4/sipiiiii/app/utils/formatConversion.py` & `sipiiiii-0.8.6/sipiiiii/app/utils/formatConversion.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.4/sipiiiii/main.py` & `sipiiiii-0.8.6/sipiiiii/main.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.4/sipiiiii.egg-info/PKG-INFO` & `sipiiiii-0.8.6/sipiiiii.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 0.8.4
+Version: 0.8.6
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sipiiiii-0.8.4/sipiiiii.egg-info/SOURCES.txt` & `sipiiiii-0.8.6/sipiiiii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.4/template/python_openai.j2` & `sipiiiii-0.8.6/template/python_openai.j2`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.4/template/template_openai.yaml` & `sipiiiii-0.8.6/template/template_openai.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 openapi: 3.0.1
 info:
   title: OpenAi Framework
   description: Get current and historical stats for sport players and games.
   version: 'v1'
 servers:
-  - url: !HOSTNAME!
+  - url: '!HOSTNAME!'
 paths:
   /players:
     get:
       operationId: getPlayers
       summary: Retrieves all players from all seasons whose names match the query string.
       parameters:
       - in: query
```

### Comparing `sipiiiii-0.8.4/template/template_other.yaml` & `sipiiiii-0.8.6/template/template_other.yaml`

 * *Files identical despite different names*

