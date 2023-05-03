# Comparing `tmp/ausbildungsnachweise_utils-0.0.7.tar.gz` & `tmp/ausbildungsnachweise_utils-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ausbildungsnachweise_utils-0.0.7.tar", last modified: Wed May  3 10:51:06 2023, max compression
+gzip compressed data, was "ausbildungsnachweise_utils-0.0.8.tar", last modified: Wed May  3 11:01:02 2023, max compression
```

## Comparing `ausbildungsnachweise_utils-0.0.7.tar` & `ausbildungsnachweise_utils-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-03 10:51:06.439607 ausbildungsnachweise_utils-0.0.7/
--rw-rw-r--   0 sam       (1000) sam       (1000)      380 2023-05-03 10:51:06.435608 ausbildungsnachweise_utils-0.0.7/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)       28 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.7/README.md
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-03 10:51:06.435608 ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils/
--rw-r--r--   0 sam       (1000) sam       (1000)        0 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)       90 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils/__main__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3281 2023-05-03 10:37:49.000000 ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils/processor.py
--rw-r--r--   0 sam       (1000) sam       (1000)     2204 2023-05-03 10:35:16.000000 ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils/starter.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-03 10:51:06.435608 ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils.egg-info/
--rw-rw-r--   0 sam       (1000) sam       (1000)      380 2023-05-03 10:51:06.000000 ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils.egg-info/PKG-INFO
--rw-rw-r--   0 sam       (1000) sam       (1000)      476 2023-05-03 10:51:06.000000 ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)        1 2023-05-03 10:51:06.000000 ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)       88 2023-05-03 10:51:06.000000 ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils.egg-info/entry_points.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)       20 2023-05-03 10:51:06.000000 ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils.egg-info/requires.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)       27 2023-05-03 10:51:06.000000 ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils.egg-info/top_level.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)       38 2023-05-03 10:51:06.439607 ausbildungsnachweise_utils-0.0.7/setup.cfg
--rw-r--r--   0 sam       (1000) sam       (1000)      891 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.7/setup.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-03 11:01:02.405671 ausbildungsnachweise_utils-0.0.8/
+-rw-rw-r--   0 sam       (1000) sam       (1000)      380 2023-05-03 11:01:02.405671 ausbildungsnachweise_utils-0.0.8/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)       28 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.8/README.md
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-03 11:01:02.405671 ausbildungsnachweise_utils-0.0.8/ausbildungsnachweise_utils/
+-rw-r--r--   0 sam       (1000) sam       (1000)        0 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.8/ausbildungsnachweise_utils/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)       90 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.8/ausbildungsnachweise_utils/__main__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3281 2023-05-03 10:37:49.000000 ausbildungsnachweise_utils-0.0.8/ausbildungsnachweise_utils/processor.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2267 2023-05-03 10:59:11.000000 ausbildungsnachweise_utils-0.0.8/ausbildungsnachweise_utils/starter.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-03 11:01:02.405671 ausbildungsnachweise_utils-0.0.8/ausbildungsnachweise_utils.egg-info/
+-rw-rw-r--   0 sam       (1000) sam       (1000)      380 2023-05-03 11:01:02.000000 ausbildungsnachweise_utils-0.0.8/ausbildungsnachweise_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)      476 2023-05-03 11:01:02.000000 ausbildungsnachweise_utils-0.0.8/ausbildungsnachweise_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        1 2023-05-03 11:01:02.000000 ausbildungsnachweise_utils-0.0.8/ausbildungsnachweise_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       88 2023-05-03 11:01:02.000000 ausbildungsnachweise_utils-0.0.8/ausbildungsnachweise_utils.egg-info/entry_points.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       20 2023-05-03 11:01:02.000000 ausbildungsnachweise_utils-0.0.8/ausbildungsnachweise_utils.egg-info/requires.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       27 2023-05-03 11:01:02.000000 ausbildungsnachweise_utils-0.0.8/ausbildungsnachweise_utils.egg-info/top_level.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       38 2023-05-03 11:01:02.405671 ausbildungsnachweise_utils-0.0.8/setup.cfg
+-rw-r--r--   0 sam       (1000) sam       (1000)      891 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.8/setup.py
```

### Comparing `ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils/processor.py` & `ausbildungsnachweise_utils-0.0.8/ausbildungsnachweise_utils/processor.py`

 * *Files identical despite different names*

### Comparing `ausbildungsnachweise_utils-0.0.7/ausbildungsnachweise_utils/starter.py` & `ausbildungsnachweise_utils-0.0.8/ausbildungsnachweise_utils/starter.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 
 def start():
     parser = argparse.ArgumentParser()
     parser.add_argument("input_dir", nargs='?', default=INPUT_DIR)
     parser.add_argument("output_dir", nargs='?', default=OUTPUT_DIR)
     args = parser.parse_args()
 
+    print(Path().absolute())
+    print(Path(__file__).parent)
+
     if Path(FILE_DIR, args.input_dir).is_dir() and Path(FILE_DIR, args.output_dir).is_dir():
         get_new_files(args.input_dir, args.output_dir)
 
 
 def get_new_files(input_dir, output_dir):
     input_files = set((f.stem for f in Path(FILE_DIR, input_dir).glob("*" + INPUT_SUFFIX) if f.is_file()))
     output_files = set((f.stem for f in Path(FILE_DIR, output_dir).glob("*" + OUTPUT_SUFFIX) if f.is_file()))
```

### Comparing `ausbildungsnachweise_utils-0.0.7/setup.py` & `ausbildungsnachweise_utils-0.0.8/setup.py`

 * *Files identical despite different names*

