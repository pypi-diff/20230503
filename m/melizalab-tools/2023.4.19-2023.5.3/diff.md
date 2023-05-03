# Comparing `tmp/melizalab-tools-2023.4.19.tar.gz` & `tmp/melizalab-tools-2023.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melizalab-tools-2023.4.19.tar", last modified: Wed Apr 19 14:42:31 2023, max compression
+gzip compressed data, was "melizalab-tools-2023.5.3.tar", last modified: Wed May  3 15:07:50 2023, max compression
```

## Comparing `melizalab-tools-2023.4.19.tar` & `melizalab-tools-2023.5.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-04-19 14:42:31.432894 melizalab-tools-2023.4.19/
--rw-r--r--   0 dmeliza    (503) staff       (20)     1379 2023-04-19 14:42:31.433019 melizalab-tools-2023.4.19/PKG-INFO
--rw-r--r--   0 dmeliza    (503) staff       (20)      852 2023-03-17 16:55:38.000000 melizalab-tools-2023.4.19/README.md
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-04-19 14:42:31.417307 melizalab-tools-2023.4.19/dlab/
--rw-r--r--   0 dmeliza    (503) staff       (20)       24 2022-10-13 22:35:34.000000 melizalab-tools-2023.4.19/dlab/__init__.py
--rw-r--r--   0 dmeliza    (503) staff       (20)      898 2023-03-16 17:12:17.000000 melizalab-tools-2023.4.19/dlab/cache.py
--rw-r--r--   0 dmeliza    (503) staff       (20)      122 2023-04-19 14:41:51.000000 melizalab-tools-2023.4.19/dlab/core.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     1838 2023-03-16 17:04:03.000000 melizalab-tools-2023.4.19/dlab/extracellular.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     6024 2023-03-16 17:04:03.000000 melizalab-tools-2023.4.19/dlab/extract_waveforms.py
--rw-r--r--   0 dmeliza    (503) staff       (20)    17548 2023-04-19 14:41:51.000000 melizalab-tools-2023.4.19/dlab/kilo.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     6483 2023-03-17 16:55:38.000000 melizalab-tools-2023.4.19/dlab/nbank.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     2034 2023-03-10 23:03:29.000000 melizalab-tools-2023.4.19/dlab/plotting.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     5048 2023-03-08 19:24:21.000000 melizalab-tools-2023.4.19/dlab/pprox.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     1790 2023-03-10 23:03:29.000000 melizalab-tools-2023.4.19/dlab/signal.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     4275 2023-04-19 14:41:51.000000 melizalab-tools-2023.4.19/dlab/spikes.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     2055 2023-03-16 17:04:03.000000 melizalab-tools-2023.4.19/dlab/util.py
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-04-19 14:42:31.422634 melizalab-tools-2023.4.19/melizalab_tools.egg-info/
--rw-r--r--   0 dmeliza    (503) staff       (20)     1379 2023-04-19 14:42:31.000000 melizalab-tools-2023.4.19/melizalab_tools.egg-info/PKG-INFO
--rw-r--r--   0 dmeliza    (503) staff       (20)      572 2023-04-19 14:42:31.000000 melizalab-tools-2023.4.19/melizalab_tools.egg-info/SOURCES.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)        1 2023-04-19 14:42:31.000000 melizalab-tools-2023.4.19/melizalab_tools.egg-info/dependency_links.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)       65 2023-04-19 14:42:31.000000 melizalab-tools-2023.4.19/melizalab_tools.egg-info/entry_points.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)        1 2022-10-12 18:42:40.000000 melizalab-tools-2023.4.19/melizalab_tools.egg-info/not-zip-safe
--rw-r--r--   0 dmeliza    (503) staff       (20)      131 2023-04-19 14:42:31.000000 melizalab-tools-2023.4.19/melizalab_tools.egg-info/requires.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)        5 2023-04-19 14:42:31.000000 melizalab-tools-2023.4.19/melizalab_tools.egg-info/top_level.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)      121 2023-02-16 22:14:18.000000 melizalab-tools-2023.4.19/pyproject.toml
--rw-r--r--   0 dmeliza    (503) staff       (20)     1087 2023-04-19 14:42:31.434216 melizalab-tools-2023.4.19/setup.cfg
--rw-r--r--   0 dmeliza    (503) staff       (20)      106 2020-11-05 14:34:56.000000 melizalab-tools-2023.4.19/setup.py
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-04-19 14:42:31.432384 melizalab-tools-2023.4.19/tests/
--rw-r--r--   0 dmeliza    (503) staff       (20)     8717 2023-03-08 19:24:21.000000 melizalab-tools-2023.4.19/tests/test_pprox.py
--rw-r--r--   0 dmeliza    (503) staff       (20)      506 2023-03-10 19:08:55.000000 melizalab-tools-2023.4.19/tests/test_signal.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     1601 2023-04-19 14:41:51.000000 melizalab-tools-2023.4.19/tests/test_spikes.py
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-05-03 15:07:50.464938 melizalab-tools-2023.5.3/
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1378 2023-05-03 15:07:50.465088 melizalab-tools-2023.5.3/PKG-INFO
+-rw-r--r--   0 dmeliza    (503) staff       (20)      852 2023-03-17 16:55:38.000000 melizalab-tools-2023.5.3/README.md
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-05-03 15:07:50.450790 melizalab-tools-2023.5.3/dlab/
+-rw-r--r--   0 dmeliza    (503) staff       (20)       24 2022-10-13 22:35:34.000000 melizalab-tools-2023.5.3/dlab/__init__.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)      898 2023-03-16 17:12:17.000000 melizalab-tools-2023.5.3/dlab/cache.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)      122 2023-05-03 15:07:13.000000 melizalab-tools-2023.5.3/dlab/core.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1838 2023-03-16 17:04:03.000000 melizalab-tools-2023.5.3/dlab/extracellular.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     6024 2023-03-16 17:04:03.000000 melizalab-tools-2023.5.3/dlab/extract_waveforms.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)    18016 2023-05-03 15:00:58.000000 melizalab-tools-2023.5.3/dlab/kilo.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     6483 2023-05-03 15:03:04.000000 melizalab-tools-2023.5.3/dlab/nbank.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     2034 2023-03-10 23:03:29.000000 melizalab-tools-2023.5.3/dlab/plotting.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     5200 2023-05-03 15:00:58.000000 melizalab-tools-2023.5.3/dlab/pprox.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1790 2023-03-10 23:03:29.000000 melizalab-tools-2023.5.3/dlab/signal.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     4213 2023-05-03 15:00:58.000000 melizalab-tools-2023.5.3/dlab/spikes.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     2055 2023-03-16 17:04:03.000000 melizalab-tools-2023.5.3/dlab/util.py
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-05-03 15:07:50.458987 melizalab-tools-2023.5.3/melizalab_tools.egg-info/
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1378 2023-05-03 15:07:50.000000 melizalab-tools-2023.5.3/melizalab_tools.egg-info/PKG-INFO
+-rw-r--r--   0 dmeliza    (503) staff       (20)      572 2023-05-03 15:07:50.000000 melizalab-tools-2023.5.3/melizalab_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)        1 2023-05-03 15:07:50.000000 melizalab-tools-2023.5.3/melizalab_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)       65 2023-05-03 15:07:50.000000 melizalab-tools-2023.5.3/melizalab_tools.egg-info/entry_points.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)        1 2022-10-12 18:42:40.000000 melizalab-tools-2023.5.3/melizalab_tools.egg-info/not-zip-safe
+-rw-r--r--   0 dmeliza    (503) staff       (20)      131 2023-05-03 15:07:50.000000 melizalab-tools-2023.5.3/melizalab_tools.egg-info/requires.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)        5 2023-05-03 15:07:50.000000 melizalab-tools-2023.5.3/melizalab_tools.egg-info/top_level.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)      121 2023-02-16 22:14:18.000000 melizalab-tools-2023.5.3/pyproject.toml
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1087 2023-05-03 15:07:50.467892 melizalab-tools-2023.5.3/setup.cfg
+-rw-r--r--   0 dmeliza    (503) staff       (20)      106 2020-11-05 14:34:56.000000 melizalab-tools-2023.5.3/setup.py
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-05-03 15:07:50.464156 melizalab-tools-2023.5.3/tests/
+-rw-r--r--   0 dmeliza    (503) staff       (20)     8722 2023-05-03 15:00:58.000000 melizalab-tools-2023.5.3/tests/test_pprox.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)      506 2023-03-10 19:08:55.000000 melizalab-tools-2023.5.3/tests/test_signal.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1601 2023-04-19 14:41:51.000000 melizalab-tools-2023.5.3/tests/test_spikes.py
```

### Comparing `melizalab-tools-2023.4.19/PKG-INFO` & `melizalab-tools-2023.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melizalab-tools
-Version: 2023.4.19
+Version: 2023.5.3
 Summary: Meliza lab scripts and modules for auditory neurophysiology
 Home-page: https://github.com/melizalab/melizalab-tools
 Author: Dan Meliza
 Author-email: dan@meliza.org
 Maintainer: Dan Meliza
 Maintainer-email: dan@meliza.org
 License: BSD 3-Clause License
