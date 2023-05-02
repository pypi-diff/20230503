# Comparing `tmp/dreamai_pdf-0.0.4.tar.gz` & `tmp/dreamai_pdf-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamai_pdf-0.0.4.tar", last modified: Tue May  2 22:38:06 2023, max compression
+gzip compressed data, was "dreamai_pdf-0.0.5.tar", last modified: Tue May  2 22:45:30 2023, max compression
```

## Comparing `dreamai_pdf-0.0.4.tar` & `dreamai_pdf-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 22:38:06.145317 dreamai_pdf-0.0.4/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.4/LICENSE
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.4/MANIFEST.in
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      927 2023-05-02 22:38:06.145317 dreamai_pdf-0.0.4/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      138 2023-05-02 22:37:14.000000 dreamai_pdf-0.0.4/README.md
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 22:38:06.145317 dreamai_pdf-0.0.4/dreamai_pdf/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-02 22:36:37.000000 dreamai_pdf-0.0.4/dreamai_pdf/__init__.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     5299 2023-05-02 22:36:37.000000 dreamai_pdf-0.0.4/dreamai_pdf/_modidx.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     3434 2023-05-02 22:36:37.000000 dreamai_pdf-0.0.4/dreamai_pdf/core.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      494 2023-05-02 20:33:15.000000 dreamai_pdf-0.0.4/dreamai_pdf/imports.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     9207 2023-05-02 22:36:37.000000 dreamai_pdf-0.0.4/dreamai_pdf/parse.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2101 2023-05-02 22:36:37.000000 dreamai_pdf-0.0.4/dreamai_pdf/segment.py
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 22:38:06.145317 dreamai_pdf-0.0.4/dreamai_pdf.egg-info/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      927 2023-05-02 22:38:06.000000 dreamai_pdf-0.0.4/dreamai_pdf.egg-info/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      431 2023-05-02 22:38:06.000000 dreamai_pdf-0.0.4/dreamai_pdf.egg-info/SOURCES.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-02 22:38:06.000000 dreamai_pdf-0.0.4/dreamai_pdf.egg-info/dependency_links.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       44 2023-05-02 22:38:06.000000 dreamai_pdf-0.0.4/dreamai_pdf.egg-info/entry_points.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-04-28 14:00:17.000000 dreamai_pdf-0.0.4/dreamai_pdf.egg-info/not-zip-safe
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     1053 2023-05-02 22:38:06.000000 dreamai_pdf-0.0.4/dreamai_pdf.egg-info/requires.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       12 2023-05-02 22:38:06.000000 dreamai_pdf-0.0.4/dreamai_pdf.egg-info/top_level.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     1738 2023-05-02 22:33:52.000000 dreamai_pdf-0.0.4/settings.ini
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-02 22:38:06.145317 dreamai_pdf-0.0.4/setup.cfg
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.4/setup.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 22:45:30.915928 dreamai_pdf-0.0.5/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.5/LICENSE
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.5/MANIFEST.in
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      927 2023-05-02 22:45:30.915928 dreamai_pdf-0.0.5/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      138 2023-05-02 22:37:14.000000 dreamai_pdf-0.0.5/README.md
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 22:45:30.915928 dreamai_pdf-0.0.5/dreamai_pdf/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-02 22:45:02.000000 dreamai_pdf-0.0.5/dreamai_pdf/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     5299 2023-05-02 22:44:50.000000 dreamai_pdf-0.0.5/dreamai_pdf/_modidx.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     3434 2023-05-02 22:44:50.000000 dreamai_pdf-0.0.5/dreamai_pdf/core.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      494 2023-05-02 20:33:15.000000 dreamai_pdf-0.0.5/dreamai_pdf/imports.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     9207 2023-05-02 22:44:50.000000 dreamai_pdf-0.0.5/dreamai_pdf/parse.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2101 2023-05-02 22:44:50.000000 dreamai_pdf-0.0.5/dreamai_pdf/segment.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 22:45:30.915928 dreamai_pdf-0.0.5/dreamai_pdf.egg-info/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      927 2023-05-02 22:45:30.000000 dreamai_pdf-0.0.5/dreamai_pdf.egg-info/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      431 2023-05-02 22:45:30.000000 dreamai_pdf-0.0.5/dreamai_pdf.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-02 22:45:30.000000 dreamai_pdf-0.0.5/dreamai_pdf.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       44 2023-05-02 22:45:30.000000 dreamai_pdf-0.0.5/dreamai_pdf.egg-info/entry_points.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-04-28 14:00:17.000000 dreamai_pdf-0.0.5/dreamai_pdf.egg-info/not-zip-safe
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     1683 2023-05-02 22:45:30.000000 dreamai_pdf-0.0.5/dreamai_pdf.egg-info/requires.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       12 2023-05-02 22:45:30.000000 dreamai_pdf-0.0.5/dreamai_pdf.egg-info/top_level.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2368 2023-05-02 22:45:02.000000 dreamai_pdf-0.0.5/settings.ini
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-02 22:45:30.915928 dreamai_pdf-0.0.5/setup.cfg
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.5/setup.py
```

### Comparing `dreamai_pdf-0.0.4/LICENSE` & `dreamai_pdf-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.4/PKG-INFO` & `dreamai_pdf-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai_pdf
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library based on dreamai for parsing PDFs
 Home-page: https://github.com/HamzaFarhan/dreamai_pdf
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai_pdf-0.0.4/dreamai_pdf/_modidx.py` & `dreamai_pdf-0.0.5/dreamai_pdf/_modidx.py`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.4/dreamai_pdf/core.py` & `dreamai_pdf-0.0.5/dreamai_pdf/core.py`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.4/dreamai_pdf/parse.py` & `dreamai_pdf-0.0.5/dreamai_pdf/parse.py`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.4/dreamai_pdf/segment.py` & `dreamai_pdf-0.0.5/dreamai_pdf/segment.py`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.4/dreamai_pdf.egg-info/PKG-INFO` & `dreamai_pdf-0.0.5/dreamai_pdf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai-pdf
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library based on dreamai for parsing PDFs
 Home-page: https://github.com/HamzaFarhan/dreamai_pdf
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai_pdf-0.0.4/dreamai_pdf.egg-info/requires.txt` & `dreamai_pdf-0.0.5/dreamai_pdf.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,112 +1,172 @@
 aiohttp
 aiosignal
