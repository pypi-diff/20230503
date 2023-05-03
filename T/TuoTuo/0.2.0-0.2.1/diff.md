# Comparing `tmp/TuoTuo-0.2.0.tar.gz` & `tmp/TuoTuo-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TuoTuo-0.2.0.tar", last modified: Tue May  2 14:47:51 2023, max compression
+gzip compressed data, was "TuoTuo-0.2.1.tar", last modified: Wed May  3 14:59:34 2023, max compression
```

## Comparing `TuoTuo-0.2.0.tar` & `TuoTuo-0.2.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 14:47:51.261454 TuoTuo-0.2.0/
--rw-r--r--   0 ericliu    (501) staff       (20)     6148 2023-03-15 07:18:48.000000 TuoTuo-0.2.0/.DS_Store
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 14:47:51.245336 TuoTuo-0.2.0/.github/
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 14:47:51.249707 TuoTuo-0.2.0/.github/workflows/
--rw-r--r--   0 ericliu    (501) staff       (20)     1313 2023-04-29 20:29:10.000000 TuoTuo-0.2.0/.github/workflows/python-package.yml
--rw-r--r--   0 ericliu    (501) staff       (20)     1337 2023-05-01 20:35:00.000000 TuoTuo-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 ericliu    (501) staff       (20)       89 2023-05-01 21:37:45.000000 TuoTuo-0.2.0/.gitignore
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 14:47:51.250354 TuoTuo-0.2.0/.vscode/
--rw-r--r--   0 ericliu    (501) staff       (20)      520 2023-04-19 20:08:42.000000 TuoTuo-0.2.0/.vscode/c_cpp_properties.json
--rw-r--r--   0 ericliu    (501) staff       (20)     1069 2023-04-29 19:24:24.000000 TuoTuo-0.2.0/LICENSE
--rw-r--r--   0 ericliu    (501) staff       (20)       24 2023-05-02 13:32:32.000000 TuoTuo-0.2.0/MANIFEST.in
--rw-r--r--   0 ericliu    (501) staff       (20)     1538 2023-05-02 14:47:51.261642 TuoTuo-0.2.0/PKG-INFO
--rw-r--r--   0 ericliu    (501) staff       (20)      693 2023-04-22 09:04:54.000000 TuoTuo-0.2.0/README.md
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 14:47:51.251431 TuoTuo-0.2.0/TuoTuo.egg-info/
--rw-r--r--   0 ericliu    (501) staff       (20)     1538 2023-05-02 14:47:51.000000 TuoTuo-0.2.0/TuoTuo.egg-info/PKG-INFO
--rw-r--r--   0 ericliu    (501) staff       (20)      907 2023-05-02 14:47:51.000000 TuoTuo-0.2.0/TuoTuo.egg-info/SOURCES.txt
--rw-r--r--   0 ericliu    (501) staff       (20)        1 2023-05-02 14:47:51.000000 TuoTuo-0.2.0/TuoTuo.egg-info/dependency_links.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       59 2023-05-02 14:47:51.000000 TuoTuo-0.2.0/TuoTuo.egg-info/requires.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       21 2023-05-02 14:47:51.000000 TuoTuo-0.2.0/TuoTuo.egg-info/top_level.txt
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-05-02 13:35:36.000000 TuoTuo-0.2.0/cutils.cpython-38-darwin.so
--rw-r--r--   0 ericliu    (501) staff       (20)    13943 2023-05-02 13:32:32.000000 TuoTuo-0.2.0/cysetuptools.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 14:47:51.252538 TuoTuo-0.2.0/notebook/
--rw-r--r--   0 ericliu    (501) staff       (20)    56829 2023-05-02 09:53:49.000000 TuoTuo-0.2.0/notebook/Our Model vs SKLearn.ipynb
--rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:28.000000 TuoTuo-0.2.0/notebook/__init__.py
--rw-r--r--   0 ericliu    (501) staff       (20)      123 2023-05-02 13:10:01.000000 TuoTuo-0.2.0/project.toml
--rw-r--r--   0 ericliu    (501) staff       (20)     1542 2023-05-01 12:02:13.000000 TuoTuo-0.2.0/requirements.txt
--rw-r--r--   0 ericliu    (501) staff       (20)      197 2023-05-02 14:47:51.264814 TuoTuo-0.2.0/setup.cfg
--rw-r--r--   0 ericliu    (501) staff       (20)     2030 2023-05-02 14:47:46.000000 TuoTuo-0.2.0/setup.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 14:47:51.257087 TuoTuo-0.2.0/tuotuo/
--rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:21.000000 TuoTuo-0.2.0/tuotuo/__init__.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 14:47:51.245853 TuoTuo-0.2.0/tuotuo/build/
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 14:47:51.257513 TuoTuo-0.2.0/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.2.0/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 14:47:51.258825 TuoTuo-0.2.0/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/
--rw-r--r--   0 ericliu    (501) staff       (20)  1829576 2023-04-19 20:17:36.000000 TuoTuo-0.2.0/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o
--rw-r--r--   0 ericliu    (501) staff       (20)  1030110 2023-05-02 07:25:21.000000 TuoTuo-0.2.0/tuotuo/cutils.c
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.2.0/tuotuo/cutils.cpython-38-darwin.so
--rw-r--r--   0 ericliu    (501) staff       (20)     2477 2023-04-19 20:11:37.000000 TuoTuo-0.2.0/tuotuo/cutils.pyx
--rw-r--r--   0 ericliu    (501) staff       (20)     9448 2023-04-28 13:26:46.000000 TuoTuo-0.2.0/tuotuo/generator.py
--rw-r--r--   0 ericliu    (501) staff       (20)    16225 2023-05-02 09:53:34.000000 TuoTuo-0.2.0/tuotuo/lda_model.py
--rw-r--r--   0 ericliu    (501) staff       (20)     5422 2023-04-29 19:52:57.000000 TuoTuo-0.2.0/tuotuo/text_pre_processor.py
--rw-r--r--   0 ericliu    (501) staff       (20)     9792 2023-05-02 09:53:39.000000 TuoTuo-0.2.0/tuotuo/utils.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 14:59:34.919585 TuoTuo-0.2.1/
+-rw-r--r--   0 ericliu    (501) staff       (20)     6148 2023-03-15 07:18:48.000000 TuoTuo-0.2.1/.DS_Store
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 14:59:34.889152 TuoTuo-0.2.1/.github/
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 14:59:34.894574 TuoTuo-0.2.1/.github/workflows/
+-rw-r--r--   0 ericliu    (501) staff       (20)     1313 2023-04-29 20:29:10.000000 TuoTuo-0.2.1/.github/workflows/python-package.yml
+-rw-r--r--   0 ericliu    (501) staff       (20)     1337 2023-05-01 20:35:00.000000 TuoTuo-0.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 ericliu    (501) staff       (20)       89 2023-05-01 21:37:45.000000 TuoTuo-0.2.1/.gitignore
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 14:59:34.894902 TuoTuo-0.2.1/.vscode/
+-rw-r--r--   0 ericliu    (501) staff       (20)      520 2023-04-19 20:08:42.000000 TuoTuo-0.2.1/.vscode/c_cpp_properties.json
+-rw-r--r--   0 ericliu    (501) staff       (20)     1069 2023-04-29 19:24:24.000000 TuoTuo-0.2.1/LICENSE
+-rw-r--r--   0 ericliu    (501) staff       (20)       24 2023-05-02 13:32:32.000000 TuoTuo-0.2.1/MANIFEST.in
+-rw-r--r--   0 ericliu    (501) staff       (20)     1538 2023-05-03 14:59:34.919742 TuoTuo-0.2.1/PKG-INFO
+-rw-r--r--   0 ericliu    (501) staff       (20)      693 2023-04-22 09:04:54.000000 TuoTuo-0.2.1/README.md
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 14:59:34.895855 TuoTuo-0.2.1/TuoTuo.egg-info/
+-rw-r--r--   0 ericliu    (501) staff       (20)     1538 2023-05-03 14:59:34.000000 TuoTuo-0.2.1/TuoTuo.egg-info/PKG-INFO
+-rw-r--r--   0 ericliu    (501) staff       (20)      907 2023-05-03 14:59:34.000000 TuoTuo-0.2.1/TuoTuo.egg-info/SOURCES.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)        1 2023-05-03 14:59:34.000000 TuoTuo-0.2.1/TuoTuo.egg-info/dependency_links.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)       66 2023-05-03 14:59:34.000000 TuoTuo-0.2.1/TuoTuo.egg-info/requires.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)       21 2023-05-03 14:59:34.000000 TuoTuo-0.2.1/TuoTuo.egg-info/top_level.txt
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-05-02 13:35:36.000000 TuoTuo-0.2.1/cutils.cpython-38-darwin.so
+-rw-r--r--   0 ericliu    (501) staff       (20)    13943 2023-05-02 13:32:32.000000 TuoTuo-0.2.1/cysetuptools.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 14:59:34.897814 TuoTuo-0.2.1/notebook/
+-rw-r--r--   0 ericliu    (501) staff       (20)    56829 2023-05-02 09:53:49.000000 TuoTuo-0.2.1/notebook/Our Model vs SKLearn.ipynb
+-rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:28.000000 TuoTuo-0.2.1/notebook/__init__.py
+-rw-r--r--   0 ericliu    (501) staff       (20)      122 2023-05-03 14:55:45.000000 TuoTuo-0.2.1/project.toml
+-rw-r--r--   0 ericliu    (501) staff       (20)     1542 2023-05-01 12:02:13.000000 TuoTuo-0.2.1/requirements.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)      197 2023-05-03 14:59:34.920074 TuoTuo-0.2.1/setup.cfg
+-rw-r--r--   0 ericliu    (501) staff       (20)     2048 2023-05-03 14:59:21.000000 TuoTuo-0.2.1/setup.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 14:59:34.901773 TuoTuo-0.2.1/tuotuo/
+-rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:21.000000 TuoTuo-0.2.1/tuotuo/__init__.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 14:59:34.889645 TuoTuo-0.2.1/tuotuo/build/
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 14:59:34.902197 TuoTuo-0.2.1/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.2.1/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-03 14:59:34.903754 TuoTuo-0.2.1/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/
+-rw-r--r--   0 ericliu    (501) staff       (20)  1829576 2023-04-19 20:17:36.000000 TuoTuo-0.2.1/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o
+-rw-r--r--   0 ericliu    (501) staff       (20)  1030110 2023-05-02 07:25:21.000000 TuoTuo-0.2.1/tuotuo/cutils.c
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.2.1/tuotuo/cutils.cpython-38-darwin.so
+-rw-r--r--   0 ericliu    (501) staff       (20)     2477 2023-04-19 20:11:37.000000 TuoTuo-0.2.1/tuotuo/cutils.pyx
+-rw-r--r--   0 ericliu    (501) staff       (20)     9448 2023-04-28 13:26:46.000000 TuoTuo-0.2.1/tuotuo/generator.py
+-rw-r--r--   0 ericliu    (501) staff       (20)    16225 2023-05-02 09:53:34.000000 TuoTuo-0.2.1/tuotuo/lda_model.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     5422 2023-04-29 19:52:57.000000 TuoTuo-0.2.1/tuotuo/text_pre_processor.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     9792 2023-05-02 09:53:39.000000 TuoTuo-0.2.1/tuotuo/utils.py
```

### Comparing `TuoTuo-0.2.0/.DS_Store` & `TuoTuo-0.2.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.0/.github/workflows/python-package.yml` & `TuoTuo-0.2.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.0/.github/workflows/python-publish.yml` & `TuoTuo-0.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.0/.vscode/c_cpp_properties.json` & `TuoTuo-0.2.1/.vscode/c_cpp_properties.json`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.0/LICENSE` & `TuoTuo-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.0/PKG-INFO` & `TuoTuo-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: TuoTuo
-Version: 0.2.0
+Version: 0.2.1
 Summary: LDA & Neura based topic modelling library
 Home-page: https://github.com/RobbenRibery/TuoTuo
-Download-URL: https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/pypi-test-0.01.tar.gz
+Download-URL: https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/pypi-test-0.02.tar.gz
 Author: tuotuo Superman
 Author-email: tuotuo@HanwellSquare.BigForce.com
 License: MIT
 Keywords: Generative Topic Modelling,Latent Dirichlet Allocation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `TuoTuo-0.2.0/README.md` & `TuoTuo-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.0/TuoTuo.egg-info/PKG-INFO` & `TuoTuo-0.2.1/TuoTuo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: TuoTuo
