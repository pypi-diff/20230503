# Comparing `tmp/twb_project-0.9.0.tar.gz` & `tmp/twb_project-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twb_project-0.9.0.tar", max compression
+gzip compressed data, was "twb_project-0.9.1.tar", max compression
```

## Comparing `twb_project-0.9.0.tar` & `twb_project-0.9.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-0.9.0/LICENSE
--rw-r--r--   0        0        0     1547 2023-02-27 01:45:34.838817 twb_project-0.9.0/README.md
--rw-r--r--   0        0        0      760 2023-05-03 04:36:49.662491 twb_project-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      218 2023-05-02 04:53:16.027176 twb_project-0.9.0/twb/__init__.py
--rw-r--r--   0        0        0      788 2023-02-26 15:18:15.849792 twb_project-0.9.0/twb/bip.py
--rw-r--r--   0        0        0    18740 2023-05-03 04:39:07.821059 twb_project-0.9.0/twb/builder.py
--rw-r--r--   0        0        0      227 2023-05-03 04:36:18.661146 twb_project-0.9.0/twb/builder_helpers.py
--rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-0.9.0/twb/decompressor.py
--rw-r--r--   0        0        0     9493 2023-03-26 18:01:42.380403 twb_project-0.9.0/twb/downloader.py
--rw-r--r--   0        0        0     3794 2023-04-20 07:59:01.227219 twb_project-0.9.0/twb/logger.py
--rw-r--r--   0        0        0     1594 2023-05-02 23:19:18.752642 twb_project-0.9.0/twb/logger_init.py
--rw-r--r--   0        0        0    10603 2023-05-02 23:19:18.752689 twb_project-0.9.0/twb/modifier.py
--rw-r--r--   0        0        0     9161 2023-04-20 02:54:12.926181 twb_project-0.9.0/twb/parallelization.py
--rw-r--r--   0        0        0     5527 2023-05-02 04:49:02.953589 twb_project-0.9.0/twb/reader.py
--rw-r--r--   0        0        0     6203 2023-04-20 00:32:02.529127 twb_project-0.9.0/twb/utils.py
--rw-r--r--   0        0        0     5284 2023-05-03 04:25:54.008631 twb_project-0.9.0/twb/warehouse.py
--rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 twb_project-0.9.0/setup.py
--rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 twb_project-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-0.9.1/LICENSE
+-rw-r--r--   0        0        0     1547 2023-02-27 01:45:34.838817 twb_project-0.9.1/README.md
+-rw-r--r--   0        0        0      760 2023-05-03 08:01:25.664328 twb_project-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      218 2023-05-02 04:53:16.027176 twb_project-0.9.1/twb/__init__.py
+-rw-r--r--   0        0        0      788 2023-02-26 15:18:15.849792 twb_project-0.9.1/twb/bip.py
+-rw-r--r--   0        0        0    18828 2023-05-03 07:53:55.757688 twb_project-0.9.1/twb/builder.py
+-rw-r--r--   0        0        0      227 2023-05-03 04:36:18.661146 twb_project-0.9.1/twb/builder_helpers.py
+-rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-0.9.1/twb/decompressor.py
+-rw-r--r--   0        0        0     9493 2023-03-26 18:01:42.380403 twb_project-0.9.1/twb/downloader.py
+-rw-r--r--   0        0        0     3794 2023-04-20 07:59:01.227219 twb_project-0.9.1/twb/logger.py
+-rw-r--r--   0        0        0     1594 2023-05-02 23:19:18.752642 twb_project-0.9.1/twb/logger_init.py
+-rw-r--r--   0        0        0    10603 2023-05-02 23:19:18.752689 twb_project-0.9.1/twb/modifier.py
+-rw-r--r--   0        0        0     9161 2023-04-20 02:54:12.926181 twb_project-0.9.1/twb/parallelization.py
+-rw-r--r--   0        0        0     5527 2023-05-02 04:49:02.953589 twb_project-0.9.1/twb/reader.py
+-rw-r--r--   0        0        0     6203 2023-04-20 00:32:02.529127 twb_project-0.9.1/twb/utils.py
+-rw-r--r--   0        0        0     5284 2023-05-03 04:25:54.008631 twb_project-0.9.1/twb/warehouse.py
+-rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 twb_project-0.9.1/setup.py
+-rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 twb_project-0.9.1/PKG-INFO
```

### Comparing `twb_project-0.9.0/LICENSE` & `twb_project-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.0/README.md` & `twb_project-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.0/pyproject.toml` & `twb_project-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twb-project"
-version = "0.9.0"
+version = "0.9.1"
 description = "An unified tool for the research in extracting information from Wikipedia Edit History chunk."
 authors = ["Lingxi Li <hi@lingxi.li>"]
 license = "GNU GPL"
 readme = "README.md"
 packages = [
     { include = "twb" },
 ]
