# Comparing `tmp/semisup-segmentation-0.0.5.tar.gz` & `tmp/semisup-segmentation-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/semisup-segmentation-0.0.5.tar", last modified: Wed May  3 11:25:17 2023, max compression
+gzip compressed data, was "dist/semisup-segmentation-0.0.6.tar", last modified: Wed May  3 11:29:06 2023, max compression
```

## Comparing `semisup-segmentation-0.0.5.tar` & `semisup-segmentation-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adines    (1000) adines    (1000)        0 2023-05-03 11:25:17.000000 semisup-segmentation-0.0.5/
--rw-rw-r--   0 adines    (1000) adines    (1000)      635 2023-05-03 11:25:17.000000 semisup-segmentation-0.0.5/PKG-INFO
--rw-rw-r--   0 adines    (1000) adines    (1000)     1071 2020-12-11 12:52:05.000000 semisup-segmentation-0.0.5/LICENSE.txt
--rw-rw-r--   0 adines    (1000) adines    (1000)     1197 2020-12-16 16:41:18.000000 semisup-segmentation-0.0.5/README.rst
-drwxrwxr-x   0 adines    (1000) adines    (1000)        0 2023-05-03 11:25:17.000000 semisup-segmentation-0.0.5/semisup_segmentation.egg-info/
--rw-rw-r--   0 adines    (1000) adines    (1000)      635 2023-05-03 11:25:16.000000 semisup-segmentation-0.0.5/semisup_segmentation.egg-info/PKG-INFO
--rw-rw-r--   0 adines    (1000) adines    (1000)      157 2023-05-03 11:25:16.000000 semisup-segmentation-0.0.5/semisup_segmentation.egg-info/requires.txt
--rw-rw-r--   0 adines    (1000) adines    (1000)        1 2023-05-03 11:25:16.000000 semisup-segmentation-0.0.5/semisup_segmentation.egg-info/dependency_links.txt
--rw-rw-r--   0 adines    (1000) adines    (1000)      344 2023-05-03 11:25:16.000000 semisup-segmentation-0.0.5/semisup_segmentation.egg-info/SOURCES.txt
--rw-rw-r--   0 adines    (1000) adines    (1000)       11 2023-05-03 11:25:16.000000 semisup-segmentation-0.0.5/semisup_segmentation.egg-info/top_level.txt
--rw-rw-r--   0 adines    (1000) adines    (1000)     8384 2023-05-03 11:25:10.000000 semisup-segmentation-0.0.5/setup.py
--rw-rw-r--   0 adines    (1000) adines    (1000)       46 2020-12-11 12:52:32.000000 semisup-segmentation-0.0.5/MANIFEST.in
--rw-rw-r--   0 adines    (1000) adines    (1000)       67 2023-05-03 11:25:17.000000 semisup-segmentation-0.0.5/setup.cfg
-drwxrwxr-x   0 adines    (1000) adines    (1000)        0 2023-05-03 11:25:17.000000 semisup-segmentation-0.0.5/SemiSegAPI/
--rw-rw-r--   0 adines    (1000) adines    (1000)     8342 2023-05-02 16:24:16.000000 semisup-segmentation-0.0.5/SemiSegAPI/semiSupervised.py
--rw-rw-r--   0 adines    (1000) adines    (1000)      249 2023-05-03 11:25:10.000000 semisup-segmentation-0.0.5/SemiSegAPI/__init__.py
--rw-rw-r--   0 adines    (1000) adines    (1000)    10397 2023-05-03 07:51:02.000000 semisup-segmentation-0.0.5/SemiSegAPI/utils.py
+drwxrwxr-x   0 adines    (1000) adines    (1000)        0 2023-05-03 11:29:06.000000 semisup-segmentation-0.0.6/
+-rw-rw-r--   0 adines    (1000) adines    (1000)      635 2023-05-03 11:29:06.000000 semisup-segmentation-0.0.6/PKG-INFO
+-rw-rw-r--   0 adines    (1000) adines    (1000)     1071 2020-12-11 12:52:05.000000 semisup-segmentation-0.0.6/LICENSE.txt
+-rw-rw-r--   0 adines    (1000) adines    (1000)     1197 2020-12-16 16:41:18.000000 semisup-segmentation-0.0.6/README.rst
+drwxrwxr-x   0 adines    (1000) adines    (1000)        0 2023-05-03 11:29:06.000000 semisup-segmentation-0.0.6/semisup_segmentation.egg-info/
+-rw-rw-r--   0 adines    (1000) adines    (1000)      635 2023-05-03 11:29:06.000000 semisup-segmentation-0.0.6/semisup_segmentation.egg-info/PKG-INFO
+-rw-rw-r--   0 adines    (1000) adines    (1000)      157 2023-05-03 11:29:06.000000 semisup-segmentation-0.0.6/semisup_segmentation.egg-info/requires.txt
+-rw-rw-r--   0 adines    (1000) adines    (1000)        1 2023-05-03 11:29:06.000000 semisup-segmentation-0.0.6/semisup_segmentation.egg-info/dependency_links.txt
+-rw-rw-r--   0 adines    (1000) adines    (1000)      344 2023-05-03 11:29:06.000000 semisup-segmentation-0.0.6/semisup_segmentation.egg-info/SOURCES.txt
+-rw-rw-r--   0 adines    (1000) adines    (1000)       11 2023-05-03 11:29:06.000000 semisup-segmentation-0.0.6/semisup_segmentation.egg-info/top_level.txt
+-rw-rw-r--   0 adines    (1000) adines    (1000)     8410 2023-05-03 11:29:01.000000 semisup-segmentation-0.0.6/setup.py
+-rw-rw-r--   0 adines    (1000) adines    (1000)       46 2020-12-11 12:52:32.000000 semisup-segmentation-0.0.6/MANIFEST.in
+-rw-rw-r--   0 adines    (1000) adines    (1000)       67 2023-05-03 11:29:06.000000 semisup-segmentation-0.0.6/setup.cfg
+drwxrwxr-x   0 adines    (1000) adines    (1000)        0 2023-05-03 11:29:06.000000 semisup-segmentation-0.0.6/SemiSegAPI/
+-rw-rw-r--   0 adines    (1000) adines    (1000)     8342 2023-05-02 16:24:16.000000 semisup-segmentation-0.0.6/SemiSegAPI/semiSupervised.py
+-rw-rw-r--   0 adines    (1000) adines    (1000)      249 2023-05-03 11:25:10.000000 semisup-segmentation-0.0.6/SemiSegAPI/__init__.py
+-rw-rw-r--   0 adines    (1000) adines    (1000)    10397 2023-05-03 07:51:02.000000 semisup-segmentation-0.0.6/SemiSegAPI/utils.py
```

### Comparing `semisup-segmentation-0.0.5/PKG-INFO` & `semisup-segmentation-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semisup-segmentation
-Version: 0.0.5
+Version: 0.0.6
 Summary: API that provides methods to construct deep segmentation models using semi-supervised methods.
 Home-page: https://github.com/adines/SemiSeg
 Author: Adrian Ines
 Author-email: adines@unirioja.es
 License: UNKNOWN
 Keywords: segmentation,deep learning,semi-supervised
 Platform: UNKNOWN
