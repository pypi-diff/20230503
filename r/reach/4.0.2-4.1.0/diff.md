# Comparing `tmp/reach-4.0.2.tar.gz` & `tmp/reach-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reach-4.0.2.tar", last modified: Wed May  3 10:42:06 2023, max compression
+gzip compressed data, was "reach-4.1.0.tar", last modified: Wed May  3 10:42:23 2023, max compression
```

## Comparing `reach-4.0.2.tar` & `reach-4.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 stephantulkens   (501) staff       (20)        0 2023-05-03 10:42:06.094861 reach-4.0.2/
--rw-r--r--   0 stephantulkens   (501) staff       (20)     1082 2022-08-10 12:06:48.000000 reach-4.0.2/LICENSE
--rw-r--r--   0 stephantulkens   (501) staff       (20)     6933 2023-05-03 10:42:06.094700 reach-4.0.2/PKG-INFO
--rw-r--r--   0 stephantulkens   (501) staff       (20)     5992 2023-05-03 10:41:54.000000 reach-4.0.2/README.md
--rw-r--r--   0 stephantulkens   (501) staff       (20)      178 2023-04-30 19:03:35.000000 reach-4.0.2/pyproject.toml
-drwxr-xr-x   0 stephantulkens   (501) staff       (20)        0 2023-05-03 10:42:06.090926 reach-4.0.2/reach/
--rw-r--r--   0 stephantulkens   (501) staff       (20)      290 2023-05-03 10:41:54.000000 reach-4.0.2/reach/__init__.py
--rw-r--r--   0 stephantulkens   (501) staff       (20)     2656 2023-04-30 19:01:37.000000 reach-4.0.2/reach/autoreach.py
--rw-r--r--   0 stephantulkens   (501) staff       (20)    34095 2023-05-03 08:16:28.000000 reach-4.0.2/reach/reach.py
-drwxr-xr-x   0 stephantulkens   (501) staff       (20)        0 2023-05-03 10:42:06.092969 reach-4.0.2/reach.egg-info/
--rw-r--r--   0 stephantulkens   (501) staff       (20)     6933 2023-05-03 10:42:06.000000 reach-4.0.2/reach.egg-info/PKG-INFO
--rw-r--r--   0 stephantulkens   (501) staff       (20)      365 2023-05-03 10:42:06.000000 reach-4.0.2/reach.egg-info/SOURCES.txt
--rw-r--r--   0 stephantulkens   (501) staff       (20)        1 2023-05-03 10:42:06.000000 reach-4.0.2/reach.egg-info/dependency_links.txt
--rw-r--r--   0 stephantulkens   (501) staff       (20)       33 2023-05-03 10:42:06.000000 reach-4.0.2/reach.egg-info/requires.txt
--rw-r--r--   0 stephantulkens   (501) staff       (20)        6 2023-05-03 10:42:06.000000 reach-4.0.2/reach.egg-info/top_level.txt
--rw-r--r--   0 stephantulkens   (501) staff       (20)        1 2023-04-30 18:08:45.000000 reach-4.0.2/reach.egg-info/zip-safe
--rw-r--r--   0 stephantulkens   (501) staff       (20)       38 2023-05-03 10:42:06.094910 reach-4.0.2/setup.cfg
--rw-r--r--   0 stephantulkens   (501) staff       (20)     1318 2023-05-03 10:41:54.000000 reach-4.0.2/setup.py
-drwxr-xr-x   0 stephantulkens   (501) staff       (20)        0 2023-05-03 10:42:06.094375 reach-4.0.2/tests/
--rw-r--r--   0 stephantulkens   (501) staff       (20)     3292 2023-05-03 08:13:38.000000 reach-4.0.2/tests/test_auto.py
--rw-r--r--   0 stephantulkens   (501) staff       (20)     1860 2023-05-03 08:13:38.000000 reach-4.0.2/tests/test_init.py
--rw-r--r--   0 stephantulkens   (501) staff       (20)    10853 2023-05-03 08:12:10.000000 reach-4.0.2/tests/test_io.py
--rw-r--r--   0 stephantulkens   (501) staff       (20)     6300 2023-05-03 08:13:38.000000 reach-4.0.2/tests/test_similarity.py
--rw-r--r--   0 stephantulkens   (501) staff       (20)     5288 2023-05-03 08:13:38.000000 reach-4.0.2/tests/test_vectorize.py
+drwxr-xr-x   0 stephantulkens   (501) staff       (20)        0 2023-05-03 10:42:23.660777 reach-4.1.0/
+-rw-r--r--   0 stephantulkens   (501) staff       (20)     1082 2022-08-10 12:06:48.000000 reach-4.1.0/LICENSE
+-rw-r--r--   0 stephantulkens   (501) staff       (20)     7217 2023-05-03 10:42:23.660612 reach-4.1.0/PKG-INFO
+-rw-r--r--   0 stephantulkens   (501) staff       (20)     6277 2023-05-03 10:42:20.000000 reach-4.1.0/README.md
+-rw-r--r--   0 stephantulkens   (501) staff       (20)      178 2023-04-30 19:03:35.000000 reach-4.1.0/pyproject.toml
+drwxr-xr-x   0 stephantulkens   (501) staff       (20)        0 2023-05-03 10:42:23.657779 reach-4.1.0/reach/
+-rw-r--r--   0 stephantulkens   (501) staff       (20)      290 2023-05-03 10:42:20.000000 reach-4.1.0/reach/__init__.py
+-rw-r--r--   0 stephantulkens   (501) staff       (20)     2656 2023-04-30 19:01:37.000000 reach-4.1.0/reach/autoreach.py
+-rw-r--r--   0 stephantulkens   (501) staff       (20)    34095 2023-05-03 08:16:28.000000 reach-4.1.0/reach/reach.py
+drwxr-xr-x   0 stephantulkens   (501) staff       (20)        0 2023-05-03 10:42:23.658990 reach-4.1.0/reach.egg-info/
+-rw-r--r--   0 stephantulkens   (501) staff       (20)     7217 2023-05-03 10:42:23.000000 reach-4.1.0/reach.egg-info/PKG-INFO
+-rw-r--r--   0 stephantulkens   (501) staff       (20)      365 2023-05-03 10:42:23.000000 reach-4.1.0/reach.egg-info/SOURCES.txt
+-rw-r--r--   0 stephantulkens   (501) staff       (20)        1 2023-05-03 10:42:23.000000 reach-4.1.0/reach.egg-info/dependency_links.txt
+-rw-r--r--   0 stephantulkens   (501) staff       (20)       33 2023-05-03 10:42:23.000000 reach-4.1.0/reach.egg-info/requires.txt
+-rw-r--r--   0 stephantulkens   (501) staff       (20)        6 2023-05-03 10:42:23.000000 reach-4.1.0/reach.egg-info/top_level.txt
+-rw-r--r--   0 stephantulkens   (501) staff       (20)        1 2023-04-30 18:08:45.000000 reach-4.1.0/reach.egg-info/zip-safe
+-rw-r--r--   0 stephantulkens   (501) staff       (20)       38 2023-05-03 10:42:23.660819 reach-4.1.0/setup.cfg
+-rw-r--r--   0 stephantulkens   (501) staff       (20)     1310 2023-05-03 10:42:20.000000 reach-4.1.0/setup.py
+drwxr-xr-x   0 stephantulkens   (501) staff       (20)        0 2023-05-03 10:42:23.660250 reach-4.1.0/tests/
+-rw-r--r--   0 stephantulkens   (501) staff       (20)     3292 2023-05-03 08:13:38.000000 reach-4.1.0/tests/test_auto.py
+-rw-r--r--   0 stephantulkens   (501) staff       (20)     1860 2023-05-03 08:13:38.000000 reach-4.1.0/tests/test_init.py
+-rw-r--r--   0 stephantulkens   (501) staff       (20)    10853 2023-05-03 08:12:10.000000 reach-4.1.0/tests/test_io.py
+-rw-r--r--   0 stephantulkens   (501) staff       (20)     6300 2023-05-03 08:13:38.000000 reach-4.1.0/tests/test_similarity.py
+-rw-r--r--   0 stephantulkens   (501) staff       (20)     5288 2023-05-03 08:13:38.000000 reach-4.1.0/tests/test_vectorize.py
```

### Comparing `reach-4.0.2/LICENSE` & `reach-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reach-4.0.2/PKG-INFO` & `reach-4.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reach
-Version: 4.0.2
+Version: 4.1.0
 Summary: A light-weight package for working with pre-trained word embeddings
 Home-page: https://github.com/stephantul/reach
 Author: Stéphan Tulkens
 Author-email: stephantul@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/stephantul/reach
 Project-URL: Issue Tracker, https://github.com/stephantul/reach/issues
