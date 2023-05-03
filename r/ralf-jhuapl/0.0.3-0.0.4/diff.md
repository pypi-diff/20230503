# Comparing `tmp/ralf-jhuapl-0.0.3.tar.gz` & `tmp/ralf-jhuapl-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralf-jhuapl-0.0.3.tar", last modified: Tue May  2 13:25:49 2023, max compression
+gzip compressed data, was "ralf-jhuapl-0.0.4.tar", last modified: Wed May  3 02:54:28 2023, max compression
```

## Comparing `ralf-jhuapl-0.0.3.tar` & `ralf-jhuapl-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0      705 2023-05-01 22:24:53.483639 ralf-jhuapl-0.0.3/.readthedocs.yaml
--rw-r--r--   0        0        0     1955 2023-05-01 23:06:16.306652 ralf-jhuapl-0.0.3/README.md
--rw-r--r--   0        0        0   162364 2023-05-01 22:24:53.484177 ralf-jhuapl-0.0.3/assets/ralf_logo_v1.png
--rw-r--r--   0        0        0   186140 2023-05-01 22:24:53.484562 ralf-jhuapl-0.0.3/assets/ralf_logo_v2.png
--rwxr-xr-x   0        0        0      855 2023-05-01 22:24:53.484713 ralf-jhuapl-0.0.3/demos/classifier_demo.py
--rwxr-xr-x   0        0        0     1635 2023-05-01 22:24:53.484807 ralf-jhuapl-0.0.3/demos/dispatcher_demo.py
--rw-r--r--   0        0        0      126 2023-05-01 22:24:53.485011 ralf-jhuapl-0.0.3/demos/ralf_data/models.yml
--rw-r--r--   0        0        0      451 2023-05-01 22:24:53.485156 ralf-jhuapl-0.0.3/demos/ralf_data/prompts.yml
--rwxr-xr-x   0        0        0     1738 2023-05-01 22:24:53.485314 ralf-jhuapl-0.0.3/demos/simple_chat.py
--rw-r--r--   0        0        0      634 2023-05-01 22:24:53.485531 ralf-jhuapl-0.0.3/docs/Makefile
--rw-r--r--   0        0        0       49 2023-05-01 22:24:53.485776 ralf-jhuapl-0.0.3/docs/api/modules.rst
--rw-r--r--   0        0        0      522 2023-05-01 22:24:53.485919 ralf-jhuapl-0.0.3/docs/api/ralf.rst
--rw-r--r--   0        0        0     2177 2023-05-01 22:24:53.486030 ralf-jhuapl-0.0.3/docs/conf.py
--rw-r--r--   0        0        0     2531 2023-05-01 22:24:53.486115 ralf-jhuapl-0.0.3/docs/index.rst
--rw-r--r--   0        0        0     1226 2023-05-01 22:24:53.486222 ralf-jhuapl-0.0.3/docs/introduction/quickstart.rst
--rw-r--r--   0        0        0      800 2023-05-01 22:24:53.486292 ralf-jhuapl-0.0.3/docs/make.bat
--rw-r--r--   0        0        0       49 2023-05-01 22:24:53.486355 ralf-jhuapl-0.0.3/docs/modules.rst
--rw-r--r--   0        0        0      545 2023-05-01 22:24:53.486421 ralf-jhuapl-0.0.3/docs/ralf.rst
--rw-r--r--   0        0        0     1285 2023-05-01 22:24:53.486534 ralf-jhuapl-0.0.3/docs/tutorials/actions.rst
--rw-r--r--   0        0        0     4654 2023-05-01 22:24:53.486634 ralf-jhuapl-0.0.3/docs/tutorials/classification.ipynb
--rw-r--r--   0        0        0    14497 2023-05-01 22:24:53.486764 ralf-jhuapl-0.0.3/docs/tutorials/executing_actions.ipynb
--rw-r--r--   0        0        0      838 2023-05-02 13:20:27.205929 ralf-jhuapl-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-02 13:25:34.132307 ralf-jhuapl-0.0.3/ralf/__init__.py
--rw-r--r--   0        0        0     6979 2023-05-01 22:24:53.487064 ralf-jhuapl-0.0.3/ralf/classifier.py
--rw-r--r--   0        0        0    11817 2023-05-01 22:24:53.487170 ralf-jhuapl-0.0.3/ralf/dispatcher.py
--rw-r--r--   0        0        0     4570 2023-05-01 22:24:53.487263 ralf-jhuapl-0.0.3/ralf/utils.py
--rw-r--r--   0        0        0       56 2023-05-01 22:24:53.487331 ralf-jhuapl-0.0.3/requirements.txt
--rw-r--r--   0        0        0     2577 1970-01-01 00:00:00.000000 ralf-jhuapl-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     3077 2023-05-02 13:36:20.805453 ralf-jhuapl-0.0.4/.gitignore
+-rw-r--r--   0        0        0      705 2023-05-01 22:24:53.483639 ralf-jhuapl-0.0.4/.readthedocs.yaml
+-rw-r--r--   0        0        0     1112 2023-05-02 23:47:05.913100 ralf-jhuapl-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3356 2023-05-03 02:51:51.521458 ralf-jhuapl-0.0.4/README.md
+-rw-r--r--   0        0        0   162364 2023-05-01 22:24:53.484177 ralf-jhuapl-0.0.4/assets/ralf_logo_v1.png
+-rw-r--r--   0        0        0   186140 2023-05-01 22:24:53.484562 ralf-jhuapl-0.0.4/assets/ralf_logo_v2.png
+-rwxr-xr-x   0        0        0      855 2023-05-01 22:24:53.484713 ralf-jhuapl-0.0.4/demos/classifier_demo.py
+-rwxr-xr-x   0        0        0     1635 2023-05-01 22:24:53.484807 ralf-jhuapl-0.0.4/demos/dispatcher_demo.py
+-rw-r--r--   0        0        0      126 2023-05-01 22:24:53.485011 ralf-jhuapl-0.0.4/demos/ralf_data/models.yml
+-rw-r--r--   0        0        0      451 2023-05-01 22:24:53.485156 ralf-jhuapl-0.0.4/demos/ralf_data/prompts.yml
+-rwxr-xr-x   0        0        0     1738 2023-05-01 22:24:53.485314 ralf-jhuapl-0.0.4/demos/simple_chat.py
+-rw-r--r--   0        0        0      634 2023-05-01 22:24:53.485531 ralf-jhuapl-0.0.4/docs/Makefile
+-rw-r--r--   0        0        0       49 2023-05-01 22:24:53.485776 ralf-jhuapl-0.0.4/docs/api/modules.rst
+-rw-r--r--   0        0        0      522 2023-05-01 22:24:53.485919 ralf-jhuapl-0.0.4/docs/api/ralf.rst
+-rw-r--r--   0        0        0     2177 2023-05-01 22:24:53.486030 ralf-jhuapl-0.0.4/docs/conf.py
+-rw-r--r--   0        0        0     2531 2023-05-01 22:24:53.486115 ralf-jhuapl-0.0.4/docs/index.rst
+-rw-r--r--   0        0        0     1605 2023-05-03 02:40:43.168068 ralf-jhuapl-0.0.4/docs/introduction/quickstart.rst
+-rw-r--r--   0        0        0      800 2023-05-01 22:24:53.486292 ralf-jhuapl-0.0.4/docs/make.bat
+-rw-r--r--   0        0        0       49 2023-05-01 22:24:53.486355 ralf-jhuapl-0.0.4/docs/modules.rst
+-rw-r--r--   0        0        0      545 2023-05-01 22:24:53.486421 ralf-jhuapl-0.0.4/docs/ralf.rst
+-rw-r--r--   0        0        0     1285 2023-05-01 22:24:53.486534 ralf-jhuapl-0.0.4/docs/tutorials/actions.rst
+-rw-r--r--   0        0        0     4654 2023-05-01 22:24:53.486634 ralf-jhuapl-0.0.4/docs/tutorials/classification.ipynb
+-rw-r--r--   0        0        0    14497 2023-05-01 22:24:53.486764 ralf-jhuapl-0.0.4/docs/tutorials/executing_actions.ipynb
+-rw-r--r--   0        0        0      838 2023-05-02 13:20:27.205929 ralf-jhuapl-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-03 02:53:05.180192 ralf-jhuapl-0.0.4/ralf/__init__.py
+-rw-r--r--   0        0        0     6979 2023-05-01 22:24:53.487064 ralf-jhuapl-0.0.4/ralf/classifier.py
+-rw-r--r--   0        0        0    11817 2023-05-01 22:24:53.487170 ralf-jhuapl-0.0.4/ralf/dispatcher.py
+-rw-r--r--   0        0        0     4570 2023-05-01 22:24:53.487263 ralf-jhuapl-0.0.4/ralf/utils.py
+-rw-r--r--   0        0        0       56 2023-05-01 22:24:53.487331 ralf-jhuapl-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     3978 1970-01-01 00:00:00.000000 ralf-jhuapl-0.0.4/PKG-INFO
```

### Comparing `ralf-jhuapl-0.0.3/.readthedocs.yaml` & `ralf-jhuapl-0.0.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.3/assets/ralf_logo_v1.png` & `ralf-jhuapl-0.0.4/assets/ralf_logo_v1.png`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.3/assets/ralf_logo_v2.png` & `ralf-jhuapl-0.0.4/assets/ralf_logo_v2.png`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.3/demos/classifier_demo.py` & `ralf-jhuapl-0.0.4/demos/classifier_demo.py`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.3/demos/dispatcher_demo.py` & `ralf-jhuapl-0.0.4/demos/dispatcher_demo.py`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.3/demos/simple_chat.py` & `ralf-jhuapl-0.0.4/demos/simple_chat.py`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.3/docs/Makefile` & `ralf-jhuapl-0.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.3/docs/api/ralf.rst` & `ralf-jhuapl-0.0.4/docs/api/ralf.rst`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.3/docs/conf.py` & `ralf-jhuapl-0.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.3/docs/index.rst` & `ralf-jhuapl-0.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.3/docs/introduction/quickstart.rst` & `ralf-jhuapl-0.0.4/docs/introduction/quickstart.rst`

 * *Files 22% similar despite different names*

```diff
@@ -2,20 +2,36 @@
 ================
 This quickstart guide is intended to get you up and running with **ralf** within
 a few minutes.
 
 
 Installation
 ------------
