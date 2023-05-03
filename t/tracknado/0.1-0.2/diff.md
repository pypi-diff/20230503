# Comparing `tmp/tracknado-0.1.tar.gz` & `tmp/tracknado-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracknado-0.1.tar", last modified: Fri Apr 28 09:45:01 2023, max compression
+gzip compressed data, was "tracknado-0.2.tar", last modified: Wed May  3 11:16:17 2023, max compression
```

## Comparing `tracknado-0.1.tar` & `tracknado-0.2.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:45:01.739642 tracknado-0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:45:01.735642 tracknado-0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:45:01.735642 tracknado-0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-28 09:44:50.000000 tracknado-0.1/.github/workflows/python-publish.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-04-28 09:44:50.000000 tracknado-0.1/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-04-28 09:44:50.000000 tracknado-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-28 09:45:01.739642 tracknado-0.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2422 2023-04-28 09:44:50.000000 tracknado-0.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-04-28 09:44:50.000000 tracknado-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 09:45:01.739642 tracknado-0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-04-28 09:44:50.000000 tracknado-0.1/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    63958 2023-04-28 09:44:50.000000 tracknado-0.1/test_hub_creation.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:45:01.735642 tracknado-0.1/tracknado/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:44:50.000000 tracknado-0.1/tracknado/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-28 09:45:01.000000 tracknado-0.1/tracknado/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-04-28 09:44:50.000000 tracknado-0.1/tracknado/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    25765 2023-04-28 09:44:50.000000 tracknado-0.1/tracknado/design.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:45:01.739642 tracknado-0.1/tracknado/old/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3967 2023-04-28 09:44:50.000000 tracknado-0.1/tracknado/old/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6644 2023-04-28 09:44:50.000000 tracknado-0.1/tracknado/old/grouping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1359 2023-04-28 09:44:50.000000 tracknado-0.1/tracknado/old/hub_setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6442 2023-04-28 09:44:50.000000 tracknado-0.1/tracknado/old/make_hub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2356 2023-04-28 09:44:50.000000 tracknado-0.1/tracknado/old/track.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2257 2023-04-28 09:44:50.000000 tracknado-0.1/tracknado/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:45:01.739642 tracknado-0.1/tracknado.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-28 09:45:01.000000 tracknado-0.1/tracknado.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-28 09:45:01.000000 tracknado-0.1/tracknado.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:45:01.000000 tracknado-0.1/tracknado.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-28 09:45:01.000000 tracknado-0.1/tracknado.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 09:45:01.000000 tracknado-0.1/tracknado.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 09:45:01.000000 tracknado-0.1/tracknado.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:16:17.082956 tracknado-0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:16:17.078956 tracknado-0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:16:17.078956 tracknado-0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-03 11:16:05.000000 tracknado-0.2/.github/workflows/python-publish.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-05-03 11:16:05.000000 tracknado-0.2/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-05-03 11:16:05.000000 tracknado-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-03 11:16:17.082956 tracknado-0.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2422 2023-05-03 11:16:05.000000 tracknado-0.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      765 2023-05-03 11:16:05.000000 tracknado-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 11:16:17.082956 tracknado-0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-03 11:16:05.000000 tracknado-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:16:17.078956 tracknado-0.2/tracknado/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-03 11:16:05.000000 tracknado-0.2/tracknado/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-03 11:16:16.000000 tracknado-0.2/tracknado/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27527 2023-05-03 11:16:05.000000 tracknado-0.2/tracknado/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-05-03 11:16:05.000000 tracknado-0.2/tracknado/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:16:17.082956 tracknado-0.2/tracknado/old/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3967 2023-05-03 11:16:05.000000 tracknado-0.2/tracknado/old/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6644 2023-05-03 11:16:05.000000 tracknado-0.2/tracknado/old/grouping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1359 2023-05-03 11:16:05.000000 tracknado-0.2/tracknado/old/hub_setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6442 2023-05-03 11:16:05.000000 tracknado-0.2/tracknado/old/make_hub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2356 2023-05-03 11:16:05.000000 tracknado-0.2/tracknado/old/track.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      559 2023-05-03 11:16:05.000000 tracknado-0.2/tracknado/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:16:17.082956 tracknado-0.2/tracknado.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-03 11:16:17.000000 tracknado-0.2/tracknado.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-03 11:16:17.000000 tracknado-0.2/tracknado.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 11:16:17.000000 tracknado-0.2/tracknado.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-03 11:16:17.000000 tracknado-0.2/tracknado.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-03 11:16:17.000000 tracknado-0.2/tracknado.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 11:16:17.000000 tracknado-0.2/tracknado.egg-info/top_level.txt
```

### Comparing `tracknado-0.1/.github/workflows/python-publish.yml` & `tracknado-0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tracknado-0.1/LICENSE` & `tracknado-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tracknado-0.1/PKG-INFO` & `tracknado-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracknado
-Version: 0.1
+Version: 0.2
 Summary: CLI library to generate UCSC trackhubs from sequencing data
 Author-email: Alastair Smith <alastair.smith@ndcls.ox.ac.uk>
 License: GNU GENERAL PUBLIC LICENSE Version 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tracknado-0.1/README.md` & `tracknado-0.2/README.md`

 * *Files identical despite different names*

### Comparing `tracknado-0.1/pyproject.toml` & `tracknado-0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     "click",
     "pandas",
     "cookiecutter",
     "setuptools_scm",
     "seaborn",
     "trackhub",
     "Pillow",
