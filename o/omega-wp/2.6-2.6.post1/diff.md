# Comparing `tmp/omega_wp-2.6.tar.gz` & `tmp/omega_wp-2.6.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omega_wp-2.6.tar", last modified: Mon Jan  3 17:24:01 2022, max compression
+gzip compressed data, was "omega_wp-2.6.post1.tar", last modified: Wed May  3 10:21:59 2023, max compression
```

## Comparing `omega_wp-2.6.tar` & `omega_wp-2.6.post1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 17:24:01.153569 omega_wp-2.6/
--rw-r--r--   0 runner    (1001) docker     (121)    18092 2022-01-03 17:23:24.000000 omega_wp-2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3644 2022-01-03 17:24:01.153569 omega_wp-2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2752 2022-01-03 17:23:24.000000 omega_wp-2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 17:24:01.149569 omega_wp-2.6/omega_wp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 17:23:24.000000 omega_wp-2.6/omega_wp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3155 2022-01-03 17:23:24.000000 omega_wp-2.6/omega_wp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5322 2022-01-03 17:23:24.000000 omega_wp-2.6/omega_wp/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 17:24:01.149569 omega_wp-2.6/omega_wp/services/
--rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-01-03 17:23:24.000000 omega_wp-2.6/omega_wp/services/LoginService.py
--rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-01-03 17:23:24.000000 omega_wp-2.6/omega_wp/services/ParametersParserService.py
--rw-r--r--   0 runner    (1001) docker     (121)     2663 2022-01-03 17:23:24.000000 omega_wp-2.6/omega_wp/services/PayloadService.py
--rw-r--r--   0 runner    (1001) docker     (121)     3199 2022-01-03 17:23:24.000000 omega_wp-2.6/omega_wp/services/ShellService.py
--rw-r--r--   0 runner    (1001) docker     (121)      325 2022-01-03 17:23:24.000000 omega_wp-2.6/omega_wp/services/TerminalService.py
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-01-03 17:23:24.000000 omega_wp-2.6/omega_wp/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 17:24:01.149569 omega_wp-2.6/omega_wp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3644 2022-01-03 17:24:00.000000 omega_wp-2.6/omega_wp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-01-03 17:24:00.000000 omega_wp-2.6/omega_wp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-03 17:24:00.000000 omega_wp-2.6/omega_wp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-01-03 17:24:00.000000 omega_wp-2.6/omega_wp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-01-03 17:24:00.000000 omega_wp-2.6/omega_wp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-01-03 17:24:00.000000 omega_wp-2.6/omega_wp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-01-03 17:24:01.153569 omega_wp-2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      723 2022-01-03 17:23:24.000000 omega_wp-2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 17:24:01.153569 omega_wp-2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 17:23:24.000000 omega_wp-2.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6687 2022-01-03 17:23:24.000000 omega_wp-2.6/tests/mocks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2834 2022-01-03 17:23:24.000000 omega_wp-2.6/tests/test_login_service.py
--rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-01-03 17:23:24.000000 omega_wp-2.6/tests/test_parameters_parser_service.py
--rw-r--r--   0 runner    (1001) docker     (121)     4679 2022-01-03 17:23:24.000000 omega_wp-2.6/tests/test_payload_service.py
--rw-r--r--   0 runner    (1001) docker     (121)    12261 2022-01-03 17:23:24.000000 omega_wp-2.6/tests/test_shell_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:21:59.372665 omega_wp-2.6.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-03 10:21:14.000000 omega_wp-2.6.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-03 10:21:59.372665 omega_wp-2.6.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-03 10:21:14.000000 omega_wp-2.6.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:21:59.368665 omega_wp-2.6.post1/omega_wp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:21:14.000000 omega_wp-2.6.post1/omega_wp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3155 2023-05-03 10:21:14.000000 omega_wp-2.6.post1/omega_wp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-05-03 10:21:14.000000 omega_wp-2.6.post1/omega_wp/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:21:59.372665 omega_wp-2.6.post1/omega_wp/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-03 10:21:14.000000 omega_wp-2.6.post1/omega_wp/services/LoginService.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-03 10:21:14.000000 omega_wp-2.6.post1/omega_wp/services/ParametersParserService.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-03 10:21:14.000000 omega_wp-2.6.post1/omega_wp/services/PayloadService.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-03 10:21:14.000000 omega_wp-2.6.post1/omega_wp/services/ShellService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-03 10:21:14.000000 omega_wp-2.6.post1/omega_wp/services/TerminalService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-03 10:21:14.000000 omega_wp-2.6.post1/omega_wp/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:21:59.368665 omega_wp-2.6.post1/omega_wp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-03 10:21:59.000000 omega_wp-2.6.post1/omega_wp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-03 10:21:59.000000 omega_wp-2.6.post1/omega_wp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 10:21:59.000000 omega_wp-2.6.post1/omega_wp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-03 10:21:59.000000 omega_wp-2.6.post1/omega_wp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-03 10:21:59.000000 omega_wp-2.6.post1/omega_wp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 10:21:59.000000 omega_wp-2.6.post1/omega_wp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-03 10:21:59.372665 omega_wp-2.6.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-03 10:21:14.000000 omega_wp-2.6.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:21:59.372665 omega_wp-2.6.post1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:21:14.000000 omega_wp-2.6.post1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-05-03 10:21:14.000000 omega_wp-2.6.post1/tests/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-03 10:21:14.000000 omega_wp-2.6.post1/tests/test_login_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-03 10:21:14.000000 omega_wp-2.6.post1/tests/test_parameters_parser_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-05-03 10:21:14.000000 omega_wp-2.6.post1/tests/test_payload_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-05-03 10:21:14.000000 omega_wp-2.6.post1/tests/test_shell_service.py
```

### Comparing `omega_wp-2.6/LICENSE` & `omega_wp-2.6.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `omega_wp-2.6/PKG-INFO` & `omega_wp-2.6.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: omega_wp
-Version: 2.6
+Version: 2.6.post1
 Summary: From Wordpress admin to pty automatically!
 Home-page: https://github.com/anthares101/omega
 Author: Ángel Heredia
 License: GPL-2.0
 Project-URL: Release notes, https://github.com/anthares101/omega/releases
-Description: <img alt="Test suite status" src="https://img.shields.io/github/workflow/status/anthares101/omega/CI?style=for-the-badge"> <img alt="Version v2.6" src="https://img.shields.io/badge/version-v2.6-blue?style=for-the-badge"> <img alt="GPL-2.0 license" src="https://img.shields.io/github/license/anthares101/omega?style=for-the-badge">
+Description: <img alt="Test suite status" src="https://img.shields.io/github/actions/workflow/status/anthares101/omega/ci.yml?style=for-the-badge"> <img alt="Version v2.6" src="https://img.shields.io/badge/version-v2.6-blue?style=for-the-badge"> <img alt="GPL-2.0 license" src="https://img.shields.io/github/license/anthares101/omega?style=for-the-badge">
         
         # Omega - From Wordpress admin to pty
         
         The Linux tool to automate the process of getting a pty once you got admin credentials in a Wordpress site. Works in Linux, Windows and MacOS hosts! 
         
         The shell code used for Windows hosts is a modified version of the [PHP reverse shell](https://github.com/ivan-sincek/php-reverse-shell/blob/master/src/php_reverse_shell.php) by [ivan-sincek](https://github.com/ivan-sincek), credits to the author.
```

