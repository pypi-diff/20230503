# Comparing `tmp/inference-server-0.1.0.tar.gz` & `tmp/inference-server-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inference-server-0.1.0.tar", last modified: Tue May  2 10:09:10 2023, max compression
+gzip compressed data, was "inference-server-0.2.0.tar", last modified: Wed May  3 19:11:13 2023, max compression
```

## Comparing `inference-server-0.1.0.tar` & `inference-server-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:09:10.437518 inference-server-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-02 10:08:51.000000 inference-server-0.1.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-02 10:08:51.000000 inference-server-0.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:09:10.433518 inference-server-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:09:10.433518 inference-server-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-02 10:08:51.000000 inference-server-0.1.0/.github/workflows/release-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-02 10:08:51.000000 inference-server-0.1.0/.github/workflows/test-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-05-02 10:08:52.000000 inference-server-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-02 10:08:52.000000 inference-server-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-05-02 10:08:52.000000 inference-server-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-02 10:08:52.000000 inference-server-0.1.0/LICENSE_HEADER.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14171 2023-05-02 10:09:10.433518 inference-server-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-02 10:08:52.000000 inference-server-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-02 10:08:52.000000 inference-server-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 10:09:10.437518 inference-server-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:09:10.433518 inference-server-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:09:10.433518 inference-server-0.1.0/src/inference_server/
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-02 10:08:52.000000 inference-server-0.1.0/src/inference_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-05-02 10:08:52.000000 inference-server-0.1.0/src/inference_server/_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-02 10:08:52.000000 inference-server-0.1.0/src/inference_server/default_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-02 10:08:52.000000 inference-server-0.1.0/src/inference_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-02 10:08:52.000000 inference-server-0.1.0/src/inference_server/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:09:10.433518 inference-server-0.1.0/src/inference_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14171 2023-05-02 10:09:10.000000 inference-server-0.1.0/src/inference_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-02 10:09:10.000000 inference-server-0.1.0/src/inference_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:09:10.000000 inference-server-0.1.0/src/inference_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-02 10:09:10.000000 inference-server-0.1.0/src/inference_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 10:09:10.000000 inference-server-0.1.0/src/inference_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:09:10.433518 inference-server-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-02 10:08:52.000000 inference-server-0.1.0/tests/test_inference_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-02 10:08:52.000000 inference-server-0.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:11:13.912146 inference-server-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-03 19:11:01.000000 inference-server-0.2.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-03 19:11:01.000000 inference-server-0.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:11:13.908146 inference-server-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:11:13.908146 inference-server-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-03 19:11:01.000000 inference-server-0.2.0/.github/workflows/release-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-03 19:11:01.000000 inference-server-0.2.0/.github/workflows/test-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-05-03 19:11:01.000000 inference-server-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-03 19:11:01.000000 inference-server-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-03 19:11:01.000000 inference-server-0.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-05-03 19:11:01.000000 inference-server-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-03 19:11:01.000000 inference-server-0.2.0/LICENSE_HEADER.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14171 2023-05-03 19:11:13.912146 inference-server-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-03 19:11:01.000000 inference-server-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:11:13.912146 inference-server-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-03 19:11:01.000000 inference-server-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-05-03 19:11:01.000000 inference-server-0.2.0/docs/deployment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-03 19:11:01.000000 inference-server-0.2.0/docs/hooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-03 19:11:01.000000 inference-server-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-03 19:11:01.000000 inference-server-0.2.0/docs/inference_server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-03 19:11:01.000000 inference-server-0.2.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-03 19:11:01.000000 inference-server-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 19:11:13.912146 inference-server-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:11:13.908146 inference-server-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:11:13.912146 inference-server-0.2.0/src/inference_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-03 19:11:01.000000 inference-server-0.2.0/src/inference_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-05-03 19:11:01.000000 inference-server-0.2.0/src/inference_server/_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-03 19:11:01.000000 inference-server-0.2.0/src/inference_server/default_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-03 19:11:01.000000 inference-server-0.2.0/src/inference_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-03 19:11:01.000000 inference-server-0.2.0/src/inference_server/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:11:13.912146 inference-server-0.2.0/src/inference_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14171 2023-05-03 19:11:13.000000 inference-server-0.2.0/src/inference_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-03 19:11:13.000000 inference-server-0.2.0/src/inference_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:11:13.000000 inference-server-0.2.0/src/inference_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-03 19:11:13.000000 inference-server-0.2.0/src/inference_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-03 19:11:13.000000 inference-server-0.2.0/src/inference_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:11:13.912146 inference-server-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-03 19:11:01.000000 inference-server-0.2.0/tests/test_inference_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-03 19:11:01.000000 inference-server-0.2.0/tox.ini
```

### Comparing `inference-server-0.1.0/.flake8` & `inference-server-0.2.0/.flake8`

 * *Files identical despite different names*

### Comparing `inference-server-0.1.0/.github/workflows/release-package.yml` & `inference-server-0.2.0/.github/workflows/release-package.yml`

 * *Files identical despite different names*

### Comparing `inference-server-0.1.0/.github/workflows/test-package.yml` & `inference-server-0.2.0/.github/workflows/test-package.yml`

 * *Files identical despite different names*

### Comparing `inference-server-0.1.0/.gitignore` & `inference-server-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `inference-server-0.1.0/.pre-commit-config.yaml` & `inference-server-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `inference-server-0.1.0/LICENSE` & `inference-server-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inference-server-0.1.0/LICENSE_HEADER.txt` & `inference-server-0.2.0/LICENSE_HEADER.txt`

 * *Files identical despite different names*

### Comparing `inference-server-0.1.0/PKG-INFO` & `inference-server-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inference-server
-Version: 0.1.0
+Version: 0.2.0
 Summary: Pluggable Python HTTP web service (WSGI) for real-time AI/ML model inference compatible with Amazon SageMaker.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `inference-server-0.1.0/README.md` & `inference-server-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `inference-server-0.1.0/pyproject.toml` & `inference-server-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `inference-server-0.1.0/src/inference_server/__init__.py` & `inference-server-0.2.0/src/inference_server/__init__.py`

 * *Files identical despite different names*

