# Comparing `tmp/cadati-0.0.2.tar.gz` & `tmp/cadati-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cadati-0.0.2.tar", last modified: Mon Jun 29 14:06:09 2020, max compression
+gzip compressed data, was "cadati-0.0.4.tar", last modified: Wed May  3 19:59:07 2023, max compression
```

## Comparing `cadati-0.0.2.tar` & `cadati-0.0.4.tar`

### file list

```diff
@@ -1,42 +1,46 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-29 14:06:09.000000 cadati-0.0.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)      589 2020-06-29 14:04:47.000000 cadati-0.0.2/.coveragerc
--rw-rw-r--   0 travis    (2000) travis    (2000)      520 2020-06-29 14:04:47.000000 cadati-0.0.2/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)     1315 2020-06-29 14:04:47.000000 cadati-0.0.2/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)       91 2020-06-29 14:04:47.000000 cadati-0.0.2/AUTHORS.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      148 2020-06-29 14:04:47.000000 cadati-0.0.2/CHANGELOG.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1116 2020-06-29 14:04:47.000000 cadati-0.0.2/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2428 2020-06-29 14:06:09.000000 cadati-0.0.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1627 2020-06-29 14:04:47.000000 cadati-0.0.2/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-29 14:06:09.000000 cadati-0.0.2/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7606 2020-06-29 14:04:47.000000 cadati-0.0.2/docs/Makefile
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-29 14:06:09.000000 cadati-0.0.2/docs/_static/
--rw-rw-r--   0 travis    (2000) travis    (2000)       18 2020-06-29 14:04:47.000000 cadati-0.0.2/docs/_static/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)       41 2020-06-29 14:04:47.000000 cadati-0.0.2/docs/authors.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       43 2020-06-29 14:04:47.000000 cadati-0.0.2/docs/changelog.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     9202 2020-06-29 14:04:47.000000 cadati-0.0.2/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2217 2020-06-29 14:04:47.000000 cadati-0.0.2/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2020-06-29 14:04:47.000000 cadati-0.0.2/docs/license.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       98 2020-06-29 14:04:47.000000 cadati-0.0.2/environment.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1251 2020-06-29 14:06:09.000000 cadati-0.0.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      570 2020-06-29 14:04:47.000000 cadati-0.0.2/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-29 14:06:09.000000 cadati-0.0.2/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-29 14:06:09.000000 cadati-0.0.2/src/cadati/
--rw-rw-r--   0 travis    (2000) travis    (2000)      363 2020-06-29 14:04:47.000000 cadati-0.0.2/src/cadati/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1821 2020-06-29 14:04:47.000000 cadati-0.0.2/src/cadati/cal_date.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      579 2020-06-29 14:04:47.000000 cadati-0.0.2/src/cadati/check_date.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2513 2020-06-29 14:04:47.000000 cadati-0.0.2/src/cadati/conv_doy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6277 2020-06-29 14:04:47.000000 cadati-0.0.2/src/cadati/dekad.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8894 2020-06-29 14:04:47.000000 cadati-0.0.2/src/cadati/jd_date.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2242 2020-06-29 14:04:47.000000 cadati-0.0.2/src/cadati/np_date.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-29 14:06:09.000000 cadati-0.0.2/src/cadati.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2428 2020-06-29 14:06:09.000000 cadati-0.0.2/src/cadati.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      688 2020-06-29 14:06:09.000000 cadati-0.0.2/src/cadati.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-29 14:06:09.000000 cadati-0.0.2/src/cadati.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-29 14:06:09.000000 cadati-0.0.2/src/cadati.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       55 2020-06-29 14:06:09.000000 cadati-0.0.2/src/cadati.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2020-06-29 14:06:09.000000 cadati-0.0.2/src/cadati.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-29 14:06:09.000000 cadati-0.0.2/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      227 2020-06-29 14:04:47.000000 cadati-0.0.2/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1361 2020-06-29 14:04:47.000000 cadati-0.0.2/tests/test_conv_doy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6947 2020-06-29 14:04:47.000000 cadati-0.0.2/tests/test_date_conversion.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5169 2020-06-29 14:04:47.000000 cadati-0.0.2/tests/test_dekad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:59:07.134353 cadati-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-03 19:58:58.000000 cadati-0.0.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:59:07.130353 cadati-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:59:07.130353 cadati-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-03 19:58:58.000000 cadati-0.0.4/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-03 19:58:58.000000 cadati-0.0.4/.github/workflows/upload_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-03 19:58:58.000000 cadati-0.0.4/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-03 19:58:58.000000 cadati-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-03 19:58:58.000000 cadati-0.0.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-03 19:58:58.000000 cadati-0.0.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-03 19:58:58.000000 cadati-0.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-03 19:59:07.134353 cadati-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-03 19:58:58.000000 cadati-0.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:59:07.134353 cadati-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-05-03 19:58:58.000000 cadati-0.0.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:59:07.134353 cadati-0.0.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-03 19:58:58.000000 cadati-0.0.4/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 19:58:58.000000 cadati-0.0.4/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 19:58:58.000000 cadati-0.0.4/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-05-03 19:58:58.000000 cadati-0.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-03 19:58:58.000000 cadati-0.0.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-03 19:58:58.000000 cadati-0.0.4/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-03 19:58:58.000000 cadati-0.0.4/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-03 19:59:07.134353 cadati-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-03 19:58:58.000000 cadati-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:59:07.130353 cadati-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:59:07.134353 cadati-0.0.4/src/cadati/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-03 19:58:58.000000 cadati-0.0.4/src/cadati/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-03 19:58:58.000000 cadati-0.0.4/src/cadati/cal_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-03 19:58:58.000000 cadati-0.0.4/src/cadati/check_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-03 19:58:58.000000 cadati-0.0.4/src/cadati/conv_doy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-03 19:58:58.000000 cadati-0.0.4/src/cadati/dekad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8894 2023-05-03 19:58:58.000000 cadati-0.0.4/src/cadati/jd_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-03 19:58:58.000000 cadati-0.0.4/src/cadati/np_date.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:59:07.134353 cadati-0.0.4/src/cadati.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-03 19:59:07.000000 cadati-0.0.4/src/cadati.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-03 19:59:07.000000 cadati-0.0.4/src/cadati.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:59:07.000000 cadati-0.0.4/src/cadati.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:59:07.000000 cadati-0.0.4/src/cadati.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-03 19:59:07.000000 cadati-0.0.4/src/cadati.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 19:59:07.000000 cadati-0.0.4/src/cadati.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:59:07.134353 cadati-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-03 19:58:58.000000 cadati-0.0.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-03 19:58:58.000000 cadati-0.0.4/tests/test_conv_doy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-05-03 19:58:58.000000 cadati-0.0.4/tests/test_date_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-03 19:58:58.000000 cadati-0.0.4/tests/test_dekad.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cadati-0.0.2/.coveragerc` & `cadati-0.0.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `cadati-0.0.2/.gitignore` & `cadati-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `cadati-0.0.2/LICENSE.txt` & `cadati-0.0.4/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2020 TU Wien, Department of Geodesy and Geoinformation
+Copyright (c) 2023 TU Wien, Department of Geodesy and Geoinformation
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `cadati-0.0.2/README.rst` & `cadati-0.0.4/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 ======
 cadati
 ======
 
-.. image:: https://travis-ci.org/TUW-GEO/cadati.svg?branch=master
-    :target: https://travis-ci.org/TUW-GEO/cadati
+.. image:: https://github.com/TUW-GEO/cadati/workflows/ubuntu/badge.svg
+   :target: https://github.com/TUW-GEO/cadati/actions/workflows/ubuntu.yml
+
+.. image:: https://github.com/TUW-GEO/cadati/workflows/windows/badge.svg
+   :target: https://github.com/TUW-GEO/cadati/actions/workflows/windows.yml
 
 .. image:: https://coveralls.io/repos/github/TUW-GEO/cadati/badge.svg?branch=master
    :target: https://coveralls.io/github/TUW-GEO/cadati?branch=master
 
 .. image:: https://badge.fury.io/py/cadati.svg
     :target: http://badge.fury.io/py/cadati
```

