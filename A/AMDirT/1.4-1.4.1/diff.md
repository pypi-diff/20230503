# Comparing `tmp/AMDirT-1.4.tar.gz` & `tmp/AMDirT-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AMDirT-1.4.tar", last modified: Fri Apr 28 14:37:52 2023, max compression
+gzip compressed data, was "AMDirT-1.4.1.tar", last modified: Wed May  3 12:46:49 2023, max compression
```

## Comparing `AMDirT-1.4.tar` & `AMDirT-1.4.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:37:52.661318 AMDirT-1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:37:52.657318 AMDirT-1.4/AMDirT/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-28 14:37:49.000000 AMDirT-1.4/AMDirT/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:37:52.657318 AMDirT-1.4/AMDirT/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:37:49.000000 AMDirT-1.4/AMDirT/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:37:52.657318 AMDirT-1.4/AMDirT/autofill/
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-04-28 14:37:49.000000 AMDirT-1.4/AMDirT/autofill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-28 14:37:49.000000 AMDirT-1.4/AMDirT/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:37:52.657318 AMDirT-1.4/AMDirT/convert/
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-28 14:37:49.000000 AMDirT-1.4/AMDirT/convert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:37:52.657318 AMDirT-1.4/AMDirT/core/
--rw-r--r--   0 runner    (1001) docker     (123)    15210 2023-04-28 14:37:49.000000 AMDirT-1.4/AMDirT/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-28 14:37:49.000000 AMDirT-1.4/AMDirT/core/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-04-28 14:37:49.000000 AMDirT-1.4/AMDirT/core/ena.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:37:52.657318 AMDirT-1.4/AMDirT/merge/
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-28 14:37:49.000000 AMDirT-1.4/AMDirT/merge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:37:52.657318 AMDirT-1.4/AMDirT/validate/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-28 14:37:49.000000 AMDirT-1.4/AMDirT/validate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:37:52.657318 AMDirT-1.4/AMDirT/validate/application/
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-04-28 14:37:49.000000 AMDirT-1.4/AMDirT/validate/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:37:52.657318 AMDirT-1.4/AMDirT/validate/domain/
--rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-04-28 14:37:49.000000 AMDirT-1.4/AMDirT/validate/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-28 14:37:49.000000 AMDirT-1.4/AMDirT/validate/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:37:52.657318 AMDirT-1.4/AMDirT/viewer/
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-28 14:37:49.000000 AMDirT-1.4/AMDirT/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-04-28 14:37:49.000000 AMDirT-1.4/AMDirT/viewer/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:37:52.657318 AMDirT-1.4/AMDirT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-28 14:37:52.000000 AMDirT-1.4/AMDirT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-28 14:37:52.000000 AMDirT-1.4/AMDirT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 14:37:52.000000 AMDirT-1.4/AMDirT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 14:37:52.000000 AMDirT-1.4/AMDirT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 14:37:52.000000 AMDirT-1.4/AMDirT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 14:37:52.000000 AMDirT-1.4/AMDirT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 14:37:49.000000 AMDirT-1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-28 14:37:52.657318 AMDirT-1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-28 14:37:49.000000 AMDirT-1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 14:37:52.661318 AMDirT-1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-28 14:37:49.000000 AMDirT-1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:49.638845 AMDirT-1.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:49.634845 AMDirT-1.4.1/AMDirT/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:49.634845 AMDirT-1.4.1/AMDirT/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:49.634845 AMDirT-1.4.1/AMDirT/autofill/
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/autofill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:49.634845 AMDirT-1.4.1/AMDirT/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/convert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:49.634845 AMDirT-1.4.1/AMDirT/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    15205 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/core/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/core/ena.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:49.634845 AMDirT-1.4.1/AMDirT/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/merge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:49.634845 AMDirT-1.4.1/AMDirT/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/validate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:49.634845 AMDirT-1.4.1/AMDirT/validate/application/
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/validate/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:49.634845 AMDirT-1.4.1/AMDirT/validate/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/validate/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/validate/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:49.634845 AMDirT-1.4.1/AMDirT/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-05-03 12:46:44.000000 AMDirT-1.4.1/AMDirT/viewer/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:46:49.634845 AMDirT-1.4.1/AMDirT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-03 12:46:49.000000 AMDirT-1.4.1/AMDirT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-03 12:46:49.000000 AMDirT-1.4.1/AMDirT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:46:49.000000 AMDirT-1.4.1/AMDirT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 12:46:49.000000 AMDirT-1.4.1/AMDirT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-03 12:46:49.000000 AMDirT-1.4.1/AMDirT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 12:46:49.000000 AMDirT-1.4.1/AMDirT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-03 12:46:44.000000 AMDirT-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-03 12:46:49.634845 AMDirT-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-03 12:46:44.000000 AMDirT-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 12:46:49.638845 AMDirT-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-03 12:46:44.000000 AMDirT-1.4.1/setup.py
```

### Comparing `AMDirT-1.4/AMDirT/autofill/__init__.py` & `AMDirT-1.4.1/AMDirT/autofill/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4/AMDirT/cli.py` & `AMDirT-1.4.1/AMDirT/cli.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4/AMDirT/convert/__init__.py` & `AMDirT-1.4.1/AMDirT/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4/AMDirT/core/__init__.py` & `AMDirT-1.4.1/AMDirT/core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 logger = colorlog.getLogger('AMDirT')
 logger.addHandler(handler)
 logger.propagate = False
 
 
 def get_json_path():
