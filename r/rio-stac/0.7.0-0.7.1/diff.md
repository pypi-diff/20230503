# Comparing `tmp/rio-stac-0.7.0.tar.gz` & `tmp/rio-stac-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rio-stac-0.7.0.tar", last modified: Tue Apr  4 22:18:48 2023, max compression
+gzip compressed data, was "rio-stac-0.7.1.tar", last modified: Wed May  3 19:06:41 2023, max compression
```

## Comparing `rio-stac-0.7.0.tar` & `rio-stac-0.7.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      212 2023-04-04 22:18:33.697752 rio-stac-0.7.0/.bumpversion.cfg
--rw-r--r--   0        0        0     1172 2023-04-04 22:18:33.697752 rio-stac-0.7.0/.gitignore
--rw-r--r--   0        0        0      822 2023-04-04 22:18:33.697752 rio-stac-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1073 2023-04-04 22:18:33.697752 rio-stac-0.7.0/LICENSE
--rw-r--r--   0        0        0     5232 2023-04-04 22:18:33.697752 rio-stac-0.7.0/README.md
--rw-r--r--   0        0        0     2127 2023-04-04 22:18:33.697752 rio-stac-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      127 2023-04-04 22:18:33.697752 rio-stac-0.7.0/rio_stac/__init__.py
--rw-r--r--   0        0        0       28 2023-04-04 22:18:33.697752 rio-stac-0.7.0/rio_stac/scripts/__init__.py
--rw-r--r--   0        0        0     4782 2023-04-04 22:18:33.697752 rio-stac-0.7.0/rio_stac/scripts/cli.py
--rw-r--r--   0        0        0    13887 2023-04-04 22:18:33.697752 rio-stac-0.7.0/rio_stac/stac.py
--rw-r--r--   0        0        0     6503 1970-01-01 00:00:00.000000 rio-stac-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      212 2023-05-03 19:06:28.322383 rio-stac-0.7.1/.bumpversion.cfg
+-rw-r--r--   0        0        0     1172 2023-05-03 19:06:28.322383 rio-stac-0.7.1/.gitignore
+-rw-r--r--   0        0        0      822 2023-05-03 19:06:28.322383 rio-stac-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1073 2023-05-03 19:06:28.322383 rio-stac-0.7.1/LICENSE
+-rw-r--r--   0        0        0     5232 2023-05-03 19:06:28.322383 rio-stac-0.7.1/README.md
+-rw-r--r--   0        0        0     2127 2023-05-03 19:06:28.322383 rio-stac-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      127 2023-05-03 19:06:28.326383 rio-stac-0.7.1/rio_stac/__init__.py
+-rw-r--r--   0        0        0       28 2023-05-03 19:06:28.326383 rio-stac-0.7.1/rio_stac/scripts/__init__.py
+-rw-r--r--   0        0        0     4801 2023-05-03 19:06:28.326383 rio-stac-0.7.1/rio_stac/scripts/cli.py
+-rw-r--r--   0        0        0    13889 2023-05-03 19:06:28.326383 rio-stac-0.7.1/rio_stac/stac.py
+-rw-r--r--   0        0        0     6503 1970-01-01 00:00:00.000000 rio-stac-0.7.1/PKG-INFO
```

### Comparing `rio-stac-0.7.0/.gitignore` & `rio-stac-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `rio-stac-0.7.0/.pre-commit-config.yaml` & `rio-stac-0.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rio-stac-0.7.0/LICENSE` & `rio-stac-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rio-stac-0.7.0/README.md` & `rio-stac-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `rio-stac-0.7.0/pyproject.toml` & `rio-stac-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rio-stac-0.7.0/rio_stac/scripts/cli.py` & `rio-stac-0.7.1/rio_stac/scripts/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,16 @@
     "--densify-geom",
     type=int,
     help="Densifies the number of points on each edges of the polygon geometry to account for non-linear transformation.",
 )
 @click.option(
     "--geom-precision",
     type=int,
-    help="Round geometry coordinates to this number of decimal.",
+    default=-1,
+    help="Round geometry coordinates to this number of decimal. By default, coordinates will not be rounded",
 )
 @click.option("--output", "-o", type=click.Path(exists=False), help="Output file name")
 @click.option(
     "--config",
     "config",
     metavar="NAME=VALUE",
     multiple=True,
@@ -133,15 +134,14 @@
     geom_precision,
     output,
     config,
 ):
     """Rasterio STAC plugin: Create a STAC Item for raster dataset."""
     property = property or {}
     densify_geom = densify_geom or 0
-    geom_precision = geom_precision or 0
 
     if input_datetime:
         if "/" in input_datetime:
             start_datetime, end_datetime = input_datetime.split("/")
             property["start_datetime"] = datetime_to_str(
                 str_to_datetime(start_datetime)
             )
```

### Comparing `rio-stac-0.7.0/rio_stac/stac.py` & `rio-stac-0.7.1/rio_stac/stac.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         ],
     }
 
 
 def get_dataset_geom(
     src_dst: Union[DatasetReader, DatasetWriter, WarpedVRT, MemoryFile],
     densify_pts: int = 0,
-    precision: int = 0,
+    precision: int = -1,
 ) -> Dict:
     """Get Raster Footprint."""
     if densify_pts < 0:
         raise ValueError("`densify_pts` must be positive")
 
     if src_dst.crs is not None:
         # 1. Create Polygon from raster bounds
@@ -277,15 +277,15 @@
     asset_media_type: Optional[Union[str, pystac.MediaType]] = "auto",
     asset_href: Optional[str] = None,
     with_proj: bool = False,
     with_raster: bool = False,
     with_eo: bool = False,
     raster_max_size: int = 1024,
     geom_densify_pts: int = 0,
-    geom_precision: int = 0,
+    geom_precision: int = -1,
 ) -> pystac.Item:
     """Create a Stac Item.
 
     Args:
         source (str or opened rasterio dataset): input path or rasterio dataset.
         input_datetime (datetime.datetime, optional): datetime associated with the item.
         extensions (list of str): input list of extensions to use in the item.
```

### Comparing `rio-stac-0.7.0/PKG-INFO` & `rio-stac-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rio-stac
-Version: 0.7.0
+Version: 0.7.1
 Summary: Create STAC Items from raster datasets.
 Author-email: Vincent Sarago <vincent@developmentseed.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rio-stac Version: 0.7.0 Summary: Create STAC Items
+Metadata-Version: 2.1 Name: rio-stac Version: 0.7.1 Summary: Create STAC Items
 from raster datasets. Author-email: Vincent Sarago
 developmentseed.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
```

