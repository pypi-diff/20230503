# Comparing `tmp/dcentrapi-0.1.8.tar.gz` & `tmp/dcentrapi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcentrapi-0.1.8.tar", last modified: Tue Apr  4 11:45:21 2023, max compression
+gzip compressed data, was "dcentrapi-0.1.9.tar", last modified: Wed May  3 13:09:00 2023, max compression
```

## Comparing `dcentrapi-0.1.8.tar` & `dcentrapi-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-04-04 11:45:21.904838 dcentrapi-0.1.8/
--rw-r--r--   0 nivshitrit   (501) staff       (20)     1073 2022-10-09 08:58:27.000000 dcentrapi-0.1.8/LICENSE.rst
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6780 2023-04-04 11:45:21.904706 dcentrapi-0.1.8/PKG-INFO
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6211 2022-10-09 08:58:27.000000 dcentrapi-0.1.8/README.md
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-04-04 11:45:21.903914 dcentrapi-0.1.8/dcentrapi/
--rw-r--r--   0 nivshitrit   (501) staff       (20)      851 2023-03-08 10:39:09.000000 dcentrapi-0.1.8/dcentrapi/Base.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      280 2023-03-08 10:39:09.000000 dcentrapi-0.1.8/dcentrapi/__init__.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)       63 2023-04-04 11:43:09.000000 dcentrapi-0.1.8/dcentrapi/common.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     8172 2023-01-17 14:33:05.000000 dcentrapi-0.1.8/dcentrapi/eventPolling.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      491 2023-03-02 14:02:13.000000 dcentrapi-0.1.8/dcentrapi/gasMonitor.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     3078 2022-11-22 15:13:50.000000 dcentrapi-0.1.8/dcentrapi/merkleTree.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     3140 2023-04-04 11:41:50.000000 dcentrapi-0.1.8/dcentrapi/rpcAggregation.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      823 2023-04-04 11:43:09.000000 dcentrapi-0.1.8/dcentrapi/web3Index.py
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-04-04 11:45:21.904535 dcentrapi-0.1.8/dcentrapi.egg-info/
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6780 2023-04-04 11:45:21.000000 dcentrapi-0.1.8/dcentrapi.egg-info/PKG-INFO
--rw-r--r--   0 nivshitrit   (501) staff       (20)      379 2023-04-04 11:45:21.000000 dcentrapi-0.1.8/dcentrapi.egg-info/SOURCES.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)        1 2023-04-04 11:45:21.000000 dcentrapi-0.1.8/dcentrapi.egg-info/dependency_links.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)        9 2023-04-04 11:45:21.000000 dcentrapi-0.1.8/dcentrapi.egg-info/requires.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)       10 2023-04-04 11:45:21.000000 dcentrapi-0.1.8/dcentrapi.egg-info/top_level.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)       38 2023-04-04 11:45:21.904876 dcentrapi-0.1.8/setup.cfg
--rw-r--r--   0 nivshitrit   (501) staff       (20)     1167 2023-04-04 11:45:09.000000 dcentrapi-0.1.8/setup.py
+drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-05-03 13:09:00.382685 dcentrapi-0.1.9/
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     1073 2022-10-09 08:58:27.000000 dcentrapi-0.1.9/LICENSE.rst
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     6780 2023-05-03 13:09:00.382439 dcentrapi-0.1.9/PKG-INFO
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     6211 2022-10-09 08:58:27.000000 dcentrapi-0.1.9/README.md
+drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-05-03 13:09:00.381141 dcentrapi-0.1.9/dcentrapi/
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      851 2023-03-08 10:39:09.000000 dcentrapi-0.1.9/dcentrapi/Base.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      280 2023-03-08 10:39:09.000000 dcentrapi-0.1.9/dcentrapi/__init__.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)       63 2023-05-03 13:07:56.000000 dcentrapi-0.1.9/dcentrapi/common.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     8597 2023-05-03 13:07:34.000000 dcentrapi-0.1.9/dcentrapi/eventPolling.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      491 2023-03-02 14:02:13.000000 dcentrapi-0.1.9/dcentrapi/gasMonitor.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     3078 2022-11-22 15:13:50.000000 dcentrapi-0.1.9/dcentrapi/merkleTree.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     3140 2023-04-04 11:41:50.000000 dcentrapi-0.1.9/dcentrapi/rpcAggregation.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      823 2023-04-04 11:43:09.000000 dcentrapi-0.1.9/dcentrapi/web3Index.py
+drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-05-03 13:09:00.382194 dcentrapi-0.1.9/dcentrapi.egg-info/
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     6780 2023-05-03 13:09:00.000000 dcentrapi-0.1.9/dcentrapi.egg-info/PKG-INFO
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      379 2023-05-03 13:09:00.000000 dcentrapi-0.1.9/dcentrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)        1 2023-05-03 13:09:00.000000 dcentrapi-0.1.9/dcentrapi.egg-info/dependency_links.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)        9 2023-05-03 13:09:00.000000 dcentrapi-0.1.9/dcentrapi.egg-info/requires.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)       10 2023-05-03 13:09:00.000000 dcentrapi-0.1.9/dcentrapi.egg-info/top_level.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)       38 2023-05-03 13:09:00.382763 dcentrapi-0.1.9/setup.cfg
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     1167 2023-04-09 07:57:53.000000 dcentrapi-0.1.9/setup.py
```

### Comparing `dcentrapi-0.1.8/LICENSE.rst` & `dcentrapi-0.1.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.1.8/PKG-INFO` & `dcentrapi-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.1.8
+Version: 0.1.9
 Summary: Dcentralab Pypi packages
 Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
 Platform: UNKNOWN
```

### Comparing `dcentrapi-0.1.8/README.md` & `dcentrapi-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.1.8/dcentrapi/Base.py` & `dcentrapi-0.1.9/dcentrapi/Base.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.1.8/dcentrapi/eventPolling.py` & `dcentrapi-0.1.9/dcentrapi/eventPolling.py`

 * *Files 3% similar despite different names*

```diff
@@ -195,7 +195,17 @@
     def get_nof_token_transfers(self, contract_addresses):
         url = self.url + "event_polling/token_transfers"
         data = {
             "contract_addresses": contract_addresses
         }
         response = requests.get(url, params=data, headers=self.headers)
         return response.json()
+
+    def get_event_details(self, collection_name, list_of_events, event_parameter):
+        url = self.url + "event_polling/get_event_details"
+        data = {
+                "collection_name": collection_name,
+                "list_of_events": list_of_events,
+                "event_parameter": event_parameter
+        }
+        response = requests.post(url, json=data, headers=self.headers)
+        return response.json()
```

### Comparing `dcentrapi-0.1.8/dcentrapi/merkleTree.py` & `dcentrapi-0.1.9/dcentrapi/merkleTree.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.1.8/dcentrapi/rpcAggregation.py` & `dcentrapi-0.1.9/dcentrapi/rpcAggregation.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.1.8/dcentrapi/web3Index.py` & `dcentrapi-0.1.9/dcentrapi/web3Index.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.1.8/dcentrapi.egg-info/PKG-INFO` & `dcentrapi-0.1.9/dcentrapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.1.8
+Version: 0.1.9
 Summary: Dcentralab Pypi packages
 Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
 Platform: UNKNOWN
```

### Comparing `dcentrapi-0.1.8/setup.py` & `dcentrapi-0.1.9/setup.py`

 * *Files identical despite different names*

