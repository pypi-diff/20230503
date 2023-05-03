# Comparing `tmp/braincube-aws-core-alpha-0.0.14.tar.gz` & `tmp/braincube-aws-core-alpha-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braincube-aws-core-alpha-0.0.14.tar", last modified: Tue May  2 13:52:32 2023, max compression
+gzip compressed data, was "braincube-aws-core-alpha-0.0.15.tar", last modified: Wed May  3 19:12:01 2023, max compression
```

## Comparing `braincube-aws-core-alpha-0.0.14.tar` & `braincube-aws-core-alpha-0.0.15.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 13:52:32.504890 braincube-aws-core-alpha-0.0.14/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 13:41:49.000000 braincube-aws-core-alpha-0.0.14/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     7084 2023-05-02 13:52:32.505195 braincube-aws-core-alpha-0.0.14/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     6134 2023-05-02 13:52:15.000000 braincube-aws-core-alpha-0.0.14/README.md
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-02 13:42:37.000000 braincube-aws-core-alpha-0.0.14/pyproject.toml
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1086 2023-05-02 13:52:32.506249 braincube-aws-core-alpha-0.0.14/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 13:44:20.000000 braincube-aws-core-alpha-0.0.14/setup.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 13:52:32.486788 braincube-aws-core-alpha-0.0.14/src/
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 13:52:32.491874 braincube-aws-core-alpha-0.0.14/src/braincube_aws_core_alpha.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     7084 2023-05-02 13:52:32.000000 braincube-aws-core-alpha-0.0.14/src/braincube_aws_core_alpha.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      733 2023-05-02 13:52:32.000000 braincube-aws-core-alpha-0.0.14/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-02 13:52:32.000000 braincube-aws-core-alpha-0.0.14/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-02 13:52:32.000000 braincube-aws-core-alpha-0.0.14/src/braincube_aws_core_alpha.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-02 13:52:32.000000 braincube-aws-core-alpha-0.0.14/src/braincube_aws_core_alpha.egg-info/top_level.txt
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 13:52:32.492363 braincube-aws-core-alpha-0.0.14/src/core/
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 09:47:38.000000 braincube-aws-core-alpha-0.0.14/src/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 13:52:32.496087 braincube-aws-core-alpha-0.0.14/src/core/dal/
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 09:47:38.000000 braincube-aws-core-alpha-0.0.14/src/core/dal/__init__.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     1289 2023-05-02 09:47:38.000000 braincube-aws-core-alpha-0.0.14/src/core/dal/data.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)      281 2023-05-02 09:47:38.000000 braincube-aws-core-alpha-0.0.14/src/core/dal/database_errors.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     1497 2023-05-02 09:47:38.000000 braincube-aws-core-alpha-0.0.14/src/core/dal/postgres_connection.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)    20547 2023-05-02 09:47:38.000000 braincube-aws-core-alpha-0.0.14/src/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 13:52:32.499205 braincube-aws-core-alpha-0.0.14/src/core/di/
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 09:47:38.000000 braincube-aws-core-alpha-0.0.14/src/core/di/__init__.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)      623 2023-05-02 09:47:38.000000 braincube-aws-core-alpha-0.0.14/src/core/di/data.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     3472 2023-05-02 09:47:38.000000 braincube-aws-core-alpha-0.0.14/src/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 13:52:32.502234 braincube-aws-core-alpha-0.0.14/src/core/rest/
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 09:47:38.000000 braincube-aws-core-alpha-0.0.14/src/core/rest/__init__.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     1112 2023-05-02 09:47:38.000000 braincube-aws-core-alpha-0.0.14/src/core/rest/app_controller.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     3026 2023-05-02 09:47:38.000000 braincube-aws-core-alpha-0.0.14/src/core/rest/app_module.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     3631 2023-05-02 09:47:38.000000 braincube-aws-core-alpha-0.0.14/src/core/rest/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 13:52:32.504262 braincube-aws-core-alpha-0.0.14/src/core/utils/
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 09:47:38.000000 braincube-aws-core-alpha-0.0.14/src/core/utils/__init__.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)      580 2023-05-02 09:47:38.000000 braincube-aws-core-alpha-0.0.14/src/core/utils/convert.py
--rw-rw-r--   0 evangelosboudis   (501) staff       (20)     1111 2023-05-02 09:47:38.000000 braincube-aws-core-alpha-0.0.14/src/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 19:12:01.332219 braincube-aws-core-alpha-0.0.15/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 13:41:49.000000 braincube-aws-core-alpha-0.0.15/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     9298 2023-05-03 19:12:01.332453 braincube-aws-core-alpha-0.0.15/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8348 2023-05-03 19:09:10.000000 braincube-aws-core-alpha-0.0.15/README.md
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-02 13:42:37.000000 braincube-aws-core-alpha-0.0.15/pyproject.toml
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1086 2023-05-03 19:12:01.333741 braincube-aws-core-alpha-0.0.15/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 13:44:20.000000 braincube-aws-core-alpha-0.0.15/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 19:12:01.319860 braincube-aws-core-alpha-0.0.15/src/
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 19:12:01.324077 braincube-aws-core-alpha-0.0.15/src/braincube_aws_core_alpha.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     9298 2023-05-03 19:12:01.000000 braincube-aws-core-alpha-0.0.15/src/braincube_aws_core_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      733 2023-05-03 19:12:01.000000 braincube-aws-core-alpha-0.0.15/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-03 19:12:01.000000 braincube-aws-core-alpha-0.0.15/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-03 19:12:01.000000 braincube-aws-core-alpha-0.0.15/src/braincube_aws_core_alpha.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-03 19:12:01.000000 braincube-aws-core-alpha-0.0.15/src/braincube_aws_core_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 19:12:01.324561 braincube-aws-core-alpha-0.0.15/src/core/
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 16:58:19.000000 braincube-aws-core-alpha-0.0.15/src/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 19:12:01.327113 braincube-aws-core-alpha-0.0.15/src/core/dal/
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 16:58:19.000000 braincube-aws-core-alpha-0.0.15/src/core/dal/__init__.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)     1289 2023-05-03 16:58:19.000000 braincube-aws-core-alpha-0.0.15/src/core/dal/data.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)      281 2023-05-03 16:58:19.000000 braincube-aws-core-alpha-0.0.15/src/core/dal/database_errors.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)     2257 2023-05-03 16:58:19.000000 braincube-aws-core-alpha-0.0.15/src/core/dal/postgres_connection.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)    26355 2023-05-03 16:58:19.000000 braincube-aws-core-alpha-0.0.15/src/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 19:12:01.328515 braincube-aws-core-alpha-0.0.15/src/core/di/
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 16:58:19.000000 braincube-aws-core-alpha-0.0.15/src/core/di/__init__.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)      623 2023-05-03 16:58:19.000000 braincube-aws-core-alpha-0.0.15/src/core/di/data.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)     4235 2023-05-03 16:58:19.000000 braincube-aws-core-alpha-0.0.15/src/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 19:12:01.330513 braincube-aws-core-alpha-0.0.15/src/core/rest/
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 16:58:19.000000 braincube-aws-core-alpha-0.0.15/src/core/rest/__init__.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)     2883 2023-05-03 16:58:19.000000 braincube-aws-core-alpha-0.0.15/src/core/rest/app_controller.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)     3169 2023-05-03 16:58:19.000000 braincube-aws-core-alpha-0.0.15/src/core/rest/app_module.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)     3631 2023-05-03 16:58:19.000000 braincube-aws-core-alpha-0.0.15/src/core/rest/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 19:12:01.331849 braincube-aws-core-alpha-0.0.15/src/core/utils/
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 16:58:19.000000 braincube-aws-core-alpha-0.0.15/src/core/utils/__init__.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)      580 2023-05-03 16:58:19.000000 braincube-aws-core-alpha-0.0.15/src/core/utils/convert.py
+-rw-rw-r--   0 evangelosboudis   (501) staff       (20)     1111 2023-05-03 16:58:19.000000 braincube-aws-core-alpha-0.0.15/src/core/utils/data.py
```

### Comparing `braincube-aws-core-alpha-0.0.14/LICENSE` & `braincube-aws-core-alpha-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.14/PKG-INFO` & `braincube-aws-core-alpha-0.0.15/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,62 +1,95 @@
-Metadata-Version: 2.1
-Name: braincube-aws-core-alpha
-Version: 0.0.14
-Summary: Microframework for python aws lambdas
-Home-page: https://bitbucket.org/braincube-common/core-aws.git
-Author: Braincube
-Author-email: v.boudis@braincube.gr
-License: MIT
-Keywords: python,amazon,aws,lambda,routing,dal,injection
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: <4,>=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# braincube-aws-core
 
