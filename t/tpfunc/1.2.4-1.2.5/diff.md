# Comparing `tmp/tpfunc-1.2.4.tar.gz` & `tmp/tpfunc-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpfunc-1.2.4.tar", last modified: Thu Apr 20 07:36:00 2023, max compression
+gzip compressed data, was "tpfunc-1.2.5.tar", last modified: Wed May  3 07:26:11 2023, max compression
```

## Comparing `tpfunc-1.2.4.tar` & `tpfunc-1.2.5.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:36:00.217606 tpfunc-1.2.4/
--rw-r--r--   0 root         (0) root         (0)     1256 2023-04-20 07:36:00.217606 tpfunc-1.2.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-20 07:35:51.000000 tpfunc-1.2.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 07:36:00.217606 tpfunc-1.2.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-04-20 07:35:51.000000 tpfunc-1.2.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:36:00.217606 tpfunc-1.2.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:36:00.217606 tpfunc-1.2.4/src/thingspro/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 07:35:51.000000 tpfunc-1.2.4/src/thingspro/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:36:00.217606 tpfunc-1.2.4/src/thingspro/edge/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 07:35:51.000000 tpfunc-1.2.4/src/thingspro/edge/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:36:00.217606 tpfunc-1.2.4/src/thingspro/edge/api_v1/
--rwxrwxrwx   0 root         (0) root         (0)       42 2023-04-20 07:35:51.000000 tpfunc-1.2.4/src/thingspro/edge/api_v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1951 2023-04-20 07:35:51.000000 tpfunc-1.2.4/src/thingspro/edge/api_v1/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:36:00.217606 tpfunc-1.2.4/src/thingspro/edge/func_v1/
--rwxrwxrwx   0 root         (0) root         (0)       42 2023-04-20 07:35:51.000000 tpfunc-1.2.4/src/thingspro/edge/func_v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2913 2023-04-20 07:35:51.000000 tpfunc-1.2.4/src/thingspro/edge/func_v1/datadriven.py
--rw-rw-rw-   0 root         (0) root         (0)     3151 2023-04-20 07:35:51.000000 tpfunc-1.2.4/src/thingspro/edge/func_v1/package.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:36:00.217606 tpfunc-1.2.4/src/thingspro/edge/http_v1/
--rwxrwxrwx   0 root         (0) root         (0)       42 2023-04-20 07:35:51.000000 tpfunc-1.2.4/src/thingspro/edge/http_v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7967 2023-04-20 07:35:51.000000 tpfunc-1.2.4/src/thingspro/edge/http_v1/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:36:00.217606 tpfunc-1.2.4/src/thingspro/edge/tag_v1/
--rwxrwxrwx   0 root         (0) root         (0)       42 2023-04-20 07:35:51.000000 tpfunc-1.2.4/src/thingspro/edge/tag_v1/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    11410 2023-04-20 07:35:51.000000 tpfunc-1.2.4/src/thingspro/edge/tag_v1/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:36:00.217606 tpfunc-1.2.4/src/tpfunc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1256 2023-04-20 07:36:00.000000 tpfunc-1.2.4/src/tpfunc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      578 2023-04-20 07:36:00.000000 tpfunc-1.2.4/src/tpfunc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 07:36:00.000000 tpfunc-1.2.4/src/tpfunc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-20 07:36:00.000000 tpfunc-1.2.4/src/tpfunc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-20 07:36:00.000000 tpfunc-1.2.4/src/tpfunc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:26:11.142226 tpfunc-1.2.5/
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-05-03 07:26:11.142226 tpfunc-1.2.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-05-03 07:26:00.000000 tpfunc-1.2.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 07:26:11.142226 tpfunc-1.2.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-05-03 07:26:00.000000 tpfunc-1.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:26:11.142226 tpfunc-1.2.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:26:11.142226 tpfunc-1.2.5/src/thingspro/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 07:26:00.000000 tpfunc-1.2.5/src/thingspro/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:26:11.142226 tpfunc-1.2.5/src/thingspro/edge/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 07:26:00.000000 tpfunc-1.2.5/src/thingspro/edge/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:26:11.142226 tpfunc-1.2.5/src/thingspro/edge/api_v1/
+-rwxrwxrwx   0 root         (0) root         (0)       42 2023-05-03 07:26:00.000000 tpfunc-1.2.5/src/thingspro/edge/api_v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1951 2023-05-03 07:26:00.000000 tpfunc-1.2.5/src/thingspro/edge/api_v1/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:26:11.142226 tpfunc-1.2.5/src/thingspro/edge/func_v1/
+-rwxrwxrwx   0 root         (0) root         (0)       42 2023-05-03 07:26:00.000000 tpfunc-1.2.5/src/thingspro/edge/func_v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2913 2023-05-03 07:26:00.000000 tpfunc-1.2.5/src/thingspro/edge/func_v1/datadriven.py
+-rw-rw-rw-   0 root         (0) root         (0)     3151 2023-05-03 07:26:00.000000 tpfunc-1.2.5/src/thingspro/edge/func_v1/package.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:26:11.142226 tpfunc-1.2.5/src/thingspro/edge/http_v1/
+-rwxrwxrwx   0 root         (0) root         (0)       42 2023-05-03 07:26:00.000000 tpfunc-1.2.5/src/thingspro/edge/http_v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7967 2023-05-03 07:26:00.000000 tpfunc-1.2.5/src/thingspro/edge/http_v1/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:26:11.142226 tpfunc-1.2.5/src/thingspro/edge/http_v1/rpc/
+-rw-rw-rw-   0 root         (0) root         (0)     8191 2023-05-03 07:26:00.000000 tpfunc-1.2.5/src/thingspro/edge/http_v1/rpc/reverseproxy_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3851 2023-05-03 07:26:00.000000 tpfunc-1.2.5/src/thingspro/edge/http_v1/rpc/reverseproxy_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:26:11.142226 tpfunc-1.2.5/src/thingspro/edge/tag_v1/
+-rwxrwxrwx   0 root         (0) root         (0)       42 2023-05-03 07:26:00.000000 tpfunc-1.2.5/src/thingspro/edge/tag_v1/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11410 2023-05-03 07:26:00.000000 tpfunc-1.2.5/src/thingspro/edge/tag_v1/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:26:11.142226 tpfunc-1.2.5/src/tpfunc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-05-03 07:26:11.000000 tpfunc-1.2.5/src/tpfunc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      685 2023-05-03 07:26:11.000000 tpfunc-1.2.5/src/tpfunc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 07:26:11.000000 tpfunc-1.2.5/src/tpfunc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-05-03 07:26:11.000000 tpfunc-1.2.5/src/tpfunc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-03 07:26:11.000000 tpfunc-1.2.5/src/tpfunc.egg-info/top_level.txt
```

### Comparing `tpfunc-1.2.4/PKG-INFO` & `tpfunc-1.2.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpfunc
-Version: 1.2.4
+Version: 1.2.5
 Summary: ThingsPro Edge Function SDK
 Home-page: https://github.com/MOXA-ISD/edge-thingspro-function
 Author: Justin Tung
 Author-email: justincp.tung@moxa.com
 License: UNKNOWN
 Description: # ThingsPro Edge Function SDK
         
