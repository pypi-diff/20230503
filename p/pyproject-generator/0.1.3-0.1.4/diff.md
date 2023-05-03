# Comparing `tmp/pyproject-generator-0.1.3.tar.gz` & `tmp/pyproject-generator-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-generator-0.1.3.tar", last modified: Sun Apr 30 15:01:14 2023, max compression
+gzip compressed data, was "pyproject-generator-0.1.4.tar", last modified: Wed May  3 20:45:51 2023, max compression
```

## Comparing `pyproject-generator-0.1.3.tar` & `pyproject-generator-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 15:01:14.351850 pyproject-generator-0.1.3/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     2082 2023-04-30 15:01:14.352158 pyproject-generator-0.1.3/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1563 2023-04-30 01:14:26.000000 pyproject-generator-0.1.3/README.md
--rw-r--r--   0 cangyuanli   (501) staff       (20)      232 2023-04-19 15:24:26.000000 pyproject-generator-0.1.3/pyproject.toml
--rw-r--r--   0 cangyuanli   (501) staff       (20)      868 2023-04-30 15:01:14.353438 pyproject-generator-0.1.3/setup.cfg
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 15:01:14.324777 pyproject-generator-0.1.3/src/
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 15:01:14.331470 pyproject-generator-0.1.3/src/pyproject/
--rw-r--r--   0 cangyuanli   (501) staff       (20)       37 2023-04-19 15:24:27.000000 pyproject-generator-0.1.3/src/pyproject/__init__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-04-30 15:00:59.000000 pyproject-generator-0.1.3/src/pyproject/__version__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     2835 2023-04-30 14:29:20.000000 pyproject-generator-0.1.3/src/pyproject/cli.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 15:01:14.333552 pyproject-generator-0.1.3/src/pyproject/config/
--rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:04.000000 pyproject-generator-0.1.3/src/pyproject/config/config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)      259 2023-04-30 01:22:22.000000 pyproject-generator-0.1.3/src/pyproject/config/default_config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)    11353 2023-04-30 14:59:52.000000 pyproject-generator-0.1.3/src/pyproject/project_builder.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 15:01:14.344993 pyproject-generator-0.1.3/src/pyproject/templates/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1477 2023-04-13 18:28:38.000000 pyproject-generator-0.1.3/src/pyproject/templates/gitignore.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      548 2023-04-30 01:20:52.000000 pyproject-generator-0.1.3/src/pyproject/templates/license_apache.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1074 2023-04-30 01:18:24.000000 pyproject-generator-0.1.3/src/pyproject/templates/license_mit.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      231 2023-04-12 23:53:39.000000 pyproject-generator-0.1.3/src/pyproject/templates/pyproject.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      398 2023-04-14 17:01:55.000000 pyproject-generator-0.1.3/src/pyproject/templates/readme.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      578 2023-04-14 17:03:04.000000 pyproject-generator-0.1.3/src/pyproject/templates/setup.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.1.3/src/pyproject/templates/tests.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.1.3/src/pyproject/templates/tox.template
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 15:01:14.350473 pyproject-generator-0.1.3/src/pyproject_generator.egg-info/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     2082 2023-04-30 15:01:14.000000 pyproject-generator-0.1.3/src/pyproject_generator.egg-info/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)      859 2023-04-30 15:01:14.000000 pyproject-generator-0.1.3/src/pyproject_generator.egg-info/SOURCES.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-04-30 15:01:14.000000 pyproject-generator-0.1.3/src/pyproject_generator.egg-info/dependency_links.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-04-30 15:01:14.000000 pyproject-generator-0.1.3/src/pyproject_generator.egg-info/entry_points.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       13 2023-04-30 15:01:14.000000 pyproject-generator-0.1.3/src/pyproject_generator.egg-info/requires.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-04-30 15:01:14.000000 pyproject-generator-0.1.3/src/pyproject_generator.egg-info/top_level.txt
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-30 15:01:14.351316 pyproject-generator-0.1.3/tests/
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-19 15:24:26.000000 pyproject-generator-0.1.3/tests/test_pyproject.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-03 20:45:51.787041 pyproject-generator-0.1.4/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     2082 2023-05-03 20:45:51.787178 pyproject-generator-0.1.4/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1563 2023-04-30 01:14:26.000000 pyproject-generator-0.1.4/README.md
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      232 2023-04-19 15:24:26.000000 pyproject-generator-0.1.4/pyproject.toml
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      868 2023-05-03 20:45:51.788104 pyproject-generator-0.1.4/setup.cfg
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-03 20:45:51.759606 pyproject-generator-0.1.4/src/
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-03 20:45:51.766649 pyproject-generator-0.1.4/src/pyproject/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       37 2023-05-03 20:45:40.000000 pyproject-generator-0.1.4/src/pyproject/__init__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-05-03 20:45:03.000000 pyproject-generator-0.1.4/src/pyproject/__version__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3494 2023-05-02 21:04:44.000000 pyproject-generator-0.1.4/src/pyproject/cli.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-03 20:45:51.769282 pyproject-generator-0.1.4/src/pyproject/config/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:04.000000 pyproject-generator-0.1.4/src/pyproject/config/config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      281 2023-05-03 20:05:37.000000 pyproject-generator-0.1.4/src/pyproject/config/default_config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1312 2023-05-03 20:35:21.000000 pyproject-generator-0.1.4/src/pyproject/logger.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    14894 2023-05-03 20:38:37.000000 pyproject-generator-0.1.4/src/pyproject/project_builder.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     2727 2023-05-03 18:55:58.000000 pyproject-generator-0.1.4/src/pyproject/spinner.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-03 20:45:51.781844 pyproject-generator-0.1.4/src/pyproject/templates/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1498 2023-05-03 19:23:49.000000 pyproject-generator-0.1.4/src/pyproject/templates/gitignore.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      548 2023-04-30 01:20:52.000000 pyproject-generator-0.1.4/src/pyproject/templates/license_apache.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-30 15:11:38.000000 pyproject-generator-0.1.4/src/pyproject/templates/license_gpl_v3.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1074 2023-04-30 01:18:24.000000 pyproject-generator-0.1.4/src/pyproject/templates/license_mit.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      231 2023-04-12 23:53:39.000000 pyproject-generator-0.1.4/src/pyproject/templates/pyproject.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      398 2023-04-14 17:01:55.000000 pyproject-generator-0.1.4/src/pyproject/templates/readme.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      583 2023-04-30 15:11:46.000000 pyproject-generator-0.1.4/src/pyproject/templates/setup.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.1.4/src/pyproject/templates/tests.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.1.4/src/pyproject/templates/tox.template
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-03 20:45:51.786280 pyproject-generator-0.1.4/src/pyproject_generator.egg-info/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     2082 2023-05-03 20:45:51.000000 pyproject-generator-0.1.4/src/pyproject_generator.egg-info/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      956 2023-05-03 20:45:51.000000 pyproject-generator-0.1.4/src/pyproject_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-05-03 20:45:51.000000 pyproject-generator-0.1.4/src/pyproject_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-05-03 20:45:51.000000 pyproject-generator-0.1.4/src/pyproject_generator.egg-info/entry_points.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       13 2023-05-03 20:45:51.000000 pyproject-generator-0.1.4/src/pyproject_generator.egg-info/requires.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-05-03 20:45:51.000000 pyproject-generator-0.1.4/src/pyproject_generator.egg-info/top_level.txt
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-03 20:45:51.786811 pyproject-generator-0.1.4/tests/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-19 15:24:26.000000 pyproject-generator-0.1.4/tests/test_pyproject.py
```

### Comparing `pyproject-generator-0.1.3/PKG-INFO` & `pyproject-generator-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.1.3
+Version: 0.1.4
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyproject-generator-0.1.3/README.md` & `pyproject-generator-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.3/setup.cfg` & `pyproject-generator-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.3/src/pyproject/cli.py` & `pyproject-generator-0.1.4/src/pyproject/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,35 @@
 import argparse
 import typing