```

### Comparing `melizalab-tools-2023.4.19/README.md` & `melizalab-tools-2023.5.3/README.md`

 * *Files identical despite different names*

### Comparing `melizalab-tools-2023.4.19/dlab/cache.py` & `melizalab-tools-2023.5.3/dlab/cache.py`

 * *Files identical despite different names*

### Comparing `melizalab-tools-2023.4.19/dlab/extracellular.py` & `melizalab-tools-2023.5.3/dlab/extracellular.py`

 * *Files identical despite different names*

### Comparing `melizalab-tools-2023.4.19/dlab/extract_waveforms.py` & `melizalab-tools-2023.5.3/dlab/extract_waveforms.py`

 * *Files identical despite different names*

### Comparing `melizalab-tools-2023.4.19/dlab/kilo.py` & `melizalab-tools-2023.5.3/dlab/kilo.py`

 * *Files 7% similar despite different names*

```diff
@@ -217,15 +217,15 @@
     import argparse
     import os
 
     from dlab.core import __version__
     from dlab.extracellular import entry_metadata, iter_entries
     from dlab.util import json_serializable
 
-    version = "2023.04.18"
+    version = "2023.04.26"
 
     p = argparse.ArgumentParser(
         description="group kilosorted spikes into pprox files based on cluster and trial"
     )
     p.add_argument(
         "-v",
         "--version",
@@ -276,17 +276,19 @@
     )
     p.add_argument(
         "--mua",
         action="store_true",
         help="save multiunit clusters along with single units",
     )
     p.add_argument(
-        "--name",
-        "-n",
-        help="base name of the unit (default is based on 'recording' field of trials pprox) ",
+        "--artifact-reject-thresh",
+        type=float,
+        default=6.0,
+        help="threshold for rejecting artifact spikes (max absolute amplitude"
+        " more than x times max absolute amplitude of the mean spike)",
     )
     p.add_argument(
         "--save-waveforms",
         "-W",
         action="store_true",
         help="save representative waveforms from each unit's main channel in an hdf5 file",
     )
