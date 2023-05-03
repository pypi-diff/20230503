# Comparing `tmp/phomemo-p12-tools-0.0.4.tar.gz` & `tmp/phomemo-p12-tools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phomemo-p12-tools-0.0.4.tar", last modified: Wed May  3 05:56:04 2023, max compression
+gzip compressed data, was "phomemo-p12-tools-0.0.5.tar", last modified: Wed May  3 06:03:05 2023, max compression
```

## Comparing `phomemo-p12-tools-0.0.4.tar` & `phomemo-p12-tools-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 05:56:04.848873 phomemo-p12-tools-0.0.4/
--rwx------   0 crs       (1000) crs       (1000)     1082 2023-05-01 10:02:31.000000 phomemo-p12-tools-0.0.4/LICENSE
--rw-rw-r--   0 crs       (1000) crs       (1000)     2570 2023-05-03 05:56:04.844873 phomemo-p12-tools-0.0.4/PKG-INFO
--rw-rw-r--   0 crs       (1000) crs       (1000)      764 2023-05-03 05:55:47.000000 phomemo-p12-tools-0.0.4/README.md
-drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 05:56:04.836872 phomemo-p12-tools-0.0.4/phomemo/
--rw-rw-r--   0 crs       (1000) crs       (1000)        0 2023-05-03 05:38:49.000000 phomemo-p12-tools-0.0.4/phomemo/__init__.py
--rw-rw-r--   0 crs       (1000) crs       (1000)     3452 2023-05-03 05:55:47.000000 phomemo-p12-tools-0.0.4/phomemo/print_p12.py
--rw-rw-r--   0 crs       (1000) crs       (1000)     3601 2023-05-03 05:55:47.000000 phomemo-p12-tools-0.0.4/phomemo/render_label.py
-drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 05:56:04.844873 phomemo-p12-tools-0.0.4/phomemo_p12_tools.egg-info/
--rw-rw-r--   0 crs       (1000) crs       (1000)     2570 2023-05-03 05:56:04.000000 phomemo-p12-tools-0.0.4/phomemo_p12_tools.egg-info/PKG-INFO
--rw-rw-r--   0 crs       (1000) crs       (1000)      631 2023-05-03 05:56:04.000000 phomemo-p12-tools-0.0.4/phomemo_p12_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 crs       (1000) crs       (1000)        1 2023-05-03 05:56:04.000000 phomemo-p12-tools-0.0.4/phomemo_p12_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 crs       (1000) crs       (1000)      110 2023-05-03 05:56:04.000000 phomemo-p12-tools-0.0.4/phomemo_p12_tools.egg-info/entry_points.txt
--rw-rw-r--   0 crs       (1000) crs       (1000)       24 2023-05-03 05:56:04.000000 phomemo-p12-tools-0.0.4/phomemo_p12_tools.egg-info/requires.txt
--rw-rw-r--   0 crs       (1000) crs       (1000)       18 2023-05-03 05:56:04.000000 phomemo-p12-tools-0.0.4/phomemo_p12_tools.egg-info/top_level.txt
--rw-rw-r--   0 crs       (1000) crs       (1000)      882 2023-05-03 05:55:47.000000 phomemo-p12-tools-0.0.4/pyproject.toml
--rw-rw-r--   0 crs       (1000) crs       (1000)       47 2023-05-03 04:07:23.000000 phomemo-p12-tools-0.0.4/requirements.txt
--rw-rw-r--   0 crs       (1000) crs       (1000)       38 2023-05-03 05:56:04.848873 phomemo-p12-tools-0.0.4/setup.cfg
-drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 05:56:04.836872 phomemo-p12-tools-0.0.4/venv/
-drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 05:56:04.844873 phomemo-p12-tools-0.0.4/venv/bin/
--rwxrwxr-x   0 crs       (1000) crs       (1000)      614 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.4/venv/bin/rst2html.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      736 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.4/venv/bin/rst2html4.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)     1081 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.4/venv/bin/rst2html5.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      813 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.4/venv/bin/rst2latex.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      636 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.4/venv/bin/rst2man.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      802 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.4/venv/bin/rst2odt.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)     1740 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.4/venv/bin/rst2odt_prepstyles.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      621 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.4/venv/bin/rst2pseudoxml.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      657 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.4/venv/bin/rst2s5.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      893 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.4/venv/bin/rst2xetex.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      622 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.4/venv/bin/rst2xml.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      690 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.4/venv/bin/rstpep2html.py
+drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 06:03:05.688773 phomemo-p12-tools-0.0.5/
+-rwx------   0 crs       (1000) crs       (1000)     1082 2023-05-01 10:02:31.000000 phomemo-p12-tools-0.0.5/LICENSE
+-rw-rw-r--   0 crs       (1000) crs       (1000)     2558 2023-05-03 06:03:05.688773 phomemo-p12-tools-0.0.5/PKG-INFO
+-rw-rw-r--   0 crs       (1000) crs       (1000)      752 2023-05-03 06:02:31.000000 phomemo-p12-tools-0.0.5/README.md
+drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 06:03:05.680773 phomemo-p12-tools-0.0.5/phomemo/
+-rw-rw-r--   0 crs       (1000) crs       (1000)        0 2023-05-03 05:38:49.000000 phomemo-p12-tools-0.0.5/phomemo/__init__.py
+-rw-rw-r--   0 crs       (1000) crs       (1000)     3452 2023-05-03 05:55:47.000000 phomemo-p12-tools-0.0.5/phomemo/print_p12.py
+-rw-rw-r--   0 crs       (1000) crs       (1000)     3601 2023-05-03 05:55:47.000000 phomemo-p12-tools-0.0.5/phomemo/render_label.py
+drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 06:03:05.680773 phomemo-p12-tools-0.0.5/phomemo_p12_tools.egg-info/
+-rw-rw-r--   0 crs       (1000) crs       (1000)     2558 2023-05-03 06:03:05.000000 phomemo-p12-tools-0.0.5/phomemo_p12_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 crs       (1000) crs       (1000)      631 2023-05-03 06:03:05.000000 phomemo-p12-tools-0.0.5/phomemo_p12_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 crs       (1000) crs       (1000)        1 2023-05-03 06:03:05.000000 phomemo-p12-tools-0.0.5/phomemo_p12_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 crs       (1000) crs       (1000)      110 2023-05-03 06:03:05.000000 phomemo-p12-tools-0.0.5/phomemo_p12_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 crs       (1000) crs       (1000)       24 2023-05-03 06:03:05.000000 phomemo-p12-tools-0.0.5/phomemo_p12_tools.egg-info/requires.txt
+-rw-rw-r--   0 crs       (1000) crs       (1000)       18 2023-05-03 06:03:05.000000 phomemo-p12-tools-0.0.5/phomemo_p12_tools.egg-info/top_level.txt
+-rw-rw-r--   0 crs       (1000) crs       (1000)      882 2023-05-03 06:02:41.000000 phomemo-p12-tools-0.0.5/pyproject.toml
+-rw-rw-r--   0 crs       (1000) crs       (1000)       47 2023-05-03 04:07:23.000000 phomemo-p12-tools-0.0.5/requirements.txt
+-rw-rw-r--   0 crs       (1000) crs       (1000)       38 2023-05-03 06:03:05.688773 phomemo-p12-tools-0.0.5/setup.cfg
+drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 06:03:05.680773 phomemo-p12-tools-0.0.5/venv/
+drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 06:03:05.688773 phomemo-p12-tools-0.0.5/venv/bin/
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      614 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.5/venv/bin/rst2html.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      736 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.5/venv/bin/rst2html4.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)     1081 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.5/venv/bin/rst2html5.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      813 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.5/venv/bin/rst2latex.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      636 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.5/venv/bin/rst2man.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      802 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.5/venv/bin/rst2odt.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)     1740 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.5/venv/bin/rst2odt_prepstyles.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      621 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.5/venv/bin/rst2pseudoxml.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      657 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.5/venv/bin/rst2s5.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      893 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.5/venv/bin/rst2xetex.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      622 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.5/venv/bin/rst2xml.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      690 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.5/venv/bin/rstpep2html.py
```

### Comparing `phomemo-p12-tools-0.0.4/LICENSE` & `phomemo-p12-tools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.4/PKG-INFO` & `phomemo-p12-tools-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phomemo-p12-tools
-Version: 0.0.4
+Version: 0.0.5
 Summary: Phomemo P12 printing tools
 Author-email: TOKITA Hiroshi <tokita.hiroshi@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Timo 'polskafan' Dobbrick
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,31 +40,31 @@
 # Acknowledgements
 Based on [phomemo_d30](https://github.com/polskafan/phomemo_d30) by polskafan,
 [phomemo-tools](https://github.com/vivier/phomemo-tools) by Laurent Vivier and
 [phomemo_m02s](https://github.com/theacodes/phomemo_m02s) by theacodes.
 
 # Checkout and install
 ```bash
-venv/bin/pip install phomemo-p12-tool
+pip3 install phomemo-p12-tools
 ```
 
-# Usage
+# Setup
 Connect to printer with rfcomm
 
 ```bash
 sudo rfcomm connect 1 XX:XX:XX:XX:XX:XX
 ```
 
 Or windows, connect to P12 by 'Bluetooth & device' menu.
 
-Basic usage
+# Usage
+
 ```bash
 phomemo_render_label "Hello world!" | phomemo_print_p12 --port=[device]
 ```
 
-Or windows, 
+Or windows,
 
 ```cmd
 phomemo_render_label "Hello world!" > label.pbm
 phomemo_print_p12 --port=[device] label.pbm
 ```
-
```

### Comparing `phomemo-p12-tools-0.0.4/phomemo/print_p12.py` & `phomemo-p12-tools-0.0.5/phomemo/print_p12.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.4/phomemo/render_label.py` & `phomemo-p12-tools-0.0.5/phomemo/render_label.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.4/phomemo_p12_tools.egg-info/PKG-INFO` & `phomemo-p12-tools-0.0.5/phomemo_p12_tools.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phomemo-p12-tools
-Version: 0.0.4
+Version: 0.0.5
 Summary: Phomemo P12 printing tools
 Author-email: TOKITA Hiroshi <tokita.hiroshi@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Timo 'polskafan' Dobbrick
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,31 +40,31 @@
 # Acknowledgements
 Based on [phomemo_d30](https://github.com/polskafan/phomemo_d30) by polskafan,
 [phomemo-tools](https://github.com/vivier/phomemo-tools) by Laurent Vivier and
 [phomemo_m02s](https://github.com/theacodes/phomemo_m02s) by theacodes.
 
 # Checkout and install
 ```bash
-venv/bin/pip install phomemo-p12-tool
+pip3 install phomemo-p12-tools
 ```
 
-# Usage
+# Setup
 Connect to printer with rfcomm
 
 ```bash
 sudo rfcomm connect 1 XX:XX:XX:XX:XX:XX
 ```
 
 Or windows, connect to P12 by 'Bluetooth & device' menu.
 
-Basic usage
+# Usage
+
 ```bash
 phomemo_render_label "Hello world!" | phomemo_print_p12 --port=[device]
 ```
 
-Or windows, 
+Or windows,
 
 ```cmd
 phomemo_render_label "Hello world!" > label.pbm
 phomemo_print_p12 --port=[device] label.pbm
 ```
-
```

### Comparing `phomemo-p12-tools-0.0.4/phomemo_p12_tools.egg-info/SOURCES.txt` & `phomemo-p12-tools-0.0.5/phomemo_p12_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.4/pyproject.toml` & `phomemo-p12-tools-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
-version = "0.0.4"
+version = "0.0.5"
 name = "phomemo-p12-tools"
 description='Phomemo P12 printing tools'
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
 	{name = 'TOKITA Hiroshi', email='tokita.hiroshi@gmail.com'},
 ]
```

### Comparing `phomemo-p12-tools-0.0.4/venv/bin/rst2html.py` & `phomemo-p12-tools-0.0.5/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.4/venv/bin/rst2html4.py` & `phomemo-p12-tools-0.0.5/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.4/venv/bin/rst2html5.py` & `phomemo-p12-tools-0.0.5/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.4/venv/bin/rst2latex.py` & `phomemo-p12-tools-0.0.5/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.4/venv/bin/rst2man.py` & `phomemo-p12-tools-0.0.5/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.4/venv/bin/rst2odt.py` & `phomemo-p12-tools-0.0.5/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.4/venv/bin/rst2odt_prepstyles.py` & `phomemo-p12-tools-0.0.5/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.4/venv/bin/rst2pseudoxml.py` & `phomemo-p12-tools-0.0.5/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.4/venv/bin/rst2s5.py` & `phomemo-p12-tools-0.0.5/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.4/venv/bin/rst2xetex.py` & `phomemo-p12-tools-0.0.5/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.4/venv/bin/rst2xml.py` & `phomemo-p12-tools-0.0.5/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.4/venv/bin/rstpep2html.py` & `phomemo-p12-tools-0.0.5/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

