# Comparing `tmp/cmeel-0.8.0.tar.gz` & `tmp/cmeel-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmeel-0.8.0.tar", max compression
+gzip compressed data, was "cmeel-0.9.0.tar", max compression
```

## Comparing `cmeel-0.8.0.tar` & `cmeel-0.9.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1494 2022-05-28 20:33:43.194099 cmeel-0.8.0/README.md
--rw-r--r--   0        0        0       22 2022-05-28 20:33:43.194099 cmeel-0.8.0/cmeel/__init__.py
--rw-r--r--   0        0        0     4393 2022-05-28 20:33:43.194099 cmeel-0.8.0/cmeel/build.py
--rw-r--r--   0        0        0     2408 2022-05-28 20:33:43.194099 cmeel-0.8.0/cmeel/config.py
--rw-r--r--   0        0        0      155 2022-05-28 20:33:43.194099 cmeel-0.8.0/cmeel/consts.py
--rw-r--r--   0        0        0      156 2022-05-28 20:33:43.194099 cmeel-0.8.0/cmeel/pth.py
--rw-r--r--   0        0        0       17 2022-05-28 20:33:43.194099 cmeel-0.8.0/cmeel.pth
--rw-r--r--   0        0        0      635 2022-05-28 20:33:43.194099 cmeel-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2330 2022-05-28 20:33:50.321076 cmeel-0.8.0/setup.py
--rw-r--r--   0        0        0     2268 2022-05-28 20:33:50.321416 cmeel-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1756 2022-05-31 20:43:51.998556 cmeel-0.9.0/README.md
+-rw-r--r--   0        0        0       22 2022-05-31 20:43:51.998556 cmeel-0.9.0/cmeel/__init__.py
+-rw-r--r--   0        0        0     4775 2022-05-31 20:43:51.998556 cmeel-0.9.0/cmeel/build.py
+-rw-r--r--   0        0        0     2459 2022-05-31 20:43:51.998556 cmeel-0.9.0/cmeel/config.py
+-rw-r--r--   0        0        0      155 2022-05-31 20:43:51.998556 cmeel-0.9.0/cmeel/consts.py
+-rw-r--r--   0        0        0      156 2022-05-31 20:43:51.998556 cmeel-0.9.0/cmeel/pth.py
+-rw-r--r--   0        0        0      676 2022-05-31 20:43:51.998556 cmeel-0.9.0/cmeel/run.py
+-rw-r--r--   0        0        0       17 2022-05-31 20:43:51.998556 cmeel-0.9.0/cmeel.pth
+-rw-r--r--   0        0        0      635 2022-05-31 20:43:52.002557 cmeel-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2594 2022-05-31 20:44:00.193622 cmeel-0.9.0/setup.py
+-rw-r--r--   0        0        0     2530 2022-05-31 20:44:00.193950 cmeel-0.9.0/PKG-INFO
```

### Comparing `cmeel-0.8.0/README.md` & `cmeel-0.9.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # CMake Wheels
 
 [![PyPI version](https://badge.fury.io/py/cmeel.svg)](https://pypi.org/project/cmeel)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/cmake-wheel/cmeel/main.svg)](https://results.pre-commit.ci/latest/github/cmake-wheel/cmeel/main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-Pip build backend using CMake.
+Wheel build backend using CMake, to package anything with pip and distribut on PyPI.
 
 Following those relevant PEPs:
+- [PEP 427](https://peps.python.org/pep-0427/), The Wheel Binary Package Format 1.0
 - [PEP 517](https://peps.python.org/pep-0517/), A build-system independent format for source trees
 - [PEP 518](https://peps.python.org/pep-0518/), Specifying Minimum Build System Requirements for Python Projects
+- [PEP 600](https://peps.python.org/pep-0600/), Future ‘manylinux’ Platform Tags for Portable Linux Built Distributions
 - [PEP 621](https://peps.python.org/pep-0621/), Storing project metadata in pyproject.toml
 
 ## Basic idea
 
 - Glue between PEP 517 `build_wheel` function and modern CMake standard project configuration / build / test / install
 - Install in `${PYTHON_SITELIB}/cmeel.prefix/`
     - As there is a dot, it is not a valid python module name, so no risk of importing anything there by mistake
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cmeel-0.8.0/cmeel/build.py` & `cmeel-0.9.0/cmeel/build.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,19 @@
     raise ImportError(err) from e
 import tomli
 
 from .consts import CMEEL_PREFIX
 from .config import cmeel_config
 from . import __version__
 
+EXECUTABLE = """#!python
+from cmeel.run import cmeel_run
+cmeel_run()
+"""
+
 
 def build_wheel(wheel_directory, config_settings=None, metadata_directory=None):
     logging.info("CMake Wheel")
 
     TEMP = Path(TemporaryDirectory(prefix="cmeel-").name)
     BUILD = TEMP / "bld"
     PREFIX = TEMP / "pfx"
@@ -114,17 +119,24 @@
                     f"Generator: cmeel {__version__}",
                     "Root-Is-Purelib: false",
                     f"Tag: {TAG}",
                 ]
             )
         )
 
-    if (INSTALL / "bin").is_dir():
-        logging.info("adding entrypoint")
-        # TODO
+    BIN = INSTALL / "bin"
+    if BIN.is_dir():
+        logging.info("adding executables")
+        scripts = PREFIX / f"{DISTRIBUTION}-{CONF['version']}.data" / "scripts"
+        scripts.mkdir(parents=True)
+        for fn in BIN.glob("*"):
+            executable = scripts / fn.name
+            with executable.open("w") as fe:
+                fe.write(EXECUTABLE)
+            executable.chmod(0o755)
 
     logging.info("wheel pack")
     name = check_output(
         [sys.executable, "-m", "wheel", "pack", "-d", wheel_directory, PREFIX]
     ).decode()
     name = name.split("/")[-1][:-6]
```

### Comparing `cmeel-0.8.0/cmeel/config.py` & `cmeel-0.9.0/cmeel/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,15 @@
                 "-DBoost_NO_WARN_NEW_VERSIONS=ON",
                 "-DCMAKE_BUILD_TYPE=Release",
                 f"-DCMAKE_INSTALL_PREFIX={install}",
                 f"-DPYTHON_EXECUTABLE={sys.executable}",
                 f"-DPython3_INCLUDE_DIR={distutils.sysconfig.get_python_inc()}",
                 f"-DPYTHON_INCLUDE_DIRS={distutils.sysconfig.get_python_inc()}",
                 f"-DPYTHON_SITELIB={SITELIB}",
+                "-DPYTHON_COMPONENTS=Interpreter",
             ]
             + conf.get("configure_args", [])
             + self.conf.get("configure_args", [])
         )
         if project in self.conf:
             ret += self.conf[project].get("configure_args", [])
         return ret
```

### Comparing `cmeel-0.8.0/pyproject.toml` & `cmeel-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmeel"
-version = "0.8.0"
+version = "0.9.0"
 description = "Create Wheel from CMake projects"
 authors = ["Guilhem Saurel <guilhem.saurel@laas.fr>"]
 license = "BSD-2-Clause"
 readme = "README.md"
 include = ['cmeel.pth']
 homepage = "https://github.com/cmake-wheel/cmeel"
```

### Comparing `cmeel-0.8.0/setup.py` & `cmeel-0.9.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 extras_require = \
 {'build': ['cmake>=3.22.3,<4.0.0',
            'packaging>=21.3,<22.0',
            'wheel>=0.37.1,<0.38.0']}
 
 setup_kwargs = {
     'name': 'cmeel',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Create Wheel from CMake projects',
-    'long_description': '# CMake Wheels\n\n[![PyPI version](https://badge.fury.io/py/cmeel.svg)](https://pypi.org/project/cmeel)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/cmake-wheel/cmeel/main.svg)](https://results.pre-commit.ci/latest/github/cmake-wheel/cmeel/main)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\nPip build backend using CMake.\n\nFollowing those relevant PEPs:\n- [PEP 517](https://peps.python.org/pep-0517/), A build-system independent format for source trees\n- [PEP 518](https://peps.python.org/pep-0518/), Specifying Minimum Build System Requirements for Python Projects\n- [PEP 621](https://peps.python.org/pep-0621/), Storing project metadata in pyproject.toml\n\n## Basic idea\n\n- Glue between PEP 517 `build_wheel` function and modern CMake standard project configuration / build / test / install\n- Install in `${PYTHON_SITELIB}/cmeel.prefix/`\n    - As there is a dot, it is not a valid python module name, so no risk of importing anything there by mistake\n    - `${PYTHON_SITELIB}/cmeel.pth` automatically load `${PYTHON_SITELIB}/cmeel.prefix/${PYTHON_SITELIB}`, so python\n      packages work out of the box\n    - Existing `${PYTHON_SITELIB}/cmeel.prefix` are automatically added to `$CMAKE_PREFIX_PATH`, so we can build CMake\n      packages whose dependencies are provided by other CMake packages installed with cmeel\n    - Stuff in `${PYTHON_SITELIB}/cmeel.prefix/bin` gets wrapped into entrypoints (TODO)\n',
+    'long_description': '# CMake Wheels\n\n[![PyPI version](https://badge.fury.io/py/cmeel.svg)](https://pypi.org/project/cmeel)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/cmake-wheel/cmeel/main.svg)](https://results.pre-commit.ci/latest/github/cmake-wheel/cmeel/main)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\nWheel build backend using CMake, to package anything with pip and distribut on PyPI.\n\nFollowing those relevant PEPs:\n- [PEP 427](https://peps.python.org/pep-0427/), The Wheel Binary Package Format 1.0\n- [PEP 517](https://peps.python.org/pep-0517/), A build-system independent format for source trees\n- [PEP 518](https://peps.python.org/pep-0518/), Specifying Minimum Build System Requirements for Python Projects\n- [PEP 600](https://peps.python.org/pep-0600/), Future ‘manylinux’ Platform Tags for Portable Linux Built Distributions\n- [PEP 621](https://peps.python.org/pep-0621/), Storing project metadata in pyproject.toml\n\n## Basic idea\n\n- Glue between PEP 517 `build_wheel` function and modern CMake standard project configuration / build / test / install\n- Install in `${PYTHON_SITELIB}/cmeel.prefix/`\n    - As there is a dot, it is not a valid python module name, so no risk of importing anything there by mistake\n    - `${PYTHON_SITELIB}/cmeel.pth` automatically load `${PYTHON_SITELIB}/cmeel.prefix/${PYTHON_SITELIB}`, so python\n      packages work out of the box\n    - Existing `${PYTHON_SITELIB}/cmeel.prefix` are automatically added to `$CMAKE_PREFIX_PATH`, so we can build CMake\n      packages whose dependencies are provided by other CMake packages installed with cmeel\n    - Stuff in `${PYTHON_SITELIB}/cmeel.prefix/bin` gets wrapped into entrypoints (TODO)\n',
     'author': 'Guilhem Saurel',
     'author_email': 'guilhem.saurel@laas.fr',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/cmake-wheel/cmeel',
     'packages': packages,
     'package_data': package_data,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cmeel-0.8.0/PKG-INFO` & `cmeel-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmeel
-Version: 0.8.0
+Version: 0.9.0
 Summary: Create Wheel from CMake projects
 Home-page: https://github.com/cmake-wheel/cmeel
 License: BSD-2-Clause
 Author: Guilhem Saurel
 Author-email: guilhem.saurel@laas.fr
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
@@ -21,19 +21,21 @@
 
 # CMake Wheels
 
 [![PyPI version](https://badge.fury.io/py/cmeel.svg)](https://pypi.org/project/cmeel)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/cmake-wheel/cmeel/main.svg)](https://results.pre-commit.ci/latest/github/cmake-wheel/cmeel/main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-Pip build backend using CMake.
+Wheel build backend using CMake, to package anything with pip and distribut on PyPI.
 
 Following those relevant PEPs:
+- [PEP 427](https://peps.python.org/pep-0427/), The Wheel Binary Package Format 1.0
 - [PEP 517](https://peps.python.org/pep-0517/), A build-system independent format for source trees
 - [PEP 518](https://peps.python.org/pep-0518/), Specifying Minimum Build System Requirements for Python Projects
+- [PEP 600](https://peps.python.org/pep-0600/), Future ‘manylinux’ Platform Tags for Portable Linux Built Distributions
 - [PEP 621](https://peps.python.org/pep-0621/), Storing project metadata in pyproject.toml
 
 ## Basic idea
 
 - Glue between PEP 517 `build_wheel` function and modern CMake standard project configuration / build / test / install
 - Install in `${PYTHON_SITELIB}/cmeel.prefix/`
     - As there is a dot, it is not a valid python module name, so no risk of importing anything there by mistake
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

