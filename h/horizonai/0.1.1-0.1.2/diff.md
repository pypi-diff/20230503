# Comparing `tmp/horizonai-0.1.1.tar.gz` & `tmp/horizonai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horizonai-0.1.1.tar", last modified: Wed May  3 18:21:41 2023, max compression
+gzip compressed data, was "horizonai-0.1.2.tar", last modified: Wed May  3 19:25:05 2023, max compression
```

## Comparing `horizonai-0.1.1.tar` & `horizonai-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-03 18:21:41.357352 horizonai-0.1.1/
--rw-r--r--   0 linatawfik   (501) staff       (20)     1070 2023-05-03 16:55:57.000000 horizonai-0.1.1/LICENSE
--rw-r--r--   0 linatawfik   (501) staff       (20)     2313 2023-05-03 18:21:41.357432 horizonai-0.1.1/PKG-INFO
--rw-r--r--   0 linatawfik   (501) staff       (20)     1575 2023-05-03 16:55:57.000000 horizonai-0.1.1/README.md
-drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-03 18:21:41.356530 horizonai-0.1.1/horizonai/
--rw-r--r--   0 linatawfik   (501) staff       (20)       63 2023-05-03 16:55:57.000000 horizonai-0.1.1/horizonai/__init__.py
--rw-r--r--   0 linatawfik   (501) staff       (20)     1515 2023-05-03 16:55:57.000000 horizonai-0.1.1/horizonai/base.py
--rw-r--r--   0 linatawfik   (501) staff       (20)    14372 2023-05-03 16:55:57.000000 horizonai-0.1.1/horizonai/cli.py
--rw-r--r--   0 linatawfik   (501) staff       (20)     1206 2023-05-03 16:55:57.000000 horizonai-0.1.1/horizonai/project.py
--rw-r--r--   0 linatawfik   (501) staff       (20)     3288 2023-05-03 16:55:57.000000 horizonai-0.1.1/horizonai/task.py
--rw-r--r--   0 linatawfik   (501) staff       (20)      355 2023-05-03 16:55:57.000000 horizonai-0.1.1/horizonai/user.py
-drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-03 18:21:41.357214 horizonai-0.1.1/horizonai.egg-info/
--rw-r--r--   0 linatawfik   (501) staff       (20)     2313 2023-05-03 18:21:41.000000 horizonai-0.1.1/horizonai.egg-info/PKG-INFO
--rw-r--r--   0 linatawfik   (501) staff       (20)      350 2023-05-03 18:21:41.000000 horizonai-0.1.1/horizonai.egg-info/SOURCES.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)        1 2023-05-03 18:21:41.000000 horizonai-0.1.1/horizonai.egg-info/dependency_links.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)       46 2023-05-03 18:21:41.000000 horizonai-0.1.1/horizonai.egg-info/entry_points.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)       15 2023-05-03 18:21:41.000000 horizonai-0.1.1/horizonai.egg-info/requires.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)       10 2023-05-03 18:21:41.000000 horizonai-0.1.1/horizonai.egg-info/top_level.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)       79 2023-05-03 18:21:41.357861 horizonai-0.1.1/setup.cfg
--rw-r--r--   0 linatawfik   (501) staff       (20)     1286 2023-05-03 18:21:15.000000 horizonai-0.1.1/setup.py
+drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-03 19:25:05.690964 horizonai-0.1.2/
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1070 2023-05-03 16:55:57.000000 horizonai-0.1.2/LICENSE
+-rw-r--r--   0 linatawfik   (501) staff       (20)     2313 2023-05-03 19:25:05.691047 horizonai-0.1.2/PKG-INFO
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1575 2023-05-03 16:55:57.000000 horizonai-0.1.2/README.md
+drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-03 19:25:05.689978 horizonai-0.1.2/horizonai/
+-rw-r--r--   0 linatawfik   (501) staff       (20)       63 2023-05-03 16:55:57.000000 horizonai-0.1.2/horizonai/__init__.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1542 2023-05-03 19:21:12.000000 horizonai-0.1.2/horizonai/base.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)    14474 2023-05-03 18:31:03.000000 horizonai-0.1.2/horizonai/cli.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1206 2023-05-03 16:55:57.000000 horizonai-0.1.2/horizonai/project.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)     3288 2023-05-03 16:55:57.000000 horizonai-0.1.2/horizonai/task.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)      355 2023-05-03 16:55:57.000000 horizonai-0.1.2/horizonai/user.py
+drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-03 19:25:05.690858 horizonai-0.1.2/horizonai.egg-info/
+-rw-r--r--   0 linatawfik   (501) staff       (20)     2313 2023-05-03 19:25:05.000000 horizonai-0.1.2/horizonai.egg-info/PKG-INFO
+-rw-r--r--   0 linatawfik   (501) staff       (20)      350 2023-05-03 19:25:05.000000 horizonai-0.1.2/horizonai.egg-info/SOURCES.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)        1 2023-05-03 19:25:05.000000 horizonai-0.1.2/horizonai.egg-info/dependency_links.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)       46 2023-05-03 19:25:05.000000 horizonai-0.1.2/horizonai.egg-info/entry_points.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)       15 2023-05-03 19:25:05.000000 horizonai-0.1.2/horizonai.egg-info/requires.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)       10 2023-05-03 19:25:05.000000 horizonai-0.1.2/horizonai.egg-info/top_level.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)       79 2023-05-03 19:25:05.691345 horizonai-0.1.2/setup.cfg
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1286 2023-05-03 19:24:44.000000 horizonai-0.1.2/setup.py
```

### Comparing `horizonai-0.1.1/LICENSE` & `horizonai-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `horizonai-0.1.1/PKG-INFO` & `horizonai-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: horizonai
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package and command line interface to access the Horizon AI API
 Home-page: https://www.gethorizon.ai
-Download-URL: https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.1-alpha.tar.gz
+Download-URL: https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.2-alpha.tar.gz
 Author: Horizon Team
 Author-email: team@gethorizon.ai
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `horizonai-0.1.1/README.md` & `horizonai-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `horizonai-0.1.1/horizonai/base.py` & `horizonai-0.1.2/horizonai/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Defines utility methods for API package."""
 
 import requests
 from urllib.parse import urljoin
 
 # Base url for API calls
-base_url = "https://35.164.129.93:5000"
+base_url = "http://35.164.129.93:5000"
 
 # API keys for user to set
 api_key = None
 openai_api_key = None
 anthropic_api_key = None
 
 
@@ -33,15 +33,16 @@
     global base_url
     response = requests.delete(urljoin(base_url, endpoint), headers=headers)
     return _handle_response(response)
 
 
 def _put(endpoint, json=None, headers=None):
     global base_url
-    response = requests.put(urljoin(base_url, endpoint), json=json, headers=headers)
+    response = requests.put(urljoin(base_url, endpoint),
+                            json=json, headers=headers)
     return _handle_response(response)
 
 
 def _get_auth_headers():
     global api_key
     if api_key == None:
         raise Exception("Must set Horizon API key.")
```