-    path = os.path.join(get_module_dir("AMDirT.assets"), "tables.json")
+    path = get_module_dir("AMDirT.assets").joinpath("tables.json")
     return path
 
 
 @st.cache_data
 def get_amdir_tags():
     r = requests.get(
         "https://api.github.com/repos/SPAAM-community/AncientMetagenomeDir/tags"
```

### Comparing `AMDirT-1.4/AMDirT/core/diff.py` & `AMDirT-1.4.1/AMDirT/core/diff.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4/AMDirT/core/ena.py` & `AMDirT-1.4.1/AMDirT/core/ena.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4/AMDirT/merge/__init__.py` & `AMDirT-1.4.1/AMDirT/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4/AMDirT/validate/__init__.py` & `AMDirT-1.4.1/AMDirT/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4/AMDirT/validate/application/__init__.py` & `AMDirT-1.4.1/AMDirT/validate/application/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4/AMDirT/validate/domain/__init__.py` & `AMDirT-1.4.1/AMDirT/validate/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4/AMDirT/validate/exceptions.py` & `AMDirT-1.4.1/AMDirT/validate/exceptions.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4/AMDirT/viewer/__init__.py` & `AMDirT-1.4.1/AMDirT/viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4/AMDirT/viewer/streamlit.py` & `AMDirT-1.4.1/AMDirT/viewer/streamlit.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,19 @@
     prepare_eager_table,
     prepare_mag_table,
     prepare_accession_table,
     prepare_aMeta_table,
     prepare_taxprofiler_table,
     is_merge_size_zero,
     get_amdir_tags,
-    get_libraries
+    get_libraries,
+    get_json_path
 )
 
 
-
 st.set_page_config(
     page_title="AMDirT viewer",
     page_icon="https://raw.githubusercontent.com/SPAAM-community/AncientMetagenomeDir/master/assets/images/logos/spaam-AncientMetagenomeDir_logo_mini.png",
     layout="wide",
 )
 
 supported_archives = ["ENA", "SRA"]
@@ -36,15 +36,19 @@
     st.session_state.force_validation = False
 if "table_name" not in st.session_state:
     st.session_state.table_name = None
 
 
 def parse_args():
     parser = argparse.ArgumentParser("Run Streamlit app")
-    parser.add_argument("-c", "--config", help="json config file", required=True)
+    parser.add_argument(
+        "-c", 
+        "--config", 
+        help="json config file", 
+        default=get_json_path())
     try:
         args = parser.parse_args()
     except SystemExit as e:
         os._exit(e.code)
     return args
```

### Comparing `AMDirT-1.4/AMDirT.egg-info/PKG-INFO` & `AMDirT-1.4.1/AMDirT.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AMDirT
-Version: 1.4
+Version: 1.4.1
 Summary: AMDirT: AncientMetagenomeDir Toolkit
 Home-page: https://github.com/SPAAM-community/AMDirT
 License: GNU-GPLv3
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -17,23 +17,25 @@
 
 AMDirT is a toolkit for interacting with the AncientMetagenomeDir metadata repository of ancient metagenomic samples and ancient microbial genomes. This tool provides ways to validate AncientMetagenomeDir submissions, explore and download sequencing data for ancient microbial and environmental (meta)genomes, and automatically prepare input samplesheets for a range of bioinformatic processing pipelines.
 
 For documentation on using the tool, please see [How Tos](how_to/index), [Tutorials](/tutorials) and/or [Quick Reference](/reference).
 
 ## Install
 
-Before we release AMDirt on (bio)Conda, please follow the instructions below.
-
 ### 1. With pip
 
-...upon release of v 1.4
+```bash
+pip install amdirt
+```
 
 ### 2. With conda
 
-...upon release of v 1.4
+```bash
+conda install -c bioconda amdirt
+```
 
 ### The latest development version, directly from GitHub
 
 ```bash
 pip install --upgrade --force-reinstall git+https://github.com/SPAAM-community/AMDirT.git@dev
 ```
 
@@ -41,15 +43,15 @@
 
 - Fork AMDirT on GitHub
 - Clone your fork `git clone [your-AMDirT-fork]`
 - Checkout the `dev` branch `git switch dev`
 - Create the conda environment `conda env create -f environment.yml`
 - Activate the environment `conda activate amdirt`
 - Install amdirt in development mode `pip install -e .`
