# Comparing `tmp/flake8_annotations-3.0.0.tar.gz` & `tmp/flake8_annotations-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_annotations-3.0.0.tar", max compression
+gzip compressed data, was "flake8_annotations-3.0.1.tar", max compression
```

## Comparing `flake8_annotations-3.0.0.tar` & `flake8_annotations-3.0.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     7365 2023-01-22 20:35:35.986265 flake8_annotations-3.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1073 2023-01-22 20:35:35.986265 flake8_annotations-3.0.0/LICENSE
--rw-r--r--   0        0        0    10662 2023-01-22 20:35:35.986265 flake8_annotations-3.0.0/README.md
--rw-r--r--   0        0        0       22 2023-01-22 20:35:35.986265 flake8_annotations-3.0.0/flake8_annotations/__init__.py
--rw-r--r--   0        0        0    17378 2023-01-22 20:35:35.986265 flake8_annotations-3.0.0/flake8_annotations/ast_walker.py
--rw-r--r--   0        0        0    12896 2023-01-22 20:35:35.986265 flake8_annotations-3.0.0/flake8_annotations/checker.py
--rw-r--r--   0        0        0      893 2023-01-22 20:35:35.986265 flake8_annotations-3.0.0/flake8_annotations/enums.py
--rw-r--r--   0        0        0     6046 2023-01-22 20:35:35.986265 flake8_annotations-3.0.0/flake8_annotations/error_codes.py
--rw-r--r--   0        0        0     2371 2023-01-22 20:35:35.986265 flake8_annotations-3.0.0/pyproject.toml
--rw-r--r--   0        0        0    11700 1970-01-01 00:00:00.000000 flake8_annotations-3.0.0/setup.py
--rw-r--r--   0        0        0    12186 1970-01-01 00:00:00.000000 flake8_annotations-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     7437 2023-05-03 02:44:35.950697 flake8_annotations-3.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1073 2023-05-03 02:44:35.950697 flake8_annotations-3.0.1/LICENSE
+-rw-r--r--   0        0        0    10787 2023-05-03 02:44:35.950697 flake8_annotations-3.0.1/README.md
+-rw-r--r--   0        0        0       22 2023-05-03 02:44:35.950697 flake8_annotations-3.0.1/flake8_annotations/__init__.py
+-rw-r--r--   0        0        0    17378 2023-05-03 02:44:35.950697 flake8_annotations-3.0.1/flake8_annotations/ast_walker.py
+-rw-r--r--   0        0        0    12896 2023-05-03 02:44:35.950697 flake8_annotations-3.0.1/flake8_annotations/checker.py
+-rw-r--r--   0        0        0      893 2023-05-03 02:44:35.950697 flake8_annotations-3.0.1/flake8_annotations/enums.py
+-rw-r--r--   0        0        0     6046 2023-05-03 02:44:35.950697 flake8_annotations-3.0.1/flake8_annotations/error_codes.py
+-rw-r--r--   0        0        0     2398 2023-05-03 02:44:35.954697 flake8_annotations-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0    12304 1970-01-01 00:00:00.000000 flake8_annotations-3.0.1/PKG-INFO
```

### Comparing `flake8_annotations-3.0.0/CHANGELOG.md` & `flake8_annotations-3.0.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # Changelog
 Versions follow [Semantic Versioning](https://semver.org/spec/v2.0.0.html) (`<major>`.`<minor>`.`<patch>`)
 
+## [v3.0.1]
+### Changed
+* #155 Remove upper bound on Python constraint
+
 ## [v3.0.0]
 ### Added
 * Add `ANN402` for the presence of type comments
 ### Changed
 * Python 3.8.1 is now the minimum supported version
 * Flake8 v5.0 is now the minimum supported version
```

### Comparing `flake8_annotations-3.0.0/LICENSE` & `flake8_annotations-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_annotations-3.0.0/README.md` & `flake8_annotations-3.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # flake8-annotations
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flake8-annotations/3.0.0?logo=python&logoColor=FFD43B)](https://pypi.org/project/flake8-annotations/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flake8-annotations/3.0.1?logo=python&logoColor=FFD43B)](https://pypi.org/project/flake8-annotations/)
 [![PyPI](https://img.shields.io/pypi/v/flake8-annotations?logo=Python&logoColor=FFD43B)](https://pypi.org/project/flake8-annotations/)
 [![PyPI - License](https://img.shields.io/pypi/l/flake8-annotations?color=magenta)](https://github.com/sco1/flake8-annotations/blob/main/LICENSE)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sco1/flake8-annotations/main.svg)](https://results.pre-commit.ci/latest/github/sco1/flake8-annotations/main)
 [![Open in Visual Studio Code](https://img.shields.io/badge/Open%20in-VSCode.dev-blue)](https://github.dev/sco1/flake8-annotations)
 
 `flake8-annotations` is a plugin for [Flake8](http://flake8.pycqa.org/en/latest/) that detects the absence of [PEP 3107-style](https://www.python.org/dev/peps/pep-3107/) function annotations.
 
@@ -28,15 +28,15 @@
 ver_str = out.stdout.replace("\n", "")
 cog.out(
     f"```bash\n$ flake8 --version\n{ver_str}\n```"
 )
 ]]] -->
 ```bash
 $ flake8 --version
-6.0.0 (flake8-annotations: 3.0.0, mccabe: 0.7.0, pycodestyle: 2.10.0, pyflakes: 3.0.1) CPython 3.11.0 on Darwin
+6.0.0 (flake8-annotations: 3.0.1, mccabe: 0.7.0, pycodestyle: 2.10.0, pyflakes: 3.0.1) CPython 3.11.0 on Darwin
 ```
 <!-- [[[end]]] -->
 
 ## Table of Warnings
 With the exception of `ANN4xx`-level warnings, all warnings are enabled by default.
 
 ### Function Annotations
@@ -60,25 +60,26 @@
 | `ANN203` | Missing return type annotation for secret function    |
 | `ANN204` | Missing return type annotation for special method     |
 | `ANN205` | Missing return type annotation for staticmethod       |
 | `ANN206` | Missing return type annotation for classmethod        |
 
 ### Opinionated Warnings
 These warnings are disabled by default.
-| ID       | Description                                                            |
-|----------|------------------------------------------------------------------------|
-| `ANN401` | Dynamically typed expressions (typing.Any) are disallowed.<sup>2</sup> |
-| `ANN402` | Type comments are disallowed.                                          |
+| ID       | Description                                                             |
+|----------|-------------------------------------------------------------------------|
+| `ANN401` | Dynamically typed expressions (typing.Any) are disallowed<sup>2,3</sup> |
+| `ANN402` | Type comments are disallowed<sup>3</sup>                                |
 
-Use [`extend-select`](https://flake8.pycqa.org/en/latest/user/options.html#cmdoption-flake8-extend-ignore) to enable opinionated warnings without overriding other implicit configurations<sup>3</sup>.
+Use [`extend-select`](https://flake8.pycqa.org/en/latest/user/options.html#cmdoption-flake8-extend-ignore) to enable opinionated warnings without overriding other implicit configurations<sup>4</sup>.
 
 **Notes:**
 1. See: [PEP 484](https://www.python.org/dev/peps/pep-0484/#annotating-instance-and-class-methods) and [PEP 563](https://www.python.org/dev/peps/pep-0563/) for suggestions on annotating `self` and `cls` arguments
 2. See: [Dynamic Typing Caveats](#dynamic-typing-caveats)
-3. Common pitfall: the use of [`ignore`](https://flake8.pycqa.org/en/latest/user/options.html#cmdoption-flake8-ignore) will enable all implicitly disabled warnings
+3. Only function declarations are considered by this plugin; type annotations in function/module bodies are not checked 
+4. Common pitfall: the use of [`ignore`](https://flake8.pycqa.org/en/latest/user/options.html#cmdoption-flake8-ignore) will enable all implicitly disabled warnings
 
 ## Configuration Options
 Some opinionated flags are provided to tailor the linting errors emitted.
 
 ### `--suppress-none-returning`: `bool`
 Suppress `ANN200`-level errors for functions that meet one of the following criteria:
   * Contain no `return` statement, or
```

### Comparing `flake8_annotations-3.0.0/flake8_annotations/ast_walker.py` & `flake8_annotations-3.0.1/flake8_annotations/ast_walker.py`

 * *Files identical despite different names*

### Comparing `flake8_annotations-3.0.0/flake8_annotations/checker.py` & `flake8_annotations-3.0.1/flake8_annotations/checker.py`

 * *Files identical despite different names*

### Comparing `flake8_annotations-3.0.0/flake8_annotations/enums.py` & `flake8_annotations-3.0.1/flake8_annotations/enums.py`

 * *Files identical despite different names*

### Comparing `flake8_annotations-3.0.0/flake8_annotations/error_codes.py` & `flake8_annotations-3.0.1/flake8_annotations/error_codes.py`

 * *Files identical despite different names*

### Comparing `flake8_annotations-3.0.0/pyproject.toml` & `flake8_annotations-3.0.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flake8-annotations"
-version = "3.0.0"
+version = "3.0.1"
 description = "Flake8 Type Annotation Checks"
 license = "MIT"
 readme = "README.md"
 authors = ["S Co1 <sco1.git@gmail.com>"]
 homepage = "https://github.com/sco1/flake8-annotations"
 repository = "https://github.com/sco1/flake8-annotations"
 classifiers = [
@@ -31,34 +31,34 @@
     {path = "./CHANGELOG.md", format = "sdist"}
 ]
 
 [tool.poetry.urls]
 "Issue Tracker" = "https://github.com/sco1/flake8-annotations/issues"
 
 [tool.poetry.dependencies]
-python = "^3.8.1"
+python = ">=3.8.1"
 attrs = ">=21.4"
 flake8 = ">=5.0"
 
 [tool.poetry.dev-dependencies]
-black = "^22.12"
+black = "^23.1"
 bump2version = "^1.0"
 cogapp = "^3.3"
-flake8-bugbear = "^22.10"
-flake8-docstrings = "^1.6"
+flake8-bugbear = "^23.1"
+flake8-docstrings = "^1.7"
 flake8-fixme = "^1.1"
 isort = "^5.10"
-mypy = "^0.991"
+mypy = "^1.0"
 pep8-naming = "^0.13"
-pre-commit = "^2.20"
+pre-commit = "^3.0"
 pytest = "^7.2"
 pytest-check = "^2.0"
 pytest-cov = "^4.0"
 pytest-randomly = "^3.12"
-tox = "^4.0"
+tox = { version = "^4.4", python = "<4.0" }
 
 [tool.poetry.plugins]
 [tool.poetry.plugins."flake8.extension"]
 "ANN" = "flake8_annotations.checker:TypeHintChecker"
 
 [tool.black]
 line-length = 100
```

### Comparing `flake8_annotations-3.0.0/setup.py` & `flake8_annotations-3.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,263 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: flake8-annotations
+Version: 3.0.1
+Summary: Flake8 Type Annotation Checks
+Home-page: https://github.com/sco1/flake8-annotations
+License: MIT
+Author: S Co1
+Author-email: sco1.git@gmail.com
+Requires-Python: >=3.8.1
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Framework :: Flake8
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Typing :: Typed
+Requires-Dist: attrs (>=21.4)
+Requires-Dist: flake8 (>=5.0)
+Project-URL: Issue Tracker, https://github.com/sco1/flake8-annotations/issues
+Project-URL: Repository, https://github.com/sco1/flake8-annotations
+Description-Content-Type: text/markdown
 
-packages = \
-['flake8_annotations']
+# flake8-annotations
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flake8-annotations/3.0.1?logo=python&logoColor=FFD43B)](https://pypi.org/project/flake8-annotations/)
+[![PyPI](https://img.shields.io/pypi/v/flake8-annotations?logo=Python&logoColor=FFD43B)](https://pypi.org/project/flake8-annotations/)
+[![PyPI - License](https://img.shields.io/pypi/l/flake8-annotations?color=magenta)](https://github.com/sco1/flake8-annotations/blob/main/LICENSE)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sco1/flake8-annotations/main.svg)](https://results.pre-commit.ci/latest/github/sco1/flake8-annotations/main)
+[![Open in Visual Studio Code](https://img.shields.io/badge/Open%20in-VSCode.dev-blue)](https://github.dev/sco1/flake8-annotations)
 
-package_data = \
-{'': ['*']}
+`flake8-annotations` is a plugin for [Flake8](http://flake8.pycqa.org/en/latest/) that detects the absence of [PEP 3107-style](https://www.python.org/dev/peps/pep-3107/) function annotations.
 
-install_requires = \
-['attrs>=21.4', 'flake8>=5.0']
-
-entry_points = \
-{'flake8.extension': ['ANN = flake8_annotations.checker:TypeHintChecker']}
-
-setup_kwargs = {
-    'name': 'flake8-annotations',
-    'version': '3.0.0',
-    'description': 'Flake8 Type Annotation Checks',
-    'long_description': '# flake8-annotations\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flake8-annotations/3.0.0?logo=python&logoColor=FFD43B)](https://pypi.org/project/flake8-annotations/)\n[![PyPI](https://img.shields.io/pypi/v/flake8-annotations?logo=Python&logoColor=FFD43B)](https://pypi.org/project/flake8-annotations/)\n[![PyPI - License](https://img.shields.io/pypi/l/flake8-annotations?color=magenta)](https://github.com/sco1/flake8-annotations/blob/main/LICENSE)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sco1/flake8-annotations/main.svg)](https://results.pre-commit.ci/latest/github/sco1/flake8-annotations/main)\n[![Open in Visual Studio Code](https://img.shields.io/badge/Open%20in-VSCode.dev-blue)](https://github.dev/sco1/flake8-annotations)\n\n`flake8-annotations` is a plugin for [Flake8](http://flake8.pycqa.org/en/latest/) that detects the absence of [PEP 3107-style](https://www.python.org/dev/peps/pep-3107/) function annotations.\n\nWhat this won\'t do: replace [mypy](http://mypy-lang.org/), check type comments (see: [PEP 484](https://peps.python.org/pep-0484/#type-comments)), check variable annotations (see: [PEP 526](https://www.python.org/dev/peps/pep-0526/)), or respect stub files.\n\n## Installation\nInstall from PyPi with your favorite `pip` invocation:\n\n```bash\n$ pip install flake8-annotations\n```\n\nIt will then be run automatically as part of flake8.\n\nYou can verify it\'s being picked up by invoking the following in your shell:\n\n\n<!-- [[[cog\nimport cog\nfrom subprocess import PIPE, run\nout = run(["flake8", "--version"], stdout=PIPE, encoding="ascii")\nver_str = out.stdout.replace("\\n", "")\ncog.out(\n    f"```bash\\n$ flake8 --version\\n{ver_str}\\n```"\n)\n]]] -->\n```bash\n$ flake8 --version\n6.0.0 (flake8-annotations: 3.0.0, mccabe: 0.7.0, pycodestyle: 2.10.0, pyflakes: 3.0.1) CPython 3.11.0 on Darwin\n```\n<!-- [[[end]]] -->\n\n## Table of Warnings\nWith the exception of `ANN4xx`-level warnings, all warnings are enabled by default.\n\n### Function Annotations\n| ID       | Description                                   |\n|----------|-----------------------------------------------|\n| `ANN001` | Missing type annotation for function argument |\n| `ANN002` | Missing type annotation for `*args`           |\n| `ANN003` | Missing type annotation for `**kwargs`        |\n\n### Method Annotations\n| ID       | Description                                                  |\n|----------|--------------------------------------------------------------|\n| `ANN101` | Missing type annotation for `self` in method<sup>1</sup>     |\n| `ANN102` | Missing type annotation for `cls` in classmethod<sup>1</sup> |\n\n### Return Annotations\n| ID       | Description                                           |\n|----------|-------------------------------------------------------|\n| `ANN201` | Missing return type annotation for public function    |\n| `ANN202` | Missing return type annotation for protected function |\n| `ANN203` | Missing return type annotation for secret function    |\n| `ANN204` | Missing return type annotation for special method     |\n| `ANN205` | Missing return type annotation for staticmethod       |\n| `ANN206` | Missing return type annotation for classmethod        |\n\n### Opinionated Warnings\nThese warnings are disabled by default.\n| ID       | Description                                                            |\n|----------|------------------------------------------------------------------------|\n| `ANN401` | Dynamically typed expressions (typing.Any) are disallowed.<sup>2</sup> |\n| `ANN402` | Type comments are disallowed.                                          |\n\nUse [`extend-select`](https://flake8.pycqa.org/en/latest/user/options.html#cmdoption-flake8-extend-ignore) to enable opinionated warnings without overriding other implicit configurations<sup>3</sup>.\n\n**Notes:**\n1. See: [PEP 484](https://www.python.org/dev/peps/pep-0484/#annotating-instance-and-class-methods) and [PEP 563](https://www.python.org/dev/peps/pep-0563/) for suggestions on annotating `self` and `cls` arguments\n2. See: [Dynamic Typing Caveats](#dynamic-typing-caveats)\n3. Common pitfall: the use of [`ignore`](https://flake8.pycqa.org/en/latest/user/options.html#cmdoption-flake8-ignore) will enable all implicitly disabled warnings\n\n## Configuration Options\nSome opinionated flags are provided to tailor the linting errors emitted.\n\n### `--suppress-none-returning`: `bool`\nSuppress `ANN200`-level errors for functions that meet one of the following criteria:\n  * Contain no `return` statement, or\n  * Explicit `return` statement(s) all return `None` (explicitly or implicitly).\n\nDefault: `False`\n\n### `--suppress-dummy-args`: `bool`\nSuppress `ANN000`-level errors for dummy arguments, defined as `_`.\n\nDefault: `False`\n\n### `--allow-untyped-defs`: `bool`\nSuppress all errors for dynamically typed functions. A function is considered dynamically typed if it does not contain any type hints.\n\nDefault: `False`\n\n### `--allow-untyped-nested`: `bool`\nSuppress all errors for dynamically typed nested functions. A function is considered dynamically typed if it does not contain any type hints.\n\nDefault: `False`\n\n### `--mypy-init-return`: `bool`\nAllow omission of a return type hint for `__init__` if at least one argument is annotated. See [mypy\'s documentation](https://mypy.readthedocs.io/en/stable/class_basics.html?#annotating-init-methods) for additional details.\n\nDefault: `False`\n\n### `--dispatch-decorators`: `list[str]`\nComma-separated list of decorators flake8-annotations should consider as dispatch decorators. Linting errors are suppressed for functions decorated with at least one of these functions.\n\nDecorators are matched based on their attribute name. For example, `"singledispatch"` will match any of the following:\n  * `import functools; @functools.singledispatch`\n  * `import functools as <alias>; @<alias>.singledispatch`\n  * `from functools import singledispatch; @singledispatch`\n\n**NOTE:** Deeper imports, such as `a.b.singledispatch` are not supported.\n\nSee: [Generic Functions](#generic-functions) for additional information.\n\nDefault: `"singledispatch, singledispatchmethod"`\n\n### `--overload-decorators`: `list[str]`\nComma-separated list of decorators flake8-annotations should consider as [`typing.overload`](https://docs.python.org/3/library/typing.html#typing.overload) decorators.\n\nDecorators are matched based on their attribute name. For example, `"overload"` will match any of the following:\n  * `import typing; @typing.overload`\n  * `import typing as <alias>; @<alias>.overload`\n  * `from typing import overload; @overload`\n\n**NOTE:** Deeper imports, such as `a.b.overload` are not supported.\n\nSee: [The `typing.overload` Decorator](#the-typingoverload-decorator) for additional information.\n\nDefault: `"overload"`\n\n### `--allow-star-arg-any`\nSuppress `ANN401` for dynamically typed `*args` and `**kwargs`.\n\nDefault: `False`\n\n## Generic Functions\nPer the Python Glossary, a [generic function](https://docs.python.org/3/glossary.html#term-generic-function) is defined as:\n\n> A function composed of multiple functions implementing the same operation for different types. Which implementation should be used during a call is determined by the dispatch algorithm.\n\nIn the standard library we have some examples of decorators for implementing these generic functions: [`functools.singledispatch`](https://docs.python.org/3/library/functools.html#functools.singledispatch) and [`functools.singledispatchmethod`](https://docs.python.org/3/library/functools.html#functools.singledispatchmethod). In the spirit of the purpose of these decorators, errors for missing annotations for functions decorated with at least one of these are ignored.\n\nFor example, this code:\n\n```py\nimport functools\n\n@functools.singledispatch\ndef foo(a):\n    print(a)\n\n@foo.register\ndef _(a: list) -> None:\n    for idx, thing in enumerate(a):\n        print(idx, thing)\n```\n\nWill not raise any linting errors for `foo`.\n\nDecorator(s) to treat as defining generic functions may be specified by the [`--dispatch-decorators`](#--dispatch-decorators-liststr) configuration option.\n\n## The `typing.overload` Decorator\nPer the [`typing`](https://docs.python.org/3/library/typing.html#typing.overload) documentation:\n\n> The `@overload` decorator allows describing functions and methods that support multiple different combinations of argument types. A series of `@overload`-decorated definitions must be followed by exactly one non-`@overload`-decorated definition (for the same function/method).\n\nIn the spirit of the purpose of this decorator, errors for missing annotations for non-`@overload`-decorated functions are ignored if they meet this criteria.\n\nFor example, this code:\n\n```py\nimport typing\n\n\n@typing.overload\ndef foo(a: int) -> int:\n    ...\n\ndef foo(a):\n    ...\n```\n\nWill not raise linting errors for missing annotations for the arguments & return of the non-decorated `foo` definition.\n\nDecorator(s) to treat as `typing.overload` may be specified by the [`--overload-decorators`](#--overload-decorators-liststr) configuration option.\n\n## Dynamic Typing Caveats\nSupport is only provided for the following patterns:\n  * `from typing import any; foo: Any`\n  * `import typing; foo: typing.Any`\n  * `import typing as <alias>; foo: <alias>.Any`\n\nNested dynamic types (e.g. `typing.Tuple[typing.Any]`) and redefinition (e.g. `from typing import Any as Foo`) will not be identified.\n\n## Contributing\n\n### Development Environment\nThis project uses [Poetry](https://python-poetry.org/) to manage dependencies. With your fork cloned to your local machine, you can install the project and its dependencies to create a development environment using:\n\n```bash\n$ poetry install\n```\n\nNote: An editable installation of `flake8-annotations` in the developer environment is required in order for the plugin to be registered for Flake8. By default, Poetry includes an editable install of the project itself when `poetry install` is invoked.\n\nA [pre-commit](https://pre-commit.com) configuration is also provided to create a pre-commit hook so linting errors aren\'t committed:\n\n```bash\n$ pre-commit install\n```\n\n### Testing & Coverage\nA [pytest](https://docs.pytest.org/en/latest/) suite is provided, with coverage reporting from [pytest-cov](https://github.com/pytest-dev/pytest-cov). A [tox](https://github.com/tox-dev/tox/) configuration is provided to test across all supported versions of Python. Testing will be skipped for Python versions that cannot be found.\n\n```bash\n$ tox\n```\n\nDetails on missing coverage, including in the test suite, is provided in the report to allow the user to generate additional tests for full coverage.\n',
-    'author': 'S Co1',
-    'author_email': 'sco1.git@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/sco1/flake8-annotations',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8.1,<4.0.0',
-}
+What this won't do: replace [mypy](http://mypy-lang.org/), check type comments (see: [PEP 484](https://peps.python.org/pep-0484/#type-comments)), check variable annotations (see: [PEP 526](https://www.python.org/dev/peps/pep-0526/)), or respect stub files.
 
+## Installation
+Install from PyPi with your favorite `pip` invocation:
+
+```bash
+$ pip install flake8-annotations
+```
+
+It will then be run automatically as part of flake8.
+
+You can verify it's being picked up by invoking the following in your shell:
+
+
+<!-- [[[cog
+import cog
+from subprocess import PIPE, run
+out = run(["flake8", "--version"], stdout=PIPE, encoding="ascii")
+ver_str = out.stdout.replace("\n", "")
+cog.out(
+    f"```bash\n$ flake8 --version\n{ver_str}\n```"
+)
+]]] -->
+```bash
+$ flake8 --version
+6.0.0 (flake8-annotations: 3.0.1, mccabe: 0.7.0, pycodestyle: 2.10.0, pyflakes: 3.0.1) CPython 3.11.0 on Darwin
+```
+<!-- [[[end]]] -->
+
+## Table of Warnings
+With the exception of `ANN4xx`-level warnings, all warnings are enabled by default.
+
+### Function Annotations
+| ID       | Description                                   |
+|----------|-----------------------------------------------|
+| `ANN001` | Missing type annotation for function argument |
+| `ANN002` | Missing type annotation for `*args`           |
+| `ANN003` | Missing type annotation for `**kwargs`        |
+
+### Method Annotations
+| ID       | Description                                                  |
+|----------|--------------------------------------------------------------|
+| `ANN101` | Missing type annotation for `self` in method<sup>1</sup>     |
+| `ANN102` | Missing type annotation for `cls` in classmethod<sup>1</sup> |
+
+### Return Annotations
+| ID       | Description                                           |
+|----------|-------------------------------------------------------|
+| `ANN201` | Missing return type annotation for public function    |
+| `ANN202` | Missing return type annotation for protected function |
+| `ANN203` | Missing return type annotation for secret function    |
+| `ANN204` | Missing return type annotation for special method     |
+| `ANN205` | Missing return type annotation for staticmethod       |
+| `ANN206` | Missing return type annotation for classmethod        |
+
+### Opinionated Warnings
+These warnings are disabled by default.
+| ID       | Description                                                             |
+|----------|-------------------------------------------------------------------------|
+| `ANN401` | Dynamically typed expressions (typing.Any) are disallowed<sup>2,3</sup> |
+| `ANN402` | Type comments are disallowed<sup>3</sup>                                |
+
+Use [`extend-select`](https://flake8.pycqa.org/en/latest/user/options.html#cmdoption-flake8-extend-ignore) to enable opinionated warnings without overriding other implicit configurations<sup>4</sup>.
+
+**Notes:**
+1. See: [PEP 484](https://www.python.org/dev/peps/pep-0484/#annotating-instance-and-class-methods) and [PEP 563](https://www.python.org/dev/peps/pep-0563/) for suggestions on annotating `self` and `cls` arguments
+2. See: [Dynamic Typing Caveats](#dynamic-typing-caveats)
+3. Only function declarations are considered by this plugin; type annotations in function/module bodies are not checked 
+4. Common pitfall: the use of [`ignore`](https://flake8.pycqa.org/en/latest/user/options.html#cmdoption-flake8-ignore) will enable all implicitly disabled warnings
+
+## Configuration Options
+Some opinionated flags are provided to tailor the linting errors emitted.
+
+### `--suppress-none-returning`: `bool`
+Suppress `ANN200`-level errors for functions that meet one of the following criteria:
+  * Contain no `return` statement, or
+  * Explicit `return` statement(s) all return `None` (explicitly or implicitly).
+
+Default: `False`
+
+### `--suppress-dummy-args`: `bool`
+Suppress `ANN000`-level errors for dummy arguments, defined as `_`.
+
+Default: `False`
+
+### `--allow-untyped-defs`: `bool`
+Suppress all errors for dynamically typed functions. A function is considered dynamically typed if it does not contain any type hints.
+
+Default: `False`
+
+### `--allow-untyped-nested`: `bool`
+Suppress all errors for dynamically typed nested functions. A function is considered dynamically typed if it does not contain any type hints.
+
+Default: `False`
+
+### `--mypy-init-return`: `bool`
+Allow omission of a return type hint for `__init__` if at least one argument is annotated. See [mypy's documentation](https://mypy.readthedocs.io/en/stable/class_basics.html?#annotating-init-methods) for additional details.
+
+Default: `False`
+
+### `--dispatch-decorators`: `list[str]`
+Comma-separated list of decorators flake8-annotations should consider as dispatch decorators. Linting errors are suppressed for functions decorated with at least one of these functions.
+
+Decorators are matched based on their attribute name. For example, `"singledispatch"` will match any of the following:
+  * `import functools; @functools.singledispatch`
+  * `import functools as <alias>; @<alias>.singledispatch`
+  * `from functools import singledispatch; @singledispatch`
+
+**NOTE:** Deeper imports, such as `a.b.singledispatch` are not supported.
+
+See: [Generic Functions](#generic-functions) for additional information.
+
+Default: `"singledispatch, singledispatchmethod"`
+
+### `--overload-decorators`: `list[str]`
+Comma-separated list of decorators flake8-annotations should consider as [`typing.overload`](https://docs.python.org/3/library/typing.html#typing.overload) decorators.
+
+Decorators are matched based on their attribute name. For example, `"overload"` will match any of the following:
+  * `import typing; @typing.overload`
+  * `import typing as <alias>; @<alias>.overload`
+  * `from typing import overload; @overload`
+
+**NOTE:** Deeper imports, such as `a.b.overload` are not supported.
+
+See: [The `typing.overload` Decorator](#the-typingoverload-decorator) for additional information.
+
+Default: `"overload"`
+
+### `--allow-star-arg-any`
+Suppress `ANN401` for dynamically typed `*args` and `**kwargs`.
+
+Default: `False`
+
+## Generic Functions
+Per the Python Glossary, a [generic function](https://docs.python.org/3/glossary.html#term-generic-function) is defined as:
+
+> A function composed of multiple functions implementing the same operation for different types. Which implementation should be used during a call is determined by the dispatch algorithm.
+
+In the standard library we have some examples of decorators for implementing these generic functions: [`functools.singledispatch`](https://docs.python.org/3/library/functools.html#functools.singledispatch) and [`functools.singledispatchmethod`](https://docs.python.org/3/library/functools.html#functools.singledispatchmethod). In the spirit of the purpose of these decorators, errors for missing annotations for functions decorated with at least one of these are ignored.
+
+For example, this code:
+
+```py
+import functools
+
+@functools.singledispatch
+def foo(a):
+    print(a)
+
+@foo.register
+def _(a: list) -> None:
+    for idx, thing in enumerate(a):
+        print(idx, thing)
+```
+
+Will not raise any linting errors for `foo`.
+
+Decorator(s) to treat as defining generic functions may be specified by the [`--dispatch-decorators`](#--dispatch-decorators-liststr) configuration option.
+
+## The `typing.overload` Decorator
+Per the [`typing`](https://docs.python.org/3/library/typing.html#typing.overload) documentation:
+
+> The `@overload` decorator allows describing functions and methods that support multiple different combinations of argument types. A series of `@overload`-decorated definitions must be followed by exactly one non-`@overload`-decorated definition (for the same function/method).
+
+In the spirit of the purpose of this decorator, errors for missing annotations for non-`@overload`-decorated functions are ignored if they meet this criteria.
+
+For example, this code:
+
+```py
+import typing
+
+
+@typing.overload
+def foo(a: int) -> int:
+    ...
+
+def foo(a):
+    ...
+```
+
+Will not raise linting errors for missing annotations for the arguments & return of the non-decorated `foo` definition.
+
+Decorator(s) to treat as `typing.overload` may be specified by the [`--overload-decorators`](#--overload-decorators-liststr) configuration option.
+
+## Dynamic Typing Caveats
+Support is only provided for the following patterns:
+  * `from typing import any; foo: Any`
+  * `import typing; foo: typing.Any`
+  * `import typing as <alias>; foo: <alias>.Any`
+
+Nested dynamic types (e.g. `typing.Tuple[typing.Any]`) and redefinition (e.g. `from typing import Any as Foo`) will not be identified.
+
+## Contributing
+
+### Development Environment
+This project uses [Poetry](https://python-poetry.org/) to manage dependencies. With your fork cloned to your local machine, you can install the project and its dependencies to create a development environment using:
+
+```bash
+$ poetry install
+```
+
+Note: An editable installation of `flake8-annotations` in the developer environment is required in order for the plugin to be registered for Flake8. By default, Poetry includes an editable install of the project itself when `poetry install` is invoked.
+
+A [pre-commit](https://pre-commit.com) configuration is also provided to create a pre-commit hook so linting errors aren't committed:
+
+```bash
+$ pre-commit install
+```
+
+### Testing & Coverage
+A [pytest](https://docs.pytest.org/en/latest/) suite is provided, with coverage reporting from [pytest-cov](https://github.com/pytest-dev/pytest-cov). A [tox](https://github.com/tox-dev/tox/) configuration is provided to test across all supported versions of Python. Testing will be skipped for Python versions that cannot be found.
+
+```bash
+$ tox
+```
+
+Details on missing coverage, including in the test suite, is provided in the report to allow the user to generate additional tests for full coverage.
 
-setup(**setup_kwargs)
```

