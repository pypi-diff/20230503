# Comparing `tmp/phomemo-p12-tools-0.0.1.tar.gz` & `tmp/phomemo-p12-tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phomemo-p12-tools-0.0.1.tar", last modified: Wed May  3 04:46:01 2023, max compression
+gzip compressed data, was "phomemo-p12-tools-0.0.2.tar", last modified: Wed May  3 05:01:35 2023, max compression
```

## Comparing `phomemo-p12-tools-0.0.1.tar` & `phomemo-p12-tools-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 04:46:01.747545 phomemo-p12-tools-0.0.1/
--rwx------   0 crs       (1000) crs       (1000)     1082 2023-05-01 10:02:31.000000 phomemo-p12-tools-0.0.1/LICENSE
--rw-rw-r--   0 crs       (1000) crs       (1000)     3891 2023-05-03 04:46:01.747545 phomemo-p12-tools-0.0.1/PKG-INFO
--rw-rw-r--   0 crs       (1000) crs       (1000)     2085 2023-05-03 04:03:56.000000 phomemo-p12-tools-0.0.1/README.md
-drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 04:46:01.743545 phomemo-p12-tools-0.0.1/phomemo_p12_tools.egg-info/
--rw-rw-r--   0 crs       (1000) crs       (1000)     3891 2023-05-03 04:46:01.000000 phomemo-p12-tools-0.0.1/phomemo_p12_tools.egg-info/PKG-INFO
--rw-rw-r--   0 crs       (1000) crs       (1000)      611 2023-05-03 04:46:01.000000 phomemo-p12-tools-0.0.1/phomemo_p12_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 crs       (1000) crs       (1000)        1 2023-05-03 04:46:01.000000 phomemo-p12-tools-0.0.1/phomemo_p12_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 crs       (1000) crs       (1000)      110 2023-05-03 04:46:01.000000 phomemo-p12-tools-0.0.1/phomemo_p12_tools.egg-info/entry_points.txt
--rw-rw-r--   0 crs       (1000) crs       (1000)       22 2023-05-03 04:46:01.000000 phomemo-p12-tools-0.0.1/phomemo_p12_tools.egg-info/requires.txt
--rw-rw-r--   0 crs       (1000) crs       (1000)       10 2023-05-03 04:46:01.000000 phomemo-p12-tools-0.0.1/phomemo_p12_tools.egg-info/top_level.txt
--rw-rw-r--   0 crs       (1000) crs       (1000)     3432 2023-05-03 04:06:16.000000 phomemo-p12-tools-0.0.1/phomemo_print_p12.py
--rw-rw-r--   0 crs       (1000) crs       (1000)     3601 2023-05-03 04:06:16.000000 phomemo-p12-tools-0.0.1/phomemo_render_label.py
--rw-rw-r--   0 crs       (1000) crs       (1000)      880 2023-05-03 04:44:58.000000 phomemo-p12-tools-0.0.1/pyproject.toml
--rw-rw-r--   0 crs       (1000) crs       (1000)       47 2023-05-03 04:07:23.000000 phomemo-p12-tools-0.0.1/requirements.txt
--rw-rw-r--   0 crs       (1000) crs       (1000)       38 2023-05-03 04:46:01.747545 phomemo-p12-tools-0.0.1/setup.cfg
-drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 04:46:01.739545 phomemo-p12-tools-0.0.1/venv/
-drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 04:46:01.747545 phomemo-p12-tools-0.0.1/venv/bin/
--rwxrwxr-x   0 crs       (1000) crs       (1000)      614 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.1/venv/bin/rst2html.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      736 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.1/venv/bin/rst2html4.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)     1081 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.1/venv/bin/rst2html5.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      813 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.1/venv/bin/rst2latex.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      636 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.1/venv/bin/rst2man.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      802 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.1/venv/bin/rst2odt.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)     1740 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.1/venv/bin/rst2odt_prepstyles.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      621 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.1/venv/bin/rst2pseudoxml.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      657 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.1/venv/bin/rst2s5.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      893 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.1/venv/bin/rst2xetex.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      622 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.1/venv/bin/rst2xml.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      690 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.1/venv/bin/rstpep2html.py
+drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 05:01:35.317466 phomemo-p12-tools-0.0.2/
+-rwx------   0 crs       (1000) crs       (1000)     1082 2023-05-01 10:02:31.000000 phomemo-p12-tools-0.0.2/LICENSE
+-rw-rw-r--   0 crs       (1000) crs       (1000)     3891 2023-05-03 05:01:35.317466 phomemo-p12-tools-0.0.2/PKG-INFO
+-rw-rw-r--   0 crs       (1000) crs       (1000)     2085 2023-05-03 04:03:56.000000 phomemo-p12-tools-0.0.2/README.md
+drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 05:01:35.313466 phomemo-p12-tools-0.0.2/phomemo_p12_tools.egg-info/
+-rw-rw-r--   0 crs       (1000) crs       (1000)     3891 2023-05-03 05:01:35.000000 phomemo-p12-tools-0.0.2/phomemo_p12_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 crs       (1000) crs       (1000)      611 2023-05-03 05:01:35.000000 phomemo-p12-tools-0.0.2/phomemo_p12_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 crs       (1000) crs       (1000)        1 2023-05-03 05:01:35.000000 phomemo-p12-tools-0.0.2/phomemo_p12_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 crs       (1000) crs       (1000)      110 2023-05-03 05:01:35.000000 phomemo-p12-tools-0.0.2/phomemo_p12_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 crs       (1000) crs       (1000)       24 2023-05-03 05:01:35.000000 phomemo-p12-tools-0.0.2/phomemo_p12_tools.egg-info/requires.txt
+-rw-rw-r--   0 crs       (1000) crs       (1000)       10 2023-05-03 05:01:35.000000 phomemo-p12-tools-0.0.2/phomemo_p12_tools.egg-info/top_level.txt
+-rw-rw-r--   0 crs       (1000) crs       (1000)     3452 2023-05-03 05:01:02.000000 phomemo-p12-tools-0.0.2/phomemo_print_p12.py
+-rw-rw-r--   0 crs       (1000) crs       (1000)     3601 2023-05-03 04:06:16.000000 phomemo-p12-tools-0.0.2/phomemo_render_label.py
+-rw-rw-r--   0 crs       (1000) crs       (1000)      882 2023-05-03 05:01:23.000000 phomemo-p12-tools-0.0.2/pyproject.toml
+-rw-rw-r--   0 crs       (1000) crs       (1000)       47 2023-05-03 04:07:23.000000 phomemo-p12-tools-0.0.2/requirements.txt
+-rw-rw-r--   0 crs       (1000) crs       (1000)       38 2023-05-03 05:01:35.317466 phomemo-p12-tools-0.0.2/setup.cfg
+drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 05:01:35.309466 phomemo-p12-tools-0.0.2/venv/
+drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 05:01:35.317466 phomemo-p12-tools-0.0.2/venv/bin/
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      614 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.2/venv/bin/rst2html.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      736 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.2/venv/bin/rst2html4.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)     1081 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.2/venv/bin/rst2html5.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      813 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.2/venv/bin/rst2latex.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      636 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.2/venv/bin/rst2man.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      802 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.2/venv/bin/rst2odt.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)     1740 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.2/venv/bin/rst2odt_prepstyles.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      621 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.2/venv/bin/rst2pseudoxml.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      657 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.2/venv/bin/rst2s5.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      893 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.2/venv/bin/rst2xetex.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      622 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.2/venv/bin/rst2xml.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      690 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.2/venv/bin/rstpep2html.py
```

### Comparing `phomemo-p12-tools-0.0.1/LICENSE` & `phomemo-p12-tools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.1/PKG-INFO` & `phomemo-p12-tools-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phomemo-p12-tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Phomemo P12 printing tools
 Author-email: TOKITA Hiroshi <tokita.hiroshi@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Timo 'polskafan' Dobbrick
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phomemo-p12-tools Version: 0.0.1 Summary: Phomemo
+Metadata-Version: 2.1 Name: phomemo-p12-tools Version: 0.0.2 Summary: Phomemo
 P12 printing tools Author-email: TOKITA Hiroshi
 hiroshi@gmail.com> License: MIT License Copyright (c) 2022 Timo 'polskafan'
 Dobbrick Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
