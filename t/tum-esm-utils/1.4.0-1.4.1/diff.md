# Comparing `tmp/tum_esm_utils-1.4.0.tar.gz` & `tmp/tum_esm_utils-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tum_esm_utils-1.4.0.tar", max compression
+gzip compressed data, was "tum_esm_utils-1.4.1.tar", max compression
```

## Comparing `tum_esm_utils-1.4.0.tar` & `tum_esm_utils-1.4.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    34523 2023-03-19 02:25:01.728953 tum_esm_utils-1.4.0/LICENSE
--rw-r--r--   0        0        0      311 2023-03-19 01:58:42.297575 tum_esm_utils-1.4.0/README.md
--rw-r--r--   0        0        0     1288 2023-04-17 17:10:34.521783 tum_esm_utils-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      324 2023-03-24 22:12:39.730536 tum_esm_utils-1.4.0/tum_esm_utils/__init__.py
--rw-r--r--   0        0        0     3177 2023-04-15 14:16:07.544110 tum_esm_utils-1.4.0/tum_esm_utils/datastructures.py
--rw-r--r--   0        0        0     1094 2023-03-19 00:09:51.433019 tum_esm_utils-1.4.0/tum_esm_utils/decorators.py
--rw-r--r--   0        0        0     1052 2023-04-17 17:40:27.776962 tum_esm_utils-1.4.0/tum_esm_utils/files.py
--rw-r--r--   0        0        0      571 2023-03-18 12:27:22.283048 tum_esm_utils-1.4.0/tum_esm_utils/github.py
--rw-r--r--   0        0        0       44 2023-03-24 22:36:46.147084 tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/.gitignore
--rw-r--r--   0        0        0     2462 2023-03-24 21:29:53.767147 tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/glob_OPUSparms.F90
--rw-r--r--   0        0        0     2459 2023-03-24 21:29:53.777058 tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/glob_prepro4.F90
--rw-r--r--   0        0        0    28408 2023-03-24 21:29:53.783183 tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/ifg_parser.F90
--rw-r--r--   0        0        0      758 2023-03-24 21:29:53.790831 tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/ifg_parser.template.inp
--rw-r--r--   0        0        0   983040 2023-03-24 21:29:53.798327 tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/refspec.dat
--rw-r--r--   0        0        0   983040 2023-03-24 21:29:53.802664 tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/refspec2.dat
--rw-r--r--   0        0        0     3902 2023-03-24 22:39:47.173064 tum_esm_utils-1.4.0/tum_esm_utils/interferograms.py
--rw-r--r--   0        0        0     7829 2023-03-19 00:26:19.544914 tum_esm_utils-1.4.0/tum_esm_utils/logger.py
--rw-r--r--   0        0        0      309 2023-03-19 00:38:17.496564 tum_esm_utils-1.4.0/tum_esm_utils/mathematics.py
--rw-r--r--   0        0        0     1553 2023-03-18 13:50:38.104259 tum_esm_utils-1.4.0/tum_esm_utils/processes.py
--rw-r--r--   0        0        0        0 2023-03-18 12:27:05.965015 tum_esm_utils-1.4.0/tum_esm_utils/py.typed
--rw-r--r--   0        0        0     2856 2023-04-17 17:10:20.854083 tum_esm_utils-1.4.0/tum_esm_utils/shell.py
--rw-r--r--   0        0        0     1289 2023-03-18 14:22:32.105297 tum_esm_utils-1.4.0/tum_esm_utils/system.py
--rw-r--r--   0        0        0      851 2023-03-18 14:37:55.541792 tum_esm_utils-1.4.0/tum_esm_utils/testing.py
--rw-r--r--   0        0        0     3129 2023-04-17 17:44:42.149505 tum_esm_utils-1.4.0/tum_esm_utils/text.py
--rw-r--r--   0        0        0     6777 2023-04-17 17:41:44.557063 tum_esm_utils-1.4.0/tum_esm_utils/validators.py
--rw-r--r--   0        0        0     3607 1970-01-01 00:00:00.000000 tum_esm_utils-1.4.0/setup.py
--rw-r--r--   0        0        0     1299 1970-01-01 00:00:00.000000 tum_esm_utils-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-03-19 02:25:01.728953 tum_esm_utils-1.4.1/LICENSE
+-rw-r--r--   0        0        0      311 2023-03-19 01:58:42.297575 tum_esm_utils-1.4.1/README.md
+-rw-r--r--   0        0        0     1288 2023-04-25 03:35:00.743049 tum_esm_utils-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0      324 2023-03-24 22:12:39.730536 tum_esm_utils-1.4.1/tum_esm_utils/__init__.py
+-rw-r--r--   0        0        0     3177 2023-04-15 14:16:07.544110 tum_esm_utils-1.4.1/tum_esm_utils/datastructures.py
+-rw-r--r--   0        0        0     1094 2023-03-19 00:09:51.433019 tum_esm_utils-1.4.1/tum_esm_utils/decorators.py
+-rw-r--r--   0        0        0     1052 2023-04-17 17:40:27.776962 tum_esm_utils-1.4.1/tum_esm_utils/files.py
+-rw-r--r--   0        0        0      571 2023-03-18 12:27:22.283048 tum_esm_utils-1.4.1/tum_esm_utils/github.py
+-rw-r--r--   0        0        0       64 2023-04-25 03:34:37.353328 tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/.gitignore
+-rw-r--r--   0        0        0     2462 2023-03-24 21:29:53.767147 tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/glob_OPUSparms.F90
+-rw-r--r--   0        0        0     2459 2023-03-24 21:29:53.777058 tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/glob_prepro4.F90
+-rw-r--r--   0        0        0    28408 2023-04-25 03:08:42.468142 tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/ifg_parser.F90
+-rw-r--r--   0        0        0      758 2023-04-25 02:57:45.344815 tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/ifg_parser.template.inp
+-rw-r--r--   0        0        0   983040 2023-03-24 21:29:53.798327 tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/refspec.dat
+-rw-r--r--   0        0        0   983040 2023-03-24 21:29:53.802664 tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/refspec2.dat
+-rw-r--r--   0        0        0     4437 2023-04-25 03:34:11.213272 tum_esm_utils-1.4.1/tum_esm_utils/interferograms.py
+-rw-r--r--   0        0        0     7829 2023-03-19 00:26:19.544914 tum_esm_utils-1.4.1/tum_esm_utils/logger.py
+-rw-r--r--   0        0        0      309 2023-03-19 00:38:17.496564 tum_esm_utils-1.4.1/tum_esm_utils/mathematics.py
+-rw-r--r--   0        0        0     1553 2023-03-18 13:50:38.104259 tum_esm_utils-1.4.1/tum_esm_utils/processes.py
+-rw-r--r--   0        0        0        0 2023-03-18 12:27:05.965015 tum_esm_utils-1.4.1/tum_esm_utils/py.typed
+-rw-r--r--   0        0        0     2856 2023-04-17 17:10:20.854083 tum_esm_utils-1.4.1/tum_esm_utils/shell.py
+-rw-r--r--   0        0        0     1289 2023-03-18 14:22:32.105297 tum_esm_utils-1.4.1/tum_esm_utils/system.py
+-rw-r--r--   0        0        0      851 2023-03-18 14:37:55.541792 tum_esm_utils-1.4.1/tum_esm_utils/testing.py
+-rw-r--r--   0        0        0     3129 2023-04-17 17:44:42.149505 tum_esm_utils-1.4.1/tum_esm_utils/text.py
+-rw-r--r--   0        0        0     6777 2023-04-17 17:41:44.557063 tum_esm_utils-1.4.1/tum_esm_utils/validators.py
+-rw-r--r--   0        0        0     3607 1970-01-01 00:00:00.000000 tum_esm_utils-1.4.1/setup.py
+-rw-r--r--   0        0        0     1299 1970-01-01 00:00:00.000000 tum_esm_utils-1.4.1/PKG-INFO
```

### Comparing `tum_esm_utils-1.4.0/LICENSE` & `tum_esm_utils-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.0/pyproject.toml` & `tum_esm_utils-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tum_esm_utils"
-version = "1.4.0"
+version = "1.4.1"
 description = "Python utilities by the Professorship of Environmental Sensing and Modeling at the Technical University of Munich"
 authors = ["Moritz Makowski <moritz.makowski@tum.de>"]
 readme = "README.md"
 packages = [
     {include = "tum_esm_utils"},
     {include = "tum_esm_utils/py.typed"}
 ]
