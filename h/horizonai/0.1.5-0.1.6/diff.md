# Comparing `tmp/horizonai-0.1.5.tar.gz` & `tmp/horizonai-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horizonai-0.1.5.tar", last modified: Wed May  3 20:18:49 2023, max compression
+gzip compressed data, was "horizonai-0.1.6.tar", last modified: Wed May  3 20:41:19 2023, max compression
```

## Comparing `horizonai-0.1.5.tar` & `horizonai-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-03 20:18:49.967282 horizonai-0.1.5/
--rw-r--r--   0 linatawfik   (501) staff       (20)     1070 2023-05-03 16:55:57.000000 horizonai-0.1.5/LICENSE
--rw-r--r--   0 linatawfik   (501) staff       (20)     2313 2023-05-03 20:18:49.967351 horizonai-0.1.5/PKG-INFO
--rw-r--r--   0 linatawfik   (501) staff       (20)     1575 2023-05-03 16:55:57.000000 horizonai-0.1.5/README.md
-drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-03 20:18:49.966407 horizonai-0.1.5/horizonai/
--rw-r--r--   0 linatawfik   (501) staff       (20)       83 2023-05-03 20:15:40.000000 horizonai-0.1.5/horizonai/__init__.py
--rw-r--r--   0 linatawfik   (501) staff       (20)     1542 2023-05-03 20:09:16.000000 horizonai-0.1.5/horizonai/base.py
--rw-r--r--   0 linatawfik   (501) staff       (20)    14474 2023-05-03 18:31:03.000000 horizonai-0.1.5/horizonai/cli.py
--rw-r--r--   0 linatawfik   (501) staff       (20)     1206 2023-05-03 16:55:57.000000 horizonai-0.1.5/horizonai/project.py
--rw-r--r--   0 linatawfik   (501) staff       (20)     3288 2023-05-03 16:55:57.000000 horizonai-0.1.5/horizonai/task.py
--rw-r--r--   0 linatawfik   (501) staff       (20)      355 2023-05-03 16:55:57.000000 horizonai-0.1.5/horizonai/user.py
-drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-03 20:18:49.967181 horizonai-0.1.5/horizonai.egg-info/
--rw-r--r--   0 linatawfik   (501) staff       (20)     2313 2023-05-03 20:18:49.000000 horizonai-0.1.5/horizonai.egg-info/PKG-INFO
--rw-r--r--   0 linatawfik   (501) staff       (20)      350 2023-05-03 20:18:49.000000 horizonai-0.1.5/horizonai.egg-info/SOURCES.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)        1 2023-05-03 20:18:49.000000 horizonai-0.1.5/horizonai.egg-info/dependency_links.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)       46 2023-05-03 20:18:49.000000 horizonai-0.1.5/horizonai.egg-info/entry_points.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)       15 2023-05-03 20:18:49.000000 horizonai-0.1.5/horizonai.egg-info/requires.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)       10 2023-05-03 20:18:49.000000 horizonai-0.1.5/horizonai.egg-info/top_level.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)       79 2023-05-03 20:18:49.967566 horizonai-0.1.5/setup.cfg
--rw-r--r--   0 linatawfik   (501) staff       (20)     1286 2023-05-03 20:18:13.000000 horizonai-0.1.5/setup.py
+drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-03 20:41:19.383935 horizonai-0.1.6/
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1070 2023-05-03 16:55:57.000000 horizonai-0.1.6/LICENSE
+-rw-r--r--   0 linatawfik   (501) staff       (20)     2313 2023-05-03 20:41:19.384004 horizonai-0.1.6/PKG-INFO
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1575 2023-05-03 16:55:57.000000 horizonai-0.1.6/README.md
+drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-03 20:41:19.383070 horizonai-0.1.6/horizonai/
+-rw-r--r--   0 linatawfik   (501) staff       (20)       83 2023-05-03 20:15:40.000000 horizonai-0.1.6/horizonai/__init__.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1542 2023-05-03 20:09:16.000000 horizonai-0.1.6/horizonai/base.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)    14474 2023-05-03 18:31:03.000000 horizonai-0.1.6/horizonai/cli.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1231 2023-05-03 20:35:32.000000 horizonai-0.1.6/horizonai/project.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)     3374 2023-05-03 20:39:34.000000 horizonai-0.1.6/horizonai/task.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)      354 2023-05-03 20:36:00.000000 horizonai-0.1.6/horizonai/user.py
+drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-03 20:41:19.383833 horizonai-0.1.6/horizonai.egg-info/
+-rw-r--r--   0 linatawfik   (501) staff       (20)     2313 2023-05-03 20:41:19.000000 horizonai-0.1.6/horizonai.egg-info/PKG-INFO
+-rw-r--r--   0 linatawfik   (501) staff       (20)      350 2023-05-03 20:41:19.000000 horizonai-0.1.6/horizonai.egg-info/SOURCES.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)        1 2023-05-03 20:41:19.000000 horizonai-0.1.6/horizonai.egg-info/dependency_links.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)       48 2023-05-03 20:41:19.000000 horizonai-0.1.6/horizonai.egg-info/entry_points.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)       15 2023-05-03 20:41:19.000000 horizonai-0.1.6/horizonai.egg-info/requires.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)       10 2023-05-03 20:41:19.000000 horizonai-0.1.6/horizonai.egg-info/top_level.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)       79 2023-05-03 20:41:19.384212 horizonai-0.1.6/setup.cfg
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1288 2023-05-03 20:40:38.000000 horizonai-0.1.6/setup.py
```

### Comparing `horizonai-0.1.5/LICENSE` & `horizonai-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `horizonai-0.1.5/PKG-INFO` & `horizonai-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: horizonai
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python package and command line interface to access the Horizon AI API
 Home-page: https://www.gethorizon.ai
-Download-URL: https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.5-alpha.tar.gz
+Download-URL: https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.6-alpha.tar.gz
 Author: Horizon Team
 Author-email: team@gethorizon.ai
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `horizonai-0.1.5/README.md` & `horizonai-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `horizonai-0.1.5/horizonai/base.py` & `horizonai-0.1.6/horizonai/base.py`

 * *Files identical despite different names*