### Comparing `inference-server-0.1.0/src/inference_server/_plugin.py` & `inference-server-0.2.0/src/inference_server/_plugin.py`

 * *Files identical despite different names*

### Comparing `inference-server-0.1.0/src/inference_server/default_plugin.py` & `inference-server-0.2.0/src/inference_server/default_plugin.py`

 * *Files identical despite different names*

### Comparing `inference-server-0.1.0/src/inference_server/testing.py` & `inference-server-0.2.0/src/inference_server/testing.py`

 * *Files identical despite different names*

### Comparing `inference-server-0.1.0/src/inference_server.egg-info/PKG-INFO` & `inference-server-0.2.0/src/inference_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inference-server
-Version: 0.1.0
+Version: 0.2.0
 Summary: Pluggable Python HTTP web service (WSGI) for real-time AI/ML model inference compatible with Amazon SageMaker.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `inference-server-0.1.0/src/inference_server.egg-info/SOURCES.txt` & `inference-server-0.2.0/src/inference_server.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 .editorconfig
 .flake8
 .gitignore
 .pre-commit-config.yaml
+.readthedocs.yaml
 LICENSE
 LICENSE_HEADER.txt
 README.md
 pyproject.toml
 tox.ini
 .github/workflows/release-package.yml
 .github/workflows/test-package.yml
+docs/conf.py
+docs/deployment.rst
+docs/hooks.rst
+docs/index.rst
+docs/inference_server.rst
+docs/modules.rst
 src/inference_server/__init__.py
 src/inference_server/_plugin.py
 src/inference_server/default_plugin.py
 src/inference_server/py.typed
 src/inference_server/testing.py
 src/inference_server.egg-info/PKG-INFO
 src/inference_server.egg-info/SOURCES.txt
```

### Comparing `inference-server-0.1.0/tests/test_inference_server.py` & `inference-server-0.2.0/tests/test_inference_server.py`

 * *Files identical despite different names*

### Comparing `inference-server-0.1.0/tox.ini` & `inference-server-0.2.0/tox.ini`

 * *Files identical despite different names*

