# Comparing `tmp/peltak-changelog-0.0.3.tar.gz` & `tmp/peltak-changelog-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peltak-changelog-0.0.3.tar", max compression
+gzip compressed data, was "peltak-changelog-0.0.4.tar", max compression
```

## Comparing `peltak-changelog-0.0.3.tar` & `peltak-changelog-0.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0        0 2022-10-17 22:51:25.751695 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/_pytest/py.typed
--rw-r--r--   0        0        0        0 2022-10-17 22:51:18.061730 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/attr/py.typed
--rw-r--r--   0        0        0        0 2022-10-17 22:51:18.067191 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/attrs/py.typed
--rw-r--r--   0        0        0        0 2022-10-17 22:51:11.913125 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/certifi/py.typed
--rw-r--r--   0        0        0        0 2022-10-17 22:51:11.913193 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/charset_normalizer/py.typed
--rw-r--r--   0        0        0        0 2022-10-17 22:51:11.912992 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/idna/py.typed
--rw-r--r--   0        0        0        0 2022-10-17 22:51:17.514558 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/iniconfig/py.typed
--rw-r--r--   0        0        0       26 2022-10-17 22:51:25.233529 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0        0        0        0 2022-10-17 22:51:25.246401 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/isort/py.typed
--rw-r--r--   0        0        0        0 2022-10-17 22:51:17.832468 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/jinja2/py.typed
--rw-r--r--   0        0        0        0 2022-10-17 22:51:11.911045 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/markupsafe/py.typed
--rw-r--r--   0        0        0       64 2022-10-17 22:51:29.894391 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/mypy/py.typed
--rw-r--r--   0        0        0        0 2022-10-17 22:51:17.823513 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/packaging/py.typed
--rw-r--r--   0        0        0      286 2022-10-17 22:51:05.813501 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/pip/py.typed
--rw-r--r--   0        0        0        0 2022-10-17 22:51:24.840705 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/platformdirs/py.typed
--rw-r--r--   0        0        0        0 2022-10-17 22:51:18.306699 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/py/_vendored_packages/iniconfig/py.typed
--rw-r--r--   0        0        0        0 2022-10-17 22:51:18.279154 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/py/py.typed
--rw-r--r--   0        0        0        0 2022-10-17 22:51:11.914300 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/pyparsing/py.typed
--rw-r--r--   0        0        0        0 2022-10-17 22:51:25.790730 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/pytest/py.typed
--rw-r--r--   0        0        0        0 2022-10-17 22:51:17.989422 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/soupsieve/py.typed
--rw-r--r--   0        0        0        0 2022-10-17 22:51:25.794520 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/sphinx/py.typed
--rw-r--r--   0        0        0        0 2022-10-17 22:51:29.459445 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/sphinx_autodoc_typehints/py.typed
--rw-r--r--   0        0        0        0 2022-10-17 22:51:25.710619 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/termcolor/py.typed
--rw-r--r--   0        0        0       26 2022-10-17 22:51:19.538465 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/tomli/py.typed
--rw-r--r--   0        0        0        0 2022-10-17 22:51:25.698936 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/tomlkit/py.typed
--rw-r--r--   0        0        0        0 2022-10-17 22:51:19.709504 peltak-changelog-0.0.3/.venv/lib/python3.8/site-packages/unidecode/py.typed
--rw-r--r--   0        0        0      239 2022-10-17 12:21:58.568436 peltak-changelog-0.0.3/AUTHORS
--rw-r--r--   0        0        0    11357 2022-10-17 12:21:58.568620 peltak-changelog-0.0.3/LICENSE
--rw-r--r--   0        0        0     1433 2022-10-17 12:21:58.569036 peltak-changelog-0.0.3/README.rst
--rw-r--r--   0        0        0     1696 2022-10-29 05:27:21.380421 peltak-changelog-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2473 2022-10-29 05:27:21.380730 peltak-changelog-0.0.3/src/peltak_changelog/__init__.py
--rw-r--r--   0        0        0     1931 2022-10-29 02:22:44.287847 peltak-changelog-0.0.3/src/peltak_changelog/commands.py
--rw-r--r--   0        0        0     7090 2022-10-17 12:21:58.577205 peltak-changelog-0.0.3/src/peltak_changelog/logic.py
--rw-r--r--   0        0        0        0 2022-10-17 12:21:58.577281 peltak-changelog-0.0.3/src/peltak_changelog/py.typed
--rw-r--r--   0        0        0     1136 2022-10-17 12:21:58.577824 peltak-changelog-0.0.3/src/peltak_changelog/types.py
--rw-r--r--   0        0        0      611 2022-10-29 05:29:59.606145 peltak-changelog-0.0.3/setup.py
--rw-r--r--   0        0        0      561 2022-10-29 05:29:59.606360 peltak-changelog-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-10-17 22:51:25.751695 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/_pytest/py.typed
+-rw-r--r--   0        0        0        0 2022-10-17 22:51:18.061730 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/attr/py.typed
+-rw-r--r--   0        0        0        0 2022-10-17 22:51:18.067191 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/attrs/py.typed
+-rw-r--r--   0        0        0        0 2022-10-17 22:51:11.913125 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/certifi/py.typed
+-rw-r--r--   0        0        0        0 2022-10-17 22:51:11.913193 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/charset_normalizer/py.typed
+-rw-r--r--   0        0        0        0 2022-10-17 22:51:11.912992 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/idna/py.typed
+-rw-r--r--   0        0        0        0 2022-10-17 22:51:17.514558 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/iniconfig/py.typed
+-rw-r--r--   0        0        0       26 2022-10-17 22:51:25.233529 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0        0        0        0 2022-10-17 22:51:25.246401 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/isort/py.typed
+-rw-r--r--   0        0        0        0 2022-10-17 22:51:17.832468 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/jinja2/py.typed
+-rw-r--r--   0        0        0        0 2022-10-17 22:51:11.911045 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/markupsafe/py.typed
+-rw-r--r--   0        0        0       64 2022-10-17 22:51:29.894391 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/mypy/py.typed
+-rw-r--r--   0        0        0        0 2022-10-17 22:51:17.823513 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/packaging/py.typed
+-rw-r--r--   0        0        0      286 2022-10-17 22:51:05.813501 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/pip/py.typed
+-rw-r--r--   0        0        0        0 2022-10-17 22:51:24.840705 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/platformdirs/py.typed
+-rw-r--r--   0        0        0        0 2022-10-17 22:51:18.306699 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0        0        0        0 2022-10-17 22:51:18.279154 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/py/py.typed
+-rw-r--r--   0        0        0        0 2022-10-17 22:51:11.914300 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/pyparsing/py.typed
+-rw-r--r--   0        0        0        0 2022-10-17 22:51:25.790730 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/pytest/py.typed
+-rw-r--r--   0        0        0        0 2022-10-17 22:51:17.989422 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/soupsieve/py.typed
+-rw-r--r--   0        0        0        0 2022-10-17 22:51:25.794520 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/sphinx/py.typed
+-rw-r--r--   0        0        0        0 2022-10-17 22:51:29.459445 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/sphinx_autodoc_typehints/py.typed
+-rw-r--r--   0        0        0        0 2022-10-17 22:51:25.710619 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/termcolor/py.typed
+-rw-r--r--   0        0        0       26 2022-10-17 22:51:19.538465 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/tomli/py.typed
+-rw-r--r--   0        0        0        0 2022-10-17 22:51:25.698936 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/tomlkit/py.typed
+-rw-r--r--   0        0        0        0 2022-10-17 22:51:19.709504 peltak-changelog-0.0.4/.venv/lib/python3.8/site-packages/unidecode/py.typed
+-rw-r--r--   0        0        0      239 2022-10-17 12:21:58.568436 peltak-changelog-0.0.4/AUTHORS
+-rw-r--r--   0        0        0    11357 2022-10-17 12:21:58.568620 peltak-changelog-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3171 2022-12-28 06:25:44.753571 peltak-changelog-0.0.4/README.rst
+-rw-r--r--   0        0        0     1698 2023-05-03 12:23:57.968475 peltak-changelog-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2473 2023-05-03 12:23:57.968805 peltak-changelog-0.0.4/src/peltak_changelog/__init__.py
+-rw-r--r--   0        0        0     1931 2022-11-19 20:59:17.760321 peltak-changelog-0.0.4/src/peltak_changelog/commands.py
+-rw-r--r--   0        0        0     7090 2022-10-17 12:21:58.577205 peltak-changelog-0.0.4/src/peltak_changelog/logic.py
+-rw-r--r--   0        0        0        0 2022-10-17 12:21:58.577281 peltak-changelog-0.0.4/src/peltak_changelog/py.typed
+-rw-r--r--   0        0        0     1119 2023-05-03 10:18:01.931306 peltak-changelog-0.0.4/src/peltak_changelog/types.py
+-rw-r--r--   0        0        0      611 2023-05-03 12:24:11.006507 peltak-changelog-0.0.4/setup.py
+-rw-r--r--   0        0        0      561 2023-05-03 12:24:11.006746 peltak-changelog-0.0.4/PKG-INFO
```

### Comparing `peltak-changelog-0.0.3/LICENSE` & `peltak-changelog-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `peltak-changelog-0.0.3/pyproject.toml` & `peltak-changelog-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "peltak-changelog"
-version = "0.0.3"
+version = "0.0.4"
 description = ""
 authors = ["Mateusz Klos <novopl@gmail.com>"]
 repository = "https://github.com/novopl/peltak-changelog"
 homepage = "https://novopl.github.io/peltak-changelog"
 documentation = "https://novopl.github.io/peltak-changelog"
 license = "Proprietary"
 packages = [
@@ -68,14 +68,16 @@
 enable = [
     # 'missing-docstring',
     'redefined-builtin',
     'wrong-import-order',
 ]
 
 
+
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 ##################
 #     PYTEST     #
```

