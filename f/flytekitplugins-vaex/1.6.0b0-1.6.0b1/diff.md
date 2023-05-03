# Comparing `tmp/flytekitplugins-vaex-1.6.0b0.tar.gz` & `tmp/flytekitplugins-vaex-1.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-vaex-1.6.0b0.tar", last modified: Wed Apr 19 20:54:36 2023, max compression
+gzip compressed data, was "flytekitplugins-vaex-1.6.0b1.tar", last modified: Wed May  3 04:48:13 2023, max compression
```

## Comparing `flytekitplugins-vaex-1.6.0b0.tar` & `flytekitplugins-vaex-1.6.0b1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:36.235175 flytekitplugins-vaex-1.6.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-19 20:54:36.235175 flytekitplugins-vaex-1.6.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-19 20:54:06.000000 flytekitplugins-vaex-1.6.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:36.231175 flytekitplugins-vaex-1.6.0b0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:36.231175 flytekitplugins-vaex-1.6.0b0/flytekitplugins/vaex/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-19 20:54:06.000000 flytekitplugins-vaex-1.6.0b0/flytekitplugins/vaex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-19 20:54:06.000000 flytekitplugins-vaex-1.6.0b0/flytekitplugins/vaex/sd_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:36.235175 flytekitplugins-vaex-1.6.0b0/flytekitplugins_vaex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-19 20:54:36.000000 flytekitplugins-vaex-1.6.0b0/flytekitplugins_vaex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-19 20:54:36.000000 flytekitplugins-vaex-1.6.0b0/flytekitplugins_vaex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:54:36.000000 flytekitplugins-vaex-1.6.0b0/flytekitplugins_vaex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-19 20:54:36.000000 flytekitplugins-vaex-1.6.0b0/flytekitplugins_vaex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:36.000000 flytekitplugins-vaex-1.6.0b0/flytekitplugins_vaex.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 20:54:36.000000 flytekitplugins-vaex-1.6.0b0/flytekitplugins_vaex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:36.000000 flytekitplugins-vaex-1.6.0b0/flytekitplugins_vaex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:54:36.235175 flytekitplugins-vaex-1.6.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-19 20:54:25.000000 flytekitplugins-vaex-1.6.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:13.688324 flytekitplugins-vaex-1.6.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-03 04:48:13.688324 flytekitplugins-vaex-1.6.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-03 04:47:44.000000 flytekitplugins-vaex-1.6.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:13.688324 flytekitplugins-vaex-1.6.0b1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:13.688324 flytekitplugins-vaex-1.6.0b1/flytekitplugins/vaex/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-03 04:47:44.000000 flytekitplugins-vaex-1.6.0b1/flytekitplugins/vaex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-03 04:47:44.000000 flytekitplugins-vaex-1.6.0b1/flytekitplugins/vaex/sd_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:13.688324 flytekitplugins-vaex-1.6.0b1/flytekitplugins_vaex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-03 04:48:13.000000 flytekitplugins-vaex-1.6.0b1/flytekitplugins_vaex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-03 04:48:13.000000 flytekitplugins-vaex-1.6.0b1/flytekitplugins_vaex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 04:48:13.000000 flytekitplugins-vaex-1.6.0b1/flytekitplugins_vaex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 04:48:13.000000 flytekitplugins-vaex-1.6.0b1/flytekitplugins_vaex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 04:48:13.000000 flytekitplugins-vaex-1.6.0b1/flytekitplugins_vaex.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-03 04:48:13.000000 flytekitplugins-vaex-1.6.0b1/flytekitplugins_vaex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 04:48:13.000000 flytekitplugins-vaex-1.6.0b1/flytekitplugins_vaex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 04:48:13.688324 flytekitplugins-vaex-1.6.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-03 04:48:03.000000 flytekitplugins-vaex-1.6.0b1/setup.py
```

### Comparing `flytekitplugins-vaex-1.6.0b0/PKG-INFO` & `flytekitplugins-vaex-1.6.0b1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-vaex
-Version: 1.6.0b0
+Version: 1.6.0b1
 Summary: Vaex plugin for flytekit
 Author: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `flytekitplugins-vaex-1.6.0b0/flytekitplugins/vaex/sd_transformers.py` & `flytekitplugins-vaex-1.6.0b1/flytekitplugins/vaex/sd_transformers.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-vaex-1.6.0b0/flytekitplugins_vaex.egg-info/PKG-INFO` & `flytekitplugins-vaex-1.6.0b1/flytekitplugins_vaex.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-vaex
-Version: 1.6.0b0
+Version: 1.6.0b1
 Summary: Vaex plugin for flytekit
 Author: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `flytekitplugins-vaex-1.6.0b0/setup.py` & `flytekitplugins-vaex-1.6.0b1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "vaex"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "vaex-core>=4.13.0,<4.14"]
 
-__version__ = "1.6.0b0"
+__version__ = "1.6.0b1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="admin@flyte.org",
     description="Vaex plugin for flytekit",
     namespace_packages=["flytekitplugins"],
```

