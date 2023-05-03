# Comparing `tmp/sipiiiii-0.7.4.tar.gz` & `tmp/sipiiiii-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sipiiiii-0.7.4.tar", last modified: Tue May  2 13:33:31 2023, max compression
+gzip compressed data, was "sipiiiii-0.7.5.tar", last modified: Wed May  3 10:07:26 2023, max compression
```

## Comparing `sipiiiii-0.7.4.tar` & `sipiiiii-0.7.5.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-02 13:33:31.615801 sipiiiii-0.7.4/
--rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-02 13:33:31.615073 sipiiiii-0.7.4/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)     3326 2023-05-02 13:20:44.000000 sipiiiii-0.7.4/README.md
--rw-r--r--   0 j0hn       (501) staff       (20)      468 2023-05-02 13:32:45.000000 sipiiiii-0.7.4/pyproject.toml
--rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-02 13:33:31.616112 sipiiiii-0.7.4/setup.cfg
--rw-r--r--   0 j0hn       (501) staff       (20)     1587 2023-05-02 13:22:18.000000 sipiiiii-0.7.4/setup.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-02 13:33:31.587492 sipiiiii-0.7.4/sipiiiii/
--rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-0.7.4/sipiiiii/__init__.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-02 13:33:31.597095 sipiiiii-0.7.4/sipiiiii/app/
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-0.7.4/sipiiiii/app/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)    10610 2023-04-27 14:53:07.000000 sipiiiii-0.7.4/sipiiiii/app/core.py
--rw-r--r--   0 j0hn       (501) staff       (20)    22091 2023-05-02 13:33:08.000000 sipiiiii-0.7.4/sipiiiii/app/new_app.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-02 13:33:31.604911 sipiiiii-0.7.4/sipiiiii/app/utils/
--rw-r--r--   0 j0hn       (501) staff       (20)     7849 2023-04-28 03:07:59.000000 sipiiiii-0.7.4/sipiiiii/app/utils/HttpSDK.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-02 13:33:31.614102 sipiiiii-0.7.4/sipiiiii/app/utils/PPI/
--rw-rw-r--   0 j0hn       (501) staff       (20)      174 2018-04-19 14:27:03.000000 sipiiiii-0.7.4/sipiiiii/app/utils/PPI/__init__.py
--rw-rw-r--   0 j0hn       (501) staff       (20)      524 2018-04-19 14:27:03.000000 sipiiiii-0.7.4/sipiiiii/app/utils/PPI/generator_factory.py
--rw-rw-r--   0 j0hn       (501) staff       (20)     6829 2023-04-10 15:58:16.000000 sipiiiii-0.7.4/sipiiiii/app/utils/PPI/prog_class.py
--rw-rw-r--   0 j0hn       (501) staff       (20)     3470 2018-04-19 14:27:03.000000 sipiiiii-0.7.4/sipiiiii/app/utils/PPI/progbar.py
--rw-rw-r--   0 j0hn       (501) staff       (20)     2460 2018-04-19 14:27:03.000000 sipiiiii-0.7.4/sipiiiii/app/utils/PPI/progpercent.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1653 2023-05-01 16:40:26.000000 sipiiiii-0.7.4/sipiiiii/app/utils/Tools.py
--rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-0.7.4/sipiiiii/app/utils/ZipFileTool.py
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-0.7.4/sipiiiii/app/utils/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)      138 2023-05-02 13:32:29.000000 sipiiiii-0.7.4/sipiiiii/app/utils/config.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-0.7.4/sipiiiii/app/utils/formatConversion.py
--rw-r--r--   0 j0hn       (501) staff       (20)       15 2023-05-02 13:32:52.000000 sipiiiii-0.7.4/sipiiiii/app/version.py
--rw-r--r--   0 j0hn       (501) staff       (20)     8367 2023-05-01 16:20:14.000000 sipiiiii-0.7.4/sipiiiii/main.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-02 13:33:31.592540 sipiiiii-0.7.4/sipiiiii.egg-info/
--rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-02 13:33:31.000000 sipiiiii-0.7.4/sipiiiii.egg-info/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)      707 2023-05-02 13:33:31.000000 sipiiiii-0.7.4/sipiiiii.egg-info/SOURCES.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-02 13:33:31.000000 sipiiiii-0.7.4/sipiiiii.egg-info/dependency_links.txt
--rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-02 13:33:31.000000 sipiiiii-0.7.4/sipiiiii.egg-info/entry_points.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-02 13:33:31.000000 sipiiiii-0.7.4/sipiiiii.egg-info/top_level.txt
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 10:07:26.926427 sipiiiii-0.7.5/
+-rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-03 10:07:26.925765 sipiiiii-0.7.5/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)     3326 2023-05-02 13:20:44.000000 sipiiiii-0.7.5/README.md
+-rw-r--r--   0 j0hn       (501) staff       (20)      468 2023-05-03 10:05:31.000000 sipiiiii-0.7.5/pyproject.toml
+-rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-03 10:07:26.926781 sipiiiii-0.7.5/setup.cfg
+-rw-r--r--   0 j0hn       (501) staff       (20)     1839 2023-05-03 10:04:56.000000 sipiiiii-0.7.5/setup.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 10:07:26.903745 sipiiiii-0.7.5/sipiiiii/
+-rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-0.7.5/sipiiiii/__init__.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 10:07:26.912421 sipiiiii-0.7.5/sipiiiii/app/
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-0.7.5/sipiiiii/app/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    10722 2023-05-03 10:00:47.000000 sipiiiii-0.7.5/sipiiiii/app/core.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    22517 2023-05-03 10:05:09.000000 sipiiiii-0.7.5/sipiiiii/app/new_app.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 10:07:26.918609 sipiiiii-0.7.5/sipiiiii/app/utils/
+-rw-r--r--   0 j0hn       (501) staff       (20)     7845 2023-05-03 09:19:05.000000 sipiiiii-0.7.5/sipiiiii/app/utils/HttpSDK.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 10:07:26.924531 sipiiiii-0.7.5/sipiiiii/app/utils/PPI/
+-rw-rw-r--   0 j0hn       (501) staff       (20)      174 2018-04-19 14:27:03.000000 sipiiiii-0.7.5/sipiiiii/app/utils/PPI/__init__.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)      524 2018-04-19 14:27:03.000000 sipiiiii-0.7.5/sipiiiii/app/utils/PPI/generator_factory.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)     6829 2023-04-10 15:58:16.000000 sipiiiii-0.7.5/sipiiiii/app/utils/PPI/prog_class.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)     3470 2018-04-19 14:27:03.000000 sipiiiii-0.7.5/sipiiiii/app/utils/PPI/progbar.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)     2460 2018-04-19 14:27:03.000000 sipiiiii-0.7.5/sipiiiii/app/utils/PPI/progpercent.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1695 2023-05-03 09:56:22.000000 sipiiiii-0.7.5/sipiiiii/app/utils/Tools.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-0.7.5/sipiiiii/app/utils/ZipFileTool.py
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-0.7.5/sipiiiii/app/utils/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      138 2023-05-03 08:02:36.000000 sipiiiii-0.7.5/sipiiiii/app/utils/config.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-0.7.5/sipiiiii/app/utils/formatConversion.py
+-rw-r--r--   0 j0hn       (501) staff       (20)       15 2023-05-03 10:05:02.000000 sipiiiii-0.7.5/sipiiiii/app/version.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     8501 2023-05-03 09:49:18.000000 sipiiiii-0.7.5/sipiiiii/main.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-03 10:07:26.908619 sipiiiii-0.7.5/sipiiiii.egg-info/
+-rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-03 10:07:26.000000 sipiiiii-0.7.5/sipiiiii.egg-info/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)      738 2023-05-03 10:07:26.000000 sipiiiii-0.7.5/sipiiiii.egg-info/SOURCES.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-03 10:07:26.000000 sipiiiii-0.7.5/sipiiiii.egg-info/dependency_links.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-03 10:07:26.000000 sipiiiii-0.7.5/sipiiiii.egg-info/entry_points.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)      102 2023-05-03 10:07:26.000000 sipiiiii-0.7.5/sipiiiii.egg-info/requires.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-03 10:07:26.000000 sipiiiii-0.7.5/sipiiiii.egg-info/top_level.txt
```

### Comparing `sipiiiii-0.7.4/PKG-INFO` & `sipiiiii-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 0.7.4
+Version: 0.7.5
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sipiiiii-0.7.4/README.md` & `sipiiiii-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.4/setup.py` & `sipiiiii-0.7.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,14 +28,27 @@
     long_description=long_description,
     # 和上条命令配合使用，声明加载的是markdown文件
     long_description_content_type="text/markdown",
     # 项目开源地址
     url="http://www.depl.run/",
     # 如果项目由多个文件组成，我们可以使用find_packages()自动发现所有包和子包，而不是手动列出每个包，在这种情况下，包列表将是example_pkg
     packages=setuptools.find_packages(),