@@ -15,23 +15,32 @@
           - Direct Access
         - Http Server (v1)
           - Get
           - Post
           - Put
           - Delete
         
-        Besides, SDK written in Python3.5, theoretically compatible with all other modules which you can refer to [Python3.5 official website](https://docs.python.org/3.5/library/index.html).
+        Besides, SDK is tested with Python3.6, theoretically compatible with all other modules which you can refer to [Python3.6 official website](https://docs.python.org/3.6/library/index.html). Python3.5 is no longer in the support list.
         
         # Release Note
+        ## 2023-05-03 V1.2.5
+        ### Bug Fix:
+        - fix: http function missing essential module folder
+        
+        ## 2023-04-26 V1.2.4
+        ### Features:
+        - feat: support unsubscribe all
+        
         ## 2021-07-26 V1.2.3
         ### Bug Fix:
         - fix: can't receive messages after tag_v1 subscribe callback exception
         
         ## 2021-07-23 V1.2.2
         ### Bug Fix:
         - fix: tag_v1 subscribe init always run into exception
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `tpfunc-1.2.4/README.md` & `tpfunc-1.2.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -7,17 +7,25 @@
   - Direct Access
 - Http Server (v1)
   - Get
   - Post
   - Put
   - Delete
 
-Besides, SDK written in Python3.5, theoretically compatible with all other modules which you can refer to [Python3.5 official website](https://docs.python.org/3.5/library/index.html).
+Besides, SDK is tested with Python3.6, theoretically compatible with all other modules which you can refer to [Python3.6 official website](https://docs.python.org/3.6/library/index.html). Python3.5 is no longer in the support list.
 
 # Release Note
+## 2023-05-03 V1.2.5
+### Bug Fix:
+- fix: http function missing essential module folder
+
+## 2023-04-26 V1.2.4
+### Features:
+- feat: support unsubscribe all
+
 ## 2021-07-26 V1.2.3
 ### Bug Fix:
 - fix: can't receive messages after tag_v1 subscribe callback exception
 
 ## 2021-07-23 V1.2.2
 ### Bug Fix:
-- fix: tag_v1 subscribe init always run into exception
+- fix: tag_v1 subscribe init always run into exception
```

### Comparing `tpfunc-1.2.4/setup.py` & `tpfunc-1.2.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tpfunc", # Replace with your own username
-    version="1.2.4",
+    version="1.2.5",
     author="Justin Tung",
     author_email="justincp.tung@moxa.com",
     description="ThingsPro Edge Function SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MOXA-ISD/edge-thingspro-function",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     package_dir={"": "src"},
-    packages=setuptools.find_packages(where="src"),
+    packages=setuptools.find_packages(where="src") + ["thingspro.edge.http_v1.rpc"],
     install_requires=[
         'grpcio',
         'requests',
         'protobuf',
     ]
 )
```

### Comparing `tpfunc-1.2.4/src/thingspro/edge/api_v1/api.py` & `tpfunc-1.2.5/src/thingspro/edge/api_v1/api.py`

 * *Files identical despite different names*

### Comparing `tpfunc-1.2.4/src/thingspro/edge/func_v1/datadriven.py` & `tpfunc-1.2.5/src/thingspro/edge/func_v1/datadriven.py`

 * *Files identical despite different names*

### Comparing `tpfunc-1.2.4/src/thingspro/edge/func_v1/package.py` & `tpfunc-1.2.5/src/thingspro/edge/func_v1/package.py`

 * *Files identical despite different names*

### Comparing `tpfunc-1.2.4/src/thingspro/edge/http_v1/http.py` & `tpfunc-1.2.5/src/thingspro/edge/http_v1/http.py`

 * *Files identical despite different names*

### Comparing `tpfunc-1.2.4/src/thingspro/edge/tag_v1/tag.py` & `tpfunc-1.2.5/src/thingspro/edge/tag_v1/tag.py`

 * *Files identical despite different names*

### Comparing `tpfunc-1.2.4/src/tpfunc.egg-info/PKG-INFO` & `tpfunc-1.2.5/src/tpfunc.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpfunc
-Version: 1.2.4
+Version: 1.2.5
 Summary: ThingsPro Edge Function SDK
 Home-page: https://github.com/MOXA-ISD/edge-thingspro-function
 Author: Justin Tung
 Author-email: justincp.tung@moxa.com
 License: UNKNOWN
 Description: # ThingsPro Edge Function SDK
         
@@ -15,23 +15,32 @@
           - Direct Access
         - Http Server (v1)
           - Get
           - Post
           - Put
           - Delete
         
-        Besides, SDK written in Python3.5, theoretically compatible with all other modules which you can refer to [Python3.5 official website](https://docs.python.org/3.5/library/index.html).
+        Besides, SDK is tested with Python3.6, theoretically compatible with all other modules which you can refer to [Python3.6 official website](https://docs.python.org/3.6/library/index.html). Python3.5 is no longer in the support list.
         
         # Release Note
+        ## 2023-05-03 V1.2.5
+        ### Bug Fix:
+        - fix: http function missing essential module folder
+        
+        ## 2023-04-26 V1.2.4
+        ### Features:
+        - feat: support unsubscribe all
+        
         ## 2021-07-26 V1.2.3
         ### Bug Fix:
         - fix: can't receive messages after tag_v1 subscribe callback exception
         
         ## 2021-07-23 V1.2.2
         ### Bug Fix:
         - fix: tag_v1 subscribe init always run into exception
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `tpfunc-1.2.4/src/tpfunc.egg-info/SOURCES.txt` & `tpfunc-1.2.5/src/tpfunc.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 src/thingspro/edge/api_v1/__init__.py
 src/thingspro/edge/api_v1/api.py
 src/thingspro/edge/func_v1/__init__.py
 src/thingspro/edge/func_v1/datadriven.py
 src/thingspro/edge/func_v1/package.py
 src/thingspro/edge/http_v1/__init__.py
 src/thingspro/edge/http_v1/http.py
+src/thingspro/edge/http_v1/rpc/reverseproxy_pb2.py
+src/thingspro/edge/http_v1/rpc/reverseproxy_pb2_grpc.py
 src/thingspro/edge/tag_v1/__init__.py
 src/thingspro/edge/tag_v1/tag.py
 src/tpfunc.egg-info/PKG-INFO
 src/tpfunc.egg-info/SOURCES.txt
 src/tpfunc.egg-info/dependency_links.txt
 src/tpfunc.egg-info/requires.txt
 src/tpfunc.egg-info/top_level.txt
```