-First, clone the Gitlab project::
+We recommend creating a Conda environment before installing the package::
+
+    conda create -n ralf python=3.10
+    conda activate ralf
+
+Install from PyPI
++++++++++++++++++
+
+You may install **ralf** from PyPI using ``pip``::
+
+    pip install ralf-jhuapl
+
+Install from Source
++++++++++++++++++++
+
+Alternatively, you can build the package from source. First, clone the Github repository::
 
     git clone https://gitlab.jhuapl.edu/ralf/ralf
 
 Next, install the requirements using ``pip``::
-   
+    
+    cd ralf
     pip install -r requirements.txt
 
 Then, build the package using ``flit`` and install it using ``pip``::
 
     flit build
     pip install .
 
@@ -34,14 +50,15 @@
     source ~/.bashrc
 
 Running the Demos
 -----------------
 
 To test if installation was successful, try running the demo scripts::
 
+    cd demos
     python demos/dispatcher_demo.py
     python demos/classifier_demo.py
 
 If the scripts execute successfully, you are good to go! You may want to look 
 through the demo scripts to learn about some of the things **ralf** can do, or 
 follow the more detailed tutorials.
```

### Comparing `ralf-jhuapl-0.0.3/docs/make.bat` & `ralf-jhuapl-0.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.3/docs/ralf.rst` & `ralf-jhuapl-0.0.4/docs/ralf.rst`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.3/docs/tutorials/actions.rst` & `ralf-jhuapl-0.0.4/docs/tutorials/actions.rst`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.3/docs/tutorials/classification.ipynb` & `ralf-jhuapl-0.0.4/docs/tutorials/classification.ipynb`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.3/docs/tutorials/executing_actions.ipynb` & `ralf-jhuapl-0.0.4/docs/tutorials/executing_actions.ipynb`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.3/pyproject.toml` & `ralf-jhuapl-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.3/ralf/classifier.py` & `ralf-jhuapl-0.0.4/ralf/classifier.py`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.3/ralf/dispatcher.py` & `ralf-jhuapl-0.0.4/ralf/dispatcher.py`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.3/ralf/utils.py` & `ralf-jhuapl-0.0.4/ralf/utils.py`

 * *Files identical despite different names*

### Comparing `ralf-jhuapl-0.0.3/PKG-INFO` & `ralf-jhuapl-0.0.4/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,16 @@
-Metadata-Version: 2.1
-Name: ralf-jhuapl
-Version: 0.0.3
-Summary: A lightweight library to support the development of applications using LLMs.
-Author-email: JHUAPL <ralf@jhuapl.edu>
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: openai
-Requires-Dist: numpy
-Requires-Dist: PyYAML
-Requires-Dist: sentence-transformers
-Project-URL: Documentation, https://ralf-test.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/jhuapl-fomo/ralf
-
 
 <div align="center">
