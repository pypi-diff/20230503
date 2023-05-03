# Comparing `tmp/ft_package_42_jekim-0.0.3.tar.gz` & `tmp/ft_package_42_jekim-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ft_package_42_jekim-0.0.3.tar", last modified: Wed May  3 17:28:46 2023, max compression
+gzip compressed data, was "dist/ft_package_42_jekim-0.0.4.tar", last modified: Wed May  3 17:31:33 2023, max compression
```

## Comparing `ft_package_42_jekim-0.0.3.tar` & `ft_package_42_jekim-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kimjeongjun   (501) staff       (20)        0 2023-05-03 17:28:46.000000 ft_package_42_jekim-0.0.3/
--rw-r--r--   0 kimjeongjun   (501) staff       (20)      396 2023-05-03 17:28:46.000000 ft_package_42_jekim-0.0.3/PKG-INFO
-drwxr-xr-x   0 kimjeongjun   (501) staff       (20)        0 2023-05-03 17:28:46.000000 ft_package_42_jekim-0.0.3/ ft_package/
--rw-r--r--   0 kimjeongjun   (501) staff       (20)      219 2023-05-03 16:23:03.000000 ft_package_42_jekim-0.0.3/ ft_package/ft.py
--rw-r--r--   0 kimjeongjun   (501) staff       (20)       17 2023-05-03 17:26:02.000000 ft_package_42_jekim-0.0.3/ ft_package/__init__.py
--rw-r--r--   0 kimjeongjun   (501) staff       (20)      124 2023-05-03 16:33:03.000000 ft_package_42_jekim-0.0.3/README.md
--rw-r--r--   0 kimjeongjun   (501) staff       (20)      753 2023-05-03 17:27:36.000000 ft_package_42_jekim-0.0.3/setup.py
--rw-r--r--   0 kimjeongjun   (501) staff       (20)       38 2023-05-03 17:28:46.000000 ft_package_42_jekim-0.0.3/setup.cfg
-drwxr-xr-x   0 kimjeongjun   (501) staff       (20)        0 2023-05-03 17:28:46.000000 ft_package_42_jekim-0.0.3/ft_package_42_jekim.egg-info/
--rw-r--r--   0 kimjeongjun   (501) staff       (20)      396 2023-05-03 17:28:46.000000 ft_package_42_jekim-0.0.3/ft_package_42_jekim.egg-info/PKG-INFO
--rw-r--r--   0 kimjeongjun   (501) staff       (20)      232 2023-05-03 17:28:46.000000 ft_package_42_jekim-0.0.3/ft_package_42_jekim.egg-info/SOURCES.txt
--rw-r--r--   0 kimjeongjun   (501) staff       (20)       12 2023-05-03 17:28:46.000000 ft_package_42_jekim-0.0.3/ft_package_42_jekim.egg-info/top_level.txt
--rw-r--r--   0 kimjeongjun   (501) staff       (20)        1 2023-05-03 17:28:46.000000 ft_package_42_jekim-0.0.3/ft_package_42_jekim.egg-info/dependency_links.txt
+drwxr-xr-x   0 kimjeongjun   (501) staff       (20)        0 2023-05-03 17:31:33.000000 ft_package_42_jekim-0.0.4/
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)      396 2023-05-03 17:31:33.000000 ft_package_42_jekim-0.0.4/PKG-INFO
+drwxr-xr-x   0 kimjeongjun   (501) staff       (20)        0 2023-05-03 17:31:33.000000 ft_package_42_jekim-0.0.4/ ft_package/
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)      219 2023-05-03 16:23:03.000000 ft_package_42_jekim-0.0.4/ ft_package/ft.py
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)       17 2023-05-03 17:26:02.000000 ft_package_42_jekim-0.0.4/ ft_package/__init__.py
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)      124 2023-05-03 16:33:03.000000 ft_package_42_jekim-0.0.4/README.md
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)      790 2023-05-03 17:31:22.000000 ft_package_42_jekim-0.0.4/setup.py
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)       38 2023-05-03 17:31:33.000000 ft_package_42_jekim-0.0.4/setup.cfg
+drwxr-xr-x   0 kimjeongjun   (501) staff       (20)        0 2023-05-03 17:31:33.000000 ft_package_42_jekim-0.0.4/ft_package_42_jekim.egg-info/
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)      396 2023-05-03 17:31:33.000000 ft_package_42_jekim-0.0.4/ft_package_42_jekim.egg-info/PKG-INFO
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)      232 2023-05-03 17:31:33.000000 ft_package_42_jekim-0.0.4/ft_package_42_jekim.egg-info/SOURCES.txt
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)       12 2023-05-03 17:31:33.000000 ft_package_42_jekim-0.0.4/ft_package_42_jekim.egg-info/top_level.txt
+-rw-r--r--   0 kimjeongjun   (501) staff       (20)        1 2023-05-03 17:31:33.000000 ft_package_42_jekim-0.0.4/ft_package_42_jekim.egg-info/dependency_links.txt
```

### Comparing `ft_package_42_jekim-0.0.3/setup.py` & `ft_package_42_jekim-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
+VERSION = "0.0.4"
+SUMMARY = "A small example package"
+
 setuptools.setup(
     name="ft_package_42_jekim",
-    version="0.0.3",
+    version=VERSION,
     author="Two-Jay",
     author_email="djeeee1272@gmail.com",
     license="MIT",
-    description="A small example package",
+    description=SUMMARY,
     long_description=long_description,
     url="https://github.com/Two-Jay/42_Python_for_DataScience",
     packages=setuptools.find_packages(),
 )
 
 # how to install:
```

