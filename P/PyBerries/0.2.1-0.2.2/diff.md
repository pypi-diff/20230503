# Comparing `tmp/PyBerries-0.2.1.tar.gz` & `tmp/PyBerries-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyBerries-0.2.1.tar", last modified: Wed May  3 10:52:25 2023, max compression
+gzip compressed data, was "PyBerries-0.2.2.tar", last modified: Wed May  3 11:08:58 2023, max compression
```

## Comparing `PyBerries-0.2.1.tar` & `PyBerries-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 10:52:25.351198 PyBerries-0.2.1/
--rw-rw-rw-   0        0        0    33074 2022-12-22 10:37:47.000000 PyBerries-0.2.1/LICENSE
--rw-rw-rw-   0        0        0    14455 2023-05-03 10:52:25.351198 PyBerries-0.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 10:52:25.335196 PyBerries-0.2.1/PyBerries.egg-info/
--rw-rw-rw-   0        0        0    14455 2023-05-03 10:52:25.000000 PyBerries-0.2.1/PyBerries.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1062 2023-05-03 10:52:25.000000 PyBerries-0.2.1/PyBerries.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 10:52:25.000000 PyBerries-0.2.1/PyBerries.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-03 10:52:25.000000 PyBerries-0.2.1/PyBerries.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-03 10:52:25.000000 PyBerries-0.2.1/PyBerries.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    14137 2023-05-02 10:54:16.000000 PyBerries-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 10:52:25.335196 PyBerries-0.2.1/pyberries/
-drwxrwxrwx   0        0        0        0 2023-05-03 10:52:25.335196 PyBerries-0.2.1/pyberries/File_utilities/
--rw-rw-rw-   0        0        0     2877 2023-03-14 14:43:41.000000 PyBerries-0.2.1/pyberries/File_utilities/Filename_utils.py
--rw-rw-rw-   0        0        0     2782 2023-03-14 14:14:07.000000 PyBerries-0.2.1/pyberries/File_utilities/Stack_tiffs.py
--rw-rw-rw-   0        0        0      795 2023-03-14 14:14:07.000000 PyBerries-0.2.1/pyberries/File_utilities/Unpack_omero_folders.py
--rw-rw-rw-   0        0        0      119 2023-03-14 14:14:07.000000 PyBerries-0.2.1/pyberries/File_utilities/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:52:25.339196 PyBerries-0.2.1/pyberries/Metrics/
--rw-rw-rw-   0        0        0     1242 2023-05-02 10:54:16.000000 PyBerries-0.2.1/pyberries/Metrics/Metrics.py
--rw-rw-rw-   0        0        0     6475 2023-05-02 10:54:16.000000 PyBerries-0.2.1/pyberries/Metrics/Time_metrics.py
--rw-rw-rw-   0        0        0       69 2023-03-10 16:15:28.000000 PyBerries-0.2.1/pyberries/Metrics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:52:25.347198 PyBerries-0.2.1/pyberries/Plots/
--rw-rw-rw-   0        0        0     1037 2023-05-02 16:02:09.000000 PyBerries-0.2.1/pyberries/Plots/Fits.py
--rw-rw-rw-   0        0        0     4132 2023-05-02 15:52:54.000000 PyBerries-0.2.1/pyberries/Plots/Plot_presets.py
--rw-rw-rw-   0        0        0      353 2023-04-05 10:31:09.000000 PyBerries-0.2.1/pyberries/Plots/Plot_utilities.py
--rw-rw-rw-   0        0        0     1372 2023-04-03 13:51:01.000000 PyBerries-0.2.1/pyberries/Plots/Plots.py
--rw-rw-rw-   0        0        0      117 2023-05-02 10:54:16.000000 PyBerries-0.2.1/pyberries/Plots/__init__.py
--rw-rw-rw-   0        0        0      118 2023-05-02 10:54:16.000000 PyBerries-0.2.1/pyberries/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:52:25.343196 PyBerries-0.2.1/pyberries/data/
--rw-rw-rw-   0        0        0    15487 2023-05-02 15:31:41.000000 PyBerries-0.2.1/pyberries/data/DatasetPool.py
--rw-rw-rw-   0        0        0     1922 2023-05-02 15:22:46.000000 PyBerries-0.2.1/pyberries/data/Fitting.py
--rw-rw-rw-   0        0        0       86 2023-05-02 15:00:14.000000 PyBerries-0.2.1/pyberries/data/__init__.py
--rw-rw-rw-   0        0        0     1567 2023-05-02 15:50:42.000000 PyBerries-0.2.1/pyberries/data/util.py
--rw-rw-rw-   0        0        0       42 2023-05-03 10:52:25.351198 PyBerries-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      614 2023-05-03 10:46:19.000000 PyBerries-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:08:58.428418 PyBerries-0.2.2/
+-rw-rw-rw-   0        0        0    33074 2022-12-22 10:37:47.000000 PyBerries-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0    14455 2023-05-03 11:08:58.427415 PyBerries-0.2.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 11:08:58.397766 PyBerries-0.2.2/PyBerries.egg-info/
+-rw-rw-rw-   0        0        0    14455 2023-05-03 11:08:58.000000 PyBerries-0.2.2/PyBerries.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1062 2023-05-03 11:08:58.000000 PyBerries-0.2.2/PyBerries.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 11:08:58.000000 PyBerries-0.2.2/PyBerries.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-05-03 11:08:58.000000 PyBerries-0.2.2/PyBerries.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-03 11:08:58.000000 PyBerries-0.2.2/PyBerries.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    14137 2023-05-02 10:54:16.000000 PyBerries-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 11:08:58.398766 PyBerries-0.2.2/pyberries/
+drwxrwxrwx   0        0        0        0 2023-05-03 11:08:58.405766 PyBerries-0.2.2/pyberries/File_utilities/
+-rw-rw-rw-   0        0        0     2877 2023-03-14 14:43:41.000000 PyBerries-0.2.2/pyberries/File_utilities/Filename_utils.py
+-rw-rw-rw-   0        0        0     2782 2023-03-14 14:14:07.000000 PyBerries-0.2.2/pyberries/File_utilities/Stack_tiffs.py
+-rw-rw-rw-   0        0        0      795 2023-03-14 14:14:07.000000 PyBerries-0.2.2/pyberries/File_utilities/Unpack_omero_folders.py
+-rw-rw-rw-   0        0        0      119 2023-03-14 14:14:07.000000 PyBerries-0.2.2/pyberries/File_utilities/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:08:58.409764 PyBerries-0.2.2/pyberries/Metrics/
+-rw-rw-rw-   0        0        0     1242 2023-05-02 10:54:16.000000 PyBerries-0.2.2/pyberries/Metrics/Metrics.py
+-rw-rw-rw-   0        0        0     6475 2023-05-02 10:54:16.000000 PyBerries-0.2.2/pyberries/Metrics/Time_metrics.py
+-rw-rw-rw-   0        0        0       69 2023-03-10 16:15:28.000000 PyBerries-0.2.2/pyberries/Metrics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:08:58.425390 PyBerries-0.2.2/pyberries/Plots/
+-rw-rw-rw-   0        0        0     1037 2023-05-02 16:02:09.000000 PyBerries-0.2.2/pyberries/Plots/Fits.py
+-rw-rw-rw-   0        0        0     4132 2023-05-02 15:52:54.000000 PyBerries-0.2.2/pyberries/Plots/Plot_presets.py
+-rw-rw-rw-   0        0        0      353 2023-04-05 10:31:09.000000 PyBerries-0.2.2/pyberries/Plots/Plot_utilities.py
+-rw-rw-rw-   0        0        0     1372 2023-04-03 13:51:01.000000 PyBerries-0.2.2/pyberries/Plots/Plots.py
+-rw-rw-rw-   0        0        0      117 2023-05-02 10:54:16.000000 PyBerries-0.2.2/pyberries/Plots/__init__.py
+-rw-rw-rw-   0        0        0      118 2023-05-02 10:54:16.000000 PyBerries-0.2.2/pyberries/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:08:58.418765 PyBerries-0.2.2/pyberries/data/
+-rw-rw-rw-   0        0        0    15559 2023-05-03 11:07:36.000000 PyBerries-0.2.2/pyberries/data/DatasetPool.py
+-rw-rw-rw-   0        0        0     1922 2023-05-02 15:22:46.000000 PyBerries-0.2.2/pyberries/data/Fitting.py
+-rw-rw-rw-   0        0        0       86 2023-05-02 15:00:14.000000 PyBerries-0.2.2/pyberries/data/__init__.py
+-rw-rw-rw-   0        0        0     1567 2023-05-02 15:50:42.000000 PyBerries-0.2.2/pyberries/data/util.py
+-rw-rw-rw-   0        0        0       42 2023-05-03 11:08:58.428418 PyBerries-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      625 2023-05-03 11:06:25.000000 PyBerries-0.2.2/setup.py
```

### Comparing `PyBerries-0.2.1/LICENSE` & `PyBerries-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.1/PKG-INFO` & `PyBerries-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBerries
-Version: 0.2.1
+Version: 0.2.2
 Summary: Processing of Bacmman measurement tables
 Home-page: https://gitlab.com/MEKlab/pyberries
 Author: Daniel Thedie
 Author-email: daniel.thedie@ed.ac.uk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `PyBerries-0.2.1/PyBerries.egg-info/PKG-INFO` & `PyBerries-0.2.2/PyBerries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBerries
-Version: 0.2.1
+Version: 0.2.2
 Summary: Processing of Bacmman measurement tables
 Home-page: https://gitlab.com/MEKlab/pyberries
 Author: Daniel Thedie
 Author-email: daniel.thedie@ed.ac.uk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `PyBerries-0.2.1/PyBerries.egg-info/SOURCES.txt` & `PyBerries-0.2.2/PyBerries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.1/README.md` & `PyBerries-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.1/pyberries/File_utilities/Filename_utils.py` & `PyBerries-0.2.2/pyberries/File_utilities/Filename_utils.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.1/pyberries/File_utilities/Stack_tiffs.py` & `PyBerries-0.2.2/pyberries/File_utilities/Stack_tiffs.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.1/pyberries/File_utilities/Unpack_omero_folders.py` & `PyBerries-0.2.2/pyberries/File_utilities/Unpack_omero_folders.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.1/pyberries/Metrics/Metrics.py` & `PyBerries-0.2.2/pyberries/Metrics/Metrics.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.1/pyberries/Metrics/Time_metrics.py` & `PyBerries-0.2.2/pyberries/Metrics/Time_metrics.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.1/pyberries/Plots/Fits.py` & `PyBerries-0.2.2/pyberries/Plots/Fits.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.1/pyberries/Plots/Plot_presets.py` & `PyBerries-0.2.2/pyberries/Plots/Plot_presets.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.1/pyberries/Plots/Plots.py` & `PyBerries-0.2.2/pyberries/Plots/Plots.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.1/pyberries/data/DatasetPool.py` & `PyBerries-0.2.2/pyberries/data/DatasetPool.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,16 @@
                  dsList,
                  groups=[],
                  metadata={},
                  filters={},
                  preprocessing={}
                  ):
         
+        path = arg_to_list(path)
+        dsList = arg_to_list(dsList)
         self.path = path
         self.dsList = dsList
         self.table = dict()
         self.parent = dict()
         self.channel = dict()
         preprocessing = dict_val_to_list(preprocessing)
```

### Comparing `PyBerries-0.2.1/pyberries/data/Fitting.py` & `PyBerries-0.2.2/pyberries/data/Fitting.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.1/pyberries/data/util.py` & `PyBerries-0.2.2/pyberries/data/util.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.1/setup.py` & `PyBerries-0.2.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyBerries",
-    version="0.2.1",
+    version="0.2.2",
     author="Daniel Thedie",
     author_email="daniel.thedie@ed.ac.uk",
     description="Processing of Bacmman measurement tables",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/MEKlab/pyberries",
     packages=setuptools.find_packages(),
     python_requires='>=3.8',
-    install_requires=['numpy', 'scipy', 'pandas', 'matplotlib', 'tifffile', 'h5py','seaborn', 'pybacmman']
+    install_requires=['numpy', 'scipy', 'pandas', 'matplotlib', 'tifffile', 'h5py','seaborn', 'pybacmman', 'IPython']
 )
```