+    install_requires=[
+        'httpx',
+        'prettytable',
+        'jinja2',
+        'requests',
+        'yaml',
+        'shutil',
+        'requests_toolbelt',
+        'xmltodict',
+        'validators',
+        'pathlib',
+        'jsonpath'
+    ],
     entry_points={
         'console_scripts': [
             'sipiiiii = sipiiiii.main:main'
         ]
     },
     # 关于包的其他元数据(metadata)
     classifiers=[
```

### Comparing `sipiiiii-0.7.4/sipiiiii/app/core.py` & `sipiiiii-0.7.5/sipiiiii/app/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,14 +205,16 @@
     new_fix = {v: k for k, v in fix.items()}
     return True, new_fix[_fix]
 
 
 def yaml_app_info(yaml_file, app_type):
     openapi_yaml = None
     aiapi_dir = get_current_path()
+    if app_type != "openai":
+        app_type = "other"
     if yaml_file is None:
         openapi_yaml = read_app_yaml(aiapi_dir, app_type)
     else:
         openapi_yaml = read_app_yaml(yaml_file, app_type)
     if openapi_yaml == "":
         return False, "没找到yaml文件.", None, None
     app_name = ""
@@ -309,14 +311,16 @@
 
     # print(f"code_yaml: {openapi_yaml}")
 
     # current_path = get_current_path()
 
     env = Environment(loader=FileSystemLoader(f"{directory_path}"))
     # template.j2
+    if app_type != "openai":
+        app_type = "other"
     j2_file = f"{code_type}_{app_type}"
     template = env.get_template(f'{j2_file}.j2')
     output = template.render(paths=openapi_yaml['paths'])
     _fix = fix.get(code_type, None)
     if _fix is None:
         return False
     # Write the output to a Python file
```

### Comparing `sipiiiii-0.7.4/sipiiiii/app/new_app.py` & `sipiiiii-0.7.5/sipiiiii/app/new_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,55 +50,58 @@
     return True, _token
 
 
 # 创建项目
 def create_app_project():
     status, _token = get_token()
     if not status:
-        return False, _token
+        return False, _token, ""
 
     print("""
     *** 应用名称必须英文
     *** 可以使用向导模式创建应用和使用模版创建应用
         """)
 
-    app_name = input("请输入应用名:")
-    if app_name == "":
-        return False, "项目名不能为空"
-    if not is_encomm_char(app_name):
-        return False, "项目名必须是英文"
-
-    app_desc = input("请输入应用说明:")
-    app_version = input("请输入应用版本(不输入默认 v1.0):")
-    if app_version == "":
-        app_version = "v1.0"
-    print(f"项目名: {app_name}, 项目说明: {app_desc}, 项目版本: {app_version}")
     while True:
         is_ai_create = input("是否使用向导创建应用(y/n):")
         is_ai_create = is_ai_create.lower()
-
+        
         if is_ai_create == "y":
+            app_name = input("请输入应用名:")
+            if app_name == "":
+                return False, "项目名不能为空", ""
+            if not is_encomm_char(app_name):
+                return False, "项目名必须是英文", ""
+
+            app_desc = input("请输入应用说明:")
+            app_version = input("请输入应用版本(不输入默认 v1.0):")
+            if app_version == "":
+                app_version = "v1.0"
+            print(f"项目名: {app_name}, 项目说明: {app_desc}, 项目版本: {app_version}")
             status, yaml_data = create_yaml(
                 app_name, app_version, app_desc)
             if not status:
                 print(yaml_data)
 
             with open(f"{os.getcwd()}{os.sep}aiapi.yaml", "w", encoding="utf-8") as f:
                 f.write(yaml_data)
 
-            status, msg = create_app(f"{os.getcwd()}{os.sep}aiapi.yaml")
+            status, msg, app_name = create_app(f"{os.getcwd()}{os.sep}aiapi.yaml")
+            if status:
+                write_new_yaml(f"{msg}{os.sep}aiapi.yaml")
+            
             os.remove(f"{os.getcwd()}{os.sep}aiapi.yaml")
-            return status, msg
+            return status, msg, app_name
         elif is_ai_create == "n":
-            status, msg = create_app(None)
-            if status:
-                write_new_yaml(f"{app_name}{os.sep}aiapi.yaml")
+            status, msg, app_name = create_app(None)
+            # if status:
+            #     write_new_yaml(f"{msg}{os.sep}aiapi.yaml")
             break
-
-    return status, msg
+    
+    return status, msg, app_name
 
 
 # 创建yaml模版
 def create_yaml(app_name, app_version, app_desc):
     status, _token = get_token()
     if not status:
         return False, _token
@@ -162,39 +165,39 @@
 
 # 通过yaml直接创建APP
 
 
 def create_app(yaml_file=None):
     status, _token = get_token()
     if not status:
-        return False, _token
+        return False, _token, ""
 
     code_type = input(
         f"请输入创建编程语言{list(fix.keys())}: "
     )
 
     _code_type = app_all_types.get(code_type, None)
     if _code_type is None:
-        return False, f"输入的编程语言的范围: {list(fix.keys())}"
+        return False, f"输入的编程语言的范围: {list(fix.keys())}", ""
 
     app_type = input(
         f"请创建应用程序类型({', '.join(app_all_types[code_type])}): "
     )
 
     if app_type not in app_all_types[code_type]:
-        return False, f"输入应用程序的范围: {app_all_types[code_type]}"
-
+        return False, f"输入应用程序的范围: {app_all_types[code_type]}", ""
+        
     status, app_name, app_yaml, app_dir = yaml_app_info(yaml_file, app_type)
     if not status:
-        return False, app_name
+        return False, app_name, ""
 
     catc = CreateAppTypeClass(app_name, app_yaml, app_dir)
     method_of_catc = getattr(catc, f"create_{app_type}_app")
     status, msg = method_of_catc(code_type)
-    return status, msg
+    return status, msg, app_name
 
 
 def dev_app():
     print("测试运行....\r\n")
     run_main = input("请输入APP运行文件:")
     cwd = os.getcwd()
     # file_path = os.path.join(cwd, "ai-plugin.json")
@@ -467,15 +470,19 @@
     if not response.success:
         return False, response.msg
 
     home_dir_file = os.path.join(Path.home(), ".sipitoken")
     with open(home_dir_file, 'w', encoding='utf-8') as f:
         f.write(response.data['token'])
 
-    return True, "登录成功, 登录有效期3天."
+    status, tally = get_tally()
+    if status:
+        return True, f"登录成功, 登录有效期3天, 剩余积分: {tally}"
+    
+    return False, "登录成功, 登录有效期3天, 获取积分失败."
 
 
 def init_framework():
     aiapi_dir = get_current_path()
 
     # Replace 'template/template.yaml' with the path to the file you want to copy
     # src_file = f'sipiiiii{os.sep}template/template.yaml'
@@ -634,15 +641,15 @@
         table.add_row((app['AppName'], app['AppCnName'], app['Domain'],
                       app['ServerStatus'], app['AppStast'], app['CreateTime']))
 
     return True, table
 
 
 def get_cli_server_version():
-    return "0.7.4"
+    return "0.7.5"
 
 
 def update_template():
     pass
 
 
 def activate_account():
```

### Comparing `sipiiiii-0.7.4/sipiiiii/app/utils/HttpSDK.py` & `sipiiiii-0.7.5/sipiiiii/app/utils/HttpSDK.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 try:
-    from .formatConversion import verify_json, DottableDict
+    from utils.formatConversion import verify_json, DottableDict
 except ImportError:
-    from app.utils.formatConversion import verify_json, DottableDict
+    from .formatConversion import verify_json, DottableDict
 
 import validators
 import httpx
 import time
 
 
 def log_request(request):
```

### Comparing `sipiiiii-0.7.4/sipiiiii/app/utils/PPI/generator_factory.py` & `sipiiiii-0.7.5/sipiiiii/app/utils/PPI/generator_factory.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.4/sipiiiii/app/utils/PPI/prog_class.py` & `sipiiiii-0.7.5/sipiiiii/app/utils/PPI/prog_class.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.4/sipiiiii/app/utils/PPI/progbar.py` & `sipiiiii-0.7.5/sipiiiii/app/utils/PPI/progbar.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.4/sipiiiii/app/utils/PPI/progpercent.py` & `sipiiiii-0.7.5/sipiiiii/app/utils/PPI/progpercent.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.4/sipiiiii/app/utils/Tools.py` & `sipiiiii-0.7.5/sipiiiii/app/utils/Tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 import yaml
 import os
+from pathlib import Path
 
 
 def get_outside_ip():
     ip = ""
     try:
         ip = requests.get("http://ifconfig.me/ip", timeout=5).text.strip()
     except Exception as e:
@@ -39,15 +40,16 @@
         if directory_path.find(".yaml") == -1:
             openapi_yaml_file_path = os.path.join(
                 directory_path, f"template_{app_type}.yaml")
     try:
         with open(openapi_yaml_file_path, "r", encoding="utf-8") as f:
             openapi_yaml = f.read()
         openapi_yaml = yaml.safe_load(openapi_yaml)
-    except Exception as _:
+    except Exception as e:
+        print(e)
         return ""
     return openapi_yaml
 
 
 def write_new_yaml(yaml_file):
     with open(yaml_file, "r", encoding="utf-8") as f:
         openapi_yaml = f.read()
```

### Comparing `sipiiiii-0.7.4/sipiiiii/app/utils/ZipFileTool.py` & `sipiiiii-0.7.5/sipiiiii/app/utils/ZipFileTool.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.4/sipiiiii/app/utils/formatConversion.py` & `sipiiiii-0.7.5/sipiiiii/app/utils/formatConversion.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.4/sipiiiii/main.py` & `sipiiiii-0.7.5/sipiiiii/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -139,19 +139,22 @@
         print(msg)
 
     elif args['new']:
         # execute new code here
         status = False
         msg = ""
         if args['new'] == "default_value":
-            status, msg = create_app_project()
+            status, msg, app_name = create_app_project()
         else:
-            status, msg = create_app(args['new'])
+            status, msg, app_name = create_app(args['new'])
 
-        print(msg)
+        if status:
+            print(f"{msg} 项目目录在当前文件夹下的: {app_name}")
+        else:
+            print(msg)
 
     elif args['login']:
         email = input("输入你的email:")
         password = getpass.getpass('输入你的密码:')
         if email == "" or email is None:
             print("没有输入email.")
             sys.exit(1)
```

### Comparing `sipiiiii-0.7.4/sipiiiii.egg-info/PKG-INFO` & `sipiiiii-0.7.5/sipiiiii.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 0.7.4
+Version: 0.7.5
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sipiiiii-0.7.4/sipiiiii.egg-info/SOURCES.txt` & `sipiiiii-0.7.5/sipiiiii.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 sipiiiii/__init__.py
 sipiiiii/main.py
 sipiiiii.egg-info/PKG-INFO
 sipiiiii.egg-info/SOURCES.txt
 sipiiiii.egg-info/dependency_links.txt
 sipiiiii.egg-info/entry_points.txt
+sipiiiii.egg-info/requires.txt
 sipiiiii.egg-info/top_level.txt
 sipiiiii/app/__init__.py
 sipiiiii/app/core.py
 sipiiiii/app/new_app.py
 sipiiiii/app/version.py
 sipiiiii/app/utils/HttpSDK.py
 sipiiiii/app/utils/Tools.py
```

