# Comparing `tmp/collectmeterdigits-1.0.6.tar.gz` & `tmp/collectmeterdigits-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collectmeterdigits-1.0.6.tar", last modified: Tue May  2 21:56:31 2023, max compression
+gzip compressed data, was "collectmeterdigits-1.0.7.tar", last modified: Tue May  2 22:16:28 2023, max compression
```

## Comparing `collectmeterdigits-1.0.6.tar` & `collectmeterdigits-1.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:56:31.371687 collectmeterdigits-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 21:56:18.000000 collectmeterdigits-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-02 21:56:31.371687 collectmeterdigits-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-02 21:56:18.000000 collectmeterdigits-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:56:31.367687 collectmeterdigits-1.0.6/collectmeterdigits/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:56:18.000000 collectmeterdigits-1.0.6/collectmeterdigits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-02 21:56:18.000000 collectmeterdigits-1.0.6/collectmeterdigits/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-05-02 21:56:18.000000 collectmeterdigits-1.0.6/collectmeterdigits/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-02 21:56:18.000000 collectmeterdigits-1.0.6/collectmeterdigits/glob.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-02 21:56:18.000000 collectmeterdigits-1.0.6/collectmeterdigits/hash_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-05-02 21:56:18.000000 collectmeterdigits-1.0.6/collectmeterdigits/labeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:56:31.371687 collectmeterdigits-1.0.6/collectmeterdigits/models/
--rw-r--r--   0 runner    (1001) docker     (123)   226480 2023-05-02 21:56:18.000000 collectmeterdigits-1.0.6/collectmeterdigits/models/dig-class100-0160_s2_q.tflite
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-02 21:56:18.000000 collectmeterdigits-1.0.6/collectmeterdigits/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:56:31.371687 collectmeterdigits-1.0.6/collectmeterdigits.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-02 21:56:31.000000 collectmeterdigits-1.0.6/collectmeterdigits.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-02 21:56:31.000000 collectmeterdigits-1.0.6/collectmeterdigits.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:56:31.000000 collectmeterdigits-1.0.6/collectmeterdigits.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-02 21:56:31.000000 collectmeterdigits-1.0.6/collectmeterdigits.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 21:56:31.000000 collectmeterdigits-1.0.6/collectmeterdigits.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:56:31.371687 collectmeterdigits-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-02 21:56:18.000000 collectmeterdigits-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:16:28.923728 collectmeterdigits-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 22:16:18.000000 collectmeterdigits-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-02 22:16:28.923728 collectmeterdigits-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-02 22:16:18.000000 collectmeterdigits-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:16:28.923728 collectmeterdigits-1.0.7/collectmeterdigits/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 22:16:18.000000 collectmeterdigits-1.0.7/collectmeterdigits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-02 22:16:18.000000 collectmeterdigits-1.0.7/collectmeterdigits/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-05-02 22:16:18.000000 collectmeterdigits-1.0.7/collectmeterdigits/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-02 22:16:18.000000 collectmeterdigits-1.0.7/collectmeterdigits/glob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-02 22:16:18.000000 collectmeterdigits-1.0.7/collectmeterdigits/hash_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-05-02 22:16:18.000000 collectmeterdigits-1.0.7/collectmeterdigits/labeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:16:28.923728 collectmeterdigits-1.0.7/collectmeterdigits/models/
+-rw-r--r--   0 runner    (1001) docker     (123)   226480 2023-05-02 22:16:18.000000 collectmeterdigits-1.0.7/collectmeterdigits/models/dig-class100-0160_s2_q.tflite
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-02 22:16:18.000000 collectmeterdigits-1.0.7/collectmeterdigits/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:16:28.923728 collectmeterdigits-1.0.7/collectmeterdigits.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-02 22:16:28.000000 collectmeterdigits-1.0.7/collectmeterdigits.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-02 22:16:28.000000 collectmeterdigits-1.0.7/collectmeterdigits.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 22:16:28.000000 collectmeterdigits-1.0.7/collectmeterdigits.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-02 22:16:28.000000 collectmeterdigits-1.0.7/collectmeterdigits.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 22:16:28.000000 collectmeterdigits-1.0.7/collectmeterdigits.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 22:16:28.923728 collectmeterdigits-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-02 22:16:18.000000 collectmeterdigits-1.0.7/setup.py
```

### Comparing `collectmeterdigits-1.0.6/LICENSE` & `collectmeterdigits-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `collectmeterdigits-1.0.6/PKG-INFO` & `collectmeterdigits-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collectmeterdigits
-Version: 1.0.6
+Version: 1.0.7
 Summary: Reads images from digital meters.
 Home-page: https://github.com/haverland/collectmeterdigits
 Author: Frank Haverland
 Author-email: iotson@t-online.de
 License: Apache 2.0
 Keywords: different tags here
 Platform: any
```

