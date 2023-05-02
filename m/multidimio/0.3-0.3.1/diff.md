# Comparing `tmp/multidimio-0.3.tar.gz` & `tmp/multidimio-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidimio-0.3.tar", max compression
+gzip compressed data, was "multidimio-0.3.1.tar", max compression
```

## Comparing `multidimio-0.3.tar` & `multidimio-0.3.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    10203 2023-05-02 22:26:43.331880 multidimio-0.3/LICENSE
--rw-r--r--   0        0        0     6043 2023-05-02 22:26:43.331880 multidimio-0.3/README.md
--rw-r--r--   0        0        0     2859 2023-05-02 22:27:06.088113 multidimio-0.3/pyproject.toml
--rw-r--r--   0        0        0      474 2023-05-02 22:26:43.351881 multidimio-0.3/src/mdio/__init__.py
--rw-r--r--   0        0        0     2697 2023-05-02 22:26:43.351881 multidimio-0.3/src/mdio/__main__.py
--rw-r--r--   0        0        0      127 2023-05-02 22:26:43.351881 multidimio-0.3/src/mdio/api/__init__.py
--rw-r--r--   0        0        0    24779 2023-05-02 22:26:43.351881 multidimio-0.3/src/mdio/api/accessor.py
--rw-r--r--   0        0        0     2322 2023-05-02 22:26:43.351881 multidimio-0.3/src/mdio/api/convenience.py
--rw-r--r--   0        0        0     4451 2023-05-02 22:26:43.351881 multidimio-0.3/src/mdio/api/io_utils.py
--rw-r--r--   0        0        0      105 2023-05-02 22:26:43.351881 multidimio-0.3/src/mdio/commands/__init__.py
--rw-r--r--   0        0        0    10623 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/commands/segy.py
--rw-r--r--   0        0        0      529 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/constants.py
--rw-r--r--   0        0        0      141 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/converters/__init__.py
--rw-r--r--   0        0        0      597 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/converters/exceptions.py
--rw-r--r--   0        0        0     6510 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/converters/mdio.py
--rw-r--r--   0        0        0    12386 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/converters/segy.py
--rw-r--r--   0        0        0      143 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/core/__init__.py
--rw-r--r--   0        0        0     3811 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/core/dimension.py
--rw-r--r--   0        0        0      268 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/core/exceptions.py
--rw-r--r--   0        0        0     3765 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/core/grid.py
--rw-r--r--   0        0        0     2917 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/core/indexing.py
--rw-r--r--   0        0        0     2727 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/core/serialization.py
--rw-r--r--   0        0        0      429 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/core/utils_write.py
--rw-r--r--   0        0        0     1646 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/py.typed
--rw-r--r--   0        0        0       44 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/__init__.py
--rw-r--r--   0        0        0      636 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/_standards_common.py
--rw-r--r--   0        0        0     9384 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/_standards_rev0.py
--rw-r--r--   0        0        0     7560 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/_workers.py
--rw-r--r--   0        0        0    11173 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/blocked_io.py
--rw-r--r--   0        0        0     1760 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/byte_utils.py
--rw-r--r--   0        0        0     9396 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/creation.py
--rw-r--r--   0        0        0     4856 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/ebcdic.py
--rw-r--r--   0        0        0      181 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/exceptions.py
--rw-r--r--   0        0        0     2748 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/headers.py
--rw-r--r--   0        0        0     3561 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/headers_text.py
--rw-r--r--   0        0        0     3232 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/helpers_segy.py
--rw-r--r--   0        0        0     5785 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/ibm_float.py
--rw-r--r--   0        0        0     4393 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/parsers.py
--rw-r--r--   0        0        0     6160 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/utilities.py
--rw-r--r--   0        0        0     7673 1970-01-01 00:00:00.000000 multidimio-0.3/PKG-INFO
+-rw-r--r--   0        0        0    10203 2023-05-02 23:32:42.112554 multidimio-0.3.1/LICENSE
+-rw-r--r--   0        0        0     6043 2023-05-02 23:32:42.112554 multidimio-0.3.1/README.md
+-rw-r--r--   0        0        0     2860 2023-05-02 23:32:58.152803 multidimio-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      474 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/__init__.py
+-rw-r--r--   0        0        0     2697 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/__main__.py
+-rw-r--r--   0        0        0      127 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/api/__init__.py
+-rw-r--r--   0        0        0    24779 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/api/accessor.py
+-rw-r--r--   0        0        0     2322 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/api/convenience.py
+-rw-r--r--   0        0        0     4451 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/api/io_utils.py
+-rw-r--r--   0        0        0      105 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/commands/__init__.py
+-rw-r--r--   0        0        0    10623 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/commands/segy.py
+-rw-r--r--   0        0        0      529 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/constants.py
+-rw-r--r--   0        0        0      141 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/converters/__init__.py
+-rw-r--r--   0        0        0      597 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/converters/exceptions.py
+-rw-r--r--   0        0        0     6510 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/converters/mdio.py
+-rw-r--r--   0        0        0    12386 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/converters/segy.py
+-rw-r--r--   0        0        0      143 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/core/__init__.py
+-rw-r--r--   0        0        0     3811 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/core/dimension.py
+-rw-r--r--   0        0        0      268 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/core/exceptions.py
+-rw-r--r--   0        0        0     3765 2023-05-02 23:32:42.128554 multidimio-0.3.1/src/mdio/core/grid.py
+-rw-r--r--   0        0        0     2917 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/core/indexing.py
+-rw-r--r--   0        0        0     2727 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/core/serialization.py
+-rw-r--r--   0        0        0      429 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/core/utils_write.py
+-rw-r--r--   0        0        0     1646 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/py.typed
+-rw-r--r--   0        0        0       44 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/__init__.py
+-rw-r--r--   0        0        0      636 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/_standards_common.py
+-rw-r--r--   0        0        0     9384 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/_standards_rev0.py
+-rw-r--r--   0        0        0     7560 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/_workers.py
+-rw-r--r--   0        0        0    11173 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/blocked_io.py
+-rw-r--r--   0        0        0     1760 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/byte_utils.py
+-rw-r--r--   0        0        0     9396 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/creation.py
+-rw-r--r--   0        0        0     4856 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/ebcdic.py
+-rw-r--r--   0        0        0      181 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/exceptions.py
+-rw-r--r--   0        0        0     2748 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/headers.py
+-rw-r--r--   0        0        0     3561 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/headers_text.py
+-rw-r--r--   0        0        0     3232 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/helpers_segy.py
+-rw-r--r--   0        0        0     5785 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/ibm_float.py
+-rw-r--r--   0        0        0     4393 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/parsers.py
+-rw-r--r--   0        0        0     6160 2023-05-02 23:32:42.132554 multidimio-0.3.1/src/mdio/segy/utilities.py
+-rw-r--r--   0        0        0     7731 1970-01-01 00:00:00.000000 multidimio-0.3.1/PKG-INFO
```

### Comparing `multidimio-0.3/LICENSE` & `multidimio-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/README.md` & `multidimio-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/pyproject.toml` & `multidimio-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multidimio"
-version = "0.3"
+version = "0.3.1"
 description = "Cloud-native, scalable, and user-friendly multi dimensional energy data!"
 authors = ["TGS <sys-opensource@tgs.com>"]
 maintainers = [
     "Altay Sansal <altay.sansal@tgs.com>",
     "Sri Kainkaryam <sribharath.kainkaryam@tgs.com>",
 ]
 license = "Apache-2.0"