```

### Comparing `tum_esm_utils-1.4.0/tum_esm_utils/datastructures.py` & `tum_esm_utils-1.4.1/tum_esm_utils/datastructures.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.0/tum_esm_utils/decorators.py` & `tum_esm_utils-1.4.1/tum_esm_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.0/tum_esm_utils/files.py` & `tum_esm_utils-1.4.1/tum_esm_utils/files.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.0/tum_esm_utils/github.py` & `tum_esm_utils-1.4.1/tum_esm_utils/github.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/glob_OPUSparms.F90` & `tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/glob_OPUSparms.F90`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/glob_prepro4.F90` & `tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/glob_prepro4.F90`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/ifg_parser.F90` & `tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/ifg_parser.F90`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 use glob_prepro4
 
 implicit none
 
 logical :: dateidadec
 integer :: imeas,itest,iunit,iscan,narg,next_free_unit
-character(len=200) :: inputdatei,logdatei,logdatei_test
+character(len=300) :: inputdatei,logdatei,logdatei_test
 character(len=10) :: idchar
 character(len=7) :: imeaschar
 character(len=4) :: argchar
 
 character(len=lengthcharmeas),dimension(:),allocatable :: measfile
 logical,dimension(:),allocatable :: dualifg
 integer,dimension(:),allocatable :: nptrfirstdir,nofblock,nifg &
```

### Comparing `tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/ifg_parser.template.inp` & `tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/ifg_parser.template.inp`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/refspec.dat` & `tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/refspec.dat`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.0/tum_esm_utils/ifg_parser/refspec2.dat` & `tum_esm_utils-1.4.1/tum_esm_utils/ifg_parser/refspec2.dat`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.0/tum_esm_utils/interferograms.py` & `tum_esm_utils-1.4.1/tum_esm_utils/interferograms.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import re
 import subprocess
 from typing import Literal
 
