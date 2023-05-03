# Comparing `tmp/TuoTuo-0.2.4.tar.gz` & `tmp/TuoTuo-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TuoTuo-0.2.4.tar", last modified: Wed May  3 17:10:38 2023, max compression
+gzip compressed data, was "TuoTuo-0.2.5.tar", last modified: Wed May  3 17:20:58 2023, max compression
```

## Comparing `TuoTuo-0.2.4.tar` & `TuoTuo-0.2.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 17:10:38.624464 TuoTuo-0.2.4/
--rw-r--r--   0 ericliu    (501) staff       (20)     6148 2023-03-15 07:18:48.000000 TuoTuo-0.2.4/.DS_Store
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 17:10:38.608046 TuoTuo-0.2.4/.github/
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 17:10:38.612537 TuoTuo-0.2.4/.github/workflows/
--rw-r--r--   0 ericliu    (501) staff       (20)     1313 2023-04-29 20:29:10.000000 TuoTuo-0.2.4/.github/workflows/python-package.yml
--rw-r--r--   0 ericliu    (501) staff       (20)     1337 2023-05-01 20:35:00.000000 TuoTuo-0.2.4/.github/workflows/python-publish.yml
--rw-r--r--   0 ericliu    (501) staff       (20)       89 2023-05-01 21:37:45.000000 TuoTuo-0.2.4/.gitignore
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 17:10:38.613036 TuoTuo-0.2.4/.vscode/
--rw-r--r--   0 ericliu    (501) staff       (20)      520 2023-04-19 20:08:42.000000 TuoTuo-0.2.4/.vscode/c_cpp_properties.json
--rw-r--r--   0 ericliu    (501) staff       (20)     1069 2023-04-29 19:24:24.000000 TuoTuo-0.2.4/LICENSE
--rw-r--r--   0 ericliu    (501) staff       (20)       41 2023-05-03 15:52:33.000000 TuoTuo-0.2.4/MANIFEST.in
--rw-r--r--   0 ericliu    (501) staff       (20)     1538 2023-05-03 17:10:38.624636 TuoTuo-0.2.4/PKG-INFO
--rw-r--r--   0 ericliu    (501) staff       (20)      693 2023-04-22 09:04:54.000000 TuoTuo-0.2.4/README.md
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 17:10:38.613995 TuoTuo-0.2.4/TuoTuo.egg-info/
--rw-r--r--   0 ericliu    (501) staff       (20)     1538 2023-05-03 17:10:38.000000 TuoTuo-0.2.4/TuoTuo.egg-info/PKG-INFO
--rw-r--r--   0 ericliu    (501) staff       (20)      893 2023-05-03 17:10:38.000000 TuoTuo-0.2.4/TuoTuo.egg-info/SOURCES.txt
--rw-r--r--   0 ericliu    (501) staff       (20)        1 2023-05-03 17:10:38.000000 TuoTuo-0.2.4/TuoTuo.egg-info/dependency_links.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       66 2023-05-03 17:10:38.000000 TuoTuo-0.2.4/TuoTuo.egg-info/requires.txt
--rw-r--r--   0 ericliu    (501) staff       (20)        7 2023-05-03 17:10:38.000000 TuoTuo-0.2.4/TuoTuo.egg-info/top_level.txt
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-05-02 13:35:36.000000 TuoTuo-0.2.4/cutils.cpython-38-darwin.so
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 17:10:38.614937 TuoTuo-0.2.4/notebook/
--rw-r--r--   0 ericliu    (501) staff       (20)    56829 2023-05-02 09:53:49.000000 TuoTuo-0.2.4/notebook/Our Model vs SKLearn.ipynb
--rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:28.000000 TuoTuo-0.2.4/notebook/__init__.py
--rw-r--r--   0 ericliu    (501) staff       (20)     1255 2023-05-03 16:56:05.000000 TuoTuo-0.2.4/pyproject.toml
--rw-r--r--   0 ericliu    (501) staff       (20)     1542 2023-05-01 12:02:13.000000 TuoTuo-0.2.4/requirements.txt
--rw-r--r--   0 ericliu    (501) staff       (20)      197 2023-05-03 17:10:38.625001 TuoTuo-0.2.4/setup.cfg
--rw-r--r--   0 ericliu    (501) staff       (20)     2048 2023-05-03 17:10:35.000000 TuoTuo-0.2.4/setup.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 17:10:38.619930 TuoTuo-0.2.4/tuotuo/
--rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:21.000000 TuoTuo-0.2.4/tuotuo/__init__.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 17:10:38.608544 TuoTuo-0.2.4/tuotuo/build/
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 17:10:38.620340 TuoTuo-0.2.4/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.2.4/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 17:10:38.621684 TuoTuo-0.2.4/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/
--rw-r--r--   0 ericliu    (501) staff       (20)  1829576 2023-04-19 20:17:36.000000 TuoTuo-0.2.4/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o
--rw-r--r--   0 ericliu    (501) staff       (20)  1030110 2023-05-02 07:25:21.000000 TuoTuo-0.2.4/tuotuo/cutils.c
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.2.4/tuotuo/cutils.cpython-38-darwin.so
--rw-r--r--   0 ericliu    (501) staff       (20)     2477 2023-04-19 20:11:37.000000 TuoTuo-0.2.4/tuotuo/cutils.pyx
--rw-r--r--   0 ericliu    (501) staff       (20)     9448 2023-04-28 13:26:46.000000 TuoTuo-0.2.4/tuotuo/generator.py
--rw-r--r--   0 ericliu    (501) staff       (20)    16225 2023-05-02 09:53:34.000000 TuoTuo-0.2.4/tuotuo/lda_model.py
--rw-r--r--   0 ericliu    (501) staff       (20)     5422 2023-04-29 19:52:57.000000 TuoTuo-0.2.4/tuotuo/text_pre_processor.py
--rw-r--r--   0 ericliu    (501) staff       (20)     9792 2023-05-02 09:53:39.000000 TuoTuo-0.2.4/tuotuo/utils.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 17:20:58.644782 TuoTuo-0.2.5/
+-rw-r--r--   0 ericliu    (501) staff       (20)     6148 2023-03-15 07:18:48.000000 TuoTuo-0.2.5/.DS_Store
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 17:20:58.629723 TuoTuo-0.2.5/.github/
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 17:20:58.634202 TuoTuo-0.2.5/.github/workflows/
+-rw-r--r--   0 ericliu    (501) staff       (20)     1313 2023-04-29 20:29:10.000000 TuoTuo-0.2.5/.github/workflows/python-package.yml
+-rw-r--r--   0 ericliu    (501) staff       (20)     1337 2023-05-01 20:35:00.000000 TuoTuo-0.2.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 ericliu    (501) staff       (20)       89 2023-05-01 21:37:45.000000 TuoTuo-0.2.5/.gitignore
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 17:20:58.634614 TuoTuo-0.2.5/.vscode/
+-rw-r--r--   0 ericliu    (501) staff       (20)      520 2023-04-19 20:08:42.000000 TuoTuo-0.2.5/.vscode/c_cpp_properties.json
+-rw-r--r--   0 ericliu    (501) staff       (20)     1069 2023-04-29 19:24:24.000000 TuoTuo-0.2.5/LICENSE
+-rw-r--r--   0 ericliu    (501) staff       (20)       41 2023-05-03 15:52:33.000000 TuoTuo-0.2.5/MANIFEST.in
+-rw-r--r--   0 ericliu    (501) staff       (20)     1538 2023-05-03 17:20:58.644906 TuoTuo-0.2.5/PKG-INFO
+-rw-r--r--   0 ericliu    (501) staff       (20)      693 2023-04-22 09:04:54.000000 TuoTuo-0.2.5/README.md
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 17:20:58.635584 TuoTuo-0.2.5/TuoTuo.egg-info/
+-rw-r--r--   0 ericliu    (501) staff       (20)     1538 2023-05-03 17:20:58.000000 TuoTuo-0.2.5/TuoTuo.egg-info/PKG-INFO
+-rw-r--r--   0 ericliu    (501) staff       (20)      893 2023-05-03 17:20:58.000000 TuoTuo-0.2.5/TuoTuo.egg-info/SOURCES.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)        1 2023-05-03 17:20:58.000000 TuoTuo-0.2.5/TuoTuo.egg-info/dependency_links.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)       66 2023-05-03 17:20:58.000000 TuoTuo-0.2.5/TuoTuo.egg-info/requires.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)        7 2023-05-03 17:20:58.000000 TuoTuo-0.2.5/TuoTuo.egg-info/top_level.txt
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-05-02 13:35:36.000000 TuoTuo-0.2.5/cutils.cpython-38-darwin.so
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 17:20:58.636508 TuoTuo-0.2.5/notebook/
+-rw-r--r--   0 ericliu    (501) staff       (20)    56829 2023-05-02 09:53:49.000000 TuoTuo-0.2.5/notebook/Our Model vs SKLearn.ipynb
+-rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:28.000000 TuoTuo-0.2.5/notebook/__init__.py
+-rw-r--r--   0 ericliu    (501) staff       (20)      505 2023-05-03 17:19:05.000000 TuoTuo-0.2.5/pyproject.toml
+-rw-r--r--   0 ericliu    (501) staff       (20)     1542 2023-05-01 12:02:13.000000 TuoTuo-0.2.5/requirements.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)      197 2023-05-03 17:20:58.645239 TuoTuo-0.2.5/setup.cfg
+-rw-r--r--   0 ericliu    (501) staff       (20)     2022 2023-05-03 17:20:51.000000 TuoTuo-0.2.5/setup.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 17:20:58.640511 TuoTuo-0.2.5/tuotuo/
+-rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:21.000000 TuoTuo-0.2.5/tuotuo/__init__.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 17:20:58.630232 TuoTuo-0.2.5/tuotuo/build/
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 17:20:58.640944 TuoTuo-0.2.5/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.2.5/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 17:20:58.642216 TuoTuo-0.2.5/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/
+-rw-r--r--   0 ericliu    (501) staff       (20)  1829576 2023-04-19 20:17:36.000000 TuoTuo-0.2.5/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o
+-rw-r--r--   0 ericliu    (501) staff       (20)  1030110 2023-05-02 07:25:21.000000 TuoTuo-0.2.5/tuotuo/cutils.c
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.2.5/tuotuo/cutils.cpython-38-darwin.so
+-rw-r--r--   0 ericliu    (501) staff       (20)     2477 2023-04-19 20:11:37.000000 TuoTuo-0.2.5/tuotuo/cutils.pyx
+-rw-r--r--   0 ericliu    (501) staff       (20)     9448 2023-04-28 13:26:46.000000 TuoTuo-0.2.5/tuotuo/generator.py
+-rw-r--r--   0 ericliu    (501) staff       (20)    16225 2023-05-02 09:53:34.000000 TuoTuo-0.2.5/tuotuo/lda_model.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     5422 2023-04-29 19:52:57.000000 TuoTuo-0.2.5/tuotuo/text_pre_processor.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     9792 2023-05-02 09:53:39.000000 TuoTuo-0.2.5/tuotuo/utils.py
```

### Comparing `TuoTuo-0.2.4/.DS_Store` & `TuoTuo-0.2.5/.DS_Store`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.4/.github/workflows/python-package.yml` & `TuoTuo-0.2.5/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.4/.github/workflows/python-publish.yml` & `TuoTuo-0.2.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.4/.vscode/c_cpp_properties.json` & `TuoTuo-0.2.5/.vscode/c_cpp_properties.json`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.4/LICENSE` & `TuoTuo-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.4/PKG-INFO` & `TuoTuo-0.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: TuoTuo
-Version: 0.2.4
+Version: 0.2.5
 Summary: LDA & Neura based topic modelling library
 Home-page: https://github.com/RobbenRibery/TuoTuo