-Version: 0.2.0
+Version: 0.2.1
 Summary: LDA & Neura based topic modelling library
 Home-page: https://github.com/RobbenRibery/TuoTuo
-Download-URL: https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/pypi-test-0.01.tar.gz
+Download-URL: https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/pypi-test-0.02.tar.gz
 Author: tuotuo Superman
 Author-email: tuotuo@HanwellSquare.BigForce.com
 License: MIT
 Keywords: Generative Topic Modelling,Latent Dirichlet Allocation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `TuoTuo-0.2.0/TuoTuo.egg-info/SOURCES.txt` & `TuoTuo-0.2.1/TuoTuo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.0/cutils.cpython-38-darwin.so` & `TuoTuo-0.2.1/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.0/cysetuptools.py` & `TuoTuo-0.2.1/cysetuptools.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.0/notebook/Our Model vs SKLearn.ipynb` & `TuoTuo-0.2.1/notebook/Our Model vs SKLearn.ipynb`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.0/requirements.txt` & `TuoTuo-0.2.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.0/setup.py` & `TuoTuo-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,32 +28,33 @@
         annotate = True,
 
     )
 
 setup(
     name = 'TuoTuo',
     packages = ['tuotuo'],
-    version = '0.2.0',  
+    version = '0.2.1',  
     license='MIT',
     description = 'LDA & Neura based topic modelling library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'tuotuo Superman',
     author_email = 'tuotuo@HanwellSquare.BigForce.com',
     url = 'https://github.com/RobbenRibery/TuoTuo',
-    download_url = 'https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/pypi-test-0.01.tar.gz',
+    download_url = 'https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/pypi-test-0.02.tar.gz',
     keywords = ['Generative Topic Modelling','Latent Dirichlet Allocation'],
     install_requires=[            
         'numpy',
         'torch',
         'scipy',
         'pyro-ppl',
         'pandas',
         'nltk',
         'spacy',
+        'cython',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha', 
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'License :: OSI Approved :: MIT License',  
         'Programming Language :: Python :: 3.8',
```

### Comparing `TuoTuo-0.2.0/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so` & `TuoTuo-0.2.1/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.0/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o` & `TuoTuo-0.2.1/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.0/tuotuo/cutils.c` & `TuoTuo-0.2.1/tuotuo/cutils.c`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.0/tuotuo/cutils.cpython-38-darwin.so` & `TuoTuo-0.2.1/tuotuo/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.0/tuotuo/cutils.pyx` & `TuoTuo-0.2.1/tuotuo/cutils.pyx`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.0/tuotuo/generator.py` & `TuoTuo-0.2.1/tuotuo/generator.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.0/tuotuo/lda_model.py` & `TuoTuo-0.2.1/tuotuo/lda_model.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.0/tuotuo/text_pre_processor.py` & `TuoTuo-0.2.1/tuotuo/text_pre_processor.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.2.0/tuotuo/utils.py` & `TuoTuo-0.2.1/tuotuo/utils.py`

 * *Files identical despite different names*