### Comparing `collectmeterdigits-1.0.6/README.md` & `collectmeterdigits-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `collectmeterdigits-1.0.6/collectmeterdigits/__main__.py` & `collectmeterdigits-1.0.7/collectmeterdigits/__main__.py`

 * *Files identical despite different names*

### Comparing `collectmeterdigits-1.0.6/collectmeterdigits/collect.py` & `collectmeterdigits-1.0.7/collectmeterdigits/collect.py`

 * *Files identical despite different names*

### Comparing `collectmeterdigits-1.0.6/collectmeterdigits/hash_manual.py` & `collectmeterdigits-1.0.7/collectmeterdigits/hash_manual.py`

 * *Files identical despite different names*

### Comparing `collectmeterdigits-1.0.6/collectmeterdigits/labeling.py` & `collectmeterdigits-1.0.7/collectmeterdigits/labeling.py`

 * *Files identical despite different names*

### Comparing `collectmeterdigits-1.0.6/collectmeterdigits/models/dig-class100-0160_s2_q.tflite` & `collectmeterdigits-1.0.7/collectmeterdigits/models/dig-class100-0160_s2_q.tflite`

 * *Files identical despite different names*

### Comparing `collectmeterdigits-1.0.6/collectmeterdigits/predict.py` & `collectmeterdigits-1.0.7/collectmeterdigits/predict.py`

 * *Files identical despite different names*

### Comparing `collectmeterdigits-1.0.6/collectmeterdigits.egg-info/PKG-INFO` & `collectmeterdigits-1.0.7/collectmeterdigits.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collectmeterdigits
-Version: 1.0.6
+Version: 1.0.7
 Summary: Reads images from digital meters.
 Home-page: https://github.com/haverland/collectmeterdigits
 Author: Frank Haverland
 Author-email: iotson@t-online.de
 License: Apache 2.0
 Keywords: different tags here
 Platform: any
```

### Comparing `collectmeterdigits-1.0.6/setup.py` & `collectmeterdigits-1.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,29 +15,30 @@
     and removes duplicated.
     The images will be anonymized (name replaced with hash).
     At last step, the images will be pre labeled by a neuronal network
     """
 
 setup(
     name='collectmeterdigits',
-    version='1.0.6',
+    version='1.0.7',
     url='https://github.com/haverland/collectmeterdigits',
     license='Apache 2.0',
     author='Frank Haverland',
     author_email='iotson@t-online.de',
     install_requires=['pillow',
                     'numpy',
                     'matplotlib',
                     'scipy',
                     'scikit-learn',
                     'imagehash',
                     'urllib3',
                     'requests',
                     'pandas',
-                    'tflite-runtime;sys_platform == "linux"'],
+                    'tflite-runtime;sys_platform == "linux"',
+                    'msvc-runtime;sys_platform == "windows"' ],
     tests_require=['nose'],
     packages=find_packages(exclude=['tests']),
     description='Reads images from digital meters.',
     long_description = long_description,
     platforms='any',
     keywords = "different tags here",
     classifiers = [
```

