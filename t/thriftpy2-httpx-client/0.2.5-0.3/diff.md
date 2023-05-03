# Comparing `tmp/thriftpy2-httpx-client-0.2.5.tar.gz` & `tmp/thriftpy2-httpx-client-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thriftpy2-httpx-client-0.2.5.tar", last modified: Tue May 24 06:18:46 2022, max compression
+gzip compressed data, was "thriftpy2-httpx-client-0.3.tar", last modified: Wed May  3 06:34:28 2023, max compression
```

## Comparing `thriftpy2-httpx-client-0.2.5.tar` & `thriftpy2-httpx-client-0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 06:18:46.601245 thriftpy2-httpx-client-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-05-24 06:18:40.000000 thriftpy2-httpx-client-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-05-24 06:18:40.000000 thriftpy2-httpx-client-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2869 2022-05-24 06:18:46.601245 thriftpy2-httpx-client-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1899 2022-05-24 06:18:40.000000 thriftpy2-httpx-client-0.2.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2072 2022-05-24 06:18:46.605245 thriftpy2-httpx-client-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-05-24 06:18:40.000000 thriftpy2-httpx-client-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 06:18:46.601245 thriftpy2-httpx-client-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-24 06:18:40.000000 thriftpy2-httpx-client-0.2.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2719 2022-05-24 06:18:40.000000 thriftpy2-httpx-client-0.2.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 06:18:46.601245 thriftpy2-httpx-client-0.2.5/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-05-24 06:18:40.000000 thriftpy2-httpx-client-0.2.5/tests/resources/addressbook.thrift
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-05-24 06:18:40.000000 thriftpy2-httpx-client-0.2.5/tests/resources/container.thrift
--rw-r--r--   0 runner    (1001) docker     (121)     2684 2022-05-24 06:18:40.000000 thriftpy2-httpx-client-0.2.5/tests/test_aio.py
--rw-r--r--   0 runner    (1001) docker     (121)     2101 2022-05-24 06:18:40.000000 thriftpy2-httpx-client-0.2.5/tests/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 06:18:46.605245 thriftpy2-httpx-client-0.2.5/thriftpy2_httpx_client/
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-05-24 06:18:40.000000 thriftpy2-httpx-client-0.2.5/thriftpy2_httpx_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-05-24 06:18:46.605245 thriftpy2-httpx-client-0.2.5/thriftpy2_httpx_client/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 06:18:46.601245 thriftpy2-httpx-client-0.2.5/thriftpy2_httpx_client/aio/
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-05-24 06:18:40.000000 thriftpy2-httpx-client-0.2.5/thriftpy2_httpx_client/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2351 2022-05-24 06:18:40.000000 thriftpy2-httpx-client-0.2.5/thriftpy2_httpx_client/aio/rpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     3478 2022-05-24 06:18:40.000000 thriftpy2-httpx-client-0.2.5/thriftpy2_httpx_client/aio/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 06:18:46.601245 thriftpy2-httpx-client-0.2.5/thriftpy2_httpx_client/sync/
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-05-24 06:18:40.000000 thriftpy2-httpx-client-0.2.5/thriftpy2_httpx_client/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2572 2022-05-24 06:18:40.000000 thriftpy2-httpx-client-0.2.5/thriftpy2_httpx_client/sync/rpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     3645 2022-05-24 06:18:40.000000 thriftpy2-httpx-client-0.2.5/thriftpy2_httpx_client/sync/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 06:18:46.601245 thriftpy2-httpx-client-0.2.5/thriftpy2_httpx_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2869 2022-05-24 06:18:46.000000 thriftpy2-httpx-client-0.2.5/thriftpy2_httpx_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-05-24 06:18:46.000000 thriftpy2-httpx-client-0.2.5/thriftpy2_httpx_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-24 06:18:46.000000 thriftpy2-httpx-client-0.2.5/thriftpy2_httpx_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-05-24 06:18:46.000000 thriftpy2-httpx-client-0.2.5/thriftpy2_httpx_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-05-24 06:18:46.000000 thriftpy2-httpx-client-0.2.5/thriftpy2_httpx_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2022-05-24 06:18:40.000000 thriftpy2-httpx-client-0.2.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:34:28.662552 thriftpy2-httpx-client-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-03 06:34:23.000000 thriftpy2-httpx-client-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-03 06:34:23.000000 thriftpy2-httpx-client-0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-03 06:34:28.662552 thriftpy2-httpx-client-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-03 06:34:23.000000 thriftpy2-httpx-client-0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-03 06:34:28.666552 thriftpy2-httpx-client-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-03 06:34:23.000000 thriftpy2-httpx-client-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:34:28.662552 thriftpy2-httpx-client-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:34:23.000000 thriftpy2-httpx-client-0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-03 06:34:23.000000 thriftpy2-httpx-client-0.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:34:28.662552 thriftpy2-httpx-client-0.3/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-03 06:34:23.000000 thriftpy2-httpx-client-0.3/tests/resources/addressbook.thrift
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-03 06:34:23.000000 thriftpy2-httpx-client-0.3/tests/resources/container.thrift
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-03 06:34:23.000000 thriftpy2-httpx-client-0.3/tests/test_aio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-03 06:34:23.000000 thriftpy2-httpx-client-0.3/tests/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:34:28.666552 thriftpy2-httpx-client-0.3/thriftpy2_httpx_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-03 06:34:23.000000 thriftpy2-httpx-client-0.3/thriftpy2_httpx_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-03 06:34:28.666552 thriftpy2-httpx-client-0.3/thriftpy2_httpx_client/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:34:28.662552 thriftpy2-httpx-client-0.3/thriftpy2_httpx_client/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-03 06:34:23.000000 thriftpy2-httpx-client-0.3/thriftpy2_httpx_client/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-03 06:34:23.000000 thriftpy2-httpx-client-0.3/thriftpy2_httpx_client/aio/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-03 06:34:23.000000 thriftpy2-httpx-client-0.3/thriftpy2_httpx_client/aio/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:34:28.662552 thriftpy2-httpx-client-0.3/thriftpy2_httpx_client/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-03 06:34:23.000000 thriftpy2-httpx-client-0.3/thriftpy2_httpx_client/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-03 06:34:23.000000 thriftpy2-httpx-client-0.3/thriftpy2_httpx_client/sync/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-05-03 06:34:23.000000 thriftpy2-httpx-client-0.3/thriftpy2_httpx_client/sync/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:34:28.662552 thriftpy2-httpx-client-0.3/thriftpy2_httpx_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-03 06:34:28.000000 thriftpy2-httpx-client-0.3/thriftpy2_httpx_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-03 06:34:28.000000 thriftpy2-httpx-client-0.3/thriftpy2_httpx_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:34:28.000000 thriftpy2-httpx-client-0.3/thriftpy2_httpx_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-03 06:34:28.000000 thriftpy2-httpx-client-0.3/thriftpy2_httpx_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 06:34:28.000000 thriftpy2-httpx-client-0.3/thriftpy2_httpx_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-05-03 06:34:23.000000 thriftpy2-httpx-client-0.3/versioneer.py
```

### Comparing `thriftpy2-httpx-client-0.2.5/LICENSE` & `thriftpy2-httpx-client-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thriftpy2-httpx-client-0.2.5/PKG-INFO` & `thriftpy2-httpx-client-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: thriftpy2-httpx-client
-Version: 0.2.5
+Version: 0.3
 Summary: HTTPX Client for ThriftPy2
 Home-page: https://github.com/aiudirog/ThriftPy2-HTTPX-Client
 Author: Roger Aiudi
 Author-email: aiudirog@gmail.com
 License: MIT
 Keywords: thrift,async,asyncio,httpx
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: all
 License-File: LICENSE
 
 ThriftPy2 HTTPX Client
 ======================