+from filelock import FileLock
+import tum_esm_utils
 
 _PARSER_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), "ifg_parser")
 
 
 def _compile_fortran_code(
     silent: bool = True,
     fortran_compiler: Literal["gfortran", "gfortran-9"] = "gfortran",
@@ -29,18 +31,18 @@
             stderr = p.stderr.decode("utf-8", errors="replace").strip()
             raise Exception(
                 f"command '{command}' failed with exit code {p.returncode}, "
                 + f"stderr: {stderr}, stout:{stdout}",
             )
 
 
-def _write_input_file(ifgs: list[str]) -> None:
+def _write_input_file(random_id: str, ifgs: list[str]) -> None:
     with open(f"{_PARSER_DIR}/ifg_parser.template.inp", "r") as f:
         template_content = f.read()
-    with open(f"{_PARSER_DIR}/ifg_parser.inp", "w") as f:
+    with open(f"{_PARSER_DIR}/ifg_parser.inp.{random_id}", "w") as f:
         f.write(template_content.replace("%IFG_LIST%", "\n".join(ifgs)))
 
 
 def detect_corrupt_ifgs(
     ifg_directory: str,
     silent: bool = True,
     fortran_compiler: Literal["gfortran", "gfortran-9"] = "gfortran",
@@ -55,21 +57,31 @@
     ifgs = [f"{ifg_directory}/{x}" for x in os.listdir(ifg_directory)]
     ifgs = list(sorted(list(filter(os.path.isfile, ifgs))))
 
     # run the parser
     results: dict[str, list[str]] = {}
     stdout: str = ""
     while True:
-        _write_input_file(ifgs)
+        with FileLock(f"{_PARSER_DIR}/ifg_parser.inp.lock"):
+            random_id = tum_esm_utils.text.get_random_string(
+                10,
+                forbidden=[
+                    f.replace("ifg_parser.inp.", "")
+                    for f in os.listdir(_PARSER_DIR)
+                    if f.startswith("ifg_parser.inp.")
+                ],
+            )
+            _write_input_file(random_id, ifgs)
         process = subprocess.run(
-            ["./ifg_parser", "ifg_parser.inp"],
+            ["./ifg_parser", f"ifg_parser.inp.{random_id}"],
             cwd=_PARSER_DIR,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
+        os.remove(f"{_PARSER_DIR}/ifg_parser.inp.{random_id}")
         stdout = process.stdout.decode()
         stderr = process.stderr.decode()
         if process.returncode == 0:
             break
         else:
             # find the filename that caused the error
             failing_filenames = list(filter(lambda f: f in ifgs, stderr.split("'")))
```

### Comparing `tum_esm_utils-1.4.0/tum_esm_utils/logger.py` & `tum_esm_utils-1.4.1/tum_esm_utils/logger.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.0/tum_esm_utils/processes.py` & `tum_esm_utils-1.4.1/tum_esm_utils/processes.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.0/tum_esm_utils/shell.py` & `tum_esm_utils-1.4.1/tum_esm_utils/shell.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.0/tum_esm_utils/system.py` & `tum_esm_utils-1.4.1/tum_esm_utils/system.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.0/tum_esm_utils/testing.py` & `tum_esm_utils-1.4.1/tum_esm_utils/testing.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.0/tum_esm_utils/text.py` & `tum_esm_utils-1.4.1/tum_esm_utils/text.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.0/tum_esm_utils/validators.py` & `tum_esm_utils-1.4.1/tum_esm_utils/validators.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-1.4.0/setup.py` & `tum_esm_utils-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 ['filelock>=3.10.0,<4.0.0',
  'pendulum>=2.1.2,<3.0.0',
  'psutil>=5.9.4,<6.0.0',
  'requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'tum-esm-utils',
-    'version': '1.4.0',
+    'version': '1.4.1',
     'description': 'Python utilities by the Professorship of Environmental Sensing and Modeling at the Technical University of Munich',
     'long_description': '# 🔬 &nbsp;TUM ESM Python Utilities\n\n**Install the Python library with:**\n\n```bash\npoetry add tum_esm_utils\n# or\npip install tum_esm_utils\n```\n\n<br/>\n\n## For Developers\n\n**Publish the Package to PyPI:**\n\n```bash\npoetry build\npoetry publish\n```\n\n**Serve documentation page:**\n\n```bash\ndocsify serve ./docs\n```\n',
     'author': 'Moritz Makowski',
     'author_email': 'moritz.makowski@tum.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tum-esm/utils',
```

### Comparing `tum_esm_utils-1.4.0/PKG-INFO` & `tum_esm_utils-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tum-esm-utils
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python utilities by the Professorship of Environmental Sensing and Modeling at the Technical University of Munich
 Home-page: https://github.com/tum-esm/utils
 License: AGPL-3.0-only
 Keywords: python,library,utilities,lazydocs,docsify
 Author: Moritz Makowski
 Author-email: moritz.makowski@tum.de
 Requires-Python: >=3.9,<4.0
```

