# Comparing `tmp/raster2dggs-0.1.2.tar.gz` & `tmp/raster2dggs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster2dggs-0.1.2.tar", max compression
+gzip compressed data, was "raster2dggs-0.2.0.tar", max compression
```

## Comparing `raster2dggs-0.1.2.tar` & `raster2dggs-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     8160 2023-04-21 02:14:48.691969 raster2dggs-0.1.2/README.md
--rw-r--r--   0        0        0     1091 2023-04-21 02:14:35.259789 raster2dggs-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-15 20:09:40.034837 raster2dggs-0.1.2/raster2dggs/__init__.py
--rw-r--r--   0        0        0      520 2023-03-15 20:09:40.034837 raster2dggs-0.1.2/raster2dggs/cli.py
--rw-r--r--   0        0        0    14503 2023-04-21 02:05:36.690560 raster2dggs-0.1.2/raster2dggs/h3.py
--rw-r--r--   0        0        0     9579 1970-01-01 00:00:00.000000 raster2dggs-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     8362 2023-05-03 02:57:00.605422 raster2dggs-0.2.0/README.md
+-rw-r--r--   0        0        0     1091 2023-05-03 02:57:00.605422 raster2dggs-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-05-03 02:59:48.530270 raster2dggs-0.2.0/raster2dggs/__init__.py
+-rw-r--r--   0        0        0      599 2023-05-03 02:59:13.750096 raster2dggs-0.2.0/raster2dggs/cli.py
+-rw-r--r--   0        0        0    15356 2023-05-03 03:00:03.146344 raster2dggs-0.2.0/raster2dggs/h3.py
+-rw-r--r--   0        0        0     9781 1970-01-01 00:00:00.000000 raster2dggs-0.2.0/PKG-INFO
```

### Comparing `raster2dggs-0.1.2/README.md` & `raster2dggs-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,17 @@
   s3://).
 
 Options:
   -v, --verbosity LVL             Either CRITICAL, ERROR, WARNING, INFO or
                                   DEBUG  [default: INFO]
   -r, --resolution [0|1|2|3|4|5|6|7|8|9|10|11|12|13|14|15]
                                   H3 resolution to index  [required]
+  -pr,--parent_res [0|1|2|3|4|5|6|7|8|9|10|11|12|13|14|15]
+                                  H3 Parent resolution to index and aggregate
+                                  to. Defaults to resolution - 6
   -u, --upscale INTEGER           Upscaling factor, used to upsample input
                                   data on the fly; useful when the raster
                                   resolution is lower than the target DGGS
                                   resolution. Default (1) applies no
                                   upscaling. The resampling method controls
                                   interpolation.  [default: 1]
   -c, --compression [snappy|gzip|zstd]
@@ -144,17 +147,17 @@
 ## Citation
 
 ```bibtex
 @software{raster2dggs,
   title={{raster2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/raster2dggs},
-  version={0.1.2},
+  version={0.2.0},
   date={2023-02-09}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). raster2dggs (0.1.2) [Computer software]. https://github.com/manaakiwhenua/raster2dggs 
+> Ardo, J., & Law, R. (2023). raster2dggs (0.2.0) [Computer software]. https://github.com/manaakiwhenua/raster2dggs 
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/raster2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

### Comparing `raster2dggs-0.1.2/pyproject.toml` & `raster2dggs-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "raster2dggs"
-version = "0.1.2"
+version = "0.2.0"
 description = ""
 authors = ["James Ardo <ardoj@landcareresearch.co.nz>"]
 maintainers = ["Richard Law <lawr@landcareresearch.co.nz>"]
 readme = "README.md"
 license = "LGPL-3.0-or-later"
 repository = "https://github.com/manaakiwhenua/raster2dggs"
 keywords = ["dggs", "raster", "h3", "cli"]
@@ -15,15 +15,15 @@
     "Topic :: Scientific/Engineering :: Information Analysis"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 gdal = "^3.6.2"
 geopandas = "^0.12.2"
-h3pandas = "^0.2.3"
+h3pandas = "^0.2.4"
 rioxarray = "^0.13.4"
 dask-geopandas = "^0.3.0"
 pyarrow = "^11.0.0"
 dask = "^2023.3.0"
 click = "^8.1.3"
 boto3 = "^1.26.85"
 tqdm = "^4.65.0"
```

### Comparing `raster2dggs-0.1.2/raster2dggs/cli.py` & `raster2dggs-0.2.0/raster2dggs/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import click
 
