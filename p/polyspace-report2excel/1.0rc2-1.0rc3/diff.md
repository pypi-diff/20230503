# Comparing `tmp/polyspace-report2excel-1.0rc2.tar.gz` & `tmp/polyspace-report2excel-1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyspace-report2excel-1.0rc2.tar", last modified: Mon Mar 20 11:32:10 2023, max compression
+gzip compressed data, was "polyspace-report2excel-1.0rc3.tar", last modified: Tue Mar 21 09:00:40 2023, max compression
```

## Comparing `polyspace-report2excel-1.0rc2.tar` & `polyspace-report2excel-1.0rc3.tar`

### file list

```diff
@@ -1,17 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 11:32:10.364513 polyspace-report2excel-1.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-20 11:31:56.000000 polyspace-report2excel-1.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    43112 2023-03-20 11:32:10.364513 polyspace-report2excel-1.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-03-20 11:31:56.000000 polyspace-report2excel-1.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 11:32:10.360513 polyspace-report2excel-1.0rc2/polyspace_report2excel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43112 2023-03-20 11:32:10.000000 polyspace-report2excel-1.0rc2/polyspace_report2excel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-20 11:32:10.000000 polyspace-report2excel-1.0rc2/polyspace_report2excel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 11:32:10.000000 polyspace-report2excel-1.0rc2/polyspace_report2excel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-20 11:32:10.000000 polyspace-report2excel-1.0rc2/polyspace_report2excel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-20 11:32:10.000000 polyspace-report2excel-1.0rc2/polyspace_report2excel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 11:32:10.000000 polyspace-report2excel-1.0rc2/polyspace_report2excel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-20 11:31:56.000000 polyspace-report2excel-1.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 11:32:10.364513 polyspace-report2excel-1.0rc2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 11:32:10.364513 polyspace-report2excel-1.0rc2/test/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-20 11:31:56.000000 polyspace-report2excel-1.0rc2/test/test_HTMLReader.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-20 11:31:56.000000 polyspace-report2excel-1.0rc2/test/test_csvexporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-20 11:31:56.000000 polyspace-report2excel-1.0rc2/test/test_xlsxexporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:00:40.114405 polyspace-report2excel-1.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-21 09:00:22.000000 polyspace-report2excel-1.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43054 2023-03-21 09:00:40.110405 polyspace-report2excel-1.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-03-21 09:00:22.000000 polyspace-report2excel-1.0rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-21 09:00:22.000000 polyspace-report2excel-1.0rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 09:00:40.114405 polyspace-report2excel-1.0rc3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:00:40.106405 polyspace-report2excel-1.0rc3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:00:40.110405 polyspace-report2excel-1.0rc3/src/p2e/
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-03-21 09:00:22.000000 polyspace-report2excel-1.0rc3/src/p2e/HTMLReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-03-21 09:00:22.000000 polyspace-report2excel-1.0rc3/src/p2e/RTFReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-21 09:00:22.000000 polyspace-report2excel-1.0rc3/src/p2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-03-21 09:00:22.000000 polyspace-report2excel-1.0rc3/src/p2e/exportcsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-03-21 09:00:22.000000 polyspace-report2excel-1.0rc3/src/p2e/exportxlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-03-21 09:00:22.000000 polyspace-report2excel-1.0rc3/src/p2e/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:00:40.110405 polyspace-report2excel-1.0rc3/src/polyspace_report2excel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43054 2023-03-21 09:00:40.000000 polyspace-report2excel-1.0rc3/src/polyspace_report2excel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-21 09:00:40.000000 polyspace-report2excel-1.0rc3/src/polyspace_report2excel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 09:00:40.000000 polyspace-report2excel-1.0rc3/src/polyspace_report2excel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-21 09:00:40.000000 polyspace-report2excel-1.0rc3/src/polyspace_report2excel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-21 09:00:40.000000 polyspace-report2excel-1.0rc3/src/polyspace_report2excel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-21 09:00:40.000000 polyspace-report2excel-1.0rc3/src/polyspace_report2excel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:00:40.110405 polyspace-report2excel-1.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-21 09:00:22.000000 polyspace-report2excel-1.0rc3/tests/test_HTMLReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-21 09:00:22.000000 polyspace-report2excel-1.0rc3/tests/test_csvexporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-21 09:00:22.000000 polyspace-report2excel-1.0rc3/tests/test_xlsxexporter.py
```

### Comparing `polyspace-report2excel-1.0rc2/LICENSE` & `polyspace-report2excel-1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `polyspace-report2excel-1.0rc2/PKG-INFO` & `polyspace-report2excel-1.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyspace-report2excel
-Version: 1.0rc2
+Version: 1.0rc3
 Summary: read a polyspace report and export misra or run-time results
 Author-email: CAT Lab <L-lequal@cnes.fr>
 Maintainer-email: CAT Lab <L-lequal@cnes.fr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -711,29 +711,29 @@
 Use arguments to filter what you need.
 
 :warning: by converting RTF file you must precise --runtime or --misra
 
 
 ### Usage example with the pip package
 ```