### Comparing `horizonai-0.1.1/horizonai/cli.py` & `horizonai-0.1.2/horizonai/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,14 @@
 
 @click.group()
 def prompt():
     pass
 
 
 # User-related methods
-
-
 # Generate new Horizon API key for user
 @click.command(name="api-key")
 @click.option("--email", prompt="Email", help="The email for the user.")
 @click.password_option(
     "--password", prompt="Password", help="The password for the user."
 )
 def generate_new_api_key(email, password):
@@ -55,22 +53,21 @@
         formatted_output = json.dumps(result, indent=4)
         click.echo(formatted_output)
     except Exception as e:
         click.echo(str(e))
 
 
 # Project-related methods
-
-
 # List projects
 @click.command(name="list")
 @click.option(
     "--horizon_api_key",
     default=os.environ.get("HORIZON_API_KEY"),
-    prompt="Horizon API Key" if not os.environ.get("HORIZON_API_KEY") else False,
+    prompt="Horizon API Key" if not os.environ.get(
+        "HORIZON_API_KEY") else False,
     help="The Horizon API key for the user.",
     hide_input=True,
 )
 def list_projects(horizon_api_key):
     horizonai.api_key = horizon_api_key
     try:
         result = horizonai.list_projects()
@@ -81,15 +78,16 @@
 
 
 # Create project
 @click.command(name="create")
 @click.option(
     "--horizon_api_key",
     default=os.environ.get("HORIZON_API_KEY"),
-    prompt="Horizon API Key" if not os.environ.get("HORIZON_API_KEY") else False,
+    prompt="Horizon API Key" if not os.environ.get(
+        "HORIZON_API_KEY") else False,
     help="The Horizon API key for the user.",
     hide_input=True,
 )
 @click.option(
     "--name", prompt="Project name", help="The name of the project to create."
 )
 def create_project(name, horizon_api_key):