@@ -373,90 +375,103 @@
             entry_attrs = tuple(entry_metadata(e) for _, e in iter_entries(afp))
 
         # this pandas magic sorts the events by cluster and trial
         logging.info("- sorting events into trials:")
         events["trial"] = (
             trials.recording_start.searchsorted(events.time, side="left") - 1
         )
-        clusters = events.groupby("clust").apply(
-            lambda df: df.groupby("trial").apply(lambda x: x.time.to_numpy())
-        )
-        # for some reason the trials end up in columns if we're only looking at
-        # a subset of clusters. This sort of undefined behavior in pandas is
-        # sure annoying.
-        if args.cluster is not None:
-            clusters = clusters.stack("trial")
 
         total_spikes = 0
         total_clusters = 0
-        for clust_id, cluster in clusters.groupby("clust"):
+        for clust_id, cluster in events.groupby("clust"):
             clust_info = info.loc[clust_id]
             clust_type = clust_info["group"]
-            n_spikes = cluster.apply(len).agg("sum")
-            # left join to trial information table - empty trials will be nan
-            clust_trials = trials.join(
-                cluster.reset_index(0, drop=True).rename("events")
-            )
+            n_spikes = len(cluster)
             if clust_type == "noise" or (clust_type == "mua" and not args.mua):
                 logging.info(
                     "  - cluster %d (%d spikes, %s) -> skipped",
                     clust_id,
                     n_spikes,
                     clust_type,
                 )
                 continue
