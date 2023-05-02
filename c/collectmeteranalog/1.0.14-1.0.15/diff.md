# Comparing `tmp/collectmeteranalog-1.0.14.tar.gz` & `tmp/collectmeteranalog-1.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collectmeteranalog-1.0.14.tar", last modified: Tue May  2 21:57:19 2023, max compression
+gzip compressed data, was "collectmeteranalog-1.0.15.tar", last modified: Tue May  2 22:14:22 2023, max compression
```

## Comparing `collectmeteranalog-1.0.14.tar` & `collectmeteranalog-1.0.15.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:19.895984 collectmeteranalog-1.0.14/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 21:57:03.000000 collectmeteranalog-1.0.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-02 21:57:19.895984 collectmeteranalog-1.0.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-02 21:57:03.000000 collectmeteranalog-1.0.14/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:19.895984 collectmeteranalog-1.0.14/collectmeteranalog/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:57:03.000000 collectmeteranalog-1.0.14/collectmeteranalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-02 21:57:03.000000 collectmeteranalog-1.0.14/collectmeteranalog/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8933 2023-05-02 21:57:03.000000 collectmeteranalog-1.0.14/collectmeteranalog/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 21:57:03.000000 collectmeteranalog-1.0.14/collectmeteranalog/glob.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-02 21:57:03.000000 collectmeteranalog-1.0.14/collectmeteranalog/hash_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-05-02 21:57:03.000000 collectmeteranalog-1.0.14/collectmeteranalog/labeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:19.895984 collectmeteranalog-1.0.14/collectmeteranalog/models/
--rw-r--r--   0 runner    (1001) docker     (123)   132304 2023-05-02 21:57:03.000000 collectmeteranalog-1.0.14/collectmeteranalog/models/ana-class100_0157_s1_q.tflite
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-02 21:57:03.000000 collectmeteranalog-1.0.14/collectmeteranalog/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:19.895984 collectmeteranalog-1.0.14/collectmeteranalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-02 21:57:19.000000 collectmeteranalog-1.0.14/collectmeteranalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-02 21:57:19.000000 collectmeteranalog-1.0.14/collectmeteranalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:57:19.000000 collectmeteranalog-1.0.14/collectmeteranalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-02 21:57:19.000000 collectmeteranalog-1.0.14/collectmeteranalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 21:57:19.000000 collectmeteranalog-1.0.14/collectmeteranalog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:57:19.895984 collectmeteranalog-1.0.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-02 21:57:03.000000 collectmeteranalog-1.0.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:14:22.666493 collectmeteranalog-1.0.15/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 22:14:06.000000 collectmeteranalog-1.0.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-02 22:14:22.666493 collectmeteranalog-1.0.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-02 22:14:06.000000 collectmeteranalog-1.0.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:14:22.666493 collectmeteranalog-1.0.15/collectmeteranalog/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 22:14:06.000000 collectmeteranalog-1.0.15/collectmeteranalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-02 22:14:06.000000 collectmeteranalog-1.0.15/collectmeteranalog/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8933 2023-05-02 22:14:06.000000 collectmeteranalog-1.0.15/collectmeteranalog/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 22:14:06.000000 collectmeteranalog-1.0.15/collectmeteranalog/glob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-02 22:14:06.000000 collectmeteranalog-1.0.15/collectmeteranalog/hash_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-05-02 22:14:06.000000 collectmeteranalog-1.0.15/collectmeteranalog/labeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:14:22.666493 collectmeteranalog-1.0.15/collectmeteranalog/models/
+-rw-r--r--   0 runner    (1001) docker     (123)   132304 2023-05-02 22:14:06.000000 collectmeteranalog-1.0.15/collectmeteranalog/models/ana-class100_0157_s1_q.tflite
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-02 22:14:06.000000 collectmeteranalog-1.0.15/collectmeteranalog/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:14:22.666493 collectmeteranalog-1.0.15/collectmeteranalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-02 22:14:22.000000 collectmeteranalog-1.0.15/collectmeteranalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-02 22:14:22.000000 collectmeteranalog-1.0.15/collectmeteranalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 22:14:22.000000 collectmeteranalog-1.0.15/collectmeteranalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-02 22:14:22.000000 collectmeteranalog-1.0.15/collectmeteranalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 22:14:22.000000 collectmeteranalog-1.0.15/collectmeteranalog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 22:14:22.666493 collectmeteranalog-1.0.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-02 22:14:06.000000 collectmeteranalog-1.0.15/setup.py
```

### Comparing `collectmeteranalog-1.0.14/LICENSE` & `collectmeteranalog-1.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `collectmeteranalog-1.0.14/PKG-INFO` & `collectmeteranalog-1.0.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collectmeteranalog
-Version: 1.0.14
+Version: 1.0.15
 Summary: Reads images from water meter pointers.
 Home-page: https://github.com/haverland/collectmeteranalog
 Author: Frank Haverland
 Author-email: iotson@t-online.de
 License: Apache 2.0
 Keywords: different tags here
 Platform: any
```

