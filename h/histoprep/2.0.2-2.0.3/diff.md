# Comparing `tmp/histoprep-2.0.2.tar.gz` & `tmp/histoprep-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histoprep-2.0.2.tar", max compression
+gzip compressed data, was "histoprep-2.0.3.tar", max compression
```

## Comparing `histoprep-2.0.2.tar` & `histoprep-2.0.3.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0     1064 2023-04-13 12:39:17.917382 histoprep-2.0.2/LICENSE
--rw-r--r--   0        0        0     4498 2023-04-13 12:39:17.917382 histoprep-2.0.2/README.md
--rw-r--r--   0        0        0      208 2023-04-13 12:39:17.921382 histoprep-2.0.2/histoprep/__init__.py
--rw-r--r--   0        0        0    12824 2023-04-13 12:39:17.921382 histoprep-2.0.2/histoprep/_backend.py
--rw-r--r--   0        0        0    12916 2023-04-13 12:39:17.921382 histoprep-2.0.2/histoprep/_cli.py
--rw-r--r--   0        0        0     2632 2023-04-13 12:39:17.921382 histoprep-2.0.2/histoprep/_data.py
--rw-r--r--   0        0        0    27360 2023-04-13 12:39:17.921382 histoprep-2.0.2/histoprep/_reader.py
--rw-r--r--   0        0        0      907 2023-04-13 12:39:17.921382 histoprep-2.0.2/histoprep/functional/__init__.py
--rw-r--r--   0        0        0     1021 2023-04-13 12:39:17.921382 histoprep-2.0.2/histoprep/functional/_check.py
--rw-r--r--   0        0        0     1297 2023-04-13 12:39:17.921382 histoprep-2.0.2/histoprep/functional/_concurrent.py
--rw-r--r--   0        0        0     5400 2023-04-13 12:39:17.921382 histoprep-2.0.2/histoprep/functional/_dearray.py
--rw-r--r--   0        0        0     4305 2023-04-13 12:39:17.921382 histoprep-2.0.2/histoprep/functional/_draw.py
--rw-r--r--   0        0        0     2641 2023-04-13 12:39:17.925382 histoprep-2.0.2/histoprep/functional/_images.py
--rw-r--r--   0        0        0      410 2023-04-13 12:39:17.925382 histoprep-2.0.2/histoprep/functional/_level.py
--rw-r--r--   0        0        0     1881 2023-04-13 12:39:17.925382 histoprep-2.0.2/histoprep/functional/_mean_std.py
--rw-r--r--   0        0        0     5490 2023-04-13 12:39:17.925382 histoprep-2.0.2/histoprep/functional/_metrics.py
--rw-r--r--   0        0        0     5476 2023-04-13 12:39:17.925382 histoprep-2.0.2/histoprep/functional/_normalize.py
--rw-r--r--   0        0        0     8211 2023-04-13 12:39:17.925382 histoprep-2.0.2/histoprep/functional/_tiles.py
--rw-r--r--   0        0        0     4766 2023-04-13 12:39:17.925382 histoprep-2.0.2/histoprep/functional/_tissue.py
--rw-r--r--   0        0        0      421 2023-04-13 12:39:17.925382 histoprep-2.0.2/histoprep/utils/__init__.py
--rw-r--r--   0        0        0     5870 2023-04-13 12:39:17.925382 histoprep-2.0.2/histoprep/utils/_normalize.py
--rw-r--r--   0        0        0    12291 2023-04-13 12:39:17.925382 histoprep-2.0.2/histoprep/utils/_process.py
--rw-r--r--   0        0        0     5008 2023-04-19 08:36:38.807381 histoprep-2.0.2/histoprep/utils/_torch.py
--rw-r--r--   0        0        0      724 2023-04-19 08:38:19.227324 histoprep-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     5637 1970-01-01 00:00:00.000000 histoprep-2.0.2/setup.py
--rw-r--r--   0        0        0     5310 1970-01-01 00:00:00.000000 histoprep-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-13 12:39:17.917382 histoprep-2.0.3/LICENSE
+-rw-r--r--   0        0        0     4498 2023-04-13 12:39:17.917382 histoprep-2.0.3/README.md
+-rw-r--r--   0        0        0      208 2023-04-13 12:39:17.921382 histoprep-2.0.3/histoprep/__init__.py
+-rw-r--r--   0        0        0    12824 2023-04-13 12:39:17.921382 histoprep-2.0.3/histoprep/_backend.py
+-rw-r--r--   0        0        0    13109 2023-05-03 06:56:36.411842 histoprep-2.0.3/histoprep/_cli.py
+-rw-r--r--   0        0        0     2632 2023-04-13 12:39:17.921382 histoprep-2.0.3/histoprep/_data.py
+-rw-r--r--   0        0        0    27500 2023-05-03 07:09:28.294664 histoprep-2.0.3/histoprep/_reader.py
+-rw-r--r--   0        0        0      907 2023-04-13 12:39:17.921382 histoprep-2.0.3/histoprep/functional/__init__.py
+-rw-r--r--   0        0        0     1021 2023-04-13 12:39:17.921382 histoprep-2.0.3/histoprep/functional/_check.py
+-rw-r--r--   0        0        0     1297 2023-04-13 12:39:17.921382 histoprep-2.0.3/histoprep/functional/_concurrent.py
+-rw-r--r--   0        0        0     5400 2023-04-13 12:39:17.921382 histoprep-2.0.3/histoprep/functional/_dearray.py
+-rw-r--r--   0        0        0     4305 2023-04-13 12:39:17.921382 histoprep-2.0.3/histoprep/functional/_draw.py
+-rw-r--r--   0        0        0     2641 2023-04-13 12:39:17.925382 histoprep-2.0.3/histoprep/functional/_images.py
+-rw-r--r--   0        0        0      410 2023-04-13 12:39:17.925382 histoprep-2.0.3/histoprep/functional/_level.py
+-rw-r--r--   0        0        0     1881 2023-04-13 12:39:17.925382 histoprep-2.0.3/histoprep/functional/_mean_std.py
+-rw-r--r--   0        0        0     5490 2023-04-13 12:39:17.925382 histoprep-2.0.3/histoprep/functional/_metrics.py
+-rw-r--r--   0        0        0     5476 2023-04-13 12:39:17.925382 histoprep-2.0.3/histoprep/functional/_normalize.py
+-rw-r--r--   0        0        0     8211 2023-04-13 12:39:17.925382 histoprep-2.0.3/histoprep/functional/_tiles.py
+-rw-r--r--   0        0        0     4766 2023-04-13 12:39:17.925382 histoprep-2.0.3/histoprep/functional/_tissue.py
+-rw-r--r--   0        0        0      421 2023-04-13 12:39:17.925382 histoprep-2.0.3/histoprep/utils/__init__.py
+-rw-r--r--   0        0        0     5870 2023-04-13 12:39:17.925382 histoprep-2.0.3/histoprep/utils/_normalize.py
+-rw-r--r--   0        0        0    12291 2023-04-13 12:39:17.925382 histoprep-2.0.3/histoprep/utils/_process.py
+-rw-r--r--   0        0        0     5436 2023-05-03 07:09:58.615718 histoprep-2.0.3/histoprep/utils/_torch.py
+-rw-r--r--   0        0        0      724 2023-04-20 09:43:03.036936 histoprep-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5310 1970-01-01 00:00:00.000000 histoprep-2.0.3/PKG-INFO
```

### Comparing `histoprep-2.0.2/LICENSE` & `histoprep-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.2/README.md` & `histoprep-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.2/histoprep/_backend.py` & `histoprep-2.0.3/histoprep/_backend.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.2/histoprep/_cli.py` & `histoprep-2.0.3/histoprep/_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,69 +9,92 @@
 from typing import NoReturn, Optional, Union
 
 import mpire
 import rich_click as click
 
 from histoprep import SlideReader
 
