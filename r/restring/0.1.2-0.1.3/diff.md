# Comparing `tmp/restring-0.1.2.tar.gz` & `tmp/restring-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/restring-0.1.2.tar", last modified: Tue Mar 23 12:46:11 2021, max compression
+gzip compressed data, was "dist/restring-0.1.3.tar", last modified: Tue Mar 23 13:17:21 2021, max compression
```

## Comparing `restring-0.1.2.tar` & `restring-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 manz       (501) staff       (20)        0 2021-03-23 12:46:11.794479 restring-0.1.2/
--rw-r--r--   0 manz       (501) staff       (20)    29895 2021-03-23 12:46:11.795287 restring-0.1.2/PKG-INFO
--rwxr-xr-x   0 manz       (501) staff       (20)    25743 2021-03-23 04:39:48.000000 restring-0.1.2/README.md
-drwxr-xr-x   0 manz       (501) staff       (20)        0 2021-03-23 12:46:11.778668 restring-0.1.2/bin/
--rwxr-xr-x   0 manz       (501) staff       (20)       22 2021-03-23 04:39:48.000000 restring-0.1.2/bin/restring-gui
-drwxr-xr-x   0 manz       (501) staff       (20)        0 2021-03-23 12:46:11.785471 restring-0.1.2/restring/
--rwxr-xr-x   0 manz       (501) staff       (20)      564 2021-03-23 04:39:48.000000 restring-0.1.2/restring/__init__.py
--rwxr-xr-x   0 manz       (501) staff       (20)    39432 2021-03-23 04:39:48.000000 restring-0.1.2/restring/gears.py
--rwxr-xr-x   0 manz       (501) staff       (20)     3735 2021-03-23 04:39:48.000000 restring-0.1.2/restring/guigears.py
--rwxr-xr-x   0 manz       (501) staff       (20)    57158 2021-03-23 04:39:48.000000 restring-0.1.2/restring/restring.py
--rwxr-xr-x   0 manz       (501) staff       (20)     1287 2021-03-23 04:39:48.000000 restring-0.1.2/restring/settings.py
-drwxr-xr-x   0 manz       (501) staff       (20)        0 2021-03-23 12:46:11.793699 restring-0.1.2/restring.egg-info/
--rw-r--r--   0 manz       (501) staff       (20)    29895 2021-03-23 12:46:11.000000 restring-0.1.2/restring.egg-info/PKG-INFO
--rw-r--r--   0 manz       (501) staff       (20)      306 2021-03-23 12:46:11.000000 restring-0.1.2/restring.egg-info/SOURCES.txt
--rw-r--r--   0 manz       (501) staff       (20)        1 2021-03-23 12:46:11.000000 restring-0.1.2/restring.egg-info/dependency_links.txt
--rw-r--r--   0 manz       (501) staff       (20)       26 2021-03-23 12:46:11.000000 restring-0.1.2/restring.egg-info/requires.txt
--rw-r--r--   0 manz       (501) staff       (20)        9 2021-03-23 12:46:11.000000 restring-0.1.2/restring.egg-info/top_level.txt
--rwxr-xr-x   0 manz       (501) staff       (20)       79 2021-03-23 12:46:11.796850 restring-0.1.2/setup.cfg
--rwxr-xr-x   0 manz       (501) staff       (20)      844 2021-03-23 04:39:48.000000 restring-0.1.2/setup.py
+drwxr-xr-x   0 manz       (501) staff       (20)        0 2021-03-23 13:17:21.219136 restring-0.1.3/
+-rw-r--r--   0 manz       (501) staff       (20)    29895 2021-03-23 13:17:21.219892 restring-0.1.3/PKG-INFO
+-rwxr-xr-x   0 manz       (501) staff       (20)    25743 2021-03-23 05:16:30.000000 restring-0.1.3/README.md
+drwxr-xr-x   0 manz       (501) staff       (20)        0 2021-03-23 13:17:21.210114 restring-0.1.3/bin/
+-rwxr-xr-x   0 manz       (501) staff       (20)       22 2021-03-23 05:16:30.000000 restring-0.1.3/bin/restring-gui
+drwxr-xr-x   0 manz       (501) staff       (20)        0 2021-03-23 13:17:21.214362 restring-0.1.3/restring/
+-rwxr-xr-x   0 manz       (501) staff       (20)      564 2021-03-23 05:16:30.000000 restring-0.1.3/restring/__init__.py
+-rwxr-xr-x   0 manz       (501) staff       (20)    39433 2021-03-23 05:16:30.000000 restring-0.1.3/restring/gears.py
+-rwxr-xr-x   0 manz       (501) staff       (20)     3735 2021-03-23 05:16:30.000000 restring-0.1.3/restring/guigears.py
+-rwxr-xr-x   0 manz       (501) staff       (20)    57094 2021-03-23 05:16:30.000000 restring-0.1.3/restring/restring.py
+-rwxr-xr-x   0 manz       (501) staff       (20)     1287 2021-03-23 05:16:30.000000 restring-0.1.3/restring/settings.py
+drwxr-xr-x   0 manz       (501) staff       (20)        0 2021-03-23 13:17:21.218466 restring-0.1.3/restring.egg-info/
+-rw-r--r--   0 manz       (501) staff       (20)    29895 2021-03-23 13:17:20.000000 restring-0.1.3/restring.egg-info/PKG-INFO
+-rw-r--r--   0 manz       (501) staff       (20)      306 2021-03-23 13:17:20.000000 restring-0.1.3/restring.egg-info/SOURCES.txt
+-rw-r--r--   0 manz       (501) staff       (20)        1 2021-03-23 13:17:20.000000 restring-0.1.3/restring.egg-info/dependency_links.txt
+-rw-r--r--   0 manz       (501) staff       (20)       26 2021-03-23 13:17:20.000000 restring-0.1.3/restring.egg-info/requires.txt
+-rw-r--r--   0 manz       (501) staff       (20)        9 2021-03-23 13:17:20.000000 restring-0.1.3/restring.egg-info/top_level.txt
+-rwxr-xr-x   0 manz       (501) staff       (20)       79 2021-03-23 13:17:21.221149 restring-0.1.3/setup.cfg
+-rwxr-xr-x   0 manz       (501) staff       (20)      844 2021-03-23 05:16:30.000000 restring-0.1.3/setup.py
```

### Comparing `restring-0.1.2/PKG-INFO` & `restring-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restring
-Version: 0.1.2
+Version: 0.1.3
 Summary: Functional enrichment terms aggregator.
 Home-page: https://github.com/Stemanz/restring
 Author: Stefano Manzini
 Author-email: stefano.manzini@gmail.com
 License: GPL-3.0
 Download-URL: https://github.com/Stemanz/restring/archive/master.zip
 Description: # restring