@@ -90,27 +90,33 @@
 
 # vectorized representation.
 vectorized = r.vectorize(sentence)
 
 # can remove OOV words automatically.
 vectorized = r.vectorize(sentence, remove_oov=True)
 
+# Can mean pool out of the box.
+mean = r.mean_pool(sentence)
+# Automatically take care of incorrect sentences
+# these are set to the vector of the UNK word, or a vector of zeros.
+corpus_mean = r.mean_pool_corpus([sentence, sentence, ["not_a_word"]], remove_oov=True, safeguard=False)
+
 # vectorize corpus.
 transformed = r.transform(corpus)
 
 # Get nearest words to arbitrary vector
 nearest = r.nearest_neighbor(np.random.randn(1, 300))
 
 # Get every word within a certain threshold
 thresholded = r.threshold("cat", threshold=.0)
 ```
 
 ## Loading and saving
 
-`reach` has many options for saving and loading files, including custom separators, custom number of dimensions, loading a custom wordlist, custom number of words, and error recovery. One difference between `gensim` and `reach` is that `reach` loads both GloVe-style .vec files and regular word2vec files. Unlike `gensim`, `reach` does not support loading binary files. 
+`reach` has many options for saving and loading files, including custom separators, custom number of dimensions, loading a custom wordlist, custom number of words, and error recovery. One difference between `gensim` and `reach` is that `reach` loads both GloVe-style .vec files and regular word2vec files. Unlike `gensim`, `reach` does not support loading binary files.
 
 ### benchmark
 
 On my machine (a 2022 M1 macbook pro), we get the following times for [`COW BIG`](https://github.com/clips/dutchembeddings), a file containing about 3 million rows and 320 dimensions.
 
 | System | Time (7 loops)    |
 |--------|-------------------|
```