-LOGO = """
-██╗  ██╗██╗███████╗████████╗ ██████╗ ██████╗ ██████╗ ███████╗██████╗
-██║  ██║██║██╔════╝╚══██╔══╝██╔═══██╗██╔══██╗██╔══██╗██╔════╝██╔══██╗
-███████║██║███████╗   ██║   ██║   ██║██████╔╝██████╔╝█████╗  ██████╔╝
-██╔══██║██║╚════██║   ██║   ██║   ██║██╔═══╝ ██╔══██╗██╔══╝  ██╔═══╝
-██║  ██║██║███████║   ██║   ╚██████╔╝██║     ██║  ██║███████╗██║
-╚═╝  ╚═╝╚═╝╚══════╝   ╚═╝    ╚═════╝ ╚═╝     ╚═╝  ╚═╝╚══════╝╚═╝
-                        by jopo666 (2023)
-"""
+# LOGO = """
+# ██╗  ██╗██╗███████╗████████╗ ██████╗ ██████╗ ██████╗ ███████╗██████╗
+# ██║  ██║██║██╔════╝╚══██╔══╝██╔═══██╗██╔══██╗██╔══██╗██╔════╝██╔══██╗
+# ███████║██║███████╗   ██║   ██║   ██║██████╔╝██████╔╝█████╗  ██████╔╝
+# ██╔══██║██║╚════██║   ██║   ██║   ██║██╔═══╝ ██╔══██╗██╔══╝  ██╔═══╝
+# ██║  ██║██║███████║   ██║   ╚██████╔╝██║     ██║  ██║███████╗██║
+# ╚═╝  ╚═╝╚═╝╚══════╝   ╚═╝    ╚═════╝ ╚═╝     ╚═╝  ╚═╝╚══════╝╚═╝
+#                         by jopo666 (2023)
+# """
 # Rich-click options.
 click.rich_click.USE_RICH_MARKUP = True
 click.rich_click.RANGE_STRING = ""
-click.rich_click.HEADER_TEXT = LOGO
+# click.rich_click.HEADER_TEXT = LOGO
 click.rich_click.STYLE_HEADER_TEXT = "dim"
-click.rich_click.MAX_WIDTH = 120
+click.rich_click.MAX_WIDTH = 100
 click.rich_click.SHOW_METAVARS_COLUMN = False
 click.rich_click.APPEND_METAVARS_HELP = True
 click.rich_click.GROUP_ARGUMENTS_OPTIONS = True
 click.rich_click.USE_CLICK_SHORT_HELP = False
 IO_OPTIONS = ["--input", "--output", "--backend"]
 TILE_OPTIONS = [
     "--level",
     "--width",
     "--height",
     "--overlap",
     "--max-background",
-    "--out-of-bounds",
+    "--in-bounds",
 ]
 SAVE_OPTIONS = [
-    "--save-metrics",
-    "--save-masks",
-    "--save-thumbnails",
+    "--metrics",
+    "--masks",
     "--overwrite",
     "--unfinished",
-    "--format",
+    "--image-format",
     "--quality",
-    "--use-csv",
     "--num-workers",
 ]
 TISSUE_OPTIONS = [
     "--threshold",
     "--multiplier",
     "--tissue-level",
     "--max-dimension",
     "--sigma",
 ]
 click.rich_click.OPTION_GROUPS = {
     "HistoPrep": [
         {"name": "Input/output", "options": IO_OPTIONS},
         {"name": "Tile extraction", "options": TILE_OPTIONS},
-        {"name": "Tile saving", "options": SAVE_OPTIONS},
         {"name": "Tissue detection", "options": TISSUE_OPTIONS},
+        {"name": "Tile saving", "options": SAVE_OPTIONS},
     ]
 }
 
+DEFAULT_OPTIONS = {
+    # Input/output
+    "backend": None,
+    # Tile extraction.
+    "level": 0,
+    "width": 640,
+    "height": None,
+    "overlap": 0.0,
+    "max_background": 0.75,
+    "in_bounds": False,
+    # Tissue detection.
+    "threshold": None,
+    "multiplier": 1.05,
+    "tissue_level": None,
+    "max_dimension": 8192,
+    "sigma": 1.0,
+    "save_metrics": False,
+    "save_masks": False,
+    "overwrite": False,
+    "overwrite_unfinished": False,
+    "image_format": "jpeg",
+    "quality": 80,
+    "num_workers": None,
+}
+
 
 def glob_pattern(*args) -> list[Path]:
     pattern = args[-1]
     output = [
         z for z in (Path(x) for x in glob.glob(pattern, recursive=True)) if z.is_file()
     ]
     if len(output) == 0:
@@ -99,188 +122,169 @@
     metavar="DIRECTORY",
     required=True,
     callback=lambda *args: Path(args[-1]),
     type=click.Path(file_okay=False),
     help="Parent directory for all outputs.",
 )
 @click.option(  # backend
-    "-b",
     "--backend",
     type=click.Choice(choices=["PIL", "OPENSLIDE", "CZI"], case_sensitive=False),
-    default=None,
+    default=DEFAULT_OPTIONS["backend"],
     show_default="automatic",
     help="Backend for reading slides.",
 )
 # Tiles.
 @click.option(  # level
     "-l",
     "--level",
     metavar="INT",
     type=click.IntRange(min=0),
-    default=0,
+    default=DEFAULT_OPTIONS["level"],
     show_default=True,
-    help="Slide pyramid level for tile extraction.",
+    help="Pyramid level for tile extraction.",
 )
 @click.option(  # width
     "-w",
     "--width",
     metavar="INT",
     type=click.IntRange(min=0, min_open=False),
-    default=640,
+    default=DEFAULT_OPTIONS["width"],
     show_default=True,
     help="Tile width.",
 )
 @click.option(  # height
+    "-h",
     "--height",
     metavar="INT",
     type=click.IntRange(min=0, min_open=False),
-    default=None,
+    default=DEFAULT_OPTIONS["height"],
     show_default="width",
     help="Tile height.",
 )
 @click.option(  # overlap
     "-n",
     "--overlap",
     metavar="FLOAT",
     type=click.FloatRange(min=0, max=1, min_open=False, max_open=False),
-    default=0.0,
+    default=DEFAULT_OPTIONS["overlap"],
     show_default=True,
     help="Overlap between neighbouring tiles.",
 )
 @click.option(  # background
-    "-m",
+    "-b",
     "--max-background",
     metavar="FLOAT",
     type=click.FloatRange(min=0, max=1, min_open=True, max_open=True),
-    default=0.75,
+    default=DEFAULT_OPTIONS["max_background"],
     show_default=True,
-    help="Maximum background in tile.",
+    help="Maximum background for tiles.",
 )
 @click.option(  # out-of-bounds
-    "--out-of-bounds",
-    type=click.BOOL,
-    default=True,
-    show_default=True,
-    help="Allow tiles to go out-of-bounds. ",
+    "--in-bounds",
+    show_default="False",
+    is_flag=True,
+    help="Do not allow tiles to go out-of-bounds. ",
 )
