# Comparing `tmp/netpwn-1.4.tar.gz` & `tmp/netpwn-1.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netpwn-1.4.tar", last modified: Mon Jan  3 16:53:29 2022, max compression
+gzip compressed data, was "netpwn-1.4.post1.tar", last modified: Wed May  3 10:24:49 2023, max compression
```

## Comparing `netpwn-1.4.tar` & `netpwn-1.4.post1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 16:53:29.888057 netpwn-1.4/
--rw-r--r--   0 runner    (1001) docker     (121)    18092 2022-01-03 16:52:58.000000 netpwn-1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1978 2022-01-03 16:53:29.888057 netpwn-1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1262 2022-01-03 16:52:58.000000 netpwn-1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 16:53:29.888057 netpwn-1.4/netpwn/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 16:52:58.000000 netpwn-1.4/netpwn/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2206 2022-01-03 16:52:58.000000 netpwn-1.4/netpwn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-01-03 16:52:58.000000 netpwn-1.4/netpwn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 16:53:29.888057 netpwn-1.4/netpwn/services/
--rw-r--r--   0 runner    (1001) docker     (121)     2158 2022-01-03 16:52:58.000000 netpwn-1.4/netpwn/services/ListenerService.py
--rw-r--r--   0 runner    (1001) docker     (121)      682 2022-01-03 16:52:58.000000 netpwn-1.4/netpwn/services/ParametersParserService.py
--rw-r--r--   0 runner    (1001) docker     (121)      325 2022-01-03 16:52:58.000000 netpwn-1.4/netpwn/services/TerminalService.py
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-01-03 16:52:58.000000 netpwn-1.4/netpwn/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 16:53:29.888057 netpwn-1.4/netpwn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1978 2022-01-03 16:53:29.000000 netpwn-1.4/netpwn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-01-03 16:53:29.000000 netpwn-1.4/netpwn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-03 16:53:29.000000 netpwn-1.4/netpwn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-01-03 16:53:29.000000 netpwn-1.4/netpwn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-01-03 16:53:29.000000 netpwn-1.4/netpwn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-01-03 16:53:29.000000 netpwn-1.4/netpwn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-01-03 16:53:29.892057 netpwn-1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-01-03 16:52:58.000000 netpwn-1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 16:53:29.888057 netpwn-1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 16:52:58.000000 netpwn-1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3089 2022-01-03 16:52:58.000000 netpwn-1.4/tests/test_listenner_service.py
--rw-r--r--   0 runner    (1001) docker     (121)     1611 2022-01-03 16:52:58.000000 netpwn-1.4/tests/test_parameters_parser_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:24:49.062347 netpwn-1.4.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-03 10:24:17.000000 netpwn-1.4.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-03 10:24:49.062347 netpwn-1.4.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-03 10:24:17.000000 netpwn-1.4.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:24:49.058346 netpwn-1.4.post1/netpwn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:24:17.000000 netpwn-1.4.post1/netpwn/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2206 2023-05-03 10:24:17.000000 netpwn-1.4.post1/netpwn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-03 10:24:17.000000 netpwn-1.4.post1/netpwn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:24:49.058346 netpwn-1.4.post1/netpwn/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-03 10:24:17.000000 netpwn-1.4.post1/netpwn/services/ListenerService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-03 10:24:17.000000 netpwn-1.4.post1/netpwn/services/ParametersParserService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-03 10:24:17.000000 netpwn-1.4.post1/netpwn/services/TerminalService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-03 10:24:17.000000 netpwn-1.4.post1/netpwn/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:24:49.058346 netpwn-1.4.post1/netpwn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-03 10:24:48.000000 netpwn-1.4.post1/netpwn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-03 10:24:49.000000 netpwn-1.4.post1/netpwn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 10:24:48.000000 netpwn-1.4.post1/netpwn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-03 10:24:48.000000 netpwn-1.4.post1/netpwn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 10:24:48.000000 netpwn-1.4.post1/netpwn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 10:24:48.000000 netpwn-1.4.post1/netpwn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-03 10:24:49.062347 netpwn-1.4.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-03 10:24:17.000000 netpwn-1.4.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:24:49.058346 netpwn-1.4.post1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:24:17.000000 netpwn-1.4.post1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-03 10:24:17.000000 netpwn-1.4.post1/tests/test_listenner_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-03 10:24:17.000000 netpwn-1.4.post1/tests/test_parameters_parser_service.py
```

### Comparing `netpwn-1.4/LICENSE` & `netpwn-1.4.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `netpwn-1.4/PKG-INFO` & `netpwn-1.4.post1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: netpwn
-Version: 1.4
+Version: 1.4.post1
 Summary: A netcat listener alternative with automatic shell stabilization.
 Home-page: https://github.com/anthares101/netpwn
 Author: Ángel Heredia
 License: GPL-2.0
 Project-URL: Release notes, https://github.com/anthares101/netpwn/releases
-Description: <img alt="Test status" src="https://img.shields.io/github/workflow/status/anthares101/netpwn/CI?style=for-the-badge"> <img alt="Version v1.4" src="https://img.shields.io/badge/version-v1.4-blue?style=for-the-badge"> <img alt="GPL-2.0 license" src="https://img.shields.io/github/license/anthares101/netpwn?style=for-the-badge">
+Description: <img alt="Test status" src="https://img.shields.io/github/actions/workflow/status/anthares101/netpwn/ci.yml?style=for-the-badge"> <img alt="Version v1.4" src="https://img.shields.io/badge/version-v1.4-blue?style=for-the-badge"> <img alt="GPL-2.0 license" src="https://img.shields.io/github/license/anthares101/netpwn?style=for-the-badge">
         
         # Netpwn - A netcat listener alternative
         
         The idea of this Linux tool is to be an alternative to a Netcat listener but with the ability to determine if the received conection is a shell or not. If the conection is a shell Netpwn will also try to stabilize it to get a pty (Only Linux and MacOS shells).
         
         ## Installation
```

