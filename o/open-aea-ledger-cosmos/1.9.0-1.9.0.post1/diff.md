# Comparing `tmp/open-aea-ledger-cosmos-1.9.0.tar.gz` & `tmp/open-aea-ledger-cosmos-1.9.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-aea-ledger-cosmos-1.9.0.tar", last modified: Thu May 26 17:38:41 2022, max compression
+gzip compressed data, was "open-aea-ledger-cosmos-1.9.0.post1.tar", last modified: Wed Jun  1 12:04:22 2022, max compression
```

## Comparing `open-aea-ledger-cosmos-1.9.0.tar` & `open-aea-ledger-cosmos-1.9.0.post1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:41.797374 open-aea-ledger-cosmos-1.9.0/
--rw-r--r--   0 root         (0) root         (0)    11374 2022-05-26 15:42:34.000000 open-aea-ledger-cosmos-1.9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      100 2022-05-26 15:42:34.000000 open-aea-ledger-cosmos-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      978 2022-05-26 17:38:41.797374 open-aea-ledger-cosmos-1.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      169 2022-05-26 15:42:34.000000 open-aea-ledger-cosmos-1.9.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:41.793374 open-aea-ledger-cosmos-1.9.0/aea_ledger_cosmos/
--rw-r--r--   0 root         (0) root         (0)     1040 2022-05-26 15:42:34.000000 open-aea-ledger-cosmos-1.9.0/aea_ledger_cosmos/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58462 2022-05-26 15:42:34.000000 open-aea-ledger-cosmos-1.9.0/aea_ledger_cosmos/cosmos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:41.793374 open-aea-ledger-cosmos-1.9.0/open_aea_ledger_cosmos.egg-info/
--rw-r--r--   0 root         (0) root         (0)      978 2022-05-26 17:38:41.000000 open-aea-ledger-cosmos-1.9.0/open_aea_ledger_cosmos.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      680 2022-05-26 17:38:41.000000 open-aea-ledger-cosmos-1.9.0/open_aea_ledger_cosmos.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-26 17:38:41.000000 open-aea-ledger-cosmos-1.9.0/open_aea_ledger_cosmos.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      173 2022-05-26 17:38:41.000000 open-aea-ledger-cosmos-1.9.0/open_aea_ledger_cosmos.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       99 2022-05-26 17:38:41.000000 open-aea-ledger-cosmos-1.9.0/open_aea_ledger_cosmos.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-05-26 17:38:41.000000 open-aea-ledger-cosmos-1.9.0/open_aea_ledger_cosmos.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       90 2022-05-26 15:42:34.000000 open-aea-ledger-cosmos-1.9.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-26 17:38:41.797374 open-aea-ledger-cosmos-1.9.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2404 2022-05-26 17:32:20.000000 open-aea-ledger-cosmos-1.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:41.793374 open-aea-ledger-cosmos-1.9.0/tests/
--rw-r--r--   0 root         (0) root         (0)      872 2022-05-26 15:42:34.000000 open-aea-ledger-cosmos-1.9.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1310 2022-05-26 15:42:34.000000 open-aea-ledger-cosmos-1.9.0/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:41.793374 open-aea-ledger-cosmos-1.9.0/tests/data/
--rw-r--r--   0 root         (0) root         (0)       64 2022-05-26 15:42:34.000000 open-aea-ledger-cosmos-1.9.0/tests/data/cosmos_private_key.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:41.797374 open-aea-ledger-cosmos-1.9.0/tests/data/dummy_contract/
--rw-r--r--   0 root         (0) root         (0)      881 2022-05-26 15:42:34.000000 open-aea-ledger-cosmos-1.9.0/tests/data/dummy_contract/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:41.797374 open-aea-ledger-cosmos-1.9.0/tests/data/dummy_contract/build/
--rw-r--r--   0 root         (0) root         (0)   120902 2022-05-26 15:42:34.000000 open-aea-ledger-cosmos-1.9.0/tests/data/dummy_contract/build/some.json
--rw-r--r--   0 root         (0) root         (0)   220992 2022-05-13 16:38:39.000000 open-aea-ledger-cosmos-1.9.0/tests/data/dummy_contract/build/some.wasm
--rw-r--r--   0 root         (0) root         (0)     1166 2022-05-26 15:42:34.000000 open-aea-ledger-cosmos-1.9.0/tests/data/dummy_contract/contract.py
--rw-r--r--   0 root         (0) root         (0)      640 2022-05-26 15:42:34.000000 open-aea-ledger-cosmos-1.9.0/tests/data/dummy_contract/contract.yaml
--rw-r--r--   0 root         (0) root         (0)     9564 2022-05-26 15:42:34.000000 open-aea-ledger-cosmos-1.9.0/tests/test_cosmos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:22.372564 open-aea-ledger-cosmos-1.9.0.post1/
+-rw-r--r--   0 root         (0) root         (0)    11374 2022-06-01 11:11:15.000000 open-aea-ledger-cosmos-1.9.0.post1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      100 2022-06-01 11:11:15.000000 open-aea-ledger-cosmos-1.9.0.post1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      984 2022-06-01 12:04:22.372564 open-aea-ledger-cosmos-1.9.0.post1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      169 2022-06-01 11:11:15.000000 open-aea-ledger-cosmos-1.9.0.post1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:22.368564 open-aea-ledger-cosmos-1.9.0.post1/aea_ledger_cosmos/
+-rw-r--r--   0 root         (0) root         (0)     1040 2022-06-01 11:11:15.000000 open-aea-ledger-cosmos-1.9.0.post1/aea_ledger_cosmos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58462 2022-06-01 11:11:15.000000 open-aea-ledger-cosmos-1.9.0.post1/aea_ledger_cosmos/cosmos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:22.368564 open-aea-ledger-cosmos-1.9.0.post1/open_aea_ledger_cosmos.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      984 2022-06-01 12:04:22.000000 open-aea-ledger-cosmos-1.9.0.post1/open_aea_ledger_cosmos.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      680 2022-06-01 12:04:22.000000 open-aea-ledger-cosmos-1.9.0.post1/open_aea_ledger_cosmos.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-01 12:04:22.000000 open-aea-ledger-cosmos-1.9.0.post1/open_aea_ledger_cosmos.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      173 2022-06-01 12:04:22.000000 open-aea-ledger-cosmos-1.9.0.post1/open_aea_ledger_cosmos.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       99 2022-06-01 12:04:22.000000 open-aea-ledger-cosmos-1.9.0.post1/open_aea_ledger_cosmos.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2022-06-01 12:04:22.000000 open-aea-ledger-cosmos-1.9.0.post1/open_aea_ledger_cosmos.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2022-06-01 11:11:15.000000 open-aea-ledger-cosmos-1.9.0.post1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-06-01 12:04:22.372564 open-aea-ledger-cosmos-1.9.0.post1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2410 2022-06-01 12:00:48.000000 open-aea-ledger-cosmos-1.9.0.post1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:22.368564 open-aea-ledger-cosmos-1.9.0.post1/tests/
+-rw-r--r--   0 root         (0) root         (0)      872 2022-06-01 11:11:15.000000 open-aea-ledger-cosmos-1.9.0.post1/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1310 2022-06-01 11:11:15.000000 open-aea-ledger-cosmos-1.9.0.post1/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:22.368564 open-aea-ledger-cosmos-1.9.0.post1/tests/data/
+-rw-r--r--   0 root         (0) root         (0)       64 2022-06-01 11:11:15.000000 open-aea-ledger-cosmos-1.9.0.post1/tests/data/cosmos_private_key.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:22.372564 open-aea-ledger-cosmos-1.9.0.post1/tests/data/dummy_contract/
+-rw-r--r--   0 root         (0) root         (0)      881 2022-06-01 11:11:15.000000 open-aea-ledger-cosmos-1.9.0.post1/tests/data/dummy_contract/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:22.372564 open-aea-ledger-cosmos-1.9.0.post1/tests/data/dummy_contract/build/
+-rw-r--r--   0 root         (0) root         (0)   120902 2022-06-01 11:11:15.000000 open-aea-ledger-cosmos-1.9.0.post1/tests/data/dummy_contract/build/some.json
+-rw-r--r--   0 root         (0) root         (0)   220992 2022-05-13 16:38:39.000000 open-aea-ledger-cosmos-1.9.0.post1/tests/data/dummy_contract/build/some.wasm
+-rw-r--r--   0 root         (0) root         (0)     1166 2022-06-01 11:11:15.000000 open-aea-ledger-cosmos-1.9.0.post1/tests/data/dummy_contract/contract.py
+-rw-r--r--   0 root         (0) root         (0)      640 2022-06-01 11:11:15.000000 open-aea-ledger-cosmos-1.9.0.post1/tests/data/dummy_contract/contract.yaml
+-rw-r--r--   0 root         (0) root         (0)     9564 2022-06-01 11:11:15.000000 open-aea-ledger-cosmos-1.9.0.post1/tests/test_cosmos.py
```

### Comparing `open-aea-ledger-cosmos-1.9.0/LICENSE` & `open-aea-ledger-cosmos-1.9.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-cosmos-1.9.0/PKG-INFO` & `open-aea-ledger-cosmos-1.9.0.post1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-cosmos
-Version: 1.9.0
+Version: 1.9.0.post1
 Summary: Python package wrapping the public and private key cryptography and ledger api of Cosmos.
 Home-page: UNKNOWN
 Author: Valory AG
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `open-aea-ledger-cosmos-1.9.0/aea_ledger_cosmos/__init__.py` & `open-aea-ledger-cosmos-1.9.0.post1/aea_ledger_cosmos/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-cosmos-1.9.0/aea_ledger_cosmos/cosmos.py` & `open-aea-ledger-cosmos-1.9.0.post1/aea_ledger_cosmos/cosmos.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-cosmos-1.9.0/open_aea_ledger_cosmos.egg-info/PKG-INFO` & `open-aea-ledger-cosmos-1.9.0.post1/open_aea_ledger_cosmos.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-cosmos
-Version: 1.9.0
+Version: 1.9.0.post1
 Summary: Python package wrapping the public and private key cryptography and ledger api of Cosmos.
 Home-page: UNKNOWN
 Author: Valory AG
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `open-aea-ledger-cosmos-1.9.0/open_aea_ledger_cosmos.egg-info/SOURCES.txt` & `open-aea-ledger-cosmos-1.9.0.post1/open_aea_ledger_cosmos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-cosmos-1.9.0/setup.py` & `open-aea-ledger-cosmos-1.9.0.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 """Setup script for "aea_ledger_cosmos" package."""
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="open-aea-ledger-cosmos",
-    version="1.9.0",
+    version="1.9.0.post1",
     author="Valory AG",
     license="Apache-2.0",
     description="Python package wrapping the public and private key cryptography and ledger api of Cosmos.",
     packages=find_packages(include=["aea_ledger_cosmos*"]),
     install_requires=[
         "open-aea>=1.0.0, <2.0.0",
         "ecdsa>=0.15,<0.17.0",
```

### Comparing `open-aea-ledger-cosmos-1.9.0/tests/__init__.py` & `open-aea-ledger-cosmos-1.9.0.post1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-cosmos-1.9.0/tests/conftest.py` & `open-aea-ledger-cosmos-1.9.0.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-cosmos-1.9.0/tests/data/dummy_contract/__init__.py` & `open-aea-ledger-cosmos-1.9.0.post1/tests/data/dummy_contract/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-cosmos-1.9.0/tests/data/dummy_contract/build/some.json` & `open-aea-ledger-cosmos-1.9.0.post1/tests/data/dummy_contract/build/some.json`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-cosmos-1.9.0/tests/data/dummy_contract/build/some.wasm` & `open-aea-ledger-cosmos-1.9.0.post1/tests/data/dummy_contract/build/some.wasm`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-cosmos-1.9.0/tests/data/dummy_contract/contract.py` & `open-aea-ledger-cosmos-1.9.0.post1/tests/data/dummy_contract/contract.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-cosmos-1.9.0/tests/data/dummy_contract/contract.yaml` & `open-aea-ledger-cosmos-1.9.0.post1/tests/data/dummy_contract/contract.yaml`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-cosmos-1.9.0/tests/test_cosmos.py` & `open-aea-ledger-cosmos-1.9.0.post1/tests/test_cosmos.py`

 * *Files identical despite different names*