### Comparing `collectmeteranalog-1.0.14/README.md` & `collectmeteranalog-1.0.15/README.md`

 * *Files identical despite different names*

### Comparing `collectmeteranalog-1.0.14/collectmeteranalog/__main__.py` & `collectmeteranalog-1.0.15/collectmeteranalog/__main__.py`

 * *Files identical despite different names*

### Comparing `collectmeteranalog-1.0.14/collectmeteranalog/collect.py` & `collectmeteranalog-1.0.15/collectmeteranalog/collect.py`

 * *Files identical despite different names*

### Comparing `collectmeteranalog-1.0.14/collectmeteranalog/hash_manual.py` & `collectmeteranalog-1.0.15/collectmeteranalog/hash_manual.py`

 * *Files identical despite different names*

### Comparing `collectmeteranalog-1.0.14/collectmeteranalog/labeling.py` & `collectmeteranalog-1.0.15/collectmeteranalog/labeling.py`

 * *Files identical despite different names*

### Comparing `collectmeteranalog-1.0.14/collectmeteranalog/models/ana-class100_0157_s1_q.tflite` & `collectmeteranalog-1.0.15/collectmeteranalog/models/ana-class100_0157_s1_q.tflite`

 * *Files identical despite different names*

### Comparing `collectmeteranalog-1.0.14/collectmeteranalog/predict.py` & `collectmeteranalog-1.0.15/collectmeteranalog/predict.py`

 * *Files identical despite different names*

### Comparing `collectmeteranalog-1.0.14/collectmeteranalog.egg-info/PKG-INFO` & `collectmeteranalog-1.0.15/collectmeteranalog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collectmeteranalog
-Version: 1.0.14
+Version: 1.0.15
 Summary: Reads images from water meter pointers.
 Home-page: https://github.com/haverland/collectmeteranalog
 Author: Frank Haverland
 Author-email: iotson@t-online.de
 License: Apache 2.0
 Keywords: different tags here
 Platform: any
```

### Comparing `collectmeteranalog-1.0.14/setup.py` & `collectmeteranalog-1.0.15/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     and removes duplicated.
     The images will be anonymized (name replaced with hash).
     At last step, the images will be pre labeled by a neuronal network
     """
 
 setup(
     name='collectmeteranalog',
-    version='1.0.14',
+    version='1.0.15',
     url='https://github.com/haverland/collectmeteranalog',
     license='Apache 2.0',
     author='Frank Haverland',
     author_email='iotson@t-online.de',
     include_package_data=True,
     install_requires=['pillow',
                     'numpy',
@@ -31,15 +31,16 @@
                     'scipy',
                     'scikit-learn',
                     'imagehash',
                     'urllib3',
                     'requests',
                     'pandas',
                     'tflite-runtime; sys_platform == "linux"',
-                    'importlib-metadata; python_version == "3.9"'],
+                    'importlib-metadata; python_version == "3.9"',
+                    'msvc-runtime;sys_platform == "windows"'],
     tests_require=['nose'],
     packages=find_packages(exclude=['tests']),
     description='Reads images from water meter pointers.',
     long_description = long_description,
     platforms='any',
     keywords = "different tags here",
     classifiers = [
```

