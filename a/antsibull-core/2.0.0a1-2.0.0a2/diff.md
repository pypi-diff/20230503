# Comparing `tmp/antsibull_core-2.0.0a1.tar.gz` & `tmp/antsibull_core-2.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antsibull_core-2.0.0a1.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `antsibull_core-2.0.0a1.tar` & `antsibull_core-2.0.0a2.tar`

### file list

```diff
@@ -1,41 +1,66 @@
--rw-r--r--   0        0        0    35149 2022-04-05 05:38:49.478039 antsibull_core-2.0.0a1/LICENSE
-drwxr-xr-x   0        0        0        0 2022-07-31 17:40:16.789172 antsibull_core-2.0.0a1/LICENSES/
--rw-r--r--   0        0        0     4222 2022-12-09 07:22:40.650976 antsibull_core-2.0.0a1/README.md
--rw-r--r--   0        0        0     1669 2022-12-09 07:22:40.650976 antsibull_core-2.0.0a1/pyproject.toml
--rw-r--r--   0        0        0      209 2022-07-31 17:40:16.795838 antsibull_core-2.0.0a1/src/antsibull_core/__init__.py
--rw-r--r--   0        0        0    13763 2022-12-09 07:22:45.831010 antsibull_core-2.0.0a1/src/antsibull_core/ansible_core.py
--rw-r--r--   0        0        0    16177 2022-12-09 07:22:45.831010 antsibull_core-2.0.0a1/src/antsibull_core/app_context.py
--rw-r--r--   0        0        0     2363 2022-12-09 07:22:45.831010 antsibull_core-2.0.0a1/src/antsibull_core/args.py
--rw-r--r--   0        0        0     3608 2022-12-09 07:22:45.831010 antsibull_core-2.0.0a1/src/antsibull_core/collections.py
--rw-r--r--   0        0        0     1636 2022-12-09 07:22:34.624270 antsibull_core-2.0.0a1/src/antsibull_core/compat.py
--rw-r--r--   0        0        0     5588 2022-12-09 07:22:45.831010 antsibull_core-2.0.0a1/src/antsibull_core/config.py
--rw-r--r--   0        0        0     8418 2022-12-09 07:22:45.831010 antsibull_core-2.0.0a1/src/antsibull_core/dependency_files.py
--rw-r--r--   0        0        0     3000 2022-12-09 07:22:45.831010 antsibull_core-2.0.0a1/src/antsibull_core/filesystem.py
--rw-r--r--   0        0        0    12717 2022-12-09 07:22:45.831010 antsibull_core-2.0.0a1/src/antsibull_core/galaxy.py
--rw-r--r--   0        0        0    11768 2022-12-09 07:22:45.834344 antsibull_core-2.0.0a1/src/antsibull_core/logging.py
--rw-r--r--   0        0        0        0 2022-08-19 06:53:18.336141 antsibull_core-2.0.0a1/src/antsibull_core/py.typed
--rw-r--r--   0        0        0      203 2022-07-31 17:40:16.802505 antsibull_core-2.0.0a1/src/antsibull_core/schemas/__init__.py
--rw-r--r--   0        0        0     5149 2022-12-09 07:22:45.834344 antsibull_core-2.0.0a1/src/antsibull_core/schemas/config.py
--rw-r--r--   0        0        0     5314 2022-12-07 20:54:39.541494 antsibull_core-2.0.0a1/src/antsibull_core/schemas/context.py
--rw-r--r--   0        0        0     1964 2022-12-09 07:22:45.834344 antsibull_core-2.0.0a1/src/antsibull_core/schemas/validators.py
--rw-r--r--   0        0        0     1686 2022-12-09 07:22:45.834344 antsibull_core-2.0.0a1/src/antsibull_core/tarball.py
--rw-r--r--   0        0        0      203 2022-07-31 17:40:16.805838 antsibull_core-2.0.0a1/src/antsibull_core/utils/__init__.py
--rw-r--r--   0        0        0     5005 2022-12-09 07:22:45.834344 antsibull_core-2.0.0a1/src/antsibull_core/utils/collections.py
--rw-r--r--   0        0        0     1143 2022-12-09 07:22:45.834344 antsibull_core-2.0.0a1/src/antsibull_core/utils/hashing.py
--rw-r--r--   0        0        0     4000 2022-12-09 07:22:45.834344 antsibull_core-2.0.0a1/src/antsibull_core/utils/http.py
--rw-r--r--   0        0        0     3863 2022-12-09 07:22:34.630936 antsibull_core-2.0.0a1/src/antsibull_core/utils/io.py
--rw-r--r--   0        0        0      203 2022-07-31 17:40:16.805838 antsibull_core-2.0.0a1/src/antsibull_core/vendored/__init__.py
--rw-r--r--   0        0        0     3030 2022-12-06 19:46:24.409458 antsibull_core-2.0.0a1/src/antsibull_core/vendored/_argparse_booleanoptionalaction.py
--rw-r--r--   0        0        0     3645 2022-12-07 06:54:22.799523 antsibull_core-2.0.0a1/src/antsibull_core/vendored/collections.py
--rw-r--r--   0        0        0     1957 2022-12-07 20:37:52.389765 antsibull_core-2.0.0a1/src/antsibull_core/vendored/json_utils.py
--rw-r--r--   0        0        0     3471 2022-12-09 07:22:45.834344 antsibull_core-2.0.0a1/src/antsibull_core/venv.py
--rw-r--r--   0        0        0     1606 2022-12-09 20:07:32.500540 antsibull_core-2.0.0a1/src/antsibull_core/yaml.py
--rw-r--r--   0        0        0     3965 2022-12-06 19:46:24.409458 antsibull_core-2.0.0a1/tests/functional/aiohttp_utils.py
--rw-r--r--   0        0        0     3928 2022-12-06 19:46:24.409458 antsibull_core-2.0.0a1/tests/functional/certificate_utils.py
--rw-r--r--   0        0        0     1464 2022-12-06 19:46:24.412792 antsibull_core-2.0.0a1/tests/functional/test_dependency_files.py
--rw-r--r--   0        0        0     1368 2022-12-06 19:46:24.412792 antsibull_core-2.0.0a1/tests/functional/test_logging.py
--rw-r--r--   0        0        0     1264 2022-12-06 19:46:24.412792 antsibull_core-2.0.0a1/tests/units/test_ansible_core.py
--rw-r--r--   0        0        0     8003 2022-07-31 17:40:16.812505 antsibull_core-2.0.0a1/tests/units/test_context.py
--rw-r--r--   0        0        0     4404 2022-07-31 17:40:16.812505 antsibull_core-2.0.0a1/tests/units/test_parse_pieces.py
--rw-r--r--   0        0        0     5278 1970-01-01 00:00:00.000000 antsibull_core-2.0.0a1/setup.py
--rw-r--r--   0        0        0     5466 1970-01-01 00:00:00.000000 antsibull_core-2.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/.flake8
+-rw-r--r--   0        0        0    15698 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/.pylintrc.automated
+-rw-r--r--   0        0        0     7111 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/CHANGELOG.rst
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/CHANGELOG.rst.license
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/LICENSE
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/antsibull.cfg
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/codecov.yml
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/noxfile.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/.github/dependabot.yml
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/.github/patchback.yml
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/.github/workflows/antsibull-docs.yml
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/.github/workflows/antsibull.yml
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/.github/workflows/nox.yml
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/.reuse/dep5
+-rw-r--r--   0        0        0     8224 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/changelogs/changelog.yaml
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/changelogs/changelog.yaml.license
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/changelogs/config.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/changelogs/fragments/.keep
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/__init__.py
+-rw-r--r--   0        0        0    13001 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/ansible_core.py
+-rw-r--r--   0        0        0    16176 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/app_context.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/args.py
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/collections.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/compat.py
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/config.py
+-rw-r--r--   0        0        0     8418 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/dependency_files.py
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/filesystem.py
+-rw-r--r--   0        0        0    18233 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/galaxy.py
+-rw-r--r--   0        0        0    11768 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/py.typed
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/subprocess_util.py
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/tarball.py
+-rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/venv.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/yaml.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/schemas/__init__.py
+-rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/schemas/config.py
+-rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/schemas/context.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/schemas/validators.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/utils/__init__.py
+-rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/utils/collections.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/utils/hashing.py
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/utils/http.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/utils/io.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/vendored/__init__.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/vendored/_argparse_booleanoptionalaction.py
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/vendored/collections.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/src/antsibull_core/vendored/json_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/stubs/.keep
+-rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/tests/functional/aiohttp_utils.py
+-rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/tests/functional/certificate_utils.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/tests/functional/test_dependency_files.py
+-rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/tests/functional/test_galaxy.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/tests/functional/test_logging.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/tests/functional/test_venv.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/tests/units/test_ansible_core.py
+-rw-r--r--   0        0        0     8003 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/tests/units/test_context.py
+-rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/tests/units/test_parse_pieces.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/tests/units/test_subprocess_util.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/.gitignore
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/README.md
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/LICENSES/BSD-2-Clause.txt
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/LICENSES/GPL-3.0-or-later.txt -> ../LICENSE
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/LICENSES/PSF-2.0.txt
+-rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 antsibull_core-2.0.0a2/PKG-INFO
```

