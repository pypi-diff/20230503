# Comparing `tmp/ansys_materials_manager-0.2.2.tar.gz` & `tmp/ansys_materials_manager-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_materials_manager-0.2.2.tar", max compression
+gzip compressed data, was "ansys_materials_manager-0.2.3.tar", max compression
```

## Comparing `ansys_materials_manager-0.2.2.tar` & `ansys_materials_manager-0.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1089 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/LICENSE
--rw-r--r--   0        0        0     6343 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/README.rst
--rw-r--r--   0        0        0     2119 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      368 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/__init__.py
--rw-r--r--   0        0        0      512 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/_models/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/_models/_common/__init__.py
--rw-r--r--   0        0        0     2111 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/_models/_common/_base.py
--rw-r--r--   0        0        0      480 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/_models/_common/_exceptions.py
--rw-r--r--   0        0        0      189 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/_models/_common/_packages.py
--rw-r--r--   0        0        0     3974 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/_models/_common/constant.py
--rw-r--r--   0        0        0     6199 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/_models/_common/piecewise_linear.py
--rw-r--r--   0        0        0     6052 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/_models/_common/polynomial.py
--rw-r--r--   0        0        0        0 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/_models/_fluent/__init__.py
--rw-r--r--   0        0        0     2981 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/_models/_fluent/ideal_gas.py
--rw-r--r--   0        0        0      334 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/_models/_fluent/simple_properties.py
--rw-r--r--   0        0        0        0 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/_models/_mapdl/__init__.py
--rw-r--r--   0        0        0    14912 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/_models/_mapdl/anisotropic_elasticity.py
--rw-r--r--   0        0        0     2033 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/_models/_mapdl/simple_properties.py
--rw-r--r--   0        0        0        0 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/_models/py.typed
--rw-r--r--   0        0        0     2967 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/material.py
--rw-r--r--   0        0        0     3070 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/material_manager.py
--rw-r--r--   0        0        0     1495 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/serialize.py
--rw-r--r--   0        0        0        0 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/util/__init__.py
--rw-r--r--   0        0        0     2972 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/util/common.py
--rw-r--r--   0        0        0        0 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/util/mapdl/__init__.py
--rw-r--r--   0        0        0     1073 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/util/mapdl/mapdl_reader.py
--rw-r--r--   0        0        0     6565 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/util/mapdl/mpdata_parser.py
--rw-r--r--   0        0        0     3217 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/util/mapdl/tbdata_parser.py
--rw-r--r--   0        0        0      117 2023-04-20 12:28:04.172807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/util/matml/__init__.py
--rw-r--r--   0        0        0     9501 2023-04-20 12:28:04.176807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/util/matml/matml_from_material.py
--rw-r--r--   0        0        0     7378 2023-04-20 12:28:04.176807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/util/matml/matml_parser.py
--rw-r--r--   0        0        0     2993 2023-04-20 12:28:04.176807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/util/matml/matml_property_map.py
--rw-r--r--   0        0        0     3081 2023-04-20 12:28:04.176807 ansys_materials_manager-0.2.2/src/ansys/materials/manager/util/matml/matml_to_material.py
--rw-r--r--   0        0        0     7963 1970-01-01 00:00:00.000000 ansys_materials_manager-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-05-03 15:33:54.742359 ansys_materials_manager-0.2.3/LICENSE
+-rw-r--r--   0        0        0     6343 2023-05-03 15:33:54.742359 ansys_materials_manager-0.2.3/README.rst
+-rw-r--r--   0        0        0     2028 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      368 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/__init__.py
+-rw-r--r--   0        0        0      512 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/_models/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/_models/_common/__init__.py
+-rw-r--r--   0        0        0     2111 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/_models/_common/_base.py
+-rw-r--r--   0        0        0      480 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/_models/_common/_exceptions.py
+-rw-r--r--   0        0        0      189 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/_models/_common/_packages.py
+-rw-r--r--   0        0        0     3974 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/_models/_common/constant.py
+-rw-r--r--   0        0        0     6199 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/_models/_common/piecewise_linear.py
+-rw-r--r--   0        0        0     6052 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/_models/_common/polynomial.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/_models/_fluent/__init__.py
+-rw-r--r--   0        0        0     2981 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/_models/_fluent/ideal_gas.py
+-rw-r--r--   0        0        0      334 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/_models/_fluent/simple_properties.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/_models/_mapdl/__init__.py
+-rw-r--r--   0        0        0    14912 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/_models/_mapdl/anisotropic_elasticity.py
+-rw-r--r--   0        0        0     2033 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/_models/_mapdl/simple_properties.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/_models/py.typed
+-rw-r--r--   0        0        0     2967 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/material.py
+-rw-r--r--   0        0        0     3070 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/material_manager.py
+-rw-r--r--   0        0        0     1495 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/serialize.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/util/__init__.py
+-rw-r--r--   0        0        0     2972 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/util/common.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/util/mapdl/__init__.py
+-rw-r--r--   0        0        0     1073 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/util/mapdl/mapdl_reader.py
+-rw-r--r--   0        0        0     6565 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/util/mapdl/mpdata_parser.py
+-rw-r--r--   0        0        0     3217 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/util/mapdl/tbdata_parser.py
+-rw-r--r--   0        0        0      117 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/util/matml/__init__.py
+-rw-r--r--   0        0        0     9501 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/util/matml/matml_from_material.py
+-rw-r--r--   0        0        0     7378 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/util/matml/matml_parser.py
+-rw-r--r--   0        0        0     2993 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/util/matml/matml_property_map.py
+-rw-r--r--   0        0        0     3081 2023-05-03 15:33:54.746359 ansys_materials_manager-0.2.3/src/ansys/materials/manager/util/matml/matml_to_material.py
+-rw-r--r--   0        0        0     7826 1970-01-01 00:00:00.000000 ansys_materials_manager-0.2.3/PKG-INFO
```

### Comparing `ansys_materials_manager-0.2.2/LICENSE` & `ansys_materials_manager-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.2/README.rst` & `ansys_materials_manager-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.2/pyproject.toml` & `ansys_materials_manager-0.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 # Check https://python-poetry.org/docs/pyproject/ for all available sections
 name = "ansys-materials-manager"
