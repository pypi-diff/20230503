# Comparing `tmp/pvlive_api-1.0.0.tar.gz` & `tmp/pvlive_api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvlive_api-1.0.0.tar", last modified: Tue May  2 16:49:49 2023, max compression
+gzip compressed data, was "pvlive_api-1.1.0.tar", last modified: Wed May  3 20:27:59 2023, max compression
```

## Comparing `pvlive_api-1.0.0.tar` & `pvlive_api-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 16:49:49.397793 pvlive_api-1.0.0/
--rw-rw-rw-   0        0        0    12410 2023-05-02 16:49:49.397793 pvlive_api-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    11433 2023-05-02 16:23:49.000000 pvlive_api-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 16:49:49.379450 pvlive_api-1.0.0/Tests/
--rw-rw-rw-   0        0        0        0 2023-02-15 16:12:03.000000 pvlive_api-1.0.0/Tests/__init__.py
--rw-rw-rw-   0        0        0    10205 2023-05-02 16:44:24.000000 pvlive_api-1.0.0/Tests/test_pvlive_api.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:49:49.381427 pvlive_api-1.0.0/pvlive_api/
--rw-rw-rw-   0        0        0       62 2023-02-15 16:12:03.000000 pvlive_api-1.0.0/pvlive_api/__init__.py
--rw-rw-rw-   0        0        0    23398 2023-05-02 16:46:04.000000 pvlive_api-1.0.0/pvlive_api/pvlive.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:49:49.396783 pvlive_api-1.0.0/pvlive_api.egg-info/
--rw-rw-rw-   0        0        0    12410 2023-05-02 16:49:49.000000 pvlive_api-1.0.0/pvlive_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-05-02 16:49:49.000000 pvlive_api-1.0.0/pvlive_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 16:49:49.000000 pvlive_api-1.0.0/pvlive_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-02 16:49:49.000000 pvlive_api-1.0.0/pvlive_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2023-05-02 16:49:49.000000 pvlive_api-1.0.0/pvlive_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-02 16:49:49.000000 pvlive_api-1.0.0/pvlive_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-02 16:49:49.401321 pvlive_api-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     4330 2023-05-02 16:24:35.000000 pvlive_api-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 20:27:59.972836 pvlive_api-1.1.0/
+-rw-rw-rw-   0        0        0    12410 2023-05-03 20:27:59.972836 pvlive_api-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11433 2023-05-03 20:21:07.000000 pvlive_api-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 20:27:59.962711 pvlive_api-1.1.0/Tests/
+-rw-rw-rw-   0        0        0        0 2023-02-15 16:12:03.000000 pvlive_api-1.1.0/Tests/__init__.py
+-rw-rw-rw-   0        0        0    10205 2023-05-02 16:44:24.000000 pvlive_api-1.1.0/Tests/test_pvlive_api.py
+drwxrwxrwx   0        0        0        0 2023-05-03 20:27:59.962711 pvlive_api-1.1.0/pvlive_api/
+-rw-rw-rw-   0        0        0       62 2023-02-15 16:12:03.000000 pvlive_api-1.1.0/pvlive_api/__init__.py
+-rw-rw-rw-   0        0        0    24027 2023-05-03 20:17:28.000000 pvlive_api-1.1.0/pvlive_api/pvlive.py
+drwxrwxrwx   0        0        0        0 2023-05-03 20:27:59.972836 pvlive_api-1.1.0/pvlive_api.egg-info/
+-rw-rw-rw-   0        0        0    12410 2023-05-03 20:27:59.000000 pvlive_api-1.1.0/pvlive_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-05-03 20:27:59.000000 pvlive_api-1.1.0/pvlive_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 20:27:59.000000 pvlive_api-1.1.0/pvlive_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-03 20:27:59.000000 pvlive_api-1.1.0/pvlive_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-05-03 20:27:59.000000 pvlive_api-1.1.0/pvlive_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-03 20:27:59.000000 pvlive_api-1.1.0/pvlive_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-03 20:27:59.981342 pvlive_api-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     4330 2023-05-03 20:21:08.000000 pvlive_api-1.1.0/setup.py
```

### Comparing `pvlive_api-1.0.0/PKG-INFO` & `pvlive_api-1.1.0/pvlive_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: pvlive_api
-Version: 1.0.0
+Name: pvlive-api
+Version: 1.1.0
 Summary: A Python interface for the PV_Live web API from Sheffield Solar.
 Home-page: https://github.com/SheffieldSolar/PV_Live