```

### Comparing `semisup-segmentation-0.0.5/LICENSE.txt` & `semisup-segmentation-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `semisup-segmentation-0.0.5/README.rst` & `semisup-segmentation-0.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `semisup-segmentation-0.0.5/semisup_segmentation.egg-info/PKG-INFO` & `semisup-segmentation-0.0.6/semisup_segmentation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semisup-segmentation
-Version: 0.0.5
+Version: 0.0.6
 Summary: API that provides methods to construct deep segmentation models using semi-supervised methods.
 Home-page: https://github.com/adines/SemiSeg
 Author: Adrian Ines
 Author-email: adines@unirioja.es
 License: UNKNOWN
 Keywords: segmentation,deep learning,semi-supervised
 Platform: UNKNOWN
```

### Comparing `semisup-segmentation-0.0.5/setup.py` & `semisup-segmentation-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     long_description = f.read()
 
 def parse_requirements(filename):
     """ load requirements from a pip requirements file """
     lineiter = (line.strip() for line in open(filename))
     return [line for line in lineiter if line and not line.startswith("#")]
 
-install_reqs = parse_requirements("requirements.txt")
+install_reqs = parse_requirements("semisup_segmentation.egg-info/requires.txt")
 
 def remove_requirements(requirements, remove_elem):
     new_requirements = []
     for requirement in requirements:
         if remove_elem not in requirement:
             new_requirements.append(requirement)
 
@@ -81,15 +81,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.5',  # Required
+    version='0.0.6',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='API that provides methods to construct deep segmentation models using semi-supervised methods.',  # Required
 
     # This is an optional longer description of your project that represents
```

### Comparing `semisup-segmentation-0.0.5/SemiSegAPI/semiSupervised.py` & `semisup-segmentation-0.0.6/SemiSegAPI/semiSupervised.py`

 * *Files identical despite different names*

### Comparing `semisup-segmentation-0.0.5/SemiSegAPI/utils.py` & `semisup-segmentation-0.0.6/SemiSegAPI/utils.py`

 * *Files identical despite different names*

