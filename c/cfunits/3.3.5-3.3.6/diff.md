# Comparing `tmp/cfunits-3.3.5.tar.gz` & `tmp/cfunits-3.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfunits-3.3.5.tar", last modified: Thu Sep 22 15:31:49 2022, max compression
+gzip compressed data, was "cfunits-3.3.6.tar", last modified: Wed May  3 10:52:46 2023, max compression
```

## Comparing `cfunits-3.3.5.tar` & `cfunits-3.3.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-09-22 15:31:49.826167 cfunits-3.3.5/
--rw-rw-r--   0 david     (1000) david     (1000)     1065 2022-08-01 08:33:36.000000 cfunits-3.3.5/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)      333 2022-08-01 08:33:36.000000 cfunits-3.3.5/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)     2163 2022-09-22 15:31:49.826167 cfunits-3.3.5/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     2124 2022-08-01 08:33:36.000000 cfunits-3.3.5/README.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-09-22 15:31:49.826167 cfunits-3.3.5/cfunits/
--rw-rw-r--   0 david     (1000) david     (1000)     1360 2022-09-22 15:23:31.000000 cfunits-3.3.5/cfunits/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-09-22 15:31:49.822167 cfunits-3.3.5/cfunits/etc/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-09-22 15:31:49.826167 cfunits-3.3.5/cfunits/etc/udunits/
--rw-rw-r--   0 david     (1000) david     (1000)      301 2022-08-01 08:33:36.000000 cfunits-3.3.5/cfunits/etc/udunits/README
--rw-rw-r--   0 david     (1000) david     (1000)     7100 2022-08-01 08:33:36.000000 cfunits-3.3.5/cfunits/etc/udunits/udunits2-accepted.xml
--rw-rw-r--   0 david     (1000) david     (1000)     6994 2022-08-01 08:33:36.000000 cfunits-3.3.5/cfunits/etc/udunits/udunits2-accepted.xml.nonCF
--rw-rw-r--   0 david     (1000) david     (1000)     3170 2022-08-01 08:33:36.000000 cfunits-3.3.5/cfunits/etc/udunits/udunits2-base.xml
--rw-rw-r--   0 david     (1000) david     (1000)    55074 2022-08-01 08:33:36.000000 cfunits-3.3.5/cfunits/etc/udunits/udunits2-common.xml
--rw-rw-r--   0 david     (1000) david     (1000)    53091 2022-08-01 08:33:36.000000 cfunits-3.3.5/cfunits/etc/udunits/udunits2-common.xml.nonCF
--rw-rw-r--   0 david     (1000) david     (1000)     4034 2022-08-01 08:33:36.000000 cfunits-3.3.5/cfunits/etc/udunits/udunits2-derived.xml
--rw-rw-r--   0 david     (1000) david     (1000)     3915 2022-08-01 08:33:36.000000 cfunits-3.3.5/cfunits/etc/udunits/udunits2-derived.xml.nonCF
--rw-rw-r--   0 david     (1000) david     (1000)     2308 2022-08-01 08:33:36.000000 cfunits-3.3.5/cfunits/etc/udunits/udunits2-prefixes.xml
--rw-rw-r--   0 david     (1000) david     (1000)      517 2022-08-01 08:33:36.000000 cfunits-3.3.5/cfunits/etc/udunits/udunits2.xml
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-09-22 15:31:49.826167 cfunits-3.3.5/cfunits/test/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2022-08-01 08:33:36.000000 cfunits-3.3.5/cfunits/test/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     2596 2022-08-01 08:33:36.000000 cfunits-3.3.5/cfunits/test/run_tests.py
--rwxrwxr-x   0 david     (1000) david     (1000)     2083 2022-08-01 08:33:36.000000 cfunits-3.3.5/cfunits/test/run_tests_and_coverage
--rw-rw-r--   0 david     (1000) david     (1000)    15578 2022-09-22 07:57:25.000000 cfunits-3.3.5/cfunits/test/test_Units.py
--rw-rw-r--   0 david     (1000) david     (1000)     2117 2022-08-01 08:33:36.000000 cfunits-3.3.5/cfunits/test/test_style.py
--rw-rw-r--   0 david     (1000) david     (1000)    82912 2022-09-22 11:03:36.000000 cfunits-3.3.5/cfunits/units.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-09-22 15:31:49.826167 cfunits-3.3.5/cfunits.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     2163 2022-09-22 15:31:49.000000 cfunits-3.3.5/cfunits.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      806 2022-09-22 15:31:49.000000 cfunits-3.3.5/cfunits.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2022-09-22 15:31:49.000000 cfunits-3.3.5/cfunits.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)      243 2022-09-22 15:31:49.000000 cfunits-3.3.5/cfunits.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)        8 2022-09-22 15:31:49.000000 cfunits-3.3.5/cfunits.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)      433 2022-08-01 08:33:37.000000 cfunits-3.3.5/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)       42 2022-09-22 15:21:51.000000 cfunits-3.3.5/requirements.txt
--rw-rw-r--   0 david     (1000) david     (1000)       38 2022-09-22 15:31:49.826167 cfunits-3.3.5/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)     4222 2022-08-01 08:33:37.000000 cfunits-3.3.5/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 10:52:46.394537 cfunits-3.3.6/
+-rw-rw-r--   0 david     (1000) david     (1000)     1065 2022-08-01 08:33:36.000000 cfunits-3.3.6/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)      333 2022-08-01 08:33:36.000000 cfunits-3.3.6/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)     2161 2023-05-03 10:52:46.394537 cfunits-3.3.6/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     2122 2022-10-07 10:16:20.000000 cfunits-3.3.6/README.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 10:52:46.394537 cfunits-3.3.6/cfunits/
+-rw-rw-r--   0 david     (1000) david     (1000)     1360 2023-05-03 10:46:34.000000 cfunits-3.3.6/cfunits/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 10:52:46.394537 cfunits-3.3.6/cfunits/etc/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 10:52:46.394537 cfunits-3.3.6/cfunits/etc/udunits/
+-rw-rw-r--   0 david     (1000) david     (1000)      301 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/etc/udunits/README
+-rw-rw-r--   0 david     (1000) david     (1000)     7100 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/etc/udunits/udunits2-accepted.xml
+-rw-rw-r--   0 david     (1000) david     (1000)     6994 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/etc/udunits/udunits2-accepted.xml.nonCF
+-rw-rw-r--   0 david     (1000) david     (1000)     3170 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/etc/udunits/udunits2-base.xml
+-rw-rw-r--   0 david     (1000) david     (1000)    55074 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/etc/udunits/udunits2-common.xml
+-rw-rw-r--   0 david     (1000) david     (1000)    53091 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/etc/udunits/udunits2-common.xml.nonCF
+-rw-rw-r--   0 david     (1000) david     (1000)     4034 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/etc/udunits/udunits2-derived.xml
+-rw-rw-r--   0 david     (1000) david     (1000)     3915 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/etc/udunits/udunits2-derived.xml.nonCF
+-rw-rw-r--   0 david     (1000) david     (1000)     2308 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/etc/udunits/udunits2-prefixes.xml
+-rw-rw-r--   0 david     (1000) david     (1000)      517 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/etc/udunits/udunits2.xml
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 10:52:46.394537 cfunits-3.3.6/cfunits/test/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/test/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2596 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/test/run_tests.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     2083 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/test/run_tests_and_coverage
+-rw-rw-r--   0 david     (1000) david     (1000)    16697 2023-05-03 10:45:26.000000 cfunits-3.3.6/cfunits/test/test_Units.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2117 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/test/test_style.py
+-rw-rw-r--   0 david     (1000) david     (1000)    83127 2023-05-03 10:45:26.000000 cfunits-3.3.6/cfunits/units.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 10:52:46.394537 cfunits-3.3.6/cfunits.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     2161 2023-05-03 10:52:46.000000 cfunits-3.3.6/cfunits.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      806 2023-05-03 10:52:46.000000 cfunits-3.3.6/cfunits.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-05-03 10:52:46.000000 cfunits-3.3.6/cfunits.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      243 2023-05-03 10:52:46.000000 cfunits-3.3.6/cfunits.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        8 2023-05-03 10:52:46.000000 cfunits-3.3.6/cfunits.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      433 2022-08-01 08:33:37.000000 cfunits-3.3.6/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)       42 2022-09-22 15:21:51.000000 cfunits-3.3.6/requirements.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2023-05-03 10:52:46.394537 cfunits-3.3.6/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)     4234 2023-05-03 10:45:26.000000 cfunits-3.3.6/setup.py
```

### Comparing `cfunits-3.3.5/LICENSE` & `cfunits-3.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.5/PKG-INFO` & `cfunits-3.3.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfunits
-Version: 3.3.5
+Version: 3.3.6
 Summary: A python interface to UNIDATA's UDUNITS-2 package with CF extensions 
 Home-page: https://bitbucket.org/cfpython/cfunits-python
 Download-URL: https://bitbucket.org/cfpython/cfunits-python/downloads
 Author: David Hassell
 Author-email: david.hassell@ncas.ac.uk
 Maintainer: David Hassell
 Maintainer-email: david.hassell@ncas.ac.uk