-version = "0.2.2"
+version = "0.2.3"
 description = "Python package to unify material management across the ansys portfolio"
 license = "MIT"
 authors = ["ANSYS, Inc. <ansys.support@ansys.com>"]
 maintainers = ["PyAnsys developers <pyansys.core@ansys.com>"]
 readme = "README.rst"
 repository = "https://github.com/pyansys/pymaterials-manager"
 documentation = "https://manager.materials.docs.pyansys.com"
@@ -22,16 +22,14 @@
 packages = [
     { include = "ansys", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 numpy = {python = ">3.8", version = "^1.24.2"}
-scipy = {python = ">3.8", version = "^1.9.3"}
-pandas = {python = ">3.8", version = "^2.0"}
 
 
 # Documentation dependencies
 ansys-sphinx-theme = {version = "==0.9.7", optional = true}
 importlib-metadata = {version = "^6.3", python = "<3.7"}
 numpydoc = {version = "==1.5.0", optional = true}
 Sphinx = {version = "==5.1.1", optional = true}
```

### Comparing `ansys_materials_manager-0.2.2/src/ansys/materials/manager/_models/__init__.py` & `ansys_materials_manager-0.2.3/src/ansys/materials/manager/_models/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.2/src/ansys/materials/manager/_models/_common/_base.py` & `ansys_materials_manager-0.2.3/src/ansys/materials/manager/_models/_common/_base.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.2/src/ansys/materials/manager/_models/_common/constant.py` & `ansys_materials_manager-0.2.3/src/ansys/materials/manager/_models/_common/constant.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.2/src/ansys/materials/manager/_models/_common/piecewise_linear.py` & `ansys_materials_manager-0.2.3/src/ansys/materials/manager/_models/_common/piecewise_linear.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.2/src/ansys/materials/manager/_models/_common/polynomial.py` & `ansys_materials_manager-0.2.3/src/ansys/materials/manager/_models/_common/polynomial.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.2/src/ansys/materials/manager/_models/_fluent/ideal_gas.py` & `ansys_materials_manager-0.2.3/src/ansys/materials/manager/_models/_fluent/ideal_gas.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.2/src/ansys/materials/manager/_models/_mapdl/anisotropic_elasticity.py` & `ansys_materials_manager-0.2.3/src/ansys/materials/manager/_models/_mapdl/anisotropic_elasticity.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.2/src/ansys/materials/manager/_models/_mapdl/simple_properties.py` & `ansys_materials_manager-0.2.3/src/ansys/materials/manager/_models/_mapdl/simple_properties.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.2/src/ansys/materials/manager/material.py` & `ansys_materials_manager-0.2.3/src/ansys/materials/manager/material.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.2/src/ansys/materials/manager/material_manager.py` & `ansys_materials_manager-0.2.3/src/ansys/materials/manager/material_manager.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.2/src/ansys/materials/manager/serialize.py` & `ansys_materials_manager-0.2.3/src/ansys/materials/manager/serialize.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.2/src/ansys/materials/manager/util/common.py` & `ansys_materials_manager-0.2.3/src/ansys/materials/manager/util/common.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.2/src/ansys/materials/manager/util/mapdl/mapdl_reader.py` & `ansys_materials_manager-0.2.3/src/ansys/materials/manager/util/mapdl/mapdl_reader.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.2/src/ansys/materials/manager/util/mapdl/mpdata_parser.py` & `ansys_materials_manager-0.2.3/src/ansys/materials/manager/util/mapdl/mpdata_parser.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.2/src/ansys/materials/manager/util/mapdl/tbdata_parser.py` & `ansys_materials_manager-0.2.3/src/ansys/materials/manager/util/mapdl/tbdata_parser.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.2/src/ansys/materials/manager/util/matml/matml_from_material.py` & `ansys_materials_manager-0.2.3/src/ansys/materials/manager/util/matml/matml_from_material.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.2/src/ansys/materials/manager/util/matml/matml_parser.py` & `ansys_materials_manager-0.2.3/src/ansys/materials/manager/util/matml/matml_parser.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.2/src/ansys/materials/manager/util/matml/matml_property_map.py` & `ansys_materials_manager-0.2.3/src/ansys/materials/manager/util/matml/matml_property_map.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.2/src/ansys/materials/manager/util/matml/matml_to_material.py` & `ansys_materials_manager-0.2.3/src/ansys/materials/manager/util/matml/matml_to_material.py`

 * *Files identical despite different names*

### Comparing `ansys_materials_manager-0.2.2/PKG-INFO` & `ansys_materials_manager-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-materials-manager
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python package to unify material management across the ansys portfolio
 Home-page: https://github.com/pyansys/pymaterials-manager
 License: MIT
 Author: ANSYS, Inc.
 Author-email: ansys.support@ansys.com
 Maintainer: PyAnsys developers
 Maintainer-email: pyansys.core@ansys.com
@@ -21,16 +21,14 @@
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: doc
 Requires-Dist: Sphinx (==5.1.1) ; extra == "doc"
 Requires-Dist: ansys-sphinx-theme (==0.9.7) ; extra == "doc"
 Requires-Dist: importlib-metadata (>=6.3,<7.0) ; python_version < "3.7"
 Requires-Dist: numpy (>=1.24.2,<2.0.0) ; python_full_version > "3.8.0"
 Requires-Dist: numpydoc (==1.5.0) ; extra == "doc"
-Requires-Dist: pandas (>=2.0,<3.0) ; python_full_version > "3.8.0"
-Requires-Dist: scipy (>=1.9.3,<2.0.0) ; python_full_version > "3.8.0"
 Requires-Dist: sphinx-autoapi (==2.0.1) ; extra == "doc"
 Requires-Dist: sphinx-copybutton (==0.5.2) ; extra == "doc"
 Project-URL: Documentation, https://manager.materials.docs.pyansys.com
 Project-URL: Repository, https://github.com/pyansys/pymaterials-manager
 Description-Content-Type: text/x-rst
 
 PyMaterials Manager
```

