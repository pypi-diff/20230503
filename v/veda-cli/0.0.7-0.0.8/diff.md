# Comparing `tmp/veda_cli-0.0.7.tar.gz` & `tmp/veda_cli-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veda_cli-0.0.7.tar", max compression
+gzip compressed data, was "veda_cli-0.0.8.tar", max compression
```

## Comparing `veda_cli-0.0.7.tar` & `veda_cli-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       72 2023-03-12 06:19:04.046534 veda_cli-0.0.7/README.md
--rw-r--r--   0        0        0     1664 2023-05-01 10:24:05.161406 veda_cli-0.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-12 04:30:35.194796 veda_cli-0.0.7/veda_cli/__init__.py
--rw-r--r--   0        0        0      915 2023-05-01 02:28:32.474565 veda_cli-0.0.7/veda_cli/applications/__init__.py
--rw-r--r--   0        0        0     1148 2023-05-01 05:41:01.645101 veda_cli-0.0.7/veda_cli/applications/ecco/__init__.py
--rw-r--r--   0        0        0    13066 2023-05-01 10:04:03.508678 veda_cli-0.0.7/veda_cli/applications/ecco/ecco_app.py
--rw-r--r--   0        0        0        0 2023-03-12 05:07:59.351295 veda_cli-0.0.7/veda_cli/applications/wrf/__init__.py
--rw-r--r--   0        0        0     1996 2023-05-01 10:17:38.133257 veda_cli-0.0.7/veda_cli/datasets/__init__.py
--rw-r--r--   0        0        0     2070 2023-05-01 10:04:58.155027 veda_cli-0.0.7/veda_cli/executions/__init__.py
--rw-r--r--   0        0        0     1002 2023-05-01 10:06:18.881461 veda_cli-0.0.7/veda_cli/executions/ouput.py
--rw-r--r--   0        0        0     1204 2023-05-01 08:52:05.066412 veda_cli-0.0.7/veda_cli/main.py
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 veda_cli-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       72 2023-03-12 06:19:04.046534 veda_cli-0.0.8/README.md
+-rw-r--r--   0        0        0     1664 2023-05-03 07:40:44.049177 veda_cli-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-12 04:30:35.194796 veda_cli-0.0.8/veda_cli/__init__.py
+-rw-r--r--   0        0        0      915 2023-05-01 02:28:32.474565 veda_cli-0.0.8/veda_cli/applications/__init__.py
+-rw-r--r--   0        0        0     1148 2023-05-01 05:41:01.645101 veda_cli-0.0.8/veda_cli/applications/ecco/__init__.py
+-rw-r--r--   0        0        0    13066 2023-05-01 10:04:03.508678 veda_cli-0.0.8/veda_cli/applications/ecco/ecco_app.py
+-rw-r--r--   0        0        0        0 2023-03-12 05:07:59.351295 veda_cli-0.0.8/veda_cli/applications/wrf/__init__.py
+-rw-r--r--   0        0        0     2374 2023-05-03 07:36:40.389908 veda_cli-0.0.8/veda_cli/datasets/__init__.py
+-rw-r--r--   0        0        0     2070 2023-05-01 10:04:58.155027 veda_cli-0.0.8/veda_cli/executions/__init__.py
+-rw-r--r--   0        0        0     1002 2023-05-01 10:33:28.153528 veda_cli-0.0.8/veda_cli/executions/ouput.py
+-rw-r--r--   0        0        0     1204 2023-05-01 08:52:05.066412 veda_cli-0.0.8/veda_cli/main.py
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 veda_cli-0.0.8/PKG-INFO
```

### Comparing `veda_cli-0.0.7/pyproject.toml` & `veda_cli-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 [tool.poetry]
 name = "veda-cli"
-version = "0.0.7"
+version = "0.0.8"
 description = "Command Line Client NASA VEDA Analytics"
 authors = ["Dimuthu Wannipurage <dwannipu@iu.edu>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 veda = "veda_cli.main:app"
```

### Comparing `veda_cli-0.0.7/veda_cli/applications/__init__.py` & `veda_cli-0.0.8/veda_cli/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `veda_cli-0.0.7/veda_cli/applications/ecco/__init__.py` & `veda_cli-0.0.8/veda_cli/applications/ecco/__init__.py`

 * *Files identical despite different names*

### Comparing `veda_cli-0.0.7/veda_cli/applications/ecco/ecco_app.py` & `veda_cli-0.0.8/veda_cli/applications/ecco/ecco_app.py`

 * *Files identical despite different names*

### Comparing `veda_cli-0.0.7/veda_cli/datasets/__init__.py` & `veda_cli-0.0.8/veda_cli/datasets/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 
 app = typer.Typer()
 
 def get_db():
     return db.getDb(os.path.join(os.path.expanduser('~'), ".veda", "ds.json"))
 
+def get_exec_db():
+    return db.getDb(os.path.join(os.path.expanduser('~'), ".veda", "db.json"))
+
 @app.command("list")
 def list_datasets():
     console = Console()
     table = Table()
 
     table.add_column('Dataset Name', justify='left')
     table.add_column('Description', justify='left')
@@ -39,27 +42,36 @@
 def get_file_list(root_dir):
     files = [os.path.relpath(os.path.join(dirpath, file), root_dir) 
              for (dirpath, dirnames, filenames) in os.walk(root_dir) for file in filenames]
 
     return files
 
 @app.command("register")
-def register_dataset(dataset_name, dataset_path):
+def register_dataset(execution_id, dataset_name, dataset_path):
     print("Registring the dataset")
+
+    db_conn = get_exec_db()
+    executions = db_conn.getBy({"type":"Execution", "executionId": execution_id})
+    execution = executions[0]
+    storage_id = execution["storageId"]
+    output_dir = execution["outputDir"]
+
+    dataset_path = output_dir + "/" + dataset_path
+
     db_conn = get_db()
     db_conn.add({
         "type": "Dataset",
-        "storageId": "local-agent",
+        "storageId": storage_id,
         "name": dataset_name, 
         "base_path": dataset_path, 
         "createdTime": datetime.now().strftime("%m/%d/%Y, %H:%M:%S"),
         "files": get_file_list(dataset_path)})
     
-@app.command("publish")
-def publish_dataset(dataset_name, storage_id):
+@app.command("copy")
+def copy_dataset(dataset_name, storage_id):
     print("Publishing the Dataset to storage " + storage_id)
     db_conn = get_db()
     datasets = db_conn.getBy({"type":"Dataset", "storageId": "local-agent", "name": dataset_name})
     if len(datasets) > 0:
         ds = datasets[0]
         ops.copy(ds["storageId"] + "/" + ds["base_path"], storage_id + "/" + ds["name"] + "/")
         ds["storageId"] = storage_id
```

### Comparing `veda_cli-0.0.7/veda_cli/executions/__init__.py` & `veda_cli-0.0.8/veda_cli/executions/__init__.py`

 * *Files identical despite different names*

### Comparing `veda_cli-0.0.7/veda_cli/executions/ouput.py` & `veda_cli-0.0.8/veda_cli/executions/ouput.py`

 * *Files identical despite different names*

### Comparing `veda_cli-0.0.7/veda_cli/main.py` & `veda_cli-0.0.8/veda_cli/main.py`

 * *Files identical despite different names*

### Comparing `veda_cli-0.0.7/PKG-INFO` & `veda_cli-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veda-cli
-Version: 0.0.7
+Version: 0.0.8
 Summary: Command Line Client NASA VEDA Analytics
 Author: Dimuthu Wannipurage
 Author-email: dwannipu@iu.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

