# Comparing `tmp/open-aea-ledger-fetchai-1.9.0.tar.gz` & `tmp/open-aea-ledger-fetchai-1.9.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-aea-ledger-fetchai-1.9.0.tar", last modified: Thu May 26 17:38:52 2022, max compression
+gzip compressed data, was "open-aea-ledger-fetchai-1.9.0.post1.tar", last modified: Wed Jun  1 12:04:43 2022, max compression
```

## Comparing `open-aea-ledger-fetchai-1.9.0.tar` & `open-aea-ledger-fetchai-1.9.0.post1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:52.497264 open-aea-ledger-fetchai-1.9.0/
--rw-r--r--   0 root         (0) root         (0)    11374 2022-05-26 15:42:34.000000 open-aea-ledger-fetchai-1.9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      101 2022-05-26 15:42:34.000000 open-aea-ledger-fetchai-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      981 2022-05-26 17:38:52.493264 open-aea-ledger-fetchai-1.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      173 2022-05-26 15:42:34.000000 open-aea-ledger-fetchai-1.9.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:52.493264 open-aea-ledger-fetchai-1.9.0/aea_ledger_fetchai/
--rw-r--r--   0 root         (0) root         (0)     1086 2022-05-26 15:42:34.000000 open-aea-ledger-fetchai-1.9.0/aea_ledger_fetchai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58462 2022-05-26 15:42:34.000000 open-aea-ledger-fetchai-1.9.0/aea_ledger_fetchai/_cosmos.py
--rw-r--r--   0 root         (0) root         (0)     3809 2022-05-26 16:13:15.000000 open-aea-ledger-fetchai-1.9.0/aea_ledger_fetchai/fetchai.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:52.493264 open-aea-ledger-fetchai-1.9.0/open_aea_ledger_fetchai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      981 2022-05-26 17:38:52.000000 open-aea-ledger-fetchai-1.9.0/open_aea_ledger_fetchai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2022-05-26 17:38:52.000000 open-aea-ledger-fetchai-1.9.0/open_aea_ledger_fetchai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-26 17:38:52.000000 open-aea-ledger-fetchai-1.9.0/open_aea_ledger_fetchai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      182 2022-05-26 17:38:52.000000 open-aea-ledger-fetchai-1.9.0/open_aea_ledger_fetchai.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       99 2022-05-26 17:38:52.000000 open-aea-ledger-fetchai-1.9.0/open_aea_ledger_fetchai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-05-26 17:38:52.000000 open-aea-ledger-fetchai-1.9.0/open_aea_ledger_fetchai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       90 2022-05-26 15:42:34.000000 open-aea-ledger-fetchai-1.9.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-26 17:38:52.497264 open-aea-ledger-fetchai-1.9.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2535 2022-05-26 17:32:20.000000 open-aea-ledger-fetchai-1.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:52.493264 open-aea-ledger-fetchai-1.9.0/tests/
--rw-r--r--   0 root         (0) root         (0)      873 2022-05-26 15:42:34.000000 open-aea-ledger-fetchai-1.9.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1325 2022-05-26 16:13:15.000000 open-aea-ledger-fetchai-1.9.0/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:52.493264 open-aea-ledger-fetchai-1.9.0/tests/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:52.493264 open-aea-ledger-fetchai-1.9.0/tests/data/dummy_contract/
--rw-r--r--   0 root         (0) root         (0)      881 2022-05-26 15:42:34.000000 open-aea-ledger-fetchai-1.9.0/tests/data/dummy_contract/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:52.493264 open-aea-ledger-fetchai-1.9.0/tests/data/dummy_contract/build/
--rw-r--r--   0 root         (0) root         (0)   120902 2022-05-26 15:42:34.000000 open-aea-ledger-fetchai-1.9.0/tests/data/dummy_contract/build/some.json
--rw-r--r--   0 root         (0) root         (0)   220992 2022-05-13 16:38:39.000000 open-aea-ledger-fetchai-1.9.0/tests/data/dummy_contract/build/some.wasm
--rw-r--r--   0 root         (0) root         (0)     1166 2022-05-26 15:42:34.000000 open-aea-ledger-fetchai-1.9.0/tests/data/dummy_contract/contract.py
--rw-r--r--   0 root         (0) root         (0)      640 2022-05-26 15:42:34.000000 open-aea-ledger-fetchai-1.9.0/tests/data/dummy_contract/contract.yaml
--rw-r--r--   0 root         (0) root         (0)    29050 2022-05-26 15:42:34.000000 open-aea-ledger-fetchai-1.9.0/tests/test_fetchai.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:43.872352 open-aea-ledger-fetchai-1.9.0.post1/
+-rw-r--r--   0 root         (0) root         (0)    11374 2022-06-01 11:11:15.000000 open-aea-ledger-fetchai-1.9.0.post1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      101 2022-06-01 11:11:15.000000 open-aea-ledger-fetchai-1.9.0.post1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      987 2022-06-01 12:04:43.872352 open-aea-ledger-fetchai-1.9.0.post1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      173 2022-06-01 11:11:15.000000 open-aea-ledger-fetchai-1.9.0.post1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:43.872352 open-aea-ledger-fetchai-1.9.0.post1/aea_ledger_fetchai/
+-rw-r--r--   0 root         (0) root         (0)     1086 2022-06-01 11:11:15.000000 open-aea-ledger-fetchai-1.9.0.post1/aea_ledger_fetchai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58462 2022-06-01 11:11:15.000000 open-aea-ledger-fetchai-1.9.0.post1/aea_ledger_fetchai/_cosmos.py
+-rw-r--r--   0 root         (0) root         (0)     3782 2022-06-01 11:11:15.000000 open-aea-ledger-fetchai-1.9.0.post1/aea_ledger_fetchai/fetchai.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:43.872352 open-aea-ledger-fetchai-1.9.0.post1/open_aea_ledger_fetchai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      987 2022-06-01 12:04:43.000000 open-aea-ledger-fetchai-1.9.0.post1/open_aea_ledger_fetchai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2022-06-01 12:04:43.000000 open-aea-ledger-fetchai-1.9.0.post1/open_aea_ledger_fetchai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-01 12:04:43.000000 open-aea-ledger-fetchai-1.9.0.post1/open_aea_ledger_fetchai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      182 2022-06-01 12:04:43.000000 open-aea-ledger-fetchai-1.9.0.post1/open_aea_ledger_fetchai.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       99 2022-06-01 12:04:43.000000 open-aea-ledger-fetchai-1.9.0.post1/open_aea_ledger_fetchai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2022-06-01 12:04:43.000000 open-aea-ledger-fetchai-1.9.0.post1/open_aea_ledger_fetchai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2022-06-01 11:11:15.000000 open-aea-ledger-fetchai-1.9.0.post1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-06-01 12:04:43.872352 open-aea-ledger-fetchai-1.9.0.post1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2541 2022-06-01 12:00:50.000000 open-aea-ledger-fetchai-1.9.0.post1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:43.872352 open-aea-ledger-fetchai-1.9.0.post1/tests/
+-rw-r--r--   0 root         (0) root         (0)      873 2022-06-01 11:11:15.000000 open-aea-ledger-fetchai-1.9.0.post1/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1319 2022-06-01 11:11:15.000000 open-aea-ledger-fetchai-1.9.0.post1/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:43.872352 open-aea-ledger-fetchai-1.9.0.post1/tests/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:43.872352 open-aea-ledger-fetchai-1.9.0.post1/tests/data/dummy_contract/
+-rw-r--r--   0 root         (0) root         (0)      881 2022-06-01 11:11:15.000000 open-aea-ledger-fetchai-1.9.0.post1/tests/data/dummy_contract/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:43.872352 open-aea-ledger-fetchai-1.9.0.post1/tests/data/dummy_contract/build/
+-rw-r--r--   0 root         (0) root         (0)   120902 2022-06-01 11:11:15.000000 open-aea-ledger-fetchai-1.9.0.post1/tests/data/dummy_contract/build/some.json
+-rw-r--r--   0 root         (0) root         (0)   220992 2022-05-13 16:38:39.000000 open-aea-ledger-fetchai-1.9.0.post1/tests/data/dummy_contract/build/some.wasm
+-rw-r--r--   0 root         (0) root         (0)     1166 2022-06-01 11:11:15.000000 open-aea-ledger-fetchai-1.9.0.post1/tests/data/dummy_contract/contract.py
+-rw-r--r--   0 root         (0) root         (0)      640 2022-06-01 11:11:15.000000 open-aea-ledger-fetchai-1.9.0.post1/tests/data/dummy_contract/contract.yaml
+-rw-r--r--   0 root         (0) root         (0)    29050 2022-06-01 11:11:15.000000 open-aea-ledger-fetchai-1.9.0.post1/tests/test_fetchai.py
```

### Comparing `open-aea-ledger-fetchai-1.9.0/LICENSE` & `open-aea-ledger-fetchai-1.9.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-fetchai-1.9.0/PKG-INFO` & `open-aea-ledger-fetchai-1.9.0.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-fetchai
-Version: 1.9.0
+Version: 1.9.0.post1
 Summary: Python package wrapping the public and private key cryptography and ledger API of Fetch.AI.
 Home-page: UNKNOWN
 Author: Valory AG
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `open-aea-ledger-fetchai-1.9.0/aea_ledger_fetchai/__init__.py` & `open-aea-ledger-fetchai-1.9.0.post1/aea_ledger_fetchai/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-fetchai-1.9.0/aea_ledger_fetchai/_cosmos.py` & `open-aea-ledger-fetchai-1.9.0.post1/aea_ledger_fetchai/_cosmos.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-fetchai-1.9.0/aea_ledger_fetchai/fetchai.py` & `open-aea-ledger-fetchai-1.9.0.post1/aea_ledger_fetchai/fetchai.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,18 +30,18 @@
 
 from aea.common import JSONLike
 
 
 _FETCHAI = "fetchai"
 _FETCH = "fetch"
 TESTNET_NAME = "testnet"
-FETCHAI_TESTNET_FAUCET_URL = "https://faucet-capricorn.t-v2-london-c.fetch-ai.com"
-DEFAULT_ADDRESS = "https://rest-capricorn.fetch.ai:443"
+FETCHAI_TESTNET_FAUCET_URL = "https://faucet-dorado.fetch.ai"
+DEFAULT_ADDRESS = "https://rest-dorado.fetch.ai:443"
 DEFAULT_CURRENCY_DENOM = "atestfet"
-DEFAULT_CHAIN_ID = "capricorn-1"
+DEFAULT_CHAIN_ID = "dorado-1"
 
 
 class FetchAIHelper(CosmosHelper):
     """Helper class usable as Mixin for FetchAIApi or as standalone class."""
 
     address_prefix = _FETCH
```

