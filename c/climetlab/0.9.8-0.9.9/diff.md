# Comparing `tmp/climetlab-0.9.8.tar.gz` & `tmp/climetlab-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climetlab-0.9.8.tar", last modified: Mon Dec 13 20:24:01 2021, max compression
+gzip compressed data, was "climetlab-0.9.9.tar", last modified: Wed Jan 12 20:42:01 2022, max compression
```

## Comparing `climetlab-0.9.8.tar` & `climetlab-0.9.9.tar`

### file list

```diff
@@ -1,227 +1,227 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.387686 climetlab-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11380 2021-12-13 20:23:45.000000 climetlab-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      251 2021-12-13 20:23:45.000000 climetlab-0.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2321 2021-12-13 20:24:01.387686 climetlab-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1244 2021-12-13 20:23:45.000000 climetlab-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.367690 climetlab-0.9.8/climetlab/
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.367690 climetlab-0.9.8/climetlab/arguments/
--rw-r--r--   0 runner    (1001) docker     (121)      576 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/arguments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2523 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/arguments/args_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2183 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/arguments/argument.py
--rw-r--r--   0 runner    (1001) docker     (121)    10113 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/arguments/climetlab_types.py
--rw-r--r--   0 runner    (1001) docker     (121)      625 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/arguments/guess.py
--rw-r--r--   0 runner    (1001) docker     (121)     4334 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/arguments/input_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     4433 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/arguments/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.367690 climetlab-0.9.8/climetlab/config/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/config/units.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.371689 climetlab-0.9.8/climetlab/core/
--rw-r--r--   0 runner    (1001) docker     (121)     2336 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21939 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/core/caching.py
--rw-r--r--   0 runner    (1001) docker     (121)     4753 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/core/data.py
--rw-r--r--   0 runner    (1001) docker     (121)      833 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/core/initialise.py
--rw-r--r--   0 runner    (1001) docker     (121)     3023 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/core/ipython.py
--rw-r--r--   0 runner    (1001) docker     (121)     3008 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/core/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     6152 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/core/plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)    11652 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     3199 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/core/statistics.py
--rw-r--r--   0 runner    (1001) docker     (121)     1503 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/core/temporary.py
--rw-r--r--   0 runner    (1001) docker     (121)     2708 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/core/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.359691 climetlab-0.9.8/climetlab/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.371689 climetlab-0.9.8/climetlab/data/css/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/css/table.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.371689 climetlab-0.9.8/climetlab/data/layers/
--rw-r--r--   0 runner    (1001) docker     (121)      268 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/layers/default-background.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      114 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/layers/default-foreground.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      127 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/layers/example-foreground.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      347 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/layers/land-sea.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.371689 climetlab-0.9.8/climetlab/data/projections/
--rw-r--r--   0 runner    (1001) docker     (121)      206 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/africa.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      204 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/asia.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       54 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/bonne.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/collignon.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      247 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/euro-atlantic.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      216 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/europe-cylindrical.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      260 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/europe.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      208 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/global.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       54 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/goode.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/mercator.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/mollweide.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      256 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/north-america.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      207 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/north-america1.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      246 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/north-atlantic.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      254 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/north-hemisphere.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      237 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/polar-north.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/robinson.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      206 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/south-america.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      204 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/south-atlantic.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      254 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/south-hemisphere.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      206 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/south-pacific.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      295 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/tapestry.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      205 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/tropics-east.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      206 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/tropics-west.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      289 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/projections/web-mercator.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.375688 climetlab-0.9.8/climetlab/data/styles/
--rw-r--r--   0 runner    (1001) docker     (121)      382 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/styles/cyclone-track.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       74 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/styles/default-style-fields.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      172 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/styles/default-style-observations.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      399 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/styles/land-sea-mask.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/styles/no-style.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1851 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/styles/orography.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      568 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/styles/rainbow-markers.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      314 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/data/styles/tapestry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.375688 climetlab-0.9.8/climetlab/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)     6554 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      595 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/datasets/era5_precipitations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1971 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/datasets/era5_single_levels.py
--rw-r--r--   0 runner    (1001) docker     (121)      589 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/datasets/era5_temperature.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/datasets/example-dataset.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5134 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/datasets/high_low.py
--rw-r--r--   0 runner    (1001) docker     (121)     4538 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/datasets/hurricane_database.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.375688 climetlab-0.9.8/climetlab/datasets/meteonet_samples/
--rw-r--r--   0 runner    (1001) docker     (121)      690 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/datasets/meteonet_samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      125 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/datasets/meteonet_samples/dataset.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1274 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/datasets/meteonet_samples/ground_stations.py
--rw-r--r--   0 runner    (1001) docker     (121)      789 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/datasets/meteonet_samples/masks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2716 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/datasets/meteonet_samples/radar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.375688 climetlab-0.9.8/climetlab/datasets/meteonet_samples/styles/
--rw-r--r--   0 runner    (1001) docker     (121)      729 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/datasets/meteonet_samples/styles/meteonet-radar-rainfall.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      995 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/datasets/meteonet_samples/weather_models.py
--rw-r--r--   0 runner    (1001) docker     (121)      180 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/datasets/sample-bufr-data.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      161 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/datasets/sample-grib-data.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2314 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/datasets/weather_bench.py
--rw-r--r--   0 runner    (1001) docker     (121)     4117 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.375688 climetlab-0.9.8/climetlab/indexing/
--rw-r--r--   0 runner    (1001) docker     (121)     4566 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/indexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      625 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/indexing/backends.py
--rw-r--r--   0 runner    (1001) docker     (121)     4837 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/indexing/database.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.375688 climetlab-0.9.8/climetlab/mergers/
--rw-r--r--   0 runner    (1001) docker     (121)     5350 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/mergers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      650 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/mergers/pandas.py
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/mergers/tfdataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/mergers/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.375688 climetlab-0.9.8/climetlab/metview/
--rw-r--r--   0 runner    (1001) docker     (121)      789 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/metview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2708 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/mockup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1320 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.375688 climetlab-0.9.8/climetlab/plotting/
--rw-r--r--   0 runner    (1001) docker     (121)     3904 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/plotting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.375688 climetlab-0.9.8/climetlab/plotting/backends/
--rw-r--r--   0 runner    (1001) docker     (121)      379 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/plotting/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.375688 climetlab-0.9.8/climetlab/plotting/backends/bokeh/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/plotting/backends/bokeh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      514 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/plotting/backends/bokeh/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.375688 climetlab-0.9.8/climetlab/plotting/backends/magics/
--rw-r--r--   0 runner    (1001) docker     (121)     1348 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/plotting/backends/magics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3093 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/plotting/backends/magics/actions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5258 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/plotting/backends/magics/apply.py
--rw-r--r--   0 runner    (1001) docker     (121)    14648 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/plotting/backends/magics/backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     4832 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/plotting/backends/magics/colour.py
--rw-r--r--   0 runner    (1001) docker     (121)     2024 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/plotting/backends/magics/convertions.py
--rw-r--r--   0 runner    (1001) docker     (121)    47675 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/plotting/backends/magics/magics.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.379687 climetlab-0.9.8/climetlab/plotting/backends/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/plotting/backends/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1700 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/plotting/backends/matplotlib/backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     1495 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/plotting/options.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.379687 climetlab-0.9.8/climetlab/plotting/wms/
--rw-r--r--   0 runner    (1001) docker     (121)      475 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/plotting/wms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4379 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/plotting/wms/_folium.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/plotting/wms/_ipyleafet.py
--rw-r--r--   0 runner    (1001) docker     (121)     2581 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.379687 climetlab-0.9.8/climetlab/readers/
--rw-r--r--   0 runner    (1001) docker     (121)     4172 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2073 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/readers/archive.py
--rw-r--r--   0 runner    (1001) docker     (121)      836 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/readers/bufr.py
--rw-r--r--   0 runner    (1001) docker     (121)     5918 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/readers/csv.py
--rw-r--r--   0 runner    (1001) docker     (121)     2538 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/readers/directory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/readers/fwf.py
--rw-r--r--   0 runner    (1001) docker     (121)    15633 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/readers/grib.py
--rw-r--r--   0 runner    (1001) docker     (121)    10192 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/readers/netcdf.py
--rw-r--r--   0 runner    (1001) docker     (121)      998 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/readers/numpy.py
--rw-r--r--   0 runner    (1001) docker     (121)      968 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/readers/odb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/readers/tar.py
--rw-r--r--   0 runner    (1001) docker     (121)     1379 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/readers/text.py
--rw-r--r--   0 runner    (1001) docker     (121)     1569 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/readers/tfrecord.py
--rw-r--r--   0 runner    (1001) docker     (121)      774 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/readers/unknown.py
--rw-r--r--   0 runner    (1001) docker     (121)     2635 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/readers/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.379687 climetlab-0.9.8/climetlab/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      442 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      901 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/scripts/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.379687 climetlab-0.9.8/climetlab/scripts/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/scripts/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6992 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/scripts/benchmarks/indexed_url.py
--rw-r--r--   0 runner    (1001) docker     (121)     9137 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/scripts/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     9079 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/scripts/check.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3592 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/scripts/grib.py
--rw-r--r--   0 runner    (1001) docker     (121)     2930 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     1496 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/scripts/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1590 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/scripts/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.383686 climetlab-0.9.8/climetlab/sources/
--rw-r--r--   0 runner    (1001) docker     (121)     3912 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3974 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sources/cds.py
--rw-r--r--   0 runner    (1001) docker     (121)      378 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sources/dummy.grib
--rw-r--r--   0 runner    (1001) docker     (121)     6149 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sources/dummy_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     2386 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sources/ecmwf_open_data.py
--rw-r--r--   0 runner    (1001) docker     (121)      567 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sources/empty.py
--rw-r--r--   0 runner    (1001) docker     (121)     4598 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sources/file.py
--rw-r--r--   0 runner    (1001) docker     (121)      897 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sources/file_pattern.py
--rw-r--r--   0 runner    (1001) docker     (121)     1452 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sources/indexed_urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     3632 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sources/mars.py
--rw-r--r--   0 runner    (1001) docker     (121)     4360 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sources/multi.py
--rw-r--r--   0 runner    (1001) docker     (121)     1151 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sources/multi_url.py
--rw-r--r--   0 runner    (1001) docker     (121)      618 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sources/opendap.py
--rw-r--r--   0 runner    (1001) docker     (121)     4808 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sources/prompt.py
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sources/sentinel_hub.py
--rw-r--r--   0 runner    (1001) docker     (121)     3569 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sources/url.py
--rw-r--r--   0 runner    (1001) docker     (121)      788 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sources/url_pattern.py
--rw-r--r--   0 runner    (1001) docker     (121)     3222 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sources/zarr.py
--rw-r--r--   0 runner    (1001) docker     (121)     2909 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sources/zarr_s3.py
--rw-r--r--   0 runner    (1001) docker     (121)     1795 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sources/zenodo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.383686 climetlab-0.9.8/climetlab/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (121)      379 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sphinxext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1667 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sphinxext/command_output.py
--rw-r--r--   0 runner    (1001) docker     (121)      847 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sphinxext/file_content.py
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sphinxext/generate_cmdline_help.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3579 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sphinxext/generate_gallery_rst.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1603 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sphinxext/generate_settings_rst.py
--rw-r--r--   0 runner    (1001) docker     (121)     1812 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/sphinxext/module_output.py
--rw-r--r--   0 runner    (1001) docker     (121)     3124 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.383686 climetlab-0.9.8/climetlab/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     4003 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4955 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/utils/availability.py
--rw-r--r--   0 runner    (1001) docker     (121)     5280 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/utils/bbox.py
--rw-r--r--   0 runner    (1001) docker     (121)      697 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/utils/conventions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2667 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (121)     2328 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/utils/domains.py
--rw-r--r--   0 runner    (1001) docker     (121)    19720 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/utils/factorise.py
--rw-r--r--   0 runner    (1001) docker     (121)     1272 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (121)     7159 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/utils/humanize.py
--rw-r--r--   0 runner    (1001) docker     (121)     1738 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/utils/lazy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/utils/mirror.py
--rw-r--r--   0 runner    (1001) docker     (121)     4770 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/utils/patterns.py
--rw-r--r--   0 runner    (1001) docker     (121)     1584 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/utils/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/version
--rw-r--r--   0 runner    (1001) docker     (121)      664 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.383686 climetlab-0.9.8/climetlab/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (121)     2873 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/vocabularies/aliases.py
--rw-r--r--   0 runner    (1001) docker     (121)      885 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/vocabularies/cf.py
--rw-r--r--   0 runner    (1001) docker     (121)      742 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/vocabularies/grib.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.387686 climetlab-0.9.8/climetlab/wrappers/
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1056 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/wrappers/integer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/wrappers/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (121)      695 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/wrappers/none.py
--rw-r--r--   0 runner    (1001) docker     (121)     2632 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/wrappers/pandas.py
--rw-r--r--   0 runner    (1001) docker     (121)     1802 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/wrappers/string.py
--rw-r--r--   0 runner    (1001) docker     (121)     4873 2021-12-13 20:23:45.000000 climetlab-0.9.8/climetlab/wrappers/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:24:01.367690 climetlab-0.9.8/climetlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2321 2021-12-13 20:24:00.000000 climetlab-0.9.8/climetlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6618 2021-12-13 20:24:01.000000 climetlab-0.9.8/climetlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-13 20:24:00.000000 climetlab-0.9.8/climetlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2021-12-13 20:24:00.000000 climetlab-0.9.8/climetlab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      647 2021-12-13 20:24:00.000000 climetlab-0.9.8/climetlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-12-13 20:24:01.000000 climetlab-0.9.8/climetlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-13 20:24:00.000000 climetlab-0.9.8/climetlab.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-13 20:24:01.387686 climetlab-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3312 2021-12-13 20:23:46.000000 climetlab-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.162478 climetlab-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11380 2022-01-12 20:41:50.000000 climetlab-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2022-01-12 20:41:50.000000 climetlab-0.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2321 2022-01-12 20:42:01.162478 climetlab-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-01-12 20:41:50.000000 climetlab-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.142478 climetlab-0.9.9/climetlab/
+-rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.142478 climetlab-0.9.9/climetlab/arguments/
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/arguments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2523 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/arguments/args_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2183 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/arguments/argument.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10113 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/arguments/climetlab_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)      625 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/arguments/guess.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4334 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/arguments/input_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4433 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/arguments/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.142478 climetlab-0.9.9/climetlab/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      233 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/config/units.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.146478 climetlab-0.9.9/climetlab/core/
+-rw-r--r--   0 runner    (1001) docker     (121)     2336 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21939 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/core/caching.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4753 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)      833 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/core/initialise.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3023 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/core/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3008 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/core/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6152 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/core/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11666 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3199 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/core/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1503 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/core/temporary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2708 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/core/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.138478 climetlab-0.9.9/climetlab/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.146478 climetlab-0.9.9/climetlab/data/css/
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/css/table.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.146478 climetlab-0.9.9/climetlab/data/layers/
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/layers/default-background.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/layers/default-foreground.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/layers/example-foreground.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/layers/land-sea.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.146478 climetlab-0.9.9/climetlab/data/projections/
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/africa.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/asia.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/bonne.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/collignon.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      247 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/euro-atlantic.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/europe-cylindrical.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/europe.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/global.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/goode.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/mercator.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/mollweide.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/north-america.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/north-america1.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/north-atlantic.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/north-hemisphere.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      237 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/polar-north.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/robinson.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/south-america.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/south-atlantic.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/south-hemisphere.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/south-pacific.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      295 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/tapestry.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      205 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/tropics-east.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/tropics-west.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      289 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/projections/web-mercator.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.150478 climetlab-0.9.9/climetlab/data/styles/
+-rw-r--r--   0 runner    (1001) docker     (121)      382 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/styles/cyclone-track.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/styles/default-style-fields.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      172 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/styles/default-style-observations.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/styles/land-sea-mask.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/styles/no-style.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1851 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/styles/orography.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/styles/rainbow-markers.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      314 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/data/styles/tapestry.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.150478 climetlab-0.9.9/climetlab/datasets/
+-rw-r--r--   0 runner    (1001) docker     (121)     6554 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      595 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/datasets/era5_precipitations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1971 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/datasets/era5_single_levels.py
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/datasets/era5_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/datasets/example-dataset.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     5134 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/datasets/high_low.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4538 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/datasets/hurricane_database.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.150478 climetlab-0.9.9/climetlab/datasets/meteonet_samples/
+-rw-r--r--   0 runner    (1001) docker     (121)      690 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/datasets/meteonet_samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/datasets/meteonet_samples/dataset.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1274 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/datasets/meteonet_samples/ground_stations.py
+-rw-r--r--   0 runner    (1001) docker     (121)      789 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/datasets/meteonet_samples/masks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2716 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/datasets/meteonet_samples/radar.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.150478 climetlab-0.9.9/climetlab/datasets/meteonet_samples/styles/
+-rw-r--r--   0 runner    (1001) docker     (121)      729 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/datasets/meteonet_samples/styles/meteonet-radar-rainfall.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      995 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/datasets/meteonet_samples/weather_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/datasets/sample-bufr-data.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/datasets/sample-grib-data.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2314 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/datasets/weather_bench.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4117 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.150478 climetlab-0.9.9/climetlab/indexing/
+-rw-r--r--   0 runner    (1001) docker     (121)     4566 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/indexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      625 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/indexing/backends.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4837 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/indexing/database.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.150478 climetlab-0.9.9/climetlab/mergers/
+-rw-r--r--   0 runner    (1001) docker     (121)     5350 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/mergers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      650 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/mergers/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/mergers/tfdataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/mergers/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.150478 climetlab-0.9.9/climetlab/metview/
+-rw-r--r--   0 runner    (1001) docker     (121)      789 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/metview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2708 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/mockup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.150478 climetlab-0.9.9/climetlab/plotting/
+-rw-r--r--   0 runner    (1001) docker     (121)     3904 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/plotting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.150478 climetlab-0.9.9/climetlab/plotting/backends/
+-rw-r--r--   0 runner    (1001) docker     (121)      379 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/plotting/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.150478 climetlab-0.9.9/climetlab/plotting/backends/bokeh/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/plotting/backends/bokeh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      514 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/plotting/backends/bokeh/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.150478 climetlab-0.9.9/climetlab/plotting/backends/magics/
+-rw-r--r--   0 runner    (1001) docker     (121)     1348 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/plotting/backends/magics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3093 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/plotting/backends/magics/actions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5258 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/plotting/backends/magics/apply.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14648 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/plotting/backends/magics/backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4832 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/plotting/backends/magics/colour.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2024 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/plotting/backends/magics/convertions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    47675 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/plotting/backends/magics/magics.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.150478 climetlab-0.9.9/climetlab/plotting/backends/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/plotting/backends/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/plotting/backends/matplotlib/backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1495 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/plotting/options.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.154478 climetlab-0.9.9/climetlab/plotting/wms/
+-rw-r--r--   0 runner    (1001) docker     (121)      475 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/plotting/wms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4379 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/plotting/wms/_folium.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/plotting/wms/_ipyleafet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2581 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.154478 climetlab-0.9.9/climetlab/readers/
+-rw-r--r--   0 runner    (1001) docker     (121)     4172 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2073 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/readers/archive.py
+-rw-r--r--   0 runner    (1001) docker     (121)      836 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/readers/bufr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5918 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/readers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2538 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/readers/directory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/readers/fwf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15633 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/readers/grib.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10192 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/readers/netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      998 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/readers/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      968 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/readers/odb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/readers/tar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1379 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/readers/text.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1569 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/readers/tfrecord.py
+-rw-r--r--   0 runner    (1001) docker     (121)      774 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/readers/unknown.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2635 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/readers/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.154478 climetlab-0.9.9/climetlab/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      901 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/scripts/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.154478 climetlab-0.9.9/climetlab/scripts/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/scripts/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6992 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/scripts/benchmarks/indexed_url.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9137 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/scripts/cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9079 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/scripts/check.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3592 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/scripts/grib.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3246 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1496 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/scripts/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/scripts/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.154478 climetlab-0.9.9/climetlab/sources/
+-rw-r--r--   0 runner    (1001) docker     (121)     3912 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3974 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sources/cds.py
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sources/dummy.grib
+-rw-r--r--   0 runner    (1001) docker     (121)     6149 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sources/dummy_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2386 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sources/ecmwf_open_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)      567 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sources/empty.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4598 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sources/file.py
+-rw-r--r--   0 runner    (1001) docker     (121)      897 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sources/file_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1452 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sources/indexed_urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3632 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sources/mars.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4360 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sources/multi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sources/multi_url.py
+-rw-r--r--   0 runner    (1001) docker     (121)      618 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sources/opendap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4808 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sources/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sources/sentinel_hub.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3569 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sources/url.py
+-rw-r--r--   0 runner    (1001) docker     (121)      788 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sources/url_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3222 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sources/zarr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2909 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sources/zarr_s3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1795 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sources/zenodo.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.158478 climetlab-0.9.9/climetlab/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (121)      379 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sphinxext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1667 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sphinxext/command_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)      847 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sphinxext/file_content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sphinxext/generate_cmdline_help.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3579 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sphinxext/generate_gallery_rst.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1603 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sphinxext/generate_settings_rst.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1812 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/sphinxext/module_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3124 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.158478 climetlab-0.9.9/climetlab/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     4003 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4955 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/utils/availability.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5280 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/utils/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (121)      697 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/utils/conventions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2667 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2328 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/utils/domains.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19720 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/utils/factorise.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1272 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7159 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/utils/humanize.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/utils/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/utils/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4770 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/utils/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1584 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/utils/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/version
+-rw-r--r--   0 runner    (1001) docker     (121)      664 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.158478 climetlab-0.9.9/climetlab/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (121)     2873 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/vocabularies/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (121)      885 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/vocabularies/cf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      742 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/vocabularies/grib.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.162478 climetlab-0.9.9/climetlab/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/wrappers/integer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/wrappers/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (121)      695 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/wrappers/none.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2632 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/wrappers/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1802 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/wrappers/string.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4873 2022-01-12 20:41:50.000000 climetlab-0.9.9/climetlab/wrappers/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 20:42:01.142478 climetlab-0.9.9/climetlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2321 2022-01-12 20:42:00.000000 climetlab-0.9.9/climetlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6618 2022-01-12 20:42:01.000000 climetlab-0.9.9/climetlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-12 20:42:00.000000 climetlab-0.9.9/climetlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-01-12 20:42:00.000000 climetlab-0.9.9/climetlab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      631 2022-01-12 20:42:00.000000 climetlab-0.9.9/climetlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-01-12 20:42:00.000000 climetlab-0.9.9/climetlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-12 20:42:00.000000 climetlab-0.9.9/climetlab.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-12 20:42:01.162478 climetlab-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3304 2022-01-12 20:41:50.000000 climetlab-0.9.9/setup.py
```

### Comparing `climetlab-0.9.8/LICENSE` & `climetlab-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/PKG-INFO` & `climetlab-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climetlab
-Version: 0.9.8
+Version: 0.9.9
 Summary: Handling of climate/meteorological data
 Home-page: https://github.com/ecmwf/climetlab
 Author: ECMWF
 Author-email: software.support@ecmwf.int
 License: Apache 2.0
 Description: # CliMetLab
