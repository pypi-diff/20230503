# Comparing `tmp/open-aea-ledger-ethereum-1.9.0.tar.gz` & `tmp/open-aea-ledger-ethereum-1.9.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-aea-ledger-ethereum-1.9.0.tar", last modified: Thu May 26 17:38:47 2022, max compression
+gzip compressed data, was "open-aea-ledger-ethereum-1.9.0.post1.tar", last modified: Wed Jun  1 12:04:31 2022, max compression
```

## Comparing `open-aea-ledger-ethereum-1.9.0.tar` & `open-aea-ledger-ethereum-1.9.0.post1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:47.361317 open-aea-ledger-ethereum-1.9.0/
--rw-r--r--   0 root         (0) root         (0)    11374 2022-05-26 15:42:34.000000 open-aea-ledger-ethereum-1.9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      102 2022-05-26 15:42:34.000000 open-aea-ledger-ethereum-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      982 2022-05-26 17:38:47.361317 open-aea-ledger-ethereum-1.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      173 2022-05-26 15:42:34.000000 open-aea-ledger-ethereum-1.9.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:47.357317 open-aea-ledger-ethereum-1.9.0/aea_ledger_ethereum/
--rw-r--r--   0 root         (0) root         (0)     1035 2022-05-26 15:42:34.000000 open-aea-ledger-ethereum-1.9.0/aea_ledger_ethereum/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53559 2022-05-26 15:42:34.000000 open-aea-ledger-ethereum-1.9.0/aea_ledger_ethereum/ethereum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:47.357317 open-aea-ledger-ethereum-1.9.0/open_aea_ledger_ethereum.egg-info/
--rw-r--r--   0 root         (0) root         (0)      982 2022-05-26 17:38:47.000000 open-aea-ledger-ethereum-1.9.0/open_aea_ledger_ethereum.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      756 2022-05-26 17:38:47.000000 open-aea-ledger-ethereum-1.9.0/open_aea_ledger_ethereum.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-26 17:38:47.000000 open-aea-ledger-ethereum-1.9.0/open_aea_ledger_ethereum.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      191 2022-05-26 17:38:47.000000 open-aea-ledger-ethereum-1.9.0/open_aea_ledger_ethereum.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       79 2022-05-26 17:38:47.000000 open-aea-ledger-ethereum-1.9.0/open_aea_ledger_ethereum.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-05-26 17:38:47.000000 open-aea-ledger-ethereum-1.9.0/open_aea_ledger_ethereum.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       90 2022-05-26 15:42:34.000000 open-aea-ledger-ethereum-1.9.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-26 17:38:47.361317 open-aea-ledger-ethereum-1.9.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2399 2022-05-26 17:32:20.000000 open-aea-ledger-ethereum-1.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:47.357317 open-aea-ledger-ethereum-1.9.0/tests/
--rw-r--r--   0 root         (0) root         (0)      874 2022-05-26 15:42:34.000000 open-aea-ledger-ethereum-1.9.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7818 2022-05-26 15:42:34.000000 open-aea-ledger-ethereum-1.9.0/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:47.357317 open-aea-ledger-ethereum-1.9.0/tests/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:47.357317 open-aea-ledger-ethereum-1.9.0/tests/data/dummy_contract/
--rw-r--r--   0 root         (0) root         (0)      881 2022-05-26 15:42:34.000000 open-aea-ledger-ethereum-1.9.0/tests/data/dummy_contract/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:47.361317 open-aea-ledger-ethereum-1.9.0/tests/data/dummy_contract/build/
--rw-r--r--   0 root         (0) root         (0)   120902 2022-05-26 15:42:34.000000 open-aea-ledger-ethereum-1.9.0/tests/data/dummy_contract/build/some.json
--rw-r--r--   0 root         (0) root         (0)   220992 2022-05-13 16:38:39.000000 open-aea-ledger-ethereum-1.9.0/tests/data/dummy_contract/build/some.wasm
--rw-r--r--   0 root         (0) root         (0)     1166 2022-05-26 15:42:34.000000 open-aea-ledger-ethereum-1.9.0/tests/data/dummy_contract/contract.py
--rw-r--r--   0 root         (0) root         (0)      640 2022-05-26 15:42:34.000000 open-aea-ledger-ethereum-1.9.0/tests/data/dummy_contract/contract.yaml
--rw-r--r--   0 root         (0) root         (0)       66 2022-05-26 15:42:34.000000 open-aea-ledger-ethereum-1.9.0/tests/data/ethereum_private_key.txt
--rw-r--r--   0 root         (0) root         (0)     6026 2022-05-26 15:42:34.000000 open-aea-ledger-ethereum-1.9.0/tests/docker_image.py
--rw-r--r--   0 root         (0) root         (0)    28010 2022-05-26 15:42:34.000000 open-aea-ledger-ethereum-1.9.0/tests/test_ethereum.py
--rw-r--r--   0 root         (0) root         (0)     4489 2022-05-26 15:42:34.000000 open-aea-ledger-ethereum-1.9.0/tests/test_ethereum_contract.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:31.464475 open-aea-ledger-ethereum-1.9.0.post1/
+-rw-r--r--   0 root         (0) root         (0)    11374 2022-06-01 11:11:15.000000 open-aea-ledger-ethereum-1.9.0.post1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      102 2022-06-01 11:11:15.000000 open-aea-ledger-ethereum-1.9.0.post1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      988 2022-06-01 12:04:31.460475 open-aea-ledger-ethereum-1.9.0.post1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      173 2022-06-01 11:11:15.000000 open-aea-ledger-ethereum-1.9.0.post1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:31.460475 open-aea-ledger-ethereum-1.9.0.post1/aea_ledger_ethereum/
+-rw-r--r--   0 root         (0) root         (0)     1035 2022-06-01 11:11:15.000000 open-aea-ledger-ethereum-1.9.0.post1/aea_ledger_ethereum/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53559 2022-06-01 11:11:15.000000 open-aea-ledger-ethereum-1.9.0.post1/aea_ledger_ethereum/ethereum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:31.460475 open-aea-ledger-ethereum-1.9.0.post1/open_aea_ledger_ethereum.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      988 2022-06-01 12:04:31.000000 open-aea-ledger-ethereum-1.9.0.post1/open_aea_ledger_ethereum.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      756 2022-06-01 12:04:31.000000 open-aea-ledger-ethereum-1.9.0.post1/open_aea_ledger_ethereum.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-01 12:04:31.000000 open-aea-ledger-ethereum-1.9.0.post1/open_aea_ledger_ethereum.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      191 2022-06-01 12:04:31.000000 open-aea-ledger-ethereum-1.9.0.post1/open_aea_ledger_ethereum.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2022-06-01 12:04:31.000000 open-aea-ledger-ethereum-1.9.0.post1/open_aea_ledger_ethereum.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2022-06-01 12:04:31.000000 open-aea-ledger-ethereum-1.9.0.post1/open_aea_ledger_ethereum.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2022-06-01 11:11:15.000000 open-aea-ledger-ethereum-1.9.0.post1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-06-01 12:04:31.464475 open-aea-ledger-ethereum-1.9.0.post1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2405 2022-06-01 12:00:46.000000 open-aea-ledger-ethereum-1.9.0.post1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:31.460475 open-aea-ledger-ethereum-1.9.0.post1/tests/
+-rw-r--r--   0 root         (0) root         (0)      874 2022-06-01 11:11:15.000000 open-aea-ledger-ethereum-1.9.0.post1/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7818 2022-06-01 11:11:15.000000 open-aea-ledger-ethereum-1.9.0.post1/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:31.460475 open-aea-ledger-ethereum-1.9.0.post1/tests/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:31.460475 open-aea-ledger-ethereum-1.9.0.post1/tests/data/dummy_contract/
+-rw-r--r--   0 root         (0) root         (0)      881 2022-06-01 11:11:15.000000 open-aea-ledger-ethereum-1.9.0.post1/tests/data/dummy_contract/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:31.460475 open-aea-ledger-ethereum-1.9.0.post1/tests/data/dummy_contract/build/
+-rw-r--r--   0 root         (0) root         (0)   120902 2022-06-01 11:11:15.000000 open-aea-ledger-ethereum-1.9.0.post1/tests/data/dummy_contract/build/some.json
+-rw-r--r--   0 root         (0) root         (0)   220992 2022-05-13 16:38:39.000000 open-aea-ledger-ethereum-1.9.0.post1/tests/data/dummy_contract/build/some.wasm
+-rw-r--r--   0 root         (0) root         (0)     1166 2022-06-01 11:11:15.000000 open-aea-ledger-ethereum-1.9.0.post1/tests/data/dummy_contract/contract.py
+-rw-r--r--   0 root         (0) root         (0)      640 2022-06-01 11:11:15.000000 open-aea-ledger-ethereum-1.9.0.post1/tests/data/dummy_contract/contract.yaml
+-rw-r--r--   0 root         (0) root         (0)       66 2022-06-01 11:11:15.000000 open-aea-ledger-ethereum-1.9.0.post1/tests/data/ethereum_private_key.txt
+-rw-r--r--   0 root         (0) root         (0)     6026 2022-06-01 11:11:15.000000 open-aea-ledger-ethereum-1.9.0.post1/tests/docker_image.py
+-rw-r--r--   0 root         (0) root         (0)    28010 2022-06-01 11:11:15.000000 open-aea-ledger-ethereum-1.9.0.post1/tests/test_ethereum.py
+-rw-r--r--   0 root         (0) root         (0)     4489 2022-06-01 11:11:15.000000 open-aea-ledger-ethereum-1.9.0.post1/tests/test_ethereum_contract.py
```

### Comparing `open-aea-ledger-ethereum-1.9.0/LICENSE` & `open-aea-ledger-ethereum-1.9.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-1.9.0/PKG-INFO` & `open-aea-ledger-ethereum-1.9.0.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-ethereum
-Version: 1.9.0
+Version: 1.9.0.post1
 Summary: Python package wrapping the public and private key cryptography and ledger api of Ethereum.
 Home-page: UNKNOWN
 Author: Valory AG
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `open-aea-ledger-ethereum-1.9.0/aea_ledger_ethereum/__init__.py` & `open-aea-ledger-ethereum-1.9.0.post1/aea_ledger_ethereum/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-1.9.0/aea_ledger_ethereum/ethereum.py` & `open-aea-ledger-ethereum-1.9.0.post1/aea_ledger_ethereum/ethereum.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-1.9.0/open_aea_ledger_ethereum.egg-info/PKG-INFO` & `open-aea-ledger-ethereum-1.9.0.post1/open_aea_ledger_ethereum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-ethereum
-Version: 1.9.0
+Version: 1.9.0.post1
 Summary: Python package wrapping the public and private key cryptography and ledger api of Ethereum.
 Home-page: UNKNOWN
 Author: Valory AG
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `open-aea-ledger-ethereum-1.9.0/open_aea_ledger_ethereum.egg-info/SOURCES.txt` & `open-aea-ledger-ethereum-1.9.0.post1/open_aea_ledger_ethereum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-1.9.0/setup.py` & `open-aea-ledger-ethereum-1.9.0.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 """Setup script for "aea_ledger_ethereum" package."""
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="open-aea-ledger-ethereum",
-    version="1.9.0",
+    version="1.9.0.post1",
     author="Valory AG",
     license="Apache-2.0",
     description="Python package wrapping the public and private key cryptography and ledger api of Ethereum.",
     packages=find_packages(include=["aea_ledger_ethereum*"]),
     install_requires=[
         "open-aea>=1.0.0, <2.0.0",
         "web3==5.25.0",
```

### Comparing `open-aea-ledger-ethereum-1.9.0/tests/__init__.py` & `open-aea-ledger-ethereum-1.9.0.post1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-1.9.0/tests/conftest.py` & `open-aea-ledger-ethereum-1.9.0.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-1.9.0/tests/data/dummy_contract/__init__.py` & `open-aea-ledger-ethereum-1.9.0.post1/tests/data/dummy_contract/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-1.9.0/tests/data/dummy_contract/build/some.json` & `open-aea-ledger-ethereum-1.9.0.post1/tests/data/dummy_contract/build/some.json`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-1.9.0/tests/data/dummy_contract/build/some.wasm` & `open-aea-ledger-ethereum-1.9.0.post1/tests/data/dummy_contract/build/some.wasm`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-1.9.0/tests/data/dummy_contract/contract.py` & `open-aea-ledger-ethereum-1.9.0.post1/tests/data/dummy_contract/contract.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-1.9.0/tests/data/dummy_contract/contract.yaml` & `open-aea-ledger-ethereum-1.9.0.post1/tests/data/dummy_contract/contract.yaml`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-1.9.0/tests/docker_image.py` & `open-aea-ledger-ethereum-1.9.0.post1/tests/docker_image.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-1.9.0/tests/test_ethereum.py` & `open-aea-ledger-ethereum-1.9.0.post1/tests/test_ethereum.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-1.9.0/tests/test_ethereum_contract.py` & `open-aea-ledger-ethereum-1.9.0.post1/tests/test_ethereum_contract.py`

 * *Files identical despite different names*

