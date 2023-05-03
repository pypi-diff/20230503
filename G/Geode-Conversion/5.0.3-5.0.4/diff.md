# Comparing `tmp/Geode_Conversion-5.0.3-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Conversion-5.0.4-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 1208903 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      171 b- defN 23-May-03 09:35 geode_conversion/__init__.py
--rw-rw-rw-  2.0 fat      199 b- defN 23-May-03 09:35 geode_conversion/model.py
--rw-rw-rw-  2.0 fat  2394112 b- defN 23-May-03 09:36 geode_conversion/bin/Geode-Conversion_model.dll
--rw-rw-rw-  2.0 fat   150528 b- defN 23-May-03 09:36 geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2048 b- defN 23-May-03 09:36 Geode_Conversion-5.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-03 09:36 Geode_Conversion-5.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-May-03 09:36 Geode_Conversion-5.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      731 b- defN 23-May-03 09:36 Geode_Conversion-5.0.3.dist-info/RECORD
-8 files, 2547906 bytes uncompressed, 1207615 bytes compressed:  52.6%
+Zip file size: 1778276 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       67 b- defN 23-May-03 15:30 geode_conversion/__init__.py
+-rw-r--r--  2.0 unx      192 b- defN 23-May-03 15:30 geode_conversion/model.py
+-rwxr-xr-x  2.0 unx   167448 b- defN 23-May-03 15:30 geode_conversion/lib64/geode_conversion_py_model.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx  4228640 b- defN 23-May-03 15:30 geode_conversion/lib64/libGeode-Conversion_model.so
+-rw-r--r--  2.0 unx     1989 b- defN 23-May-03 15:30 Geode_Conversion-5.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      103 b- defN 23-May-03 15:30 Geode_Conversion-5.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-May-03 15:30 Geode_Conversion-5.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      748 b- defN 23-May-03 15:30 Geode_Conversion-5.0.4.dist-info/RECORD
+8 files, 4399204 bytes uncompressed, 1776952 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: geode_conversion/__init__.py
 Comment: 
 
 Filename: geode_conversion/model.py
 Comment: 
 
-Filename: geode_conversion/bin/Geode-Conversion_model.dll
+Filename: geode_conversion/lib64/geode_conversion_py_model.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd
+Filename: geode_conversion/lib64/libGeode-Conversion_model.so
 Comment: 
 
-Filename: Geode_Conversion-5.0.3.dist-info/METADATA
+Filename: Geode_Conversion-5.0.4.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Conversion-5.0.3.dist-info/WHEEL
+Filename: Geode_Conversion-5.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Conversion-5.0.3.dist-info/top_level.txt
+Filename: Geode_Conversion-5.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Conversion-5.0.3.dist-info/RECORD
+Filename: Geode_Conversion-5.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_conversion/__init__.py

```diff
@@ -1,6 +1,3 @@
-## Copyright (c) 2019 - 2023 Geode-solutions
-
-import os, pathlib
-os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
-
-from .model import *
+## Copyright (c) 2019 - 2023 Geode-solutions
+
+from .model import *
```

## geode_conversion/model.py

```diff
@@ -1,9 +1,9 @@
-#
-# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-
-from .bin.geode_conversion_py_model import *
-ConversionModelLibrary.initialize()
+#
+# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+
+from .lib64.geode_conversion_py_model import *
+ConversionModelLibrary.initialize()
```