### Comparing `reach-4.0.2/README.md` & `reach-4.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -67,27 +67,33 @@
 
 # vectorized representation.
 vectorized = r.vectorize(sentence)
 
 # can remove OOV words automatically.
 vectorized = r.vectorize(sentence, remove_oov=True)
 
+# Can mean pool out of the box.
+mean = r.mean_pool(sentence)
+# Automatically take care of incorrect sentences
+# these are set to the vector of the UNK word, or a vector of zeros.
+corpus_mean = r.mean_pool_corpus([sentence, sentence, ["not_a_word"]], remove_oov=True, safeguard=False)
+
 # vectorize corpus.
 transformed = r.transform(corpus)
 
 # Get nearest words to arbitrary vector
 nearest = r.nearest_neighbor(np.random.randn(1, 300))
 
 # Get every word within a certain threshold
 thresholded = r.threshold("cat", threshold=.0)
 ```
 
 ## Loading and saving
 
-`reach` has many options for saving and loading files, including custom separators, custom number of dimensions, loading a custom wordlist, custom number of words, and error recovery. One difference between `gensim` and `reach` is that `reach` loads both GloVe-style .vec files and regular word2vec files. Unlike `gensim`, `reach` does not support loading binary files. 
+`reach` has many options for saving and loading files, including custom separators, custom number of dimensions, loading a custom wordlist, custom number of words, and error recovery. One difference between `gensim` and `reach` is that `reach` loads both GloVe-style .vec files and regular word2vec files. Unlike `gensim`, `reach` does not support loading binary files.
 
 ### benchmark
 
 On my machine (a 2022 M1 macbook pro), we get the following times for [`COW BIG`](https://github.com/clips/dutchembeddings), a file containing about 3 million rows and 320 dimensions.
 
 | System | Time (7 loops)    |
 |--------|-------------------|
@@ -156,8 +162,8 @@
 
 # License
 
 MIT
 
 # Author
 
-Stéphan Tulkens
+Stéphan Tulkens
```

