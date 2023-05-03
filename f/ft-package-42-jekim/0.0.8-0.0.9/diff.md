# Comparing `tmp/ft_package_42_jekim-0.0.8.tar.gz` & `tmp/ft_package_42_jekim-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ft_package_42_jekim-0.0.8.tar", last modified: Wed May  3 17:59:15 2023, max compression
+gzip compressed data, was "dist/ft_package_42_jekim-0.0.9.tar", last modified: Wed May  3 18:02:40 2023, max compression
```

## Comparing `ft_package_42_jekim-0.0.8.tar` & `ft_package_42_jekim-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 kimjeongjun   (501) staff       (20)        0 2023-05-03 17:59:15.000000 ft_package_42_jekim-0.0.8/
--rw-r--r--   0 kimjeongjun   (501) staff       (20)      396 2023-05-03 17:59:15.000000 ft_package_42_jekim-0.0.8/PKG-INFO
--rw-r--r--   0 kimjeongjun   (501) staff       (20)      124 2023-05-03 16:33:03.000000 ft_package_42_jekim-0.0.8/README.md
--rw-r--r--   0 kimjeongjun   (501) staff       (20)      811 2023-05-03 17:58:57.000000 ft_package_42_jekim-0.0.8/setup.py
--rw-r--r--   0 kimjeongjun   (501) staff       (20)       38 2023-05-03 17:59:15.000000 ft_package_42_jekim-0.0.8/setup.cfg
-drwxr-xr-x   0 kimjeongjun   (501) staff       (20)        0 2023-05-03 17:59:15.000000 ft_package_42_jekim-0.0.8/ft_package_42_jekim.egg-info/
--rw-r--r--   0 kimjeongjun   (501) staff       (20)      396 2023-05-03 17:59:15.000000 ft_package_42_jekim-0.0.8/ft_package_42_jekim.egg-info/PKG-INFO
--rw-r--r--   0 kimjeongjun   (501) staff       (20)      190 2023-05-03 17:59:15.000000 ft_package_42_jekim-0.0.8/ft_package_42_jekim.egg-info/SOURCES.txt
--rw-r--r--   0 kimjeongjun   (501) staff       (20)        1 2023-05-03 17:59:15.000000 ft_package_42_jekim-0.0.8/ft_package_42_jekim.egg-info/top_level.txt
--rw-r--r--   0 kimjeongjun   (501) staff       (20)        1 2023-05-03 17:59:15.000000 ft_package_42_jekim-0.0.8/ft_package_42_jekim.egg-info/dependency_links.txt
+drwxr-xr-x   0 kimjeongjun   (501) staff       (20)        0 2023-05-03 18:02:40.000000 ft_package_42_jekim-0.0.9/
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)      396 2023-05-03 18:02:40.000000 ft_package_42_jekim-0.0.9/PKG-INFO
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)      124 2023-05-03 16:33:03.000000 ft_package_42_jekim-0.0.9/README.md
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)      811 2023-05-03 18:02:26.000000 ft_package_42_jekim-0.0.9/setup.py
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)       38 2023-05-03 18:02:40.000000 ft_package_42_jekim-0.0.9/setup.cfg
+drwxr-xr-x   0 kimjeongjun   (501) staff       (20)        0 2023-05-03 18:02:40.000000 ft_package_42_jekim-0.0.9/ft_package_42_jekim.egg-info/
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)      396 2023-05-03 18:02:40.000000 ft_package_42_jekim-0.0.9/ft_package_42_jekim.egg-info/PKG-INFO
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)      190 2023-05-03 18:02:40.000000 ft_package_42_jekim-0.0.9/ft_package_42_jekim.egg-info/SOURCES.txt
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)        1 2023-05-03 18:02:40.000000 ft_package_42_jekim-0.0.9/ft_package_42_jekim.egg-info/top_level.txt
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)        1 2023-05-03 18:02:40.000000 ft_package_42_jekim-0.0.9/ft_package_42_jekim.egg-info/dependency_links.txt
```

### Comparing `ft_package_42_jekim-0.0.8/setup.py` & `ft_package_42_jekim-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 SUMMARY = "A small example package"
 
 setuptools.setup(
     name="ft_package_42_jekim",
     version=VERSION,
     author="Two-Jay",
     author_email="djeeee1272@gmail.com",
```

