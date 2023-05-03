# Comparing `tmp/pypotlib-0.0.8.tar.gz` & `tmp/pypotlib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypotlib-0.0.8.tar", last modified: Wed May  3 14:23:40 2023, max compression
+gzip compressed data, was "pypotlib-0.0.9.tar", last modified: Wed May  3 15:05:59 2023, max compression
```

## Comparing `pypotlib-0.0.8.tar` & `pypotlib-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 pypotlib-0.0.8/.clang-format
--rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 pypotlib-0.0.8/.github/workflows/build_test.yml
--rw-r--r--   0        0        0     2502 1970-01-01 00:00:00.000000 pypotlib-0.0.8/.github/workflows/build_wheels.yml
--rw-r--r--   0        0        0     5227 1970-01-01 00:00:00.000000 pypotlib-0.0.8/.gitignore
--rw-r--r--   0        0        0     1242 1970-01-01 00:00:00.000000 pypotlib-0.0.8/.nb/aseCuH2slab.md
--rw-r--r--   0        0        0     6534 1970-01-01 00:00:00.000000 pypotlib-0.0.8/.nb/data/cuh2/init.con
--rw-r--r--   0        0        0    16761 1970-01-01 00:00:00.000000 pypotlib-0.0.8/.nb/data/cuh2/init_shift.con
--rw-r--r--   0        0        0     6534 1970-01-01 00:00:00.000000 pypotlib-0.0.8/.nb/data/cuh2/min1_0Cu.con
--rw-r--r--   0        0        0    16761 1970-01-01 00:00:00.000000 pypotlib-0.0.8/.nb/data/cuh2/min1_0Cu_shift.con
--rw-r--r--   0        0        0     6534 1970-01-01 00:00:00.000000 pypotlib-0.0.8/.nb/data/cuh2/min2_0Cu.con
--rw-r--r--   0        0        0    16761 1970-01-01 00:00:00.000000 pypotlib-0.0.8/.nb/data/cuh2/min2_0Cu_shift.con
--rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 pypotlib-0.0.8/CODEOWNERS
--rw-r--r--   0        0        0     5488 1970-01-01 00:00:00.000000 pypotlib-0.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1117 1970-01-01 00:00:00.000000 pypotlib-0.0.8/LICENSE
--rw-r--r--   0        0        0     2978 1970-01-01 00:00:00.000000 pypotlib-0.0.8/README.md
--rw-r--r--   0        0        0      358 1970-01-01 00:00:00.000000 pypotlib-0.0.8/environment.yml
--rw-r--r--   0        0        0     1929 1970-01-01 00:00:00.000000 pypotlib-0.0.8/meson.build
--rw-r--r--   0        0        0      223 1970-01-01 00:00:00.000000 pypotlib-0.0.8/pyb11_srcs/CuH2/py_cuh2pot.cc
--rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 pypotlib-0.0.8/pyb11_srcs/CuH2/py_cuh2pot.hpp
--rw-r--r--   0        0        0      211 1970-01-01 00:00:00.000000 pypotlib-0.0.8/pyb11_srcs/LennardJones/py_ljpot.cc
--rw-r--r--   0        0        0     1219 1970-01-01 00:00:00.000000 pypotlib-0.0.8/pyb11_srcs/LennardJones/py_ljpot.hpp
--rw-r--r--   0        0        0      231 1970-01-01 00:00:00.000000 pypotlib-0.0.8/pyb11_srcs/py_potential.cc
--rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 pypotlib-0.0.8/pyb11_srcs/py_potential.hpp
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 pypotlib-0.0.8/pyb11_srcs/py_pottypes.cc
--rw-r--r--   0        0        0      151 1970-01-01 00:00:00.000000 pypotlib-0.0.8/pyb11_srcs/py_wrapper.cc
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 pypotlib-0.0.8/pyb11_srcs/py_wrapper.hpp
--rw-r--r--   0        0        0       26 1970-01-01 00:00:00.000000 pypotlib-0.0.8/pypotlib/__init__.py
--rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 pypotlib-0.0.8/pypotlib/ase_adapters.py
--rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 pypotlib-0.0.8/pypotlib/aux.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 pypotlib-0.0.8/pypotlib/systems/__init__.py
--rw-r--r--   0        0        0     3488 1970-01-01 00:00:00.000000 pypotlib-0.0.8/pypotlib/systems/cu_slab_h2.py
--rw-r--r--   0        0        0     1422 1970-01-01 00:00:00.000000 pypotlib-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      112 1970-01-01 00:00:00.000000 pypotlib-0.0.8/subprojects/potlib.wrap
--rw-r--r--   0        0        0     3379 1970-01-01 00:00:00.000000 pypotlib-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 pypotlib-0.0.9/.clang-format
+-rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 pypotlib-0.0.9/.github/workflows/build_test.yml
+-rw-r--r--   0        0        0     2744 1970-01-01 00:00:00.000000 pypotlib-0.0.9/.github/workflows/build_wheels.yml
+-rw-r--r--   0        0        0     5227 1970-01-01 00:00:00.000000 pypotlib-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1242 1970-01-01 00:00:00.000000 pypotlib-0.0.9/.nb/aseCuH2slab.md
+-rw-r--r--   0        0        0     6534 1970-01-01 00:00:00.000000 pypotlib-0.0.9/.nb/data/cuh2/init.con
+-rw-r--r--   0        0        0    16761 1970-01-01 00:00:00.000000 pypotlib-0.0.9/.nb/data/cuh2/init_shift.con
+-rw-r--r--   0        0        0     6534 1970-01-01 00:00:00.000000 pypotlib-0.0.9/.nb/data/cuh2/min1_0Cu.con
+-rw-r--r--   0        0        0    16761 1970-01-01 00:00:00.000000 pypotlib-0.0.9/.nb/data/cuh2/min1_0Cu_shift.con
+-rw-r--r--   0        0        0     6534 1970-01-01 00:00:00.000000 pypotlib-0.0.9/.nb/data/cuh2/min2_0Cu.con
+-rw-r--r--   0        0        0    16761 1970-01-01 00:00:00.000000 pypotlib-0.0.9/.nb/data/cuh2/min2_0Cu_shift.con
+-rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 pypotlib-0.0.9/CODEOWNERS
+-rw-r--r--   0        0        0     5488 1970-01-01 00:00:00.000000 pypotlib-0.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1117 1970-01-01 00:00:00.000000 pypotlib-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2978 1970-01-01 00:00:00.000000 pypotlib-0.0.9/README.md
+-rw-r--r--   0        0        0      358 1970-01-01 00:00:00.000000 pypotlib-0.0.9/environment.yml
+-rw-r--r--   0        0        0     1929 1970-01-01 00:00:00.000000 pypotlib-0.0.9/meson.build
+-rw-r--r--   0        0        0      223 1970-01-01 00:00:00.000000 pypotlib-0.0.9/pyb11_srcs/CuH2/py_cuh2pot.cc
+-rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 pypotlib-0.0.9/pyb11_srcs/CuH2/py_cuh2pot.hpp
+-rw-r--r--   0        0        0      211 1970-01-01 00:00:00.000000 pypotlib-0.0.9/pyb11_srcs/LennardJones/py_ljpot.cc
+-rw-r--r--   0        0        0     1219 1970-01-01 00:00:00.000000 pypotlib-0.0.9/pyb11_srcs/LennardJones/py_ljpot.hpp
+-rw-r--r--   0        0        0      231 1970-01-01 00:00:00.000000 pypotlib-0.0.9/pyb11_srcs/py_potential.cc
+-rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 pypotlib-0.0.9/pyb11_srcs/py_potential.hpp
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 pypotlib-0.0.9/pyb11_srcs/py_pottypes.cc
+-rw-r--r--   0        0        0      151 1970-01-01 00:00:00.000000 pypotlib-0.0.9/pyb11_srcs/py_wrapper.cc
+-rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 pypotlib-0.0.9/pyb11_srcs/py_wrapper.hpp
+-rw-r--r--   0        0        0       26 1970-01-01 00:00:00.000000 pypotlib-0.0.9/pypotlib/__init__.py
+-rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 pypotlib-0.0.9/pypotlib/ase_adapters.py
+-rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 pypotlib-0.0.9/pypotlib/aux.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 pypotlib-0.0.9/pypotlib/systems/__init__.py
+-rw-r--r--   0        0        0     3488 1970-01-01 00:00:00.000000 pypotlib-0.0.9/pypotlib/systems/cu_slab_h2.py
+-rw-r--r--   0        0        0     1422 1970-01-01 00:00:00.000000 pypotlib-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      112 1970-01-01 00:00:00.000000 pypotlib-0.0.9/subprojects/potlib.wrap
+-rw-r--r--   0        0        0     3379 1970-01-01 00:00:00.000000 pypotlib-0.0.9/PKG-INFO
```

### Comparing `pypotlib-0.0.8/.clang-format` & `pypotlib-0.0.9/.clang-format`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.8/.github/workflows/build_wheels.yml` & `pypotlib-0.0.9/.github/workflows/build_wheels.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 # Build on every branch push, tag push, and pull request change:
 # From: https://github.com/pypa/cibuildwheel/blob/main/examples/github-deploy.yml
 name: Build wheels
 on: [push, pull_request]
 
 jobs:
   build_wheels:
-    name: Build wheel for ${{ matrix.python }}-${{ matrix.buildplat[1] }}
+    name: Build wheel for ${{ matrix.python[1] }}-${{ matrix.buildplat[1] }}
     runs-on: ${{ matrix.buildplat[0] }}
     environment: pypi
     strategy:
       # Ensure that a wheel builder finishes even if another fails
       fail-fast: false
       matrix:
         # From NumPy
         # Github Actions doesn't support pairing matrix values together, let's improvise
         # https://github.com/github/feedback/discussions/7835#discussioncomment-1769026
         buildplat:
           - [ubuntu-20.04, manylinux_x86_64]
           - [ubuntu-20.04, musllinux_x86_64] # No OpenBlas, no test
           - [macos-12, macosx_x86_64]
           # - [windows-2019, win_amd64]
-        python: ["cp38", "cp39", "cp310", "cp311"]
+        python:
+          - ["3.8", "cp38"]
+          - ["3.9", "cp39"]
+          - ["3.10", "cp310"]
+          - ["3.11", "cp311"]
 
     steps:
       - uses: actions/checkout@v3
 
+      - name: Setup 🐍 ${{ matrix.python[0] }}
+        uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.python[0] }}
+
       - name: Build wheels
         uses: pypa/cibuildwheel@v2.12.3
         env:
-          CIBW_BUILD: ${{ matrix.python }}-${{ matrix.buildplat[1] }}
+          CIBW_BUILD: ${{ matrix.python[1] }}-${{ matrix.buildplat[1] }}
 
       - uses: actions/upload-artifact@v3
         with:
-          name: ${{ matrix.python }}-${{ startsWith(matrix.buildplat[1], 'macosx') && 'macosx' || matrix.buildplat[1] }}
+          name: ${{ matrix.python[1] }}-${{ startsWith(matrix.buildplat[1], 'macosx') && 'macosx' || matrix.buildplat[1] }}
           path: ./wheelhouse/*.whl
 
   build_sdist:
     name: Build source distribution
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pypotlib-0.0.8/.gitignore` & `pypotlib-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.8/.nb/aseCuH2slab.md` & `pypotlib-0.0.9/.nb/aseCuH2slab.md`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.8/.nb/data/cuh2/init.con` & `pypotlib-0.0.9/.nb/data/cuh2/init.con`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.8/.nb/data/cuh2/init_shift.con` & `pypotlib-0.0.9/.nb/data/cuh2/init_shift.con`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.8/.nb/data/cuh2/min1_0Cu.con` & `pypotlib-0.0.9/.nb/data/cuh2/min1_0Cu.con`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.8/.nb/data/cuh2/min1_0Cu_shift.con` & `pypotlib-0.0.9/.nb/data/cuh2/min1_0Cu_shift.con`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.8/.nb/data/cuh2/min2_0Cu.con` & `pypotlib-0.0.9/.nb/data/cuh2/min2_0Cu.con`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.8/.nb/data/cuh2/min2_0Cu_shift.con` & `pypotlib-0.0.9/.nb/data/cuh2/min2_0Cu_shift.con`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.8/CODEOWNERS` & `pypotlib-0.0.9/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.8/CODE_OF_CONDUCT.md` & `pypotlib-0.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.8/LICENSE` & `pypotlib-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.8/README.md` & `pypotlib-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.8/meson.build` & `pypotlib-0.0.9/meson.build`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 project('pypotlib', 'cpp',
-       version: '0.0.8',
+       version: '0.0.9',
   default_options : ['warning_level=2', 'cpp_std=c++17'])
 # IMPORTANT!! warning_level=3 passes -fimplicit-none
 # Many of the older Fortran codes need implicit typing
 
 host_system = host_machine.system()
 
 # Add C++ compiler options
```