@@ -54,9 +54,7 @@
 https://ncas-cms.github.io/cfunits
 
 Installation
 ============
 
 https://ncas-cms.github.io/cfunits/installation.html
 
-
-
```

### Comparing `cfunits-3.3.5/README.md` & `cfunits-3.3.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [UNIDATA's UDUNITS-2 package](http://www.unidata.ucar.edu/software/udunits)
 with CF extensions.
 
 [![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/NCAS-CMS/cfunits?color=000000&label=latest%20version)](https://ncas-cms.github.io/cfunits/Changelog.html)
 [![PyPI](https://img.shields.io/pypi/v/cfunits?color=000000)](https://pypi.org/project/cfunits/)
 [![Conda](https://img.shields.io/conda/v/ncas/cfunits?color=000000)](https://ncas-cms.github.io/cfunits/installation.html#conda)
 
-[![Conda](https://img.shields.io/conda/pn/ncas/cfunits?color=2d8659)](https://ncas-cms.github.io/cfunits/installation.html#operating-systems) [![Website](https://img.shields.io/website?color=2d8659&down_message=online&label=documentation&up_message=online&url=https%3A%2F%2Fncas-cms.github.io%2Fcfunits%2F)](https://ncas-cms.github.io/cfunits/index.html) [![GitHub](https://img.shields.io/github/license/NCAS-CMS/cfunits?color=2d8659)](https://github.com/NCAS-CMS/cfunits/blob/master/LICENSE)
+[![Conda](https://img.shields.io/conda/pn/ncas/cfunits?color=2d8659)](https://ncas-cms.github.io/cfunits/installation.html#operating-systems) [![Website](https://img.shields.io/website?color=2d8659&down_message=online&label=documentation&up_message=online&url=https%3A%2F%2Fncas-cms.github.io%2Fcfunits%2F)](https://ncas-cms.github.io/cfunits/index.html) [![GitHub](https://img.shields.io/github/license/NCAS-CMS/cfunits?color=2d8659)](https://github.com/NCAS-CMS/cfunits/blob/main/LICENSE)
 
 [![GitHub Workflow Status](https://img.shields.io/github/workflow/status/NCAS-CMS/cfunits/Run%20test%20suite?color=006666&label=test%20suite%20workflow)](https://github.com/NCAS-CMS/cfunits/actions) [![Codecov](https://img.shields.io/codecov/c/github/NCAS-CMS/cfunits?color=006666)](https://codecov.io/gh/NCAS-CMS/cfunits)
 
 Store, combine and compare physical units and convert numeric values
 to different units.
 
 Units are as defined in UNIDATA's UDUNITS-2 package, except for
```

### Comparing `cfunits-3.3.5/cfunits/__init__.py` & `cfunits-3.3.6/cfunits/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 In addition, some units are either new to, modified from, or removed
 from the standard UDUNITS-2 database in order to be more consistent
 with the CF conventions.
 
 """
 
 __Conventions__ = "CF-1.10"
-__date__ = "2022-09-22"
-__version__ = "3.3.5"
+__date__ = "2023-05-03"
+__version__ = "3.3.6"
 __cf_version__ = "1.10"
 
 import platform
 
 from packaging.version import Version
 
 try:
```

### Comparing `cfunits-3.3.5/cfunits/etc/udunits/udunits2-accepted.xml` & `cfunits-3.3.6/cfunits/etc/udunits/udunits2-accepted.xml`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.5/cfunits/etc/udunits/udunits2-accepted.xml.nonCF` & `cfunits-3.3.6/cfunits/etc/udunits/udunits2-accepted.xml.nonCF`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.5/cfunits/etc/udunits/udunits2-base.xml` & `cfunits-3.3.6/cfunits/etc/udunits/udunits2-base.xml`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.5/cfunits/etc/udunits/udunits2-common.xml` & `cfunits-3.3.6/cfunits/etc/udunits/udunits2-common.xml`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.5/cfunits/etc/udunits/udunits2-common.xml.nonCF` & `cfunits-3.3.6/cfunits/etc/udunits/udunits2-common.xml.nonCF`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.5/cfunits/etc/udunits/udunits2-derived.xml` & `cfunits-3.3.6/cfunits/etc/udunits/udunits2-derived.xml`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.5/cfunits/etc/udunits/udunits2-derived.xml.nonCF` & `cfunits-3.3.6/cfunits/etc/udunits/udunits2-derived.xml.nonCF`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.5/cfunits/etc/udunits/udunits2-prefixes.xml` & `cfunits-3.3.6/cfunits/etc/udunits/udunits2-prefixes.xml`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.5/cfunits/etc/udunits/udunits2.xml` & `cfunits-3.3.6/cfunits/etc/udunits/udunits2.xml`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.5/cfunits/test/run_tests.py` & `cfunits-3.3.6/cfunits/test/run_tests.py`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.5/cfunits/test/run_tests_and_coverage` & `cfunits-3.3.6/cfunits/test/run_tests_and_coverage`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.5/cfunits/test/test_Units.py` & `cfunits-3.3.6/cfunits/test/test_Units.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import faulthandler
 import math
 import os
 import unittest
 
 import numpy
+from dask.base import tokenize
 
 faulthandler.enable()  # to debug seg faults and timeouts
 
 import cfunits
 from cfunits import Units
 
 
@@ -389,13 +390,40 @@
         self.assertEqual(u.formatted(), "h since 2100-01-01 00:00:00")
 
     def test_Units_default_calendar(self):
         """Tests the default calendar on `Units`."""
         u = Units("days since 2000-01-01")
         self.assertEqual(u._canonical_calendar, "standard")
 
+    def test_Units__dask_tokenize__(self):
+        """Tests dask tokenization."""
+        u = Units("m")
+        self.assertEqual(tokenize(u), tokenize(Units("m")))
+        self.assertNotEqual(tokenize(u), tokenize(Units("metre")))
+
+        u = Units("days since 2000-01-01")
+        self.assertEqual(tokenize(u), tokenize(Units("days since 2000-01-01")))
+        self.assertNotEqual(tokenize(u), tokenize(Units("d since 2000-01-01")))
+
+        u = Units("days since 2000-01-01", calendar="365_day")
+        self.assertEqual(
+            tokenize(u),
+            tokenize(Units("days since 2000-01-01", calendar="365_day")),
+        )
+        self.assertEqual(
+            tokenize(u),
+            tokenize(Units("days since 2000-01-01", calendar="noleap")),
+        )
+
+        u = Units("days since 2000-01-01", calendar="standard")
+        self.assertEqual(tokenize(u), tokenize(Units("days since 2000-01-01")))
+
+        u = Units("bad units")
+        self.assertEqual(tokenize(u), tokenize(Units("bad units")))
+        self.assertNotEqual(tokenize(u), tokenize(Units("worse units")))
+
 
 if __name__ == "__main__":
     print("cfunits version:", cfunits.__version__)
     print("cfunits path:", os.path.abspath(cfunits.__file__))
     print("")
     unittest.main(verbosity=2)
```

### Comparing `cfunits-3.3.5/cfunits/test/test_style.py` & `cfunits-3.3.6/cfunits/test/test_style.py`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.5/cfunits/units.py` & `cfunits-3.3.6/cfunits/units.py`

 * *Files 0% similar despite different names*

```diff
@@ -866,14 +866,21 @@
         self._ut_unit = None
         self._isreftime = False
         self._calendar = None
         self._canonical_calendar = None
         self._utime = None
         self._units_since_reftime = None
 
+    def __dask_tokenize__(self):
+        """Return a value fully representative of the object."""
+        if self._isvalid:
+            return (Units, self._units, self._utime)
+
+        return (Units, self._units)
+
     def __getstate__(self):
         """Called when pickling.
 
         :Returns:
 
             `dict`
                 A dictionary of the instance's attributes
```

### Comparing `cfunits-3.3.5/cfunits.egg-info/PKG-INFO` & `cfunits-3.3.6/cfunits.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfunits
-Version: 3.3.5
+Version: 3.3.6
 Summary: A python interface to UNIDATA's UDUNITS-2 package with CF extensions 
 Home-page: https://bitbucket.org/cfpython/cfunits-python
 Download-URL: https://bitbucket.org/cfpython/cfunits-python/downloads
 Author: David Hassell
 Author-email: david.hassell@ncas.ac.uk
 Maintainer: David Hassell
 Maintainer-email: david.hassell@ncas.ac.uk
@@ -54,9 +54,7 @@
 https://ncas-cms.github.io/cfunits
 
 Installation
 ============
 
 https://ncas-cms.github.io/cfunits/installation.html
 
-
-
```

### Comparing `cfunits-3.3.5/cfunits.egg-info/SOURCES.txt` & `cfunits-3.3.6/cfunits.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.5/setup.py` & `cfunits-3.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
         "pydocstyle",
     ],
 }
 tests_require = [
     "pytest",
     "pycodestyle",
     "coverage",
+    "dask",
 ]
 
 setup(
     name="cfunits",
     long_description=long_description,
     version=version,
     description="A python interface to UNIDATA's UDUNITS-2 package with CF extensions ",
```