### Comparing `netpwn-1.4/README.md` & `netpwn-1.4.post1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img alt="Test status" src="https://img.shields.io/github/workflow/status/anthares101/netpwn/CI?style=for-the-badge"> <img alt="Version v1.4" src="https://img.shields.io/badge/version-v1.4-blue?style=for-the-badge"> <img alt="GPL-2.0 license" src="https://img.shields.io/github/license/anthares101/netpwn?style=for-the-badge">
+<img alt="Test status" src="https://img.shields.io/github/actions/workflow/status/anthares101/netpwn/ci.yml?style=for-the-badge"> <img alt="Version v1.4" src="https://img.shields.io/badge/version-v1.4-blue?style=for-the-badge"> <img alt="GPL-2.0 license" src="https://img.shields.io/github/license/anthares101/netpwn?style=for-the-badge">
 
 # Netpwn - A netcat listener alternative
 
 The idea of this Linux tool is to be an alternative to a Netcat listener but with the ability to determine if the received conection is a shell or not. If the conection is a shell Netpwn will also try to stabilize it to get a pty (Only Linux and MacOS shells).
 
 ## Installation
```

### Comparing `netpwn-1.4/netpwn/__main__.py` & `netpwn-1.4.post1/netpwn/__main__.py`

 * *Files identical despite different names*

### Comparing `netpwn-1.4/netpwn/services/ListenerService.py` & `netpwn-1.4.post1/netpwn/services/ListenerService.py`

 * *Files identical despite different names*

### Comparing `netpwn-1.4/netpwn/services/ParametersParserService.py` & `netpwn-1.4.post1/netpwn/services/ParametersParserService.py`

 * *Files identical despite different names*

### Comparing `netpwn-1.4/netpwn.egg-info/PKG-INFO` & `netpwn-1.4.post1/netpwn.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: netpwn
-Version: 1.4
+Version: 1.4.post1
 Summary: A netcat listener alternative with automatic shell stabilization.
 Home-page: https://github.com/anthares101/netpwn
 Author: Ángel Heredia
 License: GPL-2.0
 Project-URL: Release notes, https://github.com/anthares101/netpwn/releases
-Description: <img alt="Test status" src="https://img.shields.io/github/workflow/status/anthares101/netpwn/CI?style=for-the-badge"> <img alt="Version v1.4" src="https://img.shields.io/badge/version-v1.4-blue?style=for-the-badge"> <img alt="GPL-2.0 license" src="https://img.shields.io/github/license/anthares101/netpwn?style=for-the-badge">
+Description: <img alt="Test status" src="https://img.shields.io/github/actions/workflow/status/anthares101/netpwn/ci.yml?style=for-the-badge"> <img alt="Version v1.4" src="https://img.shields.io/badge/version-v1.4-blue?style=for-the-badge"> <img alt="GPL-2.0 license" src="https://img.shields.io/github/license/anthares101/netpwn?style=for-the-badge">
         
         # Netpwn - A netcat listener alternative
         
         The idea of this Linux tool is to be an alternative to a Netcat listener but with the ability to determine if the received conection is a shell or not. If the conection is a shell Netpwn will also try to stabilize it to get a pty (Only Linux and MacOS shells).
         
         ## Installation
```

### Comparing `netpwn-1.4/setup.py` & `netpwn-1.4.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='netpwn',
-    version='1.4',
+    version='1.4.post1',
     license='GPL-2.0',
     description='A netcat listener alternative with automatic shell stabilization.',
     author='Ángel Heredia',
     packages=find_packages(),
     url='https://github.com/anthares101/netpwn',
     keywords='windows macos linux shell reverse-shell tool hacking netcat tty pty cybersecurity reverse pwntools hacktoberfest kali',
     python_requires='>=3',
```

### Comparing `netpwn-1.4/tests/test_listenner_service.py` & `netpwn-1.4.post1/tests/test_listenner_service.py`

 * *Files identical despite different names*

### Comparing `netpwn-1.4/tests/test_parameters_parser_service.py` & `netpwn-1.4.post1/tests/test_parameters_parser_service.py`

 * *Files identical despite different names*