### Comparing `antsibull_core-2.0.0a1/LICENSE` & `antsibull_core-2.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `antsibull_core-2.0.0a1/src/antsibull_core/ansible_core.py` & `antsibull_core-2.0.0a2/src/antsibull_core/ansible_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,26 @@
 
 import ast
 import asyncio
 import os
 import re
 import tempfile
 import typing as t
-from functools import lru_cache, partial
 from urllib.parse import urljoin
 
 import aiofiles
-import sh
 from packaging.version import Version as PypiVer
 
 from . import app_context
 from .logging import log
+from .subprocess_util import async_log_run
 from .utils.http import retry_get
 
 if t.TYPE_CHECKING:
-    import aiohttp.client  # pylint:disable=unused-import
+    import aiohttp.client
 
 
 mlog = log.fields(mod=__name__)
 
 #: URL to checkout ansible-core from.
 _ANSIBLE_CORE_URL = str(app_context.AppContext().ansible_base_url)
 #: URL to pypi.
@@ -63,15 +62,14 @@
         """
         JSON data from a url with retries and return the data as python data structures.
         """
         async with retry_get(self.aio_session, query_url) as response:
             pkg_info = await response.json()
         return pkg_info
 
-    @lru_cache(None)
     async def get_release_info(self) -> dict[str, t.Any]:
         """
         Retrieve information about releases of the ansible-core/ansible-base package from pypi.
 
         :returns: The dict which represents the release info keyed by version number.
             To examine the data structure, use::
 
@@ -239,60 +237,46 @@
             and source_version.minor == ansible_core_version.minor
             and source_version.micro >= ansible_core_version.micro):
         return True
 
     return False
 
 
-@lru_cache(None)
 async def checkout_from_git(download_dir: str, repo_url: str = _ANSIBLE_CORE_URL) -> str:
     """
     Checkout the ansible-core git repo.
 
     :arg download_dir: Directory to checkout into.
     :kwarg: repo_url: The url to the git repo.
     :return: The directory that ansible-core has been checked out to.
     """
-    loop = asyncio.get_running_loop()
     ansible_core_dir = os.path.join(download_dir, 'ansible-core')
-    await loop.run_in_executor(None, sh.git, 'clone', repo_url, ansible_core_dir)
+    await async_log_run(['git', 'clone', repo_url, ansible_core_dir])
 
     return ansible_core_dir
 
 
-@lru_cache(None)
 async def create_sdist(source_dir: str, dest_dir: str) -> str:
     """
     Create an sdist for the python package at a given path.
 
-    Note that this is not able to create an sdist for any python package.  It has to have a setup.py
-    sdist command.
-
     :arg source_dir: the directory that the python package source is in.
     :arg dest_dir: the directory that the sdist will be written to/
     :returns: path to the sdist.
     """
-    loop = asyncio.get_running_loop()
-
-    # Make sure setup.py exists
-    setup_script = os.path.join(source_dir, 'setup.py')
-    if not os.path.exists(setup_script):
-        raise CannotBuild(f'{source_dir} does not include a setup.py script.  This script cannot'
-                          ' build the package')
 
     # Make a subdir of dest_dir for returning the dist in
     dist_dir_prefix = os.path.join(os.path.basename(source_dir))
     dist_dir = tempfile.mkdtemp(prefix=dist_dir_prefix, dir=dest_dir)
 
-    # execute python setup.py sdist --dist-dir dest_dir/
-    # sh maps attributes to commands dynamically so ignore the linting errors there
-    # pyre-ignore[16]
-    python_cmd = partial(sh.python, _cwd=source_dir)  # pylint:disable=no-member
     try:
-        await loop.run_in_executor(None, python_cmd, setup_script, 'sdist', '--dist-dir', dist_dir)
+        await async_log_run(
+            ['python', '-m', 'build', '--sdist', '--outdir', dist_dir, source_dir],
+            stderr_loglevel='warning',
+        )
     except Exception as e:
         raise CannotBuild(f'Building {source_dir} failed: {e}')  # pylint:disable=raise-missing-from
 
     dist_files = [f for f in os.listdir(dist_dir) if f.endswith('tar.gz')]
     if len(dist_files) != 1:
         if not dist_files:
             raise CannotBuild(f'Building {source_dir} did not create a tar.gz')
```

### Comparing `antsibull_core-2.0.0a1/src/antsibull_core/app_context.py` & `antsibull_core-2.0.0a2/src/antsibull_core/app_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,21 +102,20 @@
 """
 
 from __future__ import annotations
 
 import argparse
 import contextvars
 import typing as t
-from contextlib import contextmanager
 from collections.abc import Iterable, Mapping
+from contextlib import contextmanager
 
 from .schemas.context import AppContext, LibContext
 from .vendored.collections import ImmutableDict
 
-
 AppContextT = t.TypeVar('AppContextT', bound=AppContext)
 
 
 #: lib_ctx should be restricted to things which do not belong in the API but an application or
 #: user might want to tweak.  Global, internal, incidental values are good to store here.  Things
 #: that are already settable by the public API are not.  For instance, a function whose primary
 #: purpose is to retrieve a file from the internet and return the filename where it was
```

### Comparing `antsibull_core-2.0.0a1/src/antsibull_core/args.py` & `antsibull_core-2.0.0a2/src/antsibull_core/args.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 # SPDX-FileCopyrightText: 2020, Ansible Project
 """Argument parsing helpers."""
 
 from __future__ import annotations
 
 import argparse
 import os.path
-
 from importlib import metadata
 
 
 class InvalidArgumentError(Exception):
     """A problem parsing or validating a command line argument."""
