# Comparing `tmp/autoLinker-1.0.2.tar.gz` & `tmp/autoLinker-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\autoLinker-1.0.2.tar", last modified: Mon May  1 10:14:45 2023, max compression
+gzip compressed data, was "autoLinker-1.0.4.tar", last modified: Wed May  3 02:13:38 2023, max compression
```

## Comparing `autoLinker-1.0.2.tar` & `autoLinker-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 10:14:45.000000 autoLinker-1.0.2/
--rw-rw-rw-   0        0        0      229 2023-05-01 10:14:45.000000 autoLinker-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-01 10:14:45.000000 autoLinker-1.0.2/autoLinker/
--rw-rw-rw-   0        0        0       96 2023-04-30 11:06:14.000000 autoLinker-1.0.2/autoLinker/__init__.py
--rw-rw-rw-   0        0        0      434 2023-04-30 09:40:42.000000 autoLinker-1.0.2/autoLinker/file.py
-drwxrwxrwx   0        0        0        0 2023-05-01 10:14:45.000000 autoLinker-1.0.2/autoLinker.egg-info/
--rw-rw-rw-   0        0        0      229 2023-05-01 10:14:44.000000 autoLinker-1.0.2/autoLinker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-05-01 10:14:44.000000 autoLinker-1.0.2/autoLinker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 10:14:44.000000 autoLinker-1.0.2/autoLinker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-01 10:14:44.000000 autoLinker-1.0.2/autoLinker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-01 10:14:44.000000 autoLinker-1.0.2/autoLinker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      587 2023-05-01 10:07:25.000000 autoLinker-1.0.2/license.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 10:14:45.000000 autoLinker-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      469 2023-05-01 10:10:31.000000 autoLinker-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 02:13:38.357182 autoLinker-1.0.4/
+-rw-rw-rw-   0        0        0      253 2023-05-03 02:13:38.354183 autoLinker-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 02:13:38.310208 autoLinker-1.0.4/autoLinker/
+-rw-rw-rw-   0        0        0      469 2023-05-02 12:42:26.000000 autoLinker-1.0.4/autoLinker/__init__.py
+-rw-rw-rw-   0        0        0      469 2023-05-03 02:10:50.000000 autoLinker-1.0.4/autoLinker/file.py
+drwxrwxrwx   0        0        0        0 2023-05-03 02:13:38.347191 autoLinker-1.0.4/autoLinker.egg-info/
+-rw-rw-rw-   0        0        0      253 2023-05-03 02:13:37.000000 autoLinker-1.0.4/autoLinker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-05-03 02:13:37.000000 autoLinker-1.0.4/autoLinker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 02:13:37.000000 autoLinker-1.0.4/autoLinker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-03 02:13:37.000000 autoLinker-1.0.4/autoLinker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-03 02:13:37.000000 autoLinker-1.0.4/autoLinker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1093 2023-05-03 01:46:26.000000 autoLinker-1.0.4/license.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 02:13:38.358181 autoLinker-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      446 2023-05-03 01:55:19.000000 autoLinker-1.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