### Comparing `cadati-0.0.2/docs/Makefile` & `cadati-0.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cadati-0.0.2/docs/conf.py` & `cadati-0.0.4/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = u'cadati'
-copyright = u'2020, TU Wien'
+copyright = u'2023, TU Wien'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = ''  # Is set by calling `setup.py docs`
```

### Comparing `cadati-0.0.2/docs/index.rst` & `cadati-0.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cadati-0.0.2/setup.cfg` & `cadati-0.0.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
 testing = 
-	pytest==5.0.1
+	pytest==6.2.5
 	pytest-cov
 
 [options.entry_points]
 
 [test]
 extras = True
```

### Comparing `cadati-0.0.2/setup.py` & `cadati-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `cadati-0.0.2/src/cadati/cal_date.py` & `cadati-0.0.4/src/cadati/cal_date.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2023, TU Wien, Department of Geodesy and Geoinformation
 # Distributed under the MIT License (see LICENSE.txt)
 
 """
 Module contains function to convert calendar array [Y,M,D,h,m,s,ms] into
 other date formats.
 """
 
@@ -30,15 +30,15 @@
 
     Returns
     -------
     dt : numpy.datetime64
         numpy datetime64 array.
     """
     nonleap_years = np.invert(is_leap_year(cal_dt[..., 0]))
-    md = days_past[cal_dt[..., 1].astype(np.int)-1]
+    md = days_past[cal_dt[..., 1].astype(np.int64)-1]
 
     rel_days = cal_dt[..., 2]*24*3600*1e3 + cal_dt[..., 3]*3600*1e3 \
         + cal_dt[..., 4]*60*1e3 + cal_dt[..., 5] * 1e3 + cal_dt[..., 6]
 
     fd = (md - nonleap_years + np.logical_and(
         md < 60, nonleap_years)-1)*24*3600*1e3 + rel_days
```