+    "loguru",
 ]
 
 [project.scripts]
 tracknado = "tracknado.cli:cli"
 
 [tool.setuptools_scm]
 write_to = "tracknado/_version.py"
```

### Comparing `tracknado-0.1/tracknado/cli.py` & `tracknado-0.2/tracknado/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,52 @@
 import os
-import pathlib
-import sys
-
 import click
-import pandas as pd
 
-from tracknado.design import HubDesign, HubFiles, HubGenerator
-from tracknado.utils import OptionEatAll
+class OptionEatAll(click.Option):
+
+    def __init__(self, *args, **kwargs):
+        self.save_other_options = kwargs.pop('save_other_options', True)
+        nargs = kwargs.pop('nargs', -1)
+        assert nargs == -1, 'nargs, if set, must be -1 not {}'.format(nargs)
+        super(OptionEatAll, self).__init__(*args, **kwargs)
+        self._previous_parser_process = None
+        self._eat_all_parser = None
+
+    def add_to_parser(self, parser, ctx):
+
+        def parser_process(value, state):
+            # method to hook to the parser.process
+            done = False
+            value = [value]
+            if self.save_other_options:
+                # grab everything up to the next option
+                while state.rargs and not done:
+                    for prefix in self._eat_all_parser.prefixes:
+                        if state.rargs[0].startswith(prefix):
+                            done = True
+                    if not done:
+                        value.append(state.rargs.pop(0))
+            else:
+                # grab everything remaining
+                value += state.rargs
+                state.rargs[:] = []
+            value = tuple(value)
+
+            # call the actual process
+            self._previous_parser_process(value, state)
+
+        retval = super(OptionEatAll, self).add_to_parser(parser, ctx)
+        for name in self.opts:
+            our_parser = parser._long_opt.get(name) or parser._short_opt.get(name)
+            if our_parser:
+                self._eat_all_parser = our_parser
+                self._previous_parser_process = our_parser.process
+                our_parser.process = parser_process
+                break
+        return retval
 
 
 @click.group()
 def cli():
     """Tracknado: A tool for generating UCSC track hubs
     Tracknado go BRRRR!
     """
