# Comparing `tmp/tum_esm_utils-1.4.1.tar.gz` & `tmp/tum_esm_utils-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tum_esm_utils-1.4.1.tar", max compression
+gzip compressed data, was "tum_esm_utils-1.5.0.tar", max compression
```

## Comparing `tum_esm_utils-1.4.1.tar` & `tum_esm_utils-1.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    34523 2023-03-19 02:25:01.728953 tum_esm_utils-1.4.1/LICENSE
--rw-r--r--   0        0        0      311 2023-03-19 01:58:42.297575 tum_esm_utils-1.4.1/README.md
--rw-r--r--   0        0        0     1288 2023-04-25 03:35:00.743049 tum_esm_utils-1.4.1/pyproject.toml
--rw-r--r--   0        0        0      324 2023-03-24 22:12:39.730536 tum_esm_utils-1.4.1/tum_esm_utils/__init__.py
--rw-r--r--   0        0        0     3177 2023-04-15 14:16:07.544110 tum_esm_utils-1.4.1/tum_esm_utils/datastructures.py
--rw-r--r--   0        0        0     1094 2023-03-19 00:09:51.433019 tum_esm_utils-1.4.1/tum_esm_utils/decorators.py
--rw-r--r--   0        0        0     1052 2023-04-17 17:40:27.776962 tum_esm_utils-1.4.1/tum_esm_utils/files.py
--rw-r--r--   0        0        0      571 2023-03-18 12:27:22.283048 tum_esm_utils-1.4.1/tum_esm_utils/github.py
--rw-r--r--   0        0        0       64 2023-04-25 03:34:37.353328 tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/.gitignore
--rw-r--r--   0        0        0     2462 2023-03-24 21:29:53.767147 tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/glob_OPUSparms.F90
--rw-r--r--   0        0        0     2459 2023-03-24 21:29:53.777058 tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/glob_prepro4.F90
--rw-r--r--   0        0        0    28408 2023-04-25 03:08:42.468142 tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/ifg_parser.F90
--rw-r--r--   0        0        0      758 2023-04-25 02:57:45.344815 tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/ifg_parser.template.inp
--rw-r--r--   0        0        0   983040 2023-03-24 21:29:53.798327 tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/refspec.dat
--rw-r--r--   0        0        0   983040 2023-03-24 21:29:53.802664 tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/refspec2.dat
--rw-r--r--   0        0        0     4437 2023-04-25 03:34:11.213272 tum_esm_utils-1.4.1/tum_esm_utils/interferograms.py
--rw-r--r--   0        0        0     7829 2023-03-19 00:26:19.544914 tum_esm_utils-1.4.1/tum_esm_utils/logger.py
--rw-r--r--   0        0        0      309 2023-03-19 00:38:17.496564 tum_esm_utils-1.4.1/tum_esm_utils/mathematics.py
--rw-r--r--   0        0        0     1553 2023-03-18 13:50:38.104259 tum_esm_utils-1.4.1/tum_esm_utils/processes.py
--rw-r--r--   0        0        0        0 2023-03-18 12:27:05.965015 tum_esm_utils-1.4.1/tum_esm_utils/py.typed
--rw-r--r--   0        0        0     2856 2023-04-17 17:10:20.854083 tum_esm_utils-1.4.1/tum_esm_utils/shell.py
--rw-r--r--   0        0        0     1289 2023-03-18 14:22:32.105297 tum_esm_utils-1.4.1/tum_esm_utils/system.py
--rw-r--r--   0        0        0      851 2023-03-18 14:37:55.541792 tum_esm_utils-1.4.1/tum_esm_utils/testing.py
--rw-r--r--   0        0        0     3129 2023-04-17 17:44:42.149505 tum_esm_utils-1.4.1/tum_esm_utils/text.py
--rw-r--r--   0        0        0     6777 2023-04-17 17:41:44.557063 tum_esm_utils-1.4.1/tum_esm_utils/validators.py
--rw-r--r--   0        0        0     3607 1970-01-01 00:00:00.000000 tum_esm_utils-1.4.1/setup.py
--rw-r--r--   0        0        0     1299 1970-01-01 00:00:00.000000 tum_esm_utils-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-03-19 02:25:01.728953 tum_esm_utils-1.5.0/LICENSE
+-rw-r--r--   0        0        0      311 2023-03-19 01:58:42.297575 tum_esm_utils-1.5.0/README.md
+-rw-r--r--   0        0        0     1308 2023-05-03 12:39:52.495181 tum_esm_utils-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      324 2023-03-24 22:12:39.730536 tum_esm_utils-1.5.0/tum_esm_utils/__init__.py
+-rw-r--r--   0        0        0     3177 2023-04-15 14:16:07.544110 tum_esm_utils-1.5.0/tum_esm_utils/datastructures.py
+-rw-r--r--   0        0        0     1656 2023-05-03 12:05:20.117038 tum_esm_utils-1.5.0/tum_esm_utils/decorators.py
+-rw-r--r--   0        0        0     3672 2023-05-03 12:37:22.874116 tum_esm_utils-1.5.0/tum_esm_utils/files.py
+-rw-r--r--   0        0        0      571 2023-03-18 12:27:22.283048 tum_esm_utils-1.5.0/tum_esm_utils/github.py
+-rw-r--r--   0        0        0       64 2023-04-25 03:34:37.353328 tum_esm_utils-1.5.0/tum_esm_utils/ifg_parser/.gitignore
+-rw-r--r--   0        0        0     2462 2023-03-24 21:29:53.767147 tum_esm_utils-1.5.0/tum_esm_utils/ifg_parser/glob_OPUSparms.F90
+-rw-r--r--   0        0        0     2459 2023-03-24 21:29:53.777058 tum_esm_utils-1.5.0/tum_esm_utils/ifg_parser/glob_prepro4.F90
+-rw-r--r--   0        0        0    28408 2023-04-25 03:08:42.468142 tum_esm_utils-1.5.0/tum_esm_utils/ifg_parser/ifg_parser.F90
+-rw-r--r--   0        0        0      758 2023-04-25 02:57:45.344815 tum_esm_utils-1.5.0/tum_esm_utils/ifg_parser/ifg_parser.template.inp
+-rw-r--r--   0        0        0   983040 2023-03-24 21:29:53.798327 tum_esm_utils-1.5.0/tum_esm_utils/ifg_parser/refspec.dat
+-rw-r--r--   0        0        0   983040 2023-03-24 21:29:53.802664 tum_esm_utils-1.5.0/tum_esm_utils/ifg_parser/refspec2.dat
+-rw-r--r--   0        0        0     4437 2023-04-25 03:34:11.213272 tum_esm_utils-1.5.0/tum_esm_utils/interferograms.py
+-rw-r--r--   0        0        0     7829 2023-03-19 00:26:19.544914 tum_esm_utils-1.5.0/tum_esm_utils/logger.py
+-rw-r--r--   0        0        0      309 2023-03-19 00:38:17.496564 tum_esm_utils-1.5.0/tum_esm_utils/mathematics.py
+-rw-r--r--   0        0        0     1553 2023-03-18 13:50:38.104259 tum_esm_utils-1.5.0/tum_esm_utils/processes.py
+-rw-r--r--   0        0        0        0 2023-03-18 12:27:05.965015 tum_esm_utils-1.5.0/tum_esm_utils/py.typed
+-rw-r--r--   0        0        0     2856 2023-05-03 12:02:45.055012 tum_esm_utils-1.5.0/tum_esm_utils/shell.py
+-rw-r--r--   0        0        0     1289 2023-03-18 14:22:32.105297 tum_esm_utils-1.5.0/tum_esm_utils/system.py
+-rw-r--r--   0        0        0      851 2023-03-18 14:37:55.541792 tum_esm_utils-1.5.0/tum_esm_utils/testing.py
+-rw-r--r--   0        0        0     3129 2023-04-17 17:44:42.149505 tum_esm_utils-1.5.0/tum_esm_utils/text.py
+-rw-r--r--   0        0        0     6777 2023-04-17 17:41:44.557063 tum_esm_utils-1.5.0/tum_esm_utils/validators.py
+-rw-r--r--   0        0        0     3635 1970-01-01 00:00:00.000000 tum_esm_utils-1.5.0/setup.py
+-rw-r--r--   0        0        0     1341 1970-01-01 00:00:00.000000 tum_esm_utils-1.5.0/PKG-INFO
```

### Comparing `tum_esm_utils-1.4.1/LICENSE` & `tum_esm_utils-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.1/pyproject.toml` & `tum_esm_utils-1.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tum_esm_utils"
-version = "1.4.1"
+version = "1.5.0"
 description = "Python utilities by the Professorship of Environmental Sensing and Modeling at the Technical University of Munich"
 authors = ["Moritz Makowski <moritz.makowski@tum.de>"]
 readme = "README.md"
 packages = [
     {include = "tum_esm_utils"},
     {include = "tum_esm_utils/py.typed"}
 ]