-# sam-api
+Microframework for Python AWS lambdas.
 
-### Requirements
+[![Language](https://img.shields.io/badge/language-Python-blue.svg)](https://www.python.org/)
+[![pypi](https://img.shields.io/pypi/v/braincube-aws-core-alpha.svg)](https://pypi.org/project/braincube-aws-core-alpha/)
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
-To use the SAM CLI, you need the following tools.
+## Installation
 
-* [SAM CLI](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-cli-install.html)
-* [Python 3](https://www.python.org/downloads/)
-* [Docker](https://hub.docker.com/search/?type=edition&offering=community)
+```bash
+pip install braincube-aws-core-alpha
+```
 
-### Run server locally
+## Built With
 
-```bash
-# open ssh tunel
-sudo sh ssh_tunnel_Analog_JBox.sh
-# apply code changes to docker image
-sam-api$ sam build
-# start server locally on http://127.0.0.1:3000
-sam-api$ sam local start-api --warm-containers EAGER
-# or run function locally using event.json as parameter
-sam-api$ sam local invoke ApiFunction --event events/event.json
+- [asyncpg](https://github.com/MagicStack/asyncpg) - A fast PostgreSQL Database Client Library for Python/asyncio.
+- [pydantic](https://github.com/pydantic/pydantic) - Data validation using Python type hints.
+- [pypika](https://github.com/kayak/pypika) - Python Query Builder.
+
+### Application Controllers Example
+
+```python
+import asyncio
+
+from http import HTTPStatus
+
+from core.rest.data import HTTPRequest, HTTPResponse
+from core.rest.app_module import AppModule
+from core.rest.app_controller import AppController
+
+from pydantic import BaseModel
+
+
+class AccountDto(BaseModel):
+    id: int
+    iban: str
+    bban: str
+
+
+_accounts = [
+    AccountDto(1, "EUR27100777770209299700", "EURC12345612345678"),
+    AccountDto(2, "GR27100777770209299700", "GRC12345612345678"),
+]
+
+app = AppController("/accounts")
+
+
+@app.get("/{id}")
+async def get_account(request: HTTPRequest) -> HTTPResponse:
+    account = next((a for a in _accounts if a.id == request.path_parameters["id"]), None)
+    return HTTPResponse(HTTPStatus.OK if account else HTTPStatus.NO_CONTENT, account)
+
+
+@app.post()
+async def create_account(request: HTTPRequest[AccountDto]) -> HTTPResponse:
+    return HTTPResponse(HTTPStatus.OK)
+
+
+loop = asyncio.get_event_loop()
+
+module = AppModule([app])
+
+
+def main(event, context):
+    return loop.run_until_complete(module.serve(event, context))
 ```
 
-### Deploy to AWS
+### Dependency Injection Example
 
-```bash
-sam build --use-container
-sam deploy --guided --profile analog_user --region eu-west-1
+```python
+from core.di.injector import inject
+from core.dal.postgres_connection import get_pool, Pool
+
+
+@inject("data_warehouse_pool")
+async def provide_warehouse_pool() -> Pool:
+    return await get_pool()
+
+
+@inject(qualifier="pool:data_warehouse_pool")
+class BankService:
+
+    def __init__(self, pool: Pool):
+        self._pool = pool
 ```
 
-### PostgresRepository usage
+### Postgres Repository Example
 
 ```python
 from core.rest.data import HTTPRequest
 from core.utils.data import Order, OrderType
 from core.dal.data import Key, Schema, Column, Relation, SimpleColumn, JoinType, JoinThrough, StatementField
 from core.dal.postgres_connection import get_pool, Pool
 from core.dal.postgres_repository import PostgresRepository
@@ -186,15 +219,14 @@
     returning_aliases=["id", "name", "type"])
 
 await repo.fetch_raw("SELECT * FROM equities WHERE type = $1 and isin = $2", [1, "TREEGYO00017"])
 
 await repo.fetch_one_raw("SELECT * FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
 
 await repo.execute_raw("DELETE FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
-
 ```
 
 ### Query params format
 
 ```
 fields=name, type, industrySector, isin, bloombergCode, parties_name, parties_shortName
 
@@ -204,14 +236,42 @@
 
 page_no=1
 page_size=50
 top_size=50
 order=name, id DESC
 ```
 
+### Local Development Requirements
+
+To use the SAM CLI, you need the following tools.
+
+* [SAM CLI](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-cli-install.html)
+* [Python 3](https://www.python.org/downloads/)
+* [Docker](https://hub.docker.com/search/?type=edition&offering=community)
+
+### Run server locally
+
+```bash
+# open ssh tunel
+sudo sh ssh_tunnel_Analog_JBox.sh
+# apply code changes to docker image
+sam-api$ sam build
+# start server locally on http://127.0.0.1:3000
+sam-api$ sam local start-api --warm-containers EAGER
+# or run function locally using event.json as parameter
+sam-api$ sam local invoke ApiFunction --event events/event.json
+```
+
+### Deploy to AWS
+
+```bash
+sam build --use-container
+sam deploy --guided --profile analog_user --region eu-west-1
+```
+
 ### Build and deploy new package version using twine
 
 ```bash
 python3 -m pip install --upgrade pip
 python3 -m pip install --upgrade build
 python3 -m pip install --upgrade twine
 ```
```

### Comparing `braincube-aws-core-alpha-0.0.14/setup.cfg` & `braincube-aws-core-alpha-0.0.15/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = braincube-aws-core-alpha
-version = 0.0.14
+version = 0.0.15
 author = Braincube
 author_email = v.boudis@braincube.gr
 description = Microframework for python aws lambdas
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://bitbucket.org/braincube-common/core-aws.git
 license = MIT
```

### Comparing `braincube-aws-core-alpha-0.0.14/src/braincube_aws_core_alpha.egg-info/PKG-INFO` & `braincube-aws-core-alpha-0.0.15/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.14
+Version: 0.0.15
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
@@ -18,45 +18,102 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# sam-api
+# braincube-aws-core
 
-### Requirements
+Microframework for Python AWS lambdas.
 
-To use the SAM CLI, you need the following tools.
-
-* [SAM CLI](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-cli-install.html)
-* [Python 3](https://www.python.org/downloads/)
-* [Docker](https://hub.docker.com/search/?type=edition&offering=community)
+[![Language](https://img.shields.io/badge/language-Python-blue.svg)](https://www.python.org/)
+[![pypi](https://img.shields.io/pypi/v/braincube-aws-core-alpha.svg)](https://pypi.org/project/braincube-aws-core-alpha/)
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
-### Run server locally
+## Installation
 
 ```bash
-# open ssh tunel
-sudo sh ssh_tunnel_Analog_JBox.sh
-# apply code changes to docker image
-sam-api$ sam build
-# start server locally on http://127.0.0.1:3000
-sam-api$ sam local start-api --warm-containers EAGER
-# or run function locally using event.json as parameter
-sam-api$ sam local invoke ApiFunction --event events/event.json
+pip install braincube-aws-core-alpha
 ```
 
-### Deploy to AWS
+## Built With
 
-```bash
-sam build --use-container
-sam deploy --guided --profile analog_user --region eu-west-1
+- [asyncpg](https://github.com/MagicStack/asyncpg) - A fast PostgreSQL Database Client Library for Python/asyncio.
+- [pydantic](https://github.com/pydantic/pydantic) - Data validation using Python type hints.
+- [pypika](https://github.com/kayak/pypika) - Python Query Builder.
+
+### Application Controllers Example
+
+```python
+import asyncio
+
+from http import HTTPStatus
+
+from core.rest.data import HTTPRequest, HTTPResponse
+from core.rest.app_module import AppModule
+from core.rest.app_controller import AppController
+
+from pydantic import BaseModel
+
+
+class AccountDto(BaseModel):
+    id: int
+    iban: str
+    bban: str
+
+
+_accounts = [
+    AccountDto(1, "EUR27100777770209299700", "EURC12345612345678"),
+    AccountDto(2, "GR27100777770209299700", "GRC12345612345678"),
+]
+
+app = AppController("/accounts")
+
+
+@app.get("/{id}")
+async def get_account(request: HTTPRequest) -> HTTPResponse:
+    account = next((a for a in _accounts if a.id == request.path_parameters["id"]), None)
+    return HTTPResponse(HTTPStatus.OK if account else HTTPStatus.NO_CONTENT, account)
+
+
+@app.post()
+async def create_account(request: HTTPRequest[AccountDto]) -> HTTPResponse:
+    return HTTPResponse(HTTPStatus.OK)
+
+
+loop = asyncio.get_event_loop()
+
+module = AppModule([app])
+
+
+def main(event, context):
+    return loop.run_until_complete(module.serve(event, context))
 ```
 
-### PostgresRepository usage
+### Dependency Injection Example
+
+```python
+from core.di.injector import inject
+from core.dal.postgres_connection import get_pool, Pool
+
+
+@inject("data_warehouse_pool")
+async def provide_warehouse_pool() -> Pool:
+    return await get_pool()
+
+
+@inject(qualifier="pool:data_warehouse_pool")
+class BankService:
+
+    def __init__(self, pool: Pool):
+        self._pool = pool
+```
+
+### Postgres Repository Example
 
 ```python
 from core.rest.data import HTTPRequest
 from core.utils.data import Order, OrderType
 from core.dal.data import Key, Schema, Column, Relation, SimpleColumn, JoinType, JoinThrough, StatementField
 from core.dal.postgres_connection import get_pool, Pool
 from core.dal.postgres_repository import PostgresRepository
@@ -186,15 +243,14 @@
     returning_aliases=["id", "name", "type"])
 
 await repo.fetch_raw("SELECT * FROM equities WHERE type = $1 and isin = $2", [1, "TREEGYO00017"])
 
 await repo.fetch_one_raw("SELECT * FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
 
 await repo.execute_raw("DELETE FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
-
 ```
 
 ### Query params format
 
 ```
 fields=name, type, industrySector, isin, bloombergCode, parties_name, parties_shortName
 
@@ -204,14 +260,42 @@
 
 page_no=1
 page_size=50
 top_size=50
 order=name, id DESC
 ```
 
+### Local Development Requirements
+
+To use the SAM CLI, you need the following tools.
+
+* [SAM CLI](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-cli-install.html)
+* [Python 3](https://www.python.org/downloads/)
+* [Docker](https://hub.docker.com/search/?type=edition&offering=community)
+
+### Run server locally
+
+```bash
+# open ssh tunel
+sudo sh ssh_tunnel_Analog_JBox.sh
+# apply code changes to docker image
+sam-api$ sam build
+# start server locally on http://127.0.0.1:3000
+sam-api$ sam local start-api --warm-containers EAGER
+# or run function locally using event.json as parameter
+sam-api$ sam local invoke ApiFunction --event events/event.json
+```
+
+### Deploy to AWS
+
+```bash
+sam build --use-container
+sam deploy --guided --profile analog_user --region eu-west-1
+```
+
 ### Build and deploy new package version using twine
 
 ```bash
 python3 -m pip install --upgrade pip
 python3 -m pip install --upgrade build
 python3 -m pip install --upgrade twine
 ```
```

### Comparing `braincube-aws-core-alpha-0.0.14/src/braincube_aws_core_alpha.egg-info/SOURCES.txt` & `braincube-aws-core-alpha-0.0.15/src/braincube_aws_core_alpha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.14/src/core/dal/data.py` & `braincube-aws-core-alpha-0.0.15/src/core/dal/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.14/src/core/dal/postgres_connection.py` & `braincube-aws-core-alpha-0.0.15/src/core/dal/postgres_connection.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,23 +3,44 @@
 from asyncpg import create_pool, connect, Connection
 from asyncpg.pool import Pool
 
 
 async def get(user: str = os.environ["PG_USER"], password: str = os.environ["PG_PASSWORD"],
               database: str = os.environ["PG_DATABASE"], host: str = os.environ["PG_HOST"],
               port: int = os.environ["PG_PORT"]) -> Connection:
+    """Retrieve a database connection.
+    :param user: Database user.
+    :param password: Database password.
+    :param database: Database name.
+    :param host: Database host.
+    :param port: Database port number.
+    :return: (asyncpg) Connection.
+    """
+
     connection: Connection = await connect(user=user, password=password, database=database, host=host, port=port)
     await __init(connection)
     return connection
 
 
 async def get_pool(user: str = os.environ["PG_USER"], password: str = os.environ["PG_PASSWORD"],
                    database: str = os.environ["PG_DATABASE"], host: str = os.environ["PG_HOST"],
                    port: int = os.environ["PG_PORT"], min_size: int = 0,
                    max_size: int = 2, max_inactive_connection_lifetime: int = 2) -> Pool:
+    """Retrieve a database connection pool.
+    :param user: Database user.
+    :param password: Database password.
+    :param database: Database name.
+    :param host: Database host.
+    :param port: Database port number.
+    :param min_size: Number of connection the pool will be initialized with.
+    :param max_size: Max number of connections.
+    :param max_inactive_connection_lifetime: Number of seconds after which inactive connections will be closed.
+    :return: (asyncpg) Pool.
+    """
+
     return await create_pool(user=user, password=password, database=database, host=host, port=port,
                              min_size=min_size, max_size=max_size,
                              max_inactive_connection_lifetime=max_inactive_connection_lifetime,
                              init=__init)
 
 
 async def __init(conn: Connection):
```

### Comparing `braincube-aws-core-alpha-0.0.14/src/core/dal/postgres_repository.py` & `braincube-aws-core-alpha-0.0.15/src/core/dal/postgres_repository.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 from ..utils.data import Order, OrderType, Condition, ConditionType, Page, Pageable, Paging, Top, Metadata
 from .data import Key, Schema, Relation, SaveType, Column, StatementField
 from .database_errors import DatabaseError, DeleteError, SaveError
 from .postgres_connection import Pool, Connection
 
 
 class PostgresRepository:
+    """SQL based repository implementation.
+    :param pool: database connection pool
+    :param schema: representation of master and related tables including columns, sub-queries and storage restrictions
+    :param relation_separator: character that will be used in order to separate related tables from each column
+    """
+
     def __init__(self, pool: Pool, schema: Schema, relation_separator: str = "_"):
         self._pool = pool
         self._relation_separator = relation_separator
         self.__construct_schema_data(schema)
 
     def __construct_schema_data(self, schema: Schema):
 
@@ -55,33 +61,52 @@
         self._schema_columns_fields: Dict[str, tuple] = {**self._schema_columns, **self._master_statement_fields}
 
         # order by definition:
         self._schema_order: List[Tuple[Field, OrderType]] = [(self._schema_columns_fields[order.alias][0], order.type)
                                                              for order in schema.order]
 
     async def fetch_raw(self, q: str, params: Optional[list] = None, connection: Optional[Connection] = None):
+        """Retrieve records from raw PSQL query.
+        :param q: Query.
+        :param params: Query parameters.
+        :param connection: (asyncpg) Connection that will execute the query.
+        :return: Records as dictionary.
+        """
+
         try:
             print(f"query:: {q}")
             if connection:
                 return [dict(r) for r in (await connection.fetch(q, *params) if params else await connection.fetch(q))]
             async with self._pool.acquire() as connection_:
                 return [dict(r) for r in
                         (await connection_.fetch(q, *params) if params else await connection_.fetch(q))]
         except Exception as e:
             raise DatabaseError(e)
 
     async def fetch_one_raw(self, q: str,
                             params: Optional[list] = None,
                             connection: Optional[Connection] = None) -> Optional[Dict[str, any]]:
+        """Retrieve record from raw PSQL query.
+        :param q: Query.
+        :param params: Query parameters.
+        :param connection: (asyncpg) Connection that will execute the query.
+        :return: Record as dictionary.
+        """
 
         data = await self.fetch_raw(q, params, connection)
 
         return data[0] if data else None
 
     async def execute_raw(self, q: str, params: Optional[list] = None, connection: Optional[Connection] = None) -> any:
+        """Execute raw PSQL query.
+        :param q: Query.
+        :param params: Query parameters.
+        :param connection: (asyncpg) Connection that will execute the query.
+        :return: Execution results as dictionary.
+        """
 
         return await self.fetch_raw(q, params, connection)
 
     async def _fetch(self, q: QueryBuilder,
                      replace_fields=True,
                      connection: Optional[Connection] = None) -> List[Dict[str, any]]:
 
@@ -331,73 +356,120 @@
             .where(criterion)
 
         return await self._execute(dq, returning_aliases, connection)
 
     async def find_by_id(self, key: Key,
                          aliases: Optional[List[str]] = None,
                          connection: Optional[Connection] = None) -> Optional[Dict[str, any]]:
+        """Find the record from passed key.
+        :param key: Record identifier.
+        :param aliases: List of fields that will be selected by the query.
+        :param connection: (asyncpg) Connection that will execute the generated query.
+        :return: Record as dictionary.
+        """
 
         criterion = self._create_primary_key_criterion(key)
 
         q, _ = self._init_select_query(aliases, criterion, set_order=False)
 
         return await self._fetch_one(q, connection=connection)
 
     async def exists_by_id(self, key: Key, connection: Optional[Connection] = None) -> bool:
+        """Find if record exists from passed key.
+        :param key: Record identifier.
+        :param connection: (asyncpg) Connection that will execute the generated query.
+        :return: Record existence.
+        """
 
         aliases = [column.alias for field, column in self._master_primary_key.values()]
 
         return await self.find_by_id(key, aliases, connection) is not None
 
     async def find_one(self, aliases: Optional[List[str]] = None,
                        conditions: Optional[List[Condition]] = None,
                        order: Optional[List[Order]] = None,
                        connection: Optional[Connection] = None) -> Optional[Dict[str, any]]:
+        """Find one record from passed filters.
+        :param aliases: List of fields that will be selected by the query.
+        :param conditions: List of filters that will be applied to query.
+        :param order: Order that will be applied to query.
+        :param connection: (asyncpg) Connection that will execute the generated query.
+        :return: Record as dictionary.
+        """
 
         criterion = self._conditions_to_criterion(conditions)
 
         return await self._find_one(aliases, criterion, order, connection)
 
     async def find_all(self, aliases: Optional[List[str]] = None,
                        conditions: Optional[List[Condition]] = None,
                        order: Optional[List[Order]] = None,
                        connection: Optional[Connection] = None) -> List[Dict[str, any]]:
+        """Find all records from passed filters.
+        :param aliases: List of fields that will be selected by the query.
+        :param conditions: List of filters that will be applied to query.
+        :param order: Order in which the records will be returned.
+        :param connection: (asyncpg) Connection that will execute the generated query.
+        :return: Records as dictionary list.
+        """
 
         criterion = self._conditions_to_criterion(conditions)
 
         return await self._find_all(aliases, criterion, order, connection)
 
     async def find_all_by_id(self, keys: List[Key],
                              aliases: Optional[List[str]] = None,
                              order: Optional[List[Order]] = None,
                              connection: Optional[Connection] = None) -> List[Dict[str, any]]:
+        """Find all records from passed keys.
+        :param keys: Records identifiers.
+        :param aliases: List of fields that will be selected by the query.
+        :param order: Order in which the records will be returned.
+        :param connection: (asyncpg) Connection that will execute the generated query.
+        :return: Record as dictionary.
+        """
 
         if not keys:
             raise DatabaseError("no keys provided")
 
         criterion = Criterion.any([self._create_primary_key_criterion(key) for key in keys])
 
         return await self._find_all(aliases, criterion, order, connection)
 
     async def find_all_page(self, aliases: Optional[List[str]] = None,
                             conditions: Optional[List[Condition]] = None,
                             page: Pageable = Pageable(),
                             order: Optional[List[Order]] = None,
                             connection: Optional[Connection] = None) -> Union[Page, Top]:
+        """Find records from passed filters using paging.
+        :param aliases: List of fields that will be selected by the query.
+        :param conditions: List of filters that will be applied to query.
+        :param page: Limit and offset of the query.
+        :param order: Order in which the records will be returned.
+        :param connection: (asyncpg) Connection that will execute the generated query.
+        :return: Records wrapped by Page or Top dataclass.
+        """
 
         criterion = self._conditions_to_criterion(conditions)
 
         if connection:
             return await self._find_all_page(connection, aliases, criterion, page, order)
         async with self._pool.acquire() as connection_:
             return await self._find_all_page(connection_, aliases, criterion, page, order)
 
     async def insert(self, data: Dict[str, any],
                      returning_aliases: Optional[List[str]] = None,
                      connection: Optional[Connection] = None) -> Dict[str, any]:
+        """Insert one record from dictionary.
+        :param data: Master column aliases with values.
+        :param returning_aliases: Query returning data.
+        :param connection: (asyncpg) Connection that will execute the generated query.
+        :raise SaveError: When does not adjust to insert-constraints or no master column is specified.
+        :return: Execution results as dictionary.
+        """
 
         data_ = self._filter_save_data(data, SaveType.insert)
 
         iq = PostgreSQLQuery \
             .into(self._master_table[1]) \
             .columns(list(data_.keys())) \
             .insert(list(data_.values()))
@@ -406,14 +478,22 @@
 
         return records[0] if len(records) > 0 else None
 
     async def insert_bulk(self, aliases: List[str],
                           data: List[List[any]],
                           returning_aliases: Optional[List[str]] = None,
                           connection: Optional[Connection] = None) -> List[Dict[str, any]]:
+        """Insert many records at once from list.
+        :param aliases: Master column aliases.
+        :param data: Master column values.
+        :param returning_aliases: Query returning data.
+        :param connection: (asyncpg) Connection that will execute the generated query.
+        :raise SaveError: When does not adjust to insert-constraints or no master column is specified.
+        :return: Execution results as dictionary list.
+        """
 
         for d in data:
             if len(d) == len(aliases):
                 continue
             raise SaveError("invalid bulk insert data")
 
         column_names: Dict[str, int] = dict()
@@ -436,40 +516,70 @@
 
         return await self._execute(iq, returning_aliases, connection)
 
     async def update(self, data: Dict[str, any],
                      conditions: List[Condition],
                      returning_aliases: Optional[List[str]] = None,
                      connection: Optional[Connection] = None) -> Optional[List[Dict[str, any]]]:
+        """Update records with new data according conditions.
+        :param data: Master column aliases with values.
+        :param conditions: List of filters that will be applied into the query.
+        :param returning_aliases: Query returning data.
+        :param connection: (asyncpg) Connection that will execute the generated query.
+        :raise SaveError: When does not adjust to update-constraints or no master column is specified.
+        :return: Execution results as dictionary list.
+        """
 
         criterion = self._conditions_to_criterion(conditions, select=False)
 
         return await self._update(data, criterion, returning_aliases, connection)
 
     async def update_by_id(self, key: Key,
                            data: Dict[str, any],
                            returning_aliases: Optional[List[str]] = None,
                            connection: Optional[Connection] = None) -> Optional[Dict[str, any]]:
+        """Update records with new data according to passed key.
+        :param key: Record identifier.
+        :param data: Master column aliases with values.
+        :param returning_aliases: Query returning data.
+        :param connection: (asyncpg) Connection that will execute the generated query.
+        :raise SaveError: When does not adjust to update-constraints or no master column is specified.
+        :return: Execution results as dictionary.
+        """
 
         criterion = self._create_primary_key_criterion(key)
 
         records = await self._update(data, criterion, returning_aliases, connection)
 
         return records[0] if len(records) > 0 else None
 
     async def delete(self, conditions: List[Condition],
                      returning_aliases: Optional[List[str]] = None,
                      connection: Optional[Connection] = None) -> Optional[List[Dict[str, any]]]:
+        """Delete records according conditions.
+        :param conditions: List of filters that will be applied into the query.
+        :param returning_aliases: Query returning data.
+        :param connection: (asyncpg) Connection that will execute the generated query.
+        :raise SaveError: When conditions are empty.
+        :return: Execution results as dictionary list.
+        """
 
         criterion = self._conditions_to_criterion(conditions, select=False)
 
         return await self._delete(criterion, returning_aliases, connection)
 
     async def delete_by_id(self, key: Key,
                            returning_aliases: Optional[List[str]] = None,
                            connection: Optional[Connection] = None) -> Optional[Dict[str, any]]:
+        """Delete records according to passed key.
+        :param key: Record identifier.
+        :param returning_aliases: Query returning data.
+        :param connection: (asyncpg) Connection that will execute the generated query.
+        :raise SaveError: When conditions are empty.
+        :return: Execution results as dictionary.
+        """
 
         criterion = self._create_primary_key_criterion(key)
 
         records = await self._delete(criterion, returning_aliases, connection)
 
         return records[0] if len(records) > 0 else None
```

### Comparing `braincube-aws-core-alpha-0.0.14/src/core/di/data.py` & `braincube-aws-core-alpha-0.0.15/src/core/di/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.14/src/core/di/injector.py` & `braincube-aws-core-alpha-0.0.15/src/core/di/injector.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from .data import Dependency, Scope, qualifier_to_data
 from ..utils.data import module_names_from_directory
 
 T = TypeVar("T")
 
 
 class _Injector:
+    """Module that used in order to resolve dependencies from components or route functions."""
+
     dependencies: List[Dependency] = list()
 
     @staticmethod
     def component_scan(paths: List[str]):
         for path in paths:
             module_names = module_names_from_directory(f"/var/task/{path.replace('.', '/')}")
             for module_name in module_names:
@@ -65,16 +67,34 @@
 
 
 def component_scan(paths: List[str]):
     _Injector.component_scan(paths)
 
 
 def inject(name: Optional[str] = None, scope: Scope = Scope.singleton, qualifier: Optional[str] = None):
+    """Inject a class or function.
+    :param name: Component name.
+    :param scope: Class of the Scope in which to resolve.
+    :param qualifier: Comma separated string, used to specify components by name in case of multiple implementations.
+    """
+
     return _Injector.inject(name, scope, qualifier)
 
 
 async def provide(cls: Type[T], name: Optional[str] = None) -> T:
+    """Get an instance of the given type.
+    :param cls: Interface whose implementation we want.
+    :param name: Name of a specific component that implements the interface.
+    :returns: An implementation of interface.
+    """
+
     return await _Injector.provide(cls, name)
 
 
 def register_instance(cls: Type[T], instance: T, name: Optional[str] = None):
+    """Create manually and register an instance of a specific type.
+    :param cls: Component type.
+    :param instance: Component instance.
+    :param name: Component name.
+    """
+
     return _Injector.register_instance(cls, instance, name)
```

### Comparing `braincube-aws-core-alpha-0.0.14/src/core/rest/app_module.py` & `braincube-aws-core-alpha-0.0.15/src/core/rest/app_module.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,19 @@
 @dataclass()
 class _Route:
     func: callable
     request_type: Optional[type]
     dependencies: List[Tuple[type, Optional[str]]]
 
 
-@dataclass
 class AppModule:
+    """AWS lambda application main entry point.
+    :param controllers: Application controllers.
+    :param modules: Folders to be forced import.
+    """
 
     def __init__(self, controllers: List[AppController], modules: Optional[List[str]] = None):
 
         component_scan(modules if modules else ["main.repository", "main.service"])
 
         routes = dict()
```

### Comparing `braincube-aws-core-alpha-0.0.14/src/core/rest/data.py` & `braincube-aws-core-alpha-0.0.15/src/core/rest/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.14/src/core/utils/convert.py` & `braincube-aws-core-alpha-0.0.15/src/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.14/src/core/utils/data.py` & `braincube-aws-core-alpha-0.0.15/src/core/utils/data.py`

 * *Files identical despite different names*