### Comparing `omega_wp-2.6/README.md` & `omega_wp-2.6.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img alt="Test suite status" src="https://img.shields.io/github/workflow/status/anthares101/omega/CI?style=for-the-badge"> <img alt="Version v2.6" src="https://img.shields.io/badge/version-v2.6-blue?style=for-the-badge"> <img alt="GPL-2.0 license" src="https://img.shields.io/github/license/anthares101/omega?style=for-the-badge">
+<img alt="Test suite status" src="https://img.shields.io/github/actions/workflow/status/anthares101/omega/ci.yml?style=for-the-badge"> <img alt="Version v2.6" src="https://img.shields.io/badge/version-v2.6-blue?style=for-the-badge"> <img alt="GPL-2.0 license" src="https://img.shields.io/github/license/anthares101/omega?style=for-the-badge">
 
 # Omega - From Wordpress admin to pty
 
 The Linux tool to automate the process of getting a pty once you got admin credentials in a Wordpress site. Works in Linux, Windows and MacOS hosts! 
 
 The shell code used for Windows hosts is a modified version of the [PHP reverse shell](https://github.com/ivan-sincek/php-reverse-shell/blob/master/src/php_reverse_shell.php) by [ivan-sincek](https://github.com/ivan-sincek), credits to the author.
```

### Comparing `omega_wp-2.6/omega_wp/__main__.py` & `omega_wp-2.6.post1/omega_wp/__main__.py`

 * *Files identical despite different names*

### Comparing `omega_wp-2.6/omega_wp/config.py` & `omega_wp-2.6.post1/omega_wp/config.py`

 * *Files identical despite different names*

### Comparing `omega_wp-2.6/omega_wp/services/LoginService.py` & `omega_wp-2.6.post1/omega_wp/services/LoginService.py`

 * *Files identical despite different names*

### Comparing `omega_wp-2.6/omega_wp/services/ParametersParserService.py` & `omega_wp-2.6.post1/omega_wp/services/ParametersParserService.py`

 * *Files identical despite different names*

### Comparing `omega_wp-2.6/omega_wp/services/PayloadService.py` & `omega_wp-2.6.post1/omega_wp/services/PayloadService.py`

 * *Files identical despite different names*

### Comparing `omega_wp-2.6/omega_wp/services/ShellService.py` & `omega_wp-2.6.post1/omega_wp/services/ShellService.py`

 * *Files identical despite different names*

### Comparing `omega_wp-2.6/omega_wp.egg-info/PKG-INFO` & `omega_wp-2.6.post1/omega_wp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: omega-wp
-Version: 2.6
+Version: 2.6.post1
 Summary: From Wordpress admin to pty automatically!
 Home-page: https://github.com/anthares101/omega
 Author: Ángel Heredia
 License: GPL-2.0
 Project-URL: Release notes, https://github.com/anthares101/omega/releases
-Description: <img alt="Test suite status" src="https://img.shields.io/github/workflow/status/anthares101/omega/CI?style=for-the-badge"> <img alt="Version v2.6" src="https://img.shields.io/badge/version-v2.6-blue?style=for-the-badge"> <img alt="GPL-2.0 license" src="https://img.shields.io/github/license/anthares101/omega?style=for-the-badge">
+Description: <img alt="Test suite status" src="https://img.shields.io/github/actions/workflow/status/anthares101/omega/ci.yml?style=for-the-badge"> <img alt="Version v2.6" src="https://img.shields.io/badge/version-v2.6-blue?style=for-the-badge"> <img alt="GPL-2.0 license" src="https://img.shields.io/github/license/anthares101/omega?style=for-the-badge">
         
         # Omega - From Wordpress admin to pty
         
         The Linux tool to automate the process of getting a pty once you got admin credentials in a Wordpress site. Works in Linux, Windows and MacOS hosts! 
         
         The shell code used for Windows hosts is a modified version of the [PHP reverse shell](https://github.com/ivan-sincek/php-reverse-shell/blob/master/src/php_reverse_shell.php) by [ivan-sincek](https://github.com/ivan-sincek), credits to the author.
```

### Comparing `omega_wp-2.6/omega_wp.egg-info/SOURCES.txt` & `omega_wp-2.6.post1/omega_wp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omega_wp-2.6/setup.py` & `omega_wp-2.6.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='omega_wp',
-    version='2.6',
+    version='2.6.post1',
     license='GPL-2.0',
     description='From Wordpress admin to pty automatically!',
     author='Ángel Heredia',
     packages=find_packages(),
     url='https://github.com/anthares101/omega',
     keywords='windows macos linux shell wordpress reverse-shell tool hacking tty pty cybersecurity reverse pwntools hacktoberfest kali',
     python_requires='>=3',
```

### Comparing `omega_wp-2.6/tests/mocks.py` & `omega_wp-2.6.post1/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `omega_wp-2.6/tests/test_login_service.py` & `omega_wp-2.6.post1/tests/test_login_service.py`

 * *Files identical despite different names*

### Comparing `omega_wp-2.6/tests/test_parameters_parser_service.py` & `omega_wp-2.6.post1/tests/test_parameters_parser_service.py`

 * *Files identical despite different names*

### Comparing `omega_wp-2.6/tests/test_payload_service.py` & `omega_wp-2.6.post1/tests/test_payload_service.py`

 * *Files identical despite different names*

### Comparing `omega_wp-2.6/tests/test_shell_service.py` & `omega_wp-2.6.post1/tests/test_shell_service.py`

 * *Files identical despite different names*

