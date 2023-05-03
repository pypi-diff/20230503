# Comparing `tmp/phomemo-p12-tools-0.0.2.tar.gz` & `tmp/phomemo-p12-tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phomemo-p12-tools-0.0.2.tar", last modified: Wed May  3 05:01:35 2023, max compression
+gzip compressed data, was "phomemo-p12-tools-0.0.3.tar", last modified: Wed May  3 05:13:55 2023, max compression
```

## Comparing `phomemo-p12-tools-0.0.2.tar` & `phomemo-p12-tools-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 05:01:35.317466 phomemo-p12-tools-0.0.2/
--rwx------   0 crs       (1000) crs       (1000)     1082 2023-05-01 10:02:31.000000 phomemo-p12-tools-0.0.2/LICENSE
--rw-rw-r--   0 crs       (1000) crs       (1000)     3891 2023-05-03 05:01:35.317466 phomemo-p12-tools-0.0.2/PKG-INFO
--rw-rw-r--   0 crs       (1000) crs       (1000)     2085 2023-05-03 04:03:56.000000 phomemo-p12-tools-0.0.2/README.md
-drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 05:01:35.313466 phomemo-p12-tools-0.0.2/phomemo_p12_tools.egg-info/
--rw-rw-r--   0 crs       (1000) crs       (1000)     3891 2023-05-03 05:01:35.000000 phomemo-p12-tools-0.0.2/phomemo_p12_tools.egg-info/PKG-INFO
--rw-rw-r--   0 crs       (1000) crs       (1000)      611 2023-05-03 05:01:35.000000 phomemo-p12-tools-0.0.2/phomemo_p12_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 crs       (1000) crs       (1000)        1 2023-05-03 05:01:35.000000 phomemo-p12-tools-0.0.2/phomemo_p12_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 crs       (1000) crs       (1000)      110 2023-05-03 05:01:35.000000 phomemo-p12-tools-0.0.2/phomemo_p12_tools.egg-info/entry_points.txt
--rw-rw-r--   0 crs       (1000) crs       (1000)       24 2023-05-03 05:01:35.000000 phomemo-p12-tools-0.0.2/phomemo_p12_tools.egg-info/requires.txt
--rw-rw-r--   0 crs       (1000) crs       (1000)       10 2023-05-03 05:01:35.000000 phomemo-p12-tools-0.0.2/phomemo_p12_tools.egg-info/top_level.txt
--rw-rw-r--   0 crs       (1000) crs       (1000)     3452 2023-05-03 05:01:02.000000 phomemo-p12-tools-0.0.2/phomemo_print_p12.py
--rw-rw-r--   0 crs       (1000) crs       (1000)     3601 2023-05-03 04:06:16.000000 phomemo-p12-tools-0.0.2/phomemo_render_label.py
--rw-rw-r--   0 crs       (1000) crs       (1000)      882 2023-05-03 05:01:23.000000 phomemo-p12-tools-0.0.2/pyproject.toml
--rw-rw-r--   0 crs       (1000) crs       (1000)       47 2023-05-03 04:07:23.000000 phomemo-p12-tools-0.0.2/requirements.txt
--rw-rw-r--   0 crs       (1000) crs       (1000)       38 2023-05-03 05:01:35.317466 phomemo-p12-tools-0.0.2/setup.cfg
-drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 05:01:35.309466 phomemo-p12-tools-0.0.2/venv/
-drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 05:01:35.317466 phomemo-p12-tools-0.0.2/venv/bin/
--rwxrwxr-x   0 crs       (1000) crs       (1000)      614 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.2/venv/bin/rst2html.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      736 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.2/venv/bin/rst2html4.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)     1081 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.2/venv/bin/rst2html5.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      813 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.2/venv/bin/rst2latex.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      636 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.2/venv/bin/rst2man.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      802 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.2/venv/bin/rst2odt.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)     1740 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.2/venv/bin/rst2odt_prepstyles.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      621 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.2/venv/bin/rst2pseudoxml.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      657 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.2/venv/bin/rst2s5.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      893 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.2/venv/bin/rst2xetex.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      622 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.2/venv/bin/rst2xml.py
--rwxrwxr-x   0 crs       (1000) crs       (1000)      690 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.2/venv/bin/rstpep2html.py
+drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 05:13:55.384363 phomemo-p12-tools-0.0.3/
+-rwx------   0 crs       (1000) crs       (1000)     1082 2023-05-01 10:02:31.000000 phomemo-p12-tools-0.0.3/LICENSE
+-rw-rw-r--   0 crs       (1000) crs       (1000)     2451 2023-05-03 05:13:55.384363 phomemo-p12-tools-0.0.3/PKG-INFO
+-rw-rw-r--   0 crs       (1000) crs       (1000)      645 2023-05-03 05:13:30.000000 phomemo-p12-tools-0.0.3/README.md
+drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 05:13:55.380362 phomemo-p12-tools-0.0.3/phomemo_p12_tools.egg-info/
+-rw-rw-r--   0 crs       (1000) crs       (1000)     2451 2023-05-03 05:13:55.000000 phomemo-p12-tools-0.0.3/phomemo_p12_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 crs       (1000) crs       (1000)      611 2023-05-03 05:13:55.000000 phomemo-p12-tools-0.0.3/phomemo_p12_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 crs       (1000) crs       (1000)        1 2023-05-03 05:13:55.000000 phomemo-p12-tools-0.0.3/phomemo_p12_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 crs       (1000) crs       (1000)      110 2023-05-03 05:13:55.000000 phomemo-p12-tools-0.0.3/phomemo_p12_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 crs       (1000) crs       (1000)       24 2023-05-03 05:13:55.000000 phomemo-p12-tools-0.0.3/phomemo_p12_tools.egg-info/requires.txt
+-rw-rw-r--   0 crs       (1000) crs       (1000)       10 2023-05-03 05:13:55.000000 phomemo-p12-tools-0.0.3/phomemo_p12_tools.egg-info/top_level.txt
+-rw-rw-r--   0 crs       (1000) crs       (1000)     3452 2023-05-03 05:01:02.000000 phomemo-p12-tools-0.0.3/phomemo_print_p12.py
+-rw-rw-r--   0 crs       (1000) crs       (1000)     3601 2023-05-03 04:06:16.000000 phomemo-p12-tools-0.0.3/phomemo_render_label.py
+-rw-rw-r--   0 crs       (1000) crs       (1000)      882 2023-05-03 05:13:35.000000 phomemo-p12-tools-0.0.3/pyproject.toml
+-rw-rw-r--   0 crs       (1000) crs       (1000)       47 2023-05-03 04:07:23.000000 phomemo-p12-tools-0.0.3/requirements.txt
+-rw-rw-r--   0 crs       (1000) crs       (1000)       38 2023-05-03 05:13:55.384363 phomemo-p12-tools-0.0.3/setup.cfg
+drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 05:13:55.376362 phomemo-p12-tools-0.0.3/venv/
+drwxrwxr-x   0 crs       (1000) crs       (1000)        0 2023-05-03 05:13:55.380362 phomemo-p12-tools-0.0.3/venv/bin/
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      614 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.3/venv/bin/rst2html.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      736 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.3/venv/bin/rst2html4.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)     1081 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.3/venv/bin/rst2html5.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      813 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.3/venv/bin/rst2latex.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      636 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.3/venv/bin/rst2man.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      802 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.3/venv/bin/rst2odt.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)     1740 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.3/venv/bin/rst2odt_prepstyles.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      621 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.3/venv/bin/rst2pseudoxml.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      657 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.3/venv/bin/rst2s5.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      893 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.3/venv/bin/rst2xetex.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      622 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.3/venv/bin/rst2xml.py
+-rwxrwxr-x   0 crs       (1000) crs       (1000)      690 2023-05-03 04:13:27.000000 phomemo-p12-tools-0.0.3/venv/bin/rstpep2html.py
```

### Comparing `phomemo-p12-tools-0.0.2/LICENSE` & `phomemo-p12-tools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.2/phomemo_p12_tools.egg-info/SOURCES.txt` & `phomemo-p12-tools-0.0.3/phomemo_p12_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.2/phomemo_print_p12.py` & `phomemo-p12-tools-0.0.3/phomemo_print_p12.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.2/phomemo_render_label.py` & `phomemo-p12-tools-0.0.3/phomemo_render_label.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.2/pyproject.toml` & `phomemo-p12-tools-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
-version = "0.0.2"
+version = "0.0.3"
 name = "phomemo-p12-tools"
 description='Phomemo P12 printing tools'
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
 	{name = 'TOKITA Hiroshi', email='tokita.hiroshi@gmail.com'},
 ]
```

### Comparing `phomemo-p12-tools-0.0.2/venv/bin/rst2html.py` & `phomemo-p12-tools-0.0.3/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.2/venv/bin/rst2html4.py` & `phomemo-p12-tools-0.0.3/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.2/venv/bin/rst2html5.py` & `phomemo-p12-tools-0.0.3/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.2/venv/bin/rst2latex.py` & `phomemo-p12-tools-0.0.3/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.2/venv/bin/rst2man.py` & `phomemo-p12-tools-0.0.3/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.2/venv/bin/rst2odt.py` & `phomemo-p12-tools-0.0.3/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.2/venv/bin/rst2odt_prepstyles.py` & `phomemo-p12-tools-0.0.3/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.2/venv/bin/rst2pseudoxml.py` & `phomemo-p12-tools-0.0.3/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.2/venv/bin/rst2s5.py` & `phomemo-p12-tools-0.0.3/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.2/venv/bin/rst2xetex.py` & `phomemo-p12-tools-0.0.3/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.2/venv/bin/rst2xml.py` & `phomemo-p12-tools-0.0.3/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `phomemo-p12-tools-0.0.2/venv/bin/rstpep2html.py` & `phomemo-p12-tools-0.0.3/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