+from raster2dggs import __version__
 from raster2dggs.h3 import h3
 
 #   If the program does terminal interaction, make it output a short
 # notice like this when it starts in an interactive mode:
 
 #     <program>  Copyright (C) <year>  <name of author>
 #     This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
 #     This is free software, and you are welcome to redistribute it
 #     under certain conditions; type `show c' for details.
 
 
 @click.group()
+@click.version_option(version=__version__)
 def cli():
     pass
 
 
 cli.add_command(h3)
```

### Comparing `raster2dggs-0.1.2/raster2dggs/h3.py` & `raster2dggs-0.2.0/raster2dggs/h3.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 from rasterio.vrt import WarpedVRT
 from rasterio.warp import calculate_default_transform
 import rioxarray
 from tqdm import tqdm
 from tqdm.dask import TqdmCallback
 import xarray as xr
 
+from raster2dggs import __version__
+
 LOGGER = logging.getLogger(__name__)
 click_log.basic_config(LOGGER)
 
 MIN_H3, MAX_H3 = 0, 15
 DEFAULT_NAME: str = "value"
 
 DEFAULTS = {
@@ -41,28 +43,40 @@
     "threads": (multiprocessing.cpu_count() - 1),
     "aggfunc": "mean",
     "decimals": 1,
     "warp_mem_limit": 12000,
     "resampling": "average",
 }
 
+DEFAULT_PARENT_OFFSET = 6
+
+
+class ParentResolutionException(Exception):
+    pass
 
-def _get_parent_res(resolution: int) -> int:
+
+def _get_parent_res(parent_res: int, resolution: int) -> int:
     """
+    Uses a parent resolution,
+    OR,
     Given a target resolution, returns our recommended parent resolution.
 
     Used for intermediate re-partioning.
     """
