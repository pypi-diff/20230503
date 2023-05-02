# Comparing `tmp/commonpy-1.9.4.tar.gz` & `tmp/commonpy-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonpy-1.9.4.tar", last modified: Fri Jun  3 20:52:03 2022, max compression
+gzip compressed data, was "commonpy-1.9.5.tar", last modified: Thu Jul  7 23:30:09 2022, max compression
```

## Comparing `commonpy-1.9.4.tar` & `commonpy-1.9.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2022-06-03 20:52:03.896288 commonpy-1.9.4/
--rw-r--r--   0 mhucka     (511) staff       (20)     1527 2022-01-11 00:45:56.000000 commonpy-1.9.4/LICENSE
--rw-r--r--   0 mhucka     (511) staff       (20)    16237 2022-06-03 20:52:03.896483 commonpy-1.9.4/PKG-INFO
--rw-r--r--   0 mhucka     (511) staff       (20)    15235 2022-06-03 20:51:03.000000 commonpy-1.9.4/README.md
-drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2022-06-03 20:52:03.894022 commonpy-1.9.4/commonpy/
--rw-r--r--   0 mhucka     (511) staff       (20)     1509 2022-06-03 20:50:25.000000 commonpy-1.9.4/commonpy/__init__.py
--rw-r--r--   0 mhucka     (511) staff       (20)     1790 2022-01-11 00:45:56.000000 commonpy-1.9.4/commonpy/data_structures.py
--rw-r--r--   0 mhucka     (511) staff       (20)     6351 2022-04-22 17:38:17.000000 commonpy-1.9.4/commonpy/data_utils.py
--rw-r--r--   0 mhucka     (511) staff       (20)     1697 2022-03-12 04:03:42.000000 commonpy-1.9.4/commonpy/exceptions.py
--rw-r--r--   0 mhucka     (511) staff       (20)     6694 2022-01-11 00:45:56.000000 commonpy-1.9.4/commonpy/file_utils.py
--rw-r--r--   0 mhucka     (511) staff       (20)     4691 2022-01-11 00:45:56.000000 commonpy-1.9.4/commonpy/interrupt.py
--rw-r--r--   0 mhucka     (511) staff       (20)     3140 2022-01-11 00:45:56.000000 commonpy-1.9.4/commonpy/module_utils.py
--rw-r--r--   0 mhucka     (511) staff       (20)    15750 2022-04-25 23:46:53.000000 commonpy-1.9.4/commonpy/network_utils.py
--rw-r--r--   0 mhucka     (511) staff       (20)     1875 2022-01-11 00:45:56.000000 commonpy-1.9.4/commonpy/string_utils.py
--rw-r--r--   0 mhucka     (511) staff       (20)     1303 2022-01-11 00:45:56.000000 commonpy-1.9.4/commonpy/system_utils.py
--rw-r--r--   0 mhucka     (511) staff       (20)      855 2021-09-29 02:27:31.000000 commonpy-1.9.4/commonpy/tmp.py
-drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2022-06-03 20:52:03.896016 commonpy-1.9.4/commonpy.egg-info/
--rw-r--r--   0 mhucka     (511) staff       (20)    16237 2022-06-03 20:52:03.000000 commonpy-1.9.4/commonpy.egg-info/PKG-INFO
--rw-r--r--   0 mhucka     (511) staff       (20)      483 2022-06-03 20:52:03.000000 commonpy-1.9.4/commonpy.egg-info/SOURCES.txt
--rw-r--r--   0 mhucka     (511) staff       (20)        1 2022-06-03 20:52:03.000000 commonpy-1.9.4/commonpy.egg-info/dependency_links.txt
--rw-r--r--   0 mhucka     (511) staff       (20)        1 2022-06-03 20:52:03.000000 commonpy-1.9.4/commonpy.egg-info/not-zip-safe
--rw-r--r--   0 mhucka     (511) staff       (20)      234 2022-06-03 20:52:03.000000 commonpy-1.9.4/commonpy.egg-info/requires.txt
--rw-r--r--   0 mhucka     (511) staff       (20)        9 2022-06-03 20:52:03.000000 commonpy-1.9.4/commonpy.egg-info/top_level.txt
--rw-r--r--   0 mhucka     (511) staff       (20)     1004 2022-06-03 20:52:03.897030 commonpy-1.9.4/setup.cfg
--rw-r--r--   0 mhucka     (511) staff       (20)      921 2021-06-07 22:50:51.000000 commonpy-1.9.4/setup.py
+drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2022-07-07 23:30:09.369850 commonpy-1.9.5/
+-rw-r--r--   0 mhucka     (511) staff       (20)     1527 2022-01-11 00:45:56.000000 commonpy-1.9.5/LICENSE
+-rw-r--r--   0 mhucka     (511) staff       (20)    16237 2022-07-07 23:30:09.369993 commonpy-1.9.5/PKG-INFO
+-rw-r--r--   0 mhucka     (511) staff       (20)    15235 2022-07-07 23:27:59.000000 commonpy-1.9.5/README.md
+drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2022-07-07 23:30:09.367999 commonpy-1.9.5/commonpy/
+-rw-r--r--   0 mhucka     (511) staff       (20)     1509 2022-07-07 23:27:17.000000 commonpy-1.9.5/commonpy/__init__.py
+-rw-r--r--   0 mhucka     (511) staff       (20)     1790 2022-01-11 00:45:56.000000 commonpy-1.9.5/commonpy/data_structures.py
+-rw-r--r--   0 mhucka     (511) staff       (20)     6351 2022-04-22 17:38:17.000000 commonpy-1.9.5/commonpy/data_utils.py
+-rw-r--r--   0 mhucka     (511) staff       (20)     1697 2022-03-12 04:03:42.000000 commonpy-1.9.5/commonpy/exceptions.py
+-rw-r--r--   0 mhucka     (511) staff       (20)     6694 2022-01-11 00:45:56.000000 commonpy-1.9.5/commonpy/file_utils.py
+-rw-r--r--   0 mhucka     (511) staff       (20)     4691 2022-01-11 00:45:56.000000 commonpy-1.9.5/commonpy/interrupt.py
+-rw-r--r--   0 mhucka     (511) staff       (20)     3140 2022-01-11 00:45:56.000000 commonpy-1.9.5/commonpy/module_utils.py
+-rw-r--r--   0 mhucka     (511) staff       (20)    15971 2022-07-06 00:07:48.000000 commonpy-1.9.5/commonpy/network_utils.py
+-rw-r--r--   0 mhucka     (511) staff       (20)     1875 2022-01-11 00:45:56.000000 commonpy-1.9.5/commonpy/string_utils.py
+-rw-r--r--   0 mhucka     (511) staff       (20)     1303 2022-01-11 00:45:56.000000 commonpy-1.9.5/commonpy/system_utils.py
+-rw-r--r--   0 mhucka     (511) staff       (20)      855 2021-09-29 02:27:31.000000 commonpy-1.9.5/commonpy/tmp.py
+drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2022-07-07 23:30:09.369644 commonpy-1.9.5/commonpy.egg-info/
+-rw-r--r--   0 mhucka     (511) staff       (20)    16237 2022-07-07 23:30:08.000000 commonpy-1.9.5/commonpy.egg-info/PKG-INFO
+-rw-r--r--   0 mhucka     (511) staff       (20)      483 2022-07-07 23:30:09.000000 commonpy-1.9.5/commonpy.egg-info/SOURCES.txt
+-rw-r--r--   0 mhucka     (511) staff       (20)        1 2022-07-07 23:30:08.000000 commonpy-1.9.5/commonpy.egg-info/dependency_links.txt
+-rw-r--r--   0 mhucka     (511) staff       (20)        1 2022-07-07 23:30:08.000000 commonpy-1.9.5/commonpy.egg-info/not-zip-safe
+-rw-r--r--   0 mhucka     (511) staff       (20)      721 2022-07-07 23:30:09.000000 commonpy-1.9.5/commonpy.egg-info/requires.txt
+-rw-r--r--   0 mhucka     (511) staff       (20)        9 2022-07-07 23:30:09.000000 commonpy-1.9.5/commonpy.egg-info/top_level.txt
+-rw-r--r--   0 mhucka     (511) staff       (20)     1004 2022-07-07 23:30:09.370482 commonpy-1.9.5/setup.cfg
+-rwxr-xr-x   0 mhucka     (511) staff       (20)     1801 2022-07-07 21:40:12.000000 commonpy-1.9.5/setup.py
```

### Comparing `commonpy-1.9.4/LICENSE` & `commonpy-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `commonpy-1.9.4/PKG-INFO` & `commonpy-1.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: commonpy
-Version: 1.9.4
+Version: 1.9.5
 Summary: Assortment of Python helper functions and utility classes
 Home-page: https://github.com/caltechlibrary/commonpy
 Author: Michael Hucka
 Author-email: mhucka@caltech.edu
 License: BSD 3-clause
 Project-URL: Source Code, https://github.com/caltechlibrary/commonpy
 Project-URL: Bug Tracker, https://github.com/caltechlibrary/commonpy/issues
 Keywords: Python,utilities
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 CommonPy<img width="12%" align="right" src="https://github.com/caltechlibrary/commonpy/raw/main/.graphics/commonpy-icon.png">
 ===============================================
 
 This is a collection of common utility functions and classes that we at the Caltech Library have found useful in our other Python projects.
 
 [![Latest release](https://img.shields.io/github/v/release/caltechlibrary/commonpy.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/caltechlibrary/commonpy/releases)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg?style=flat-square)](https://choosealicense.com/licenses/bsd-3-clause)
 [![Python](https://img.shields.io/badge/Python-3.6+-brightgreen.svg?style=flat-square)](http://shields.io)
-[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&style=flat-square&color=lightgray&query=$.metadata.doi&uri=https://data.caltech.edu/api/record/20184)](https://data.caltech.edu/records/20184)
+[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&style=flat-square&color=lightgray&query=$.metadata.doi&uri=https://data.caltech.edu/api/record/20217)](https://data.caltech.edu/records/20217)
 [![PyPI](https://img.shields.io/pypi/v/commonpy.svg?style=flat-square&color=orange)](https://pypi.org/project/commonpy/)
 
 Table of contents
 -----------------
 
 * [Introduction](#introduction)
 * [Installation](#installation)
@@ -290,9 +290,7 @@
 
 <div align="center">
   <br>
   <a href="https://www.caltech.edu">
     <img width="100" height="100" src="https://raw.githubusercontent.com/caltechlibrary/commonpy/main/.graphics/caltech-round.png">
   </a>
 </div>
-
-
```

