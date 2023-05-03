# Comparing `tmp/actionlint_py-1.6.22.2.tar.gz` & `tmp/actionlint_py-1.6.24.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actionlint_py-1.6.22.2.tar", last modified: Mon Jan 16 12:14:26 2023, max compression
+gzip compressed data, was "actionlint_py-1.6.24.2.tar", last modified: Wed May  3 17:38:33 2023, max compression
```

## Comparing `actionlint_py-1.6.22.2.tar` & `actionlint_py-1.6.24.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-01-16 12:14:26.449447 actionlint_py-1.6.22.2/
--rw-rw-rw-   0        0        0     1087 2023-01-13 10:03:39.000000 actionlint_py-1.6.22.2/LICENSE
--rw-rw-rw-   0        0        0     1430 2023-01-16 12:14:26.449447 actionlint_py-1.6.22.2/PKG-INFO
--rw-rw-rw-   0        0        0      729 2023-01-13 11:48:18.000000 actionlint_py-1.6.22.2/README.md
-drwxrwxrwx   0        0        0        0 2023-01-16 12:14:26.448354 actionlint_py-1.6.22.2/actionlint_py.egg-info/
--rw-rw-rw-   0        0        0     1430 2023-01-16 12:14:26.000000 actionlint_py-1.6.22.2/actionlint_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2023-01-16 12:14:26.000000 actionlint_py-1.6.22.2/actionlint_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-16 12:14:26.000000 actionlint_py-1.6.22.2/actionlint_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-01-16 12:14:26.000000 actionlint_py-1.6.22.2/actionlint_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      735 2023-01-16 12:14:26.451353 actionlint_py-1.6.22.2/setup.cfg
--rw-rw-rw-   0        0        0     5164 2023-01-16 12:13:02.000000 actionlint_py-1.6.22.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 17:38:33.453090 actionlint_py-1.6.24.2/
+-rw-rw-rw-   0        0        0     1087 2023-05-03 15:51:52.000000 actionlint_py-1.6.24.2/LICENSE
+-rw-rw-rw-   0        0        0     1958 2023-05-03 17:38:33.453090 actionlint_py-1.6.24.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1257 2023-05-03 16:11:35.000000 actionlint_py-1.6.24.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 17:38:33.453090 actionlint_py-1.6.24.2/actionlint_py.egg-info/
+-rw-rw-rw-   0        0        0     1958 2023-05-03 17:38:33.000000 actionlint_py-1.6.24.2/actionlint_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2023-05-03 17:38:33.000000 actionlint_py-1.6.24.2/actionlint_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 17:38:33.000000 actionlint_py-1.6.24.2/actionlint_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-03 17:38:33.000000 actionlint_py-1.6.24.2/actionlint_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1737 2023-05-03 17:38:33.453090 actionlint_py-1.6.24.2/setup.cfg
+-rw-rw-rw-   0        0        0     5099 2023-05-03 17:13:49.000000 actionlint_py-1.6.24.2/setup.py
```

### Comparing `actionlint_py-1.6.22.2/LICENSE` & `actionlint_py-1.6.24.2/LICENSE`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.6.22.2/PKG-INFO` & `actionlint_py-1.6.24.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: actionlint_py
-Version: 1.6.22.2
-Summary: Python wrapper around invoking actionlint (https://github.com/rhysd/actionlint)
-Home-page: https://github.com/Mateusz-Grzelinski/actionlint-py
-Author: Ryan Rhee, Mateusz Grzeliński
-Author-email: grzelinskimat@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # actionlint-py
 
 A python wrapper to provide a pip-installable [actionlint] binary.
 
 Internally this package provides a convenient way to download the pre-built
 actionlint binary for your particular platform.
 
@@ -42,9 +25,26 @@
 ```yaml
 - repo: https://github.com/Mateusz-Grzelinski/actionlint-py
   rev: v1.6.22
   hooks:
   - id: actionlint
 ```
 
+or to avoid going twice to internet (might help with proxy):
+
+```yaml
+- repo: local
+  hooks:
+    - id: actionlint
+      name: actionlint
+      description: Test yaml scripts with actionlint
+#      additional_dependencies: [actionlint-py==1.6.22.2] # safer, but pre-commit autoupdate will not work
+      additional_dependencies: [actionlint-py]
+      entry: actionlint
+#      args: [-ignore "*.set-output. was depracated.*"]
+      language: python
+      types: [ "yaml" ]
+      files: "^.github/workflows/"
+```
+
 [actionlint]: https://github.com/rhysd/actionlint
 [pre-commit]: https://pre-commit.com
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `actionlint_py-1.6.22.2/actionlint_py.egg-info/PKG-INFO` & `actionlint_py-1.6.24.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: actionlint-py
-Version: 1.6.22.2
+Name: actionlint_py
+Version: 1.6.24.2
 Summary: Python wrapper around invoking actionlint (https://github.com/rhysd/actionlint)
 Home-page: https://github.com/Mateusz-Grzelinski/actionlint-py
 Author: Ryan Rhee, Mateusz Grzeliński
 Author-email: grzelinskimat@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -42,9 +42,26 @@
 ```yaml
 - repo: https://github.com/Mateusz-Grzelinski/actionlint-py
   rev: v1.6.22
   hooks:
   - id: actionlint
 ```
 
+or to avoid going twice to internet (might help with proxy):
+
+```yaml
+- repo: local
+  hooks:
+    - id: actionlint
+      name: actionlint
+      description: Test yaml scripts with actionlint
+#      additional_dependencies: [actionlint-py==1.6.22.2] # safer, but pre-commit autoupdate will not work
+      additional_dependencies: [actionlint-py]
+      entry: actionlint
+#      args: [-ignore "*.set-output. was depracated.*"]
+      language: python
+      types: [ "yaml" ]
+      files: "^.github/workflows/"
+```
+
 [actionlint]: https://github.com/rhysd/actionlint
 [pre-commit]: https://pre-commit.com
```

### Comparing `actionlint_py-1.6.22.2/setup.py` & `actionlint_py-1.6.24.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
+import configparser
 import hashlib
 import http
 import io
 import os.path
 import platform
 import stat
 import sys
@@ -13,37 +14,34 @@
 import zipfile
 
 from distutils.command.build import build as orig_build
 from distutils.core import Command
 from setuptools import setup
 from setuptools.command.install import install as orig_install
 
-ACTIONLINT_VERSION = '1.6.22'
+conf = configparser.ConfigParser()
+conf.read('./setup.cfg')
+
+# with open("setup.cfg") as configfile:
+
+ACTIONLINT_VERSION = conf['files-to-download']['tag']
 POSTFIX_SHA256 = {
-    ('linux', 'x86_64'): (
-        '_linux_amd64.tar.gz',
-        '7d7a3061b59718728788e75e6a177c621a31a683ffd21fedeabc1296fc2ee289',
-    ),
-    ('darwin', 'x86_64'): (
-        '_darwin_amd64.tar.gz',
-        '6a1a522521e2fa0351328c439a63fc1c51611d45fc8156af15ad8690165f27c3',
-    ),
-    ('win32', 'AMD64'): (
-        '_windows_amd64.zip',
-        'c0007e418e6cd2008769e55666229b50677f85975676c4246baee5ec3ae9a2b5',
-    ),
+    ('linux', 'x86_64'): '_linux_amd64.tar.gz',
+    ('darwin', 'x86_64'): '_darwin_amd64.tar.gz',
+    ('win32', 'AMD64'): '_windows_amd64.zip',
 }
 POSTFIX_SHA256[('cygwin', 'x86_64')] = POSTFIX_SHA256[('win32', 'AMD64')]
 POSTFIX_SHA256[('darwin', 'x86_64')] = POSTFIX_SHA256[('darwin', 'x86_64')]
 POSTFIX_SHA256[('linux', 'x86_64')] = POSTFIX_SHA256[('linux', 'x86_64')]
 PY_VERSION = '2'
 
 
 def get_download_url() -> tuple[str, str]:
-    postfix, sha256 = POSTFIX_SHA256[(sys.platform, platform.machine())]
+    postfix = POSTFIX_SHA256[(sys.platform, platform.machine())]
+    sha256 = conf['files-to-download'][postfix]
     url = (
         f'https://github.com/rhysd/actionlint/releases/download/'
         f'v{ACTIONLINT_VERSION}/actionlint_{ACTIONLINT_VERSION}{postfix}'
     )
     return url, sha256
 
 
@@ -158,11 +156,11 @@
             self.root_is_pure = False
 
         def get_tag(self):
             _, _, plat = orig_bdist_wheel.get_tag(self)
             # We don't contain any python source, nor any python extensions
             return 'py2.py3', 'none', plat
 
-
     command_overrides['bdist_wheel'] = bdist_wheel
 
-setup(version=f'{ACTIONLINT_VERSION}.{PY_VERSION}', cmdclass=command_overrides)
+if __name__ == '__main__':
+    setup(version=f'{ACTIONLINT_VERSION}.{PY_VERSION}', cmdclass=command_overrides)
```