```

### Comparing `thriftpy2-httpx-client-0.2.5/README.rst` & `thriftpy2-httpx-client-0.3/README.rst`

 * *Files identical despite different names*

### Comparing `thriftpy2-httpx-client-0.2.5/setup.cfg` & `thriftpy2-httpx-client-0.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -6,43 +6,42 @@
 author_email = aiudirog@gmail.com
 url = https://github.com/aiudirog/ThriftPy2-HTTPX-Client
 license = MIT
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Software Development :: Libraries :: Python Modules
 keywords = 
 	thrift
 	async
 	asyncio
 	httpx
 
 [options]
-python_requires = >=3.6
+python_requires = >=3.7
 include_package_data = True
 packages = find:
 install_requires = 
 	thriftpy2>=0.4.11
-	httpx>=0.16,<0.24
+	httpx>=0.16,<0.25
 	typing_extensions; python_version < '3.8'
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-asyncio
 	urllib3
-	async_generator; python_version < '3.7'
 all = 
 	%(test)s
 
 [options.packages.find]
 exclude = 
 	tests
 
@@ -69,22 +68,21 @@
 
 [flake8]
 max-line-length = 80
 filename = **.py
 exclude = tests,build,dist,venv,.tox,*.egg*,coverage,doc,versioneer.py
 
 [tox:tox]
