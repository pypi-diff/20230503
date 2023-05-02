# Comparing `tmp/dreamai_pdf-0.0.2.tar.gz` & `tmp/dreamai_pdf-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamai_pdf-0.0.2.tar", last modified: Fri Apr 28 14:57:17 2023, max compression
+gzip compressed data, was "dreamai_pdf-0.0.4.tar", last modified: Tue May  2 22:38:06 2023, max compression
```

## Comparing `dreamai_pdf-0.0.2.tar` & `dreamai_pdf-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-04-28 14:57:17.977030 dreamai_pdf-0.0.2/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.2/LICENSE
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.2/MANIFEST.in
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      927 2023-04-28 14:57:17.977030 dreamai_pdf-0.0.2/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      138 2023-04-28 14:57:11.000000 dreamai_pdf-0.0.2/README.md
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-04-28 14:57:17.973030 dreamai_pdf-0.0.2/dreamai_pdf/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-04-28 14:57:05.000000 dreamai_pdf-0.0.2/dreamai_pdf/__init__.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2850 2023-04-28 14:57:05.000000 dreamai_pdf-0.0.2/dreamai_pdf/_modidx.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     8233 2023-04-28 14:57:05.000000 dreamai_pdf-0.0.2/dreamai_pdf/core.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      569 2023-04-28 14:02:18.000000 dreamai_pdf-0.0.2/dreamai_pdf/imports.py
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-04-28 14:57:17.973030 dreamai_pdf-0.0.2/dreamai_pdf.egg-info/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      927 2023-04-28 14:57:17.000000 dreamai_pdf-0.0.2/dreamai_pdf.egg-info/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      387 2023-04-28 14:57:17.000000 dreamai_pdf-0.0.2/dreamai_pdf.egg-info/SOURCES.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-04-28 14:57:17.000000 dreamai_pdf-0.0.2/dreamai_pdf.egg-info/dependency_links.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       44 2023-04-28 14:57:17.000000 dreamai_pdf-0.0.2/dreamai_pdf.egg-info/entry_points.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-04-28 14:00:17.000000 dreamai_pdf-0.0.2/dreamai_pdf.egg-info/not-zip-safe
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     1053 2023-04-28 14:57:17.000000 dreamai_pdf-0.0.2/dreamai_pdf.egg-info/requires.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       12 2023-04-28 14:57:17.000000 dreamai_pdf-0.0.2/dreamai_pdf.egg-info/top_level.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     1738 2023-04-28 14:57:07.000000 dreamai_pdf-0.0.2/settings.ini
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-04-28 14:57:17.977030 dreamai_pdf-0.0.2/setup.cfg
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.2/setup.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 22:38:06.145317 dreamai_pdf-0.0.4/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.4/LICENSE
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.4/MANIFEST.in
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      927 2023-05-02 22:38:06.145317 dreamai_pdf-0.0.4/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      138 2023-05-02 22:37:14.000000 dreamai_pdf-0.0.4/README.md
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 22:38:06.145317 dreamai_pdf-0.0.4/dreamai_pdf/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-02 22:36:37.000000 dreamai_pdf-0.0.4/dreamai_pdf/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     5299 2023-05-02 22:36:37.000000 dreamai_pdf-0.0.4/dreamai_pdf/_modidx.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     3434 2023-05-02 22:36:37.000000 dreamai_pdf-0.0.4/dreamai_pdf/core.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      494 2023-05-02 20:33:15.000000 dreamai_pdf-0.0.4/dreamai_pdf/imports.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     9207 2023-05-02 22:36:37.000000 dreamai_pdf-0.0.4/dreamai_pdf/parse.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2101 2023-05-02 22:36:37.000000 dreamai_pdf-0.0.4/dreamai_pdf/segment.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 22:38:06.145317 dreamai_pdf-0.0.4/dreamai_pdf.egg-info/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      927 2023-05-02 22:38:06.000000 dreamai_pdf-0.0.4/dreamai_pdf.egg-info/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      431 2023-05-02 22:38:06.000000 dreamai_pdf-0.0.4/dreamai_pdf.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-02 22:38:06.000000 dreamai_pdf-0.0.4/dreamai_pdf.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       44 2023-05-02 22:38:06.000000 dreamai_pdf-0.0.4/dreamai_pdf.egg-info/entry_points.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-04-28 14:00:17.000000 dreamai_pdf-0.0.4/dreamai_pdf.egg-info/not-zip-safe
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     1053 2023-05-02 22:38:06.000000 dreamai_pdf-0.0.4/dreamai_pdf.egg-info/requires.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       12 2023-05-02 22:38:06.000000 dreamai_pdf-0.0.4/dreamai_pdf.egg-info/top_level.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     1738 2023-05-02 22:33:52.000000 dreamai_pdf-0.0.4/settings.ini
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-02 22:38:06.145317 dreamai_pdf-0.0.4/setup.cfg
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.4/setup.py
```

### Comparing `dreamai_pdf-0.0.2/LICENSE` & `dreamai_pdf-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.2/PKG-INFO` & `dreamai_pdf-0.0.4/dreamai_pdf.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: dreamai_pdf
-Version: 0.0.2
-Summary: Library based on DreamAI for parsing PDFs
+Name: dreamai-pdf
+Version: 0.0.4
+Summary: Library based on dreamai for parsing PDFs
 Home-page: https://github.com/HamzaFarhan/dreamai_pdf
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dreamai_pdf-0.0.2/dreamai_pdf.egg-info/PKG-INFO` & `dreamai_pdf-0.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: dreamai-pdf
-Version: 0.0.2
-Summary: Library based on DreamAI for parsing PDFs
+Name: dreamai_pdf
+Version: 0.0.4
+Summary: Library based on dreamai for parsing PDFs
 Home-page: https://github.com/HamzaFarhan/dreamai_pdf
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dreamai_pdf-0.0.2/dreamai_pdf.egg-info/requires.txt` & `dreamai_pdf-0.0.4/dreamai_pdf.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.2/settings.ini` & `dreamai_pdf-0.0.4/settings.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = dreamai_pdf
 lib_name = %(repo)s
