# Comparing `tmp/MKN_third_codes-0.6.5.1.tar.gz` & `tmp/MKN_third_codes-0.6.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN_third_codes-0.6.5.1.tar", last modified: Wed May  3 09:42:16 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.6.5.2.tar", last modified: Wed May  3 09:48:06 2023, max compression
```

## Comparing `MKN_third_codes-0.6.5.1.tar` & `MKN_third_codes-0.6.5.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 09:42:16.820560 MKN_third_codes-0.6.5.1/
--rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.6.5.1/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.6.5.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-03 09:42:16.810586 MKN_third_codes-0.6.5.1/MKN_third_codes/
--rw-rw-rw-   0        0        0      683 2023-05-03 07:35:48.000000 MKN_third_codes-0.6.5.1/MKN_third_codes/mkn_globals.py
--rw-rw-rw-   0        0        0     9636 2023-05-03 09:36:24.000000 MKN_third_codes-0.6.5.1/MKN_third_codes/mkn_utils.py
--rw-rw-rw-   0        0        0    27856 2023-05-03 09:41:53.000000 MKN_third_codes-0.6.5.1/MKN_third_codes/solutions.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:42:16.819562 MKN_third_codes-0.6.5.1/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0     7700 2023-05-03 09:42:16.000000 MKN_third_codes-0.6.5.1/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-05-03 09:42:16.000000 MKN_third_codes-0.6.5.1/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 09:42:16.000000 MKN_third_codes-0.6.5.1/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-03 09:42:16.000000 MKN_third_codes-0.6.5.1/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7700 2023-05-03 09:42:16.820560 MKN_third_codes-0.6.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     4287 2023-05-03 09:37:41.000000 MKN_third_codes-0.6.5.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-03 09:42:16.820560 MKN_third_codes-0.6.5.1/setup.cfg
--rw-rw-rw-   0        0        0      505 2023-05-03 09:41:57.000000 MKN_third_codes-0.6.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:06.820076 MKN_third_codes-0.6.5.2/
+-rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.6.5.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.6.5.2/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:06.806112 MKN_third_codes-0.6.5.2/MKN_third_codes/
+-rw-rw-rw-   0        0        0        0 2023-05-03 09:46:59.000000 MKN_third_codes-0.6.5.2/MKN_third_codes/__init__.py
+-rw-rw-rw-   0        0        0      683 2023-05-03 07:35:48.000000 MKN_third_codes-0.6.5.2/MKN_third_codes/mkn_globals.py
+-rw-rw-rw-   0        0        0     9636 2023-05-03 09:36:24.000000 MKN_third_codes-0.6.5.2/MKN_third_codes/mkn_utils.py
+-rw-rw-rw-   0        0        0    27856 2023-05-03 09:41:53.000000 MKN_third_codes-0.6.5.2/MKN_third_codes/solutions.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:06.819079 MKN_third_codes-0.6.5.2/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0     7700 2023-05-03 09:48:06.000000 MKN_third_codes-0.6.5.2/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-05-03 09:48:06.000000 MKN_third_codes-0.6.5.2/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 09:48:06.000000 MKN_third_codes-0.6.5.2/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-03 09:48:06.000000 MKN_third_codes-0.6.5.2/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7700 2023-05-03 09:48:06.820076 MKN_third_codes-0.6.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4287 2023-05-03 09:37:41.000000 MKN_third_codes-0.6.5.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-03 09:48:06.821074 MKN_third_codes-0.6.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      489 2023-05-03 09:47:56.000000 MKN_third_codes-0.6.5.2/setup.py
```

### Comparing `MKN_third_codes-0.6.5.1/LICENSE.txt` & `MKN_third_codes-0.6.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.5.1/MKN_third_codes/mkn_globals.py` & `MKN_third_codes-0.6.5.2/MKN_third_codes/mkn_globals.py`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.5.1/MKN_third_codes/mkn_utils.py` & `MKN_third_codes-0.6.5.2/MKN_third_codes/mkn_utils.py`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.5.1/MKN_third_codes/solutions.py` & `MKN_third_codes-0.6.5.2/MKN_third_codes/solutions.py`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.5.1/MKN_third_codes.egg-info/PKG-INFO` & `MKN_third_codes-0.6.5.2/MKN_third_codes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MKN-third-codes
-Version: 0.6.5.1
+Version: 0.6.5.2
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `MKN_third_codes-0.6.5.1/PKG-INFO` & `MKN_third_codes-0.6.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MKN_third_codes
-Version: 0.6.5.1
+Version: 0.6.5.2
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `MKN_third_codes-0.6.5.1/README.md` & `MKN_third_codes-0.6.5.2/README.md`

 * *Files identical despite different names*