-polyspace-report2excel p2e input.html output-folder/
+p2e input.html output-folder/
 
-polyspace-report2excel p2e input.rtf ouput-folder/ --runtime
+p2e input.rtf ouput-folder/ --runtime
 ```
 
 ### Usage example by cloning the repository
 If you don't want to install the package `polyspace-report2excel`, first install the dependencies.
 
 `pip install XlsxWriter html2text striprtf`
 
 Then, you can run:
 ``` 
-python export-all.py input.html ouput-folder/
+python main.py input.html ouput-folder/
 
-python export-all.py input.rtf ouput-folder/ --runtime
+python main.py input.rtf ouput-folder/ --runtime
 ```
 ## Arguments
 - `--misra` will export misra report only.
 - `--runtime` will export run-time report only (ignored if `--misra`).
 - `-y` will force overwrite if output files already exist.
 - `--poly14` will read report from polyspace 2014
 - `--csv` will export data in CSV instead of xlsx
```

### Comparing `polyspace-report2excel-1.0rc2/README.md` & `polyspace-report2excel-1.0rc3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,29 +18,29 @@
 Use arguments to filter what you need.
 
 :warning: by converting RTF file you must precise --runtime or --misra
 
 
 ### Usage example with the pip package
 ```
-polyspace-report2excel p2e input.html output-folder/
+p2e input.html output-folder/
 
-polyspace-report2excel p2e input.rtf ouput-folder/ --runtime
+p2e input.rtf ouput-folder/ --runtime
 ```
 
 ### Usage example by cloning the repository
 If you don't want to install the package `polyspace-report2excel`, first install the dependencies.
 
 `pip install XlsxWriter html2text striprtf`
 
 Then, you can run:
 ``` 
-python export-all.py input.html ouput-folder/
+python main.py input.html ouput-folder/
 
-python export-all.py input.rtf ouput-folder/ --runtime
+python main.py input.rtf ouput-folder/ --runtime
 ```
 ## Arguments
 - `--misra` will export misra report only.
 - `--runtime` will export run-time report only (ignored if `--misra`).
 - `-y` will force overwrite if output files already exist.
 - `--poly14` will read report from polyspace 2014
 - `--csv` will export data in CSV instead of xlsx
```

### Comparing `polyspace-report2excel-1.0rc2/polyspace_report2excel.egg-info/PKG-INFO` & `polyspace-report2excel-1.0rc3/src/polyspace_report2excel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyspace-report2excel
-Version: 1.0rc2
+Version: 1.0rc3
 Summary: read a polyspace report and export misra or run-time results
 Author-email: CAT Lab <L-lequal@cnes.fr>
 Maintainer-email: CAT Lab <L-lequal@cnes.fr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -711,29 +711,29 @@
 Use arguments to filter what you need.
 
 :warning: by converting RTF file you must precise --runtime or --misra
 
 
 ### Usage example with the pip package
 ```
-polyspace-report2excel p2e input.html output-folder/
+p2e input.html output-folder/
 
-polyspace-report2excel p2e input.rtf ouput-folder/ --runtime
+p2e input.rtf ouput-folder/ --runtime
 ```
 
 ### Usage example by cloning the repository
 If you don't want to install the package `polyspace-report2excel`, first install the dependencies.
 
 `pip install XlsxWriter html2text striprtf`
 
 Then, you can run:
 ``` 
-python export-all.py input.html ouput-folder/
+python main.py input.html ouput-folder/
 
-python export-all.py input.rtf ouput-folder/ --runtime
+python main.py input.rtf ouput-folder/ --runtime
 ```
 ## Arguments
 - `--misra` will export misra report only.
 - `--runtime` will export run-time report only (ignored if `--misra`).
 - `-y` will force overwrite if output files already exist.
 - `--poly14` will read report from polyspace 2014
 - `--csv` will export data in CSV instead of xlsx
```