@@ -103,15 +101,16 @@
 
 
 # Get Project
 @click.command(name="get")
 @click.option(
     "--horizon_api_key",
     default=os.environ.get("HORIZON_API_KEY"),
-    prompt="Horizon API Key" if not os.environ.get("HORIZON_API_KEY") else False,
+    prompt="Horizon API Key" if not os.environ.get(
+        "HORIZON_API_KEY") else False,
     help="The Horizon API key for the user.",
     hide_input=True,
 )
 @click.option(
     "--project_id", prompt="Project ID", help="The ID of the project to retrieve."
 )
 def get_project(project_id, horizon_api_key):
@@ -125,15 +124,16 @@
 
 
 # Update Project
 @click.command(name="update")
 @click.option(
     "--horizon_api_key",
     default=os.environ.get("HORIZON_API_KEY"),
-    prompt="Horizon API Key" if not os.environ.get("HORIZON_API_KEY") else False,
+    prompt="Horizon API Key" if not os.environ.get(
+        "HORIZON_API_KEY") else False,
     help="The Horizon API key for the user.",
     hide_input=True,
 )
 @click.option(
     "--project_id", prompt="Project ID", help="The ID of the project to update."
 )
 @click.option("--description", help="The new description for the project.")
@@ -149,15 +149,16 @@
 
 
 # Delete Project
 @click.command(name="delete")
 @click.option(
     "--horizon_api_key",
     default=os.environ.get("HORIZON_API_KEY"),
-    prompt="Horizon API Key" if not os.environ.get("HORIZON_API_KEY") else False,
+    prompt="Horizon API Key" if not os.environ.get(
+        "HORIZON_API_KEY") else False,
     help="The Horizon API key for the user.",
     hide_input=True,
 )
 @click.option(
     "--project_id", prompt="Project ID", help="The ID of the project to delete."
 )
 def delete_project(project_id, horizon_api_key):
@@ -167,22 +168,21 @@
         formatted_output = json.dumps(result, indent=4)
         click.echo(formatted_output)
     except Exception as e:
         click.echo(str(e))
 
 
 # Task-related methods
-
-
 # List Tasks
 @click.command(name="list")
 @click.option(
     "--horizon_api_key",
     default=os.environ.get("HORIZON_API_KEY"),
-    prompt="Horizon API Key" if not os.environ.get("HORIZON_API_KEY") else False,
+    prompt="Horizon API Key" if not os.environ.get(
+        "HORIZON_API_KEY") else False,
     help="The Horizon API key for the user.",
     hide_input=True,
 )
 def list_tasks(horizon_api_key):
     horizonai.api_key = horizon_api_key
     try:
         result = horizonai.list_tasks()