### Comparing `peltak-changelog-0.0.3/src/peltak_changelog/__init__.py` & `peltak-changelog-0.0.4/src/peltak_changelog/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,8 +90,8 @@
         - header: 'Fixes'
           tag: 'fix'
 
 """
 from .commands import changelog_cli  # noqa: F401
 
 
-__version__ = '0.0.3'
+__version__ = '0.0.4'
```

### Comparing `peltak-changelog-0.0.3/src/peltak_changelog/commands.py` & `peltak-changelog-0.0.4/src/peltak_changelog/commands.py`

 * *Files identical despite different names*

### Comparing `peltak-changelog-0.0.3/src/peltak_changelog/logic.py` & `peltak-changelog-0.0.4/src/peltak_changelog/logic.py`

 * *Files identical despite different names*

### Comparing `peltak-changelog-0.0.3/src/peltak_changelog/types.py` & `peltak-changelog-0.0.4/src/peltak_changelog/types.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,29 +9,28 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """ Types and classes used by `peltak.extra.changelog`. """
+import dataclasses
 from typing import Any, Dict, List
 
-import attr
-
 
 ChangelogItems = Dict[str, List[Any]]
 
 
-@attr.s
-class ChangelogTag(object):
+@dataclasses.dataclass
+class ChangelogTag:
     """ Changelog tag config.
 
     This is used to map the tags used in commit message details to the actual
     headers used in the generated changelog.
 
     Attributes:
         header (str):   The header used in the generated changelog.
         tag (str):      The tag used in commit message details.
 
     """
-    header = attr.ib(type=str)
-    tag = attr.ib(type=str)
+    header: str
+    tag: str
```

### Comparing `peltak-changelog-0.0.3/setup.py` & `peltak-changelog-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['peltak_changelog']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'peltak-changelog',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': '',
     'long_description': None,
     'author': 'Mateusz Klos',
     'author_email': 'novopl@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://novopl.github.io/peltak-changelog',
```

### Comparing `peltak-changelog-0.0.3/PKG-INFO` & `peltak-changelog-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peltak-changelog
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 Home-page: https://novopl.github.io/peltak-changelog
 License: Proprietary
 Author: Mateusz Klos
 Author-email: novopl@gmail.com
 Requires-Python: >=3.7.2,<4.0
 Classifier: License :: Other/Proprietary License
```