```

### Comparing `climetlab-0.9.8/README.md` & `climetlab-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/__init__.py` & `climetlab-0.9.9/climetlab/__init__.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/arguments/__init__.py` & `climetlab-0.9.9/climetlab/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/arguments/args_kwargs.py` & `climetlab-0.9.9/climetlab/arguments/args_kwargs.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/arguments/argument.py` & `climetlab-0.9.9/climetlab/arguments/argument.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/arguments/climetlab_types.py` & `climetlab-0.9.9/climetlab/arguments/climetlab_types.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/arguments/guess.py` & `climetlab-0.9.9/climetlab/arguments/guess.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/arguments/input_manager.py` & `climetlab-0.9.9/climetlab/arguments/input_manager.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/arguments/transformers.py` & `climetlab-0.9.9/climetlab/arguments/transformers.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/core/__init__.py` & `climetlab-0.9.9/climetlab/core/__init__.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/core/caching.py` & `climetlab-0.9.9/climetlab/core/caching.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/core/data.py` & `climetlab-0.9.9/climetlab/core/data.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/core/initialise.py` & `climetlab-0.9.9/climetlab/core/initialise.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/core/ipython.py` & `climetlab-0.9.9/climetlab/core/ipython.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/core/metadata.py` & `climetlab-0.9.9/climetlab/core/metadata.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/core/plugins.py` & `climetlab-0.9.9/climetlab/core/plugins.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/core/settings.py` & `climetlab-0.9.9/climetlab/core/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 _ = Settings
 
 
 SETTINGS_AND_HELP = {
     "cache-directory": _(
         os.path.join(tempfile.gettempdir(), "climetlab-%s" % (getpass.getuser(),)),
         """Directory of where the dowloaded files are cached, with ``${USER}`` is the user id.
-        See :ref:`caching` for more information.""",
+        See :doc:`/guide/caching` for more information.""",
     ),
     "styles-directories": _(
         [os.path.join(DOT_CLIMETLAB, "styles")],
         """List of directories where to search for styles definitions.
         See :ref:`styles` for more information.""",
     ),
     "projections-directories": _(
@@ -107,15 +107,15 @@
         """Maximum disk space used by the CliMetLab cache (ex: 100G or 2T).""",
         getter="_as_bytes",
         none_ok=True,
     ),
     "maximum-cache-disk-usage": _(
         "90%",
         """Disk usage threshold after which CliMetLab expires older cached entries (% of the full disk capacity).
-        See :ref:`caching` for more information.""",
+        See :doc:`/guide/caching` for more information.""",
         getter="_as_percent",
     ),
     "url-download-timeout": _(
         "30s",
         """Timeout when downloading from an url.""",
         getter="_as_seconds",
     ),
```

### Comparing `climetlab-0.9.8/climetlab/core/statistics.py` & `climetlab-0.9.9/climetlab/core/statistics.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/core/temporary.py` & `climetlab-0.9.9/climetlab/core/temporary.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/core/thread.py` & `climetlab-0.9.9/climetlab/core/thread.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/data/styles/orography.yaml` & `climetlab-0.9.9/climetlab/data/styles/orography.yaml`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/data/styles/rainbow-markers.yaml` & `climetlab-0.9.9/climetlab/data/styles/rainbow-markers.yaml`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/datasets/__init__.py` & `climetlab-0.9.9/climetlab/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/datasets/era5_precipitations.py` & `climetlab-0.9.9/climetlab/datasets/era5_precipitations.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/datasets/era5_single_levels.py` & `climetlab-0.9.9/climetlab/datasets/era5_single_levels.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/datasets/era5_temperature.py` & `climetlab-0.9.9/climetlab/datasets/era5_temperature.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/datasets/high_low.py` & `climetlab-0.9.9/climetlab/datasets/high_low.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/datasets/hurricane_database.py` & `climetlab-0.9.9/climetlab/datasets/hurricane_database.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/datasets/meteonet_samples/__init__.py` & `climetlab-0.9.9/climetlab/datasets/meteonet_samples/__init__.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/datasets/meteonet_samples/ground_stations.py` & `climetlab-0.9.9/climetlab/datasets/meteonet_samples/ground_stations.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/datasets/meteonet_samples/masks.py` & `climetlab-0.9.9/climetlab/datasets/meteonet_samples/masks.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/datasets/meteonet_samples/radar.py` & `climetlab-0.9.9/climetlab/datasets/meteonet_samples/radar.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/datasets/meteonet_samples/styles/meteonet-radar-rainfall.yaml` & `climetlab-0.9.9/climetlab/datasets/meteonet_samples/styles/meteonet-radar-rainfall.yaml`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/datasets/meteonet_samples/weather_models.py` & `climetlab-0.9.9/climetlab/datasets/meteonet_samples/weather_models.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/datasets/weather_bench.py` & `climetlab-0.9.9/climetlab/datasets/weather_bench.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/decorators.py` & `climetlab-0.9.9/climetlab/decorators.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/indexing/__init__.py` & `climetlab-0.9.9/climetlab/indexing/__init__.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/indexing/backends.py` & `climetlab-0.9.9/climetlab/indexing/backends.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/indexing/database.py` & `climetlab-0.9.9/climetlab/indexing/database.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/mergers/__init__.py` & `climetlab-0.9.9/climetlab/mergers/__init__.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/mergers/pandas.py` & `climetlab-0.9.9/climetlab/mergers/pandas.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/mergers/tfdataset.py` & `climetlab-0.9.9/climetlab/mergers/tfdataset.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/mergers/xarray.py` & `climetlab-0.9.9/climetlab/mergers/xarray.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/metview/__init__.py` & `climetlab-0.9.9/climetlab/metview/__init__.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/mockup.py` & `climetlab-0.9.9/climetlab/mockup.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/normalize.py` & `climetlab-0.9.9/climetlab/normalize.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/plotting/__init__.py` & `climetlab-0.9.9/climetlab/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/plotting/backends/bokeh/backend.py` & `climetlab-0.9.9/climetlab/plotting/backends/bokeh/backend.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/plotting/backends/magics/__init__.py` & `climetlab-0.9.9/climetlab/plotting/backends/magics/__init__.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/plotting/backends/magics/actions.py` & `climetlab-0.9.9/climetlab/plotting/backends/magics/actions.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/plotting/backends/magics/apply.py` & `climetlab-0.9.9/climetlab/plotting/backends/magics/apply.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/plotting/backends/magics/backend.py` & `climetlab-0.9.9/climetlab/plotting/backends/magics/backend.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/plotting/backends/magics/colour.py` & `climetlab-0.9.9/climetlab/plotting/backends/magics/colour.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/plotting/backends/magics/convertions.py` & `climetlab-0.9.9/climetlab/plotting/backends/magics/convertions.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/plotting/backends/magics/magics.yaml` & `climetlab-0.9.9/climetlab/plotting/backends/magics/magics.yaml`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/plotting/backends/matplotlib/backend.py` & `climetlab-0.9.9/climetlab/plotting/backends/matplotlib/backend.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/plotting/options.py` & `climetlab-0.9.9/climetlab/plotting/options.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/plotting/wms/_folium.py` & `climetlab-0.9.9/climetlab/plotting/wms/_folium.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/profiling.py` & `climetlab-0.9.9/climetlab/profiling.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/readers/__init__.py` & `climetlab-0.9.9/climetlab/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/readers/archive.py` & `climetlab-0.9.9/climetlab/readers/archive.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/readers/bufr.py` & `climetlab-0.9.9/climetlab/readers/bufr.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/readers/csv.py` & `climetlab-0.9.9/climetlab/readers/csv.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/readers/directory.py` & `climetlab-0.9.9/climetlab/readers/directory.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/readers/fwf.py` & `climetlab-0.9.9/climetlab/readers/fwf.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/readers/grib.py` & `climetlab-0.9.9/climetlab/readers/grib.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/readers/netcdf.py` & `climetlab-0.9.9/climetlab/readers/netcdf.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/readers/numpy.py` & `climetlab-0.9.9/climetlab/readers/numpy.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/readers/odb.py` & `climetlab-0.9.9/climetlab/readers/odb.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/readers/tar.py` & `climetlab-0.9.9/climetlab/readers/tar.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/readers/text.py` & `climetlab-0.9.9/climetlab/readers/text.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/readers/tfrecord.py` & `climetlab-0.9.9/climetlab/readers/tfrecord.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/readers/unknown.py` & `climetlab-0.9.9/climetlab/readers/unknown.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/readers/zip.py` & `climetlab-0.9.9/climetlab/readers/zip.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/scripts/benchmark.py` & `climetlab-0.9.9/climetlab/scripts/benchmark.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/scripts/benchmarks/indexed_url.py` & `climetlab-0.9.9/climetlab/scripts/benchmarks/indexed_url.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/scripts/cache.py` & `climetlab-0.9.9/climetlab/scripts/cache.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/scripts/check.py` & `climetlab-0.9.9/climetlab/scripts/check.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/scripts/grib.py` & `climetlab-0.9.9/climetlab/scripts/grib.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/scripts/main.py` & `climetlab-0.9.9/climetlab/scripts/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 
 import argparse
 import cmd
 import logging
 import os
 import sys
 import traceback
+from importlib import import_module
 
+import entrypoints
 from termcolor import colored
 
 from .benchmark import BenchmarkCmd
 from .cache import CacheCmd
 from .check import CheckCmd
 from .grib import GribCmd
 from .settings import SettingsCmd
@@ -33,21 +35,31 @@
         def write_history_file(*args, **kwargs):
             pass
 
         def read_history_file(*args, **kwargs):
             pass
 
 
+def get_plugins():
+    plugins = []
+    for e in entrypoints.get_group_all("climetlab.scripts"):
+        module = import_module(e.module_name)
+        klass = getattr(module, e.object_name)
+        plugins.append(klass)
+    return plugins
+
+
 class CliMetLabApp(
     cmd.Cmd,
     SettingsCmd,
     CacheCmd,
     CheckCmd,
     GribCmd,
     BenchmarkCmd,
+    *get_plugins(),
 ):
     # intro = 'Welcome to climetlab. Type ? to list commands.\n'
     prompt = colored("(climetlab) ", "yellow")
 
     rc_file = "~/.climetlab-history"
 
     def postloop(self):
```

### Comparing `climetlab-0.9.8/climetlab/scripts/settings.py` & `climetlab-0.9.9/climetlab/scripts/settings.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/scripts/tools.py` & `climetlab-0.9.9/climetlab/scripts/tools.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sources/__init__.py` & `climetlab-0.9.9/climetlab/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sources/cds.py` & `climetlab-0.9.9/climetlab/sources/cds.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sources/dummy_source.py` & `climetlab-0.9.9/climetlab/sources/dummy_source.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sources/ecmwf_open_data.py` & `climetlab-0.9.9/climetlab/sources/ecmwf_open_data.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sources/empty.py` & `climetlab-0.9.9/climetlab/sources/empty.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sources/file.py` & `climetlab-0.9.9/climetlab/sources/file.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sources/file_pattern.py` & `climetlab-0.9.9/climetlab/sources/file_pattern.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sources/indexed_urls.py` & `climetlab-0.9.9/climetlab/sources/indexed_urls.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sources/mars.py` & `climetlab-0.9.9/climetlab/sources/mars.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sources/multi.py` & `climetlab-0.9.9/climetlab/sources/multi.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sources/multi_url.py` & `climetlab-0.9.9/climetlab/sources/multi_url.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sources/opendap.py` & `climetlab-0.9.9/climetlab/sources/opendap.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sources/prompt.py` & `climetlab-0.9.9/climetlab/sources/prompt.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sources/sentinel_hub.py` & `climetlab-0.9.9/climetlab/sources/sentinel_hub.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sources/url.py` & `climetlab-0.9.9/climetlab/sources/url.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sources/url_pattern.py` & `climetlab-0.9.9/climetlab/sources/url_pattern.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sources/zarr.py` & `climetlab-0.9.9/climetlab/sources/zarr.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sources/zarr_s3.py` & `climetlab-0.9.9/climetlab/sources/zarr_s3.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sources/zenodo.py` & `climetlab-0.9.9/climetlab/sources/zenodo.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sphinxext/command_output.py` & `climetlab-0.9.9/climetlab/sphinxext/command_output.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sphinxext/file_content.py` & `climetlab-0.9.9/climetlab/sphinxext/file_content.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sphinxext/generate_cmdline_help.py` & `climetlab-0.9.9/climetlab/sphinxext/generate_cmdline_help.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sphinxext/generate_gallery_rst.py` & `climetlab-0.9.9/climetlab/sphinxext/generate_gallery_rst.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sphinxext/generate_settings_rst.py` & `climetlab-0.9.9/climetlab/sphinxext/generate_settings_rst.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/sphinxext/module_output.py` & `climetlab-0.9.9/climetlab/sphinxext/module_output.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/testing.py` & `climetlab-0.9.9/climetlab/testing.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/utils/__init__.py` & `climetlab-0.9.9/climetlab/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/utils/availability.py` & `climetlab-0.9.9/climetlab/utils/availability.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/utils/bbox.py` & `climetlab-0.9.9/climetlab/utils/bbox.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/utils/conventions.py` & `climetlab-0.9.9/climetlab/utils/conventions.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/utils/dates.py` & `climetlab-0.9.9/climetlab/utils/dates.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/utils/domains.py` & `climetlab-0.9.9/climetlab/utils/domains.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/utils/factorise.py` & `climetlab-0.9.9/climetlab/utils/factorise.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/utils/html.py` & `climetlab-0.9.9/climetlab/utils/html.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/utils/humanize.py` & `climetlab-0.9.9/climetlab/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/utils/lazy.py` & `climetlab-0.9.9/climetlab/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/utils/mirror.py` & `climetlab-0.9.9/climetlab/utils/mirror.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/utils/patterns.py` & `climetlab-0.9.9/climetlab/utils/patterns.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/utils/tensorflow.py` & `climetlab-0.9.9/climetlab/utils/tensorflow.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/version.py` & `climetlab-0.9.9/climetlab/version.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/vocabularies/__init__.py` & `climetlab-0.9.9/climetlab/vocabularies/__init__.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/vocabularies/aliases.py` & `climetlab-0.9.9/climetlab/vocabularies/aliases.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/vocabularies/cf.py` & `climetlab-0.9.9/climetlab/vocabularies/cf.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/vocabularies/grib.py` & `climetlab-0.9.9/climetlab/vocabularies/grib.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/wrappers/__init__.py` & `climetlab-0.9.9/climetlab/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/wrappers/integer.py` & `climetlab-0.9.9/climetlab/wrappers/integer.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/wrappers/ndarray.py` & `climetlab-0.9.9/climetlab/wrappers/ndarray.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/wrappers/none.py` & `climetlab-0.9.9/climetlab/wrappers/none.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/wrappers/pandas.py` & `climetlab-0.9.9/climetlab/wrappers/pandas.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/wrappers/string.py` & `climetlab-0.9.9/climetlab/wrappers/string.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab/wrappers/xarray.py` & `climetlab-0.9.9/climetlab/wrappers/xarray.py`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab.egg-info/PKG-INFO` & `climetlab-0.9.9/climetlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climetlab
-Version: 0.9.8
+Version: 0.9.9
 Summary: Handling of climate/meteorological data
 Home-page: https://github.com/ecmwf/climetlab
 Author: ECMWF
 Author-email: software.support@ecmwf.int
 License: Apache 2.0
 Description: # CliMetLab
```

### Comparing `climetlab-0.9.8/climetlab.egg-info/SOURCES.txt` & `climetlab-0.9.9/climetlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `climetlab-0.9.8/climetlab.egg-info/requires.txt` & `climetlab-0.9.9/climetlab.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 cfgrib>=0.9.8.4
 cdsapi
 ecmwf-api-client>=1.6.1
 multiurl>=0.0.8
 tqdm
 eccodes>=1.3.0
 magics>=1.5.6
-ecmwflibs==0.3.14
+ecmwflibs
 pdbufr
 pyodc
 toolz
 filelock
 pyyaml
 markdown
 termcolor
@@ -38,15 +38,15 @@
 cfgrib>=0.9.8.4
 cdsapi
 ecmwf-api-client>=1.6.1
 multiurl>=0.0.8
 tqdm
 eccodes>=1.3.0
 magics>=1.5.6
-ecmwflibs==0.3.14
+ecmwflibs
 pdbufr
 pyodc
 toolz
 filelock
 pyyaml
 markdown
 termcolor
```

### Comparing `climetlab-0.9.8/setup.py` & `climetlab-0.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     "cfgrib>=0.9.8.4",
     "cdsapi",
     "ecmwf-api-client>=1.6.1",
     "multiurl>=0.0.8",
     "tqdm",
     "eccodes>=1.3.0",
     "magics>=1.5.6",
-    "ecmwflibs==0.3.14",
+    "ecmwflibs",
     "pdbufr",
     "pyodc",
     "toolz",
     "filelock",
     "pyyaml",
     "markdown",
     "termcolor",
```