```

### Comparing `antsibull_core-2.0.0a1/src/antsibull_core/compat.py` & `antsibull_core-2.0.0a2/src/antsibull_core/compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,16 @@
 """
 
 from __future__ import annotations
 
 import argparse
 import asyncio
 import sys
-
 from importlib import metadata
 
-
 BooleanOptionalAction: type[argparse.BooleanOptionalAction]
 
 if sys.version_info < (3, 9, 11) or (
     sys.version_info >= (3, 10, 0) and sys.version_info < (3, 10, 3)
 ):
     # https://bugs.python.org/issue46080 was fixed in Python 3.11.0 alpha 5
     # (https://docs.python.org/3/whatsnew/changelog.html#python-3-11-0-alpha-5)
```

### Comparing `antsibull_core-2.0.0a1/src/antsibull_core/config.py` & `antsibull_core-2.0.0a2/src/antsibull_core/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import perky  # type: ignore[import]
 import pydantic as p
 
 from .logging import log
 from .schemas.config import ConfigModel
 from .schemas.context import AppContext, LibContext
 
-
 mlog = log.fields(mod=__name__)
 
 #: System config file location.
 SYSTEM_CONFIG_FILE = '/etc/antsibull.cfg'
 
 #: Per-user config file location.
 USER_CONFIG_FILE = '~/.antsibull.cfg'
```

### Comparing `antsibull_core-2.0.0a1/src/antsibull_core/dependency_files.py` & `antsibull_core-2.0.0a2/src/antsibull_core/dependency_files.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-2.0.0a1/src/antsibull_core/filesystem.py` & `antsibull_core-2.0.0a2/src/antsibull_core/filesystem.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # https://www.gnu.org/licenses/gpl-3.0.txt)
 # SPDX-License-Identifier: GPL-3.0-or-later
 # SPDX-FileCopyrightText: 2020, Ansible Project
 """Entrypoint to the antsibull-docs script."""
 
 from __future__ import annotations
 
-import sh
+from antsibull_core.subprocess_util import log_run
 
 try:
     # We fallback to /usr/bin/getfacl so we can ignore failure to import this
     import posix1e  # type: ignore[import] # pyre-ignore[21]
 except ImportError:
     posix1e = None
 
@@ -28,18 +28,16 @@
     """Return the acls for a given file or raise an exception."""
     acls = None
     if posix1e:
         acl = posix1e.ACL(file=path)
         acls = acl.to_any_text(options=posix1e.TEXT_NUMERIC_IDS).decode('utf-8')
     else:
         try:
-            # sh dynamically creates functions which map to executables
-            # pyre-ignore[16]
-            acls = sh.getfacl(path, '-n').stdout.decode('utf-8')  # pylint:disable=no-member
-        except sh.CommandNotFound:
+            acls = log_run(['getfacl', path, '-n']).stdout
+        except FileNotFoundError:
             pass
         except Exception as e:
             # pylint:disable-next=raise-missing-from
             raise CheckFailure(f'Error while trying to get acls for {path}: {e}')
 
     if not acls:
         raise UnableToCheck(f'No way to determine acls for {path}')
```

### Comparing `antsibull_core-2.0.0a1/src/antsibull_core/galaxy.py` & `antsibull_core-2.0.0a2/src/antsibull_core/galaxy.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,29 +3,32 @@
 # https://www.gnu.org/licenses/gpl-3.0.txt)
 # SPDX-License-Identifier: GPL-3.0-or-later
 # SPDX-FileCopyrightText: 2020, Ansible Project
 """Functions to work with Galaxy."""
 
 from __future__ import annotations
 
+import asyncio
+import dataclasses
 import os.path
 import shutil
 import typing as t
+from enum import Enum
 from urllib.parse import urljoin
 
 import aiofiles
 import semantic_version as semver
 
 from . import app_context
 from .utils.hashing import verify_hash
 from .utils.http import retry_get
 
 # The type checker can handle finding aiohttp.client but flake8 cannot :-(
 if t.TYPE_CHECKING:
-    import aiohttp.client  # pylint:disable=unused-import
+    import aiohttp.client
 
 
 #: URL to galaxy. (Get the default from the context default)
 _GALAXY_SERVER_URL = str(app_context.AppContext().galaxy_url)
 
 
 class NoSuchCollection(Exception):
@@ -45,89 +48,213 @@
 
     #: :obj:`semantic_version.Version` of the exact version of the collection that was downloaded.
     version: semver.Version
     #: Location on the filesystem of the downloaded collection.
     download_path: str
 
 
+class GalaxyVersion(Enum):
+    V2 = 2
+    V3 = 3
+
+
+@dataclasses.dataclass
+class GalaxyContext:
+    server: str
+    version: GalaxyVersion
+    base_url: str
+
+    @classmethod
+    async def create(cls, aio_session: aiohttp.client.ClientSession, galaxy_server: str
+                     ) -> GalaxyContext:
+        api_url = urljoin(galaxy_server, 'api/')
+        async with retry_get(aio_session, api_url,
+                             headers={'Accept': 'application/json'}) as response:
+            galaxy_info = await response.json()
+        available_versions: t.Mapping[str, str] = galaxy_info.get('available_versions') or {}
+        if 'v3' in available_versions:
+            version = GalaxyVersion.V3
+            base_url = urljoin(galaxy_server, 'api/' + available_versions['v3'])
+        elif 'v2' in available_versions:
+            version = GalaxyVersion.V2
+            base_url = urljoin(galaxy_server, 'api/' + available_versions['v2'])
+        else:
+            raise RuntimeError(
+                f'Information retrieved from {api_url} seems to indicate'
+                ' neither Galaxy v2 API nor Galaxy v3 API'
+            )
+        return cls(galaxy_server, version, base_url)
+
+
+_GALAXY_CONTEXT_CACHE: dict[str, t.Union[GalaxyContext, asyncio.Future]] = {}
+
+
+async def _get_cached_galaxy_context(aio_session: aiohttp.client.ClientSession,
+                                     galaxy_server: str) -> GalaxyContext:
+    context_or_future = _GALAXY_CONTEXT_CACHE.get(galaxy_server)
+    if context_or_future is not None:
+        if asyncio.isfuture(context_or_future):
+            return await context_or_future
+        return t.cast(GalaxyContext, context_or_future)
+
+    loop = asyncio.get_running_loop()
+    future = loop.create_future()
+
+    async def _init():
+        try:
+            context = await GalaxyContext.create(aio_session, galaxy_server)
+            future.set_result(context)
+            _GALAXY_CONTEXT_CACHE[galaxy_server] = context
+        except Exception as exc:  # pylint: disable=broad-exception-caught
+            future.set_exception(exc)
+
+    loop.create_task(_init())
+    _GALAXY_CONTEXT_CACHE[galaxy_server] = future
+    return await future
+
+
 class GalaxyClient:
     """Class for querying the Galaxy REST API."""
 
     def __init__(self, aio_session: aiohttp.client.ClientSession,
-                 galaxy_server: str = _GALAXY_SERVER_URL) -> None:
+                 galaxy_server: t.Optional[str] = None,
+                 context: t.Optional[GalaxyContext] = None) -> None:
         """
         Create a GalaxyClient object to query the Galaxy Server.
 
         :arg aio_session: :obj:`aiohttp.ClientSession` with which to perform all
             requests to galaxy.
-        :kwarg galaxy_server: URL to the galaxy server.
-        """
+        :kwarg galaxy_server: URL to the galaxy server. ``context`` must be provided instead
+            in the future.
+        :kwarg context: A ``GalaxyContext`` instance. Must be provided in the future.
+        """
+        if galaxy_server is None and context is None:
+            # TODO: deprecate
+            galaxy_server = _GALAXY_SERVER_URL
+        elif context is not None:
+            # TODO: deprecate
+            if galaxy_server is not None and galaxy_server != context.server:
+                raise ValueError(
+                    f'galaxy_server ({galaxy_server}) does not coincide'
+                    f' with context.server ({context.server})'
+                )
+            galaxy_server = context.server
         self.galaxy_server = galaxy_server
+        self.context = context
         self.aio_session = aio_session
-        self.params = {'format': 'json'}
+        self.headers: dict[str, str] = {'Accept': 'application/json'}
+        self.params: dict[str, str] = {}
+        if context:
+            self._update_from_context(context)
+
+    def _update_from_context(self, context: GalaxyContext) -> None:
+        if context.version == GalaxyVersion.V2:
+            self.params['format'] = 'json'
+
+    async def _ensure_context(self) -> GalaxyContext:
+        """
+        Ensure that ``self.context`` is present.
+        """
+        context = self.context
+        if context is not None:
+            return context
+        if self.galaxy_server is None:
+            raise RuntimeError('Unexpected None for GalaxyClient.galaxy_server')
+        context = await _get_cached_galaxy_context(self.aio_session, self.galaxy_server)
+        self.context = context
+        self._update_from_context(context)
+        return context
 
-    async def _get_galaxy_versions(self, versions_url: str) -> list[str]:
+    async def _get_galaxy_versions(self, context: GalaxyContext, versions_url: str,
+                                   add_params: bool = True) -> list[str]:
         """
         Retrieve the complete list of versions for a collection from a galaxy endpoint.
 
         This internal function retrieves versions for collections from a Galaxy endpoint.  If the
         information is paged, it continues to retrieve linked pages until all of the information has
         been returned.
 
+        :arg context: the ``GalaxyContext`` to use.
         :arg version_url: url to the page to retrieve.
+        :arg add_params: used internally during recursion. Do not specify when calling this.
         :returns: List of the all the versions of the collection.
         """
-        params = self.params.copy()
-        params['page_size'] = '100'
+        if add_params:
+            params = self.params.copy()
+            if context.version == GalaxyVersion.V2:
+                params['page_size'] = '100'
+            else:
+                params['limit'] = '50'
+        else:
+            params = None
         async with retry_get(self.aio_session, versions_url, params=params,
-                             acceptable_error_codes=[404]) as response:
+                             headers=self.headers, acceptable_error_codes=[404]) as response:
             if response.status == 404:
                 raise NoSuchCollection(f'No collection found at: {versions_url}')
             collection_info = await response.json()
 
         versions = []
-        for version_record in collection_info['results']:
+        if context.version == GalaxyVersion.V2:
+            results = collection_info['results']
+            next_link = collection_info['next']
+        else:
+            if 'data' in collection_info:
+                # Apparently 'data' isn't always used...
+                results = collection_info['data']
+            else:
+                results = collection_info['results']
+            next_link = collection_info['links']['next']
+            add_params = False
+        for version_record in results:
             versions.append(version_record['version'])
-
-        if collection_info['next']:
-            versions.extend(await self._get_galaxy_versions(collection_info['next']))
+        if next_link:
+            if next_link.startswith('/'):
+                next_link = urljoin(context.server, next_link)
+            versions.extend(await self._get_galaxy_versions(context, next_link, add_params))
 
         return versions
 
     async def get_versions(self, collection: str) -> list[str]:
         """
         Retrieve all versions of a collection on Galaxy.
 
         :arg collection: Name of the collection to get version info for.
         :returns: List of all the versions of this collection on galaxy.
         """
+        context = await self._ensure_context()
+
         collection = collection.replace('.', '/')
-        galaxy_url = urljoin(self.galaxy_server, f'api/v2/collections/{collection}/versions/')
-        retval = await self._get_galaxy_versions(galaxy_url)
+        galaxy_url = urljoin(context.base_url, f'collections/{collection}/versions/')
+        retval = await self._get_galaxy_versions(context, galaxy_url)
         return retval
 
     async def get_info(self, collection: str) -> dict[str, t.Any]:
         """
         Retrieve information about the collection on Galaxy.
 
         :arg collection: Namespace.collection to retrieve information about.
         :returns: Dictionary of information about the collection.
 
-        Please see the Galaxy REST API documentation for information on the structure of the
-        returned data.
+        Please see the Galaxy v2 and v3 REST API documentation for information on the
+        structure of the returned data.
 
         .. seealso::
             An example return value from the
-            `Galaxy REST API <https://galaxy.ansible.com/api/v2/collections/community/general/>`_
+            `Galaxy v2 REST API
+            <https://galaxy.ansible.com/api/v2/collections/community/general/>`_
+            and the `Galaxy v3 REST API
+            <https://beta-galaxy.ansible.com/api/v3/plugin/ansible/content/published/collections/index/community/general/>`_
         """