+arrow
 astunparse
 async-timeout
+blessed
+blis
 boto3
 botocore
 bpemb
+catalogue
 certifi
 charset-normalizer
+click
 cloudpickle
 cmake
+confection
 conllu
 contourpy
+croniter
 cryptography
 cycler
+cymem
 datasets
+dateutils
+deepdiff
 deprecated
 dill
+diskcache
 docutils
 dreamai
+dreamai-dl
+duckduckgo-search
 execnb
 faiss-cpu
+fastai
+fastapi
 fastcore
+fastdownload
+fastprogress
 filelock
 flair
 fonttools
 frozenlist
 fsspec
 ftfy
 future
 gdown
 gensim
 ghapi
+h11
+htmlmin
 huggingface-hub
 hyperopt
+imagehash
 importlib-metadata
 imutils
+inquirer
+ipywidgets
+itsdangerous
 janome
 jaraco-classes
 jeepney
 jmespath
 joblib
+jupyterlab-widgets
 keyring
 kiwisolver
+langcodes
 langdetect
+lightning
+lightning-cloud
+lightning-utilities
 lit
 markdown-it-py
 matplotlib
 mdurl
+missingno
 more-itertools
 mpld3
 mpmath
 multidict
+multimethod
 multiprocess
+murmurhash
 nbdev
 networkx
 numpy
 opencv-python
+ordered-set
 pandas
+pandas-profiling
+pathy
 pdfminer-six
 pdfplumber
+phik
 pillow
 pkginfo
 pptree
+preshed
 protobuf
 py4j
 pyarrow
+pydantic
 pygments
+pyjwt
 pyparsing
 pysocks
+python-editor
+python-multipart
+pytorch-lightning
 pytorch-revgrad
 pytz
+pywavelets
 pyyaml
+readchar
 readme-renderer
 regex
 requests
 requests-toolbelt
 responses
 rfc3986
 rich
 s3transfer
 scikit-learn
 scipy
+seaborn
 secretstorage
 segtok
 sentencepiece
 smart-open
+spacy
+spacy-legacy
+spacy-loggers
 sqlitedict
+srsly
+starlette
+starsessions
 sympy
 tabulate
