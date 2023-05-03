# Comparing `tmp/stactools-naip-0.3.1.tar.gz` & `tmp/stactools-naip-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stactools-naip-0.3.1.tar", last modified: Fri Feb 24 14:39:02 2023, max compression
+gzip compressed data, was "stactools-naip-0.3.2.tar", last modified: Wed May  3 18:24:13 2023, max compression
```

## Comparing `stactools-naip-0.3.1.tar` & `stactools-naip-0.3.2.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:39:02.337905 stactools-naip-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-02-24 14:38:45.000000 stactools-naip-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-02-24 14:39:02.337905 stactools-naip-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-02-24 14:38:45.000000 stactools-naip-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-24 14:38:45.000000 stactools-naip-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-02-24 14:39:02.337905 stactools-naip-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:39:02.333905 stactools-naip-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:39:02.333905 stactools-naip-0.3.1/src/stactools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:39:02.333905 stactools-naip-0.3.1/src/stactools/naip/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-02-24 14:38:45.000000 stactools-naip-0.3.1/src/stactools/naip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-02-24 14:38:45.000000 stactools-naip-0.3.1/src/stactools/naip/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-02-24 14:38:45.000000 stactools-naip-0.3.1/src/stactools/naip/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-02-24 14:38:45.000000 stactools-naip-0.3.1/src/stactools/naip/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-02-24 14:38:45.000000 stactools-naip-0.3.1/src/stactools/naip/stac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-02-24 14:38:45.000000 stactools-naip-0.3.1/src/stactools/naip/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:39:02.333905 stactools-naip-0.3.1/src/stactools_naip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-02-24 14:39:02.000000 stactools-naip-0.3.1/src/stactools_naip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-02-24 14:39:02.000000 stactools-naip-0.3.1/src/stactools_naip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 14:39:02.000000 stactools-naip-0.3.1/src/stactools_naip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-24 14:39:02.000000 stactools-naip-0.3.1/src/stactools_naip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-24 14:39:02.000000 stactools-naip-0.3.1/src/stactools_naip.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:39:02.337905 stactools-naip-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-02-24 14:38:45.000000 stactools-naip-0.3.1/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-02-24 14:38:45.000000 stactools-naip-0.3.1/tests/test_stac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-02-24 14:38:45.000000 stactools-naip-0.3.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:13.552901 stactools-naip-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-03 18:23:50.000000 stactools-naip-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-03 18:24:13.552901 stactools-naip-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-03 18:23:50.000000 stactools-naip-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-03 18:23:50.000000 stactools-naip-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-03 18:24:13.552901 stactools-naip-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:13.544901 stactools-naip-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:13.544901 stactools-naip-0.3.2/src/stactools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:13.548901 stactools-naip-0.3.2/src/stactools/naip/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-03 18:23:50.000000 stactools-naip-0.3.2/src/stactools/naip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-03 18:23:50.000000 stactools-naip-0.3.2/src/stactools/naip/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-03 18:23:50.000000 stactools-naip-0.3.2/src/stactools/naip/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-05-03 18:23:50.000000 stactools-naip-0.3.2/src/stactools/naip/stac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-03 18:23:50.000000 stactools-naip-0.3.2/src/stactools/naip/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:13.552901 stactools-naip-0.3.2/src/stactools_naip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-03 18:24:13.000000 stactools-naip-0.3.2/src/stactools_naip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-03 18:24:13.000000 stactools-naip-0.3.2/src/stactools_naip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 18:24:13.000000 stactools-naip-0.3.2/src/stactools_naip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 18:24:13.000000 stactools-naip-0.3.2/src/stactools_naip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 18:24:13.000000 stactools-naip-0.3.2/src/stactools_naip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:13.552901 stactools-naip-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-03 18:23:50.000000 stactools-naip-0.3.2/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-03 18:23:50.000000 stactools-naip-0.3.2/tests/test_stac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-03 18:23:50.000000 stactools-naip-0.3.2/tests/test_utils.py
```

### Comparing `stactools-naip-0.3.1/LICENSE` & `stactools-naip-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stactools-naip-0.3.1/PKG-INFO` & `stactools-naip-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-naip
-Version: 0.3.1
+Version: 0.3.2
 Summary: PROVIDE DESCRIPTION HERE
 Home-page: https://github.com/stactools-naips/stactools-naip
 Author: stac-utils
 Author-email: stac@radiant.earth
 Project-URL: Documentation, https://stactools-naip.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/stactools-naips/stactools-naip/issues
 Keywords: stactools,pystac,catalog,STAC
