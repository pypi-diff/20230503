# Comparing `tmp/docker-image-size-limit-0.4.1.tar.gz` & `tmp/docker_image_size_limit-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker-image-size-limit-0.4.1.tar", max compression
+gzip compressed data, was "docker_image_size_limit-1.0.0.tar", max compression
```

## Comparing `docker-image-size-limit-0.4.1.tar` & `docker_image_size_limit-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2019-03-03 09:05:33.030905 docker-image-size-limit-0.4.1/LICENSE
--rw-r--r--   0        0        0     3778 2020-04-15 08:35:13.870424 docker-image-size-limit-0.4.1/README.md
--rw-r--r--   0        0        0     2242 2021-02-14 13:09:14.746372 docker-image-size-limit-0.4.1/docker_image_size_limit/__init__.py
--rw-r--r--   0        0        0        0 2019-09-15 12:37:53.958132 docker-image-size-limit-0.4.1/docker_image_size_limit/py.typed
--rw-r--r--   0        0        0     1313 2021-07-23 08:10:18.989376 docker-image-size-limit-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     4829 2021-07-23 08:15:34.853665 docker-image-size-limit-0.4.1/setup.py
--rw-r--r--   0        0        0     4957 2021-07-23 08:15:34.853999 docker-image-size-limit-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-03 09:06:13.344278 docker_image_size_limit-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3778 2023-05-03 09:06:13.344565 docker_image_size_limit-1.0.0/README.md
+-rw-r--r--   0        0        0     1984 2023-05-03 09:06:13.345310 docker_image_size_limit-1.0.0/docker_image_size_limit/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 09:06:13.345443 docker_image_size_limit-1.0.0/docker_image_size_limit/py.typed
+-rw-r--r--   0        0        0      194 2023-05-03 09:38:19.523655 docker_image_size_limit-1.0.0/docker_image_size_limit/version.py
+-rw-r--r--   0        0        0     1353 2023-05-03 09:38:19.526617 docker_image_size_limit-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4980 1970-01-01 00:00:00.000000 docker_image_size_limit-1.0.0/PKG-INFO
```

### Comparing `docker-image-size-limit-0.4.1/LICENSE` & `docker_image_size_limit-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docker-image-size-limit-0.4.1/README.md` & `docker_image_size_limit-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `docker-image-size-limit-0.4.1/docker_image_size_limit/__init__.py` & `docker_image_size_limit-1.0.0/docker_image_size_limit/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 import argparse
 import os
 import sys
-from typing import TYPE_CHECKING, NoReturn
+from typing import NoReturn
 
 import docker
 from humanfriendly import format_size, parse_size
 
-if sys.version_info >= (3, 8) or TYPE_CHECKING:  # pragma: no cover
-    from importlib import metadata  # noqa: WPS433
-
-    lib_version = getattr(metadata, 'version')  # noqa: B009
-else:  # pragma: no cover
-    import importlib_metadata  # noqa: WPS433
-
-    lib_version = importlib_metadata.version
+from docker_image_size_limit.version import get_version
 
 #: We use this variable to show version spec.
-_version = lib_version(
+_version = get_version(
     os.path.basename(os.path.dirname(__file__)),
 )
 
 
 def main() -> NoReturn:
     """Main CLI entrypoint."""
     client = docker.from_env()
```

### Comparing `docker-image-size-limit-0.4.1/pyproject.toml` & `docker_image_size_limit-1.0.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,10 @@
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
-
-
-[tool.nitpick]
-style = "https://raw.githubusercontent.com/wemake-services/wemake-python-styleguide/master/styles/nitpick-style-wemake.toml"
-
-
 [tool.poetry]
 name = "docker-image-size-limit"
-version = "0.4.1"
+version = "1.0.0"
 description = ""
 license = "MIT"
 authors = [
   "Nikita Sobolev <mail@sobolevn.me>"
 ]
 
 readme = "README.md"
@@ -25,36 +16,48 @@
   "docker image",
   "size limit",
   "wemake.services",
   "code quality"
 ]
 
 classifiers = [
-  "Development Status :: 4 - Beta",
+  "Development Status :: 5 - Production/Stable",
   "Environment :: Console",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Software Development :: Quality Assurance",
 ]
 