### Comparing `reach-4.0.2/reach/autoreach.py` & `reach-4.1.0/reach/autoreach.py`

 * *Files identical despite different names*

### Comparing `reach-4.0.2/reach/reach.py` & `reach-4.1.0/reach/reach.py`

 * *Files identical despite different names*

### Comparing `reach-4.0.2/reach.egg-info/PKG-INFO` & `reach-4.1.0/reach.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reach
-Version: 4.0.2
+Version: 4.1.0
 Summary: A light-weight package for working with pre-trained word embeddings
 Home-page: https://github.com/stephantul/reach
 Author: Stéphan Tulkens
 Author-email: stephantul@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/stephantul/reach
 Project-URL: Issue Tracker, https://github.com/stephantul/reach/issues
@@ -90,27 +90,33 @@
 
 # vectorized representation.
 vectorized = r.vectorize(sentence)
 
 # can remove OOV words automatically.
 vectorized = r.vectorize(sentence, remove_oov=True)
 
+# Can mean pool out of the box.
+mean = r.mean_pool(sentence)
+# Automatically take care of incorrect sentences
+# these are set to the vector of the UNK word, or a vector of zeros.
+corpus_mean = r.mean_pool_corpus([sentence, sentence, ["not_a_word"]], remove_oov=True, safeguard=False)
+
 # vectorize corpus.
 transformed = r.transform(corpus)
 
 # Get nearest words to arbitrary vector
 nearest = r.nearest_neighbor(np.random.randn(1, 300))
 
 # Get every word within a certain threshold
 thresholded = r.threshold("cat", threshold=.0)
 ```
 
 ## Loading and saving
 
-`reach` has many options for saving and loading files, including custom separators, custom number of dimensions, loading a custom wordlist, custom number of words, and error recovery. One difference between `gensim` and `reach` is that `reach` loads both GloVe-style .vec files and regular word2vec files. Unlike `gensim`, `reach` does not support loading binary files. 
+`reach` has many options for saving and loading files, including custom separators, custom number of dimensions, loading a custom wordlist, custom number of words, and error recovery. One difference between `gensim` and `reach` is that `reach` loads both GloVe-style .vec files and regular word2vec files. Unlike `gensim`, `reach` does not support loading binary files.
 
 ### benchmark
 
 On my machine (a 2022 M1 macbook pro), we get the following times for [`COW BIG`](https://github.com/clips/dutchembeddings), a file containing about 3 million rows and 320 dimensions.
 
 | System | Time (7 loops)    |
 |--------|-------------------|
```

### Comparing `reach-4.0.2/setup.py` & `reach-4.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 """Setup file."""
 from pathlib import Path
-from setuptools import setup, find_packages
 
+from setuptools import find_packages, setup
 
 setup(
     name="reach",
-    version="4.0.2",  # noqa
+    version="4.1.0",
     description="A light-weight package for working with pre-trained word embeddings",
     author="Stéphan Tulkens",
     author_email="stephantul@gmail.com",
     url="https://github.com/stephantul/reach",
     license="MIT",
     packages=find_packages(include=["reach"]),
     install_requires=["numpy", "tqdm"],
```

### Comparing `reach-4.0.2/tests/test_auto.py` & `reach-4.1.0/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `reach-4.0.2/tests/test_init.py` & `reach-4.1.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `reach-4.0.2/tests/test_io.py` & `reach-4.1.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `reach-4.0.2/tests/test_similarity.py` & `reach-4.1.0/tests/test_similarity.py`

 * *Files identical despite different names*

### Comparing `reach-4.0.2/tests/test_vectorize.py` & `reach-4.1.0/tests/test_vectorize.py`

 * *Files identical despite different names*