```

### Comparing `stactools-naip-0.3.1/README.md` & `stactools-naip-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `stactools-naip-0.3.1/setup.cfg` & `stactools-naip-0.3.2/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 [options]
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find_namespace:
 install_requires = 
 	stactools >= 0.4.3
+	pystac >= 1.5 # for GridExtension class
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `stactools-naip-0.3.1/src/stactools/naip/commands.py` & `stactools-naip-0.3.2/src/stactools/naip/commands.py`

 * *Files identical despite different names*

### Comparing `stactools-naip-0.3.1/src/stactools/naip/constants.py` & `stactools-naip-0.3.2/src/stactools/naip/constants.py`

 * *Files identical despite different names*

### Comparing `stactools-naip-0.3.1/src/stactools/naip/stac.py` & `stactools-naip-0.3.2/src/stactools/naip/stac.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 import re
 from datetime import timedelta
 from typing import Final, List, Optional, Pattern
 
 import fsspec
 import pystac
 import rasterio as rio
+import shapely
 from lxml import etree
 from pystac.extensions.eo import EOExtension
+from pystac.extensions.grid import GridExtension
 from pystac.extensions.item_assets import ItemAssetsExtension
 from pystac.extensions.projection import ProjectionExtension
 from pystac.extensions.raster import DataType, RasterBand, RasterExtension
 from pystac.extensions.scientific import CollectionScientificExtension, Publication
 from pystac.utils import str_to_datetime
-from shapely.geometry import box, mapping, shape
 from stactools.core.io import read_text
 from stactools.core.io.xml import XmlElement
 from stactools.core.projection import reproject_geom
 
 from stactools.naip import constants
-from stactools.naip.grid import GridExtension
 from stactools.naip.utils import (
     maybe_extract_id_and_date,
     parse_fgdc_metadata,
     process_xpath_resource_desc,
 )
 
 DOQQ_PATTERN: Final[Pattern[str]] = re.compile(r"[A-Za-z]{2}_m_(\d{7})_(ne|se|nw|sw)_")
@@ -134,15 +134,18 @@
     with rio.open(cog_href) as ds:
         gsd = round(ds.res[0], 1)
         epsg = int(ds.crs.to_authority()[1])
         image_shape = list(ds.shape)
         original_bbox = list(ds.bounds)
         transform = list(ds.transform)
         geom = reproject_geom(
-            ds.crs, "epsg:4326", mapping(box(*ds.bounds)), precision=6
+            ds.crs,
+            "epsg:4326",
+            shapely.geometry.mapping(shapely.geometry.box(*ds.bounds)),
+            precision=6,
         )
 
     if fgdc_metadata_href is not None:
         if year == "2020":
             first_xpath = "gmd:fileIdentifier/gco:CharacterString"
 
             second_xpath = "idinfo/citation/citeinfo/title"
@@ -194,15 +197,17 @@
         if res is not None:
             resource_desc, dt = res
         else:
             raise Exception(f"Failed to extract item resource_desc and dt: {cog_href}")
 
     item_id = naip_item_id(state, resource_desc)
 
