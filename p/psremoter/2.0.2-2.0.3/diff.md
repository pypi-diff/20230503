# Comparing `tmp/psremoter-2.0.2.tar.gz` & `tmp/psremoter-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psremoter-2.0.2.tar", last modified: Wed May  3 13:52:13 2023, max compression
+gzip compressed data, was "psremoter-2.0.3.tar", last modified: Wed May  3 13:53:33 2023, max compression
```

## Comparing `psremoter-2.0.2.tar` & `psremoter-2.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 13:52:13.226792 psremoter-2.0.2/
--rw-rw-rw-   0        0        0     1077 2023-05-01 11:09:52.000000 psremoter-2.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1364 2023-05-03 13:52:13.225793 psremoter-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-03 13:52:13.226792 psremoter-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0      877 2023-05-03 13:52:04.000000 psremoter-2.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:52:13.198809 psremoter-2.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 13:52:13.204805 psremoter-2.0.2/src/psremoter/
--rw-rw-rw-   0        0        0       32 2023-05-01 10:47:51.000000 psremoter-2.0.2/src/psremoter/__init__.py
--rw-rw-rw-   0        0        0     3392 2023-05-01 11:16:22.000000 psremoter-2.0.2/src/psremoter/connector.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:52:13.223794 psremoter-2.0.2/src/psremoter.egg-info/
--rw-rw-rw-   0        0        0     1364 2023-05-03 13:52:13.000000 psremoter-2.0.2/src/psremoter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-05-03 13:52:13.000000 psremoter-2.0.2/src/psremoter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 13:52:13.000000 psremoter-2.0.2/src/psremoter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-03 13:52:13.000000 psremoter-2.0.2/src/psremoter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 13:53:33.901815 psremoter-2.0.3/
+-rw-rw-rw-   0        0        0     1077 2023-05-01 11:09:52.000000 psremoter-2.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      543 2023-05-03 13:53:33.900815 psremoter-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-03 13:53:33.901815 psremoter-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      743 2023-05-03 13:53:31.000000 psremoter-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 13:53:33.876830 psremoter-2.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 13:53:33.881824 psremoter-2.0.3/src/psremoter/
+-rw-rw-rw-   0        0        0       32 2023-05-01 10:47:51.000000 psremoter-2.0.3/src/psremoter/__init__.py
+-rw-rw-rw-   0        0        0     3392 2023-05-01 11:16:22.000000 psremoter-2.0.3/src/psremoter/connector.py
+drwxrwxrwx   0        0        0        0 2023-05-03 13:53:33.899820 psremoter-2.0.3/src/psremoter.egg-info/
+-rw-rw-rw-   0        0        0      543 2023-05-03 13:53:33.000000 psremoter-2.0.3/src/psremoter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-05-03 13:53:33.000000 psremoter-2.0.3/src/psremoter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 13:53:33.000000 psremoter-2.0.3/src/psremoter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-03 13:53:33.000000 psremoter-2.0.3/src/psremoter.egg-info/top_level.txt
```

### Comparing `psremoter-2.0.2/LICENSE.txt` & `psremoter-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `psremoter-2.0.2/src/psremoter/connector.py` & `psremoter-2.0.3/src/psremoter/connector.py`

 * *Files identical despite different names*

