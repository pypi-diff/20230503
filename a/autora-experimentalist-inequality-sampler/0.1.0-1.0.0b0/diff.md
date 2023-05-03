# Comparing `tmp/autora-experimentalist-inequality-sampler-0.1.0.tar.gz` & `tmp/autora-experimentalist-inequality-sampler-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-experimentalist-inequality-sampler-0.1.0.tar", last modified: Tue May  2 13:34:38 2023, max compression
+gzip compressed data, was "autora-experimentalist-inequality-sampler-1.0.0b0.tar", last modified: Wed May  3 16:30:54 2023, max compression
```

## Comparing `autora-experimentalist-inequality-sampler-0.1.0.tar` & `autora-experimentalist-inequality-sampler-1.0.0b0.tar`

### file list

```diff
@@ -1,17 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:34:38.161184 autora-experimentalist-inequality-sampler-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-02 13:34:38.161184 autora-experimentalist-inequality-sampler-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-02 13:34:26.000000 autora-experimentalist-inequality-sampler-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-02 13:34:26.000000 autora-experimentalist-inequality-sampler-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 13:34:38.161184 autora-experimentalist-inequality-sampler-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:34:38.161184 autora-experimentalist-inequality-sampler-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:34:38.157184 autora-experimentalist-inequality-sampler-0.1.0/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:34:38.157184 autora-experimentalist-inequality-sampler-0.1.0/src/autora/experimentalist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:34:38.161184 autora-experimentalist-inequality-sampler-0.1.0/src/autora/experimentalist/sampler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:34:38.161184 autora-experimentalist-inequality-sampler-0.1.0/src/autora/experimentalist/sampler/inequality/
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-02 13:34:26.000000 autora-experimentalist-inequality-sampler-0.1.0/src/autora/experimentalist/sampler/inequality/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:34:38.161184 autora-experimentalist-inequality-sampler-0.1.0/src/autora_experimentalist_inequality_sampler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-02 13:34:38.000000 autora-experimentalist-inequality-sampler-0.1.0/src/autora_experimentalist_inequality_sampler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-02 13:34:38.000000 autora-experimentalist-inequality-sampler-0.1.0/src/autora_experimentalist_inequality_sampler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:34:38.000000 autora-experimentalist-inequality-sampler-0.1.0/src/autora_experimentalist_inequality_sampler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-02 13:34:38.000000 autora-experimentalist-inequality-sampler-0.1.0/src/autora_experimentalist_inequality_sampler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 13:34:38.000000 autora-experimentalist-inequality-sampler-0.1.0/src/autora_experimentalist_inequality_sampler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:30:54.483792 autora-experimentalist-inequality-sampler-1.0.0b0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:30:54.479792 autora-experimentalist-inequality-sampler-1.0.0b0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:30:54.479792 autora-experimentalist-inequality-sampler-1.0.0b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-03 16:30:42.000000 autora-experimentalist-inequality-sampler-1.0.0b0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-03 16:30:42.000000 autora-experimentalist-inequality-sampler-1.0.0b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-03 16:30:42.000000 autora-experimentalist-inequality-sampler-1.0.0b0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-03 16:30:54.483792 autora-experimentalist-inequality-sampler-1.0.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-03 16:30:42.000000 autora-experimentalist-inequality-sampler-1.0.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:30:54.479792 autora-experimentalist-inequality-sampler-1.0.0b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-03 16:30:42.000000 autora-experimentalist-inequality-sampler-1.0.0b0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:30:54.479792 autora-experimentalist-inequality-sampler-1.0.0b0/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-03 16:30:42.000000 autora-experimentalist-inequality-sampler-1.0.0b0/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:30:54.479792 autora-experimentalist-inequality-sampler-1.0.0b0/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-03 16:30:42.000000 autora-experimentalist-inequality-sampler-1.0.0b0/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-03 16:30:42.000000 autora-experimentalist-inequality-sampler-1.0.0b0/mkdocs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-03 16:30:42.000000 autora-experimentalist-inequality-sampler-1.0.0b0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-03 16:30:42.000000 autora-experimentalist-inequality-sampler-1.0.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 16:30:54.483792 autora-experimentalist-inequality-sampler-1.0.0b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:30:54.479792 autora-experimentalist-inequality-sampler-1.0.0b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:30:54.479792 autora-experimentalist-inequality-sampler-1.0.0b0/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:30:54.479792 autora-experimentalist-inequality-sampler-1.0.0b0/src/autora/experimentalist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:30:54.479792 autora-experimentalist-inequality-sampler-1.0.0b0/src/autora/experimentalist/sampler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:30:54.479792 autora-experimentalist-inequality-sampler-1.0.0b0/src/autora/experimentalist/sampler/inequality/
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-03 16:30:42.000000 autora-experimentalist-inequality-sampler-1.0.0b0/src/autora/experimentalist/sampler/inequality/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:30:54.479792 autora-experimentalist-inequality-sampler-1.0.0b0/src/autora_experimentalist_inequality_sampler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-03 16:30:54.000000 autora-experimentalist-inequality-sampler-1.0.0b0/src/autora_experimentalist_inequality_sampler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-03 16:30:54.000000 autora-experimentalist-inequality-sampler-1.0.0b0/src/autora_experimentalist_inequality_sampler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 16:30:54.000000 autora-experimentalist-inequality-sampler-1.0.0b0/src/autora_experimentalist_inequality_sampler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-03 16:30:54.000000 autora-experimentalist-inequality-sampler-1.0.0b0/src/autora_experimentalist_inequality_sampler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 16:30:54.000000 autora-experimentalist-inequality-sampler-1.0.0b0/src/autora_experimentalist_inequality_sampler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:30:54.483792 autora-experimentalist-inequality-sampler-1.0.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-03 16:30:42.000000 autora-experimentalist-inequality-sampler-1.0.0b0/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 16:30:42.000000 autora-experimentalist-inequality-sampler-1.0.0b0/tests/__init__.py
```

### Comparing `autora-experimentalist-inequality-sampler-0.1.0/PKG-INFO` & `autora-experimentalist-inequality-sampler-1.0.0b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-inequality-sampler
-Version: 0.1.0
+Version: 1.0.0b0
 Summary: AutoRA Inequality Sampler
 Author-email: "Chad C. Williams" <cwilliams.uca@gmail.com>, Younes Strittmatter <younes_strittmatter@brown.com>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experimentalist-inequality-sampler
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-experimentalist-inequality-sampler-0.1.0/README.md` & `autora-experimentalist-inequality-sampler-1.0.0b0/README.md`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-inequality-sampler-0.1.0/pyproject.toml` & `autora-experimentalist-inequality-sampler-1.0.0b0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # UPDATE THIS BEFORE PUBLISHING
 name = "autora-experimentalist-inequality-sampler"
 description = "AutoRA Inequality Sampler"
 authors = [
     { name = "Chad C. Williams", email = "cwilliams.uca@gmail.com" },
     { name = "Younes Strittmatter", email = "younes_strittmatter@brown.com" }
 ]
-version = "0.1.0"
+dynamic = ["version"]
 
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.8,<4"
 
 # ADD NEW DEPENDENCIES HERE
 dependencies = [
@@ -24,9 +24,11 @@
 
 [project.urls]
 homepage = "http://www.empiricalresearch.ai"
 repository = "https://github.com/AutoResearch/autora-experimentalist-inequality-sampler"
 documentation = "https://autoresearch.github.io/autora/"
 
 [build-system]
-requires = ["setuptools"]
+requires = ["setuptools", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
+
+[tool.setuptools_scm]
```

### Comparing `autora-experimentalist-inequality-sampler-0.1.0/src/autora/experimentalist/sampler/inequality/__init__.py` & `autora-experimentalist-inequality-sampler-1.0.0b0/src/autora/experimentalist/sampler/inequality/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-inequality-sampler-0.1.0/src/autora_experimentalist_inequality_sampler.egg-info/PKG-INFO` & `autora-experimentalist-inequality-sampler-1.0.0b0/src/autora_experimentalist_inequality_sampler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-inequality-sampler
-Version: 0.1.0
+Version: 1.0.0b0
 Summary: AutoRA Inequality Sampler
 Author-email: "Chad C. Williams" <cwilliams.uca@gmail.com>, Younes Strittmatter <younes_strittmatter@brown.com>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experimentalist-inequality-sampler
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