+[tool.poetry.urls]
+"Funding" = "https://github.com/sponsors/wemake-services"
+
 [tool.poetry.scripts]
 disl = "docker_image_size_limit:main"
 
 [tool.poetry.dependencies]
-python = "^3.6"
-docker = ">=3.7,<6.0"
-humanfriendly = ">=4.18,<10.0"
-importlib-metadata = { version = "*", python = "<3.8" }
-
-[tool.poetry.dev-dependencies]
-pytest-cov = "^2.12"
-pytest-randomly = "^3.8"
+python = "^3.8"
+
+docker = ">=3.7,<7.0"
+humanfriendly = ">=4.18,<11.0"
+
+[tool.poetry.group.test.dependencies]
+pytest-cov = "^4.0"
+pytest-randomly = "^3.12"
 pytest-timeout = "^1.4"
-pytest = "^6.2"
+pytest = "^7.3"
+
+mypy = "^1.2"
+wemake-python-styleguide = "^0.17"
+flake8-pytest-style = "^1.6"
+nitpick = "^0.33"
+
+safety = "^2.3"
 
-mypy = "^0.910"
-wemake-python-styleguide = "^0.15"
-flake8-pytest-style = "^1.5"
-nitpick = "^0.27"
 
-safety = "^1.10"
+[build-system]
+requires = ["poetry-core>=1.5.0"]
+build-backend = "poetry.core.masonry.api"
+
+
+[tool.nitpick]
+style = "https://raw.githubusercontent.com/wemake-services/wemake-python-styleguide/master/styles/nitpick-style-wemake.toml"
```

### Comparing `docker-image-size-limit-0.4.1/setup.py` & `docker_image_size_limit-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,146 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: docker-image-size-limit
+Version: 1.0.0
+Summary: 
+Home-page: https://github.com/wemake-services/docker-image-size-limit
+License: MIT
+Keywords: docker,docker image,size limit,wemake.services,code quality
+Author: Nikita Sobolev
+Author-email: mail@sobolevn.me
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Quality Assurance
+Requires-Dist: docker (>=3.7,<7.0)
+Requires-Dist: humanfriendly (>=4.18,<11.0)
+Project-URL: Funding, https://github.com/sponsors/wemake-services
+Project-URL: Repository, https://github.com/wemake-services/docker-image-size-limit
+Description-Content-Type: text/markdown
 
-packages = \
-['docker_image_size_limit']
+# docker-image-size-limit
 