### Comparing `horizonai-0.1.5/horizonai/cli.py` & `horizonai-0.1.6/horizonai/cli.py`

 * *Files identical despite different names*

### Comparing `horizonai-0.1.5/horizonai/project.py` & `horizonai-0.1.6/horizonai/project.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 """Defines methods for Project objects."""
-
-from . import base
+from base import api_key, _get, _post, _delete
 
 
 def list_projects():
     global api_key
     if api_key == None:
         raise Exception("Must set Horizon API key.")
     headers = {"X-Api-Key": api_key}
-    response = base._get(endpoint="/api/projects", headers=headers)
+    response = _get(endpoint="/api/projects", headers=headers)
     return response
 
 
 def create_project(name):
     global api_key
     if api_key == None:
         raise Exception("Must set Horizon API key.")
     headers = {"Content-Type": "application/json", "X-Api-Key": api_key}
     data = {"name": name}
-    response = base._post(
+    response = _post(
         endpoint="/api/projects/create",
         json=data,
         headers=headers,
     )
     return response
 
 
 def get_project(project_id):
     global api_key
     if api_key == None:
         raise Exception("Must set Horizon API key.")
     headers = {"X-Api-Key": api_key}
-    response = base._get(endpoint=f"/api/projects/{project_id}", headers=headers)
+    response = _get(
+        endpoint=f"/api/projects/{project_id}", headers=headers)
     return response
 
 
 def delete_project(project_id):
     global api_key
     if api_key == None:
         raise Exception("Must set Horizon API key.")
     headers = {"X-Api-Key": api_key}
-    response = base._delete(endpoint=f"/api/projects/{project_id}", headers=headers)
+    response = _delete(
+        endpoint=f"/api/projects/{project_id}", headers=headers)
     return response
```

### Comparing `horizonai-0.1.5/horizonai/task.py` & `horizonai-0.1.6/horizonai/task.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Defines methods for Task objects."""
 
-from . import base
+from base import api_key, _get, _post, _delete, anthropic_api_key, openai_api_key
 
 
 def list_tasks():
     global api_key
     if api_key == None:
         raise Exception("Must set Horizon API key.")
     headers = {"X-Api-Key": api_key}
-    response = base._get(endpoint="/api/tasks", headers=headers)
+    response = _get(endpoint="/api/tasks", headers=headers)
     return response
 
 
 def create_task(
     name: str,
     task_type: str,
     project_id: int,
@@ -26,42 +26,43 @@
     headers = {"Content-Type": "application/json", "X-Api-Key": api_key}
     payload = {
         "name": name,
         "task_type": task_type,
         "project_id": project_id,
         "allowed_models": allowed_models,
     }
-    response = base._post(endpoint="/api/tasks/create", json=payload, headers=headers)
+    response = _post(endpoint="/api/tasks/create",
+                     json=payload, headers=headers)
     return response
 
 
 def get_task(task_id):
     global api_key
     if api_key == None:
         raise Exception("Must set Horizon API key.")
     headers = {"X-Api-Key": api_key}
-    response = base._get(endpoint=f"/api/tasks/{task_id}", headers=headers)
+    response = _get(endpoint=f"/api/tasks/{task_id}", headers=headers)
     return response
 
 
 def delete_task(task_id):
     global api_key
     if api_key == None:
         raise Exception("Must set Horizon API key.")
     headers = {"X-Api-Key": api_key}
-    response = base._delete(endpoint=f"/api/tasks/{task_id}", headers=headers)
+    response = _delete(endpoint=f"/api/tasks/{task_id}", headers=headers)
     return response
 
 
 def get_task_confirmation_details(task_id):
     global api_key
     if api_key == None:
         raise Exception("Must set Horizon API key.")
     headers = {"X-Api-Key": api_key}
-    response = base._get(
+    response = _get(
         endpoint=f"/api/tasks/{task_id}/get_task_confirmation_details",
         headers=headers,
     )
     return response
 
 
 def generate_task(task_id, objective):
@@ -71,38 +72,40 @@
     headers = {"Content-Type": "application/json", "X-Api-Key": api_key}
     payload = {
         "task_id": task_id,
         "objective": objective,
         "openai_api_key": openai_api_key,
         "anthropic_api_key": anthropic_api_key,
     }
-    response = base._post(endpoint="/api/tasks/generate", json=payload, headers=headers)
+    response = _post(endpoint="/api/tasks/generate",
+                     json=payload, headers=headers)
     return response
 
 
 def deploy_task(task_id, inputs):
     global api_key, openai_api_key, anthropic_api_key
     if api_key == None:
         raise Exception("Must set Horizon API key.")
     headers = {"Content-Type": "application/json", "X-Api-Key": api_key}
     payload = {
         "task_id": task_id,
         "inputs": inputs,
         "openai_api_key": openai_api_key,
         "anthropic_api_key": anthropic_api_key,
     }
-    response = base._post(endpoint="/api/tasks/deploy", json=payload, headers=headers)
+    response = _post(endpoint="/api/tasks/deploy",
+                     json=payload, headers=headers)
     return response
 
 
 def upload_evaluation_dataset(task_id, file_path):
     global api_key
     if api_key == None:
         raise Exception("Must set Horizon API key.")
     headers = {"X-Api-Key": api_key}
     with open(file_path, "rb") as f:
-        response = base._post(
+        response = _post(
             endpoint=f"/api/tasks/{task_id}/upload_evaluation_dataset",
             files={"evaluation_dataset": f},
             headers=headers,
         )
         return response
```

### Comparing `horizonai-0.1.5/horizonai.egg-info/PKG-INFO` & `horizonai-0.1.6/horizonai.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: horizonai
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python package and command line interface to access the Horizon AI API
 Home-page: https://www.gethorizon.ai
-Download-URL: https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.5-alpha.tar.gz
+Download-URL: https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.6-alpha.tar.gz
 Author: Horizon Team
 Author-email: team@gethorizon.ai
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `horizonai-0.1.5/setup.py` & `horizonai-0.1.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 def read(file_name):
     with open(os.path.join(os.path.dirname(__file__), file_name), "r", encoding="utf-8") as f:
         return f.read()
 
 
 setup(
     name="horizonai",
-    version="0.1.5",
+    version="0.1.6",
     packages=find_packages(),
     package_data={"": ["__init__.py"]},
     install_requires=[
         "requests",
         "click",
     ],
-    entry_points={"console_scripts": ["horizon=horizonai.cli:cli"]},
+    entry_points={"console_scripts": ["horizonai=horizonai.cli:cli"]},
     author="Horizon Team",
     author_email="team@gethorizon.ai",
     license="MIT",
     description="Python package and command line interface to access the Horizon AI API",
     long_description=read("README.md"),  # Include README.md content
     long_description_content_type="text/markdown",  # Specify content type as Markdown
     url="https://www.gethorizon.ai",
-    download_url="https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.5-alpha.tar.gz",
+    download_url="https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.6-alpha.tar.gz",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