@@ -193,15 +193,16 @@
 
 
 # Create Task record and generate prompt for it
 @click.command(name="generate")
 @click.option(
     "--horizon_api_key",
     default=os.environ.get("HORIZON_API_KEY"),
-    prompt="Horizon API Key" if not os.environ.get("HORIZON_API_KEY") else False,
+    prompt="Horizon API Key" if not os.environ.get(
+        "HORIZON_API_KEY") else False,
     help="The Horizon API key for the user.",
     hide_input=True,
 )
 @click.option("--name", prompt="Task name", help="The name of the task to create.")
 @click.option(
     "--project_id",
     prompt="Associated project ID",
@@ -256,15 +257,16 @@
         if os.environ.get("ANTHROPIC_API_KEY"):
             horizonai.anthropic_api_key = os.environ.get("ANTHROPIC_API_KEY")
         else:
             horizonai.anthropic_api_key = click.prompt(
                 text="Anthropic API Key (text hidden)", hide_input=True
             )
 
-    click.echo(f"Evaluating the following models for task generation: {allowed_models}")
+    click.echo(
+        f"Evaluating the following models for task generation: {allowed_models}")
 
     # Create task record
     try:
         task_creation_response = horizonai.create_task(
             name, task_type, project_id, allowed_models
         )
         task_id = task_creation_response["task"]["id"]
@@ -303,15 +305,16 @@
     click.echo("=====")
     click.echo(
         "Please confirm the following parameters for your task creation request:"
     )
     click.echo("")
     click.echo(f"1) Task objective: {objective}")
     click.echo("")
-    click.echo(f"2) Input variables: {task_confirmation_details['input_variables']}")
+    click.echo(
+        f"2) Input variables: {task_confirmation_details['input_variables']}")
     click.echo(
         "* Inferred based on the headers of all but the right-most column in your evaluation dataset."
     )
     click.echo("")
     click.echo(
         f"3) Estimated LLM provider cost: ${task_confirmation_details['cost_estimate']['total_cost']['low']}-{task_confirmation_details['cost_estimate']['total_cost']['high']}"
     )
@@ -345,15 +348,16 @@
 
 
 # Get Task
 @click.command(name="get")
 @click.option(
     "--horizon_api_key",
     default=os.environ.get("HORIZON_API_KEY"),
-    prompt="Horizon API Key" if not os.environ.get("HORIZON_API_KEY") else False,
+    prompt="Horizon API Key" if not os.environ.get(
+        "HORIZON_API_KEY") else False,
     help="The Horizon API key for the user.",
     hide_input=True,
 )
 @click.option("--task_id", prompt="Task ID", help="The ID of the task to retrieve.")
 def get_task(task_id, horizon_api_key):
     horizonai.api_key = horizon_api_key
     try:
@@ -365,15 +369,16 @@
 
 
 # Delete Task
 @click.command(name="delete")
 @click.option(
     "--horizon_api_key",
     default=os.environ.get("HORIZON_API_KEY"),
-    prompt="Horizon API Key" if not os.environ.get("HORIZON_API_KEY") else False,
+    prompt="Horizon API Key" if not os.environ.get(
+        "HORIZON_API_KEY") else False,
     help="The Horizon API key for the user.",
     hide_input=True,
 )
 @click.option("--task_id", prompt="Task ID", help="The ID of the task to delete.")
 def delete_task(task_id, horizon_api_key):
     horizonai.api_key = horizon_api_key
     try:
@@ -387,15 +392,16 @@
 
 
 # Deploy a task
 @click.command(name="deploy")
 @click.option(
     "--horizon_api_key",
     default=os.environ.get("HORIZON_API_KEY"),
-    prompt="Horizon API Key" if not os.environ.get("HORIZON_API_KEY") else False,
+    prompt="Horizon API Key" if not os.environ.get(
+        "HORIZON_API_KEY") else False,
     help="The Horizon API key for the user.",
     hide_input=True,
 )
 @click.option("--task_id", prompt="Task ID", help="The ID of the task to deploy.")
 @click.option(
     "--inputs", prompt="Inputs", help="The inputs to the task in JSON format."
 )
```

### Comparing `horizonai-0.1.1/horizonai/project.py` & `horizonai-0.1.2/horizonai/project.py`

 * *Files identical despite different names*

### Comparing `horizonai-0.1.1/horizonai/task.py` & `horizonai-0.1.2/horizonai/task.py`

 * *Files identical despite different names*

### Comparing `horizonai-0.1.1/horizonai.egg-info/PKG-INFO` & `horizonai-0.1.2/horizonai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: horizonai
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package and command line interface to access the Horizon AI API
 Home-page: https://www.gethorizon.ai
-Download-URL: https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.1-alpha.tar.gz
+Download-URL: https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.2-alpha.tar.gz
 Author: Horizon Team
 Author-email: team@gethorizon.ai
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `horizonai-0.1.1/setup.py` & `horizonai-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 def read(file_name):
     with open(os.path.join(os.path.dirname(__file__), file_name), "r", encoding="utf-8") as f:
         return f.read()
 
 
 setup(
     name="horizonai",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     package_data={"": ["__init__.py"]},
     install_requires=[
         "requests",
         "click",
     ],
     entry_points={"console_scripts": ["horizon=horizonai.cli:cli"]},
     author="Horizon Team",
     author_email="team@gethorizon.ai",
     license="MIT",
     description="Python package and command line interface to access the Horizon AI API",
     long_description=read("README.md"),  # Include README.md content
     long_description_content_type="text/markdown",  # Specify content type as Markdown
     url="https://www.gethorizon.ai",
-    download_url="https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.1-alpha.tar.gz",
+    download_url="https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.2-alpha.tar.gz",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