-            total_spikes += n_spikes
-            total_clusters += 1
-            outfile = args.output / f"{recording_name}_c{clust_id}.pprox"
             logging.info(
-                "  ✓ cluster %d (%d spikes, %s) -> %s",
+                "  ✓ cluster %d (%d spikes, %s)",
                 clust_id,
                 n_spikes,
                 clust_type,
+            )
+            # remove artifact spikes
+            n_before = int(args.waveform_pre_peak * params["sampling_rate"] / 1000)
+            n_after = int(args.waveform_post_peak * params["sampling_rate"] / 1000)
+            spikes = cluster[
+                (cluster.time > n_before) & (cluster.time < (nsamples - n_after))
+            ]
+            waveforms = qs.peaks(
+                recording[:, clust_info["ch"]],
+                spikes.time,
+                n_before=n_before,
+                n_after=n_after,
+            )
+            mean_spike = waveforms.mean(0)
+            included = np.abs(waveforms).max(-1) < (
+                np.abs(mean_spike).max(-1) * args.artifact_reject_thresh
+            )
+            n_included = included.sum()
+            if n_included < n_spikes:
+                cluster = cluster[included]
+                waveforms = waveforms[included]
+                logging.info(
+                    "    - %d artifact spike(s) excluded", n_spikes - n_included
+                )
+            # aggregate spikes by trial and left join to trial information table
+            # - empty trials will be nan
+            clust_trials = trials.join(
+                cluster.groupby("trial")
+                .apply(lambda x: x.time.to_numpy())
+                .rename("events")
+            )
+            total_spikes += n_spikes
+            total_clusters += 1
+            outfile = args.output / f"{recording_name}_c{clust_id}.pprox"
+            logging.info(
+                "    - %d spikes -> %s",
+                n_included,
                 outfile,
             )
             clust_trials = pprox.from_trials(
                 trials_to_pprox(clust_trials, params["sampling_rate"]),
+                schema=pprox._stimtrial_schema,
                 recording=resource_url,
                 processed_by=[f"{p.prog} {version}"],
                 kilosort_amplitude=clust_info["Amplitude"],
                 kilosort_contam_pct=clust_info["ContamPct"],
                 kilosort_source_channel=clust_info["ch"],
                 kilosort_probe_depth=clust_info["depth"],
                 kilosort_n_spikes=clust_info["n_spikes"],
                 entry_metadata=entry_attrs,
                 **resource_info["metadata"],
             )
             if not args.dry_run:
                 with open(outfile, "wt") as ofp:
                     json.dump(clust_trials, ofp, default=json_serializable)
