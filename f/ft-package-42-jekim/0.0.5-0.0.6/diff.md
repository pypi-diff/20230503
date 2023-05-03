# Comparing `tmp/ft_package_42_jekim-0.0.5.tar.gz` & `tmp/ft_package_42_jekim-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ft_package_42_jekim-0.0.5.tar", last modified: Wed May  3 17:38:23 2023, max compression
+gzip compressed data, was "dist/ft_package_42_jekim-0.0.6.tar", last modified: Wed May  3 17:45:25 2023, max compression
```

## Comparing `ft_package_42_jekim-0.0.5.tar` & `ft_package_42_jekim-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 kimjeongjun   (501) staff       (20)        0 2023-05-03 17:38:23.000000 ft_package_42_jekim-0.0.5/
--rw-r--r--   0 kimjeongjun   (501) staff       (20)      396 2023-05-03 17:38:23.000000 ft_package_42_jekim-0.0.5/PKG-INFO
--rw-r--r--   0 kimjeongjun   (501) staff       (20)      124 2023-05-03 16:33:03.000000 ft_package_42_jekim-0.0.5/README.md
--rw-r--r--   0 kimjeongjun   (501) staff       (20)      811 2023-05-03 17:38:11.000000 ft_package_42_jekim-0.0.5/setup.py
--rw-r--r--   0 kimjeongjun   (501) staff       (20)       38 2023-05-03 17:38:23.000000 ft_package_42_jekim-0.0.5/setup.cfg
-drwxr-xr-x   0 kimjeongjun   (501) staff       (20)        0 2023-05-03 17:38:23.000000 ft_package_42_jekim-0.0.5/ft_package_42_jekim.egg-info/
--rw-r--r--   0 kimjeongjun   (501) staff       (20)      396 2023-05-03 17:38:23.000000 ft_package_42_jekim-0.0.5/ft_package_42_jekim.egg-info/PKG-INFO
--rw-r--r--   0 kimjeongjun   (501) staff       (20)      190 2023-05-03 17:38:23.000000 ft_package_42_jekim-0.0.5/ft_package_42_jekim.egg-info/SOURCES.txt
--rw-r--r--   0 kimjeongjun   (501) staff       (20)        1 2023-05-03 17:38:23.000000 ft_package_42_jekim-0.0.5/ft_package_42_jekim.egg-info/top_level.txt
--rw-r--r--   0 kimjeongjun   (501) staff       (20)        1 2023-05-03 17:38:23.000000 ft_package_42_jekim-0.0.5/ft_package_42_jekim.egg-info/dependency_links.txt
+drwxr-xr-x   0 kimjeongjun   (501) staff       (20)        0 2023-05-03 17:45:25.000000 ft_package_42_jekim-0.0.6/
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)      396 2023-05-03 17:45:25.000000 ft_package_42_jekim-0.0.6/PKG-INFO
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)      124 2023-05-03 16:33:03.000000 ft_package_42_jekim-0.0.6/README.md
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)      811 2023-05-03 17:45:09.000000 ft_package_42_jekim-0.0.6/setup.py
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)       38 2023-05-03 17:45:25.000000 ft_package_42_jekim-0.0.6/setup.cfg
+drwxr-xr-x   0 kimjeongjun   (501) staff       (20)        0 2023-05-03 17:45:25.000000 ft_package_42_jekim-0.0.6/ft_package_42_jekim.egg-info/
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)      396 2023-05-03 17:45:25.000000 ft_package_42_jekim-0.0.6/ft_package_42_jekim.egg-info/PKG-INFO
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)      190 2023-05-03 17:45:25.000000 ft_package_42_jekim-0.0.6/ft_package_42_jekim.egg-info/SOURCES.txt
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)        1 2023-05-03 17:45:25.000000 ft_package_42_jekim-0.0.6/ft_package_42_jekim.egg-info/top_level.txt
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)        1 2023-05-03 17:45:25.000000 ft_package_42_jekim-0.0.6/ft_package_42_jekim.egg-info/dependency_links.txt
```

### Comparing `ft_package_42_jekim-0.0.5/setup.py` & `ft_package_42_jekim-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 SUMMARY = "A small example package"
 
 setuptools.setup(
     name="ft_package_42_jekim",
     version=VERSION,
     author="Two-Jay",
     author_email="djeeee1272@gmail.com",
```