### Comparing `cadati-0.0.2/src/cadati/check_date.py` & `cadati-0.0.4/src/cadati/check_date.py`

 * *Files identical despite different names*

### Comparing `cadati-0.0.2/src/cadati/conv_doy.py` & `cadati-0.0.4/src/cadati/conv_doy.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2023, TU Wien, Department of Geodesy and Geoinformation
 # Distributed under the MIT License (see LICENSE.txt)
 
 """
 Module provides functions related to day of year conversions.
 """
 
 
@@ -37,17 +37,17 @@
         Day of year.
     """
     day_of_year = days_past[month - 1] + day
 
     if year is not None:
         nonleap_years = np.invert(is_leap_year(year))
         day_of_year = (day_of_year -
-                       nonleap_years.astype('int') +
+                       nonleap_years.astype(np.int64) +
                        np.logical_and(
-                           day_of_year < 60, nonleap_years).astype('int'))
+                           day_of_year < 60, nonleap_years).astype(np.int64))
 
     return day_of_year
 
 
 def clim_jd2ts(clim, jd):
     """
     Convert climatology array into time series array for given timestamps
```

### Comparing `cadati-0.0.2/src/cadati/dekad.py` & `cadati-0.0.4/src/cadati/dekad.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2023, TU Wien, Department of Geodesy and Geoinformation
 # Distributed under the MIT License (see LICENSE.txt)
 
 """
 This module provides functions for date manipulation on a dekadal basis.
 
 A dekad is defined as days 1-10, 11-20 and 21-last day of a month.
```

### Comparing `cadati-0.0.2/src/cadati/jd_date.py` & `cadati-0.0.4/src/cadati/jd_date.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2023, TU Wien, Department of Geodesy and Geoinformation
 # Distributed under the MIT License (see LICENSE.txt)
 
 """
 Module provides function to convert julian dates into other date formats.
 """
```

### Comparing `cadati-0.0.2/src/cadati/np_date.py` & `cadati-0.0.4/src/cadati/np_date.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,21 @@
-# Copyright (c) 2020, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2023, TU Wien, Department of Geodesy and Geoinformation
 # Distributed under the MIT License (see LICENSE.txt)
 
 """
 Module contains function to convert numpy.datetime64 into other date formats.
 """
 
 import numpy as np
 
 from cadati.check_date import is_leap_year
 
-ref_dt = np.datetime64('1970-01-01')
-ref_jd = 2440587.5  # julian date on 1970-01-01 00:00:00
-
-
 # leap year
-days_past = np.array([0, 31, 60, 91, 121, 152, 182, 213,
-                      244, 274, 305, 335, 366])
+days_past = np.array(
+    [0, 31, 60, 91, 121, 152, 182, 213, 244, 274, 305, 335, 366])
 
 
 def dt2jd(dt):
     """
     Convert numpy.datetime to julian dates.
 
     Parameters