-            if args.save_waveforms:
-                outfile = args.output / (outfile.stem + "_spikes.h5")
-                logging.info(
-                    "    - waveforms on channel %d -> %s",
-                    clust_info["ch"],
-                    outfile,
-                )
-                n_before = int(args.waveform_pre_peak * params["sampling_rate"] / 1000)
-                n_after = int(args.waveform_post_peak * params["sampling_rate"] / 1000)
-                spikes = events.loc[clust_id]
-                spikes = spikes[
-                    (spikes.time > n_before) & (spikes.time < (nsamples - n_after))
-                ]
-                waveforms = qs.peaks(
-                    recording[:, clust_info["ch"]],
-                    spikes.time,
-                    n_before,
-                    n_after,
-                )
-                if not args.dry_run:
+                if args.save_waveforms:
+                    outfile = args.output / (outfile.stem + "_spikes.h5")
+                    logging.info(
+                        "    - waveforms on channel %d -> %s",
+                        clust_info["ch"],
+                        outfile,
+                    )
                     save_waveforms(
                         outfile,
                         SpikeWaveforms(
-                            waveforms.T, spikes.time, params["sampling_rate"], n_before
+                            waveforms,
+                            cluster.time.to_numpy(),
+                            params["sampling_rate"],
+                            n_before,
                         ),
                         recording=resource_url,
                         processed_by=f"{p.prog} {version}",
                         kilosort_amplitude=clust_info["Amplitude"],
                         kilosort_contam_pct=clust_info["ContamPct"],
                         kilosort_source_channel=clust_info["ch"],
                         kilosort_probe_depth=clust_info["depth"],
```

### Comparing `melizalab-tools-2023.4.19/dlab/nbank.py` & `melizalab-tools-2023.5.3/dlab/nbank.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -31,21 +31,21 @@
     - a local cache
     - a remote HTTP archive (caching the file for local access later)
 
     It will raise a ValueError if the resource does not exist and a
     FileNotFoundError if the resource cannot be located.
 
     """
-    url, params = registry.get_locations(registry_url, resource_id)
     if alt_base is not None:
         stem = Path(alt_base) / resource_id
         path = await resolve_local_path(stem)
         if path is not None:
             logging.debug("%s: found in alt_base", resource_id)
             return path
+    url, params = registry.get_locations(registry_url, resource_id)
     response = await session.get(url, params=params)
     response.raise_for_status()
     locations = response.json()
     # search for local files
     for loc in locations:
         if loc["scheme"] not in registry._local_schemes:
             continue
```

### Comparing `melizalab-tools-2023.4.19/dlab/plotting.py` & `melizalab-tools-2023.5.3/dlab/plotting.py`

 * *Files identical despite different names*

### Comparing `melizalab-tools-2023.4.19/dlab/pprox.py` & `melizalab-tools-2023.5.3/dlab/pprox.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,26 +6,28 @@
 
 This package deliberately does not include any functions for serialization, as
 pprox objects are just python dictionaries.
 
 Copyright (C) Dan Meliza, 2006-2020 (dan@meliza.org)
 
 """
+from typing import Iterable, Dict
 
-_schema = "https://meliza.org/spec:2/pprox.json#"
+_base_schema = "https://meliza.org/spec:2/pprox.json#"
+_stimtrial_schema = "https://meliza.org/spec:2/stimtrial.json#"
 
 
 def empty():
     """Returns a new, empty pprox object"""
     return from_trials([])
 
 
-def from_trials(trials, **metadata):
+def from_trials(trials: Iterable, *, schema: str = _base_schema, **metadata) -> Dict:
     """Wrap a sequence of trials in a pprox object, optionally specifying top-level metadata"""
-    d = {"$schema": _schema, "pprox": tuple(trials)}
+    d = {"$schema": schema, "pprox": tuple(trials)}
     d.update(**metadata)
     return d
 
 
 def wrap_uuid(b):
     """Wrap a UUID (string or bytes) in a URN string"""
     import uuid
@@ -83,15 +85,15 @@
     """Combine events from multiple pprox objects into a single object, matching based on trial number"""
     pass
 
 
 async def split_trial(trial, split_fun):
     """Split a trial into multiple intervals.
 
-    split_fun: a function that takes the name of the stimulus and returns a
+    split_fun: a coroutine that takes the name of the stimulus and returns a
     list of dictionaries, one per split. Each dict needs to have at least three
     fields: `stim_begin`, the time when the split begins (relative to the start
     of the stimulus; `stim_end`, the time when the split ends; and `name`, the
     name that should be given to the split. Any additional fields will be stored
     as metadata on the new trials. Alternatively, `split_fun` can return a
     pandas dataframe. Make sure the metadata fields are valid Python identifiers.
```

### Comparing `melizalab-tools-2023.4.19/dlab/signal.py` & `melizalab-tools-2023.5.3/dlab/signal.py`

 * *Files identical despite different names*

### Comparing `melizalab-tools-2023.4.19/dlab/spikes.py` & `melizalab-tools-2023.5.3/dlab/spikes.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     counts, bins = psth(spikes, binwidth, start=start, stop=stop)
     return np.convolve(counts, kernel, mode="same"), bins
 
 
 @dataclass
 class SpikeWaveforms:
     """
-    waveform: ntimes x nspikes array (NB: the output of `quickspikes.peaks` needs to be transposed)
+    waveform: nspikes x npoints array
     times: nspikes array (times of spikes in units of samples)
     sampling_rate: the sampling rate of the spikes and the spike times (in Hz)
     peak_index: the index corresponding to the time of the spike in the waveform
     """
 
     waveforms: ArrayLike
     times: ArrayLike
@@ -84,15 +84,15 @@
     Waveforms should be stored as they were recorded. The `peak_index` argument
     will typically refer to the maximum negative deflection of the spike given
     typical recording parameters.
 
     """
     spikes = np.asarray(waveforms.waveforms)
     times = np.asarray(waveforms.times)
-    nspikes, ntimes = spikes.shape
+    ntimes, nspikes = spikes.shape
     if ntimes != times.size:
         raise ValueError(
             "number of rows in waveform array must match number of elements in times array"
         )
     with h5.File(path, "w") as fp:
         # unchunked storage uses the most space but allows random access
         dset_spikes = fp.create_dataset("waveforms", data=spikes)
```

### Comparing `melizalab-tools-2023.4.19/dlab/util.py` & `melizalab-tools-2023.5.3/dlab/util.py`

 * *Files identical despite different names*

### Comparing `melizalab-tools-2023.4.19/melizalab_tools.egg-info/PKG-INFO` & `melizalab-tools-2023.5.3/melizalab_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melizalab-tools
-Version: 2023.4.19
+Version: 2023.5.3
 Summary: Meliza lab scripts and modules for auditory neurophysiology
 Home-page: https://github.com/melizalab/melizalab-tools
 Author: Dan Meliza
 Author-email: dan@meliza.org
 Maintainer: Dan Meliza
 Maintainer-email: dan@meliza.org
 License: BSD 3-Clause License
```

### Comparing `melizalab-tools-2023.4.19/melizalab_tools.egg-info/SOURCES.txt` & `melizalab-tools-2023.5.3/melizalab_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `melizalab-tools-2023.4.19/setup.cfg` & `melizalab-tools-2023.5.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `melizalab-tools-2023.4.19/tests/test_pprox.py` & `melizalab-tools-2023.5.3/tests/test_pprox.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,15 +215,15 @@
     info = stims[name].copy()
     info["foreground"] = info["foreground"].split("-")
     return pd.DataFrame(info).rename(lambda s: s.replace("-", "_"), axis="columns")
 
 
 def test_make_pprox():
     pp = pprox.from_trials(trials, test_attribute="blank")
-    assert pp["$schema"] == pprox._schema
+    assert pp["$schema"] == pprox._base_schema
     assert pp["test_attribute"] == "blank"
     assert pp["pprox"] == trials
 
 
 def test_group_by_stim():
     pp = pprox.from_trials(trials)
     for stim, group in pprox.groupby(pp, lambda trial: trial["stimulus"]["name"]):
```

### Comparing `melizalab-tools-2023.4.19/tests/test_spikes.py` & `melizalab-tools-2023.5.3/tests/test_spikes.py`

 * *Files identical despite different names*