+from typing import Optional
 
 from .project_builder import Action, ProjectBuilder
 from .__version__ import __version__
 
 ACTIONS = list(typing.get_args(Action))
 LICENSES = ("apache", "mit")
 
 
+def _parse_arg_to_set(string: Optional[str], sep: str = ",") -> set[str]:
+    """Expects a delimited string of arguments, e.g. `a,b,c,d`. Transforms string
+    into a set.
+
+    Args:
+        string (Optional[str]): `a,b,c,d`
+        sep (str): What to split on
+
+    Returns:
+        set[str]: string in set form
+    """
+    if string is None:
+        return set()
+
+    return set(word.strip() for word in string.split(sep))
+
+
 def get_parser():
     parser = argparse.ArgumentParser(description="Generate python project")
 
     parser.add_argument("action", type=str, choices=ACTIONS, help="Action")
     parser.add_argument(
         "project_name", type=str, nargs="?", default=None, help="Name of the project"
     )
@@ -45,14 +63,17 @@
         "--remove_dependencies",
         type=str,
         help="Remove dependencies to always download. Pass in a comma delimited string",
     )
     parser.add_argument(
         "--show", required=False, action="store_true", help="Show the current config"
     )
+    parser.add_argument(
+        "--quiet", required=False, action="store_true", help="Supress logging"
+    )
 
     parser.add_argument(
         "-v",
         "--version",
         action="version",
         version="%(prog)s {version}".format(version=__version__),
         help="Displays package version",
@@ -64,27 +85,29 @@
 def main():
     parser = get_parser()
     args = parser.parse_args()
 
     if args.action == "init" and args.project_name is None:
         parser.error("init requires project name")
 
-    config: dict[str, str] = {
+    options = {"quiet": args.quiet}
+
+    config = {
         "pypi_username": args.pypi_username,
         "pypi_password": args.pypi_password,
         "github_url": args.github_url,
         "author": args.author,
         "email": args.email,
         "license": args.license,
-        "set_dependencies": args.set_dependencies,
-        "add_dependencies": args.add_dependencies,
-        "remove_dependencies": args.remove_dependencies,
+        "set_dependencies": _parse_arg_to_set(args.set_dependencies),
+        "add_dependencies": _parse_arg_to_set(args.add_dependencies),
+        "remove_dependencies": _parse_arg_to_set(args.remove_dependencies),
         "reset_config": args.reset_config,
         "show": args.show,
     }
 
-    builder = ProjectBuilder(config=config)
+    builder = ProjectBuilder(config=config, options=options)
     builder.dispatch(action=args.action, project_name=args.project_name)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pyproject-generator-0.1.3/src/pyproject/project_builder.py` & `pyproject-generator-0.1.4/src/pyproject/project_builder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,119 @@
 # Imports
 
+from __future__ import annotations
+
+import dataclasses
 import datetime
 import os
 import json
 from pathlib import Path
-import pprint
 import re
 import shutil
 import subprocess
 import string
+import sys
 from types import SimpleNamespace
 from typing import Literal, Optional, Union
 import venv
 
 import platformdirs
+from rich.panel import Panel
 
-Action = Literal["init", "upload", "config"]
-PathLike = Union[Path, str]
+from .logger import CustomConsole, Level
+
+# Globals
 
 BASE_PATH = Path(__file__).resolve().parents[0]
 TEMPLATE_PATH = BASE_PATH / "templates"
 USER_CONFIG_PATH = platformdirs.user_config_dir(
     appname="pyproject-generator", appauthor="cangyuanli"
 )
 
+# Types
+
+Action = Literal["init", "upload", "config"]
+PathLike = Union[Path, str]
+
+
+@dataclasses.dataclass
+class License:
+    short_name: str
+    proper_name: Optional[str] = None
+
+    def __post_init__(self):
+        if self.proper_name is None:
+            name_mapper = {"mit": "MIT", "apache": "Apache", "gpl_v3": "GPL v3"}
+            self.proper_name = name_mapper[self.short_name]
+
+
+@dataclasses.dataclass
+class Config:
+    pypi_username: str
+    pypi_password: str
+    github_url: str
+    author: str
+    email: str
+    license: License
+    dependencies: set[str]
+
+    def __post_init__(self):
+        if isinstance(self.license, str):
+            self.license = License(self.license)
+        self.dependencies = set(self.dependencies)
+
+    def to_json_representable(self) -> dict:
+        _dict = self.to_dict()
+        _dict["license"] = self.license.short_name
+        _dict["dependencies"] = sorted(list(self.dependencies))
+
+        return _dict
+
+    def to_dict(self) -> dict:
+        return self.__dict__.copy()
+
+    @classmethod
+    def merge(cls, config1: Config, config2: Config):
+        c1 = config1.to_dict()
+        c2 = config2.to_dict()
+        merged_config = {}
+        for k, v in c1.items():
+            if c2[k] is None:
+                merged_config[k] = v
+            else:
+                merged_config[k] = c1[k]
+
+        return Config(**merged_config)
+
+    def __or__(self, config2: Config) -> Config:
+        dct = self.to_dict() | config2.to_dict()
+
+        return Config(**dct)
+
+
+@dataclasses.dataclass
+class CLIConfig(Config):
+    set_dependencies: set[str]
+    add_dependencies: set[str]
+    remove_dependencies: set[str]
+    reset_config: bool
+    show: bool
+
+    def __post_init__(self):
+        self.dependencies = (
+            self.dependencies | self.add_dependencies
+        ) - self.remove_dependencies
+
+        return super().__post_init__()
+
 
 class Env(venv.EnvBuilder):
     def __init__(self, *args, **kwargs) -> None:
         self.context = self.get_context()
+
         super().__init__(*args, **kwargs)
 
     def get_context(self) -> Optional[SimpleNamespace]:
         if "VIRTUAL_ENV" not in os.environ:
             self.context = None
             return None
 
@@ -66,22 +148,29 @@
 
         return subprocess.run(command, check=True, **kwargs)
 
 
 class ProjectBuilder:
     def __init__(
         self,
+        config: dict,
+        options: dict,
         template_path: PathLike = TEMPLATE_PATH,
         user_config_dir: PathLike = USER_CONFIG_PATH,
-        config: Optional[dict[str, str]] = None,
     ) -> None:
         self.proj_path = Path().cwd()
 
         self._template_path = Path(template_path)
 
+        # set up the console for logging
+        self._logging_level = Level.INFO
+        if options["quiet"]:
+            self._logging_level = Level.ERROR
+        self._console = CustomConsole(self._logging_level)
+
         self._user_config_dir = Path(user_config_dir)
         self._create_config_dir()
         self._config = self._set_config(config)
 
     @staticmethod
     def _validate_project_name(project_name: str) -> None:
         # https://packaging.python.org/en/latest/specifications/name-normalization/
@@ -94,19 +183,20 @@
 
     def _create_config_dir(self) -> None:
         """Create the user config directory if it does not exist. Since the default
         configuration may add keys, merge the two, preferring the
         existing config so we don't overwrite user changes.
         """
         self._user_config_dir.mkdir(exist_ok=True)
+        config_file = self._user_config_dir / "config.json"
 
-        if not (self._user_config_dir / "config.json").exists():
+        if not config_file.exists() or config_file.stat().st_size == 0:
             shutil.copy(
                 BASE_PATH / "config/default_config.json",
-                self._user_config_dir / "config.json",
+                config_file,
             )
 
         config = self._parse_config_file("config.json")
         default_config = self._parse_config_file("default_config.json")
 
         config = default_config | config
         self._write_config_file(config)
@@ -121,191 +211,240 @@
 
         Returns:
             dict[str, str]: {file_stem: filled_in_template}
         """
         config = self._config
         d = {
             "PACKAGE": project_name,
-            "PYPI_USERNAME": config["pypi_username"],
-            "PYPI_PASSWORD": config["pypi_password"],
-            "GITHUB_URL": config["github_url"],
-            "AUTHOR": config["author"],
-            "EMAIL": config["email"],
+            "PYPI_USERNAME": config.pypi_username,
+            "PYPI_PASSWORD": config.pypi_password,
+            "GITHUB_URL": config.github_url,
+            "AUTHOR": config.author,
+            "EMAIL": config.email,
             "YEAR": datetime.datetime.now().year,
+            "LICENSE": config.license.proper_name,
         }
 
         filled_in_templates = {}
         for file in self._template_path.glob("*.template"):
             with open(file, "r") as f:
                 src = string.Template(f.read())
                 result = src.substitute(d)
 
                 filled_in_templates[file.stem] = result
 
         return filled_in_templates
 
-    def init_project(self, project_name: str):
-        """Called when user specifies `action = init`.
-
-        Args:
-            project_name (str): User-supplied name of project
-        """
-        # Create the project directory
-        self._validate_project_name(project_name)
-
-        proj_path = self.proj_path / project_name
-        proj_path.mkdir()
-
-        # src
+    @staticmethod
+    def _init_source_directory(proj_path: Path, project_name: str):
         src_path = proj_path / "src"
         src_path.mkdir()
 
         src_proj_path = src_path / project_name
         src_proj_path.mkdir()
         (src_proj_path / "__init__.py").touch()
         (src_proj_path / "py.typed").touch()
 
-        # Fill in templates
-        templates = self._fill_in_templates(project_name)
-
-        # tests
+    @staticmethod
+    def _init_tests(proj_path: Path, project_name: str):
         tests_path = proj_path / "tests"
         tests_path.mkdir()
         (tests_path / f"test_{project_name}.py").touch()
 
-        # benchmarks
+    @staticmethod
+    def _init_benchmarks(proj_path: Path):
         benchmarks_path = proj_path / "benchmarks"
         benchmarks_path.mkdir()
         (benchmarks_path / "benchmark.py").touch()
 
-        # github actions
-        workflows_path = proj_path / ".github/workflows"
-        workflows_path.mkdir(parents=True)
-        (workflows_path / "tests.yml").write_text(templates["tests"])
-
-        # misc setup
+    def _init_config_files(self, proj_path: Path, templates: dict):
         (proj_path / "tox.ini").write_text(templates["tox"])
         (proj_path / "pyproject.toml").write_text(templates["pyproject"])
         (proj_path / "setup.cfg").write_text(templates["setup"])
         (proj_path / ".gitignore").write_text(templates["gitignore"])
         (proj_path / "README.md").write_text(templates["readme"])
 
-        license = self._config["license"]
+        license = self._config.license.short_name
         (proj_path / "LICENSE").write_text(templates[f"license_{license}"])
 
+    @staticmethod
+    def _init_github_actions(proj_path, templates: dict):
+        workflows_path = proj_path / ".github/workflows"
+        workflows_path.mkdir(parents=True)
+        (workflows_path / "tests.yml").write_text(templates["tests"])
+
+    def init_project(self, project_name: str):
+        """Called when user specifies `action = init`.
+
+        Args:
+            project_name (str): User-supplied name of project
+        """
+
+        # Create the project directory
+        try:
+            self._validate_project_name(project_name)
+        except ValueError as e:
+            self._console.error(str(e))
+            sys.exit(1)
+
+        proj_path = self.proj_path / project_name
+
+        try:
+            proj_path.mkdir()
+        except FileExistsError:
+            self._console.error(f"{proj_path} already exists")
+            sys.exit(1)
+
+        self._console.info(Panel("Creating project files..."), justify="left")
+
+        # Fill in templates
+        templates = self._console.spinner(
+            lambda: self._fill_in_templates(project_name),
+            "Filling in templates",
+            clear=True,
+            min_show_duration=0.2,
+        )
+
+        # src
+        self._console.spinner(
+            lambda: self._init_source_directory(proj_path, project_name),
+            "Creating source directory",
+            clear=True,
+            min_show_duration=0.2,
+        )
+
+        # tests
+        self._console.spinner(
+            lambda: self._init_tests(proj_path, project_name),
+            "Creating tests",
+            clear=True,
+            min_show_duration=0.2,
+        )
+
+        # benchmarks
+        self._console.spinner(
+            lambda: self._init_benchmarks(proj_path),
+            "Creating benchmarks",
+            clear=True,
+            min_show_duration=0.2,
+        )
+
+        # github actions
+        self._console.spinner(
+            lambda: self._init_github_actions(proj_path, templates),
+            "Setting up Github Actions",
+            clear=True,
+            min_show_duration=0.2,
+        )
+
+        # misc setup
+        self._console.spinner(
+            lambda: self._init_config_files(proj_path, templates),
+            "Setting up configuration files",
+            clear=True,
+            min_show_duration=0.2,
+        )
+
+        self._console.info("Building project skeleton completed with no errors.")
+
         # Setup the virtual environment
+        self._console.info(
+            Panel("Setting up the virtual environment..."), justify="left"
+        )
 
         venv_builder = Env(with_pip=True)
         venv_builder.venv_create(proj_path / "venv")
-        venv_builder.run_bin(["python", "-m", "pip", "install", "-U", "pip"])
 
         # Install developer dependencies
-        for dep in self._config["dependencies"]:
-            venv_builder.run_bin(["pip", "install", dep])
+
+        self._console.spinner(
+            lambda: venv_builder.run_bin(
+                ["python", "-m", "pip", "install", "-U", "pip"],
+                stdout=subprocess.DEVNULL,
+            ),
+            text="pip",
+        )
+
+        for dep in sorted(list(self._config.dependencies)):
+            self._console.spinner(
+                lambda: venv_builder.run_bin(
+                    ["pip", "install", dep], stdout=subprocess.DEVNULL
+                ),
+                text=dep,
+            )
 
         # Create requirements_dev file
         reqs = venv_builder.run_bin(["pip", "freeze"], capture_output=True)
         (proj_path / "requirements_dev.txt").write_bytes(reqs.stdout)
 
-    def _parse_config_file(self, filename: PathLike) -> dict:
+        self._console.info(f"Done setting up {project_name}!", style="green")
+
+    def _parse_config_file(self, filename: PathLike) -> Config:
         if filename == "default_config.json":
             path = BASE_PATH / "config/default_config.json"
         elif filename == "config.json":
             path = self._user_config_dir / filename
         else:
             raise ValueError("Name wrong.")
 
         with open(path) as f:
             config: dict = json.load(f)
 
-        return config
+        return Config(**config)
 
-    @staticmethod
-    def _parse_arg_to_set(string: Optional[str], sep: str) -> set[str]:
-        """Expects a delimited string of arguments, e.g. `a,b,c,d`. Transforms string
-        into a set.
-
-        Args:
-            string (Optional[str]): `a,b,c,d`
-            sep (str): What to split on
-
-        Returns:
-            set[str]: string in set form
-        """
-        if string is None:
-            return set()
-
-        return set(word.strip() for word in string.split(sep))
-
-    def _set_config(self, config: dict[str, str]) -> dict:
+    def _set_config(self, config: dict) -> Config:
         """Take in the arguments provided by the user and merge them with their
         saved configuration file.
 
         Args:
-            config (dict[str, str]): Expects either the saved user configuration or the
-            default configuration (if --reset flag is set).
+            config (dict[str, str]): Expects either the saved user
+            configuration or the default configuration (if --reset flag is set).
 
         Returns:
             dict: A configuration dict of {config_arg: config}
         """
         if config["reset_config"]:
             saved_path = "default_config.json"
         else:
             saved_path = "config.json"
 
         saved_config = self._parse_config_file(saved_path)
 
         # --set_dependencies overrides the saved dependencies. So simply use saved
         # if flag is not set, otherwise parse the list of provided dependencies.
         if config["set_dependencies"] is None:
-            config["dependencies"] = set(saved_config["dependencies"])
+            config["dependencies"] = saved_config.dependencies
         else:
-            config["dependencies"] = self._parse_arg_to_set(
-                config["set_dependencies"], sep=","
-            )
+            config["dependencies"] = config["set_dependencies"]
 
-        # --remove_dependencies and --add_dependencies don't overwrite. Parse them to a
-        # set so we can use union and difference operators.
-        for k in ("remove_dependencies", "add_dependencies"):
-            config[k] = self._parse_arg_to_set(config[k], sep=",")
-
-        config["dependencies"] = (
-            config["dependencies"] | config["add_dependencies"]
-        ) - config["remove_dependencies"]
+        _config = CLIConfig(**config)
 
-        merged_config = {}
-        for k, v in saved_config.items():
-            if config[k] is None:
-                merged_config[k] = v
-            else:
-                merged_config[k] = config[k]
+        merged_config = Config.merge(saved_config, _config)
 
-        if config["show"]:
-            pprint.pprint(merged_config)
+        if _config.show:
+            self._console.pprint(merged_config.to_json_representable())
 
         return merged_config
 
-    def _write_config_file(self, config: dict):
-        # set objects aren't serializable to json, so convert it to a list
-        config["dependencies"] = sorted(list(config["dependencies"]))
+    def _write_config_file(self, config: Config):
         with open(self._user_config_dir / "config.json", "w") as f:
-            json.dump(config, f, indent=4)
+            json.dump(config.to_json_representable(), f, indent=4)
 
     def config(self):
         """If the action is `config`, save the built configuration as the default. This
         method is intentionally sparse, as the bulk of the work should be done by
         creating the config on the fly--we want the user to be able to pass config flags
         in without going through the config action.
         """
         self._write_config_file(self._config)
 
     def upload(self):
         """Discover the virtual environment and upload project to PyPI."""
-        username = self._config["pypi_username"]
-        password = self._config["pypi_password"]
+        username = self._config.pypi_username
+        password = self._config.pypi_password
 
         env = Env()
 
         # python -m build generates a dist folder, remove this in preparation
         shutil.rmtree(self.proj_path / "dist", ignore_errors=True)
 
         env.run_bin(["python", "-m", "build"])
```

### Comparing `pyproject-generator-0.1.3/src/pyproject/templates/gitignore.template` & `pyproject-generator-0.1.4/src/pyproject/templates/gitignore.template`

 * *Files 5% similar despite different names*

```diff
@@ -111,14 +111,17 @@
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
+# Ruff
+.ruff_cache/
+
 # pytype static type analyzer
 .pytype/
 
 # Cython debug symbols
 cython_debug/
 
 **/venv
```

### Comparing `pyproject-generator-0.1.3/src/pyproject/templates/license_apache.template` & `pyproject-generator-0.1.4/src/pyproject/templates/license_apache.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.3/src/pyproject/templates/license_mit.template` & `pyproject-generator-0.1.4/src/pyproject/templates/license_mit.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.3/src/pyproject/templates/setup.template` & `pyproject-generator-0.1.4/src/pyproject/templates/setup.template`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = $GITHUB_URL/$PACKAGE
 project_urls =
     Bug Tracker = $GITHUB_URL/$PACKAGE/issues
 classifiers =
     Programming Language :: Python :: 3
-    License :: OSI Approved :: MIT License
+    License :: OSI Approved :: $LICENSE License
     Operating System :: OS Independent
 
 [options]
 package_dir =
     = src
 packages = find:
 python_requires = >=3.6
```

### Comparing `pyproject-generator-0.1.3/src/pyproject/templates/tests.template` & `pyproject-generator-0.1.4/src/pyproject/templates/tests.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.3/src/pyproject_generator.egg-info/PKG-INFO` & `pyproject-generator-0.1.4/src/pyproject_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.1.3
+Version: 0.1.4
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyproject-generator-0.1.3/src/pyproject_generator.egg-info/SOURCES.txt` & `pyproject-generator-0.1.4/src/pyproject_generator.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 README.md
 pyproject.toml
 setup.cfg
 src/pyproject/__init__.py
 src/pyproject/__version__.py
 src/pyproject/cli.py
+src/pyproject/logger.py
 src/pyproject/project_builder.py
+src/pyproject/spinner.py
 src/pyproject/config/config.json
 src/pyproject/config/default_config.json
 src/pyproject/templates/gitignore.template
 src/pyproject/templates/license_apache.template
+src/pyproject/templates/license_gpl_v3.template
 src/pyproject/templates/license_mit.template
 src/pyproject/templates/pyproject.template
 src/pyproject/templates/readme.template
 src/pyproject/templates/setup.template
 src/pyproject/templates/tests.template
 src/pyproject/templates/tox.template
 src/pyproject_generator.egg-info/PKG-INFO
```