-    - In some cases you may need to force update streamlit with `pip install --upgrade steamlit`
+  - In some cases you may need to force update streamlit with `pip install --upgrade steamlit`
 
 To locally render documentation:
 
 - `conda activate amdirt`
 - Install additional requirements `cd docs && pip install -r requirements.txt`
 - Build the HTML `make html`
 - Open the `build/html/README.html` file in your browser
```

### Comparing `AMDirT-1.4/AMDirT.egg-info/SOURCES.txt` & `AMDirT-1.4.1/AMDirT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4/LICENSE` & `AMDirT-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4/PKG-INFO` & `AMDirT-1.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AMDirT
-Version: 1.4
+Version: 1.4.1
 Summary: AMDirT: AncientMetagenomeDir Toolkit
 Home-page: https://github.com/SPAAM-community/AMDirT
 License: GNU-GPLv3
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -17,23 +17,25 @@
 
 AMDirT is a toolkit for interacting with the AncientMetagenomeDir metadata repository of ancient metagenomic samples and ancient microbial genomes. This tool provides ways to validate AncientMetagenomeDir submissions, explore and download sequencing data for ancient microbial and environmental (meta)genomes, and automatically prepare input samplesheets for a range of bioinformatic processing pipelines.
 
 For documentation on using the tool, please see [How Tos](how_to/index), [Tutorials](/tutorials) and/or [Quick Reference](/reference).
 
 ## Install
 
-Before we release AMDirt on (bio)Conda, please follow the instructions below.
-
 ### 1. With pip
 
-...upon release of v 1.4
+```bash
+pip install amdirt
+```
 
 ### 2. With conda
 
-...upon release of v 1.4
+```bash
+conda install -c bioconda amdirt
+```
 
 ### The latest development version, directly from GitHub
 
 ```bash
 pip install --upgrade --force-reinstall git+https://github.com/SPAAM-community/AMDirT.git@dev
 ```
 
@@ -41,15 +43,15 @@
 
 - Fork AMDirT on GitHub
 - Clone your fork `git clone [your-AMDirT-fork]`
 - Checkout the `dev` branch `git switch dev`
 - Create the conda environment `conda env create -f environment.yml`
 - Activate the environment `conda activate amdirt`
 - Install amdirt in development mode `pip install -e .`
-    - In some cases you may need to force update streamlit with `pip install --upgrade steamlit`
+  - In some cases you may need to force update streamlit with `pip install --upgrade steamlit`
 
 To locally render documentation:
 
 - `conda activate amdirt`
 - Install additional requirements `cd docs && pip install -r requirements.txt`
 - Build the HTML `make html`
 - Open the `build/html/README.html` file in your browser
```

### Comparing `AMDirT-1.4/README.md` & `AMDirT-1.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 
 AMDirT is a toolkit for interacting with the AncientMetagenomeDir metadata repository of ancient metagenomic samples and ancient microbial genomes. This tool provides ways to validate AncientMetagenomeDir submissions, explore and download sequencing data for ancient microbial and environmental (meta)genomes, and automatically prepare input samplesheets for a range of bioinformatic processing pipelines.
 
 For documentation on using the tool, please see [How Tos](how_to/index), [Tutorials](/tutorials) and/or [Quick Reference](/reference).
 
 ## Install
 
-Before we release AMDirt on (bio)Conda, please follow the instructions below.
-
 ### 1. With pip
 
-...upon release of v 1.4
+```bash
+pip install amdirt
+```
 
 ### 2. With conda
 
-...upon release of v 1.4
+```bash
+conda install -c bioconda amdirt
+```
 
 ### The latest development version, directly from GitHub
 
 ```bash
 pip install --upgrade --force-reinstall git+https://github.com/SPAAM-community/AMDirT.git@dev
 ```
 
@@ -30,15 +32,15 @@
 
 - Fork AMDirT on GitHub
 - Clone your fork `git clone [your-AMDirT-fork]`
 - Checkout the `dev` branch `git switch dev`
 - Create the conda environment `conda env create -f environment.yml`
 - Activate the environment `conda activate amdirt`
 - Install amdirt in development mode `pip install -e .`
-    - In some cases you may need to force update streamlit with `pip install --upgrade steamlit`
+  - In some cases you may need to force update streamlit with `pip install --upgrade steamlit`
 
 To locally render documentation:
 
 - `conda activate amdirt`
 - Install additional requirements `cd docs && pip install -r requirements.txt`
 - Build the HTML `make html`
 - Open the `build/html/README.html` file in your browser
```

### Comparing `AMDirT-1.4/setup.py` & `AMDirT-1.4.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,10 +37,11 @@
         "streamlit-aggrid",
         "numpy",
         "requests",
         "colorlog"
     ],
     packages=find_packages(exclude="test"),
     entry_points={"console_scripts": ["AMDirT = AMDirT.cli:cli"]},
+    package_dir={"AMDirT": "AMDirT"},
     include_package_data=True,
-    package_data={"": ["assets/tables.json"]},
+    package_data={"AMDirT.assets": ["tables.json"]},
 )
```