+tangled-up-in-unicode
+thinc
 threadpoolctl
+timm
 tokenizers
 torch
 torchaudio
+torchmetrics
 torchvision
 tqdm
 transformer-smaller-training-vocab
 transformers
 triton
 twine
 txtai
+typer
 tzdata
 urllib3
+uvicorn
+visions
 wand
+wasabi
 watchdog
+websockets
+widgetsnbextension
 wikipedia-api
 wrapt
 xxhash
 yarl
 yellowbrick
 zipp
```

### Comparing `dreamai_pdf-0.0.4/settings.ini` & `dreamai_pdf-0.0.5/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = dreamai_pdf
 lib_name = %(repo)s
-version = 0.0.4
+version = 0.0.5
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = dreamai_pdf
 nbs_path = nbs
 recursive = True
@@ -22,9 +22,9 @@
 author_email = thehamza96@gmail.com
 copyright = 2023 onwards, %(author)s
 description = Library based on dreamai for parsing PDFs
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = HamzaFarhan
-pip_requirements = aiohttp aiosignal astunparse async-timeout boto3 botocore bpemb certifi charset-normalizer cloudpickle cmake conllu contourpy cryptography cycler datasets deprecated dill docutils dreamai execnb faiss-cpu fastcore filelock flair fonttools frozenlist fsspec ftfy future gdown gensim ghapi huggingface-hub hyperopt importlib-metadata imutils janome jaraco-classes jeepney jmespath joblib keyring kiwisolver langdetect lit markdown-it-py matplotlib mdurl more-itertools mpld3 mpmath multidict multiprocess nbdev networkx numpy opencv-python pandas pdfminer-six pdfplumber pillow pkginfo pptree protobuf py4j pyarrow pygments pyparsing pysocks pytorch-revgrad pytz pyyaml readme-renderer regex requests requests-toolbelt responses rfc3986 rich s3transfer scikit-learn scipy secretstorage segtok sentencepiece smart-open sqlitedict sympy tabulate threadpoolctl tokenizers torch torchaudio torchvision tqdm transformer-smaller-training-vocab transformers triton twine txtai tzdata urllib3 wand watchdog wikipedia-api wrapt xxhash yarl yellowbrick zipp
+pip_requirements = aiohttp aiosignal arrow astunparse async-timeout blessed blis boto3 botocore bpemb catalogue certifi charset-normalizer click cloudpickle cmake confection conllu contourpy croniter cryptography cycler cymem datasets dateutils deepdiff deprecated dill diskcache docutils dreamai dreamai-dl duckduckgo-search execnb faiss-cpu fastai fastapi fastcore fastdownload fastprogress filelock flair fonttools frozenlist fsspec ftfy future gdown gensim ghapi h11 htmlmin huggingface-hub hyperopt imagehash importlib-metadata imutils inquirer ipywidgets itsdangerous janome jaraco-classes jeepney jmespath joblib jupyterlab-widgets keyring kiwisolver langcodes langdetect lightning lightning-cloud lightning-utilities lit markdown-it-py matplotlib mdurl missingno more-itertools mpld3 mpmath multidict multimethod multiprocess murmurhash nbdev networkx numpy opencv-python ordered-set pandas pandas-profiling pathy pdfminer-six pdfplumber phik pillow pkginfo pptree preshed protobuf py4j pyarrow pydantic pygments pyjwt pyparsing pysocks python-editor python-multipart pytorch-lightning pytorch-revgrad pytz pywavelets pyyaml readchar readme-renderer regex requests requests-toolbelt responses rfc3986 rich s3transfer scikit-learn scipy seaborn secretstorage segtok sentencepiece smart-open spacy spacy-legacy spacy-loggers sqlitedict srsly starlette starsessions sympy tabulate tangled-up-in-unicode thinc threadpoolctl timm tokenizers torch torchaudio torchmetrics torchvision tqdm transformer-smaller-training-vocab transformers triton twine txtai typer tzdata urllib3 uvicorn visions wand wasabi watchdog websockets widgetsnbextension wikipedia-api wrapt xxhash yarl yellowbrick zipp
```

### Comparing `dreamai_pdf-0.0.4/setup.py` & `dreamai_pdf-0.0.5/setup.py`

 * *Files identical despite different names*

