# Comparing `tmp/embody_codec-1.0.8.tar.gz` & `tmp/embody_codec-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embody_codec-1.0.8.tar", max compression
+gzip compressed data, was "embody_codec-1.0.9.tar", max compression
```

## Comparing `embody_codec-1.0.8.tar` & `embody_codec-1.0.9.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1061 2022-11-04 13:24:02.091874 embody_codec-1.0.8/LICENSE
--rw-r--r--   0        0        0     2210 2022-11-04 13:24:15.392094 embody_codec-1.0.8/README.md
--rw-r--r--   0        0        0     1844 2022-11-04 13:24:15.392094 embody_codec-1.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-04 13:24:02.091874 embody_codec-1.0.8/src/embodycodec/__init__.py
--rw-r--r--   0        0        0    12794 2022-11-04 13:24:02.091874 embody_codec-1.0.8/src/embodycodec/attributes.py
--rw-r--r--   0        0        0    22291 2022-11-04 13:24:02.091874 embody_codec-1.0.8/src/embodycodec/codec.py
--rw-r--r--   0        0        0      412 2022-11-04 13:24:02.091874 embody_codec-1.0.8/src/embodycodec/crc.py
--rw-r--r--   0        0        0        0 2022-11-04 13:24:02.091874 embody_codec-1.0.8/src/embodycodec/py.typed
--rw-r--r--   0        0        0     7577 2022-11-04 13:24:02.091874 embody_codec-1.0.8/src/embodycodec/types.py
--rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 embody_codec-1.0.8/setup.py
--rw-r--r--   0        0        0     3071 1970-01-01 00:00:00.000000 embody_codec-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2022-11-09 18:40:38.742023 embody_codec-1.0.9/LICENSE
+-rw-r--r--   0        0        0     2210 2022-11-09 18:40:38.742023 embody_codec-1.0.9/README.md
+-rw-r--r--   0        0        0     1844 2022-11-09 18:40:52.182185 embody_codec-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-09 18:40:38.742023 embody_codec-1.0.9/src/embodycodec/__init__.py
+-rw-r--r--   0        0        0    12794 2022-11-09 18:40:38.742023 embody_codec-1.0.9/src/embodycodec/attributes.py
+-rw-r--r--   0        0        0    22291 2022-11-09 18:40:38.742023 embody_codec-1.0.9/src/embodycodec/codec.py
+-rw-r--r--   0        0        0      412 2022-11-09 18:40:38.742023 embody_codec-1.0.9/src/embodycodec/crc.py
+-rw-r--r--   0        0        0    10302 2022-11-09 18:40:52.182185 embody_codec-1.0.9/src/embodycodec/file_codec.py
+-rw-r--r--   0        0        0        0 2022-11-09 18:40:38.742023 embody_codec-1.0.9/src/embodycodec/py.typed
+-rw-r--r--   0        0        0     7577 2022-11-09 18:40:38.742023 embody_codec-1.0.9/src/embodycodec/types.py
+-rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 embody_codec-1.0.9/setup.py
+-rw-r--r--   0        0        0     3071 1970-01-01 00:00:00.000000 embody_codec-1.0.9/PKG-INFO
```

### Comparing `embody_codec-1.0.8/LICENSE` & `embody_codec-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `embody_codec-1.0.8/README.md` & `embody_codec-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `embody_codec-1.0.8/pyproject.toml` & `embody_codec-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "embody-codec"
-version = "1.0.8"
+version = "1.0.9"
 description = "Embody Protocol Codec"
 authors = ["Aidee Health AS <hello@aidee.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/aidee-health/embody-protocol-codec"
 repository = "https://github.com/aidee-health/embody-protocol-codec"
 packages = [
```

### Comparing `embody_codec-1.0.8/src/embodycodec/attributes.py` & `embody_codec-1.0.9/src/embodycodec/attributes.py`

 * *Files identical despite different names*

### Comparing `embody_codec-1.0.8/src/embodycodec/codec.py` & `embody_codec-1.0.9/src/embodycodec/codec.py`

 * *Files identical despite different names*

### Comparing `embody_codec-1.0.8/src/embodycodec/types.py` & `embody_codec-1.0.9/src/embodycodec/types.py`

 * *Files identical despite different names*

### Comparing `embody_codec-1.0.8/setup.py` & `embody_codec-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['embodycodec']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'embody-codec',
-    'version': '1.0.8',
+    'version': '1.0.9',
     'description': 'Embody Protocol Codec',
     'long_description': "# EmBody protocol codec\n\n[![PyPI](https://img.shields.io/pypi/v/embody-codec.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/embody-codec.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/embody-codec)][python version]\n[![License](https://img.shields.io/pypi/l/embody-codec)][license]\n\n[![Tests](https://github.com/aidee-health/embody-codec/workflows/Tests/badge.svg)][tests]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/embody-codec/\n[status]: https://pypi.org/project/embody-codec/\n[python version]: https://pypi.org/project/embody-codec\n[tests]: https://github.com/aidee-health/embody-codec/actions?workflow=Tests\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\nThis is a Python based implementation library for the Aidee EmBody communication protocol.\n\n## Features\n\n- Encode protocol messages to binary data (bytes)\n- Decode binary data to protocol messages\n- Accessory code\n\n## Requirements\n\n- This library does not require any external libraries\n- Requires Python 3.7+\n\n# Installing package with pip from github\n\nYou can install _embody codec_ via [pip] from [PyPI]:\n\n```console\npip install embody-codec\n```\n\n## Contributing\n\nContributions are very welcome. To learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license].\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/espenwest/hypermodern-python/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/aidee-health/embody-codec/blob/main/LICENSE\n[contributor guide]: https://github.com/aidee-health/embody-codec/blob/main/CONTRIBUTING.md\n",
     'author': 'Aidee Health AS',
     'author_email': 'hello@aidee.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/aidee-health/embody-protocol-codec',
```

### Comparing `embody_codec-1.0.8/PKG-INFO` & `embody_codec-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embody-codec
-Version: 1.0.8
+Version: 1.0.9
 Summary: Embody Protocol Codec
 Home-page: https://github.com/aidee-health/embody-protocol-codec
 License: MIT
 Author: Aidee Health AS
 Author-email: hello@aidee.io
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