-Download-URL: https://github.com/SheffieldSolar/PV_Live-API/archive/refs/tags/1.0.0.tar.gz
+Download-URL: https://github.com/SheffieldSolar/PV_Live-API/archive/refs/tags/1.1.0.tar.gz
 Author: Jamie Taylor
 Author-email: jamie.taylor@sheffield.ac.uk
 License: None
 Keywords: solar pv pv_live api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 
 # PV_Live
 A Python implementation of the PV_Live web API. See https://www.solar.sheffield.ac.uk/pvlive/
 
-**Latest Version: 1.0.0**
+**Latest Version: 1.1.0**
 
 **New! Updated 2023-05-02 to provide support for proxy connections.**
 
 ## About this repository
 
 * This Python library provides a convenient interface for the PV_Live web API to facilitate accessing PV_Live results in Python code.
 * Developed and tested with Python 3.10, should work with Python 3.7+. Support for Python 2.7+ has been discontinued as of 2021-01-15.
```

### Comparing `pvlive_api-1.0.0/README.md` & `pvlive_api-1.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 # PV_Live
 A Python implementation of the PV_Live web API. See https://www.solar.sheffield.ac.uk/pvlive/
 
-**Latest Version: 1.0.0**
+**Latest Version: 1.1.0**
 
 **New! Updated 2023-05-02 to provide support for proxy connections.**
 
 ## About this repository
 
 * This Python library provides a convenient interface for the PV_Live web API to facilitate accessing PV_Live results in Python code.
 * Developed and tested with Python 3.10, should work with Python 3.7+. Support for Python 2.7+ has been discontinued as of 2021-01-15.
```

### Comparing `pvlive_api-1.0.0/Tests/test_pvlive_api.py` & `pvlive_api-1.1.0/Tests/test_pvlive_api.py`

 * *Files identical despite different names*

### Comparing `pvlive_api-1.0.0/pvlive_api/pvlive.py` & `pvlive_api-1.1.0/pvlive_api/pvlive.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import os
 import json
 from datetime import datetime, timedelta, date, time
 from time import sleep
 from typing import List, Union, Tuple, Dict, Optional
 import inspect
 import argparse
+import re
 
 import pytz
 import requests
 from numpy import nan, int64
 import pandas as pd
 
 class PVLiveException(Exception):
@@ -373,15 +374,18 @@
         delay = 1
         while not success and try_counter < self.retries + 1:
             try_counter += 1
             try:
                 page = requests.get(url, proxies=self.proxies)
                 page.raise_for_status()
                 success = True
-            except requests.exceptions.HTTPError:
+            except requests.exceptions.HTTPError as err:
+                if page.status_code == 400:
+                    helper = re.search(r"<p>(.*)</p>", page.text).group(1)
+                    raise PVLiveException(f"PV_Live API received Bad Request (400)... {helper}")
                 sleep(delay)
                 delay *= 2
                 continue
         if not success:
             raise PVLiveException("Error communicating with the PV_Live API.")
         try:
             return json.loads(page.text)
@@ -430,14 +434,18 @@
     parser.add_argument("--entity_type", metavar="<entity_type>", dest="entity_type",
                         action="store", type=str, required=False, default="gsp",
                         choices=["gsp", "pes"],
                         help="Specify an entity type, either 'gsp' or 'pes'. Default is 'gsp'.")
     parser.add_argument("--entity_id", metavar="<entity_id>", dest="entity_id", action="store",
                         type=int, required=False, default=0,
                         help="Specify an entity ID, default is 0 (i.e. national).")