@@ -141,40 +177,42 @@
     The --description-html option can be used to provide a path to an HTML file that will be used
     as the hub description. The HTML file will be copied to the hub directory and the path to the
     file will be added to the hub.txt file.
 
     """
 
     # sys.tracebacklimit = 0
+    import pandas as pd
+    from tracknado.api import TrackDesign, HubGenerator
 
     # Fix cli to api differences
     kwargs["color_by"] = kwargs["color_by"][0] if kwargs["color_by"] else None
 
 
     # Get design
     if not kwargs["details"]:
         assert kwargs[
             "input_files"
         ], "Input file MUST be provided if not specifying by a design file"
 
         kwargs.pop("details")
 
-        design = HubDesign.from_files(
+        design = TrackDesign.from_files(
             kwargs["input_files"],
             infer_attributes=kwargs["infer_details"],
             chromosome_sizes=kwargs["chrom_sizes"],
             **kwargs
         )
 
     else:
         details = pd.read_csv(kwargs["details"], sep=r"\s+|\t|,", engine="python")
         kwargs.pop("input_files")
         kwargs.pop("details")
 
-        design = HubDesign.from_design(
+        design = TrackDesign.from_design(
             details,
             infer_attributes=kwargs["infer_details"],
             chromosome_sizes=kwargs["chrom_sizes"],
             **kwargs
         )
 
 
@@ -269,19 +307,22 @@
     This command will merge multiple seqnado created hubs into a single hub. 
     
     This requires that the hubs were created with the tracknado create command and that the hub designs were saved using the --save-hub-design option.
     """
 
     assert all(os.path.exists(hub) for hub in kwargs["input_files"]), "All input files must exist"
 
+    import pandas as pd
+    from tracknado.api import TrackDesign, HubGenerator
+
     for ii, hub in enumerate(kwargs["input_files"]):
         if ii == 0:
-            design = HubDesign.from_pickle(hub)
+            design = TrackDesign.from_pickle(hub)
         else:
-            design = design + HubDesign.from_pickle(hub) # type: ignore
+            design = design + TrackDesign.from_pickle(hub) # type: ignore
         
 
     hub = HubGenerator(
         outdir=kwargs["output"],
         track_design=design, # type: ignore
         genome=kwargs["genome_name"],
         hub_name=kwargs["hub_name"],
```

### Comparing `tracknado-0.1/tracknado/design.py` & `tracknado-0.2/tracknado/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 import pickle
 import re
 import shutil
 import subprocess
 import tempfile
 from collections import defaultdict, namedtuple
 from typing import Dict, List, Literal, Tuple, Union
+import hashlib
+import json
+from loguru import logger
 
-import numpy as np
 import pandas as pd
 import seaborn as sns
 import trackhub
 
 from tracknado.utils import has_valid_chromsizes, has_tracks_to_convert
 
 
@@ -23,16 +25,32 @@
         duplicate_counts[row.basename] += 1
         if duplicate_counts[row.basename] > 1:
             name = f"{row.name}_{duplicate_counts[row.basename]}"
             basename = f"{row.basename}_{duplicate_counts[row.basename]}.{row.ext}"
             df.loc[row.Index, "name"] = name
             df.loc[row.Index, "basename"] = basename
 
+def get_hash(obj: object) -> str:
+    """Get hash of object"""
+    return hashlib.md5(json.dumps(obj).encode("utf-8")).hexdigest()
 
-class HubFiles:
+def get_hash_for_df(df: pd.DataFrame, columns: Union[List[str], pd.Index] = None) -> List[str]:
+
+    if columns is None:
+        columns = df.columns
+    
+    hashes = []
+    for row in df.itertuples():
+        x = tuple([getattr(row, x) for x in columns])
+        hash = get_hash(x)
+        hashes.append(hash)
+    
+    return hashes
+
+class TrackFiles:
     def __init__(
         self,
         files: Union[List[str], List[pathlib.Path], pd.DataFrame],
         infer_subgroups: bool = False,
         infer_attributes: bool = False,
         deduplicate: bool = False,
         convert_files: bool = False,
@@ -156,15 +174,15 @@
         df_attributes = df["name"].str.extract(regex)
 
         # Remove any columns that are all NaN
         df_attributes = df_attributes.loc[:, df_attributes.notnull().any()]
 
         return df.join(df_attributes)
 
-class HubDesign:
+class TrackDesign:
     def __init__(
         self,
         details: pd.DataFrame,
         color_by: List[str] = None,
         subgroup_by: List[str] = None,
         overlay_by: List[str] = None,
         supergroup_by: List[str] = None,
@@ -187,32 +205,32 @@
 
         self.overlay_tracks = self._get_overlay_tracks()
         self._add_overlay_track_indicators()
 
         self._add_track_colors(color_by=color_by)
 
     @classmethod
-    def from_files(cls, files: List[pathlib.Path], **kwargs) -> "HubDesign":
-        hub_files = HubFiles(files, **kwargs)
+    def from_files(cls, files: List[pathlib.Path], **kwargs) -> "TrackDesign":
+        hub_files = TrackFiles(files, **kwargs)
 
         extra_kwargs = dict()
         if hub_files.subgroup_columns:
             extra_kwargs["subgroup_by"] = hub_files.subgroup_columns
 
 
         return cls(hub_files.files, **kwargs, **extra_kwargs)
 
     @classmethod
-    def from_design(cls, design: pd.DataFrame, **kwargs) -> "HubDesign":
+    def from_design(cls, design: pd.DataFrame, **kwargs) -> "TrackDesign":
         design = design.copy()
-        design = HubFiles(design, **kwargs).files
+        design = TrackFiles(design, **kwargs).files
         return cls(design, **kwargs)
     
     @classmethod
-    def from_pickle(cls, pickle_file: pathlib.Path) -> "HubDesign":
+    def from_pickle(cls, pickle_file: pathlib.Path) -> "TrackDesign":
         with open(pickle_file, "rb") as f:
             return pickle.load(f)
 
     def _add_track_colors(
         self,
         color_by: Union[str, List[str]] = None,
         pallet: str = "tab20",
@@ -343,16 +361,21 @@
         if self._supertrack_columns:
             assert all(
                 [c in self.details.columns for c in self._supertrack_columns]
             ), f"SuperTrack columns {self._supertrack_columns} missing"
 
             supertracks = dict()
             for grouping, df in self.details.groupby(self._supertrack_columns):
-                supertracks[grouping] = trackhub.SuperTrack(
-                    name="_".join(grouping),
+                
+                track_id = tuple(grouping) if not isinstance(grouping, str) else (grouping,)
+                track_name = "_".join(grouping)
+
+
+                supertracks[get_hash(track_id)] = trackhub.SuperTrack(
+                    name=track_name,
                 )
 
         else:
             supertracks = dict()
 
         return supertracks
 
@@ -360,108 +383,120 @@
         """Add a column to the details dataframe with a SuperTrack indicator for each track"""
 
         if self._supertrack_columns:
             assert all(
                 [c in self.details.columns for c in self._supertrack_columns]
             ), f"SuperTrack columns {self._supertrack_columns} missing"
 
-            self.details["supertrack"] = self.details[self._supertrack_columns].apply(
-                lambda row: "_".join(row), axis=1
-            )
-
+            self.details["supertrack"] = get_hash_for_df(self.details, self._supertrack_columns)
+    
     def _get_composite_tracks(self) -> Dict[str, trackhub.CompositeTrack]:
         """Generate a dictionary of CompositeTracks from the details dataframe"""
 
         composite_tracks = dict()
         if "supertrack" in self.details.columns:
-            for grouping, df in self.details.groupby(["supertrack", "ext"]):
+            for (supertrack, ext) , df in self.details.groupby(["supertrack", "ext"]):
 
                 subgroupings = df.iloc[df["subgroup_names"].drop_duplicates().index, :][
                     "subgroup_definition"
                 ]
                 dimensions = dict(
                     zip(
                         [f"dim{d}" for d in ["X", "Y", "A", "B", "C", "D"]],
                         subgroupings,
                     )
                 )
 
+                supertrack_name = self.super_tracks[get_hash(supertrack)].name
+                composite_name = "_".join([supertrack_name, ext])
+
                 composite = trackhub.CompositeTrack(
-                    name="_".join(grouping) if isinstance(grouping, tuple) else grouping,
-                    tracktype=grouping[1],
+                    name=composite_name,
+                    tracktype=ext,
                     dimensions=" ".join([f"{k}={v}" for k, v in dimensions.items()])
                     if dimensions
                     else None,
                     sortOrder=" ".join([f"{k}=+" for k in subgroupings]),
                     visibility="hide",
                     dragAndDrop="subTracks",
                     allButtonPair="off",
                 )
 
-                self.super_tracks[grouping[0]].add_tracks(composite)
-                composite_tracks[grouping] = composite
+                self.super_tracks[supertrack].add_tracks(composite)
+                composite_tracks[get_hash((supertrack, ext))] = composite
 
         elif self._subgroup_columns:
-            for grouping, df in self.details.groupby("ext"):
+            for ext, df in self.details.groupby("ext"):
                 composite = trackhub.CompositeTrack(
-                    name="_".join(grouping) if isinstance(grouping, tuple) else grouping,
-                    tracktype=grouping,
+                    name=ext,
+                    tracktype=ext,
                     visibility="hide",
                     dragAndDrop="subTracks",
                     allButtonPair="off",
                 )
 
-                composite_tracks[grouping] = composite
+                composite_tracks[get_hash((ext,))] = composite
         
         else:
             composite_tracks = dict()
 
         return composite_tracks
 
     def _add_composite_track_indicators(self):
         """Add a column to the details dataframe with a CompositeTrack indicator for each track"""
 
         if self.composite_tracks:
             composite_columns = self._supertrack_columns if self._supertrack_columns else []
             composite_columns.append("ext")
 
-            self.details["composite"] = self.details.loc[:, composite_columns].apply(
-                lambda row: "_".join(row), axis=1
+            self.details["composite"] = get_hash_for_df(self.details, composite_columns)
+
+            assert self.details["composite"].isin(self.composite_tracks.keys()).all(), (
+                "Composite tracks not found in details dataframe"
             )
 
     def _get_overlay_tracks(self):
         """Generate a dictionary of OverlayTracks from the details dataframe"""
 
         if self._overlay_columns:
             assert all(
                 [c in self.details.columns for c in self._overlay_columns]
             ), f"Overlay columns {self._overlay_columns} missing"
 
             overlay_tracks = dict()
+            overlay_columns = list(self._overlay_columns) if not isinstance(self._overlay_columns, str) else [self._overlay_columns,]
 
             if "supertrack" in self.details.columns:
 
-                for grouping, df in self.details.groupby(
+                for (supertrack, overlay) , df in self.details.groupby(
                     ["supertrack", *self._overlay_columns]
                 ):
-                    overlay = trackhub.AggregateTrack(
+                    
+                    supertrack_name = self.super_tracks[supertrack].name
+                    overlay_name = "_".join([supertrack_name, *overlay]) + "_overlay"
+
+                    overlay_track = trackhub.AggregateTrack(
                         aggregate="transparentOverlay",
-                        name="_".join(grouping) if isinstance(grouping, tuple) else grouping,
+                        name=overlay_name,
                     )
 
-                    self.super_tracks[grouping[0]].add_tracks(overlay)
-                    overlay_tracks[grouping] = overlay
+                    self.super_tracks[supertrack].add_tracks(overlay)
+                    overlay_tracks[get_hash(tuple([supertrack, overlay]))] = overlay_track
 
             else:
-                for grouping, df in self.details.groupby(self._overlay_columns):
-                    overlay = trackhub.AggregateTrack(
+                for overlay, df in self.details.groupby(self._overlay_columns):
+
+                    overlay_name = "_".join(overlay) if isinstance(overlay, tuple) else overlay
+                    overlay_id = tuple(overlay) if isinstance(overlay, tuple) else (overlay,)
+
+                    overlay_track = trackhub.AggregateTrack(
                         aggregate="transparentOverlay",
-                        name="_".join(grouping) if isinstance(grouping, tuple) else grouping,
+                        name=overlay_name,
                     )
-                    overlay_tracks[grouping] = overlay
+                    overlay_tracks[get_hash(overlay_id)] = overlay_track
 
         else:
             overlay_tracks = dict()
 
         return overlay_tracks
 
     def _add_overlay_track_indicators(self):
@@ -470,22 +505,25 @@
         if self._overlay_columns:
 
             overlay_columns = (
                 self._supertrack_columns if self._supertrack_columns else []
             )
             overlay_columns.extend(self._overlay_columns)
 
-            self.details["overlay"] = self.details.loc[:, overlay_columns].apply(
-                lambda row: "_".join(row), axis=1
+            self.details["overlay"] = get_hash_for_df(self.details, overlay_columns)
+
+            assert self.details["overlay"].isin(self.overlay_tracks.keys()).all(), (
+                "Overlay tracks not found in details dataframe"
             )
 
+
     def __add__(self, other):
         """Combine two HubDesign objects"""
             
-        assert isinstance(other, HubDesign), "Can only combine HubDesign objects"
+        assert isinstance(other, TrackDesign), "Can only combine HubDesign objects"
 
         self.details = pd.concat([self.details, other.details], ignore_index=True)
         fix_duplicate_names(self.details)
 
         if any([self._supertrack_columns, other._supertrack_columns]):
             self._supertrack_columns = sorted(
                 list(set(self._supertrack_columns + other._supertrack_columns))
@@ -515,15 +553,15 @@
 
 
 class HubGenerator:
     def __init__(
         self,
         hub_name: str,
         genome: str,
-        track_design: HubDesign,
+        track_design: TrackDesign,
         outdir: pathlib.Path,
         description_html: pathlib.Path = None,
         hub_email: str = "",
         custom_genome: bool = False,
         genome_twobit: pathlib.Path = None,
         genome_organism: str = None,
         genome_default_position: str = "chr1:10000-20000",
@@ -563,26 +601,31 @@
         
         for row in self.track_design.details.itertuples():
 
             # If the row has a "composite" attribute
             if hasattr(row, "composite"):
                 composite_track = self.track_design.composite_tracks[row.composite]
                 # Create a new track and add it as a subtrack to the composite track
-                track = self._get_track(row, suffix=f"_{row.composite}")
+                track = self._get_track(row, suffix=f"_{composite_track.name}")
                 composite_track.add_subtrack(track)
 
             # If the row has an "overlay" attribute
-            elif hasattr(row, "overlay"):
+            if hasattr(row, "overlay"):
                 overlay_track = self.track_design.overlay_tracks[row.overlay]
                 # Create a new track and add it to the overlay track
-                track = self._get_track(row, suffix=f"_{row.overlay}")
-                overlay_track.add_tracks(track)
+                track = self._get_track(row, suffix=f"_{overlay_track.name}")
+
+                # Ignore the track if it is not a signal track e.g. bigWig
+                if track.tracktype not in ["bigWig", ]:
+                    logger.warning(f"Track {track.name} is not a signal track and will be ignored for the overlay track {overlay_track.name}")
+                else:
+                    overlay_track.add_subtrack(track)
 
             # If the row doesn't have a "supertrack" attribute
-            elif not hasattr(row, "supertrack"):
+            if not hasattr(row, "supertrack"):
                 # Create a new track and add it to the trackdb
                 track = self._get_track(row)
                 self.trackdb.add_tracks(track)
 
         # Add the supertracks or composite/overlay tracks to the trackdb
         if self.track_design.super_tracks:
             tracks = self.track_design.super_tracks.values()
@@ -591,14 +634,15 @@
             if self.custom_genome:
                 for t in [*self.track_design.composite_tracks.values(), *self.track_design.overlay_tracks.values()]:
                     t.add_params(group=self._hub.hub)
 
         else:
             tracks = [*self.track_design.composite_tracks.values(), *self.track_design.overlay_tracks.values()]
 
+        # Add the composite/overlay and supertracks to the trackdb
         for track in tracks:
             # Add group if custom genome
             if self.custom_genome:
                 track.add_params(group=self._hub.hub)
             self.trackdb.add_tracks(track)
```

### Comparing `tracknado-0.1/tracknado/old/cli.py` & `tracknado-0.2/tracknado/old/cli.py`

 * *Files identical despite different names*

### Comparing `tracknado-0.1/tracknado/old/grouping.py` & `tracknado-0.2/tracknado/old/grouping.py`

 * *Files identical despite different names*

### Comparing `tracknado-0.1/tracknado/old/hub_setup.py` & `tracknado-0.2/tracknado/old/hub_setup.py`

 * *Files identical despite different names*

### Comparing `tracknado-0.1/tracknado/old/make_hub.py` & `tracknado-0.2/tracknado/old/make_hub.py`

 * *Files identical despite different names*

### Comparing `tracknado-0.1/tracknado/old/track.py` & `tracknado-0.2/tracknado/old/track.py`

 * *Files identical despite different names*

### Comparing `tracknado-0.1/tracknado.egg-info/PKG-INFO` & `tracknado-0.2/tracknado.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracknado
-Version: 0.1
+Version: 0.2
 Summary: CLI library to generate UCSC trackhubs from sequencing data
 Author-email: Alastair Smith <alastair.smith@ndcls.ox.ac.uk>
 License: GNU GENERAL PUBLIC LICENSE Version 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