@@ -34,15 +34,15 @@
 numba = ">=0.55.2,<1.0.0"
 psutil = "^5.9.1"
 distributed = {version = ">=2022.11.0", optional = true}
 bokeh = {version = "^2.4.3", optional = true}
 s3fs = {version = ">=2022.7.0", optional = true}
 gcsfs = {version = ">=2022.7.0", optional = true}
 adlfs = {version = ">=2022.7.0", optional = true}
-#zfpy = {version = "^1.0.0", optional = true}
+zfpy = {version = "^0.5.5", optional = true}
 
 [tool.poetry.extras]
 distributed = ["distributed", "bokeh"]
 cloud = ["s3fs", "gcsfs", "adlfs"]
 lossy = ["zfpy"]
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `multidimio-0.3/src/mdio/__main__.py` & `multidimio-0.3.1/src/mdio/__main__.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/api/accessor.py` & `multidimio-0.3.1/src/mdio/api/accessor.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/api/convenience.py` & `multidimio-0.3.1/src/mdio/api/convenience.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/api/io_utils.py` & `multidimio-0.3.1/src/mdio/api/io_utils.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/commands/segy.py` & `multidimio-0.3.1/src/mdio/commands/segy.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/constants.py` & `multidimio-0.3.1/src/mdio/constants.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/converters/exceptions.py` & `multidimio-0.3.1/src/mdio/converters/exceptions.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/converters/mdio.py` & `multidimio-0.3.1/src/mdio/converters/mdio.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/converters/segy.py` & `multidimio-0.3.1/src/mdio/converters/segy.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/core/dimension.py` & `multidimio-0.3.1/src/mdio/core/dimension.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/core/grid.py` & `multidimio-0.3.1/src/mdio/core/grid.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/core/indexing.py` & `multidimio-0.3.1/src/mdio/core/indexing.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/core/serialization.py` & `multidimio-0.3.1/src/mdio/core/serialization.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/exceptions.py` & `multidimio-0.3.1/src/mdio/exceptions.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/segy/_standards_common.py` & `multidimio-0.3.1/src/mdio/segy/_standards_common.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/segy/_standards_rev0.py` & `multidimio-0.3.1/src/mdio/segy/_standards_rev0.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/segy/_workers.py` & `multidimio-0.3.1/src/mdio/segy/_workers.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/segy/blocked_io.py` & `multidimio-0.3.1/src/mdio/segy/blocked_io.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/segy/byte_utils.py` & `multidimio-0.3.1/src/mdio/segy/byte_utils.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/segy/creation.py` & `multidimio-0.3.1/src/mdio/segy/creation.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/segy/ebcdic.py` & `multidimio-0.3.1/src/mdio/segy/ebcdic.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/segy/headers.py` & `multidimio-0.3.1/src/mdio/segy/headers.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/segy/headers_text.py` & `multidimio-0.3.1/src/mdio/segy/headers_text.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/segy/helpers_segy.py` & `multidimio-0.3.1/src/mdio/segy/helpers_segy.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/segy/ibm_float.py` & `multidimio-0.3.1/src/mdio/segy/ibm_float.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/segy/parsers.py` & `multidimio-0.3.1/src/mdio/segy/parsers.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/src/mdio/segy/utilities.py` & `multidimio-0.3.1/src/mdio/segy/utilities.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.3/PKG-INFO` & `multidimio-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidimio
-Version: 0.3
+Version: 0.3.1
 Summary: Cloud-native, scalable, and user-friendly multi dimensional energy data!
 Home-page: https://mdio.dev
 License: Apache-2.0
 Keywords: mdio,multidimio,seismic,wind,data
 Author: TGS
 Author-email: sys-opensource@tgs.com
 Maintainer: Altay Sansal
@@ -29,14 +29,15 @@
 Requires-Dist: gcsfs (>=2022.7.0) ; extra == "cloud"
 Requires-Dist: numba (>=0.55.2,<1.0.0)
 Requires-Dist: psutil (>=5.9.1,<6.0.0)
 Requires-Dist: s3fs (>=2022.7.0) ; extra == "cloud"
 Requires-Dist: segyio (>=1.9.3,<2.0.0)
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
 Requires-Dist: zarr (>=2.12.0,<3.0.0)
+Requires-Dist: zfpy (>=0.5.5,<0.6.0) ; extra == "lossy"
 Project-URL: Changelog, https://github.com/TGSAI/mdio-python/releases
 Project-URL: Documentation, https://mdio-python.readthedocs.io
 Project-URL: Repository, https://github.com/TGSAI/mdio-python
 Description-Content-Type: text/markdown
 
 <div>
   <img
```