-    return max(MIN_H3, resolution - 8)
+    return (
+        parent_res
+        if parent_res is not None
+        else max(MIN_H3, (resolution - DEFAULT_PARENT_OFFSET))
+    )
 
 
 def _h3func(
     sdf: xr.DataArray,
     resolution: int,
-    parent_resolution: int,
+    parent_res: int,
     nodata: Number = np.nan,
     band_labels: Tuple[str] = None,
 ) -> pa.Table:
     """
     Index a raster window to H3.
     Subsequent steps are necessary to resolve issues at the boundaries of windows.
     If windows are very small, or in strips rather than blocks, processing may be slower
@@ -75,15 +89,15 @@
         subset, values=DEFAULT_NAME, index=["x", "y"], columns=["band"]
     ).reset_index()
     # Primary H3 index
     h3index = subset.h3.geo_to_h3(resolution, lat_col="y", lng_col="x").drop(
         columns=["x", "y"]
     )
     # Secondary (parent) H3 index, used later for partitioning
-    h3index = h3index.h3.h3_to_parent(parent_resolution).reset_index()
+    h3index = h3index.h3.h3_to_parent(parent_res).reset_index()
     # Renaming columns to actual band labels
     bands = sdf["band"].unique()
     band_names = dict(zip(bands, map(lambda i: band_labels[i - 1], bands)))
     for k, v in band_names.items():
         if band_names[k] is None:
             band_names[k] = str(bands[k - 1])
         else:
@@ -92,34 +106,35 @@
     return pa.Table.from_pandas(h3index)
 
 
 def _initial_index(
     raster_input: Union[Path, str],
     output: Path,
     resolution: int,
+    parent_res: int,
     warp_args: dict,
     **kwargs,
 ) -> Path:
     """
     Responsible for opening the raster_input, and performing H3 indexing per window of a WarpedVRT.
 
     A WarpedVRT is used to enforce reprojection to https://epsg.io/4326, which is required for H3 indexing.
 
     It also allows on-the-fly resampling of the input, which is useful if the target H3 resolution exceeds the resolution
         of the input.
 
     This function passes a path to a temporary directory (which contains the output of this "stage 1" processing) to
         a secondary function that addresses issues at the boundaries of raster windows.
     """
-    parent_resolution = _get_parent_res(resolution)
+    parent_res = _get_parent_res(parent_res, resolution)
     LOGGER.info(
         "Indexing %s at H3 resolution %d, parent resolution %d",
         raster_input,
         resolution,
-        parent_resolution,
+        parent_res,
     )
 
     with tempfile.TemporaryDirectory() as tmpdir:
         LOGGER.debug(f"Create temporary directory {tmpdir}")
 
         # https://rasterio.readthedocs.io/en/latest/api/rasterio.warp.html#rasterio.warp.calculate_default_transform
         with rio.Env(CHECK_WITH_INVERT_PROJ=True):
@@ -168,15 +183,15 @@
 
                     def process(window):
                         sdf = da.rio.isel_window(window)
 
                         result = _h3func(
                             sdf,
                             resolution,
-                            parent_resolution,
+                            parent_res,
                             vrt.nodata,
                             band_labels=band_names,
                         )
 
                         with write_lock:
                             pq.write_to_dataset(
                                 result,
@@ -194,58 +209,64 @@
                                 executor.submit(process, window) for window in windows
                             ]
                             for future in as_completed(futures):
                                 result = future.result()
                                 pbar.update(1)
 
             LOGGER.debug("Stage 1 (primary indexing) complete")
-            return _address_boundary_issues(tmpdir, output, resolution, **kwargs)
+            return _address_boundary_issues(
+                tmpdir, output, resolution, parent_res, **kwargs
+            )
 
 
 def _h3_parent_groupby(df, resolution: int, aggfunc: str, decimals: int):
     """
     Function for aggregating the h3 resolution values per parent partition. Each partition will be run through with a
     pandas .groupby function. This step is to ensure there are no duplicate h3 values, which will happen when indexing a
     high resolution raster at a coarser h3 resolution.
     """
     if decimals > 0:
         return df.groupby(f"h3_{resolution:02}").agg(aggfunc).round(decimals)
     else:
         return (
-            df.groupby(f"h3_{resolution:02}").agg(aggfunc).round(decimals).astype('Int64')
+            df.groupby(f"h3_{resolution:02}")
+            .agg(aggfunc)
+            .round(decimals)
+            .astype("Int64")
         )
 
 
 def _address_boundary_issues(
-    pq_input: tempfile.TemporaryDirectory, output: Path, resolution: int, **kwargs
+    pq_input: tempfile.TemporaryDirectory,
+    output: Path,
+    resolution: int,
+    parent_res: int,
+    **kwargs,
 ) -> Path:
     """
     After "stage 1" processing, there is an H3 cell and band value/s for each pixel in the input image. Partitions are based
     on raster windows.
 
     This function will re-partition based on H3 parent cell IDs at a fixed offset from the target resolution.
 
     Once re-partitioned on this basis, values are aggregated at the target resolution, to account for multiple pixels mapping
         to the same H3 cell.
 
     This re-partitioning is necessary to address the issue of the same H3 cell IDs being present in different partitions
         of the original (i.e. window-based) partitioning. Using the nested structure of the DGGS is an useful property
         to address this problem.
     """
-    parent_resolution = _get_parent_res(resolution)
+    parent_res = _get_parent_res(parent_res, resolution)
 
     LOGGER.debug(
         f"Reading Stage 1 output ({pq_input}) and setting index for parent-based partitioning"
     )
     with TqdmCallback(desc="Reading window partitions"):
-        ddf = dd.read_parquet(pq_input).set_index(  # Set index as parent cell
-            f"h3_{parent_resolution:02}"
-            if parent_resolution > 0
-            else "h3_parent"  # https://github.com/DahnJ/H3-Pandas/issues/15
-        )
+        # Set index as parent cell
+        ddf = dd.read_parquet(pq_input).set_index(f"h3_{parent_res:02}")
 
     with TqdmCallback(desc="Counting parents"):
         # Count parents, to get target number of partitions
         uniqueh3 = sorted(list(ddf.index.unique().compute()))
 
     LOGGER.debug(
         "Repartitioning into %d partitions, based on parent cells", len(uniqueh3) + 1
@@ -285,14 +306,21 @@
     "-r",
     "--resolution",
     required=True,
     type=click.Choice(list(map(str, range(MIN_H3, MAX_H3 + 1)))),
     help="H3 resolution to index",
 )
 @click.option(
+    "-pr",
+    "--parent_res",
+    required=False,
+    type=click.Choice(list(map(str, range(MIN_H3, MAX_H3 + 1)))),
+    help="H3 Parent resolution to index and aggregate to. Defaults to resolution - 6",
+)
+@click.option(
     "-u",
     "--upscale",
     default=DEFAULTS["upscale"],
     type=int,
     help="Upscaling factor, used to upsample input data on the fly; useful when the raster resolution is lower than the target DGGS resolution. Default (1) applies no upscaling. The resampling method controls interpolation.",
 )
 @click.option(
@@ -333,18 +361,20 @@
 )
 @click.option(
     "--resampling",
     default=DEFAULTS["resampling"],
     type=click.Choice(Resampling._member_names_),
     help="Input raster may be warped to EPSG:4326 if it is not already in this CRS. Or, if the upscale parameter is greater than 1, there is a need to resample. This setting specifies this resampling algorithm.",
 )
+@click.version_option(version=__version__)
 def h3(
     raster_input: Union[str, Path],
     output_directory: Union[str, Path],
     resolution: str,
+    parent_res: str,
     upscale: int,
     compression: str,
     threads: int,
     aggfunc: str,
     decimals: int,
     overwrite: bool,
     warp_mem_limit: int,
@@ -352,14 +382,20 @@
 ):
     """
     Ingest a raster image and index it to the H3 DGGS.
 
     RASTER_INPUT is the path to input raster data; prepend with protocol like s3:// or hdfs:// for remote data.
     OUTPUT_DIRECTORY should be a directory, not a file, as it will be the write location for an Apache Parquet data store, with partitions equivalent to parent cells of target cells at a fixed offset. However, this can also be remote (use the appropriate prefix, e.g. s3://).
     """
+    if not int(parent_res) < int(resolution):
+        raise ParentResolutionException(
+            "Parent resolution ({pr}) must be less than target resolution ({r})".format(
+                pr=parent_res, r=resolution
+            )
+        )
     if not Path(raster_input).exists():
         if not urlparse(raster_input).scheme:
             LOGGER.warning(
                 f"Input raster {raster_input} does not exist, and is not recognised as a remote URI"
             )
             raise FileNotFoundError(
                 errno.ENOENT, os.strerror(errno.ENOENT), raster_input
@@ -381,8 +417,15 @@
         "threads": threads,
         "aggfunc": aggfunc,
         "decimals": decimals,
         "warp_mem_limit": warp_mem_limit,
         "resampling": resampling,
         "overwrite": overwrite,
     }
-    _initial_index(raster_input, output_directory, int(resolution), warp_args, **kwargs)
+    _initial_index(
+        raster_input,
+        output_directory,
+        int(resolution),
+        int(parent_res),
+        warp_args,
+        **kwargs,
+    )
```

### Comparing `raster2dggs-0.1.2/PKG-INFO` & `raster2dggs-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raster2dggs
-Version: 0.1.2
+Version: 0.2.0
 Summary: 
 Home-page: https://github.com/manaakiwhenua/raster2dggs
 License: LGPL-3.0-or-later
 Keywords: dggs,raster,h3,cli
 Author: James Ardo
 Author-email: ardoj@landcareresearch.co.nz
 Maintainer: Richard Law
@@ -21,15 +21,15 @@
 Requires-Dist: boto3 (>=1.26.85,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-log (>=0.4.0,<0.5.0)
 Requires-Dist: dask (>=2023.3.0,<2024.0.0)
 Requires-Dist: dask-geopandas (>=0.3.0,<0.4.0)
 Requires-Dist: gdal (>=3.6.2,<4.0.0)
 Requires-Dist: geopandas (>=0.12.2,<0.13.0)
-Requires-Dist: h3pandas (>=0.2.3,<0.3.0)
+Requires-Dist: h3pandas (>=0.2.4,<0.3.0)
 Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
 Requires-Dist: rasterio (>=1.3.6,<2.0.0)
 Requires-Dist: rioxarray (>=0.13.4,<0.14.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/manaakiwhenua/raster2dggs
 Description-Content-Type: text/markdown
 
@@ -64,14 +64,17 @@
   s3://).
 
 Options:
   -v, --verbosity LVL             Either CRITICAL, ERROR, WARNING, INFO or
                                   DEBUG  [default: INFO]
   -r, --resolution [0|1|2|3|4|5|6|7|8|9|10|11|12|13|14|15]
                                   H3 resolution to index  [required]
+  -pr,--parent_res [0|1|2|3|4|5|6|7|8|9|10|11|12|13|14|15]
+                                  H3 Parent resolution to index and aggregate
+                                  to. Defaults to resolution - 6
   -u, --upscale INTEGER           Upscaling factor, used to upsample input
                                   data on the fly; useful when the raster
                                   resolution is lower than the target DGGS
                                   resolution. Default (1) applies no
                                   upscaling. The resampling method controls
                                   interpolation.  [default: 1]
   -c, --compression [snappy|gzip|zstd]
@@ -179,18 +182,18 @@
 ## Citation
 
 ```bibtex
 @software{raster2dggs,
   title={{raster2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/raster2dggs},
-  version={0.1.2},
+  version={0.2.0},
   date={2023-02-09}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). raster2dggs (0.1.2) [Computer software]. https://github.com/manaakiwhenua/raster2dggs 
+> Ardo, J., & Law, R. (2023). raster2dggs (0.2.0) [Computer software]. https://github.com/manaakiwhenua/raster2dggs 
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/raster2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