### Comparing `pypotlib-0.0.8/pyb11_srcs/CuH2/py_cuh2pot.hpp` & `pypotlib-0.0.9/pyb11_srcs/CuH2/py_cuh2pot.hpp`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.8/pyb11_srcs/LennardJones/py_ljpot.hpp` & `pypotlib-0.0.9/pyb11_srcs/LennardJones/py_ljpot.hpp`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.8/pyb11_srcs/py_potential.hpp` & `pypotlib-0.0.9/pyb11_srcs/py_potential.hpp`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.8/pyb11_srcs/py_wrapper.hpp` & `pypotlib-0.0.9/pyb11_srcs/py_wrapper.hpp`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.8/pypotlib/ase_adapters.py` & `pypotlib-0.0.9/pypotlib/ase_adapters.py`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.8/pypotlib/systems/cu_slab_h2.py` & `pypotlib-0.0.9/pypotlib/systems/cu_slab_h2.py`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.8/pyproject.toml` & `pypotlib-0.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm]
 
 [project]
 name = "pypotlib"
-version = "0.0.8"
+version = "0.0.9"
 description = "Python bindings and ASE adapters for potlib"
 authors = [
     {name = "Rohit Goswami", email = "rog32@hi.is"},
 ]
 # These are only if ase integration is requested, consider a group
 dependencies = [
     "numpy",
```

### Comparing `pypotlib-0.0.8/PKG-INFO` & `pypotlib-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypotlib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python bindings and ASE adapters for potlib
 Author-Email: Rohit Goswami <rog32@hi.is>
 License: MIT
 Project-URL: Source code, https://github.com/TheochemUI/pypotlib
 Project-URL: Bug tracker, https://github.com/TheochemUI/pypotlib/issues
 Requires-Python: >=3.8
 Requires-Dist: numpy
```