-Download-URL: https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/pypi-test-0.04.tar.gz
+Download-URL: https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/pypi-test-0.05.tar.gz
 Author: tuotuo Superman
 Author-email: tuotuo@HanwellSquare.BigForce.com
 License: MIT
 Keywords: Generative Topic Modelling,Latent Dirichlet Allocation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `TuoTuo-0.2.4/README.md` & `TuoTuo-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.4/TuoTuo.egg-info/PKG-INFO` & `TuoTuo-0.2.5/TuoTuo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: TuoTuo
-Version: 0.2.4
+Version: 0.2.5
 Summary: LDA & Neura based topic modelling library
 Home-page: https://github.com/RobbenRibery/TuoTuo
-Download-URL: https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/pypi-test-0.04.tar.gz
+Download-URL: https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/pypi-test-0.05.tar.gz
 Author: tuotuo Superman
 Author-email: tuotuo@HanwellSquare.BigForce.com
 License: MIT
 Keywords: Generative Topic Modelling,Latent Dirichlet Allocation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `TuoTuo-0.2.4/TuoTuo.egg-info/SOURCES.txt` & `TuoTuo-0.2.5/TuoTuo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.4/cutils.cpython-38-darwin.so` & `TuoTuo-0.2.5/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.4/notebook/Our Model vs SKLearn.ipynb` & `TuoTuo-0.2.5/notebook/Our Model vs SKLearn.ipynb`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.4/requirements.txt` & `TuoTuo-0.2.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.4/setup.py` & `TuoTuo-0.2.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,30 +21,28 @@
     libraries= ['Cython']
 )
 
 def cythonise_extensions(extensions): 
     from Cython.Build import cythonize
     return cythonize(
         extensions, 
-        annotate = True,
-
     )
 
 setup(
     name = 'TuoTuo',
     packages = ['tuotuo'],
-    version = '0.2.4',  
+    version = '0.2.5',  
     license='MIT',
     description = 'LDA & Neura based topic modelling library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'tuotuo Superman',
     author_email = 'tuotuo@HanwellSquare.BigForce.com',
     url = 'https://github.com/RobbenRibery/TuoTuo',
-    download_url = 'https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/pypi-test-0.04.tar.gz',
+    download_url = 'https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/pypi-test-0.05.tar.gz',
     keywords = ['Generative Topic Modelling','Latent Dirichlet Allocation'],
     install_requires=[            
         'numpy',
         'torch',
         'scipy',
         'pyro-ppl',
         'pandas',
```

### Comparing `TuoTuo-0.2.4/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so` & `TuoTuo-0.2.5/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.4/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o` & `TuoTuo-0.2.5/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.4/tuotuo/cutils.c` & `TuoTuo-0.2.5/tuotuo/cutils.c`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.4/tuotuo/cutils.cpython-38-darwin.so` & `TuoTuo-0.2.5/tuotuo/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.4/tuotuo/cutils.pyx` & `TuoTuo-0.2.5/tuotuo/cutils.pyx`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.4/tuotuo/generator.py` & `TuoTuo-0.2.5/tuotuo/generator.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.4/tuotuo/lda_model.py` & `TuoTuo-0.2.5/tuotuo/lda_model.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.4/tuotuo/text_pre_processor.py` & `TuoTuo-0.2.5/tuotuo/text_pre_processor.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.4/tuotuo/utils.py` & `TuoTuo-0.2.5/tuotuo/utils.py`

 * *Files identical despite different names*