-envlist = py36, py37, py38, py39, py310, pypy3
+envlist = py37, py38, py39, py310, py311, pypy3
 
 [testenv]
 deps = 
 	.
 	pytest
 	pytest-asyncio
-	async_generator
 	urllib3
 commands = 
 	python -m pytest
 
 [versioneer]
 VCS = git
 style = pep440
```

### Comparing `thriftpy2-httpx-client-0.2.5/tests/conftest.py` & `thriftpy2-httpx-client-0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-httpx-client-0.2.5/tests/resources/addressbook.thrift` & `thriftpy2-httpx-client-0.3/tests/resources/addressbook.thrift`

 * *Files identical despite different names*

### Comparing `thriftpy2-httpx-client-0.2.5/tests/test_aio.py` & `thriftpy2-httpx-client-0.3/tests/test_aio.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,18 +9,15 @@
 from thriftpy2.thrift import TApplicationException
 from thriftpy2.contrib.aio.client import TAsyncClient
 
 from thriftpy2_httpx_client.aio import make_client
 
 import addressbook_thrift  # noqa
 
-try:
-    from contextlib import asynccontextmanager
-except ImportError:
-    from async_generator import asynccontextmanager
+from contextlib import asynccontextmanager
 
 
 @asynccontextmanager
 async def client(timeout: Real = 3) -> TAsyncClient:
     c = await make_client(
         addressbook_thrift.AddressBookService,
         host="127.0.0.1",
```

### Comparing `thriftpy2-httpx-client-0.2.5/tests/test_sync.py` & `thriftpy2-httpx-client-0.3/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-httpx-client-0.2.5/thriftpy2_httpx_client/aio/rpc.py` & `thriftpy2-httpx-client-0.3/thriftpy2_httpx_client/aio/rpc.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-httpx-client-0.2.5/thriftpy2_httpx_client/aio/transport.py` & `thriftpy2-httpx-client-0.3/thriftpy2_httpx_client/aio/transport.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-httpx-client-0.2.5/thriftpy2_httpx_client/sync/rpc.py` & `thriftpy2-httpx-client-0.3/thriftpy2_httpx_client/sync/rpc.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-httpx-client-0.2.5/thriftpy2_httpx_client/sync/transport.py` & `thriftpy2-httpx-client-0.3/thriftpy2_httpx_client/sync/transport.py`

 * *Files identical despite different names*

### Comparing `thriftpy2-httpx-client-0.2.5/thriftpy2_httpx_client.egg-info/PKG-INFO` & `thriftpy2-httpx-client-0.3/thriftpy2_httpx_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: thriftpy2-httpx-client
-Version: 0.2.5
+Version: 0.3
 Summary: HTTPX Client for ThriftPy2
 Home-page: https://github.com/aiudirog/ThriftPy2-HTTPX-Client
 Author: Roger Aiudi
 Author-email: aiudirog@gmail.com
 License: MIT
 Keywords: thrift,async,asyncio,httpx
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: all
 License-File: LICENSE
 
 ThriftPy2 HTTPX Client
 ======================
```

### Comparing `thriftpy2-httpx-client-0.2.5/thriftpy2_httpx_client.egg-info/SOURCES.txt` & `thriftpy2-httpx-client-0.3/thriftpy2_httpx_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `thriftpy2-httpx-client-0.2.5/versioneer.py` & `thriftpy2-httpx-client-0.3/versioneer.py`

 * *Files identical despite different names*