+    parser.add_argument("--extra_fields", metavar="<field1[,field2, ...]>", dest="extra_fields",
+                        action="store", type=str, required=False, default="installedcapacity_mwp",
+                        help="Specify an extra_fields (as a comma-separated list to include when "
+                             "requesting data from the API, defaults to 'installedcapacity_mwp'.")
     parser.add_argument("--period", metavar="<5|30>", dest="period", action="store",
                         type=int, required=False, default=30, choices=(5, 30),
                         help="Desired temporal resolution (in minutes) for PV outturn estimates. "
                              "Default is 30.")
     parser.add_argument("-q", "--quiet", dest="quiet", action="store_true",
                         required=False, help="Specify to not print anything to stdout.")
     parser.add_argument("-o", "--outfile", metavar="</path/to/output/file>", dest="outfile",
@@ -487,21 +495,21 @@
 
 def main():
     """Load CLI options and access the API accordingly."""
     options = parse_options()
     pvl = PVLive(proxies=options.proxies)
     if options.start is None and options.end is None:
         data = pvl.latest(entity_type=options.entity_type, entity_id=options.entity_id,
-                          extra_fields="installedcapacity_mwp", dataframe=True)
+                          extra_fields=options.extra_fields, dataframe=True)
     else:
         start = datetime(2014, 1, 1, 0, 30, tzinfo=pytz.utc) if options.start is None \
             else options.start
         end = pytz.utc.localize(datetime.utcnow()) if options.end is None else options.end
         data = pvl.between(start, end, entity_type=options.entity_type, entity_id=options.entity_id,
-                           extra_fields="installedcapacity_mwp", period=options.period,
+                           extra_fields=options.extra_fields, period=options.period,
                            dataframe=True)
     if options.outfile is not None:
         data.to_csv(options.outfile, float_format="%.3f", index=False)
     if not options.quiet:
         print(data)
 
 if __name__ == "__main__":
```

### Comparing `pvlive_api-1.0.0/pvlive_api.egg-info/PKG-INFO` & `pvlive_api-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: pvlive-api
-Version: 1.0.0
+Name: pvlive_api
+Version: 1.1.0
 Summary: A Python interface for the PV_Live web API from Sheffield Solar.
 Home-page: https://github.com/SheffieldSolar/PV_Live
-Download-URL: https://github.com/SheffieldSolar/PV_Live-API/archive/refs/tags/1.0.0.tar.gz
+Download-URL: https://github.com/SheffieldSolar/PV_Live-API/archive/refs/tags/1.1.0.tar.gz
 Author: Jamie Taylor
 Author-email: jamie.taylor@sheffield.ac.uk
 License: None
 Keywords: solar pv pv_live api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 
 # PV_Live
 A Python implementation of the PV_Live web API. See https://www.solar.sheffield.ac.uk/pvlive/
 
-**Latest Version: 1.0.0**
+**Latest Version: 1.1.0**
 
 **New! Updated 2023-05-02 to provide support for proxy connections.**
 
 ## About this repository
 
 * This Python library provides a convenient interface for the PV_Live web API to facilitate accessing PV_Live results in Python code.
 * Developed and tested with Python 3.10, should work with Python 3.7+. Support for Python 2.7+ has been discontinued as of 2021-01-15.
```

### Comparing `pvlive_api-1.0.0/setup.py` & `pvlive_api-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,24 +18,24 @@
 
 setup(
     name="pvlive_api",
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="1.0.0",
+    version="1.1.0",
 
     description="A Python interface for the PV_Live web API from Sheffield Solar.",
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url="https://github.com/SheffieldSolar/PV_Live",
 
-    download_url="https://github.com/SheffieldSolar/PV_Live-API/archive/refs/tags/1.0.0.tar.gz",
+    download_url="https://github.com/SheffieldSolar/PV_Live-API/archive/refs/tags/1.1.0.tar.gz",
 
     # Author details
     author="Jamie Taylor",
     author_email="jamie.taylor@sheffield.ac.uk",
 
     # Choose your license
     license="None",
```