+        context = await self._ensure_context()
+
         collection = collection.replace('.', '/')
-        galaxy_url = urljoin(self.galaxy_server, f'api/v2/collections/{collection}/')
+        galaxy_url = urljoin(context.base_url, f'collections/{collection}/')
 
         async with retry_get(self.aio_session, galaxy_url, params=self.params,
-                             acceptable_error_codes=[404]) as response:
+                             headers=self.headers, acceptable_error_codes=[404]) as response:
             if response.status == 404:
                 raise NoSuchCollection(f'No collection found at: {galaxy_url}')
             collection_info = await response.json()
 
         return collection_info
 
     async def get_release_info(self, collection: str,
@@ -135,28 +262,31 @@
         """
         Retrive information about a specific version of a collection.
 
         :arg collection: Namespace.collection string naming the collection.
         :arg version: Version of the collection.
         :returns: Dictionary of information about the release.
 
-        Please see the Galaxy REST API documentation for information on the structure of the
-        returned data.
+        Please see the Galaxy v2 and v3 REST API documentation for information on the
+        structure of the returned data.
 
         .. seealso::
             An example return value from the
-            `Galaxy REST API
+            `Galaxy v2 REST API
             <https://galaxy.ansible.com/api/v2/collections/community/general/versions/0.1.1>`_
+            and the `Galaxy v3 REST API
+            <https://beta-galaxy.ansible.com/api/v3/plugin/ansible/content/published/collections/index/community/general/versions/0.1.1/>`_
         """
+        context = await self._ensure_context()
+
         collection = collection.replace('.', '/')
-        galaxy_url = urljoin(self.galaxy_server,
-                             f'api/v2/collections/{collection}/versions/{version}/')
+        galaxy_url = urljoin(context.base_url, f'collections/{collection}/versions/{version}/')
 
         async with retry_get(self.aio_session, galaxy_url, params=self.params,
-                             acceptable_error_codes=[404]) as response:
+                             headers=self.headers, acceptable_error_codes=[404]) as response:
             if response.status == 404:
                 raise NoSuchCollection(f'No collection found at: {galaxy_url}')
             collection_info = await response.json()
 
         return collection_info
 
     async def get_latest_matching_version(self, collection: str,
@@ -208,28 +338,31 @@
 
 
 class CollectionDownloader(GalaxyClient):
     """Manage downloading collections from Galaxy."""
 
     def __init__(self, aio_session: aiohttp.client.ClientSession,
                  download_dir: str,
-                 galaxy_server: str = _GALAXY_SERVER_URL,
-                 collection_cache: str | None = None) -> None:
+                 galaxy_server: t.Optional[str] = None,
+                 collection_cache: str | None = None,
+                 context: t.Optional[GalaxyContext] = None) -> None:
         """
         Create an object to download collections from galaxy.
 
         :arg aio_session: :obj:`aiohttp.ClientSession` with which to perform all
             requests to galaxy.
         :arg download_dir: Directory to download into.
-        :kwarg galaxy_server: URL to the galaxy server.
+        :kwarg galaxy_server: URL to the galaxy server. ``context`` must be provided instead
+            in the future.
+        :kwarg context: A ``GalaxyContext`` instance. Must be provided in the future.
         :kwarg collection_cache: If given, a path to a directory containing collection tarballs.
             These tarballs will be used instead of downloading new tarballs provided that the
             versions match the criteria (latest compatible version known to galaxy).
         """
-        super().__init__(aio_session, galaxy_server)
+        super().__init__(aio_session, galaxy_server=galaxy_server, context=context)
         self.download_dir = download_dir
         self.collection_cache: t.Final[str | None] = collection_cache
 
     async def download(self, collection: str, version: str | semver.Version, ) -> str:
         """
         Download a collection.
```

### Comparing `antsibull_core-2.0.0a1/src/antsibull_core/logging.py` & `antsibull_core-2.0.0a2/src/antsibull_core/logging.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-2.0.0a1/src/antsibull_core/schemas/config.py` & `antsibull_core-2.0.0a2/src/antsibull_core/schemas/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,21 @@
 import typing as t
 from collections.abc import Callable, Mapping, MutableMapping, MutableSequence, Sequence
 
 import pydantic as p
 import twiggy.formats  # type: ignore[import]
 import twiggy.outputs  # type: ignore[import]
 
-from .validators import convert_bool, convert_none, convert_path
-
+from .validators import convert_none, convert_path
 
 #: Valid choices for a logging level field
 LEVEL_CHOICES_F = p.Field(..., regex='^(CRITICAL|ERROR|WARNING|NOTICE|INFO|DEBUG|DISABLED)$')
 
 #: Valid choices for a logging level field
-DOC_PARSING_BACKEND_CHOICES_F = p.Field(
+_DOC_PARSING_BACKEND_CHOICES_F = p.Field(
     'ansible-internal', regex='^(auto|ansible-doc|ansible-core-2.13|ansible-internal)$')
 
 #: Valid choice of the logging version field
 VERSION_CHOICES_F = p.Field(..., regex=r'1\.0')
 
 
 #
@@ -117,28 +116,24 @@
      })
 
 
 # This class is no longer needed, it will eventually be removed
 class ConfigModel(BaseModel):
     # pyre-ignore[8]: https://github.com/samuelcolvin/pydantic/issues/1684
     ansible_base_url: p.HttpUrl = 'https://github.com/ansible/ansible'  # type: ignore[assignment]
-    breadcrumbs: p.StrictBool = True
     chunksize: int = 4096
-    doc_parsing_backend: str = DOC_PARSING_BACKEND_CHOICES_F
+    # DEPRECATED: doc_parsing_backend will be removed in antsibull-core 3.0.0
+    doc_parsing_backend: str = _DOC_PARSING_BACKEND_CHOICES_F
     # pyre-ignore[8]: https://github.com/samuelcolvin/pydantic/issues/1684
     galaxy_url: p.HttpUrl = 'https://galaxy.ansible.com/'  # type: ignore[assignment]
-    indexes: p.StrictBool = True
     logging_cfg: LoggingModel = DEFAULT_LOGGING_CONFIG
     max_retries: int = 10
     process_max: t.Optional[int] = None
     # pyre-ignore[8]: https://github.com/samuelcolvin/pydantic/issues/1684
     pypi_url: p.HttpUrl = 'https://pypi.org/'  # type: ignore[assignment]
-    use_html_blobs: p.StrictBool = False
     thread_max: int = 8
     file_check_content: int = 262144
     collection_cache: t.Optional[str] = None
 
     _convert_nones = p.validator('process_max', pre=True, allow_reuse=True)(convert_none)
-    _convert_bools = p.validator('breadcrumbs', 'indexes', 'use_html_blobs',
-                                 pre=True, allow_reuse=True)(convert_bool)
     _convert_paths = p.validator('collection_cache',
                                  pre=True, allow_reuse=True)(convert_path)
```

### Comparing `antsibull_core-2.0.0a1/src/antsibull_core/schemas/context.py` & `antsibull_core-2.0.0a2/src/antsibull_core/schemas/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 # SPDX-FileCopyrightText: 2021, Toshio Kuratomi
 """Schemas for app and lib contexts."""
 
 import typing as t
 
 import pydantic as p
 
-from .config import DEFAULT_LOGGING_CONFIG, LoggingModel
-from .validators import convert_bool, convert_none, convert_path
 from ..utils.collections import ContextDict
+from .config import DEFAULT_LOGGING_CONFIG, LoggingModel
+from .validators import convert_none, convert_path
 
 
 class BaseModel(p.BaseModel):
     """
     Configuration for all Context object classes.
 
     :cvar Config: Sets the following information
@@ -45,42 +45,32 @@
 
     :ivar extra: a mapping of arg/config keys to values.  Anything in here is unchecked by a
         schema.  These are usually leftover command line arguments and config entries. If
         values stored in extras need default values, they need to be set outside of the context
         or the entries can be given an actual entry in the AppContext to take advantage of the
         schema's checking, normalization, and default setting.
     :ivar ansible_base_url: Url to the ansible-core git repo.
-    :ivar breadcrumbs: If True, build with breadcrumbs on the plugin pages (this takes more memory).
-    :ivar use_html_blobs: If True, use HTML blobs instead of RST tables for option and return value
-        tables (this takes less memory).
     :ivar galaxy_url: URL of the galaxy server to get collection info from
