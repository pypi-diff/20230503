# Comparing `tmp/open-aea-cli-ipfs-1.9.0.tar.gz` & `tmp/open-aea-cli-ipfs-1.9.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-aea-cli-ipfs-1.9.0.tar", last modified: Thu May 26 17:38:04 2022, max compression
+gzip compressed data, was "open-aea-cli-ipfs-1.9.0.post1.tar", last modified: Wed Jun  1 12:04:09 2022, max compression
```

## Comparing `open-aea-cli-ipfs-1.9.0.tar` & `open-aea-cli-ipfs-1.9.0.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:04.121759 open-aea-cli-ipfs-1.9.0/
--rw-r--r--   0 root         (0) root         (0)    11374 2022-05-26 15:42:34.000000 open-aea-cli-ipfs-1.9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       95 2022-05-26 15:42:34.000000 open-aea-cli-ipfs-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      949 2022-05-26 17:38:04.121759 open-aea-cli-ipfs-1.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1126 2022-05-26 15:42:34.000000 open-aea-cli-ipfs-1.9.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:04.121759 open-aea-cli-ipfs-1.9.0/aea_cli_ipfs/
--rw-r--r--   0 root         (0) root         (0)      869 2022-05-26 15:42:34.000000 open-aea-cli-ipfs-1.9.0/aea_cli_ipfs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5821 2022-05-26 15:42:34.000000 open-aea-cli-ipfs-1.9.0/aea_cli_ipfs/core.py
--rw-r--r--   0 root         (0) root         (0)     1450 2022-05-26 15:42:34.000000 open-aea-cli-ipfs-1.9.0/aea_cli_ipfs/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    11210 2022-05-26 15:42:34.000000 open-aea-cli-ipfs-1.9.0/aea_cli_ipfs/ipfs_utils.py
--rw-r--r--   0 root         (0) root         (0)     6069 2022-05-26 15:42:34.000000 open-aea-cli-ipfs-1.9.0/aea_cli_ipfs/registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:04.121759 open-aea-cli-ipfs-1.9.0/open_aea_cli_ipfs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      949 2022-05-26 17:38:04.000000 open-aea-cli-ipfs-1.9.0/open_aea_cli_ipfs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      494 2022-05-26 17:38:04.000000 open-aea-cli-ipfs-1.9.0/open_aea_cli_ipfs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-26 17:38:04.000000 open-aea-cli-ipfs-1.9.0/open_aea_cli_ipfs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2022-05-26 17:38:04.000000 open-aea-cli-ipfs-1.9.0/open_aea_cli_ipfs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       47 2022-05-26 17:38:04.000000 open-aea-cli-ipfs-1.9.0/open_aea_cli_ipfs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-05-26 17:38:04.000000 open-aea-cli-ipfs-1.9.0/open_aea_cli_ipfs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       90 2022-05-26 15:42:34.000000 open-aea-cli-ipfs-1.9.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-26 17:38:04.121759 open-aea-cli-ipfs-1.9.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     2034 2022-05-26 17:32:20.000000 open-aea-cli-ipfs-1.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-26 17:38:04.121759 open-aea-cli-ipfs-1.9.0/tests/
--rw-r--r--   0 root         (0) root         (0)      836 2022-05-26 15:42:34.000000 open-aea-cli-ipfs-1.9.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7329 2022-05-26 15:42:34.000000 open-aea-cli-ipfs-1.9.0/tests/test_aea_cli_ipfs.py
--rw-r--r--   0 root         (0) root         (0)     5000 2022-05-26 15:42:34.000000 open-aea-cli-ipfs-1.9.0/tests/test_registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:09.648688 open-aea-cli-ipfs-1.9.0.post1/
+-rw-r--r--   0 root         (0) root         (0)    11374 2022-06-01 11:11:15.000000 open-aea-cli-ipfs-1.9.0.post1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       95 2022-06-01 11:11:15.000000 open-aea-cli-ipfs-1.9.0.post1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      955 2022-06-01 12:04:09.648688 open-aea-cli-ipfs-1.9.0.post1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1126 2022-06-01 11:11:15.000000 open-aea-cli-ipfs-1.9.0.post1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:09.644688 open-aea-cli-ipfs-1.9.0.post1/aea_cli_ipfs/
+-rw-r--r--   0 root         (0) root         (0)      869 2022-06-01 11:11:15.000000 open-aea-cli-ipfs-1.9.0.post1/aea_cli_ipfs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5821 2022-06-01 11:11:15.000000 open-aea-cli-ipfs-1.9.0.post1/aea_cli_ipfs/core.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2022-06-01 11:11:15.000000 open-aea-cli-ipfs-1.9.0.post1/aea_cli_ipfs/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    11210 2022-06-01 11:11:15.000000 open-aea-cli-ipfs-1.9.0.post1/aea_cli_ipfs/ipfs_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6069 2022-06-01 11:11:15.000000 open-aea-cli-ipfs-1.9.0.post1/aea_cli_ipfs/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:09.644688 open-aea-cli-ipfs-1.9.0.post1/open_aea_cli_ipfs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      955 2022-06-01 12:04:09.000000 open-aea-cli-ipfs-1.9.0.post1/open_aea_cli_ipfs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      494 2022-06-01 12:04:09.000000 open-aea-cli-ipfs-1.9.0.post1/open_aea_cli_ipfs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-01 12:04:09.000000 open-aea-cli-ipfs-1.9.0.post1/open_aea_cli_ipfs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2022-06-01 12:04:09.000000 open-aea-cli-ipfs-1.9.0.post1/open_aea_cli_ipfs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2022-06-01 12:04:09.000000 open-aea-cli-ipfs-1.9.0.post1/open_aea_cli_ipfs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-06-01 12:04:09.000000 open-aea-cli-ipfs-1.9.0.post1/open_aea_cli_ipfs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2022-06-01 11:11:15.000000 open-aea-cli-ipfs-1.9.0.post1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-06-01 12:04:09.648688 open-aea-cli-ipfs-1.9.0.post1/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     2040 2022-06-01 12:00:52.000000 open-aea-cli-ipfs-1.9.0.post1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-01 12:04:09.644688 open-aea-cli-ipfs-1.9.0.post1/tests/
+-rw-r--r--   0 root         (0) root         (0)      836 2022-06-01 11:11:15.000000 open-aea-cli-ipfs-1.9.0.post1/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7329 2022-06-01 11:11:15.000000 open-aea-cli-ipfs-1.9.0.post1/tests/test_aea_cli_ipfs.py
+-rw-r--r--   0 root         (0) root         (0)     5000 2022-06-01 11:11:15.000000 open-aea-cli-ipfs-1.9.0.post1/tests/test_registry.py
```

### Comparing `open-aea-cli-ipfs-1.9.0/LICENSE` & `open-aea-cli-ipfs-1.9.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `open-aea-cli-ipfs-1.9.0/PKG-INFO` & `open-aea-cli-ipfs-1.9.0.post1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-cli-ipfs
-Version: 1.9.0
+Version: 1.9.0.post1
 Summary: CLI extension for open AEA framework wrapping IPFS functionality.
 Home-page: UNKNOWN
 Author: Valory AG
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `open-aea-cli-ipfs-1.9.0/README.md` & `open-aea-cli-ipfs-1.9.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `open-aea-cli-ipfs-1.9.0/aea_cli_ipfs/__init__.py` & `open-aea-cli-ipfs-1.9.0.post1/aea_cli_ipfs/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-ipfs-1.9.0/aea_cli_ipfs/core.py` & `open-aea-cli-ipfs-1.9.0.post1/aea_cli_ipfs/core.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-ipfs-1.9.0/aea_cli_ipfs/exceptions.py` & `open-aea-cli-ipfs-1.9.0.post1/aea_cli_ipfs/exceptions.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-ipfs-1.9.0/aea_cli_ipfs/ipfs_utils.py` & `open-aea-cli-ipfs-1.9.0.post1/aea_cli_ipfs/ipfs_utils.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-ipfs-1.9.0/aea_cli_ipfs/registry.py` & `open-aea-cli-ipfs-1.9.0.post1/aea_cli_ipfs/registry.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-ipfs-1.9.0/open_aea_cli_ipfs.egg-info/PKG-INFO` & `open-aea-cli-ipfs-1.9.0.post1/open_aea_cli_ipfs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-cli-ipfs
-Version: 1.9.0
+Version: 1.9.0.post1
 Summary: CLI extension for open AEA framework wrapping IPFS functionality.
 Home-page: UNKNOWN
 Author: Valory AG
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `open-aea-cli-ipfs-1.9.0/setup.py` & `open-aea-cli-ipfs-1.9.0.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 from setuptools import setup  # type: ignore
 
 
 setup(
     name="open-aea-cli-ipfs",
-    version="1.9.0",
+    version="1.9.0.post1",
     author="Valory AG",
     license="Apache-2.0",
     description="CLI extension for open AEA framework wrapping IPFS functionality.",
     packages=["aea_cli_ipfs"],
     entry_points={"aea.cli": ["ipfs_cli_command = aea_cli_ipfs.core:ipfs"]},
     install_requires=["open-aea>=1.0.0, <2.0.0", "ipfshttpclient>=0.8.0a2"],
     classifiers=[
```

### Comparing `open-aea-cli-ipfs-1.9.0/tests/__init__.py` & `open-aea-cli-ipfs-1.9.0.post1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-ipfs-1.9.0/tests/test_aea_cli_ipfs.py` & `open-aea-cli-ipfs-1.9.0.post1/tests/test_aea_cli_ipfs.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-ipfs-1.9.0/tests/test_registry.py` & `open-aea-cli-ipfs-1.9.0.post1/tests/test_registry.py`

 * *Files identical despite different names*