-# Saving.
-@click.option(  # save_metrics
-    "--save-metrics",
-    type=click.BOOL,
-    default=True,
+# Tissue.
+@click.option(  # threshold
+    "-t",
+    "--threshold",
+    metavar="INT",
+    type=click.IntRange(min=0, max=255, min_open=False),
+    default=DEFAULT_OPTIONS["threshold"],
+    show_default="Otsu",
+    help="Global thresholding value.",
+)
+@click.option(  # multiplier
+    "-x",
+    "--multiplier",
+    metavar="FLOAT",
+    type=click.FloatRange(min=0, min_open=False),
+    default=DEFAULT_OPTIONS["multiplier"],
     show_default=True,
-    help="Save image metrics to metadata.",
+    help="Multiplier for Otsu's threshold.",
 )
-@click.option(  # save_masks
-    "--save-masks",
-    type=click.BOOL,
-    default=False,
+@click.option(  # tissue_level
+    "--tissue-level",
+    metavar="INT",
+    type=click.IntRange(min=0),
+    default=DEFAULT_OPTIONS["tissue_level"],
+    show_default="max_dimension",
+    help="Pyramid level for tissue detection.",
+)
+@click.option(  # max_dimension
+    "--max-dimension",
+    metavar="INT",
+    type=click.IntRange(min=0),
+    default=DEFAULT_OPTIONS["max_dimension"],
     show_default=True,
-    help="Save tissue masks for each tile.",
+    help="Maximum dimension for tissue detection.",
 )
-@click.option(  # save_thumbnails
-    "--save-thumbnails",
-    type=click.BOOL,
-    default=True,
+@click.option(  # sigma
+    "--sigma",
+    metavar="FLOAT",
+    type=click.FloatRange(min=0),
+    default=DEFAULT_OPTIONS["sigma"],
     show_default=True,
-    help="Save thumbnail images.",
+    help="Sigma for gaussian blurring.",
+)
+# Saving.
+@click.option(  # save_metrics
+    "--metrics",
+    "save_metrics",
+    show_default="False",
+    is_flag=True,
+    help="Save image metrics.",
+)
+@click.option(  # save_masks
+    "--masks",
+    "save_masks",
+    show_default="False",
+    is_flag=True,
+    help="Save tissue masks.",
 )
 @click.option(  # overwrite
     "-z",
     "--overwrite",
-    type=click.BOOL,
-    default=False,
-    show_default=True,
+    show_default="False",
+    is_flag=True,
     help="Overwrite any existing slide outputs.",
 )
 @click.option(  # overwrite_unfinished
     "-u",
     "--unfinished",
     "overwrite_unfinished",
-    type=click.BOOL,
-    default=False,
-    show_default=True,
+    show_default="False",
+    is_flag=True,
     help="Overwrite only if metadata is missing.",
 )
 @click.option(  # format
-    "--format",
-    "image_format",
+    "--image-format",
     type=click.STRING,
-    default="jpeg",
+    default=DEFAULT_OPTIONS["image_format"],
     show_default=True,
-    help="File format for tiles.",
+    help="File format for tile images.",
 )
 @click.option(  # quality
     "--quality",
     metavar="INT",
     type=click.IntRange(min=0, max=100),
-    default=80,
+    default=DEFAULT_OPTIONS["quality"],
     show_default=True,
     help="Quality for jpeg-compression.",
 )
-@click.option(  # overwrite_unfinished
-    "-c",
-    "--use-csv",
-    type=click.BOOL,
-    default=False,
-    show_default=True,
-    help="Write metadata to csv-files instead of parquet files.",
-)
 @click.option(  # num_workers
     "-j",
     "--num-workers",
     metavar="INT",
     type=click.IntRange(min=0, min_open=False),
-    default=None,
+    default=DEFAULT_OPTIONS["num_workers"],
     show_default="CPU-count",
     help="Number of data saving workers.",
 )
-# Tissue.
-@click.option(  # threshold
-    "-t",
-    "--threshold",
-    metavar="INT",
-    type=click.IntRange(min=0, max=255, min_open=False),
-    default=None,
-    show_default="Otsu's threshold",
-    help="Global threshold value for tissue detection.",
-)
-@click.option(  # multiplier
-    "-x",
-    "--multiplier",
-    metavar="FLOAT",
-    type=click.FloatRange(min=0, min_open=False),
-    default=1.05,
-    show_default=True,
-    help="Multiplier for Otsu's threshold. Ignored if threshold is set.",
-)
-@click.option(  # tissue_level
-    "--tissue-level",
-    metavar="INT",
-    type=click.IntRange(min=0),
-    default=None,
-    show_default="max_dimension",
-    help="Slide pyramid level for tissue detection.",
-)
-@click.option(  # max_dimension
-    "--max-dimension",
-    metavar="INT",
-    type=click.IntRange(min=0),
-    default=8192,
-    show_default=True,
-    help="Select first pyramid level with both dimensions smaller than this value.",
-)
-@click.option(  # sigma
-    "--sigma",
-    metavar="FLOAT",
-    type=click.FloatRange(min=0),
-    default=1.0,
-    show_default=True,
-    help="Sigma for gaussian blurring during tissue detection.",
-)
 def cut_slides(
     paths: list[Union[str, Path]],
     parent_dir: Union[str, Path],
     *,
     backend: Optional[str] = None,
     # Tissue detection.
     threshold: Optional[float] = None,
@@ -290,28 +294,26 @@
     sigma: float = 1.0,
     # Tile extraction.
     level: int = 0,
     width: int = 640,
     height: Optional[int] = None,
     overlap: float = 0.0,
     max_background: float = 0.75,
-    out_of_bounds: bool = True,
+    in_bounds: bool = False,
     # Tile saving.
-    save_metrics: bool = True,
-    save_masks: bool = True,
-    save_thumbnails: bool = True,
+    save_metrics: bool = False,
+    save_masks: bool = False,
     overwrite: bool = False,
     overwrite_unfinished: bool = False,
     image_format: str = "jpeg",
     quality: int = 80,
     use_csv: bool = False,
     num_workers: Optional[int] = None,
 ) -> None:
-    """CLI interface to extract tile images from slides."""
-    # Filter slide paths.
+    """Extract tile images from histological slides."""
     paths = filter_slide_paths(
         all_paths=[x if isinstance(x, Path) else Path(x) for x in paths],
         parent_dir=parent_dir,
         overwrite=overwrite,
         overwrite_unfinished=overwrite_unfinished,
     )
     # Define cut_slide kwargs.
@@ -324,23 +326,23 @@
             "multiplier": multiplier,
             "sigma": sigma,
         },
         "tile_kwargs": {
             "width": width,
             "height": height,
             "overlap": overlap,
-            "out_of_bounds": out_of_bounds,
+            "out_of_bounds": not in_bounds,
             "max_background": max_background,
         },
         "save_kwargs": {
             "parent_dir": parent_dir,
             "level": level,
             "save_metrics": save_metrics,
             "save_masks": save_masks,
-            "save_thumbnails": save_thumbnails,
+            "save_thumbnails": True,
             "image_format": image_format,
             "quality": quality,
             "use_csv": use_csv,
             "raise_exception": False,  # handled here.
             "num_workers": 0,  # slide-per-process.
             "overwrite": True,  # filtered earlier.
             "verbose": False,  # common progressbar.
```

### Comparing `histoprep-2.0.2/histoprep/_data.py` & `histoprep-2.0.3/histoprep/_data.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.2/histoprep/_reader.py` & `histoprep-2.0.3/histoprep/_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,19 @@
 
     @property
     def suffix(self) -> str:
         """Slide file-extension."""
         return self._backend.suffix
 
     @property
+    def backend_name(self) -> str:
+        """Name of the slide reader backend."""
+        return self._backend.BACKEND_NAME
+
+    @property
     def data_bounds(self) -> tuple[int, int, int, int]:
         """Data bounds defined by `xywh`-coordinates at `level=0`.
 
         Some image formats (eg. `.mrxs`) define a bounding box where image data resides,
         which may differ from the actual image dimensions. `HistoPrep` always uses the
         full image dimensions, but other software (such as `QuPath`) uses the image
         dimensions defined by this data bound.
```

### Comparing `histoprep-2.0.2/histoprep/functional/__init__.py` & `histoprep-2.0.3/histoprep/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.2/histoprep/functional/_check.py` & `histoprep-2.0.3/histoprep/functional/_check.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.2/histoprep/functional/_concurrent.py` & `histoprep-2.0.3/histoprep/functional/_concurrent.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.2/histoprep/functional/_dearray.py` & `histoprep-2.0.3/histoprep/functional/_dearray.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.2/histoprep/functional/_draw.py` & `histoprep-2.0.3/histoprep/functional/_draw.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.2/histoprep/functional/_images.py` & `histoprep-2.0.3/histoprep/functional/_images.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.2/histoprep/functional/_mean_std.py` & `histoprep-2.0.3/histoprep/functional/_mean_std.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.2/histoprep/functional/_metrics.py` & `histoprep-2.0.3/histoprep/functional/_metrics.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.2/histoprep/functional/_normalize.py` & `histoprep-2.0.3/histoprep/functional/_normalize.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.2/histoprep/functional/_tiles.py` & `histoprep-2.0.3/histoprep/functional/_tiles.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.2/histoprep/functional/_tissue.py` & `histoprep-2.0.3/histoprep/functional/_tissue.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.2/histoprep/utils/_normalize.py` & `histoprep-2.0.3/histoprep/utils/_normalize.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.2/histoprep/utils/_process.py` & `histoprep-2.0.3/histoprep/utils/_process.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.2/histoprep/utils/_torch.py` & `histoprep-2.0.3/histoprep/utils/_torch.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from collections.abc import Callable, Iterator
 from pathlib import Path
 from typing import Any, Optional, Union
 
 import numpy as np
 from PIL import Image
 
+from histoprep._backend import CziBackend
 from histoprep._reader import SlideReader
 
 try:
     from torch.utils.data import Dataset
 
     HAS_PYTORCH = True
 except ImportError:
@@ -52,19 +53,27 @@
         if not HAS_PYTORCH:
             raise ImportError(ERROR_PYTORCH)
         super().__init__()
         self.reader = reader
         self.coordinates = coordinates
         self.level = level
         self.transform = transform
+        self.__first_sample = True
 
     def __len__(self) -> int:
         return len(self.coordinates)
 
     def __getitem__(self, index: int) -> tuple[Union[np.ndarray, Any], np.ndarray]:
+        if self.__first_sample and isinstance(self.reader._backend, CziBackend):
+            # We have to initialize a new CziFile instance as it does not like
+            # concurrent reads....
+            self.reader = SlideReader(
+                self.reader.path, backend=self.reader.backend_name
+            )
+        self.__first_sample = False
         xywh = self.coordinates[index]
         tile = self.reader.read_region(xywh, level=self.level)
         if self.transform is not None:
             tile = self.transform(tile)
         return tile, np.array(xywh)
```

### Comparing `histoprep-2.0.2/pyproject.toml` & `histoprep-2.0.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "histoprep"
-version = "2.0.2"
+version = "2.0.3"
 description = "Read and process histological slide images with python!"
 authors = ["jopo666 <jopo@birdlover.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 HistoPrep = 'histoprep._cli:cut_slides'
```

### Comparing `histoprep-2.0.2/setup.py` & `histoprep-2.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,155 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['histoprep', 'histoprep.functional', 'histoprep.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aicspylibczi>=3,<4',
- 'matplotlib',
- 'mpire>=2.6,<3.0',
- 'numpy',
- 'opencv-python-headless>=4,<5',
- 'openslide-python>=1.2,<2.0',
- 'pillow>=9,<10',
- 'polars>=0.16,<0.17',
- 'rich-click>=1.6,<2.0',
- 'scikit-learn>=1,<2',
- 'tqdm']
-
-entry_points = \
-{'console_scripts': ['HistoPrep = histoprep._cli:cut_slides']}
-
-setup_kwargs = {
-    'name': 'histoprep',
-    'version': '2.0.2',
-    'description': 'Read and process histological slide images with python!',
-    'long_description': '<div align="center">\n\n# HistoPrep\nPreprocessing large medical images for machine learning made easy!\n\n<p align="center">\n  <a href="#description">Description</a> •\n  <a href="#installation">Installation</a> •\n  <a href="#usage">Usage</a> •\n  <a href="https://jopo666.github.io/HistoPrep/">API Documentation</a> •\n  <a href="#citation">Citation</a>\n</p>\n\n</div>\n\n## Description\n\n`HistoPrep` makes is easy to prepare your histological slide images for deep\nlearning models. You can easily cut large slide images into smaller tiles and then\npreprocess those tiles (remove tiles with shitty tissue, finger  marks etc).\n\n## Installation \n\nInstall [`OpenSlide`](https://openslide.org/download/) on your system and then install histoprep with `pip`!\n\n```bash\npip install histoprep\n```\n\n## Usage\n\nTypical workflow for training deep learning models with histological images is the\nfollowing:\n\n1. Cut each slide image into smaller tile images.\n2. Preprocess smaller tile images by removing tiles with bad tissue, staining artifacts.\n3. Overfit a pretrained ResNet50 model, report 100% validation accuracy and publish it\n   in [Nature](https://www.nature.com) like everyone else. \n\nWith `HistoPrep`, steps 1. and 2. are as easy as accidentally drinking too much at the\nresearch group christmas party and proceeding to work remotely until June.\n\nLet\'s start by cutting a slide from the\n[PANDA](https://www.kaggle.com/c/prostate-cancer-grade-assessment) kaggle challenge into\nsmall tiles. \n\n```python\nfrom histoprep import SlideReader\n\n# Read slide image.\nreader = SlideReader("./slides/slide_with_ink.jpeg")\n# Detect tissue.\nthreshold, tissue_mask = reader.get_tissue_mask(level=-1)\n# Extract overlapping tile coordinates with less than 50% background.\ntile_coordinates = reader.get_tile_coordinates(\n    tissue_mask, width=512, overlap=0.5, max_background=0.5\n)\n# Save tile images with image metrics for preprocessing.\ntile_metadata = reader.save_regions(\n    "./train_tiles/", tile_coordinates, threshold=threshold, save_metrics=True\n)\n```\n```\nslide_with_ink: 100%|██████████| 390/390 [00:01<00:00, 295.90it/s]\n```\n\nLet\'s take a look at the output and visualise the thumbnails.\n\n```bash\njopo666@~$ tree train_tiles\ntrain_tiles\n└── slide_with_ink\n    ├── metadata.parquet       # tile metadata\n    ├── properties.json        # tile properties\n    ├── thumbnail.jpeg         # thumbnail image\n    ├── thumbnail_tiles.jpeg   # thumbnail with tiles\n    ├── thumbnail_tissue.jpeg  # thumbnail of the tissue mask\n    └── tiles [390 entries exceeds filelimit, not opening dir]\n```\n\n![Prostate biopsy sample](images/thumbnail.jpeg)\n![Tissue mask](images/thumbnail_tissue.jpeg)\n![Thumbnail with tiles](images/thumbnail_tiles.jpeg)\n\nThat was easy, but it can be annoying to whip up a new python script every time you want\nto cut slides, and thus it is recommended to use the `HistoPrep` CLI program!\n\n```bash\n# Repeat the above code for all images in the PANDA dataset!\njopo666@~$ HistoPrep --input \'./train_images/*.tiff\' --output ./tiles --width 512 --overlap 0.5 --max-background 0.5\n```\n\nAs we can see from the above images, histological slide images often contain areas that\nwe would not like to include into our training data. Might seem like a daunting task but\nlet\'s try it out!\n\n\n```python\nfrom histoprep.utils import OutlierDetector\n\n# Let\'s wrap the tile metadata with a helper class.\ndetector = OutlierDetector(tile_metadata)\n# Cluster tiles based on image metrics.\nclusters = detector.cluster_kmeans(num_clusters=4, random_state=666)\n# Visualise first cluster.\nreader.get_annotated_thumbnail(\n    image=reader.read_level(-1), coordinates=detector.coordinates[clusters == 0]\n)\n```\n![Tiles in cluster 0](images/thumbnail_blue.jpeg)\n\nI said it was gonna be easy! Now we can mark tiles in cluster `0` as outliers and\nstart overfitting our neural network! This was a simple example but the same code can be\nused to cluster all several _million_ tiles extracted from the `PANDA` dataset and discard\noutliers simultaneously!\n\n## Citation\n\nIf you use `HistoPrep` to process the images for your publication, please cite the github repository.\n\n```\n@misc{histoprep,\n  author = {Pohjonen, Joona and Ariotta, Valeria},\n  title = {HistoPrep: Preprocessing large medical images for machine learning made easy!},\n  year = {2022},\n  publisher = {GitHub},\n  journal = {GitHub repository},\n  howpublished = {https://github.com/jopo666/HistoPrep},\n}\n```\n',
-    'author': 'jopo666',
-    'author_email': 'jopo@birdlover.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
+Metadata-Version: 2.1
+Name: histoprep
+Version: 2.0.3
+Summary: Read and process histological slide images with python!
+Author: jopo666
+Author-email: jopo@birdlover.com
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aicspylibczi (>=3,<4)
+Requires-Dist: matplotlib
+Requires-Dist: mpire (>=2.6,<3.0)
+Requires-Dist: numpy
+Requires-Dist: opencv-python-headless (>=4,<5)
+Requires-Dist: openslide-python (>=1.2,<2.0)
+Requires-Dist: pillow (>=9,<10)
+Requires-Dist: polars (>=0.16,<0.17)
+Requires-Dist: rich-click (>=1.6,<2.0)
+Requires-Dist: scikit-learn (>=1,<2)
+Requires-Dist: tqdm
+Description-Content-Type: text/markdown
+
+<div align="center">
+
+# HistoPrep
+Preprocessing large medical images for machine learning made easy!
+
+<p align="center">
+  <a href="#description">Description</a> •
+  <a href="#installation">Installation</a> •
+  <a href="#usage">Usage</a> •
+  <a href="https://jopo666.github.io/HistoPrep/">API Documentation</a> •
+  <a href="#citation">Citation</a>
+</p>
+
+</div>
+
+## Description
+
+`HistoPrep` makes is easy to prepare your histological slide images for deep
+learning models. You can easily cut large slide images into smaller tiles and then
+preprocess those tiles (remove tiles with shitty tissue, finger  marks etc).
+
+## Installation 
+
+Install [`OpenSlide`](https://openslide.org/download/) on your system and then install histoprep with `pip`!
+
+```bash
+pip install histoprep
+```
+
+## Usage
+
+Typical workflow for training deep learning models with histological images is the
+following:
+
+1. Cut each slide image into smaller tile images.
+2. Preprocess smaller tile images by removing tiles with bad tissue, staining artifacts.
+3. Overfit a pretrained ResNet50 model, report 100% validation accuracy and publish it
+   in [Nature](https://www.nature.com) like everyone else. 
+
+With `HistoPrep`, steps 1. and 2. are as easy as accidentally drinking too much at the
+research group christmas party and proceeding to work remotely until June.
+
+Let's start by cutting a slide from the
+[PANDA](https://www.kaggle.com/c/prostate-cancer-grade-assessment) kaggle challenge into
+small tiles. 
+
+```python
+from histoprep import SlideReader
+
+# Read slide image.
+reader = SlideReader("./slides/slide_with_ink.jpeg")
+# Detect tissue.
+threshold, tissue_mask = reader.get_tissue_mask(level=-1)
+# Extract overlapping tile coordinates with less than 50% background.
+tile_coordinates = reader.get_tile_coordinates(
+    tissue_mask, width=512, overlap=0.5, max_background=0.5
+)
+# Save tile images with image metrics for preprocessing.
+tile_metadata = reader.save_regions(
+    "./train_tiles/", tile_coordinates, threshold=threshold, save_metrics=True
+)
+```
+```
+slide_with_ink: 100%|██████████| 390/390 [00:01<00:00, 295.90it/s]
+```
+
+Let's take a look at the output and visualise the thumbnails.
+
+```bash
+jopo666@~$ tree train_tiles
+train_tiles
+└── slide_with_ink
+    ├── metadata.parquet       # tile metadata
+    ├── properties.json        # tile properties
+    ├── thumbnail.jpeg         # thumbnail image
+    ├── thumbnail_tiles.jpeg   # thumbnail with tiles
+    ├── thumbnail_tissue.jpeg  # thumbnail of the tissue mask
+    └── tiles [390 entries exceeds filelimit, not opening dir]
+```
+
+![Prostate biopsy sample](images/thumbnail.jpeg)
+![Tissue mask](images/thumbnail_tissue.jpeg)
+![Thumbnail with tiles](images/thumbnail_tiles.jpeg)
+
+That was easy, but it can be annoying to whip up a new python script every time you want
+to cut slides, and thus it is recommended to use the `HistoPrep` CLI program!
+
+```bash
+# Repeat the above code for all images in the PANDA dataset!
+jopo666@~$ HistoPrep --input './train_images/*.tiff' --output ./tiles --width 512 --overlap 0.5 --max-background 0.5
+```
+
+As we can see from the above images, histological slide images often contain areas that
+we would not like to include into our training data. Might seem like a daunting task but
+let's try it out!
+
+
+```python
+from histoprep.utils import OutlierDetector
+
+# Let's wrap the tile metadata with a helper class.
+detector = OutlierDetector(tile_metadata)
+# Cluster tiles based on image metrics.
+clusters = detector.cluster_kmeans(num_clusters=4, random_state=666)
+# Visualise first cluster.
+reader.get_annotated_thumbnail(
+    image=reader.read_level(-1), coordinates=detector.coordinates[clusters == 0]
+)
+```
+![Tiles in cluster 0](images/thumbnail_blue.jpeg)
+
+I said it was gonna be easy! Now we can mark tiles in cluster `0` as outliers and
+start overfitting our neural network! This was a simple example but the same code can be
+used to cluster all several _million_ tiles extracted from the `PANDA` dataset and discard
+outliers simultaneously!
+
+## Citation
+
+If you use `HistoPrep` to process the images for your publication, please cite the github repository.
+
+```
+@misc{histoprep,
+  author = {Pohjonen, Joona and Ariotta, Valeria},
+  title = {HistoPrep: Preprocessing large medical images for machine learning made easy!},
+  year = {2022},
+  publisher = {GitHub},
+  journal = {GitHub repository},
+  howpublished = {https://github.com/jopo666/HistoPrep},
 }
+```
 
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,76 +1,67 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['histoprep',
-'histoprep.functional', 'histoprep.utils'] package_data = \ {'': ['*']}
-install_requires = \ ['aicspylibczi>=3,<4', 'matplotlib', 'mpire>=2.6,<3.0',
-'numpy', 'opencv-python-headless>=4,<5', 'openslide-python>=1.2,<2.0',
-'pillow>=9,<10', 'polars>=0.16,<0.17', 'rich-click>=1.6,<2.0', 'scikit-
-learn>=1,<2', 'tqdm'] entry_points = \ {'console_scripts': ['HistoPrep =
-histoprep._cli:cut_slides']} setup_kwargs = { 'name': 'histoprep', 'version':
-'2.0.2', 'description': 'Read and process histological slide images with
-python!', 'long_description': '
- \n\n# HistoPrep\nPreprocessing large medical images for machine learning made
-                                   easy!\n\n
-  \n Description â¢\n Installation â¢\n Usage â¢\n API_Documentation â¢\n
-                                  Citation\n
-                                     \n\n
-\n\n## Description\n\n`HistoPrep` makes is easy to prepare your histological
-slide images for deep\nlearning models. You can easily cut large slide images
-into smaller tiles and then\npreprocess those tiles (remove tiles with shitty
-tissue, finger marks etc).\n\n## Installation \n\nInstall [`OpenSlide`](https:/
-/openslide.org/download/) on your system and then install histoprep with
-`pip`!\n\n```bash\npip install histoprep\n```\n\n## Usage\n\nTypical workflow
-for training deep learning models with histological images is the\nfollowing:
-\n\n1. Cut each slide image into smaller tile images.\n2. Preprocess smaller
-tile images by removing tiles with bad tissue, staining artifacts.\n3. Overfit
-a pretrained ResNet50 model, report 100% validation accuracy and publish it\n
-in [Nature](https://www.nature.com) like everyone else. \n\nWith `HistoPrep`,
-steps 1. and 2. are as easy as accidentally drinking too much at the\nresearch
-group christmas party and proceeding to work remotely until June.\n\nLet\'s
-start by cutting a slide from the\n[PANDA](https://www.kaggle.com/c/prostate-
-cancer-grade-assessment) kaggle challenge into\nsmall tiles.
-\n\n```python\nfrom histoprep import SlideReader\n\n# Read slide image.\nreader
-= SlideReader("./slides/slide_with_ink.jpeg")\n# Detect tissue.\nthreshold,
-tissue_mask = reader.get_tissue_mask(level=-1)\n# Extract overlapping tile
-coordinates with less than 50% background.\ntile_coordinates =
-reader.get_tile_coordinates(\n tissue_mask, width=512, overlap=0.5,
-max_background=0.5\n)\n# Save tile images with image metrics for
-preprocessing.\ntile_metadata = reader.save_regions(\n "./train_tiles/",
-tile_coordinates, threshold=threshold,
-save_metrics=True\n)\n```\n```\nslide_with_ink:
-100%|ââââââââââ| 390/390 [00:01<00:00, 295.90it/
-s]\n```\n\nLet\'s take a look at the output and visualise the
-thumbnails.\n\n```bash\njopo666@~$ tree train_tiles\ntrain_tiles\nâââ
-slide_with_ink\n âââ metadata.parquet # tile metadata\n âââ
-properties.json # tile properties\n âââ thumbnail.jpeg # thumbnail
-image\n âââ thumbnail_tiles.jpeg # thumbnail with tiles\n âââ
-thumbnail_tissue.jpeg # thumbnail of the tissue mask\n âââ tiles [390
-entries exceeds filelimit, not opening dir]\n```\n\n![Prostate biopsy sample]
-(images/thumbnail.jpeg)\n![Tissue mask](images/thumbnail_tissue.jpeg)\n!
-[Thumbnail with tiles](images/thumbnail_tiles.jpeg)\n\nThat was easy, but it
-can be annoying to whip up a new python script every time you want\nto cut
-slides, and thus it is recommended to use the `HistoPrep` CLI
-program!\n\n```bash\n# Repeat the above code for all images in the PANDA
-dataset!\njopo666@~$ HistoPrep --input \'./train_images/*.tiff\' --output ./
-tiles --width 512 --overlap 0.5 --max-background 0.5\n```\n\nAs we can see from
-the above images, histological slide images often contain areas that\nwe would
-not like to include into our training data. Might seem like a daunting task
-but\nlet\'s try it out!\n\n\n```python\nfrom histoprep.utils import
-OutlierDetector\n\n# Let\'s wrap the tile metadata with a helper
-class.\ndetector = OutlierDetector(tile_metadata)\n# Cluster tiles based on
-image metrics.\nclusters = detector.cluster_kmeans(num_clusters=4,
-random_state=666)\n# Visualise first cluster.\nreader.get_annotated_thumbnail
-(\n image=reader.read_level(-1), coordinates=detector.coordinates[clusters ==
-0]\n)\n```\n![Tiles in cluster 0](images/thumbnail_blue.jpeg)\n\nI said it was
-gonna be easy! Now we can mark tiles in cluster `0` as outliers and\nstart
-overfitting our neural network! This was a simple example but the same code can
-be\nused to cluster all several _million_ tiles extracted from the `PANDA`
-dataset and discard\noutliers simultaneously!\n\n## Citation\n\nIf you use
-`HistoPrep` to process the images for your publication, please cite the github
-repository.\n\n```\n@misc{histoprep,\n author = {Pohjonen, Joona and Ariotta,
-Valeria},\n title = {HistoPrep: Preprocessing large medical images for machine
-learning made easy!},\n year = {2022},\n publisher = {GitHub},\n journal =
-{GitHub repository},\n howpublished = {https://github.com/jopo666/
-HistoPrep},\n}\n```\n', 'author': 'jopo666', 'author_email':
-'jopo@birdlover.com', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
-'None', 'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'entry_points': entry_points, 'python_requires':
-'>=3.9,<4.0', } setup(**setup_kwargs)
+Metadata-Version: 2.1 Name: histoprep Version: 2.0.3 Summary: Read and process
+histological slide images with python! Author: jopo666 Author-email:
+jopo@birdlover.com Requires-Python: >=3.9,<4.0 Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Requires-Dist: aicspylibczi (>=3,<4) Requires-Dist: matplotlib
+Requires-Dist: mpire (>=2.6,<3.0) Requires-Dist: numpy Requires-Dist: opencv-
+python-headless (>=4,<5) Requires-Dist: openslide-python (>=1.2,<2.0) Requires-
+Dist: pillow (>=9,<10) Requires-Dist: polars (>=0.16,<0.17) Requires-Dist:
+rich-click (>=1.6,<2.0) Requires-Dist: scikit-learn (>=1,<2) Requires-Dist:
+tqdm Description-Content-Type: text/markdown
+# HistoPrep Preprocessing large medical images for machine learning made easy!
+   Description â¢ Installation â¢ Usage â¢ API_Documentation â¢ Citation
+## Description `HistoPrep` makes is easy to prepare your histological slide
+images for deep learning models. You can easily cut large slide images into
+smaller tiles and then preprocess those tiles (remove tiles with shitty tissue,
+finger marks etc). ## Installation Install [`OpenSlide`](https://openslide.org/
+download/) on your system and then install histoprep with `pip`! ```bash pip
+install histoprep ``` ## Usage Typical workflow for training deep learning
+models with histological images is the following: 1. Cut each slide image into
+smaller tile images. 2. Preprocess smaller tile images by removing tiles with
+bad tissue, staining artifacts. 3. Overfit a pretrained ResNet50 model, report
+100% validation accuracy and publish it in [Nature](https://www.nature.com)
+like everyone else. With `HistoPrep`, steps 1. and 2. are as easy as
+accidentally drinking too much at the research group christmas party and
+proceeding to work remotely until June. Let's start by cutting a slide from the
+[PANDA](https://www.kaggle.com/c/prostate-cancer-grade-assessment) kaggle
+challenge into small tiles. ```python from histoprep import SlideReader # Read
+slide image. reader = SlideReader("./slides/slide_with_ink.jpeg") # Detect
+tissue. threshold, tissue_mask = reader.get_tissue_mask(level=-1) # Extract
+overlapping tile coordinates with less than 50% background. tile_coordinates =
+reader.get_tile_coordinates( tissue_mask, width=512, overlap=0.5,
+max_background=0.5 ) # Save tile images with image metrics for preprocessing.
+tile_metadata = reader.save_regions( "./train_tiles/", tile_coordinates,
+threshold=threshold, save_metrics=True ) ``` ``` slide_with_ink:
+100%|ââââââââââ| 390/390 [00:01<00:00, 295.90it/s] ```
+Let's take a look at the output and visualise the thumbnails. ```bash
+jopo666@~$ tree train_tiles train_tiles âââ slide_with_ink âââ
+metadata.parquet # tile metadata âââ properties.json # tile properties
+âââ thumbnail.jpeg # thumbnail image âââ thumbnail_tiles.jpeg #
+thumbnail with tiles âââ thumbnail_tissue.jpeg # thumbnail of the tissue
+mask âââ tiles [390 entries exceeds filelimit, not opening dir] ``` !
+[Prostate biopsy sample](images/thumbnail.jpeg) ![Tissue mask](images/
+thumbnail_tissue.jpeg) ![Thumbnail with tiles](images/thumbnail_tiles.jpeg)
+That was easy, but it can be annoying to whip up a new python script every time
+you want to cut slides, and thus it is recommended to use the `HistoPrep` CLI
+program! ```bash # Repeat the above code for all images in the PANDA dataset!
+jopo666@~$ HistoPrep --input './train_images/*.tiff' --output ./tiles --width
+512 --overlap 0.5 --max-background 0.5 ``` As we can see from the above images,
+histological slide images often contain areas that we would not like to include
+into our training data. Might seem like a daunting task but let's try it out!
+```python from histoprep.utils import OutlierDetector # Let's wrap the tile
+metadata with a helper class. detector = OutlierDetector(tile_metadata) #
+Cluster tiles based on image metrics. clusters = detector.cluster_kmeans
+(num_clusters=4, random_state=666) # Visualise first cluster.
+reader.get_annotated_thumbnail( image=reader.read_level(-1),
+coordinates=detector.coordinates[clusters == 0] ) ``` ![Tiles in cluster 0]
+(images/thumbnail_blue.jpeg) I said it was gonna be easy! Now we can mark tiles
+in cluster `0` as outliers and start overfitting our neural network! This was a
+simple example but the same code can be used to cluster all several _million_
+tiles extracted from the `PANDA` dataset and discard outliers simultaneously!
+## Citation If you use `HistoPrep` to process the images for your publication,
+please cite the github repository. ``` @misc{histoprep, author = {Pohjonen,
+Joona and Ariotta, Valeria}, title = {HistoPrep: Preprocessing large medical
+images for machine learning made easy!}, year = {2022}, publisher = {GitHub},
+journal = {GitHub repository}, howpublished = {https://github.com/jopo666/
+HistoPrep}, } ```
```