-    :ivar indexes: If True, create index pages for all collections and all plugins in a collection.
     :ivar logging_cfg: Configuration of the application logging
     :ivar pypi_url: URL of the pypi server to query for information
     :ivar collection_cache: If set, must be a path pointing to a directory where collection
         tarballs are cached so they do not need to be downloaded from Galaxy twice.
     """
 
     extra: ContextDict = ContextDict()
     # pyre-ignore[8]: https://github.com/samuelcolvin/pydantic/issues/1684
     ansible_base_url: p.HttpUrl = 'https://github.com/ansible/ansible/'  # type: ignore[assignment]
-    breadcrumbs: p.StrictBool = True
     # pyre-ignore[8]: https://github.com/samuelcolvin/pydantic/issues/1684
     galaxy_url: p.HttpUrl = 'https://galaxy.ansible.com/'  # type: ignore[assignment]
-    indexes: p.StrictBool = True
     logging_cfg: LoggingModel = LoggingModel.parse_obj(DEFAULT_LOGGING_CONFIG)
     # pyre-ignore[8]: https://github.com/samuelcolvin/pydantic/issues/1684
     pypi_url: p.HttpUrl = 'https://pypi.org/'  # type: ignore[assignment]
-    use_html_blobs: p.StrictBool = False
     collection_cache: t.Optional[str] = None
 
     # pylint: disable-next=unused-private-member
-    __convert_bools = p.validator('breadcrumbs', 'indexes', 'use_html_blobs',
-                                  pre=True, allow_reuse=True)(convert_bool)
-    # pylint: disable-next=unused-private-member
     __convert_paths = p.validator('collection_cache',
                                   pre=True, allow_reuse=True)(convert_path)
 
 
 class LibContext(BaseModel):
     """
     Structure and defaults of the lib_ctx.
@@ -91,21 +81,24 @@
     :ivar thread_max: Maximum number of helper threads for parallel operations
     :ivar file_check_content: Maximum number of bytes of a file to read before writing it to
         compare contents. If contents are as expected, file is not overwritten. Set to 0 to
         disable.
     :ivar max_retries: Maximum number of times to retry an http request (in case of timeouts and
         other transient problems.
     :ivar doc_parsing_backend: The backend to use for parsing the documentation strings from
-        plugins.  'auto' selects a backend depending on the ansible-core version.
+        plugins.  This is DEPRECATED and will be removed from the library context in
+        antsibull-core 3.0.0.
+        'auto' selects a backend depending on the ansible-core version.
         'ansible-internal' is the fastest, but does not work with ansible-core 2.13+.
         'ansible-core-2.13' is also very fast, but requires ansible-core 2.13+.
         'ansible-doc' exists in case of problems with the ansible-internal backend.
     """
 
     chunksize: int = 4096
+    # DEPRECATED: doc_parsing_backend will be removed in antsibull-core 3.0.0
     doc_parsing_backend: str = 'auto'
     max_retries: int = 10
     process_max: t.Optional[int] = None
     thread_max: int = 8
     file_check_content: int = 262144
 
     # pylint: disable-next=unused-private-member
```

### Comparing `antsibull_core-2.0.0a1/src/antsibull_core/schemas/validators.py` & `antsibull_core-2.0.0a2/src/antsibull_core/schemas/validators.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-2.0.0a1/src/antsibull_core/tarball.py` & `antsibull_core-2.0.0a2/src/antsibull_core/tarball.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 # SPDX-FileCopyrightText: 2020, Ansible Project
 """Functions for working with tarballs."""
 
 from __future__ import annotations
 
 import re
 
-import sh
-
+from antsibull_core.subprocess_util import async_log_run
 
 #: Regex to find toplevel directories in tar output
 TOPLEVEL_RE: re.Pattern = re.compile('^[^/]+/$')
 
 
 class InvalidTarball(Exception):
     """Raised when a requested version does not exist."""
@@ -25,25 +24,25 @@
     Unpack a tarball.
 
     :arg tarname: The tarball to unpack.
     :arg destdir: The destination to unpack into.
     :returns: Toplevel of the unpacked directory structure.  This will be
         a subdirectory of `destdir`.
     """
-    # FIXME: Need to run tar via run_in_executor()
-    # FIXME: Use unpack_tarball for places that are manually calling tar now
-    # pyre-ignore[16]
-    manifest = sh.tar('-xzvf', tarname, f'-C{destdir}')  # pylint:disable=no-member
-    toplevel_dirs = [filename for filename in manifest if TOPLEVEL_RE.match(filename)]
+    manifest = await async_log_run(['tar', '-xzvf', tarname, f'-C{destdir}'])
+    toplevel_dirs = [
+        filename for filename in manifest.stdout.splitlines()
+        if TOPLEVEL_RE.match(filename)
+    ]
 
     if len(toplevel_dirs) != 1:
         raise InvalidTarball(f'The tarball {tarname} had more than a single toplevel dir')
 
     expected_dirname = tarname[:-len('.tar.gz')]
     if toplevel_dirs[0] != expected_dirname:
         raise InvalidTarball(f'The directory in {tarname} was not {expected_dirname}')
 
     return toplevel_dirs[0]
 
 
-async def pack_tarball(tarname: str, directory: str) -> str:  # pylint:disable=unused-argument
+async def pack_tarball(tarname: str, directory: str) -> str:
     raise NotImplementedError('pack_tarball has not yet been implemented')
```

### Comparing `antsibull_core-2.0.0a1/src/antsibull_core/utils/collections.py` & `antsibull_core-2.0.0a2/src/antsibull_core/utils/collections.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-2.0.0a1/src/antsibull_core/utils/hashing.py` & `antsibull_core-2.0.0a2/src/antsibull_core/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-2.0.0a1/src/antsibull_core/utils/http.py` & `antsibull_core-2.0.0a2/src/antsibull_core/utils/http.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from collections.abc import Iterable, Mapping
 
 import aiohttp
 
 from .. import app_context
 from ..logging import log
 
-
 mlog = log.fields(mod=__name__)
 
 
 def _format_call(command: str, args: tuple[t.Any, ...], kwargs: Mapping[str, t.Any]) -> str:
     arguments = [repr(a) for a in args] + [f'{k}={repr(v)}' for k, v in kwargs.items()]
     return f'aio_session.{command}({", ".join(arguments)})'
 
@@ -79,15 +78,15 @@
                 f'{", finally failed." if failed else ", retrying..."}')
             if failed:
                 break
 
             await asyncio.sleep(math.pow(1.5, retry) * wait_factor + (0.5 + random.uniform(0, 1)))
 
         flog.debug('Raise error')