-    bounds = list(shape(geom).bounds)
+    shapely_shape = shapely.geometry.shape(geom)
+    bounds = list(shapely_shape.bounds)
+    centroid = shapely_shape.centroid
 
     dt = dt + timedelta(hours=16)  # UTC is +4 ET, so is around 9-12 AM in CONUS
     properties = {"naip:state": state, "naip:year": year}
 
     item = pystac.Item(
         id=item_id, geometry=geom, bbox=bounds, datetime=dt, properties=properties
     )
@@ -218,14 +223,15 @@
 
     # Projection Extension
     projection = ProjectionExtension.ext(item, add_if_missing=True)
     projection.epsg = epsg
     projection.shape = image_shape
     projection.bbox = original_bbox
     projection.transform = transform
+    projection.centroid = {"lat": round(centroid.y, 5), "lon": round(centroid.x, 5)}
 
     # Grid Extension
     grid = GridExtension.ext(item, add_if_missing=True)
     if match := DOQQ_PATTERN.search(item_id):
         grid.code = f"DOQQ-{match.group(1)}{match.group(2).upper()}"
 
     # COG
```

### Comparing `stactools-naip-0.3.1/src/stactools/naip/utils.py` & `stactools-naip-0.3.2/src/stactools/naip/utils.py`

 * *Files identical despite different names*

### Comparing `stactools-naip-0.3.1/src/stactools_naip.egg-info/PKG-INFO` & `stactools-naip-0.3.2/src/stactools_naip.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-naip
-Version: 0.3.1
+Version: 0.3.2
 Summary: PROVIDE DESCRIPTION HERE
 Home-page: https://github.com/stactools-naips/stactools-naip
 Author: stac-utils
 Author-email: stac@radiant.earth
 Project-URL: Documentation, https://stactools-naip.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/stactools-naips/stactools-naip/issues
 Keywords: stactools,pystac,catalog,STAC
```

### Comparing `stactools-naip-0.3.1/tests/test_commands.py` & `stactools-naip-0.3.2/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `stactools-naip-0.3.1/tests/test_stac.py` & `stactools-naip-0.3.2/tests/test_stac.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import unittest
 from datetime import datetime
 
+import pytest
+from pystac.extensions.projection import ProjectionExtension
 from pystac.extensions.raster import DataType, RasterExtension
 from pystac.extensions.scientific import CollectionScientificExtension
 
 from stactools.naip.stac import create_collection, create_item
 from tests import test_data
 
 
@@ -34,14 +36,18 @@
         self.assertEqual(len(raster_ext.bands), 4)
         for raster_band in RasterExtension.ext(image_asset).bands:
             self.assertEqual(raster_band.nodata, 0)
             self.assertEqual(raster_band.spatial_resolution, item.properties["gsd"])
             self.assertEqual(raster_band.data_type, DataType.UINT8)
             self.assertEqual(raster_band.unit, "none")
 
+        projection = ProjectionExtension.ext(item)
+        projection.centroid["lat"] == pytest.approx(30.96876)
+        projection.centroid["lon"] == pytest.approx(-85.90624)
+
     # test stac on year = 2020
     def test_create_item_xml(self):
         item = create_item(
             "tx",
             "2020",
             test_data.get_path(
                 "data-files/m_3610332_se_13_060_20200903-downsampled.tif"
@@ -97,15 +103,14 @@
     # handles resource desc from xml (with and without ".tif" extension)
     # handles resource desc pulled from cog_href
     def test_create_item_xml_ext(self):
         for filename in [
             "data-files/m_3211605_ne_11_060_20200415_20200730.xml",
             "data-files/m_3211605_ne_11_060_20200415_20200730_missing_resource_desc.xml",
         ]:
-
             item = create_item(
                 "ca",
                 "2020",
                 test_data.get_path("data-files/m_3211605_ne_11_060_20200415.tif"),
                 test_data.get_path(filename),
             )
```

### Comparing `stactools-naip-0.3.1/tests/test_utils.py` & `stactools-naip-0.3.2/tests/test_utils.py`

 * *Files identical despite different names*