-package_data = \
-{'': ['*']}
+[![wemake.services](https://img.shields.io/badge/%20-wemake.services-green.svg?label=%20&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAABGdBTUEAALGPC%2FxhBQAAAAFzUkdCAK7OHOkAAAAbUExURQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAP%2F%2F%2F5TvxDIAAAAIdFJOUwAjRA8xXANAL%2Bv0SAAAADNJREFUGNNjYCAIOJjRBdBFWMkVQeGzcHAwksJnAPPZGOGAASzPzAEHEGVsLExQwE7YswCb7AFZSF3bbAAAAABJRU5ErkJggg%3D%3D)](https://wemake.services)
+[![Build status](https://github.com/wemake-services/docker-image-size-limit/workflows/test/badge.svg?branch=master&event=push)](https://github.com/wemake-services/docker-image-size-limit/actions?query=workflow%3Atest)
+[![codecov](https://codecov.io/gh/wemake-services/docker-image-size-limit/branch/master/graph/badge.svg)](https://codecov.io/gh/wemake-services/docker-image-size-limit)
+[![Python Version](https://img.shields.io/pypi/pyversions/docker-image-size-limit.svg)](https://pypi.org/project/docker-image-size-limit/)
+[![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)
 
-install_requires = \
-['docker>=3.7,<6.0', 'humanfriendly>=4.18,<10.0']
-
-extras_require = \
-{':python_version < "3.8"': ['importlib-metadata']}
-
-entry_points = \
-{'console_scripts': ['disl = docker_image_size_limit:main']}
-
-setup_kwargs = {
-    'name': 'docker-image-size-limit',
-    'version': '0.4.1',
-    'description': '',
-    'long_description': '# docker-image-size-limit\n\n[![wemake.services](https://img.shields.io/badge/%20-wemake.services-green.svg?label=%20&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAABGdBTUEAALGPC%2FxhBQAAAAFzUkdCAK7OHOkAAAAbUExURQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAP%2F%2F%2F5TvxDIAAAAIdFJOUwAjRA8xXANAL%2Bv0SAAAADNJREFUGNNjYCAIOJjRBdBFWMkVQeGzcHAwksJnAPPZGOGAASzPzAEHEGVsLExQwE7YswCb7AFZSF3bbAAAAABJRU5ErkJggg%3D%3D)](https://wemake.services)\n[![Build status](https://github.com/wemake-services/docker-image-size-limit/workflows/test/badge.svg?branch=master&event=push)](https://github.com/wemake-services/docker-image-size-limit/actions?query=workflow%3Atest)\n[![codecov](https://codecov.io/gh/wemake-services/docker-image-size-limit/branch/master/graph/badge.svg)](https://codecov.io/gh/wemake-services/docker-image-size-limit)\n[![Python Version](https://img.shields.io/pypi/pyversions/docker-image-size-limit.svg)](https://pypi.org/project/docker-image-size-limit/)\n[![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)\n\nLimit your `docker` image size with a simple CLI command.\nPerfect to be used inside your CI process.\n\nRead the [announcing post](https://sobolevn.me/2019/03/announcing-docker-image-size-limit).\n\n\n## Installation\n\n```bash\npip install docker-image-size-limit\n```\n\nOr use our [Github Action](https://github.com/wemake-services/docker-image-size-limit#github-action) or [pre-built docker image](https://github.com/wemake-services/docker-image-size-limit#docker-image).\n\n\n## Usage\n\nWe support just a single command:\n\n```bash\n$ disl your-image-name:label 300MiB\nyour-image-name:label exceeds 300MiB limit by 114.4 MiB\n```\n\n\n## Options\n\nYou can specify your image as:\n\n- Image name: `python`\n- Image name with tag: `python:3.6.6-alpine`\n\nYou can specify your size as:\n\n- Raw number of bytes: `1024`\n- Human-readable megabytes: `30 MB` or `30 MiB`\n- Human-readable gigabytes: `1 GB` or `1 GiB`\n- Any other size supported by [`humanfriendly`](https://humanfriendly.readthedocs.io/en/latest/api.html#humanfriendly.parse_size)\n\n\n## Programmatic usage\n\nYou can also import and use this library as `python` code:\n\n```python\nfrom docker import from_env\nfrom docker_image_size_limit import check_image_size\n\noversize = check_image_size(from_env(), \'image-name:latest\', \'1 GiB\')\nassert oversize < 0, \'Too big image!\'  # negative oversize - is a good thing!\n```\n\nWe also ship [PEP-561](https://www.python.org/dev/peps/pep-0561/)\ncompatible type annotations with this library.\n\n\n## Github Action\n\nYou can also use this check as a [Gihub Action](https://github.com/marketplace/actions/docker-image-size-limit):\n\n```yaml\n- uses: wemake-services/docker-image-size-limit@master\n  with:\n    image: "$YOUR_IMAGE_NAME"\n    size: "$YOUR_SIZE_LIMIT"\n```\n\nHere\'s [an example](https://github.com/wemake-services/docker-image-size-limit/actions?query=workflow%3Adisl).\n\n\n## Docker Image\n\nWe have a [pre-built image](https://hub.docker.com/r/wemakeservices/docker-image-size-limit) available.\n\nFirst, pull our pre-built docker image:\n\n```bash\ndocker pull wemakeservices/docker-image-size-limit\n```\n\nThen you can use it like so:\n\n```bash\ndocker run -v /var/run/docker.sock:/var/run/docker.sock --rm \\\n  -e INPUT_IMAGE="$YOUR_IMAGE_NAME" \\\n  -e INPUT_SIZE="$YOUR_SIZE_LIMIT" \\\n  wemakeservices/docker-image-size-limit\n```\n\n\n## Should I use it?\n\nYou can use this script instead:\n\n```bash\nLIMIT=1024  # adjust at your will\nIMAGE=\'your-image-name:latest\'\n\nSIZE="$(docker image inspect "$IMAGE" --format=\'{{.Size}}\')"\ntest "$SIZE" -gt "$LIMIT" && echo \'Limit exceeded\'; exit 1 || echo \'Ok!\'\n```\n\nBut I prefer to reuse tools over\ncustom `bash` scripts here and there.\n\n\n## License\n\nMIT.\n',
-    'author': 'Nikita Sobolev',
-    'author_email': 'mail@sobolevn.me',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/wemake-services/docker-image-size-limit',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.6,<4.0',
-}
+Limit your `docker` image size with a simple CLI command.
+Perfect to be used inside your CI process.
 
+Read the [announcing post](https://sobolevn.me/2019/03/announcing-docker-image-size-limit).
+
+
+## Installation
+
+```bash
+pip install docker-image-size-limit
+```
+
+Or use our [Github Action](https://github.com/wemake-services/docker-image-size-limit#github-action) or [pre-built docker image](https://github.com/wemake-services/docker-image-size-limit#docker-image).
+
+
+## Usage
+
+We support just a single command:
+
+```bash
+$ disl your-image-name:label 300MiB
+your-image-name:label exceeds 300MiB limit by 114.4 MiB
+```
+
+
+## Options
+
+You can specify your image as:
+
+- Image name: `python`
+- Image name with tag: `python:3.6.6-alpine`
+
+You can specify your size as:
+
+- Raw number of bytes: `1024`
+- Human-readable megabytes: `30 MB` or `30 MiB`
+- Human-readable gigabytes: `1 GB` or `1 GiB`
+- Any other size supported by [`humanfriendly`](https://humanfriendly.readthedocs.io/en/latest/api.html#humanfriendly.parse_size)
+
+
+## Programmatic usage
+
+You can also import and use this library as `python` code:
+
+```python
+from docker import from_env
+from docker_image_size_limit import check_image_size
+
+oversize = check_image_size(from_env(), 'image-name:latest', '1 GiB')
+assert oversize < 0, 'Too big image!'  # negative oversize - is a good thing!
+```
+
+We also ship [PEP-561](https://www.python.org/dev/peps/pep-0561/)
+compatible type annotations with this library.
+
+
+## Github Action
+
+You can also use this check as a [Gihub Action](https://github.com/marketplace/actions/docker-image-size-limit):
+
+```yaml
+- uses: wemake-services/docker-image-size-limit@master
+  with:
+    image: "$YOUR_IMAGE_NAME"
+    size: "$YOUR_SIZE_LIMIT"
+```
+
+Here's [an example](https://github.com/wemake-services/docker-image-size-limit/actions?query=workflow%3Adisl).
+
+
+## Docker Image
+
+We have a [pre-built image](https://hub.docker.com/r/wemakeservices/docker-image-size-limit) available.
+
+First, pull our pre-built docker image:
+
+```bash
+docker pull wemakeservices/docker-image-size-limit
+```
+
+Then you can use it like so:
+
+```bash
+docker run -v /var/run/docker.sock:/var/run/docker.sock --rm \
+  -e INPUT_IMAGE="$YOUR_IMAGE_NAME" \
+  -e INPUT_SIZE="$YOUR_SIZE_LIMIT" \
+  wemakeservices/docker-image-size-limit
+```
+
+
+## Should I use it?
+
+You can use this script instead:
+
+```bash
+LIMIT=1024  # adjust at your will
+IMAGE='your-image-name:latest'
+
+SIZE="$(docker image inspect "$IMAGE" --format='{{.Size}}')"
+test "$SIZE" -gt "$LIMIT" && echo 'Limit exceeded'; exit 1 || echo 'Ok!'
+```
+
+But I prefer to reuse tools over
+custom `bash` scripts here and there.
+
+
+## License
+
+MIT.
 
-setup(**setup_kwargs)
```