```

### Comparing `restring-0.1.2/README.md` & `restring-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `restring-0.1.2/restring/__init__.py` & `restring-0.1.3/restring/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # TODO: installation via Pip needs to be fixed
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 # the following tests if I can import stuff from restring.py
 from .restring import files
 
 # the following tests if I can import stuff from restring.py
 from restring.restring import working_directory
```

### Comparing `restring-0.1.2/restring/gears.py` & `restring-0.1.3/restring/gears.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from io import StringIO
 from random import choice
 from time import time, sleep
 from matplotlib import pyplot as plt
 import seaborn as sns
 
 
-from settings import (
+from .settings import (
     file_types,
     API_file_types,
     header_table,
     sep,
     PATH
 )
```

### Comparing `restring-0.1.2/restring/guigears.py` & `restring-0.1.3/restring/guigears.py`

 * *Files identical despite different names*

### Comparing `restring-0.1.2/restring/restring.py` & `restring-0.1.3/restring/restring.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,28 @@
 # -*- coding: utf-8 -*-
 # Author: Manzini Stefano; stefano.manzini@gmail.com
 
-__version__ = "0.2.040121 beta"  # dalla buonanima di __init__.py
+import tkinter as tk
+from tkinter import messagebox
+from tkinter.scrolledtext import ScrolledText
+import webbrowser
+import re
+import os
+from os.path import isdir
+from io import StringIO
+import pandas as pd
+from math import log
+from glob import glob
+import requests
+from random import choice
+from time import time, sleep
+from matplotlib import pyplot as plt
+import seaborn as sns
 
-from gears import (
+from .gears import (
     manzlog,
     get_dirs,
     aggregate_results,
     tableize_aggregated,
     summary,
     write_all_aggregated,
     write_all_summarized,
@@ -23,41 +38,24 @@
 
     # String API
     session_ID,
     get_functional_enrichment,
     write_functional_enrichment_tables,
     )
 
-from guigears import ReorderableListbox
+from .guigears import ReorderableListbox
 
-from settings import (
+from .settings import (
     file_types,
     API_file_types,
     header_table, 
     sep,
     PATH
 )
 
-import tkinter as tk
-from tkinter import messagebox
-from tkinter.scrolledtext import ScrolledText
-import webbrowser
-import re
-import os
-from os.path import isdir
-from io import StringIO
-import pandas as pd
-from math import log
-from glob import glob
-import requests
-from random import choice
-from time import time, sleep
-from matplotlib import pyplot as plt
-import seaborn as sns
-
 #TODO: unify error messages window popups
 
 # super-globals
 files = None
 working_directory = None
 SPECIES = 10090  #defaults to mouse
 ANALYSIS_TYPE = ["UP", "DOWN"]
```

### Comparing `restring-0.1.2/restring/settings.py` & `restring-0.1.3/restring/settings.py`

 * *Files identical despite different names*

### Comparing `restring-0.1.2/restring.egg-info/PKG-INFO` & `restring-0.1.3/restring.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restring
-Version: 0.1.2
+Version: 0.1.3
 Summary: Functional enrichment terms aggregator.
 Home-page: https://github.com/Stemanz/restring
 Author: Stefano Manzini
 Author-email: stefano.manzini@gmail.com
 License: GPL-3.0
 Download-URL: https://github.com/Stemanz/restring/archive/master.zip
 Description: # restring
```

### Comparing `restring-0.1.2/setup.py` & `restring-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name="restring",
-    version="0.1.2",
+    version="0.1.3",
     description="Functional enrichment terms aggregator.",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Stefano Manzini",
     author_email="stefano.manzini@gmail.com",
     url="https://github.com/Stemanz/restring",
     download_url="https://github.com/Stemanz/restring/archive/master.zip",
```