### Comparing `commonpy-1.9.4/README.md` & `commonpy-1.9.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ===============================================
 
 This is a collection of common utility functions and classes that we at the Caltech Library have found useful in our other Python projects.
 
 [![Latest release](https://img.shields.io/github/v/release/caltechlibrary/commonpy.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/caltechlibrary/commonpy/releases)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg?style=flat-square)](https://choosealicense.com/licenses/bsd-3-clause)
 [![Python](https://img.shields.io/badge/Python-3.6+-brightgreen.svg?style=flat-square)](http://shields.io)
-[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&style=flat-square&color=lightgray&query=$.metadata.doi&uri=https://data.caltech.edu/api/record/20184)](https://data.caltech.edu/records/20184)
+[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&style=flat-square&color=lightgray&query=$.metadata.doi&uri=https://data.caltech.edu/api/record/20217)](https://data.caltech.edu/records/20217)
 [![PyPI](https://img.shields.io/pypi/v/commonpy.svg?style=flat-square&color=orange)](https://pypi.org/project/commonpy/)
 
 Table of contents
 -----------------
 
 * [Introduction](#introduction)
 * [Installation](#installation)
```

### Comparing `commonpy-1.9.4/commonpy/__init__.py` & `commonpy-1.9.5/commonpy/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # Package metadata ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 #
 #  ╭────────────────────── Notice ── Notice ── Notice ─────────────────────╮
 #  |    The following values are automatically updated at every release    |
 #  |    by the Makefile. Manual changes to these values will be lost.      |
 #  ╰────────────────────── Notice ── Notice ── Notice ─────────────────────╯
 
-__version__     = '1.9.4'
+__version__     = '1.9.5'
 __description__ = 'Assortment of Python helper functions and utility classes'
 __url__         = 'https://github.com/caltechlibrary/commonpy'
 __author__      = 'Michael Hucka'
 __email__       = 'mhucka@caltech.edu'
 __license__     = 'BSD 3-clause'
```

### Comparing `commonpy-1.9.4/commonpy/data_structures.py` & `commonpy-1.9.5/commonpy/data_structures.py`

 * *Files identical despite different names*

### Comparing `commonpy-1.9.4/commonpy/data_utils.py` & `commonpy-1.9.5/commonpy/data_utils.py`

 * *Files identical despite different names*

### Comparing `commonpy-1.9.4/commonpy/exceptions.py` & `commonpy-1.9.5/commonpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `commonpy-1.9.4/commonpy/file_utils.py` & `commonpy-1.9.5/commonpy/file_utils.py`

 * *Files identical despite different names*

### Comparing `commonpy-1.9.4/commonpy/interrupt.py` & `commonpy-1.9.5/commonpy/interrupt.py`

 * *Files identical despite different names*

### Comparing `commonpy-1.9.4/commonpy/module_utils.py` & `commonpy-1.9.5/commonpy/module_utils.py`

 * *Files identical despite different names*

### Comparing `commonpy-1.9.4/commonpy/network_utils.py` & `commonpy-1.9.5/commonpy/network_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -236,68 +236,73 @@
     underlying Python HTTPX library network calls.
     '''
     known_methods = ['get', 'post', 'head', 'options', 'put', 'delete', 'patch']
     if method.lower() not in known_methods:
         raise ValueError(f'HTTP method "{method}" is not'
                          f' one of {", ".join(known_methods)}.')
 
-    def addurl(text):
-        return f'{text} for {url}'
+    def info(text, details = ''):
+        msg = f'{text} for {url}'
+        if details:
+            msg += (' (' + details + ')')
+        return msg
 
     resp = None
     try:
         resp = timed_request(method, url, client, follow_redirects = True, **kwargs)
     except (httpx.NetworkError, httpx.ProtocolError) as ex:
         # timed_request() will have retried, so if we get here, time to bail.
-        if __debug__: log(addurl(f'got network exception: {antiformat(ex)}'))
+        if __debug__: log(info(f'network exception: {antiformat(ex)}'))
         is_on_localhost = on_localhost(url)
-        msg = antiformat(ex)
+        reason = antiformat(ex)
         if isinstance(ex, httpx.ConnectError) and is_on_localhost:
-            if __debug__: log(addurl('returning ServiceFailure'))
-            return (resp, ServiceFailure(addurl(f'Access failure ({msg})')))
+            if __debug__: log(info('returning ServiceFailure'))
+            return (resp, ServiceFailure(info(f'Access failure ({reason})')))
         elif is_on_localhost or network_available():
-            if __debug__: log(addurl('returning ServiceFailure'))
-            return (resp, ServiceFailure(addurl(f'Server error ({msg})')))
+            if __debug__: log(info('returning ServiceFailure'))
+            return (resp, ServiceFailure(info(f'Server error ({reason})')))
         else:
-            if __debug__: log(addurl('returning NetworkFailure'))
-            return (resp, NetworkFailure(addurl('Network failure ({msg})')))
+            if __debug__: log(info('returning NetworkFailure'))
+            return (resp, NetworkFailure(info('Network failure ({reason})')))
     except Exception as ex:
         # Not a network or protocol error, and not a normal server response.
-        if __debug__: log(addurl(f'returning exception: {antiformat(ex)}'))
+        if __debug__: log(info(f'returning exception: {antiformat(ex)}'))
         return (resp, ex)
 
     # Interpret the response.  Note that the requests library handles code 301
     # and 302 redirects automatically, so we don't need to do it here.
     error = None
     code = resp.status_code
     reason = resp.reason_phrase
+    text = resp.text                    # Sometimes this holds more details.
     if code == 400:
-        error = ServiceFailure(addurl('Server rejected the request'))
+        error = ServiceFailure(info('Server rejected the request', text))
     elif code in [401, 402, 403, 407, 451, 511]:
-        error = AuthenticationFailure(addurl('Access is forbidden'))
+        error = AuthenticationFailure(info('Access is forbidden', text))
     elif code in [404, 410] and not polling:
-        error = NoContent(addurl("No content found"))
+        error = NoContent(info("No content found", text))
     elif code in [405, 406, 409, 411, 412, 413, 414, 417, 428, 431, 505, 510]:
-        error = InternalError(addurl(f'Server returned code {code} ({reason})'))
+        error = InternalError(info(f'Server returned code {code} ({reason})', text))
     elif code in [415, 416]:
-        error = ServiceFailure(addurl(f'Server rejected the request ({reason})'))
+        error = ServiceFailure(info(f'Server rejected the request ({reason})', text))
     elif code == 429:
         if handle_rate and recursing < _MAX_RECURSIVE_CALLS:
             pause = 5 * (recursing + 1)   # +1 b/c we start with recursing = 0.
-            if __debug__: log(addurl('rate limit hit -- pausing'))
+            if __debug__: log(info('rate limit hit -- pausing', text))
             wait(pause)                   # 5 s, then 10 s, then 15 s, etc.
-            if __debug__: log(addurl(f'doing recursive call #{recursing + 1}'))
+            if __debug__: log(info(f'doing recursive call #{recursing + 1}', text))
             return net(method, url, client, handle_rate, polling, recursing + 1, **kwargs)
-        error = RateLimitExceeded(addurl('Server blocking requests due to rate limits'))
+        error = RateLimitExceeded(info('Server blocking requests due to rate limits', text))
     elif code in [500, 501, 502, 503, 504, 506, 507, 508]:
-        error = ServiceFailure(addurl(f'Server error (code {code} -- {reason})'))
+        error = ServiceFailure(info(f'Server error (code {code} -- {reason})', text))
     elif not (200 <= code < 400):
-        error = NetworkFailure(addurl(f'Unable to resolve {url}'))
+        error = NetworkFailure(info(f'Unable to resolve {url}', text))
     # The error msg will have had the URL added already; no need to do it here.
-    if __debug__: log('returning {}'.format(f'{error}' if error else f'response for {url}'))
+    if __debug__: log('returning {}'.format(
+            f'error: {error}' if error else f'response for {url}'))
     return (resp, error)
 
 
 def download_file(url, local_destination):
     '''Returns True if the content at 'url' could be downloaded to the file
     'local_destination', and False otherwise. It does not throw an exception.'''
```

### Comparing `commonpy-1.9.4/commonpy/string_utils.py` & `commonpy-1.9.5/commonpy/string_utils.py`

 * *Files identical despite different names*

### Comparing `commonpy-1.9.4/commonpy/system_utils.py` & `commonpy-1.9.5/commonpy/system_utils.py`

 * *Files identical despite different names*

### Comparing `commonpy-1.9.4/commonpy/tmp.py` & `commonpy-1.9.5/commonpy/tmp.py`

 * *Files identical despite different names*

### Comparing `commonpy-1.9.4/commonpy.egg-info/PKG-INFO` & `commonpy-1.9.5/commonpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: commonpy
-Version: 1.9.4
+Version: 1.9.5
 Summary: Assortment of Python helper functions and utility classes
 Home-page: https://github.com/caltechlibrary/commonpy
 Author: Michael Hucka
 Author-email: mhucka@caltech.edu
 License: BSD 3-clause
 Project-URL: Source Code, https://github.com/caltechlibrary/commonpy
 Project-URL: Bug Tracker, https://github.com/caltechlibrary/commonpy/issues
 Keywords: Python,utilities
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 CommonPy<img width="12%" align="right" src="https://github.com/caltechlibrary/commonpy/raw/main/.graphics/commonpy-icon.png">
 ===============================================
 
 This is a collection of common utility functions and classes that we at the Caltech Library have found useful in our other Python projects.
 
 [![Latest release](https://img.shields.io/github/v/release/caltechlibrary/commonpy.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/caltechlibrary/commonpy/releases)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg?style=flat-square)](https://choosealicense.com/licenses/bsd-3-clause)
 [![Python](https://img.shields.io/badge/Python-3.6+-brightgreen.svg?style=flat-square)](http://shields.io)
-[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&style=flat-square&color=lightgray&query=$.metadata.doi&uri=https://data.caltech.edu/api/record/20184)](https://data.caltech.edu/records/20184)
+[![DOI](https://img.shields.io/badge/dynamic/json.svg?label=DOI&style=flat-square&color=lightgray&query=$.metadata.doi&uri=https://data.caltech.edu/api/record/20217)](https://data.caltech.edu/records/20217)
 [![PyPI](https://img.shields.io/pypi/v/commonpy.svg?style=flat-square&color=orange)](https://pypi.org/project/commonpy/)
 
 Table of contents
 -----------------
 
 * [Introduction](#introduction)
 * [Installation](#installation)
@@ -290,9 +290,7 @@
 
 <div align="center">
   <br>
   <a href="https://www.caltech.edu">
     <img width="100" height="100" src="https://raw.githubusercontent.com/caltechlibrary/commonpy/main/.graphics/caltech-round.png">
   </a>
 </div>
-
-
```

### Comparing `commonpy-1.9.4/setup.cfg` & `commonpy-1.9.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = commonpy
-version = 1.9.4
+version = 1.9.5
 description = Assortment of Python helper functions and utility classes
 author = Michael Hucka
 author_email = mhucka@caltech.edu
 license = BSD 3-clause
 license_files = LICENSE
 url = https://github.com/caltechlibrary/commonpy
 project_urls =
```