@@ -28,15 +24,18 @@
         numpy.ndarray of datetime64
 
     Returns
     -------
     jd : numpy.float64
         Array of julian dates.
     """
-    return (dt - ref_dt)/np.timedelta64(1, 'D') + ref_jd
+    # julian date on 1970-01-01 00:00:00
+    ref_jd = 2440587.5
+
+    return (dt - np.datetime64("1970-01-01")) / np.timedelta64(1, "D") + ref_jd
 
 
 def dt2cal(dt, doy_respect_nonleap_year=True):
     """
     Convert array of datetime64 to a calendar array of year, month, day, hour,
     minute, seconds, microsecond and day of year with these quantites indexed
     on the last axis.
@@ -51,15 +50,15 @@
 
     Returns
     -------
     cal_dt : numpy.uint32 (..., 8)
         calendar array with last axis representing year, month, day, hour,
         minute, second, millisecond, day of year
     """
-    cal_dt = np.empty(dt.shape + (8,), dtype="u4")
+    cal_dt = np.empty(dt.shape + (8, ), dtype="u4")
 
     Y, M, D, h, m, s = [dt.astype("M8[{}]".format(x)) for x in "YMDhms"]
     cal_dt[..., 0] = Y + 1970
     cal_dt[..., 1] = (M - Y) + 1
     cal_dt[..., 2] = (D - M) + 1
     cal_dt[..., 3] = (dt - D).astype("m8[h]")
     cal_dt[..., 4] = (dt - h).astype("m8[m]")
@@ -69,7 +68,52 @@
 
     if doy_respect_nonleap_year:
         nonleap_years = np.invert(is_leap_year(cal_dt[..., 0]))
         cal_dt[..., 7] = cal_dt[..., 7] - nonleap_years + np.logical_and(
             cal_dt[..., 7] < 60, nonleap_years)
 
     return cal_dt
+
+
+def dt2days(dt, dt_ref=np.datetime64("1900-01-01 00:00:00")):
+    """
+    Convert dates to fraction of days.
+
+    Parameters
+    ----------
+    dt : numpy.datetime64
+        Dates.
+    dt_ref : numpy.datetime64, optional
+        Date reference
+
+    Returns
+    -------
+    days : numpy.ndarray
+        Fraction of days since reference date.
+    """
+    days = (dt - dt_ref) / np.timedelta64(1, "D")
+
+    return days
+
+
+def days2dt(days, dt_ref=np.datetime64("1900-01-01 00:00:00")):
+    """
+    Fraction of days to numpy.datetime64 (rounded to milliseconds.)
+
+    Parameters
+    ----------
+    days : numpy.ndarray
+        Fraction of days since reference date.
+    dt_ref : numpy.datetime64, optional
+        Date reference
+
+    Returns
+    -------
+    dt : numpy.datetime64
+        Dates.
+    """
+    days = np.asarray(days)
+
+    dt = (dt_ref + (days * 24. * 3600 * 1e6).astype("timedelta64[us]") +
+          np.timedelta64(500, "us")).astype("datetime64[ms]")
+
+    return dt
```

### Comparing `cadati-0.0.2/src/cadati.egg-info/SOURCES.txt` & `cadati-0.0.4/src/cadati.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 .coveragerc
 .gitignore
-.travis.yml
 AUTHORS.rst
 CHANGELOG.rst
 LICENSE.txt
 README.rst
 environment.yml
 setup.cfg
 setup.py
+.github/workflows/ubuntu.yml
+.github/workflows/upload_pypi.yml
+.github/workflows/windows.yml
 docs/Makefile
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/index.rst
 docs/license.rst
 docs/_static/.gitignore
```

### Comparing `cadati-0.0.2/tests/test_conv_doy.py` & `cadati-0.0.4/tests/test_conv_doy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2023, TU Wien, Department of Geodesy and Geoinformation
 # Distributed under the MIT License (see LICENSE.txt)
 
 """
 Module testing the different datetime conversion.
 """
 
 import unittest
```

### Comparing `cadati-0.0.2/tests/test_date_conversion.py` & `cadati-0.0.4/tests/test_date_conversion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# Copyright (c) 2020, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2023, TU Wien, Department of Geodesy and Geoinformation
 # Distributed under the MIT License (see LICENSE.txt)
 
 """
 Module testing the different datetime conversion.
 """
 
 import unittest
 import datetime
 
 import numpy as np
 import pandas as pd
 import numpy.testing as nptest
 
 from cadati.cal_date import cal2jd, cal2dt
-from cadati.np_date import dt2cal, dt2jd
+from cadati.np_date import dt2cal, dt2jd, days2dt, dt2days
 from cadati.jd_date import jd2cal, jd2dt, jd2doy
 from cadati.jd_date import julian2datetime, julian2date, julday, caldat
 
 
 class TestDateFunctions(unittest.TestCase):
 
     def setUp(self):
@@ -244,10 +244,44 @@
                                    2457533.9306828701]))
     dts = datetime.datetime(2016, 5, 25, 10, 20, 10, 999976)
     dt_should = np.array([dts, dts])
 
     assert type(dt) == np.ndarray
     assert np.all(dt == dt_should)
 
+def test_dt2days():
+    """
+    Test dt2days conversion.
+    """
+    dt = np.datetime64("2021-02-02 02:54:32.511")
+
+    assert dt == days2dt(dt2days(dt))
+
+def test_dt2days_array():
+    """
+    Test dt2days array conversion.
+    """
+    dt = np.arange('2021-09-24 08:00:00',
+                   '2021-09-24 11:20:00',
+                    np.timedelta64(20,'m'), dtype='datetime64')
+
+    assert np.all(dt == days2dt(dt2days(dt)))
+
+def test_days2dt():
+    """
+    Test days2dt conversion.
+    """
+    days = 44227.12121
+
+    assert days == dt2days(days2dt(days))
+
+def test_days2dt_array():
+    """
+    Test dt2days and days2dt conversion.
+    """
+    days = 44227.12121 + np.arange(10)
+
+    assert np.all(days == dt2days(days2dt(days)))
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cadati-0.0.2/tests/test_dekad.py` & `cadati-0.0.4/tests/test_dekad.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2023, TU Wien, Department of Geodesy and Geoinformation
 # Distributed under the MIT License (see LICENSE.txt)
 
 """
 Module testing the dekad module.
 """
 
 import unittest
```

