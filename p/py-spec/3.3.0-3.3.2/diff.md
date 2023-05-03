# Comparing `tmp/py_spec-3.3.0.tar.gz` & `tmp/py_spec-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_spec-3.3.0.tar", last modified: Thu Apr 13 07:16:02 2023, max compression
+gzip compressed data, was "py_spec-3.3.2.tar", last modified: Wed May  3 07:45:45 2023, max compression
```

## Comparing `py_spec-3.3.0.tar` & `py_spec-3.3.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:16:02.567370 py_spec-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-13 07:16:02.567370 py_spec-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-13 07:15:14.000000 py_spec-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:16:02.567370 py_spec-3.3.0/py_spec/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-13 07:15:14.000000 py_spec-3.3.0/py_spec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:16:02.567370 py_spec-3.3.0/py_spec/input/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-13 07:15:14.000000 py_spec-3.3.0/py_spec/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39615 2023-04-13 07:15:14.000000 py_spec-3.3.0/py_spec/input/spec_namelist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:16:02.567370 py_spec-3.3.0/py_spec/output/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 07:15:14.000000 py_spec-3.3.0/py_spec/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-13 07:15:14.000000 py_spec-3.3.0/py_spec/output/_plot_iota.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-13 07:15:14.000000 py_spec-3.3.0/py_spec/output/_plot_kam_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-13 07:15:14.000000 py_spec-3.3.0/py_spec/output/_plot_modB.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-13 07:15:14.000000 py_spec-3.3.0/py_spec/output/_plot_poincare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-13 07:15:14.000000 py_spec-3.3.0/py_spec/output/_plot_pressure.py
--rw-r--r--   0 runner    (1001) docker     (123)    26434 2023-04-13 07:15:14.000000 py_spec-3.3.0/py_spec/output/_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-04-13 07:15:14.000000 py_spec-3.3.0/py_spec/output/spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:16:02.567370 py_spec-3.3.0/py_spec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-13 07:16:02.000000 py_spec-3.3.0/py_spec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-13 07:16:02.000000 py_spec-3.3.0/py_spec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 07:16:02.000000 py_spec-3.3.0/py_spec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 07:16:02.000000 py_spec-3.3.0/py_spec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 07:16:02.567370 py_spec-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-13 07:15:14.000000 py_spec-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:45:45.947907 py_spec-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-03 07:45:45.943907 py_spec-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-03 07:44:56.000000 py_spec-3.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:45:45.943907 py_spec-3.3.2/py_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-03 07:44:56.000000 py_spec-3.3.2/py_spec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:45:45.943907 py_spec-3.3.2/py_spec/input/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-03 07:44:56.000000 py_spec-3.3.2/py_spec/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39615 2023-05-03 07:44:56.000000 py_spec-3.3.2/py_spec/input/spec_namelist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:45:45.943907 py_spec-3.3.2/py_spec/output/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-03 07:44:56.000000 py_spec-3.3.2/py_spec/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-03 07:44:56.000000 py_spec-3.3.2/py_spec/output/_plot_iota.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-03 07:44:56.000000 py_spec-3.3.2/py_spec/output/_plot_kam_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-03 07:44:56.000000 py_spec-3.3.2/py_spec/output/_plot_modB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-03 07:44:56.000000 py_spec-3.3.2/py_spec/output/_plot_poincare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-03 07:44:56.000000 py_spec-3.3.2/py_spec/output/_plot_pressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26432 2023-05-03 07:44:56.000000 py_spec-3.3.2/py_spec/output/_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-05-03 07:44:56.000000 py_spec-3.3.2/py_spec/output/spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:45:45.943907 py_spec-3.3.2/py_spec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-03 07:45:45.000000 py_spec-3.3.2/py_spec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-03 07:45:45.000000 py_spec-3.3.2/py_spec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 07:45:45.000000 py_spec-3.3.2/py_spec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 07:45:45.000000 py_spec-3.3.2/py_spec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 07:45:45.947907 py_spec-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-03 07:44:56.000000 py_spec-3.3.2/setup.py
```

### Comparing `py_spec-3.3.0/PKG-INFO` & `py_spec-3.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_spec
-Version: 3.3.0
+Version: 3.3.2
 Summary: SPEC(Stepped-Pressure Equilibrium Code) python utilities
 Home-page: https://princetonuniversity.github.io/SPEC/
 Author: SPEC developers
 License: GNU 3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `py_spec-3.3.0/README.md` & `py_spec-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `py_spec-3.3.0/py_spec/input/spec_namelist.py` & `py_spec-3.3.2/py_spec/input/spec_namelist.py`

 * *Files identical despite different names*

### Comparing `py_spec-3.3.0/py_spec/output/_plot_iota.py` & `py_spec-3.3.2/py_spec/output/_plot_iota.py`

 * *Files identical despite different names*

### Comparing `py_spec-3.3.0/py_spec/output/_plot_kam_surface.py` & `py_spec-3.3.2/py_spec/output/_plot_kam_surface.py`

 * *Files identical despite different names*

### Comparing `py_spec-3.3.0/py_spec/output/_plot_modB.py` & `py_spec-3.3.2/py_spec/output/_plot_modB.py`

 * *Files identical despite different names*

### Comparing `py_spec-3.3.0/py_spec/output/_plot_poincare.py` & `py_spec-3.3.2/py_spec/output/_plot_poincare.py`

 * *Files identical despite different names*

### Comparing `py_spec-3.3.0/py_spec/output/_plot_pressure.py` & `py_spec-3.3.2/py_spec/output/_plot_pressure.py`

 * *Files identical despite different names*

### Comparing `py_spec-3.3.0/py_spec/output/_processing.py` & `py_spec-3.3.2/py_spec/output/_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -543,15 +543,15 @@
         betavol = 2 * nfp * press * integrate.simpson( 
             y=integrate.simpson( 
                 y=integrate.simpson( 
                     y=sg / modB**2, x=zarr ), x=tarr ), x=sarr )
         
         return betavol / vols
     else:
-        for ivol in range(0,nvol-1):
+        for ivol in range(0,nvol):
             if ivol==0: sarr=np.linspace(-0.999,1, ns)
             if ivol!=0: sarr=np.linspace(-1,    1, ns)
 
             vols[ivol] = self.get_volume( ivol )
 
             _, _, sg, g = self.get_grid_and_jacobian_and_metric(
                 lvol=ivol, sarr=sarr, tarr=tarr, zarr=zarr
```

### Comparing `py_spec-3.3.0/py_spec/output/spec.py` & `py_spec-3.3.2/py_spec/output/spec.py`

 * *Files identical despite different names*

### Comparing `py_spec-3.3.0/py_spec.egg-info/PKG-INFO` & `py_spec-3.3.2/py_spec.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-spec
-Version: 3.3.0
+Version: 3.3.2
 Summary: SPEC(Stepped-Pressure Equilibrium Code) python utilities
 Home-page: https://princetonuniversity.github.io/SPEC/
 Author: SPEC developers
 License: GNU 3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `py_spec-3.3.0/setup.py` & `py_spec-3.3.2/setup.py`

 * *Files identical despite different names*

