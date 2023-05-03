# Comparing `tmp/chromedriver-binary-auto-0.2.5.tar.gz` & `tmp/chromedriver-binary-auto-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromedriver-binary-auto-0.2.5.tar", last modified: Fri Mar 17 08:24:18 2023, max compression
+gzip compressed data, was "chromedriver-binary-auto-0.2.6.tar", last modified: Wed May  3 13:04:54 2023, max compression
```

## Comparing `chromedriver-binary-auto-0.2.5.tar` & `chromedriver-binary-auto-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 08:24:18.324079 chromedriver-binary-auto-0.2.5/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-03-17 08:24:17.000000 chromedriver-binary-auto-0.2.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2722 2023-03-17 08:24:18.324079 chromedriver-binary-auto-0.2.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2070 2023-03-17 08:24:17.000000 chromedriver-binary-auto-0.2.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 08:24:18.324079 chromedriver-binary-auto-0.2.5/chromedriver_binary/
--rw-rw-rw-   0 root         (0) root         (0)      743 2023-03-17 08:24:17.000000 chromedriver-binary-auto-0.2.5/chromedriver_binary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4590 2023-03-17 08:24:17.000000 chromedriver-binary-auto-0.2.5/chromedriver_binary/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 08:24:18.324079 chromedriver-binary-auto-0.2.5/chromedriver_binary_auto.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2722 2023-03-17 08:24:18.000000 chromedriver-binary-auto-0.2.5/chromedriver_binary_auto.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      330 2023-03-17 08:24:18.000000 chromedriver-binary-auto-0.2.5/chromedriver_binary_auto.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-17 08:24:18.000000 chromedriver-binary-auto-0.2.5/chromedriver_binary_auto.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-03-17 08:24:18.000000 chromedriver-binary-auto-0.2.5/chromedriver_binary_auto.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-03-17 08:24:18.000000 chromedriver-binary-auto-0.2.5/chromedriver_binary_auto.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-17 08:24:18.324079 chromedriver-binary-auto-0.2.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3906 2023-03-17 08:24:17.000000 chromedriver-binary-auto-0.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:04:54.351110 chromedriver-binary-auto-0.2.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-05-03 13:04:53.000000 chromedriver-binary-auto-0.2.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2722 2023-05-03 13:04:54.351110 chromedriver-binary-auto-0.2.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2070 2023-05-03 13:04:53.000000 chromedriver-binary-auto-0.2.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:04:54.351110 chromedriver-binary-auto-0.2.6/chromedriver_binary/
+-rw-rw-rw-   0 root         (0) root         (0)      743 2023-05-03 13:04:53.000000 chromedriver-binary-auto-0.2.6/chromedriver_binary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4602 2023-05-03 13:04:53.000000 chromedriver-binary-auto-0.2.6/chromedriver_binary/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:04:54.351110 chromedriver-binary-auto-0.2.6/chromedriver_binary_auto.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2722 2023-05-03 13:04:54.000000 chromedriver-binary-auto-0.2.6/chromedriver_binary_auto.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      330 2023-05-03 13:04:54.000000 chromedriver-binary-auto-0.2.6/chromedriver_binary_auto.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 13:04:54.000000 chromedriver-binary-auto-0.2.6/chromedriver_binary_auto.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-03 13:04:54.000000 chromedriver-binary-auto-0.2.6/chromedriver_binary_auto.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-03 13:04:54.000000 chromedriver-binary-auto-0.2.6/chromedriver_binary_auto.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 13:04:54.351110 chromedriver-binary-auto-0.2.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3918 2023-05-03 13:04:53.000000 chromedriver-binary-auto-0.2.6/setup.py
```

### Comparing `chromedriver-binary-auto-0.2.5/LICENSE` & `chromedriver-binary-auto-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chromedriver-binary-auto-0.2.5/PKG-INFO` & `chromedriver-binary-auto-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromedriver-binary-auto
-Version: 0.2.5
+Version: 0.2.6
 Summary: Installer for chromedriver.
 Home-page: https://github.com/danielkaiser/python-chromedriver-binary
 Author: Daniel Kaiser
 Author-email: daniel.kaiser94@gmail.com
 License: MIT
 Keywords: chromedriver chrome browser selenium splinter
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `chromedriver-binary-auto-0.2.5/README.md` & `chromedriver-binary-auto-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `chromedriver-binary-auto-0.2.5/chromedriver_binary/__init__.py` & `chromedriver-binary-auto-0.2.6/chromedriver_binary/__init__.py`

 * *Files identical despite different names*

### Comparing `chromedriver-binary-auto-0.2.5/chromedriver_binary/utils.py` & `chromedriver-binary-auto-0.2.6/chromedriver_binary/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import ssl
 import subprocess
 import re
 import platform
 
 try:
     from urllib.request import urlopen, URLError
-    ssl_context = ssl.SSLContext()
+    ssl_context = ssl.create_default_context()
 except ImportError:
     from urllib2 import urlopen, URLError
     ssl_context = ssl.SSLContext(protocol=ssl.PROTOCOL_TLS)
 
 __author__ = 'Daniel Kaiser <d.kasier@fz-juelich.de>'
```

### Comparing `chromedriver-binary-auto-0.2.5/chromedriver_binary_auto.egg-info/PKG-INFO` & `chromedriver-binary-auto-0.2.6/chromedriver_binary_auto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromedriver-binary-auto
-Version: 0.2.5
+Version: 0.2.6
 Summary: Installer for chromedriver.
 Home-page: https://github.com/danielkaiser/python-chromedriver-binary
 Author: Daniel Kaiser
 Author-email: daniel.kaiser94@gmail.com
 License: MIT
 Keywords: chromedriver chrome browser selenium splinter
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `chromedriver-binary-auto-0.2.5/setup.py` & `chromedriver-binary-auto-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import ssl
 import zipfile
 
 try:
     from io import BytesIO
     from urllib.request import urlopen, URLError
-    ssl_context = ssl.SSLContext()
+    ssl_context = ssl.create_default_context()
 except ImportError:
     from StringIO import StringIO as BytesIO
     from urllib2 import urlopen, URLError
     ssl_context = ssl.SSLContext(protocol=ssl.PROTOCOL_TLS)
 
 __author__ = 'Daniel Kaiser <d.kasier@fz-juelich.de>'
 
@@ -59,15 +59,15 @@
             if not os.access(chromedriver_filename, os.X_OK):
                 os.chmod(chromedriver_filename, 0o744)
         build_py.run(self)
 
 
 setup(
     name="chromedriver-binary-auto",
-    version="0.2.5",
+    version="0.2.6",
     author="Daniel Kaiser",
     author_email="daniel.kaiser94@gmail.com",
     description="Installer for chromedriver.",
     license="MIT",
     keywords="chromedriver chrome browser selenium splinter",
     url="https://github.com/danielkaiser/python-chromedriver-binary",
     packages=['chromedriver_binary'],
```

