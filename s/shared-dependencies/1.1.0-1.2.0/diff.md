# Comparing `tmp/shared_dependencies-1.1.0.tar.gz` & `tmp/shared_dependencies-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shared_dependencies-1.1.0.tar", max compression
+gzip compressed data, was "shared_dependencies-1.2.0.tar", max compression
```

## Comparing `shared_dependencies-1.1.0.tar` & `shared_dependencies-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1164 2023-04-19 11:50:02.909742 shared_dependencies-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-19 11:50:02.909742 shared_dependencies-1.1.0/src/shared_dependencies/__init__.py
--rw-r--r--   0        0        0     3906 2023-04-19 11:50:02.909742 shared_dependencies-1.1.0/src/shared_dependencies/encrypt.py
--rw-r--r--   0        0        0      617 2023-04-19 11:50:02.909742 shared_dependencies-1.1.0/src/shared_dependencies/fake_redis.py
--rw-r--r--   0        0        0     6225 2023-04-19 11:50:02.909742 shared_dependencies-1.1.0/src/shared_dependencies/func_utils.py
--rw-r--r--   0        0        0     6877 2023-04-19 11:50:02.909742 shared_dependencies-1.1.0/src/shared_dependencies/http_client.py
--rw-r--r--   0        0        0      775 2023-04-19 11:50:02.909742 shared_dependencies-1.1.0/src/shared_dependencies/models.py
--rw-r--r--   0        0        0     1665 2023-04-19 11:50:02.909742 shared_dependencies-1.1.0/src/shared_dependencies/sentry.py
--rw-r--r--   0        0        0     1768 2023-04-19 11:50:02.909742 shared_dependencies-1.1.0/src/shared_dependencies/session.py
--rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 shared_dependencies-1.1.0/setup.py
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 shared_dependencies-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1164 2023-05-03 12:24:32.043669 shared_dependencies-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-03 12:24:32.043669 shared_dependencies-1.2.0/src/shared_dependencies/__init__.py
+-rw-r--r--   0        0        0     3906 2023-05-03 12:24:32.043669 shared_dependencies-1.2.0/src/shared_dependencies/encrypt.py
+-rw-r--r--   0        0        0      617 2023-05-03 12:24:32.043669 shared_dependencies-1.2.0/src/shared_dependencies/fake_redis.py
+-rw-r--r--   0        0        0     6225 2023-05-03 12:24:32.043669 shared_dependencies-1.2.0/src/shared_dependencies/func_utils.py
+-rw-r--r--   0        0        0     6877 2023-05-03 12:24:32.043669 shared_dependencies-1.2.0/src/shared_dependencies/http_client.py
+-rw-r--r--   0        0        0      775 2023-05-03 12:24:32.043669 shared_dependencies-1.2.0/src/shared_dependencies/models.py
+-rw-r--r--   0        0        0     1665 2023-05-03 12:24:32.043669 shared_dependencies-1.2.0/src/shared_dependencies/sentry.py
+-rw-r--r--   0        0        0     1768 2023-05-03 12:24:32.043669 shared_dependencies-1.2.0/src/shared_dependencies/session.py
+-rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 shared_dependencies-1.2.0/setup.py
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 shared_dependencies-1.2.0/PKG-INFO
```

### Comparing `shared_dependencies-1.1.0/pyproject.toml` & `shared_dependencies-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 [tool.poetry]
 name = "shared_dependencies"