-<img alt="ralf_logo" src="assets/ralf_logo_v1.png" width="200">
+<img alt="ralf_logo" src="https://github.com/jhuapl-fomo/ralf/raw/main/assets/ralf_logo_v1.png" width="200">
 
 # ralf
 
 [![Documentation](https://readthedocs.org/projects/ralf-jhuapl/badge/?version=latest)](https://ralf-jhuapl.readthedocs.io/en/latest/)
+[![PyPI version](https://badge.fury.io/py/ralf-jhuapl.svg)](https://badge.fury.io/py/ralf-jhuapl)
+[![License](https://img.shields.io/github/license/jhuapl-fomo/ralf.svg)](https://github.com/jhuapl-fomo/ralf/blob/main/LICENSE)
 </div>
 
 **ralf** is a Python library intended to assist developers in creating applications
 that involve calls to Large Language Models (LLMs). A core concept in **ralf** is the idea of *composability*,
 which allows chaining together LLM calls such that the output of one call can be
 used to form the prompt of another. **ralf** makes it easy to chain together both
 LLM-based and Python-based actions-- enabling developers to construct complex 
@@ -35,33 +20,69 @@
 Currently, the **ralf** base library offers generic functionality for action chaining
 (through the ``Dispatcher`` and ``Action`` classes) as well as text classificaiton
 (through the ``ZeroShotClassifier`` class). Check out the other projects within
 the RALF ecosystem for more specialized functionality, like dialogue management 
 and information extraction.
 
 
+## Quickstart Guide
+This quickstart guide is intended to get you up and running with **ralf** within
+a few minutes.
+### Installation
+
+We recommend creating a Conda environment before installing the package:
+
+    conda create -n ralf python=3.10
+    conda activate ralf
+
+#### Install from PyPI
 
-## Getting Started
+You may install **ralf** from PyPI using ``pip``:
 
-First, clone the Github repository:
+    pip install ralf-jhuapl
+
+#### Install from Source
+
+Alternatively, you can build the package from source. First, clone the Github repository:
 
     git clone https://gitlab.jhuapl.edu/ralf/ralf
 
 Next, install the requirements using ``pip``:
-   
+    
+    cd ralf
     pip install -r requirements.txt
 
 Then, build the package using ``flit`` and install it using ``pip``:
 
     flit build
     pip install .
 
 Or if you would like an editable installation, you can instead use:
 
     pip install -e .
 
+### OpenAI Configuration
+**ralf** currently relies on language models provided by OpenAI. 
+In order to access the models, you must store your OpenAI API key as an 
+environment variable by executing the following in bash:
+
+    echo "export OPENAI_API_KEY='yourkey'" >> ~/.bashrc
+    source ~/.bashrc
+
+### Running the Demos
+To test if installation was successful, try running the demo scripts:
+
+    cd demos
+    python dispatcher_demo.py
+    python classifier_demo.py
+
+If the scripts execute successfully, you are good to go! You may want to look 
+through the demo scripts to learn about some of the things **ralf** can do, or 
+follow the more detailed tutorials.
 ## Documentation & Tutorials
-The best way to get started with **ralf** is to follow the tutorials in the [TODO] [Documentation site](https://google.com). If you're eager to get started and want to skip the tutorials, you might instead consider checking out the `dispatcher_demo.py` and `classifier_demo.py` files in the `demo/` directory.
+The best way to get started with **ralf** is to follow the tutorials, which can be found in the [full documentation](https://ralf-jhuapl.readthedocs.io/en/latest/).
 
 ## License
-[**TODO**]
 
+This project is released under the [MIT License](https://github.com/jhuapl-fomo/ralf/blob/main/LICENSE).
+
+Copyright 2023 The Johns Hopkins University Applied Physics Laboratory
```