@@ -21,14 +21,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 filelock = "^3.10.0"
 requests = "^2.28.2"
 psutil = "^5.9.4"
 pendulum = "^2.1.2"
+polars = "^0.17.11"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 pytest = "^7.2.2"
```

### Comparing `tum_esm_utils-1.4.1/tum_esm_utils/datastructures.py` & `tum_esm_utils-1.5.0/tum_esm_utils/datastructures.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.1/tum_esm_utils/github.py` & `tum_esm_utils-1.5.0/tum_esm_utils/github.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/glob_OPUSparms.F90` & `tum_esm_utils-1.5.0/tum_esm_utils/ifg_parser/glob_OPUSparms.F90`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/glob_prepro4.F90` & `tum_esm_utils-1.5.0/tum_esm_utils/ifg_parser/glob_prepro4.F90`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/ifg_parser.F90` & `tum_esm_utils-1.5.0/tum_esm_utils/ifg_parser/ifg_parser.F90`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/ifg_parser.template.inp` & `tum_esm_utils-1.5.0/tum_esm_utils/ifg_parser/ifg_parser.template.inp`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/refspec.dat` & `tum_esm_utils-1.5.0/tum_esm_utils/ifg_parser/refspec.dat`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/refspec2.dat` & `tum_esm_utils-1.5.0/tum_esm_utils/ifg_parser/refspec2.dat`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.1/tum_esm_utils/interferograms.py` & `tum_esm_utils-1.5.0/tum_esm_utils/interferograms.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.1/tum_esm_utils/logger.py` & `tum_esm_utils-1.5.0/tum_esm_utils/logger.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.1/tum_esm_utils/processes.py` & `tum_esm_utils-1.5.0/tum_esm_utils/processes.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.1/tum_esm_utils/shell.py` & `tum_esm_utils-1.5.0/tum_esm_utils/shell.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.1/tum_esm_utils/system.py` & `tum_esm_utils-1.5.0/tum_esm_utils/system.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.1/tum_esm_utils/testing.py` & `tum_esm_utils-1.5.0/tum_esm_utils/testing.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.1/tum_esm_utils/text.py` & `tum_esm_utils-1.5.0/tum_esm_utils/text.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.1/tum_esm_utils/validators.py` & `tum_esm_utils-1.5.0/tum_esm_utils/validators.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.1/setup.py` & `tum_esm_utils-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,20 +57,21 @@
                    'ifg_parser/refspec2.dat']}
 
 modules = \
 ['py']
 install_requires = \
 ['filelock>=3.10.0,<4.0.0',
  'pendulum>=2.1.2,<3.0.0',
+ 'polars>=0.17.11,<0.18.0',
  'psutil>=5.9.4,<6.0.0',
  'requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'tum-esm-utils',
-    'version': '1.4.1',
+    'version': '1.5.0',
     'description': 'Python utilities by the Professorship of Environmental Sensing and Modeling at the Technical University of Munich',
     'long_description': '# 🔬 &nbsp;TUM ESM Python Utilities\n\n**Install the Python library with:**\n\n```bash\npoetry add tum_esm_utils\n# or\npip install tum_esm_utils\n```\n\n<br/>\n\n## For Developers\n\n**Publish the Package to PyPI:**\n\n```bash\npoetry build\npoetry publish\n```\n\n**Serve documentation page:**\n\n```bash\ndocsify serve ./docs\n```\n',
     'author': 'Moritz Makowski',
     'author_email': 'moritz.makowski@tum.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tum-esm/utils',
```

### Comparing `tum_esm_utils-1.4.1/PKG-INFO` & `tum_esm_utils-1.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: tum-esm-utils
-Version: 1.4.1
+Version: 1.5.0
 Summary: Python utilities by the Professorship of Environmental Sensing and Modeling at the Technical University of Munich
 Home-page: https://github.com/tum-esm/utils
 License: AGPL-3.0-only
 Keywords: python,library,utilities,lazydocs,docsify
 Author: Moritz Makowski
 Author-email: moritz.makowski@tum.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: filelock (>=3.10.0,<4.0.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
+Requires-Dist: polars (>=0.17.11,<0.18.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Documentation, https://tum-esm.github.io/utils
 Project-URL: Repository, https://github.com/tum-esm/utils
 Description-Content-Type: text/markdown
 
 # 🔬 &nbsp;TUM ESM Python Utilities
```