### Comparing `open-aea-ledger-fetchai-1.9.0/open_aea_ledger_fetchai.egg-info/PKG-INFO` & `open-aea-ledger-fetchai-1.9.0.post1/open_aea_ledger_fetchai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-fetchai
-Version: 1.9.0
+Version: 1.9.0.post1
 Summary: Python package wrapping the public and private key cryptography and ledger API of Fetch.AI.
 Home-page: UNKNOWN
 Author: Valory AG
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `open-aea-ledger-fetchai-1.9.0/open_aea_ledger_fetchai.egg-info/SOURCES.txt` & `open-aea-ledger-fetchai-1.9.0.post1/open_aea_ledger_fetchai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-fetchai-1.9.0/setup.py` & `open-aea-ledger-fetchai-1.9.0.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 here = os.path.abspath(os.path.dirname(__file__))
 plugin_dir = os.path.abspath(os.path.join(here, ".."))
 
 setup(
     name="open-aea-ledger-fetchai",
-    version="1.9.0",
+    version="1.9.0.post1",
     author="Valory AG",
     license="Apache-2.0",
     description="Python package wrapping the public and private key cryptography and ledger API of Fetch.AI.",
     packages=find_packages(include=["aea_ledger_fetchai*"]),
     install_requires=[
         "open-aea>=1.0.0, <2.0.0",
         "ecdsa>=0.15,<0.17.0",
```