-version = "1.1.0"
+version = "1.2.0"
 # Given a version number MAJOR.MINOR.PATCH, increment the:
 # MAJOR version when you make incompatible API changes
 # MINOR version when you add functionality in a backwards compatible manner
 # PATCH version when you make backwards compatible bug fixes
 description = ""
 authors = ["Jean-Charles Bouchaud <jeancharles-b@evidenceb.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.10"
-httpx = "^0.23.1"
+httpx = "^0.24.0"
 colorama = "^0.4.6"
 sentry-sdk = "^1.11.0"
 pure-eval = "^0.2.2"
 executing = "^1.2.0"
 asttokens = "^2.1.0"
 pydantic = {extras = ["dotenv"], version = "^1.10.2"}
 PyJWT = "^2.6.0"
 cryptography = "^40.0.2"
 tenacity = "^8.1.0"
 redis = "^4.3.5"
 pycryptodome = "^3.15.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
-pytest-asyncio = "^0.20.2"
-pytest-httpx = "^0.21.2"
+pytest-asyncio = "^0.21.0"
 python-dotenv = "^0.21.0"
 pytest-annotate = "^1.0.5"
 black = "^23.3.0"
 flake8 = "^6.0.0"
 pre-commit = "^3.2.2"
 freezegun = "^1.2.2"
 pytest-mock = "^3.10.0"
+pytest-httpx = "^0.22.0"
 
 [build-system]
 requires = ["poetry-core>=1.3.2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 100
```

### Comparing `shared_dependencies-1.1.0/src/shared_dependencies/encrypt.py` & `shared_dependencies-1.2.0/src/shared_dependencies/encrypt.py`

 * *Files identical despite different names*

### Comparing `shared_dependencies-1.1.0/src/shared_dependencies/fake_redis.py` & `shared_dependencies-1.2.0/src/shared_dependencies/fake_redis.py`

 * *Files identical despite different names*

### Comparing `shared_dependencies-1.1.0/src/shared_dependencies/func_utils.py` & `shared_dependencies-1.2.0/src/shared_dependencies/func_utils.py`

 * *Files identical despite different names*

### Comparing `shared_dependencies-1.1.0/src/shared_dependencies/http_client.py` & `shared_dependencies-1.2.0/src/shared_dependencies/http_client.py`

 * *Files identical despite different names*

### Comparing `shared_dependencies-1.1.0/src/shared_dependencies/models.py` & `shared_dependencies-1.2.0/src/shared_dependencies/models.py`

 * *Files identical despite different names*

### Comparing `shared_dependencies-1.1.0/src/shared_dependencies/sentry.py` & `shared_dependencies-1.2.0/src/shared_dependencies/sentry.py`

 * *Files identical despite different names*

### Comparing `shared_dependencies-1.1.0/src/shared_dependencies/session.py` & `shared_dependencies-1.2.0/src/shared_dependencies/session.py`

 * *Files identical despite different names*

### Comparing `shared_dependencies-1.1.0/setup.py` & `shared_dependencies-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 
 install_requires = \
 ['PyJWT>=2.6.0,<3.0.0',
  'asttokens>=2.1.0,<3.0.0',
  'colorama>=0.4.6,<0.5.0',
  'cryptography>=40.0.2,<41.0.0',
  'executing>=1.2.0,<2.0.0',
- 'httpx>=0.23.1,<0.24.0',
+ 'httpx>=0.24.0,<0.25.0',
  'pure-eval>=0.2.2,<0.3.0',
  'pycryptodome>=3.15.0,<4.0.0',
  'pydantic[dotenv]>=1.10.2,<2.0.0',
  'redis>=4.3.5,<5.0.0',
  'sentry-sdk>=1.11.0,<2.0.0',
  'tenacity>=8.1.0,<9.0.0']
 
 setup_kwargs = {
     'name': 'shared-dependencies',
-    'version': '1.1.0',
+    'version': '1.2.0',
     'description': '',
     'long_description': 'None',
     'author': 'Jean-Charles Bouchaud',
     'author_email': 'jeancharles-b@evidenceb.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `shared_dependencies-1.1.0/PKG-INFO` & `shared_dependencies-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: shared-dependencies
-Version: 1.1.0
+Version: 1.2.0
 Summary: 
 Author: Jean-Charles Bouchaud
 Author-email: jeancharles-b@evidenceb.com
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: PyJWT (>=2.6.0,<3.0.0)
 Requires-Dist: asttokens (>=2.1.0,<3.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: cryptography (>=40.0.2,<41.0.0)
 Requires-Dist: executing (>=1.2.0,<2.0.0)
-Requires-Dist: httpx (>=0.23.1,<0.24.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: pure-eval (>=0.2.2,<0.3.0)
 Requires-Dist: pycryptodome (>=3.15.0,<4.0.0)
 Requires-Dist: pydantic[dotenv] (>=1.10.2,<2.0.0)
 Requires-Dist: redis (>=4.3.5,<5.0.0)
 Requires-Dist: sentry-sdk (>=1.11.0,<2.0.0)
 Requires-Dist: tenacity (>=8.1.0,<9.0.0)
```

