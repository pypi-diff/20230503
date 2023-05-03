# Comparing `tmp/fastapi-users-db-sqlmodel-0.2.0.tar.gz` & `tmp/fastapi_users_db_sqlmodel-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-users-db-sqlmodel-0.2.0.tar", last modified: Mon May  9 09:01:22 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `fastapi-users-db-sqlmodel-0.2.0.tar` & `fastapi_users_db_sqlmodel-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,22 @@
--rw-r--r--   0        0        0      230 2022-05-09 09:00:56.822589 fastapi-users-db-sqlmodel-0.2.0/.editorconfig
--rw-r--r--   0        0        0       94 2022-05-09 09:00:56.822589 fastapi-users-db-sqlmodel-0.2.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      647 2022-05-09 09:00:56.822589 fastapi-users-db-sqlmodel-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      243 2022-05-09 09:00:56.822589 fastapi-users-db-sqlmodel-0.2.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      171 2022-05-09 09:00:56.822589 fastapi-users-db-sqlmodel-0.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0      724 2022-05-09 09:00:56.822589 fastapi-users-db-sqlmodel-0.2.0/.github/stale.yml
--rw-r--r--   0        0        0     1335 2022-05-09 09:00:56.822589 fastapi-users-db-sqlmodel-0.2.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     1257 2022-05-09 09:00:56.822589 fastapi-users-db-sqlmodel-0.2.0/.gitignore
--rw-r--r--   0        0        0     1072 2022-05-09 09:00:56.822589 fastapi-users-db-sqlmodel-0.2.0/LICENSE
--rw-r--r--   0        0        0      286 2022-05-09 09:00:56.822589 fastapi-users-db-sqlmodel-0.2.0/Makefile
--rw-r--r--   0        0        0     2492 2022-05-09 09:00:56.822589 fastapi-users-db-sqlmodel-0.2.0/README.md
--rw-r--r--   0        0        0     8123 2022-05-09 09:00:56.822589 fastapi-users-db-sqlmodel-0.2.0/fastapi_users_db_sqlmodel/__init__.py
--rw-r--r--   0        0        0     4246 2022-05-09 09:00:56.822589 fastapi-users-db-sqlmodel-0.2.0/fastapi_users_db_sqlmodel/access_token.py
--rw-r--r--   0        0        0      625 2022-05-09 09:00:56.822589 fastapi-users-db-sqlmodel-0.2.0/fastapi_users_db_sqlmodel/generics.py
--rw-r--r--   0        0        0        0 2022-05-09 09:00:56.822589 fastapi-users-db-sqlmodel-0.2.0/fastapi_users_db_sqlmodel/py.typed
--rw-r--r--   0        0        0     1065 2022-05-09 09:00:56.822589 fastapi-users-db-sqlmodel-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      172 2022-05-09 09:00:56.822589 fastapi-users-db-sqlmodel-0.2.0/requirements.dev.txt
--rw-r--r--   0        0        0      135 2022-05-09 09:00:56.822589 fastapi-users-db-sqlmodel-0.2.0/requirements.txt
--rw-r--r--   0        0        0      386 2022-05-09 09:00:56.822589 fastapi-users-db-sqlmodel-0.2.0/setup.cfg
--rw-r--r--   0        0        0      132 2022-05-09 09:00:56.822589 fastapi-users-db-sqlmodel-0.2.0/test_build.py
--rw-r--r--   0        0        0        0 2022-05-09 09:00:56.822589 fastapi-users-db-sqlmodel-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1467 2022-05-09 09:00:56.822589 fastapi-users-db-sqlmodel-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0     4802 2022-05-09 09:00:56.822589 fastapi-users-db-sqlmodel-0.2.0/tests/test_access_token.py
--rw-r--r--   0        0        0     7064 2022-05-09 09:00:56.822589 fastapi-users-db-sqlmodel-0.2.0/tests/test_users.py
--rw-r--r--   0        0        0     3434 1970-01-01 00:00:00.000000 fastapi-users-db-sqlmodel-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastapi_users_db_sqlmodel-0.3.0/.editorconfig
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 fastapi_users_db_sqlmodel-0.3.0/test_build.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fastapi_users_db_sqlmodel-0.3.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastapi_users_db_sqlmodel-0.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 fastapi_users_db_sqlmodel-0.3.0/.github/stale.yml
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastapi_users_db_sqlmodel-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 fastapi_users_db_sqlmodel-0.3.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 fastapi_users_db_sqlmodel-0.3.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     8155 2020-02-02 00:00:00.000000 fastapi_users_db_sqlmodel-0.3.0/fastapi_users_db_sqlmodel/__init__.py
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 fastapi_users_db_sqlmodel-0.3.0/fastapi_users_db_sqlmodel/access_token.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 fastapi_users_db_sqlmodel-0.3.0/fastapi_users_db_sqlmodel/generics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_users_db_sqlmodel-0.3.0/fastapi_users_db_sqlmodel/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_users_db_sqlmodel-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 fastapi_users_db_sqlmodel-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     4802 2020-02-02 00:00:00.000000 fastapi_users_db_sqlmodel-0.3.0/tests/test_access_token.py
+-rw-r--r--   0        0        0     7064 2020-02-02 00:00:00.000000 fastapi_users_db_sqlmodel-0.3.0/tests/test_users.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 fastapi_users_db_sqlmodel-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 fastapi_users_db_sqlmodel-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 fastapi_users_db_sqlmodel-0.3.0/README.md
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 fastapi_users_db_sqlmodel-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 fastapi_users_db_sqlmodel-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 fastapi_users_db_sqlmodel-0.3.0/setup.py
```

### Comparing `fastapi-users-db-sqlmodel-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `fastapi_users_db_sqlmodel-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-db-sqlmodel-0.2.0/.github/stale.yml` & `fastapi_users_db_sqlmodel-0.3.0/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `fastapi-users-db-sqlmodel-0.2.0/.github/workflows/build.yml` & `fastapi_users_db_sqlmodel-0.3.0/.github/workflows/build.yml`

 * *Files 17% similar despite different names*

```diff
@@ -4,52 +4,66 @@
 
 jobs:
 
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python_version: [3.7, 3.8, 3.9]
+        python_version: [3.7, 3.8, 3.9, '3.10', '3.11']
 
     steps:
-    - uses: actions/checkout@v1
-    - name: Set up Python
-      uses: actions/setup-python@v1
-      with:
-        python-version: ${{ matrix.python_version }}
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        pip install -r requirements.dev.txt
-    - name: Test with pytest
-      env:
-        CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
-      run: |
-        pytest --cov=fastapi_users_db_sqlmodel/
-        codecov
-    - name: Build and install it on system host
-      run: |
-        flit build
-        flit install --python $(which python)
-        python test_build.py
+      - uses: actions/checkout@v3
+      - name: Set up Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.python_version }}
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install hatch
+          hatch env create
+      - name: Lint and typecheck
+        run: |
+          hatch run lint-check
+      - name: Test
+        run: |
+          hatch run test-cov-xml
+      - uses: codecov/codecov-action@v3
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }}
+          fail_ci_if_error: true
+          verbose: true
+      - name: Build and install it on system host
+        run: |
+          hatch build
+          pip install dist/fastapi_users_db_sqlmodel-*.whl
+          python test_build.py
 
   release:
     runs-on: ubuntu-latest
     needs: test
     if: startsWith(github.ref, 'refs/tags/')
 
     steps:
-    - uses: actions/checkout@v1
-    - name: Set up Python
-      uses: actions/setup-python@v1
-      with:
-        python-version: 3.7
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        pip install -r requirements.dev.txt
-    - name: Release on PyPI
-      env:
-        FLIT_USERNAME: ${{ secrets.FLIT_USERNAME }}
-        FLIT_PASSWORD: ${{ secrets.FLIT_PASSWORD }}
-      run: |
-        flit publish
+      - uses: actions/checkout@v3
+      - name: Set up Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: 3.7
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install hatch
+      - name: Build and publish on PyPI
+        env:
+          HATCH_INDEX_USER: ${{ secrets.HATCH_INDEX_USER }}
+          HATCH_INDEX_AUTH: ${{ secrets.HATCH_INDEX_AUTH }}
+        run: |
+          hatch build
+          hatch publish
+      - name: Create release
+        uses: ncipollo/release-action@v1
+        with:
+          draft: true
+          body: ${{ github.event.head_commit.message }}
+          artifacts: dist/*.whl,dist/*.tar.gz
+          token: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `fastapi-users-db-sqlmodel-0.2.0/.gitignore` & `fastapi_users_db_sqlmodel-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi-users-db-sqlmodel-0.2.0/LICENSE` & `fastapi_users_db_sqlmodel-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-users-db-sqlmodel-0.2.0/README.md` & `fastapi_users_db_sqlmodel-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 </p>
 
 [![build](https://github.com/fastapi-users/fastapi-users-db-sqlmodel/workflows/Build/badge.svg)](https://github.com/fastapi-users/fastapi-users/actions)
 [![codecov](https://codecov.io/gh/fastapi-users/fastapi-users-db-sqlmodel/branch/master/graph/badge.svg)](https://codecov.io/gh/fastapi-users/fastapi-users-db-sqlmodel)
 [![PyPI version](https://badge.fury.io/py/fastapi-users-db-sqlmodel.svg)](https://badge.fury.io/py/fastapi-users-db-sqlmodel)
 [![Downloads](https://pepy.tech/badge/fastapi-users-db-sqlmodel)](https://pepy.tech/project/fastapi-users-db-sqlmodel)
 <p align="center">
-    <a href="https://www.buymeacoffee.com/frankie567"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=frankie567&button_colour=FF5F5F&font_colour=ffffff&font_family=Lato&outline_colour=000000&coffee_colour=FFDD00"></a>
+<a href="https://github.com/sponsors/frankie567"><img src="https://md-btn.deta.dev/button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50"></a>
 </p>
 
 ---
 
 **Documentation**: <a href="https://fastapi-users.github.io/fastapi-users/" target="_blank">https://fastapi-users.github.io/fastapi-users/</a>
 
 **Source Code**: <a href="https://github.com/fastapi-users/fastapi-users" target="_blank">https://github.com/fastapi-users/fastapi-users</a>
```

#### html2text {}

```diff
@@ -5,16 +5,16 @@
 Build/badge.svg)](https://github.com/fastapi-users/fastapi-users/actions) [!
 [codecov](https://codecov.io/gh/fastapi-users/fastapi-users-db-sqlmodel/branch/
 master/graph/badge.svg)](https://codecov.io/gh/fastapi-users/fastapi-users-db-
 sqlmodel) [![PyPI version](https://badge.fury.io/py/fastapi-users-db-
 sqlmodel.svg)](https://badge.fury.io/py/fastapi-users-db-sqlmodel) [!
 [Downloads](https://pepy.tech/badge/fastapi-users-db-sqlmodel)](https://
 pepy.tech/project/fastapi-users-db-sqlmodel)
-            [https://img.buymeacoffee.com/button-api/?text=Buy_me_a
-coffee&emoji=&slug=frankie567&button_colour=FF5F5F&font_colour=ffffff&font_family=Lato&outline_colour=000000&coffee_colour=FFDD00]
+                           [https://md-btn.deta.dev/
+button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50]
 --- **Documentation**: https://fastapi-users.github.io/fastapi-users/ **Source
 Code**: https://github.com/fastapi-users/fastapi-users --- Add quickly a
 registration and authentication system to your [FastAPI](https://
 fastapi.tiangolo.com/) project. **FastAPI Users** is designed to be as
 customizable and adaptable as possible. **Sub-package for SQLModel support in
 FastAPI Users.** ## Development ### Setup environment You should create a
 virtual environment and activate it: ```bash python -m venv venv/ ``` ```bash
```

### Comparing `fastapi-users-db-sqlmodel-0.2.0/fastapi_users_db_sqlmodel/__init__.py` & `fastapi_users_db_sqlmodel-0.3.0/fastapi_users_db_sqlmodel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from fastapi_users.db.base import BaseUserDatabase
 from fastapi_users.models import ID, OAP, UP
 from pydantic import UUID4, EmailStr
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.orm import selectinload
 from sqlmodel import Field, Session, SQLModel, func, select
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 
 class SQLModelBaseUserDB(SQLModel):
     __tablename__ = "user"
 
     id: UUID4 = Field(default_factory=uuid.uuid4, primary_key=True, nullable=False)
     if TYPE_CHECKING:  # pragma: no cover
@@ -71,15 +71,15 @@
 
     async def get(self, id: ID) -> Optional[UP]:
         """Get a single user by id."""
         return self.session.get(self.user_model, id)
 
     async def get_by_email(self, email: str) -> Optional[UP]:
         """Get a single user by email."""
-        statement = select(self.user_model).where(
+        statement = select(self.user_model).where(  # type: ignore
             func.lower(self.user_model.email) == func.lower(email)
         )
         results = self.session.exec(statement)
         return results.first()
 
     async def get_by_oauth_account(self, oauth: str, account_id: str) -> Optional[UP]:
         """Get a single user by OAuth account id."""
@@ -167,15 +167,15 @@
 
     async def get(self, id: ID) -> Optional[UP]:
         """Get a single user by id."""
         return await self.session.get(self.user_model, id)
 
     async def get_by_email(self, email: str) -> Optional[UP]:
         """Get a single user by email."""
-        statement = select(self.user_model).where(
+        statement = select(self.user_model).where(  # type: ignore
             func.lower(self.user_model.email) == func.lower(email)
         )
         results = await self.session.execute(statement)
         object = results.first()
         if object is None:
             return None
         return object[0]
```

### Comparing `fastapi-users-db-sqlmodel-0.2.0/fastapi_users_db_sqlmodel/access_token.py` & `fastapi_users_db_sqlmodel-0.3.0/fastapi_users_db_sqlmodel/access_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def __init__(self, session: Session, access_token_model: Type[AP]):
         self.session = session
         self.access_token_model = access_token_model
 
     async def get_by_token(
         self, token: str, max_age: Optional[datetime] = None
     ) -> Optional[AP]:
-        statement = select(self.access_token_model).where(
+        statement = select(self.access_token_model).where(  # type: ignore
             self.access_token_model.token == token
         )
         if max_age is not None:
             statement = statement.where(self.access_token_model.created_at >= max_age)
 
         results = self.session.execute(statement)
         access_token = results.first()
@@ -86,15 +86,15 @@
     def __init__(self, session: AsyncSession, access_token_model: Type[AP]):
         self.session = session
         self.access_token_model = access_token_model
 
     async def get_by_token(
         self, token: str, max_age: Optional[datetime] = None
     ) -> Optional[AP]:
-        statement = select(self.access_token_model).where(
+        statement = select(self.access_token_model).where(  # type: ignore
             self.access_token_model.token == token
         )
         if max_age is not None:
             statement = statement.where(self.access_token_model.created_at >= max_age)
 
         results = await self.session.execute(statement)
         access_token = results.first()
```

### Comparing `fastapi-users-db-sqlmodel-0.2.0/fastapi_users_db_sqlmodel/generics.py` & `fastapi_users_db_sqlmodel-0.3.0/fastapi_users_db_sqlmodel/generics.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-db-sqlmodel-0.2.0/pyproject.toml` & `fastapi_users_db_sqlmodel-0.3.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,84 @@
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
+addopts = "--ignore=test_build.py"
+
+[tool.ruff]
+extend-select = ["I"]
+
+[tool.hatch]
+
+[tool.hatch.metadata]
+allow-direct-references = true
+
+[tool.hatch.version]
+source = "regex_commit"
+commit_extra_args = ["-e"]
+path = "fastapi_users_db_sqlmodel/__init__.py"
+
+[tool.hatch.envs.default]
+dependencies = [
+    "aiosqlite",
+    "pytest",
+    "pytest-asyncio",
+    "black",
+    "mypy",
+    "pytest-cov",
+    "pytest-mock",
+    "httpx",
+    "asgi_lifespan",
+    "ruff",
+]
+
+[tool.hatch.envs.default.scripts]
+test = "pytest --cov=fastapi_users_db_sqlmodel/ --cov-report=term-missing --cov-fail-under=100"
+test-cov-xml = "pytest --cov=fastapi_users_db_sqlmodel/ --cov-report=xml --cov-fail-under=100"
+lint = [
+  "black . ",
+  "ruff --fix .",
+  "mypy fastapi_users_db_sqlmodel/",
+]
+lint-check = [
+  "black --check .",
+  "ruff .",
+  "mypy fastapi_users_db_sqlmodel/",
+]
+
+[tool.hatch.build.targets.sdist]
+support-legacy = true  # Create setup.py
+
 [build-system]
-requires = ["flit_core >=2,<3"]
-build-backend = "flit_core.buildapi"
+requires = ["hatchling", "hatch-regex-commit"]
+build-backend = "hatchling.build"
 
-[tool.flit.metadata]
-module = "fastapi_users_db_sqlmodel"
-dist-name = "fastapi-users-db-sqlmodel"
-author = "François Voron"
-author-email = "fvoron@gmail.com"
-home-page = "https://github.com/fastapi-users/fastapi-users-db-sqlmodel"
+[project]
+name = "fastapi-users-db-sqlmodel"
+authors = [
+    { name = "François Voron", email = "fvoron@gmail.com" },
+]
+description = "FastAPI Users database adapter for SQLModel"
+readme = "README.md"
+dynamic = ["version"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Development Status :: 5 - Production/Stable",
+    "Framework :: FastAPI",
     "Framework :: AsyncIO",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Internet :: WWW/HTTP :: Session",
 ]
-description-file = "README.md"
 requires-python = ">=3.7"
-requires = [
+dependencies = [
     "fastapi-users >= 10.0.2",
+    "greenlet",
     "sqlmodel",
-    "sqlalchemy[asyncio] >=1.4,<1.4.36",  # Pin SQLAlchemy to prevent bug https://github.com/tiangolo/sqlmodel/issues/315
 ]
 
-[tool.flit.metadata.urls]
+[project.urls]
 Documentation = "https://fastapi-users.github.io/fastapi-users"
+Source = "https://github.com/fastapi-users/fastapi-users-db-sqlmodel"
```

### Comparing `fastapi-users-db-sqlmodel-0.2.0/tests/conftest.py` & `fastapi_users_db_sqlmodel-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-db-sqlmodel-0.2.0/tests/test_access_token.py` & `fastapi_users_db_sqlmodel-0.3.0/tests/test_access_token.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-db-sqlmodel-0.2.0/tests/test_users.py` & `fastapi_users_db_sqlmodel-0.3.0/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-db-sqlmodel-0.2.0/PKG-INFO` & `fastapi_users_db_sqlmodel-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: fastapi-users-db-sqlmodel
-Version: 0.2.0
-Summary: FastAPI Users database adapter for SQLModel.
-Home-page: https://github.com/fastapi-users/fastapi-users-db-sqlmodel
-Author: François Voron
-Author-email: fvoron@gmail.com
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Classifier: License :: OSI Approved :: MIT License
+Version: 0.3.0
+Summary: FastAPI Users database adapter for SQLModel
+Project-URL: Documentation, https://fastapi-users.github.io/fastapi-users
+Project-URL: Source, https://github.com/fastapi-users/fastapi-users-db-sqlmodel
+Author-email: François Voron <fvoron@gmail.com>
+License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
+Classifier: Framework :: FastAPI
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
-Requires-Dist: fastapi-users >= 10.0.2
+Requires-Python: >=3.7
+Requires-Dist: fastapi-users>=10.0.2
+Requires-Dist: greenlet
 Requires-Dist: sqlmodel
-Requires-Dist: sqlalchemy[asyncio] >=1.4,<1.4.36
-Project-URL: Documentation, https://fastapi-users.github.io/fastapi-users
+Description-Content-Type: text/markdown
 
 # FastAPI Users - Database adapter for SQLModel
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/frankie567/fastapi-users/master/logo.svg?sanitize=true" alt="FastAPI Users">
 </p>
 
@@ -32,15 +35,15 @@
 </p>
 
 [![build](https://github.com/fastapi-users/fastapi-users-db-sqlmodel/workflows/Build/badge.svg)](https://github.com/fastapi-users/fastapi-users/actions)
 [![codecov](https://codecov.io/gh/fastapi-users/fastapi-users-db-sqlmodel/branch/master/graph/badge.svg)](https://codecov.io/gh/fastapi-users/fastapi-users-db-sqlmodel)
 [![PyPI version](https://badge.fury.io/py/fastapi-users-db-sqlmodel.svg)](https://badge.fury.io/py/fastapi-users-db-sqlmodel)
 [![Downloads](https://pepy.tech/badge/fastapi-users-db-sqlmodel)](https://pepy.tech/project/fastapi-users-db-sqlmodel)
 <p align="center">
-    <a href="https://www.buymeacoffee.com/frankie567"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=frankie567&button_colour=FF5F5F&font_colour=ffffff&font_family=Lato&outline_colour=000000&coffee_colour=FFDD00"></a>
+<a href="https://github.com/sponsors/frankie567"><img src="https://md-btn.deta.dev/button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50"></a>
 </p>
 
 ---
 
 **Documentation**: <a href="https://fastapi-users.github.io/fastapi-users/" target="_blank">https://fastapi-users.github.io/fastapi-users/</a>
 
 **Source Code**: <a href="https://github.com/fastapi-users/fastapi-users" target="_blank">https://github.com/fastapi-users/fastapi-users</a>
@@ -98,8 +101,7 @@
 ```bash
 make format
 ```
 
 ## License
 
 This project is licensed under the terms of the MIT license.
-
```

#### html2text {}

```diff
@@ -1,32 +1,34 @@
-Metadata-Version: 2.1 Name: fastapi-users-db-sqlmodel Version: 0.2.0 Summary:
-FastAPI Users database adapter for SQLModel. Home-page: https://github.com/
-fastapi-users/fastapi-users-db-sqlmodel Author: FranÃ§ois Voron Author-email:
-fvoron@gmail.com Requires-Python: >=3.7 Description-Content-Type: text/markdown
-Classifier: License :: OSI Approved :: MIT License Classifier: Development
-Status :: 5 - Production/Stable Classifier: Framework :: AsyncIO Classifier:
-Intended Audience :: Developers Classifier: Programming Language :: Python ::
-3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3 ::
-Only Classifier: Topic :: Internet :: WWW/HTTP :: Session Requires-Dist:
-fastapi-users >= 10.0.2 Requires-Dist: sqlmodel Requires-Dist: sqlalchemy
-[asyncio] >=1.4,<1.4.36 Project-URL: Documentation, https://fastapi-
-users.github.io/fastapi-users # FastAPI Users - Database adapter for SQLModel
+Metadata-Version: 2.1 Name: fastapi-users-db-sqlmodel Version: 0.3.0 Summary:
+FastAPI Users database adapter for SQLModel Project-URL: Documentation, https:/
+/fastapi-users.github.io/fastapi-users Project-URL: Source, https://github.com/
+fastapi-users/fastapi-users-db-sqlmodel Author-email: FranÃ§ois Voron
+gmail.com> License-File: LICENSE Classifier: Development Status :: 5 -
+Production/Stable Classifier: Framework :: AsyncIO Classifier: Framework ::
+FastAPI Classifier: Intended Audience :: Developers Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Topic :: Internet :: WWW/HTTP :: Session
+Requires-Python: >=3.7 Requires-Dist: fastapi-users>=10.0.2 Requires-Dist:
+greenlet Requires-Dist: sqlmodel Description-Content-Type: text/markdown #
+FastAPI Users - Database adapter for SQLModel
                                 [FastAPI Users]
           Ready-to-use and customizable users management for FastAPI
 [![build](https://github.com/fastapi-users/fastapi-users-db-sqlmodel/workflows/
 Build/badge.svg)](https://github.com/fastapi-users/fastapi-users/actions) [!
 [codecov](https://codecov.io/gh/fastapi-users/fastapi-users-db-sqlmodel/branch/
 master/graph/badge.svg)](https://codecov.io/gh/fastapi-users/fastapi-users-db-
 sqlmodel) [![PyPI version](https://badge.fury.io/py/fastapi-users-db-
 sqlmodel.svg)](https://badge.fury.io/py/fastapi-users-db-sqlmodel) [!
 [Downloads](https://pepy.tech/badge/fastapi-users-db-sqlmodel)](https://
 pepy.tech/project/fastapi-users-db-sqlmodel)
-            [https://img.buymeacoffee.com/button-api/?text=Buy_me_a
-coffee&emoji=&slug=frankie567&button_colour=FF5F5F&font_colour=ffffff&font_family=Lato&outline_colour=000000&coffee_colour=FFDD00]
+                           [https://md-btn.deta.dev/
+button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50]
 --- **Documentation**: https://fastapi-users.github.io/fastapi-users/ **Source
 Code**: https://github.com/fastapi-users/fastapi-users --- Add quickly a
 registration and authentication system to your [FastAPI](https://
 fastapi.tiangolo.com/) project. **FastAPI Users** is designed to be as
 customizable and adaptable as possible. **Sub-package for SQLModel support in
 FastAPI Users.** ## Development ### Setup environment You should create a
 virtual environment and activate it: ```bash python -m venv venv/ ``` ```bash
```