```

### Comparing `phomemo-p12-tools-0.0.1/README.md` & `phomemo-p12-tools-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.1/phomemo_p12_tools.egg-info/PKG-INFO` & `phomemo-p12-tools-0.0.2/phomemo_p12_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phomemo-p12-tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Phomemo P12 printing tools
 Author-email: TOKITA Hiroshi <tokita.hiroshi@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Timo 'polskafan' Dobbrick
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phomemo-p12-tools Version: 0.0.1 Summary: Phomemo
+Metadata-Version: 2.1 Name: phomemo-p12-tools Version: 0.0.2 Summary: Phomemo
 P12 printing tools Author-email: TOKITA Hiroshi
 hiroshi@gmail.com> License: MIT License Copyright (c) 2022 Timo 'polskafan'
 Dobbrick Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
```

### Comparing `phomemo-p12-tools-0.0.1/phomemo_p12_tools.egg-info/SOURCES.txt` & `phomemo-p12-tools-0.0.2/phomemo_p12_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.1/phomemo_print_p12.py` & `phomemo-p12-tools-0.0.2/phomemo_print_p12.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import argparse
 import sys
 import io
 import binascii
 
 import serial
 import PIL.Image
+import PIL.ImageOps
 
 class DummySerial:
     def __init__(self, w):
         self.width = int(w/8)
 
     def write(self, x):
         with io.BytesIO(x) as bstrm:
```

### Comparing `phomemo-p12-tools-0.0.1/phomemo_render_label.py` & `phomemo-p12-tools-0.0.2/phomemo_render_label.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.1/pyproject.toml` & `phomemo-p12-tools-0.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
-version = "0.0.1"
+version = "0.0.2"
 name = "phomemo-p12-tools"
 description='Phomemo P12 printing tools'
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
 	{name = 'TOKITA Hiroshi', email='tokita.hiroshi@gmail.com'},
 ]
@@ -16,15 +16,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: System :: Hardware :: Hardware Drivers"
 ]
 dependencies = [
     "Pillow",
     "pycairo",
-    "serial",
+    "pyserial",
 ]
 
 [project.urls]
 homepage='https://github.com/soburi/phomemo-p12'
 repository='https://github.com/soburi/phomemo-p12'
 
 [project.scripts]
```

### Comparing `phomemo-p12-tools-0.0.1/venv/bin/rst2html.py` & `phomemo-p12-tools-0.0.2/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.1/venv/bin/rst2html4.py` & `phomemo-p12-tools-0.0.2/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.1/venv/bin/rst2html5.py` & `phomemo-p12-tools-0.0.2/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.1/venv/bin/rst2latex.py` & `phomemo-p12-tools-0.0.2/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.1/venv/bin/rst2man.py` & `phomemo-p12-tools-0.0.2/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.1/venv/bin/rst2odt.py` & `phomemo-p12-tools-0.0.2/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.1/venv/bin/rst2odt_prepstyles.py` & `phomemo-p12-tools-0.0.2/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.1/venv/bin/rst2pseudoxml.py` & `phomemo-p12-tools-0.0.2/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.1/venv/bin/rst2s5.py` & `phomemo-p12-tools-0.0.2/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.1/venv/bin/rst2xetex.py` & `phomemo-p12-tools-0.0.2/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.1/venv/bin/rst2xml.py` & `phomemo-p12-tools-0.0.2/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.1/venv/bin/rstpep2html.py` & `phomemo-p12-tools-0.0.2/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