-version = 0.0.2
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = dreamai_pdf
 nbs_path = nbs
 recursive = True
@@ -17,14 +17,14 @@
 doc_baseurl = /%(repo)s
 git_url = https://github.com/%(user)s/%(repo)s
 title = %(lib_name)s
 audience = Developers
 author = HamzaFarhan
 author_email = thehamza96@gmail.com
 copyright = 2023 onwards, %(author)s
-description = Library based on DreamAI for parsing PDFs
+description = Library based on dreamai for parsing PDFs
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = HamzaFarhan
 pip_requirements = aiohttp aiosignal astunparse async-timeout boto3 botocore bpemb certifi charset-normalizer cloudpickle cmake conllu contourpy cryptography cycler datasets deprecated dill docutils dreamai execnb faiss-cpu fastcore filelock flair fonttools frozenlist fsspec ftfy future gdown gensim ghapi huggingface-hub hyperopt importlib-metadata imutils janome jaraco-classes jeepney jmespath joblib keyring kiwisolver langdetect lit markdown-it-py matplotlib mdurl more-itertools mpld3 mpmath multidict multiprocess nbdev networkx numpy opencv-python pandas pdfminer-six pdfplumber pillow pkginfo pptree protobuf py4j pyarrow pygments pyparsing pysocks pytorch-revgrad pytz pyyaml readme-renderer regex requests requests-toolbelt responses rfc3986 rich s3transfer scikit-learn scipy secretstorage segtok sentencepiece smart-open sqlitedict sympy tabulate threadpoolctl tokenizers torch torchaudio torchvision tqdm transformer-smaller-training-vocab transformers triton twine txtai tzdata urllib3 wand watchdog wikipedia-api wrapt xxhash yarl yellowbrick zipp
```

### Comparing `dreamai_pdf-0.0.2/setup.py` & `dreamai_pdf-0.0.4/setup.py`

 * *Files identical despite different names*