### Comparing `open-aea-ledger-fetchai-1.9.0/tests/__init__.py` & `open-aea-ledger-fetchai-1.9.0.post1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-fetchai-1.9.0/tests/conftest.py` & `open-aea-ledger-fetchai-1.9.0.post1/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,11 +27,11 @@
 
 CUR_PATH = os.path.dirname(inspect.getfile(inspect.currentframe()))  # type: ignore
 ROOT_DIR = os.path.join(CUR_PATH, "..")
 MAX_FLAKY_RERUNS = 3
 FETCHAI = FetchAICrypto.identifier
 
 
-FETCHAI_DEFAULT_ADDRESS = "https://rest-capricorn.fetch.ai:443"
+FETCHAI_DEFAULT_ADDRESS = "https://rest-dorado.fetch.ai:443"
 FETCHAI_DEFAULT_CURRENCY_DENOM = "atestfet"
-FETCHAI_DEFAULT_CHAIN_ID = "capricorn-1"
+FETCHAI_DEFAULT_CHAIN_ID = "dorado-1"
 FETCHAI_TESTNET_CONFIG = {"address": FETCHAI_DEFAULT_ADDRESS}
```

### Comparing `open-aea-ledger-fetchai-1.9.0/tests/data/dummy_contract/__init__.py` & `open-aea-ledger-fetchai-1.9.0.post1/tests/data/dummy_contract/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-fetchai-1.9.0/tests/data/dummy_contract/build/some.json` & `open-aea-ledger-fetchai-1.9.0.post1/tests/data/dummy_contract/build/some.json`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-fetchai-1.9.0/tests/data/dummy_contract/build/some.wasm` & `open-aea-ledger-fetchai-1.9.0.post1/tests/data/dummy_contract/build/some.wasm`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-fetchai-1.9.0/tests/data/dummy_contract/contract.py` & `open-aea-ledger-fetchai-1.9.0.post1/tests/data/dummy_contract/contract.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-fetchai-1.9.0/tests/data/dummy_contract/contract.yaml` & `open-aea-ledger-fetchai-1.9.0.post1/tests/data/dummy_contract/contract.yaml`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-fetchai-1.9.0/tests/test_fetchai.py` & `open-aea-ledger-fetchai-1.9.0.post1/tests/test_fetchai.py`

 * *Files identical despite different names*