```

### Comparing `twb_project-0.9.0/twb/bip.py` & `twb_project-0.9.1/twb/bip.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.0/twb/builder.py` & `twb_project-0.9.1/twb/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,19 +198,23 @@
                     item_depth=3,
                     item_callback=_inner_callback,
                 )
 
             # Finalize the last article.
             _finalizing_metadata()
 
-            return processed_files
-
         except Exception as e:
             logging.critical(f'Error occurred when processing the file [{xml_file}]: {e}')
-            return []
+            processed_files = []
+
+        finally:
+            # Remove XML file.
+            os.remove(xml_path)
+
+        return processed_files
 
     def _warehouse_executor(self, assigned_warehouse: str, combo_files_list: List[Tuple[str, str]]):
         try:
             warehouse_filename, warehouse_metadata_filename = get_warehouse_filenames(assigned_warehouse)
             warehouse_path = os.path.join(self.output_dir, warehouse_filename)
             warehouse_metadata_path = os.path.join(self.output_dir, warehouse_metadata_filename)
```

### Comparing `twb_project-0.9.0/twb/decompressor.py` & `twb_project-0.9.1/twb/decompressor.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.0/twb/downloader.py` & `twb_project-0.9.1/twb/downloader.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.0/twb/logger.py` & `twb_project-0.9.1/twb/logger.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.0/twb/logger_init.py` & `twb_project-0.9.1/twb/logger_init.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.0/twb/modifier.py` & `twb_project-0.9.1/twb/modifier.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.0/twb/parallelization.py` & `twb_project-0.9.1/twb/parallelization.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.0/twb/reader.py` & `twb_project-0.9.1/twb/reader.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.0/twb/utils.py` & `twb_project-0.9.1/twb/utils.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.0/twb/warehouse.py` & `twb_project-0.9.1/twb/warehouse.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.0/setup.py` & `twb_project-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'py7zr>=0.20.5,<0.21.0',
  'requests>=2.28.2,<3.0.0',
  'xmltodict>=0.13.0,<0.14.0',
  'zstandard>=0.21.0,<0.22.0']
 
 setup_kwargs = {
     'name': 'twb-project',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'An unified tool for the research in extracting information from Wikipedia Edit History chunk.',
     'long_description': '<img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/49178640-2f6d-4c23-e56f-a48eca531200/HD" alt="TWB" />\n\n# Temporal Wikipedia Blocks (TWB)\n\nTemporal Wikipedia Blocks (TWB) is a powerful Python package designed to process the extensive edit history of Wikipedia pages into easily manageable and memory-friendly blocks. The package is specifically developed to enable efficient parallelization and composition of these blocks to facilitate faster processing and analysis of large Wikipedia datasets. The original design of this package is to build other Wikipedia-oriented datasets on top of it.\n\nThe package works by dividing the Wikipedia edit history into temporal blocks, which are essentially subsets of the complete dataset that are based on time intervals. These blocks can then be easily processed and analyzed without the need to load the entire dataset into memory.\n\n## Installation\n\nThe package is available on PyPI and can be installed using pip:\n\n```bash\npip install twb-project\n```\n\n## Benefits\n\n- **Efficient**: The package is designed to be memory-friendly and can be easily parallelized to process large datasets.\n- **Fast**: The package is designed to be fast and can be easily optimized to process large datasets.\n- **Flexible**: The package is designed to be flexible and can be easily extended to support other types of blocks.\n- **Composable**: The package is designed to be composable and can be easily combined with other packages to build other datasets.\n\n## Specification\n\n- Default compression method: ZStandard.\n',
     'author': 'Lingxi Li',
     'author_email': 'hi@lingxi.li',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://twb.lingxi.li/',
```

### Comparing `twb_project-0.9.0/PKG-INFO` & `twb_project-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twb-project
-Version: 0.9.0
+Version: 0.9.1
 Summary: An unified tool for the research in extracting information from Wikipedia Edit History chunk.
 Home-page: https://twb.lingxi.li/
 License: GNU GPL
 Author: Lingxi Li
 Author-email: hi@lingxi.li
 Requires-Python: >=3.8,<4
 Classifier: License :: Other/Proprietary License
```

