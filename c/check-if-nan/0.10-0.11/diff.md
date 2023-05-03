# Comparing `tmp/check_if_nan-0.10.tar.gz` & `tmp/check_if_nan-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "check_if_nan-0.10.tar", last modified: Tue Dec 27 22:21:22 2022, max compression
+gzip compressed data, was "check_if_nan-0.11.tar", last modified: Wed May  3 00:50:42 2023, max compression
```

## Comparing `check_if_nan-0.10.tar` & `check_if_nan-0.11.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-12-27 22:21:22.987669 check_if_nan-0.10/
--rw-rw-rw-   0        0        0     1148 2022-12-27 22:21:15.000000 check_if_nan-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      137 2022-12-27 22:21:14.000000 check_if_nan-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     3867 2022-12-27 22:21:22.987669 check_if_nan-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     2824 2022-12-27 22:19:16.000000 check_if_nan-0.10/README.md
-drwxrwxrwx   0        0        0        0 2022-12-27 22:21:22.983679 check_if_nan-0.10/check_if_nan/
--rw-rw-rw-   0        0        0     1069 2022-10-02 04:27:48.000000 check_if_nan-0.10/check_if_nan/LICENSE
--rw-rw-rw-   0        0        0     2824 2022-12-27 22:19:16.000000 check_if_nan-0.10/check_if_nan/README.MD
--rw-rw-rw-   0        0        0     4117 2022-12-27 22:16:24.000000 check_if_nan-0.10/check_if_nan/__init__.py
--rw-rw-rw-   0        0        0       31 2022-12-27 22:21:21.000000 check_if_nan-0.10/check_if_nan/requirements.txt
--rw-rw-rw-   0        0        0        2 2022-12-27 22:21:21.000000 check_if_nan-0.10/check_if_nan/thirdparty.json
-drwxrwxrwx   0        0        0        0 2022-12-27 22:21:22.986671 check_if_nan-0.10/check_if_nan.egg-info/
--rw-rw-rw-   0        0        0     3867 2022-12-27 22:21:22.000000 check_if_nan-0.10/check_if_nan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      359 2022-12-27 22:21:22.000000 check_if_nan-0.10/check_if_nan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-27 22:21:22.000000 check_if_nan-0.10/check_if_nan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2022-12-27 22:21:22.000000 check_if_nan-0.10/check_if_nan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-12-27 22:21:22.000000 check_if_nan-0.10/check_if_nan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2022-12-27 22:21:22.987669 check_if_nan-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1460 2022-12-27 22:21:21.000000 check_if_nan-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 00:50:42.531309 check_if_nan-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-05-03 00:50:35.000000 check_if_nan-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      137 2023-05-03 00:50:34.000000 check_if_nan-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     3600 2023-05-03 00:50:42.531309 check_if_nan-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     2824 2023-04-15 00:18:30.000000 check_if_nan-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 00:50:42.529298 check_if_nan-0.11/check_if_nan/
+-rw-rw-rw-   0        0        0     1069 2023-04-15 00:18:30.000000 check_if_nan-0.11/check_if_nan/LICENSE
+-rw-rw-rw-   0        0        0     2824 2023-04-15 00:18:30.000000 check_if_nan-0.11/check_if_nan/README.MD
+-rw-rw-rw-   0        0        0     4212 2023-05-03 00:48:23.000000 check_if_nan-0.11/check_if_nan/__init__.py
+-rw-rw-rw-   0        0        0       31 2023-05-03 00:50:41.000000 check_if_nan-0.11/check_if_nan/requirements.txt
+-rw-rw-rw-   0        0        0    50847 2023-05-03 00:50:41.000000 check_if_nan-0.11/check_if_nan/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-05-03 00:50:42.531309 check_if_nan-0.11/check_if_nan.egg-info/
+-rw-rw-rw-   0        0        0     3600 2023-05-03 00:50:42.000000 check_if_nan-0.11/check_if_nan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2023-05-03 00:50:42.000000 check_if_nan-0.11/check_if_nan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 00:50:42.000000 check_if_nan-0.11/check_if_nan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-03 00:50:42.000000 check_if_nan-0.11/check_if_nan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-03 00:50:42.000000 check_if_nan-0.11/check_if_nan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-05-03 00:50:42.531309 check_if_nan-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1376 2023-05-03 00:50:41.000000 check_if_nan-0.11/setup.py
```

### Comparing `check_if_nan-0.10/LICENSE.rst` & `check_if_nan-0.11/LICENSE.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
  The MIT License (MIT)
- Copyright (c) 2022 Johannes Fischer
+ Copyright (c) 2023 Johannes Fischer
  
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  copies of the Software, and to permit persons to whom the Software is
  furnished to do so, subject to the following conditions:
```

### Comparing `check_if_nan-0.10/PKG-INFO` & `check_if_nan-0.11/check_if_nan.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 Metadata-Version: 2.1
-Name: check_if_nan
-Version: 0.10
+Name: check-if-nan
+Version: 0.11
 Summary: Checks for all kinds of nan/None values without raising Exceptions all the time
 Home-page: https://github.com/hansalemaos/check_if_nan
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: nan,None
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Editors :: Text Processing
-Classifier: Topic :: Text Processing :: General
-Classifier: Topic :: Text Processing :: Indexing
-Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
-
 # Checks for all kinds of nan/None values without raising Exceptions all the time
 
 
 ```python
 from check_if_nan import is_nan,sort_nan_non_nan
 import numpy as np
 import pandas as pd
```

### Comparing `check_if_nan-0.10/README.md` & `check_if_nan-0.11/README.md`

 * *Files identical despite different names*

### Comparing `check_if_nan-0.10/check_if_nan/LICENSE` & `check_if_nan-0.11/check_if_nan/LICENSE`

 * *Files identical despite different names*

### Comparing `check_if_nan-0.10/check_if_nan/README.MD` & `check_if_nan-0.11/check_if_nan/README.MD`

 * *Files identical despite different names*

### Comparing `check_if_nan-0.10/check_if_nan/__init__.py` & `check_if_nan-0.11/check_if_nan/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from disable_warnings import *
 from typing import Any
-from collections import defaultdict, Iterable
+from collections import defaultdict
+try:
+    from collections import Iterable
+except Exception:
+    from collections.abc import Iterable
 from functools import reduce
 import numpy as np
 import pandas as pd
 import math
 
 
 def checkiter(x):
```

### Comparing `check_if_nan-0.10/check_if_nan.egg-info/PKG-INFO` & `check_if_nan-0.11/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 Metadata-Version: 2.1
-Name: check-if-nan
-Version: 0.10
+Name: check_if_nan
+Version: 0.11
 Summary: Checks for all kinds of nan/None values without raising Exceptions all the time
 Home-page: https://github.com/hansalemaos/check_if_nan
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: nan,None
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Editors :: Text Processing
-Classifier: Topic :: Text Processing :: General
-Classifier: Topic :: Text Processing :: Indexing
-Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
-
 # Checks for all kinds of nan/None values without raising Exceptions all the time
 
 
 ```python
 from check_if_nan import is_nan,sort_nan_non_nan
 import numpy as np
 import pandas as pd
```