-        raise Exception(
+        raise RuntimeError(
             f'Repeated error when calling {self.call_string}: received status codes '
             f'{", ".join(errors)}')
 
     async def __aexit__(self, exc_type, exc, tb) -> None:
         flog = mlog.fields(func='RetryGetManager.__aexit__')
         flog.debug('Enter')
         response = self.response
```

### Comparing `antsibull_core-2.0.0a1/src/antsibull_core/utils/io.py` & `antsibull_core-2.0.0a2/src/antsibull_core/utils/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 import typing as t
 
 import aiofiles
 
 from .. import app_context
 from ..logging import log
 
-
 if t.TYPE_CHECKING:
     from _typeshed import StrOrBytesPath
 
 mlog = log.fields(mod=__name__)
 
 
 async def copy_file(source_path: StrOrBytesPath, dest_path: StrOrBytesPath) -> None:
```

### Comparing `antsibull_core-2.0.0a1/src/antsibull_core/vendored/_argparse_booleanoptionalaction.py` & `antsibull_core-2.0.0a2/src/antsibull_core/vendored/_argparse_booleanoptionalaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # The intention is that this is used from antsibull.compat.BooleanOptionalAction rather than from
 # this file. That way we use the version in the python stdlib if it is available and use this
 # code if it is not.
 
 # pylint:disable=missing-module-docstring,redefined-builtin
 
-from argparse import Action, SUPPRESS, OPTIONAL, ZERO_OR_MORE
+from argparse import OPTIONAL, SUPPRESS, ZERO_OR_MORE, Action
 
 
 def _add_default_to_help_string(action):
     """
     Add the default value to the option help message.
 
     ArgumentDefaultsHelpFormatter and BooleanOptionalAction both want to add
```

### Comparing `antsibull_core-2.0.0a1/src/antsibull_core/vendored/collections.py` & `antsibull_core-2.0.0a2/src/antsibull_core/vendored/collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) 2018, Sviatoslav Sydorenko <ssydoren@redhat.com>
 # Copyright (c) 2018, Ansible Project
 # Simplified BSD License (see LICENSES/BSD-2-Clause.txt or
 # https://opensource.org/licenses/BSD-2-Clause)
 # SPDX-License-Identifier: BSD-2-Clause
 """Collection of low-level utility functions."""
 
-# pylint:disable=consider-using-f-string,consider-iterating-dictionary,use-dict-literal
+# pylint:disable=consider-using-f-string,consider-iterating-dictionary,use-dict-literal,broad-exception-raised
 
 from collections.abc import Hashable, Mapping, Sequence
 
 
 class ImmutableDict(Hashable, Mapping):
     """Dictionary that cannot be updated"""
     def __init__(self, *args, **kwargs):
```

### Comparing `antsibull_core-2.0.0a1/src/antsibull_core/vendored/json_utils.py` & `antsibull_core-2.0.0a2/src/antsibull_core/vendored/json_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # BSD 2-clause license (see LICENSES/BSD-2-Clause.txt)
 # SPDX-FileCopyrightText: Ansible Project
 # SPDX-License-Identifier: BSD-2-Clause
 
 # pylint:disable=missing-module-docstring,no-else-break,redundant-u-string-prefix
-# pylint:disable=undefined-loop-variable
 
 
 # NB: a copy of this function exists in ../../modules/core/async_wrapper.py. Ensure any
 # changes are propagated there.
 def _filter_non_json_lines(data):
     '''
     Used to filter unrelated output around module JSON output, like messages from
```

### Comparing `antsibull_core-2.0.0a1/src/antsibull_core/yaml.py` & `antsibull_core-2.0.0a2/src/antsibull_core/yaml.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 
 import yaml
 
 _SafeLoader: t.Any
 _SafeDumper: t.Any
 try:
     # use C version if possible for speedup
-    from yaml import CSafeLoader as _SafeLoader
     from yaml import CSafeDumper as _SafeDumper
+    from yaml import CSafeLoader as _SafeLoader
 except ImportError:
-    from yaml import SafeLoader as _SafeLoader
     from yaml import SafeDumper as _SafeDumper
+    from yaml import SafeLoader as _SafeLoader
 
 if t.TYPE_CHECKING:
-    from _typeshed import SupportsWrite, StrOrBytesPath
+    from _typeshed import StrOrBytesPath, SupportsWrite
 
 
 def load_yaml_bytes(data: bytes) -> t.Any:
     """
     Load and parse YAML from given bytes.
     """
     return yaml.load(data, Loader=_SafeLoader)
```

### Comparing `antsibull_core-2.0.0a1/tests/functional/aiohttp_utils.py` & `antsibull_core-2.0.0a2/tests/functional/aiohttp_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 # This program is distributed under the MIT license, a copy of which you should
 # have receveived along with it. If not, see <https://opensource.org/licenses/MIT>.
 #
 # SPDX-License-Identifier: MIT
 #
 # https://github.com/solid-abstractions/python/tree/master/testing-aiohttp-clients
 
-import aiohttp
-import aiohttp.test_utils
-import aiohttp.web
 import asyncio
 import collections
 import inspect
-import pytest
 import socket
 import weakref
 
+import aiohttp
+import aiohttp.test_utils
+import aiohttp.web
+import pytest
+
 # ----------------------------------------------------------------------------
 
 _RedirectContext = collections.namedtuple('RedirectContext', 'add_server session')
 
 @pytest.fixture
 async def http_redirect(ssl_certificate):
     ''' An HTTP ClientSession fixture that redirects requests to local test servers '''
```

### Comparing `antsibull_core-2.0.0a1/tests/functional/certificate_utils.py` & `antsibull_core-2.0.0a2/tests/functional/certificate_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 #
 # SPDX-License-Identifier: MIT
 #
 # https://github.com/solid-abstractions/python/tree/master/testing-aiohttp-clients
 
 import contextlib
 import datetime
-import pytest
 import ssl
 import tempfile
 
+import pytest
+
 
 class TemporaryCertificate:
     ''' Certificate representation used by :func:`ssl_certificate` fixture '''
 
     def __enter__(self):
         from cryptography import x509
         from cryptography.hazmat.backends import default_backend
```

### Comparing `antsibull_core-2.0.0a1/tests/functional/test_dependency_files.py` & `antsibull_core-2.0.0a2/tests/functional/test_dependency_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # GNU General Public License v3.0+ (see LICENSES/GPL-3.0-or-later.txt or https://www.gnu.org/licenses/gpl-3.0.txt)
 # SPDX-License-Identifier: GPL-3.0-or-later
 # SPDX-FileCopyrightText: Ansible Project
 
+import pytest
 from packaging.version import Version as PypiVer
 from semantic_version import Version as SemVer
 
-import pytest
-
 from antsibull_core.dependency_files import BuildFile
 
-
 SIMPLE_TEST_FILE = """_ansible_version: 4
 _ansible_base_version: 2.11.0rc1
 community.general: >=1.0.0,<2.0.0
 community.routeros: >=2.0.0-a2,<3.0.0
 """
 
 SIMPLE_TEST_DEPS = {'community.general': SemVer('1.0.0'),
```

### Comparing `antsibull_core-2.0.0a1/tests/functional/test_logging.py` & `antsibull_core-2.0.0a2/tests/functional/test_logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # GNU General Public License v3.0+ (see LICENSES/GPL-3.0-or-later.txt or https://www.gnu.org/licenses/gpl-3.0.txt)
 # SPDX-License-Identifier: GPL-3.0-or-later
 # SPDX-FileCopyrightText: Ansible Project
 
 import os
 
 import pytest
-
 import twiggy.levels
 
 import antsibull_core.logging as al
 
 
 def test_library_settings(capsys):
     """Importing without calling initialize_app_logging leaves logging disabled."""
```

### Comparing `antsibull_core-2.0.0a1/tests/units/test_ansible_core.py` & `antsibull_core-2.0.0a2/tests/units/test_ansible_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # GNU General Public License v3.0+ (see LICENSES/GPL-3.0-or-later.txt or https://www.gnu.org/licenses/gpl-3.0.txt)
 # SPDX-License-Identifier: GPL-3.0-or-later
 # SPDX-FileCopyrightText: Ansible Project
 
-from packaging.version import  Version
 import pytest
+from packaging.version import Version
 
 import antsibull_core.ansible_core as ac
 
 
 @pytest.mark. parametrize('version', ('2.9', '2.9.10', '1.0', '1', '0.7', '2.10', '2.10.0',
                                       '2.10.8', '2.10.12'))
 def test_get_core_package_name_returns_ansible_base(version):
```

### Comparing `antsibull_core-2.0.0a1/tests/units/test_context.py` & `antsibull_core-2.0.0a2/tests/units/test_context.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-2.0.0a1/tests/units/test_parse_pieces.py` & `antsibull_core-2.0.0a2/tests/units/test_parse_pieces.py`

 * *Files identical despite different names*

### Comparing `antsibull_core-2.0.0a1/setup.py` & `antsibull_core-2.0.0a2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,72 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+<!--
+Copyright (c) Ansible Project
+GNU General Public License v3.0+ (see LICENSES/GPL-3.0-or-later.txt or https://www.gnu.org/licenses/gpl-3.0.txt)
+SPDX-License-Identifier: GPL-3.0-or-later
+-->
+
+# antsibull-core -- Library for Ansible Build Scripts
+[![Discuss on Matrix at #community:ansible.com](https://img.shields.io/matrix/community:ansible.com.svg?server_fqdn=ansible-accounts.ems.host&label=Discuss%20on%20Matrix%20at%20%23community:ansible.com&logo=matrix)](https://matrix.to/#/#community:ansible.com)
+[![Nox badge](https://github.com/ansible-community/antsibull-core/actions/workflows/nox.yml/badge.svg)](https://github.com/ansible-community/antsibull-core/actions/workflows/nox.yml)
+[![Codecov badge](https://img.shields.io/codecov/c/github/ansible-community/antsibull-core)](https://codecov.io/gh/ansible-community/antsibull-core)
+[![REUSE status](https://api.reuse.software/badge/github.com/ansible-community/antsibull-core)](https://api.reuse.software/info/github.com/ansible-community/antsibull-core)
+
+Library needed for tooling for building various things related to Ansible.
+
+You can find a list of changes in [the antsibull-core changelog](./CHANGELOG.rst).
+
+Unless otherwise noted in the code, it is licensed under the terms of the GNU
+General Public License v3 or, at your option, later.
+
+antsibull-core is covered by the [Ansible Code of Conduct](https://docs.ansible.com/ansible/latest/community/code_of_conduct.html).
+
+## Versioning and compatibility
+
+From version 1.0.0 on, antsibull-core sticks to semantic versioning and aims at providing no backwards compatibility breaking changes during a major release cycle. We might make exceptions from this in case of security fixes for vulnerabilities that are severe enough.
+
+The current major version is 2.x.y. Development for 2.x.y occurs on the `main` branch. 2.x.y mainly differs from 1.x.y by dropping support for Python 3.6, 3.7, and 3.8. It deprecates several compatibility functions for older Python versions that are no longer needed; see the changelog for details. 1.x.y is still developed on the `stable-1` branch, but only security fixes, major bugfixes, and other changes that are absolutely necessary for the other antsibull projects will be backported.
+
+## Development
+
+Install and run `nox` to run all tests. That's it for simple contributions!
+`nox` will create virtual environments in `.nox` inside the checked out project
+and install the requirements needed to run the tests there.
+
+To run specific tests:
+
+1. `nox -e test` to only run unit tests;
+2. `nox -e coverage` to display combined coverage results after running `nox -e
+   test`;
+3. `nox -e lint` to run all linters and formatters at once;
+4. `nox -e formatters` to run `isort`;
+3. `nox -e codeqa` to run `flake8`, `pylint`, `reuse lint`, and `antsibull-changelog lint`;
+6. `nox -e typing` to run `mypy` and `pyre`
+
+## Creating a new release:
+
+1. Run `nox -e bump -- <version> <release_summary_message>`. This:
+   * Bumps the package version in `pyproject.toml`.
+   * Creates `changelogs/fragments/<version>.yml` with a `release_summary` section.
+   * Runs `antsibull-changelog release` and adds the changed files to git.
+   * Commits with message `Release <version>.` and runs `git tag -a -m 'antsibull-core <version>' <version>`.
+   * Runs `hatch build`.
+2. Run `git push` to the appropriate remotes.
+3. Once CI passes on GitHub, run `nox -e publish`. This:
+   * Runs `hatch publish`;
+   * Bumps the version to `<version>.post0`;
+   * Adds the changed file to git and run `git commit -m 'Post-release version bump.'`;
+4. Run `git push --follow-tags` to the appropriate remotes and create a GitHub release.
+
+## License
+
+Unless otherwise noted in the code, it is licensed under the terms of the GNU
+General Public License v3 or, at your option, later. See
+[LICENSES/GPL-3.0-or-later.txt](https://github.com/ansible-community/antsibull-changelog/tree/main/LICENSE)
+for a copy of the license.
+
+Parts of the code are vendored from other sources and are licensed under other licenses:
+1. `src/antsibull_core/vendored/collections.py` and `src/antsibull_core/vendored/json_utils.py` are licensed under the terms of the BSD 2-Clause license. See [LICENSES/BSD-2-Clause.txt](https://github.com/ansible-community/antsibull-changelog/tree/main/LICENSES/BSD-2-Clause.txt) for a copy of the license.
+2. `tests/functional/aiohttp_utils.py` and `tests/functional/certificate_utils.py` are licensed under the terms of the MIT license. See [LICENSES/MIT.txt](https://github.com/ansible-community/antsibull-changelog/tree/main/LICENSES/MIT.txt) for a copy of the license.
+3. `src/antsibull_core/vendored/_argparse_booleanoptionalaction.py` is licensed under the terms of the Python Software Foundation license version 2. See [LICENSES/PSF-2.0.txt](https://github.com/ansible-community/antsibull-changelog/tree/main/LICENSES/PSF-2.0.txt) for a copy of the license.
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['antsibull_core',
- 'antsibull_core.schemas',
- 'antsibull_core.utils',
- 'antsibull_core.vendored',
- 'tests',
- 'tests.functional',
- 'tests.units']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyYAML',
- 'aiofiles',
- 'aiohttp>=3.0.0',
- 'packaging>=20.0',
- 'perky',
- 'pydantic',
- 'semantic_version',
- 'sh',
- 'twiggy>=0.5.0']
-
-setup_kwargs = {
-    'name': 'antsibull-core',
-    'version': '2.0.0a1',
-    'description': 'Tools for building the Ansible Distribution',
-    'long_description': '<!--\nCopyright (c) Ansible Project\nGNU General Public License v3.0+ (see LICENSES/GPL-3.0-or-later.txt or https://www.gnu.org/licenses/gpl-3.0.txt)\nSPDX-License-Identifier: GPL-3.0-or-later\n-->\n\n# antsibull-core -- Library for Ansible Build Scripts\n[![Python linting badge](https://github.com/ansible-community/antsibull-core/workflows/Python%20linting/badge.svg?event=push&branch=main)](https://github.com/ansible-community/antsibull-core/actions?query=workflow%3A%22Python+linting%22+branch%3Amain)\n[![Python testing badge](https://github.com/ansible-community/antsibull-core/workflows/Python%20testing/badge.svg?event=push&branch=main)](https://github.com/ansible-community/antsibull-core/actions?query=workflow%3A%22Python+testing%22+branch%3Amain)\n[![Codecov badge](https://img.shields.io/codecov/c/github/ansible-community/antsibull-core)](https://codecov.io/gh/ansible-community/antsibull-core)\n\nLibrary needed for tooling for building various things related to Ansible.\n\nYou can find a list of changes in [the antsibull-core changelog](./CHANGELOG.rst).\n\nUnless otherwise noted in the code, it is licensed under the terms of the GNU\nGeneral Public License v3 or, at your option, later.\n\nantsibull-core is covered by the [Ansible Code of Conduct](https://docs.ansible.com/ansible/latest/community/code_of_conduct.html).\n\n## Versioning and compatibility\n\nFrom version 1.0.0 on, antsibull-core sticks to semantic versioning and aims at providing no backwards compatibility breaking changes during a major release cycle. We might make exceptions from this in case of security fixes for vulnerabilities that are severe enough.\n\nThe current major version is 2.x.y. Development for 2.x.y occurs on the `main` branch. 2.x.y mainly differs from 1.x.y by dropping support for Python 3.6, 3.7, and 3.8. It deprecates several compatibility functions for older Python versions that are no longer needed; see the changelog for details. 1.x.y is still developed on the `stable-1` branch, but only security fixes, major bugfixes, and other changes that are absolutely necessary for the other antsibull projects will be backported.\n\n## Creating a new release:\n\nIf you want to create a new release::\n\n    vim pyproject.toml  # Make sure version number is correct\n    vim changelogs/fragment/$VERSION_NUMBER.yml  # create \'release_summary:\' fragment\n    antsibull-changelog release --version $VERSION_NUMBER\n    git add CHANGELOG.rst changelogs\n    git commit -m "Release $VERSION_NUMBER."\n    poetry build\n    poetry publish  # Uploads to pypi.  Be sure you really want to do this\n\n    git tag $VERSION_NUMBER\n    git push --tags\n    vim pyproject.toml  # Bump the version number to X.Y.Z.post0\n    git commit -m \'Update the version number for the next release\' pyproject.toml\n    git push\n\n## License\n\nUnless otherwise noted in the code, it is licensed under the terms of the GNU\nGeneral Public License v3 or, at your option, later. See\n[LICENSES/GPL-3.0-or-later.txt](https://github.com/ansible-community/antsibull-changelog/tree/main/LICENSE)\nfor a copy of the license.\n\nParts of the code are vendored from other sources and are licensed under other licenses:\n1. `src/antsibull_core/vendored/collections.py` and `src/antsibull_core/vendored/json_utils.py` are licensed under the terms of the BSD 2-Clause license. See [LICENSES/BSD-2-Clause.txt](https://github.com/ansible-community/antsibull-changelog/tree/main/LICENSES/BSD-2-Clause.txt) for a copy of the license.\n2. `tests/functional/aiohttp_utils.py` and `tests/functional/certificate_utils.py` are licensed under the terms of the MIT license. See [LICENSES/MIT.txt](https://github.com/ansible-community/antsibull-changelog/tree/main/LICENSES/MIT.txt) for a copy of the license.\n3. `src/antsibull_core/vendored/_argparse_booleanoptionalaction.py` is licensed under the terms of the Python Software Foundation license version 2. See [LICENSES/PSF-2.0.txt](https://github.com/ansible-community/antsibull-changelog/tree/main/LICENSES/PSF-2.0.txt) for a copy of the license.\n\nThe repository follows the [REUSE Specification](https://reuse.software/spec/) for declaring copyright and\nlicensing information. The only exception are changelog fragments in ``changelog/fragments/``.\n',
-    'author': 'Toshio Kuratomi',
-    'author_email': 'a.badger@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/ansible-community/antsibull-core',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9.0,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
+The repository follows the [REUSE Specification](https://reuse.software/spec/) for declaring copyright and
+licensing information. The only exception are changelog fragments in ``changelog/fragments/``.
```

### Comparing `antsibull_core-2.0.0a1/PKG-INFO` & `antsibull_core-2.0.0a2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,79 @@
 Metadata-Version: 2.1
 Name: antsibull-core
-Version: 2.0.0a1
+Version: 2.0.0a2
 Summary: Tools for building the Ansible Distribution
-Home-page: https://github.com/ansible-community/antsibull-core
-License: GPL-3.0-or-later
-Author: Toshio Kuratomi
-Author-email: a.badger@gmail.com
-Requires-Python: >=3.9.0,<4.0.0
+Project-URL: Source code, https://github.com/ansible-community/antsibull-core
+Project-URL: Code of Conduct, https://docs.ansible.com/ansible/latest/community/code_of_conduct.html
+Project-URL: Bug tracker, https://github.com/ansible-community/antsibull-core/issues
+Author-email: Toshio Kuratomi <a.badger@gmail.com>, Felix Fontein <felix@fontein.de>
+Maintainer-email: Felix Fontein <felix@fontein.de>, Maxwell G <maxwell@gtmx.me>
+License-Expression: GPL-3.0-or-later AND BSD-2-Clause AND MIT AND PSF-2.0
+License-File: LICENSES/BSD-2-Clause.txt
+License-File: LICENSES/GPL-3.0-or-later.txt
+License-File: LICENSES/MIT.txt
+License-File: LICENSES/PSF-2.0.txt
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Ansible
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: PyYAML
+Classifier: Typing :: Typed
+Requires-Python: >=3.9
 Requires-Dist: aiofiles
-Requires-Dist: aiohttp (>=3.0.0)
-Requires-Dist: packaging (>=20.0)
+Requires-Dist: aiohttp>=3.0.0
+Requires-Dist: build
+Requires-Dist: packaging>=20.0
 Requires-Dist: perky
-Requires-Dist: pydantic
-Requires-Dist: semantic_version
-Requires-Dist: sh
-Requires-Dist: twiggy (>=0.5.0)
-Project-URL: Bug tracker, https://github.com/ansible-community/antsibull-core/issues
-Project-URL: Code of Conduct, https://docs.ansible.com/ansible/latest/community/code_of_conduct.html
-Project-URL: Repository, https://github.com/ansible-community/antsibull-core
+Requires-Dist: pydantic<2.0.0,>=1.0.0
+Requires-Dist: pyyaml
+Requires-Dist: semantic-version
+Requires-Dist: sh<2.0.0,>=1.0.0
+Requires-Dist: twiggy>=0.5.0
+Provides-Extra: codeqa
+Requires-Dist: antsibull-changelog; extra == 'codeqa'
+Requires-Dist: flake8>=6.0.0; extra == 'codeqa'
+Requires-Dist: pylint>=2.15.7; extra == 'codeqa'
+Requires-Dist: reuse; extra == 'codeqa'
+Provides-Extra: coverage
+Requires-Dist: coverage[toml]; extra == 'coverage'
+Provides-Extra: dev
+Requires-Dist: antsibull-core[codeqa]; extra == 'dev'
+Requires-Dist: antsibull-core[coverage]; extra == 'dev'
+Requires-Dist: antsibull-core[formatters]; extra == 'dev'
+Requires-Dist: antsibull-core[test]; extra == 'dev'
+Requires-Dist: antsibull-core[typing]; extra == 'dev'
+Requires-Dist: nox; extra == 'dev'
+Provides-Extra: test
+Requires-Dist: asynctest; extra == 'test'
+Requires-Dist: cryptography; extra == 'test'
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-asyncio>=0.20; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Requires-Dist: pytest-error-for-skips; extra == 'test'
+Provides-Extra: typing
+Requires-Dist: mypy; extra == 'typing'
+Requires-Dist: pyre-check>=0.9.17; extra == 'typing'
+Requires-Dist: types-aiofiles; extra == 'typing'
+Requires-Dist: types-pyyaml; extra == 'typing'
 Description-Content-Type: text/markdown
 
 <!--
 Copyright (c) Ansible Project
 GNU General Public License v3.0+ (see LICENSES/GPL-3.0-or-later.txt or https://www.gnu.org/licenses/gpl-3.0.txt)
 SPDX-License-Identifier: GPL-3.0-or-later
 -->
 
 # antsibull-core -- Library for Ansible Build Scripts
-[![Python linting badge](https://github.com/ansible-community/antsibull-core/workflows/Python%20linting/badge.svg?event=push&branch=main)](https://github.com/ansible-community/antsibull-core/actions?query=workflow%3A%22Python+linting%22+branch%3Amain)
-[![Python testing badge](https://github.com/ansible-community/antsibull-core/workflows/Python%20testing/badge.svg?event=push&branch=main)](https://github.com/ansible-community/antsibull-core/actions?query=workflow%3A%22Python+testing%22+branch%3Amain)
+[![Discuss on Matrix at #community:ansible.com](https://img.shields.io/matrix/community:ansible.com.svg?server_fqdn=ansible-accounts.ems.host&label=Discuss%20on%20Matrix%20at%20%23community:ansible.com&logo=matrix)](https://matrix.to/#/#community:ansible.com)
+[![Nox badge](https://github.com/ansible-community/antsibull-core/actions/workflows/nox.yml/badge.svg)](https://github.com/ansible-community/antsibull-core/actions/workflows/nox.yml)
 [![Codecov badge](https://img.shields.io/codecov/c/github/ansible-community/antsibull-core)](https://codecov.io/gh/ansible-community/antsibull-core)
+[![REUSE status](https://api.reuse.software/badge/github.com/ansible-community/antsibull-core)](https://api.reuse.software/info/github.com/ansible-community/antsibull-core)
 
 Library needed for tooling for building various things related to Ansible.
 
 You can find a list of changes in [the antsibull-core changelog](./CHANGELOG.rst).
 
 Unless otherwise noted in the code, it is licensed under the terms of the GNU
 General Public License v3 or, at your option, later.
@@ -51,31 +82,44 @@
 
 ## Versioning and compatibility
 
 From version 1.0.0 on, antsibull-core sticks to semantic versioning and aims at providing no backwards compatibility breaking changes during a major release cycle. We might make exceptions from this in case of security fixes for vulnerabilities that are severe enough.
 
 The current major version is 2.x.y. Development for 2.x.y occurs on the `main` branch. 2.x.y mainly differs from 1.x.y by dropping support for Python 3.6, 3.7, and 3.8. It deprecates several compatibility functions for older Python versions that are no longer needed; see the changelog for details. 1.x.y is still developed on the `stable-1` branch, but only security fixes, major bugfixes, and other changes that are absolutely necessary for the other antsibull projects will be backported.
 
-## Creating a new release:
+## Development
+
+Install and run `nox` to run all tests. That's it for simple contributions!
+`nox` will create virtual environments in `.nox` inside the checked out project
+and install the requirements needed to run the tests there.
+
+To run specific tests:
+
+1. `nox -e test` to only run unit tests;
+2. `nox -e coverage` to display combined coverage results after running `nox -e
+   test`;
+3. `nox -e lint` to run all linters and formatters at once;
+4. `nox -e formatters` to run `isort`;
+3. `nox -e codeqa` to run `flake8`, `pylint`, `reuse lint`, and `antsibull-changelog lint`;
+6. `nox -e typing` to run `mypy` and `pyre`
 
-If you want to create a new release::
+## Creating a new release:
 
-    vim pyproject.toml  # Make sure version number is correct
-    vim changelogs/fragment/$VERSION_NUMBER.yml  # create 'release_summary:' fragment
-    antsibull-changelog release --version $VERSION_NUMBER
-    git add CHANGELOG.rst changelogs
-    git commit -m "Release $VERSION_NUMBER."
-    poetry build
-    poetry publish  # Uploads to pypi.  Be sure you really want to do this
-
-    git tag $VERSION_NUMBER
-    git push --tags
-    vim pyproject.toml  # Bump the version number to X.Y.Z.post0
-    git commit -m 'Update the version number for the next release' pyproject.toml
-    git push
+1. Run `nox -e bump -- <version> <release_summary_message>`. This:
+   * Bumps the package version in `pyproject.toml`.
+   * Creates `changelogs/fragments/<version>.yml` with a `release_summary` section.
+   * Runs `antsibull-changelog release` and adds the changed files to git.
+   * Commits with message `Release <version>.` and runs `git tag -a -m 'antsibull-core <version>' <version>`.
+   * Runs `hatch build`.
+2. Run `git push` to the appropriate remotes.
+3. Once CI passes on GitHub, run `nox -e publish`. This:
+   * Runs `hatch publish`;
+   * Bumps the version to `<version>.post0`;
+   * Adds the changed file to git and run `git commit -m 'Post-release version bump.'`;
+4. Run `git push --follow-tags` to the appropriate remotes and create a GitHub release.
 
 ## License
 
 Unless otherwise noted in the code, it is licensed under the terms of the GNU
 General Public License v3 or, at your option, later. See
 [LICENSES/GPL-3.0-or-later.txt](https://github.com/ansible-community/antsibull-changelog/tree/main/LICENSE)
 for a copy of the license.
@@ -83,8 +127,7 @@
 Parts of the code are vendored from other sources and are licensed under other licenses:
 1. `src/antsibull_core/vendored/collections.py` and `src/antsibull_core/vendored/json_utils.py` are licensed under the terms of the BSD 2-Clause license. See [LICENSES/BSD-2-Clause.txt](https://github.com/ansible-community/antsibull-changelog/tree/main/LICENSES/BSD-2-Clause.txt) for a copy of the license.
 2. `tests/functional/aiohttp_utils.py` and `tests/functional/certificate_utils.py` are licensed under the terms of the MIT license. See [LICENSES/MIT.txt](https://github.com/ansible-community/antsibull-changelog/tree/main/LICENSES/MIT.txt) for a copy of the license.
 3. `src/antsibull_core/vendored/_argparse_booleanoptionalaction.py` is licensed under the terms of the Python Software Foundation license version 2. See [LICENSES/PSF-2.0.txt](https://github.com/ansible-community/antsibull-changelog/tree/main/LICENSES/PSF-2.0.txt) for a copy of the license.
 
 The repository follows the [REUSE Specification](https://reuse.software/spec/) for declaring copyright and
 licensing information. The only exception are changelog fragments in ``changelog/fragments/``.
-
```

