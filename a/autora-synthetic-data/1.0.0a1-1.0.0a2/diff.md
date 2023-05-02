# Comparing `tmp/autora-synthetic-data-1.0.0a1.tar.gz` & `tmp/autora-synthetic-data-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-synthetic-data-1.0.0a1.tar", last modified: Fri Apr 28 22:10:21 2023, max compression
+gzip compressed data, was "autora-synthetic-data-1.0.0a2.tar", last modified: Tue May  2 22:29:46 2023, max compression
```

## Comparing `autora-synthetic-data-1.0.0a1.tar` & `autora-synthetic-data-1.0.0a2.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.768044 autora-synthetic-data-1.0.0a1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.760044 autora-synthetic-data-1.0.0a1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.764044 autora-synthetic-data-1.0.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/.github/workflows/docs-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.764044 autora-synthetic-data-1.0.0a1/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-04-28 22:10:21.768044 autora-synthetic-data-1.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.764044 autora-synthetic-data-1.0.0a1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   200744 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/docs/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.764044 autora-synthetic-data-1.0.0a1/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.764044 autora-synthetic-data-1.0.0a1/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/mkdocs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 22:10:21.768044 autora-synthetic-data-1.0.0a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.760044 autora-synthetic-data-1.0.0a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.760044 autora-synthetic-data-1.0.0a1/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.764044 autora-synthetic-data-1.0.0a1/src/autora/synthetic/
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/src/autora/synthetic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.764044 autora-synthetic-data-1.0.0a1/src/autora/synthetic/data/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/src/autora/synthetic/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/src/autora/synthetic/data/expected_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/src/autora/synthetic/data/prospect_theory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/src/autora/synthetic/data/template_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/src/autora/synthetic/data/weber_fechner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/src/autora/synthetic/inventory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.768044 autora-synthetic-data-1.0.0a1/src/autora_synthetic_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-04-28 22:10:21.000000 autora-synthetic-data-1.0.0a1/src/autora_synthetic_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-28 22:10:21.000000 autora-synthetic-data-1.0.0a1/src/autora_synthetic_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 22:10:21.000000 autora-synthetic-data-1.0.0a1/src/autora_synthetic_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 22:10:21.000000 autora-synthetic-data-1.0.0a1/src/autora_synthetic_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 22:10:21.000000 autora-synthetic-data-1.0.0a1/src/autora_synthetic_data.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:10:21.768044 autora-synthetic-data-1.0.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-28 22:10:07.000000 autora-synthetic-data-1.0.0a1/tests/test_synthetic_inventory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:29:46.642225 autora-synthetic-data-1.0.0a2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:29:46.638225 autora-synthetic-data-1.0.0a2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:29:46.638225 autora-synthetic-data-1.0.0a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/.github/workflows/docs-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:29:46.638225 autora-synthetic-data-1.0.0a2/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/.idea/autora-synthetic-data.iml
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-02 22:29:46.642225 autora-synthetic-data-1.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:29:46.642225 autora-synthetic-data-1.0.0a2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   200744 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/docs/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:29:46.642225 autora-synthetic-data-1.0.0a2/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:29:46.642225 autora-synthetic-data-1.0.0a2/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/mkdocs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 22:29:46.642225 autora-synthetic-data-1.0.0a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:29:46.638225 autora-synthetic-data-1.0.0a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:29:46.638225 autora-synthetic-data-1.0.0a2/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:29:46.642225 autora-synthetic-data-1.0.0a2/src/autora/synthetic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/src/autora/synthetic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:29:46.642225 autora-synthetic-data-1.0.0a2/src/autora/synthetic/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/src/autora/synthetic/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/src/autora/synthetic/data/expected_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/src/autora/synthetic/data/prospect_theory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/src/autora/synthetic/data/template_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/src/autora/synthetic/data/weber_fechner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/src/autora/synthetic/inventory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:29:46.642225 autora-synthetic-data-1.0.0a2/src/autora_synthetic_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-02 22:29:46.000000 autora-synthetic-data-1.0.0a2/src/autora_synthetic_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-02 22:29:46.000000 autora-synthetic-data-1.0.0a2/src/autora_synthetic_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 22:29:46.000000 autora-synthetic-data-1.0.0a2/src/autora_synthetic_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-02 22:29:46.000000 autora-synthetic-data-1.0.0a2/src/autora_synthetic_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 22:29:46.000000 autora-synthetic-data-1.0.0a2/src/autora_synthetic_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:29:46.642225 autora-synthetic-data-1.0.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-02 22:29:25.000000 autora-synthetic-data-1.0.0a2/tests/test_synthetic_inventory.py
```

### Comparing `autora-synthetic-data-1.0.0a1/.github/workflows/python-publish.yml` & `autora-synthetic-data-1.0.0a2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a1/.gitignore` & `autora-synthetic-data-1.0.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a1/.pre-commit-config.yaml` & `autora-synthetic-data-1.0.0a2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a1/PKG-INFO` & `autora-synthetic-data-1.0.0a2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: autora-synthetic-data
-Version: 1.0.0a1
-Summary: AutoRA Synthetic Data
-License: MIT License
-Project-URL: homepage, http://www.empiricalresearch.ai
-Project-URL: repository, https://github.com/AutoResearch/autora-theorist-template
-Project-URL: documentation, https://autoresearch.github.io/autora/
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 # AutoRA Synthetic Experiments
 
 A package with synthetic experiment data for testing AutoRA theorists and experimentalists.
 
 ## User Guide
 
 You will need:
@@ -21,16 +10,15 @@
 
 Install the synthetic data package:
 
 ```shell
 pip install -U "autora-synthetic-data"
 ```
 
-!!! success
-    It is recommended to use a `python` environment manager like `virtualenv`.
+> 💡We recommend using a `python` environment manager like `virtualenv`.
 
 Check your installation by running:
 ```shell
 python -c "from autora.synthetic import retrieve, describe; describe(retrieve('weber_fechner'))"
 ```
 
 ## Developer Guide
@@ -89,8 +77,8 @@
 - Add code to the template as required.
 
 New experiments can be submitted as pull requests.
 
 ### Publish the package
 
 This package can be published using GitHub actions – create a new "Release" on the GitHub 
-repository, and Actions will do the rest.
+repository, and Actions will do the rest.
```

### Comparing `autora-synthetic-data-1.0.0a1/docs/example.ipynb` & `autora-synthetic-data-1.0.0a2/docs/example.ipynb`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a1/docs/index.md` & `autora-synthetic-data-1.0.0a2/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a1/mkdocs/base.yml` & `autora-synthetic-data-1.0.0a2/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a1/mkdocs/gen_ref_pages.py` & `autora-synthetic-data-1.0.0a2/mkdocs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a1/pyproject.toml` & `autora-synthetic-data-1.0.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "autora-synthetic-data"
 description = "AutoRA Synthetic Data"
 authors = []
 dynamic = ["version"]
 
-readme = "README.md"
+readme = "docs/index.md"
 license = { text = "MIT License" }
 
 # ADD NEW DEPENDENCIES HERE
 dependencies = [
     "autora-core",
 ]
```

### Comparing `autora-synthetic-data-1.0.0a1/src/autora/synthetic/__init__.py` & `autora-synthetic-data-1.0.0a2/src/autora/synthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a1/src/autora/synthetic/data/expected_value.py` & `autora-synthetic-data-1.0.0a2/src/autora/synthetic/data/expected_value.py`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a1/src/autora/synthetic/data/prospect_theory.py` & `autora-synthetic-data-1.0.0a2/src/autora/synthetic/data/prospect_theory.py`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a1/src/autora/synthetic/data/template_experiment.py` & `autora-synthetic-data-1.0.0a2/src/autora/synthetic/data/template_experiment.py`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a1/src/autora/synthetic/data/weber_fechner.py` & `autora-synthetic-data-1.0.0a2/src/autora/synthetic/data/weber_fechner.py`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a1/src/autora/synthetic/inventory.py` & `autora-synthetic-data-1.0.0a2/src/autora/synthetic/inventory.py`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a1/src/autora_synthetic_data.egg-info/SOURCES.txt` & `autora-synthetic-data-1.0.0a2/src/autora_synthetic_data.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .pre-commit-config.yaml
 README.md
 mkdocs.yml
 pyproject.toml
 .github/workflows/docs-publish.yml
 .github/workflows/python-publish.yml
 .idea/.gitignore
+.idea/autora-synthetic-data.iml
 .idea/misc.xml
 .idea/modules.xml
 .idea/vcs.xml
 docs/example.ipynb
 docs/index.md
 docs/javascripts/mathjax.js
 mkdocs/base.yml
```

### Comparing `autora-synthetic-data-1.0.0a1/tests/README.md` & `autora-synthetic-data-1.0.0a2/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a1/tests/test_synthetic_inventory.py` & `autora-synthetic-data-1.0.0a2/tests/test_synthetic_inventory.py`

 * *Files identical despite different names*