## Comparing `Geode_Conversion-5.0.3.dist-info/METADATA` & `Geode_Conversion-5.0.4.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,37 @@
-Metadata-Version: 2.1
-Name: Geode-Conversion
-Version: 5.0.3
-Summary: Conversion module for Geode-solutions OpenGeode modules
-Home-page: https://github.com/Geode-solutions/Geode-Conversion
-Author: Geode-solutions
-Author-email: contact@geode-solutions.com
-License: Proprietary
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Requires-Dist: geode-common (==25.*,>=25.0.0)
-Requires-Dist: opengeode-core (==14.*,>=14.0.0)
-
-<h1 align="center">Geode-Conversion<sup><i>by Geode-solutions</i></sup></h1>
-<h3 align="center">Conversion OpenGeode module</h3>
-
-<p align="center">
-  <img src="https://github.com/Geode-solutions/Geode-Conversion_private/workflows/CI/badge.svg" alt="Build Status">
-  <img src="https://github.com/Geode-solutions/Geode-Conversion_private/workflows/CD/badge.svg" alt="Deploy Status">
-  <img src="https://codecov.io/gh/Geode-solutions/Geode-Conversion_private/branch/master/graph/badge.svg" alt="Coverage Status">
-  <img src="https://img.shields.io/github/release/Geode-solutions/Geode-Conversion_private.svg" alt="Version">
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
-  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
-  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
-  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
-  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
-  <a href="https://opengeode-slack-invite.herokuapp.com">
-    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
-  </a>
-
-Copyright (c) 2019 - 2023, Geode-solutions
-
-
+Metadata-Version: 2.1
+Name: Geode-Conversion
+Version: 5.0.4
+Summary: Conversion module for Geode-solutions OpenGeode modules
+Home-page: https://github.com/Geode-solutions/Geode-Conversion
+Author: Geode-solutions
+Author-email: contact@geode-solutions.com
+License: Proprietary
+Description-Content-Type: text/markdown
+Requires-Dist: geode-common (==25.*,>=25.0.4)
+Requires-Dist: opengeode-core (==14.*,>=14.0.13)
+
+<h1 align="center">Geode-Conversion<sup><i>by Geode-solutions</i></sup></h1>
+<h3 align="center">Conversion OpenGeode module</h3>
+
+<p align="center">
+  <img src="https://github.com/Geode-solutions/Geode-Conversion_private/workflows/CI/badge.svg" alt="Build Status">
+  <img src="https://github.com/Geode-solutions/Geode-Conversion_private/workflows/CD/badge.svg" alt="Deploy Status">
+  <img src="https://codecov.io/gh/Geode-solutions/Geode-Conversion_private/branch/master/graph/badge.svg" alt="Coverage Status">
+  <img src="https://img.shields.io/github/release/Geode-solutions/Geode-Conversion_private.svg" alt="Version">
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
+  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
+  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
+  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
+  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
+  <a href="https://opengeode-slack-invite.herokuapp.com">
+    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
+  </a>
+
+Copyright (c) 2019 - 2023, Geode-solutions
```

### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: Geode-Conversion Version: 5.0.3 Summary: Conversion
+Metadata-Version: 2.1 Name: Geode-Conversion Version: 5.0.4 Summary: Conversion
 module for Geode-solutions OpenGeode modules Home-page: https://github.com/
 Geode-solutions/Geode-Conversion Author: Geode-solutions Author-email:
-contact@geode-solutions.com License: Proprietary Platform: UNKNOWN Description-
-Content-Type: text/markdown Requires-Dist: geode-common (==25.*,>=25.0.0)
-Requires-Dist: opengeode-core (==14.*,>=14.0.0)
+contact@geode-solutions.com License: Proprietary Description-Content-Type:
+text/markdown Requires-Dist: geode-common (==25.*,>=25.0.4) Requires-Dist:
+opengeode-core (==14.*,>=14.0.13)
                ****** Geode-Conversionby Geode-solutions ******
                      **** Conversion OpenGeode module ****
           [Build Status] [Deploy Status] [Coverage Status] [Version]
              [Windows support] [Ubuntu support] [Red Hat support]
   [Language] [License] [Semantic-release] [Slack_invite] Copyright (c) 2019 -
                             2023, Geode-solutions
```

## Comparing `Geode_Conversion-5.0.3.dist-info/RECORD` & `Geode_Conversion-5.0.4.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-geode_conversion/__init__.py,sha256=Ia-ZwhIAokDIC6uBDumiY-s6IwjLi8gNTQti1qPYKh4,171
-geode_conversion/model.py,sha256=MpZUv0-CJnUn1nVI6aRk2bGV-KxpGEobD7p1oNwSaV4,199
-geode_conversion/bin/Geode-Conversion_model.dll,sha256=mdWbxqHsYqjyo734PXHsEmXV0cwhU2V4nROqNVixBCQ,2394112
-geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd,sha256=_8FAH8JdEGBVYTcw355U0LwjkhQwlyZX8nfRFdwO8Ns,150528
-Geode_Conversion-5.0.3.dist-info/METADATA,sha256=HwdpPXsvw8MbGiPBRNXJwRBzokHfn7rhFO5ycTIuhhs,2048
-Geode_Conversion-5.0.3.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-Geode_Conversion-5.0.3.dist-info/top_level.txt,sha256=PnM_M6Sy8psC1M_rMpCs6FAGjv7uyDWsRvR46jFUpXU,17
-Geode_Conversion-5.0.3.dist-info/RECORD,,
+geode_conversion/__init__.py,sha256=gQGhP_A2S1Wn3Ap6ta75b9bQ3sMwtuA7Jc1YXvGVuIQ,67
+geode_conversion/model.py,sha256=wlwMAz7sGIPtoLnT2AdYmTqbMv5EpRAYQQLePwctbd8,192
+geode_conversion/lib64/geode_conversion_py_model.cpython-39-x86_64-linux-gnu.so,sha256=11JCmdN7bni5V6JW7rj4Qq-hfl7XhSUQTBBr2JAHTMM,167448
+geode_conversion/lib64/libGeode-Conversion_model.so,sha256=pqj0x6C-SynV6i-yonKLZIEpJNHanuO6JrcwSQtauJE,4228640
+Geode_Conversion-5.0.4.dist-info/METADATA,sha256=zkixK71z30chueI-vSyhbfMvdIp8uC4i5Cn9lyaKGps,1989
+Geode_Conversion-5.0.4.dist-info/WHEEL,sha256=3s2LSuQQhT9U1Dyv6MxBd72puf_ocSkY6hn5h0Kjf-o,103
+Geode_Conversion-5.0.4.dist-info/top_level.txt,sha256=PnM_M6Sy8psC1M_rMpCs6FAGjv7uyDWsRvR46jFUpXU,17
+Geode_Conversion-5.0.4.dist-info/RECORD,,
```

