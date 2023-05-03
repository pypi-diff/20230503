# Comparing `tmp/vivarium-1.0.4.tar.gz` & `tmp/vivarium-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vivarium-1.0.4.tar", last modified: Wed Jan 25 22:00:47 2023, max compression
+gzip compressed data, was "vivarium-1.1.0.tar", last modified: Wed May  3 21:39:46 2023, max compression
```

## Comparing `vivarium-1.0.4.tar` & `vivarium-1.1.0.tar`

### file list

```diff
@@ -1,240 +1,246 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.414388 vivarium-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-01-25 22:00:38.000000 vivarium-1.0.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-01-25 22:00:38.000000 vivarium-1.0.4/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-01-25 22:00:38.000000 vivarium-1.0.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-01-25 22:00:38.000000 vivarium-1.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-01-25 22:00:38.000000 vivarium-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-01-25 22:00:47.414388 vivarium-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-01-25 22:00:38.000000 vivarium-1.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.386388 vivarium-1.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/nitpick-exceptions
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.386388 vivarium-1.0.4/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.386388 vivarium-1.0.4/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.386388 vivarium-1.0.4/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.386388 vivarium-1.0.4/docs/source/api_reference/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/config_tree.rst
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/exceptions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.390388 vivarium-1.0.4/docs/source/api_reference/framework/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.390388 vivarium-1.0.4/docs/source/api_reference/framework/artifact/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/artifact/artifact.rst
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/artifact/hdf.rst
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/artifact/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/artifact/manager.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.390388 vivarium-1.0.4/docs/source/api_reference/framework/components/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/components/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/components/manager.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/components/parser.rst
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/engine.rst
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/event.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/lifecycle.rst
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/lookup.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/metrics.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/plugins.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.390388 vivarium-1.0.4/docs/source/api_reference/framework/population/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/population/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/population/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/population/manager.rst
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/population/population_view.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.394388 vivarium-1.0.4/docs/source/api_reference/framework/randomness/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/randomness/core.rst
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/randomness/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/randomness/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/randomness/index_map.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/randomness/manager.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/randomness/stream.rst
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/resource.rst
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/state_machine.rst
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/time.rst
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/framework/values.rst
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.394388 vivarium-1.0.4/docs/source/api_reference/interface/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/interface/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/interface/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/interface/interactive.rst
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/interface/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/interpolation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/api_reference/testing_utilities.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.394388 vivarium-1.0.4/docs/source/concepts/
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/concepts/builder.rst
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/concepts/components.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/concepts/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/concepts/crn.rst
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/concepts/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/concepts/entry_points.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/concepts/event.rst
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/concepts/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/concepts/interpolation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/concepts/lifecycle.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/concepts/lookup.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.398388 vivarium-1.0.4/docs/source/concepts/model_specification/
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/concepts/model_specification/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/concepts/model_specification/yaml_basics.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/concepts/population.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/concepts/resource.rst
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/concepts/time.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/concepts/values.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/glossary.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.398388 vivarium-1.0.4/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)    32924 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/images/crn_compare_cubes.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   474719 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/images/crn_cube.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   736204 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/images/crn_sim_alignment.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    12794 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/images/pipeline.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.398388 vivarium-1.0.4/docs/source/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/tutorials/artifact.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12496 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/tutorials/boids.rst
--rw-r--r--   0 runner    (1001) docker     (123)    30080 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/tutorials/disease_model.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/tutorials/exploration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/tutorials/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/tutorials/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.398388 vivarium-1.0.4/docs/source/tutorials/running_a_simulation/
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/tutorials/running_a_simulation/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/tutorials/running_a_simulation/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-01-25 22:00:38.000000 vivarium-1.0.4/docs/source/tutorials/running_a_simulation/interactive.rst
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-25 22:00:38.000000 vivarium-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-25 22:00:47.414388 vivarium-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-01-25 22:00:38.000000 vivarium-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.382388 vivarium-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.402388 vivarium-1.0.4/src/vivarium/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20046 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/config_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.402388 vivarium-1.0.4/src/vivarium/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.402388 vivarium-1.0.4/src/vivarium/examples/boids/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/examples/boids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/examples/boids/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/examples/boids/neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/examples/boids/population.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/examples/boids/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.406388 vivarium-1.0.4/src/vivarium/examples/disease_model/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/examples/disease_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/examples/disease_model/disease.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/examples/disease_model/disease_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/examples/disease_model/intervention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/examples/disease_model/mortality.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/examples/disease_model/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/examples/disease_model/population.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/examples/disease_model/risk.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.406388 vivarium-1.0.4/src/vivarium/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.406388 vivarium-1.0.4/src/vivarium/framework/artifact/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/artifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/artifact/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)    13293 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/artifact/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/artifact/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.410388 vivarium-1.0.4/src/vivarium/framework/components/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/components/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/components/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    22771 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)    15014 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.410388 vivarium-1.0.4/src/vivarium/framework/population/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/population/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/population/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17485 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/population/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    21337 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/population/population_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.410388 vivarium-1.0.4/src/vivarium/framework/randomness/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/randomness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/randomness/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/randomness/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/randomness/index_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/randomness/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/randomness/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    12125 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.410388 vivarium-1.0.4/src/vivarium/framework/results/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/results/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/results/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/results/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/results/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/results/stratification.py
--rw-r--r--   0 runner    (1001) docker     (123)    17224 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/state_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    23655 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/framework/values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.410388 vivarium-1.0.4/src/vivarium/interface/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/interface/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/interface/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/interface/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    14076 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-01-25 22:00:38.000000 vivarium-1.0.4/src/vivarium/testing_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.402388 vivarium-1.0.4/src/vivarium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-01-25 22:00:47.000000 vivarium-1.0.4/src/vivarium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-01-25 22:00:47.000000 vivarium-1.0.4/src/vivarium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 22:00:47.000000 vivarium-1.0.4/src/vivarium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-25 22:00:47.000000 vivarium-1.0.4/src/vivarium.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 22:00:47.000000 vivarium-1.0.4/src/vivarium.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-01-25 22:00:47.000000 vivarium-1.0.4/src/vivarium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-25 22:00:47.000000 vivarium-1.0.4/src/vivarium.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.410388 vivarium-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.410388 vivarium-1.0.4/tests/config_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/config_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/config_tree/test_basic_functionality.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/config_tree/test_ingestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.414388 vivarium-1.0.4/tests/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.414388 vivarium-1.0.4/tests/framework/artifact/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/artifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/artifact/test_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/artifact/test_hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/artifact/test_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.414388 vivarium-1.0.4/tests/framework/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/components/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/components/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/components/test_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.414388 vivarium-1.0.4/tests/framework/population/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/population/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/population/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    26165 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/population/test_population_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.414388 vivarium-1.0.4/tests/framework/randomness/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/randomness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/randomness/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/randomness/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/randomness/test_index_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/randomness/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/randomness/test_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.414388 vivarium-1.0.4/tests/framework/results/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/results/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13849 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/results/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/results/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/results/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/results/test_stratification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/test_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/test_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/test_randomness.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/test_state_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/framework/test_values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.414388 vivarium-1.0.4/tests/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/interface/test_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:00:47.414388 vivarium-1.0.4/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/test_data/bad_model_specification.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/test_data/mock_model_specification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/test_data/mock_user_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-01-25 22:00:38.000000 vivarium-1.0.4/tests/test_interpolation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.946247 vivarium-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-05-03 21:39:34.000000 vivarium-1.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-03 21:39:34.000000 vivarium-1.1.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-03 21:39:34.000000 vivarium-1.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-03 21:39:34.000000 vivarium-1.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-03 21:39:34.000000 vivarium-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-03 21:39:46.946247 vivarium-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-03 21:39:34.000000 vivarium-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.918246 vivarium-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/nitpick-exceptions
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.918246 vivarium-1.1.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.918246 vivarium-1.1.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.918246 vivarium-1.1.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.918246 vivarium-1.1.0/docs/source/api_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/config_tree.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/exceptions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.922246 vivarium-1.1.0/docs/source/api_reference/framework/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.922246 vivarium-1.1.0/docs/source/api_reference/framework/artifact/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/artifact/artifact.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/artifact/hdf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/artifact/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/artifact/manager.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.922246 vivarium-1.1.0/docs/source/api_reference/framework/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/components/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/components/manager.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/components/parser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/engine.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/event.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/lifecycle.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.922246 vivarium-1.1.0/docs/source/api_reference/framework/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/logging/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/logging/manager.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/logging/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/lookup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/metrics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/plugins.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.922246 vivarium-1.1.0/docs/source/api_reference/framework/population/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/population/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/population/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/population/manager.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/population/population_view.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.922246 vivarium-1.1.0/docs/source/api_reference/framework/randomness/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/randomness/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/randomness/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/randomness/index_map.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/randomness/manager.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/randomness/stream.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/resource.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/state_machine.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/time.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/values.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.922246 vivarium-1.1.0/docs/source/api_reference/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/interface/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/interface/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/interface/interactive.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/interface/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/interpolation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/testing_utilities.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.926246 vivarium-1.1.0/docs/source/concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/builder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/crn.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/entry_points.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/event.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/interpolation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/lifecycle.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/lookup.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.926246 vivarium-1.1.0/docs/source/concepts/model_specification/
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/model_specification/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/model_specification/yaml_basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/population.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/resource.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/time.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/values.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/glossary.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.926246 vivarium-1.1.0/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    32924 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/images/crn_compare_cubes.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   474719 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/images/crn_cube.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   736204 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/images/crn_sim_alignment.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    12794 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/images/pipeline.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.926246 vivarium-1.1.0/docs/source/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/tutorials/artifact.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12496 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/tutorials/boids.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    30080 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/tutorials/disease_model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/tutorials/exploration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/tutorials/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/tutorials/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.926246 vivarium-1.1.0/docs/source/tutorials/running_a_simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/tutorials/running_a_simulation/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/tutorials/running_a_simulation/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/tutorials/running_a_simulation/interactive.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-03 21:39:34.000000 vivarium-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 21:39:46.946247 vivarium-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-05-03 21:39:34.000000 vivarium-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.918246 vivarium-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.930246 vivarium-1.1.0/src/vivarium/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20046 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/config_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.930246 vivarium-1.1.0/src/vivarium/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.930246 vivarium-1.1.0/src/vivarium/examples/boids/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/boids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/boids/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/boids/neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/boids/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/boids/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.930246 vivarium-1.1.0/src/vivarium/examples/disease_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/disease_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/disease_model/disease.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/disease_model/disease_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/disease_model/intervention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/disease_model/mortality.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/disease_model/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/disease_model/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/disease_model/risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.930246 vivarium-1.1.0/src/vivarium/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.934247 vivarium-1.1.0/src/vivarium/framework/artifact/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/artifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/artifact/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/artifact/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/artifact/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.934247 vivarium-1.1.0/src/vivarium/framework/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/components/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/components/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15142 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22771 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/lifecycle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.934247 vivarium-1.1.0/src/vivarium/framework/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/logging/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/logging/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15012 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.934247 vivarium-1.1.0/src/vivarium/framework/population/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/population/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/population/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17485 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/population/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21337 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/population/population_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.934247 vivarium-1.1.0/src/vivarium/framework/randomness/
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/randomness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/randomness/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9330 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/randomness/index_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/randomness/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/randomness/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12195 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.934247 vivarium-1.1.0/src/vivarium/framework/results/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/results/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/results/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/results/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/results/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/results/stratification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17224 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23704 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.934247 vivarium-1.1.0/src/vivarium/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/interface/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/interface/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/interface/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14074 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/testing_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.930246 vivarium-1.1.0/src/vivarium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-03 21:39:46.000000 vivarium-1.1.0/src/vivarium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-05-03 21:39:46.000000 vivarium-1.1.0/src/vivarium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 21:39:46.000000 vivarium-1.1.0/src/vivarium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-03 21:39:46.000000 vivarium-1.1.0/src/vivarium.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 21:39:46.000000 vivarium-1.1.0/src/vivarium.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-03 21:39:46.000000 vivarium-1.1.0/src/vivarium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 21:39:46.000000 vivarium-1.1.0/src/vivarium.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.934247 vivarium-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.934247 vivarium-1.1.0/tests/config_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/config_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/config_tree/test_basic_functionality.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/config_tree/test_ingestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.942247 vivarium-1.1.0/tests/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.942247 vivarium-1.1.0/tests/framework/artifact/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/artifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/artifact/test_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/artifact/test_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/artifact/test_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.942247 vivarium-1.1.0/tests/framework/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/components/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/components/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/components/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.942247 vivarium-1.1.0/tests/framework/population/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/population/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/population/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26165 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/population/test_population_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.942247 vivarium-1.1.0/tests/framework/randomness/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/randomness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/randomness/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/randomness/test_crn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/randomness/test_index_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/randomness/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/randomness/test_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.942247 vivarium-1.1.0/tests/framework/results/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/results/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/results/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/results/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/results/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/results/test_stratification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/test_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/test_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/test_state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/test_values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.946247 vivarium-1.1.0/tests/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/interface/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.946247 vivarium-1.1.0/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/test_data/bad_model_specification.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/test_data/mock_model_specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/test_data/mock_user_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/test_interpolation.py
```

### Comparing `vivarium-1.0.4/CHANGELOG.rst` & `vivarium-1.1.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+**1.1.0 - 05/03/23**
+
+ - Clean up randomness system
+ - Fix a bug in stratification when a stratum is empty
+ - Create a dedicated logging system
+ - Fix bug in preventing passing an Iterable to `rate_to_probability`
+
 **1.0.4 - 01/25/23**
 
  - Bugfixes for ResultsContext
 
 **1.0.3 - 01/19/23**
 
  - Enhancement to use pop_data.user_data.get pattern in BasePopulation example
```

### Comparing `vivarium-1.0.4/CODE_OF_CONDUCT.rst` & `vivarium-1.1.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/CONTRIBUTING.rst` & `vivarium-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/LICENSE.txt` & `vivarium-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/PKG-INFO` & `vivarium-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vivarium
-Version: 1.0.4
+Version: 1.1.0
 Summary: vivarium is a microsimulation framework built on top of the standard scientific python stack.
 Home-page: https://github.com/ihmeuw/vivarium
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `vivarium-1.0.4/README.rst` & `vivarium-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/Makefile` & `vivarium-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/nitpick-exceptions` & `vivarium-1.1.0/docs/nitpick-exceptions`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 py:class pandas.core.indexes.multi.MultiIndex
 py:class pandas._libs.tslibs.timestamps.Timestamp
 py:class pandas._libs.tslibs.timedeltas.Timedelta
 py:class pandas.core.frame.DataFrame
 py:class pandas.core.series.Series
 py:class pandas.core.generic.PandasObject
 
+# loguru
+py:class loguru._logger.Logger
+
 # vivarium
 # Type aliases don't play nicely with sphinx when you import them
 # elsewhere.  Works fine for static type checker though.  I think this
 # is cause sphinx does runtime checks.
 py:class Time
 py:class vivarium.framework.time.Time
 py:class Timedelta
```

### Comparing `vivarium-1.0.4/docs/source/concepts/builder.rst` & `vivarium-1.1.0/docs/source/concepts/builder.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/source/concepts/crn.rst` & `vivarium-1.1.0/docs/source/concepts/crn.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/source/concepts/entry_points.rst` & `vivarium-1.1.0/docs/source/concepts/entry_points.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/source/concepts/event.rst` & `vivarium-1.1.0/docs/source/concepts/event.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/source/concepts/lifecycle.rst` & `vivarium-1.1.0/docs/source/concepts/lifecycle.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/source/concepts/lookup.rst` & `vivarium-1.1.0/docs/source/concepts/lookup.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/source/concepts/model_specification/index.rst` & `vivarium-1.1.0/docs/source/concepts/model_specification/index.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/source/concepts/model_specification/yaml_basics.rst` & `vivarium-1.1.0/docs/source/concepts/model_specification/yaml_basics.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/source/concepts/population.rst` & `vivarium-1.1.0/docs/source/concepts/population.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/source/concepts/values.rst` & `vivarium-1.1.0/docs/source/concepts/values.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/source/conf.py` & `vivarium-1.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/source/glossary.rst` & `vivarium-1.1.0/docs/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/source/images/crn_compare_cubes.jpg` & `vivarium-1.1.0/docs/source/images/crn_compare_cubes.jpg`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/source/images/crn_cube.jpg` & `vivarium-1.1.0/docs/source/images/crn_cube.jpg`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/source/images/crn_sim_alignment.jpg` & `vivarium-1.1.0/docs/source/images/crn_sim_alignment.jpg`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/source/images/pipeline.jpg` & `vivarium-1.1.0/docs/source/images/pipeline.jpg`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/source/installation.rst` & `vivarium-1.1.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/source/tutorials/artifact.rst` & `vivarium-1.1.0/docs/source/tutorials/artifact.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/source/tutorials/boids.rst` & `vivarium-1.1.0/docs/source/tutorials/boids.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/source/tutorials/disease_model.rst` & `vivarium-1.1.0/docs/source/tutorials/disease_model.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/source/tutorials/exploration.rst` & `vivarium-1.1.0/docs/source/tutorials/exploration.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/source/tutorials/getting_started.rst` & `vivarium-1.1.0/docs/source/tutorials/getting_started.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/source/tutorials/running_a_simulation/cli.rst` & `vivarium-1.1.0/docs/source/tutorials/running_a_simulation/cli.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/docs/source/tutorials/running_a_simulation/interactive.rst` & `vivarium-1.1.0/docs/source/tutorials/running_a_simulation/interactive.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/setup.py` & `vivarium-1.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,28 +16,27 @@
     sys.exit(1)
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 if __name__ == "__main__":
-
     base_dir = Path(__file__).parent
     src_dir = base_dir / "src"
 
     about = {}
     with (src_dir / "vivarium" / "__about__.py").open() as f:
         exec(f.read(), about)
 
     with (base_dir / "README.rst").open() as f:
         long_description = f.read()
 
     install_requirements = [
         "numpy",
-        "pandas",
+        "pandas<2.0.0",
         "pyyaml>=5.1",
         "scipy",
         "click",
         "tables",
         "networkx",
         "loguru",
     ]
```

### Comparing `vivarium-1.0.4/src/vivarium/__about__.py` & `vivarium-1.1.0/src/vivarium/__about__.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,14 @@
     "__copyright__",
 ]
 
 __title__ = "vivarium"
 __summary__ = "vivarium is a microsimulation framework built on top of the standard scientific python stack."
 __uri__ = "https://github.com/ihmeuw/vivarium"
 
-__version__ = "1.0.4"
+__version__ = "1.1.0"
 
 __author__ = "The vivarium developers"
 __email__ = "vivarium.dev@gmail.com"
 
 __license__ = "BSD-3-Clause"
 __copyright__ = f"Copyright 2016-2023 {__author__}"
```

### Comparing `vivarium-1.0.4/src/vivarium/config_tree.py` & `vivarium-1.1.0/src/vivarium/config_tree.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/src/vivarium/examples/boids/location.py` & `vivarium-1.1.0/src/vivarium/examples/boids/location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 import pandas as pd
 
 
 class Location:
-
     configuration_defaults = {
         "location": {
             "width": 1000,  # Width of our field
             "height": 1000,  # Height of our field
         }
     }
```

### Comparing `vivarium-1.0.4/src/vivarium/examples/boids/neighbors.py` & `vivarium-1.1.0/src/vivarium/examples/boids/neighbors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import pandas as pd
 from scipy import spatial
 
 
 class Neighbors:
-
     configuration_defaults = {"neighbors": {"radius": 10}}
 
     def __init__(self):
         self.name = "Neighbors"
 
     def setup(self, builder):
         self.radius = builder.configuration.neighbors.radius
```

### Comparing `vivarium-1.0.4/src/vivarium/examples/boids/population.py` & `vivarium-1.1.0/src/vivarium/examples/boids/population.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 import pandas as pd
 
 
 class Population:
-
     configuration_defaults = {
         "population": {
             "colors": ["red", "blue"],
         }
     }
 
     def __init__(self):
```

### Comparing `vivarium-1.0.4/src/vivarium/examples/disease_model/__init__.py` & `vivarium-1.1.0/src/vivarium/examples/disease_model/__init__.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/src/vivarium/examples/disease_model/disease.py` & `vivarium-1.1.0/src/vivarium/examples/disease_model/disease.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,14 @@
         metrics[self.state_column + "_prevalent_cases"] = len(
             pop[pop[self.state_column] != self.initial_state]
         )
         return metrics
 
 
 class SISDiseaseModel:
-
     configuration_defaults = {
         "disease": {
             "incidence_rate": 0.005,
             "remission_rate": 0.05,
             "excess_mortality_rate": 0.01,
         }
     }
```

### Comparing `vivarium-1.0.4/src/vivarium/examples/disease_model/disease_model.yaml` & `vivarium-1.1.0/src/vivarium/examples/disease_model/disease_model.yaml`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/src/vivarium/examples/disease_model/intervention.py` & `vivarium-1.1.0/src/vivarium/examples/disease_model/intervention.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import pandas as pd
 
 from vivarium.framework.engine import Builder
 
 
 class TreatmentIntervention:
-
     configuration_defaults = {
         "intervention": {
             "effect_size": 0.5,
         }
     }
 
     def __init__(self, name: str, affected_value: str):
```

### Comparing `vivarium-1.0.4/src/vivarium/examples/disease_model/mortality.py` & `vivarium-1.1.0/src/vivarium/examples/disease_model/mortality.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/src/vivarium/examples/disease_model/observer.py` & `vivarium-1.1.0/src/vivarium/examples/disease_model/observer.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import pandas as pd
 
 from vivarium.framework.engine import Builder
 
 
 class Observer:
-
     configuration_defaults = {
         "mortality": {
             "life_expectancy": 80,
         }
     }
 
     def __init__(self):
@@ -20,15 +19,14 @@
     def setup(self, builder: Builder):
         self.life_expectancy = builder.configuration.mortality.life_expectancy
         self.population_view = builder.population.get_view(["age", "alive"])
 
         builder.value.register_value_modifier("metrics", self.metrics)
 
     def metrics(self, index: pd.Index, metrics: Dict):
-
         pop = self.population_view.get(index)
         metrics["total_population_alive"] = len(pop[pop.alive == "alive"])
         metrics["total_population_dead"] = len(pop[pop.alive == "dead"])
 
         metrics["years_of_life_lost"] = (
             self.life_expectancy - pop.age[pop.alive == "dead"]
         ).sum()
```

### Comparing `vivarium-1.0.4/src/vivarium/examples/disease_model/population.py` & `vivarium-1.1.0/src/vivarium/examples/disease_model/population.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         ):
             raise ValueError(
                 "If running with CRN, you must specify ['entrance_time', 'age'] as"
                 "the randomness key columns."
             )
 
         self.age_randomness = builder.randomness.get_stream(
-            "age_initialization", for_initialization=self.with_common_random_numbers
+            "age_initialization", initializes_crn_attributes=self.with_common_random_numbers
         )
         self.sex_randomness = builder.randomness.get_stream("sex_initialization")
 
         columns_created = ["age", "sex", "alive", "entrance_time"]
         builder.population.initializes_simulants(
             self.on_initialize_simulants, creates_columns=columns_created
         )
```

### Comparing `vivarium-1.0.4/src/vivarium/examples/disease_model/risk.py` & `vivarium-1.1.0/src/vivarium/examples/disease_model/risk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pandas as pd
 
 
 class Risk:
-
     configuration_defaults = {
         "risk": {
             "proportion_exposed": 0.3,
         },
     }
 
     def __init__(self, name):
@@ -46,15 +45,14 @@
         return self.exposure_threshold(index) > propensity
 
     def __repr__(self):
         return f"Risk(name={self.name})"
 
 
 class RiskEffect:
-
     configuration_defaults = {
         "risk_effect": {
             "relative_risk": 2,
         },
     }
 
     def __init__(self, risk, disease_rate):
```

### Comparing `vivarium-1.0.4/src/vivarium/framework/artifact/artifact.py` & `vivarium-1.1.0/src/vivarium/framework/artifact/artifact.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/src/vivarium/framework/artifact/hdf.py` & `vivarium-1.1.0/src/vivarium/framework/artifact/hdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,14 @@
             entity_key.path
         ).attrs.metadata = metadata  # NOTE: must use attrs. write this up
 
 
 def _write_json_blob(path: Path, entity_key: EntityKey, data: Any):
     """Writes a Python object as json to the HDF file at the given path."""
     with tables.open_file(str(path), "a") as store:
-
         if entity_key.group_prefix not in store:
             store.create_group("/", entity_key.type)
 
         if entity_key.group not in store:
             store.create_group(entity_key.group_prefix, entity_key.group_name)
 
         with filenode.new_node(
```

### Comparing `vivarium-1.0.4/src/vivarium/framework/artifact/manager.py` & `vivarium-1.1.0/src/vivarium/framework/artifact/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 """
 import re
 from pathlib import Path
 from typing import Any, Sequence, Union
 
 import pandas as pd
-from loguru import logger
 
 from vivarium.config_tree import ConfigTree
 from vivarium.framework.artifact.artifact import Artifact
 
 _Filter = Union[str, int, Sequence[int], Sequence[str]]
 
 
@@ -33,14 +32,15 @@
 
     @property
     def name(self):
         return "artifact_manager"
 
     def setup(self, builder):
         """Performs this component's simulation setup."""
+        self.logger = builder.logging.get_logger(self.name)
         # because not all columns are accessible via artifact filter terms, apply config filters separately
         self.config_filter_term = validate_filter_term(
             builder.configuration.input_data.artifact_filter_term
         )
         self.artifact = self._load_artifact(builder.configuration)
         builder.lifecycle.add_constraint(self.load, allow_during=["setup"])
 
@@ -59,17 +59,17 @@
         -------
             An interface to the data artifact.
         """
         if not configuration.input_data.artifact_path:
             return None
         artifact_path = parse_artifact_path_config(configuration)
         base_filter_terms = get_base_filter_terms(configuration)
-        logger.debug(f"Running simulation from artifact located at {artifact_path}.")
-        logger.debug(f"Artifact base filter terms are {base_filter_terms}.")
-        logger.debug(f"Artifact additional filter terms are {self.config_filter_term}.")
+        self.logger.info(f"Running simulation from artifact located at {artifact_path}.")
+        self.logger.info(f"Artifact base filter terms are {base_filter_terms}.")
+        self.logger.info(f"Artifact additional filter terms are {self.config_filter_term}.")
         return Artifact(artifact_path, base_filter_terms)
 
     def load(self, entity_key: str, **column_filters: _Filter) -> Any:
         """Loads data associated with the given entity key.
 
         Parameters
         ----------
@@ -229,15 +229,14 @@
     -------
     str
         The path to the data artifact.
     """
     path = Path(config.input_data.artifact_path)
 
     if not path.is_absolute():
-
         path_config = config.input_data.metadata("artifact_path")[-1]
         if path_config["source"] is None:
             raise ValueError("Insufficient information provided to find artifact.")
         path = Path(path_config["source"]).parent.joinpath(path).resolve()
 
     if not path.exists():
         raise FileNotFoundError(f"Cannot find artifact at path {path}")
```

### Comparing `vivarium-1.0.4/src/vivarium/framework/components/manager.py` & `vivarium-1.1.0/src/vivarium/framework/components/manager.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/src/vivarium/framework/components/parser.py` & `vivarium-1.1.0/src/vivarium/framework/components/parser.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/src/vivarium/framework/configuration.py` & `vivarium-1.1.0/src/vivarium/framework/configuration.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/src/vivarium/framework/engine.py` & `vivarium-1.1.0/src/vivarium/framework/engine.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,49 +14,100 @@
 can read more about how the builder works and what services is exposes
 :ref:`here <builder_concept>`.
 
 Finally, there are a handful of wrapper methods that allow a user or user
 tools to easily setup and run a simulation.
 
 """
-import time
 from pathlib import Path
 from pprint import pformat
-from typing import Dict, List, Tuple, Union
+from typing import Dict, List, Set, Union
 
 import numpy as np
 import pandas as pd
-from loguru import logger
 
 from vivarium.config_tree import ConfigTree
+from vivarium.exceptions import VivariumError
 from vivarium.framework.configuration import build_model_specification
 
 from .artifact import ArtifactInterface
 from .components import ComponentInterface
 from .event import EventInterface
 from .lifecycle import LifeCycleInterface
+from .logging import LoggingInterface
 from .lookup import LookupTableInterface
 from .metrics import Metrics
 from .plugins import PluginManager
 from .population import PopulationInterface
 from .randomness import RandomnessInterface
 from .resource import ResourceInterface
 from .results import ResultsInterface
 from .time import TimeInterface
 from .values import ValuesInterface
 
 
 class SimulationContext:
+    _created_simulation_contexts: Set[str] = set()
+
+    @staticmethod
+    def _get_context_name(sim_name: Union[str, None]) -> str:
+        """Get a unique name for a simulation context.
+
+        Parameters
+        ----------
+        sim_name
+            The name of the simulation context.  If None, a unique name will be generated.
+
+        Returns
+        -------
+        str
+            A unique name for the simulation context.
+
+        Note
+        ----
+        This method mutates process global state (the class attribute
+        ``_created_simulation_contexts``) in order to keep track contexts that have been
+        generated. This functionality makes generating simulation contexts in parallel
+        a non-threadsafe operation.
+
+        """
+        if sim_name is None:
+            sim_number = len(SimulationContext._created_simulation_contexts) + 1
+            sim_name = f"simulation_{sim_number}"
+
+        if sim_name in SimulationContext._created_simulation_contexts:
+            msg = (
+                "Attempting to create two SimulationContexts "
+                f"with the same name {sim_name}"
+            )
+            raise VivariumError(msg)
+
+        SimulationContext._created_simulation_contexts.add(sim_name)
+        return sim_name
+
+    @staticmethod
+    def _clear_context_cache():
+        """Clear the cache of simulation context names.
+
+        This is primarily useful for testing purposes.
+
+        """
+        SimulationContext._created_simulation_contexts = set()
+
     def __init__(
         self,
         model_specification: Union[str, Path, ConfigTree] = None,
         components: Union[List, Dict, ConfigTree] = None,
         configuration: Union[Dict, ConfigTree] = None,
         plugin_configuration: Union[Dict, ConfigTree] = None,
+        sim_name: str = None,
+        logging_verbosity: int = 1,
     ):
+        self._name = self._get_context_name(sim_name)
+
         # Bootstrap phase: Parse arguments, make private managers
         component_configuration = (
             components if isinstance(components, (dict, ConfigTree)) else None
         )
         self._additional_components = components if isinstance(components, List) else []
         model_specification = build_model_specification(
             model_specification, component_configuration, configuration, plugin_configuration
@@ -64,15 +115,20 @@
 
         self._plugin_configuration = model_specification.plugins
         self._component_configuration = model_specification.components
         self.configuration = model_specification.configuration
 
         self._plugin_manager = PluginManager(model_specification.plugins)
 
-        # TODO: Setup logger here.
+        self._logging = self._plugin_manager.get_plugin("logging")
+        self._logging.configure_logging(
+            simulation_name=self.name,
+            verbosity=logging_verbosity,
+        )
+        self._logger = self._logging.get_logger()
 
         self._builder = Builder(self.configuration, self._plugin_manager)
 
         # This formally starts the initialization phase (this call makes the
         # life-cycle manager).
         self._lifecycle = self._plugin_manager.get_plugin("lifecycle")
         self._lifecycle.add_phase("setup", ["setup", "post_setup", "population_creation"])
@@ -96,20 +152,21 @@
         self._randomness = self._plugin_manager.get_plugin("randomness")
         self._data = self._plugin_manager.get_plugin("data")
 
         for name, controller in self._plugin_manager.get_optional_controllers().items():
             setattr(self, f"_{name}", controller)
 
         # The order the managers are added is important.  It represents the
-        # order in which they will be set up.  The clock is required by
-        # several of the other managers, including the lifecycle manager.  The
+        # order in which they will be set up.  The logging manager and the clock are
+        # required by several of the other managers, including the lifecycle manager. The
         # lifecycle manager is also required by most managers. The randomness
         # manager requires the population manager.  The remaining managers need
         # no ordering.
         managers = [
+            self._logging,
             self._clock,
             self._lifecycle,
             self._resource,
             self._values,
             self._population,
             self._randomness,
             self._events,
@@ -134,15 +191,15 @@
             self.get_population, restrict_during=["initialization", "setup", "post_setup"]
         )
 
         self.add_components(components)
 
     @property
     def name(self):
-        return "simulation_context"
+        return self._name
 
     def setup(self):
         self._lifecycle.set_state("setup")
         self.configuration.freeze()
         self._component_manager.setup_components(self._builder)
 
         self.simulant_creator = self._builder.population.get_simulant_creator()
@@ -165,46 +222,46 @@
         population_size = pop_params.population_size
         self.simulant_creator(
             population_size, population_configuration={"sim_state": "setup"}
         )
         self._clock.step_forward()
 
     def step(self):
-        logger.debug(self._clock.time)
+        self._logger.debug(self._clock.time)
         for event in self.time_step_events:
             self._lifecycle.set_state(event)
             self.time_step_emitters[event](self._population.get_population(True).index)
         self._clock.step_forward()
 
     def run(self):
         while self._clock.time < self._clock.stop_time:
             self.step()
 
     def finalize(self):
         self._lifecycle.set_state("simulation_end")
         self.end_emitter(self._population.get_population(True).index)
         unused_config_keys = self.configuration.unused_keys()
         if unused_config_keys:
-            logger.debug(
+            self._logger.warning(
                 f"Some configuration keys not used during run: {unused_config_keys}."
             )
 
     def report(self, print_results=True):
         self._lifecycle.set_state("report")
         metrics = self._values.get_value("metrics")(
             self._population.get_population(True).index
         )
         if print_results:
-            logger.debug("\n" + pformat(metrics))
+            self._logger.info("\n" + pformat(metrics))
             performance_metrics = self.get_performance_metrics()
             performance_metrics = performance_metrics.to_string(
                 index=False,
                 float_format=lambda x: f"{x:.2f}",
             )
-            logger.debug("\n" + performance_metrics)
+            self._logger.info("\n" + performance_metrics)
 
         return metrics
 
     def get_performance_metrics(self) -> pd.DataFrame:
         timing_dict = self._lifecycle.timings
         total_time = np.sum([np.sum(v) for v in timing_dict.values()])
         timing_dict["total"] = [total_time]
@@ -226,41 +283,40 @@
         """Adds new components to the simulation."""
         self._component_manager.add_components(component_list)
 
     def get_population(self, untracked: bool = True):
         return self._population.get_population(untracked)
 
     def __repr__(self):
-        return "SimulationContext()"
-
-    def __str__(self):
-        return str(self._lifecycle)
+        return f"SimulationContext({self.name})"
 
 
 class Builder:
     """Toolbox for constructing and configuring simulation components.
 
     This is the access point for components through which they are able to
     utilize a variety of interfaces to interact with the simulation framework.
 
     Attributes
     ----------
+    logging: LoggingInterface
+        Provides access to the :ref:`logging<logging_concept>` system.
     lookup: LookupTableInterface
         Provides access to simulant-specific data via the
         :ref:`lookup table<lookup_concept>` abstraction.
     value: ValuesInterface
         Provides access to computed simulant attribute values via the
         :ref:`value pipeline<values_concept>` system.
     event: EventInterface
         Provides access to event listeners utilized in the
         :ref:`event<event_concept>` system.
     population: PopulationInterface
         Provides access to simulant state table via the
         :ref:`population<population_concept>` system.
-    resource: ResourceInterface
+    resources: ResourceInterface
         Provides access to the :ref:`resource<resource_concept>` system,
         which manages dependencies between components.
     time: TimeInterface
         Provides access to the simulation's :ref:`clock<time_concept>`.
     components: ComponentInterface
         Provides access to the :ref:`component management<components_concept>`
         system, which maintains a reference to all managers and components in
@@ -278,14 +334,17 @@
     created during the initialization of a :class:`SimulationContext`
 
     """
 
     def __init__(self, configuration, plugin_manager):
         self.configuration = configuration
 
+        self.logging = plugin_manager.get_plugin_interface(
+            "logging"
+        )  # type: LoggingInterface
         self.lookup = plugin_manager.get_plugin_interface(
             "lookup"
         )  # type: LookupTableInterface
         self.value = plugin_manager.get_plugin_interface("value")  # type: ValuesInterface
         self.event = plugin_manager.get_plugin_interface("event")  # type: EventInterface
         self.population = plugin_manager.get_plugin_interface(
             "population"
```

### Comparing `vivarium-1.0.4/src/vivarium/framework/event.py` & `vivarium-1.1.0/src/vivarium/framework/event.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/src/vivarium/framework/lifecycle.py` & `vivarium-1.1.0/src/vivarium/framework/lifecycle.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/src/vivarium/framework/lookup.py` & `vivarium-1.1.0/src/vivarium/framework/lookup.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,14 @@
         parameter_columns: Union[List[str], Tuple],
         value_columns: Union[List[str], Tuple[str]],
         interpolation_order: int,
         clock: Callable,
         extrapolate: bool,
         validate: bool,
     ):
-
         self.data = data
         self.population_view = population_view
         self.key_columns = key_columns
         param_cols_with_edges = []
         for p in parameter_columns:
             param_cols_with_edges += [(p, f"{p}_start", f"{p}_end")]
         self.parameter_columns = param_cols_with_edges
@@ -134,15 +133,14 @@
     """
 
     def __init__(
         self,
         values: Union[List[ScalarValue], Tuple[ScalarValue]],
         value_columns: Union[List[str], Tuple[str]],
     ):
-
         self.values = values
         self.value_columns = value_columns
 
     def __call__(self, index: pd.Index) -> pd.DataFrame:
         """Broadcast this tables values over the provided index.
 
         Parameters
```

### Comparing `vivarium-1.0.4/src/vivarium/framework/metrics.py` & `vivarium-1.1.0/src/vivarium/framework/metrics.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/src/vivarium/framework/plugins.py` & `vivarium-1.1.0/src/vivarium/framework/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 """
 from vivarium.config_tree import ConfigTree
 from vivarium.exceptions import VivariumError
 
 from .utilities import import_by_path
 
 _MANAGERS = {
+    "logging": {
+        "controller": "vivarium.framework.logging.LoggingManager",
+        "builder_interface": "vivarium.framework.logging.LoggingInterface",
+    },
     "lookup": {
         "controller": "vivarium.framework.lookup.LookupTableManager",
         "builder_interface": "vivarium.framework.lookup.LookupTableInterface",
     },
     "randomness": {
         "controller": "vivarium.framework.randomness.RandomnessManager",
         "builder_interface": "vivarium.framework.randomness.RandomnessInterface",
```

### Comparing `vivarium-1.0.4/src/vivarium/framework/population/__init__.py` & `vivarium-1.1.0/src/vivarium/framework/population/__init__.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/src/vivarium/framework/population/manager.py` & `vivarium-1.1.0/src/vivarium/framework/population/manager.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/src/vivarium/framework/population/population_view.py` & `vivarium-1.1.0/src/vivarium/framework/population/population_view.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/src/vivarium/framework/randomness/__init__.py` & `vivarium-1.1.0/src/vivarium/framework/randomness/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 The current approach is to generate hash-based
 seeds where the key is the simulation time, the simulant's id, the draw number
 and a unique id for the decision point which needs the randomness.
 These seeds are then used to generate `numpy.random.RandomState` objects that
 can be used to create pseudo-random numbers in a repeatable manner.
 
 
-For mor information, see the Common Random Numbers
+For more information, see the Common Random Numbers
 :ref:`concept note <crn_concept>`.
 
 """
-from vivarium.framework.randomness.core import RESIDUAL_CHOICE, choice, get_hash, random
 from vivarium.framework.randomness.exceptions import RandomnessError
 from vivarium.framework.randomness.manager import RandomnessInterface, RandomnessManager
-from vivarium.framework.randomness.stream import RandomnessStream
+from vivarium.framework.randomness.stream import (
+    RESIDUAL_CHOICE,
+    RandomnessStream,
+    get_hash,
+)
```

### Comparing `vivarium-1.0.4/src/vivarium/framework/randomness/manager.py` & `vivarium-1.1.0/src/vivarium/framework/randomness/manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 """
 =========================
 Randomness System Manager
 =========================
 """
 import pandas as pd
 
-from vivarium.framework.randomness.core import get_hash
 from vivarium.framework.randomness.exceptions import RandomnessError
 from vivarium.framework.randomness.index_map import IndexMap
-from vivarium.framework.randomness.stream import RandomnessStream
+from vivarium.framework.randomness.stream import RandomnessStream, get_hash
 
 
 class RandomnessManager:
     """Access point for common random number generation."""
 
     configuration_defaults = {
         "randomness": {
             "map_size": 1_000_000,
-            "key_columns": ["entrance_time"],
+            "key_columns": [],
             "random_seed": 0,
             "additional_seed": None,
         }
     }
 
     def __init__(self):
         self._seed = None
         self._clock = None
         self._key_columns = None
-        self._key_mapping = IndexMap()
+        self._key_mapping = None
         self._decision_points = dict()
 
     @property
     def name(self):
         return "randomness_manager"
 
     def setup(self, builder):
         self._seed = str(builder.configuration.randomness.random_seed)
         if builder.configuration.randomness.additional_seed is not None:
             self._seed += str(builder.configuration.randomness.additional_seed)
         self._clock = builder.time.clock()
         self._key_columns = builder.configuration.randomness.key_columns
+
         map_size = builder.configuration.randomness.map_size
         pop_size = builder.configuration.population.population_size
-        self._key_mapping.map_size = max(map_size, 10 * pop_size)
+        map_size = max(map_size, 10 * pop_size)
+        self._key_mapping = IndexMap(self._key_columns, map_size)
 
         self.resources = builder.resources
         self._add_constraint = builder.lifecycle.add_constraint
         self._add_constraint(self.get_seed, restrict_during=["initialization"])
         self._add_constraint(self.get_randomness_stream, allow_during=["setup"])
         self._add_constraint(
             self.register_simulants,
@@ -56,40 +57,40 @@
                 "post_setup",
                 "simulation_end",
                 "report",
             ],
         )
 
     def get_randomness_stream(
-        self, decision_point: str, for_initialization: bool = False
+        self, decision_point: str, initializes_crn_attributes: bool = False
     ) -> RandomnessStream:
         """Provides a new source of random numbers for the given decision point.
 
         Parameters
         ----------
         decision_point
             A unique identifier for a stream of random numbers.  Typically
             represents a decision that needs to be made each time step like
             'moves_left' or 'gets_disease'.
-        for_initialization
+        initializes_crn_attributes
             A flag indicating whether this stream is used to generate key
             initialization information that will be used to identify simulants
             in the Common Random Number framework. These streams cannot be
             copied and should only be used to generate the state table columns
             specified in ``builder.configuration.randomness.key_columns``.
 
         Raises
         ------
         RandomnessError
             If another location in the simulation has already created a randomness stream
             with the same identifier.
 
         """
-        stream = self._get_randomness_stream(decision_point, for_initialization)
-        if not for_initialization:
+        stream = self._get_randomness_stream(decision_point, initializes_crn_attributes)
+        if not initializes_crn_attributes:
             # We need the key columns to be created before this stream can be called.
             self.resources.add_resources(
                 "stream",
                 [decision_point],
                 stream,
                 [f"column.{name}" for name in self._key_columns],
             )
@@ -106,27 +107,27 @@
         self._add_constraint(
             stream.choice, restrict_during=["initialization", "setup", "post_setup"]
         )
 
         return stream
 
     def _get_randomness_stream(
-        self, decision_point: str, for_initialization: bool = False
+        self, decision_point: str, initializes_crn_attributes: bool = False
     ) -> RandomnessStream:
         if decision_point in self._decision_points:
             raise RandomnessError(
                 f"Two separate places are attempting to create "
                 f"the same randomness stream for {decision_point}"
             )
         stream = RandomnessStream(
             key=decision_point,
             clock=self._clock,
             seed=self._seed,
             index_map=self._key_mapping,
-            for_initialization=for_initialization,
+            initializes_crn_attributes=initializes_crn_attributes,
         )
         self._decision_points[decision_point] = stream
         return stream
 
     def get_seed(self, decision_point: str) -> int:
         """Get a randomly generated seed for use with external randomness tools.
 
@@ -162,29 +163,29 @@
             in the configuration.
 
         """
         if not all(k in simulants.columns for k in self._key_columns):
             raise RandomnessError(
                 "The simulants dataframe does not have all specified key_columns."
             )
-        self._key_mapping.update(simulants.set_index(self._key_columns).index)
+        self._key_mapping.update(simulants.loc[:, self._key_columns])
 
     def __str__(self):
         return "RandomnessManager()"
 
     def __repr__(self) -> str:
         return f"RandomnessManager(seed={self._seed}, key_columns={self._key_columns})"
 
 
 class RandomnessInterface:
     def __init__(self, manager: RandomnessManager):
         self._manager = manager
 
     def get_stream(
-        self, decision_point: str, for_initialization: bool = False
+        self, decision_point: str, initializes_crn_attributes: bool = False
     ) -> RandomnessStream:
         """Provides a new source of random numbers for the given decision point.
 
         ``vivarium`` provides a framework for Common Random Numbers which
         allows for variance reduction when modeling counter-factual scenarios.
         Users interested in causal analysis and comparisons between simulation
         scenarios should be careful to use randomness streams provided by the
@@ -192,30 +193,30 @@
 
         Parameters
         ----------
         decision_point
             A unique identifier for a stream of random numbers.  Typically
             represents a decision that needs to be made each time step like
             'moves_left' or 'gets_disease'.
-        for_initialization
+        initializes_crn_attributes
             A flag indicating whether this stream is used to generate key
             initialization information that will be used to identify simulants
             in the Common Random Number framework. These streams cannot be
             copied and should only be used to generate the state table columns
             specified in ``builder.configuration.randomness.key_columns``.
 
         Returns
         -------
         RandomnessStream
             An entry point into the Common Random Number generation framework.
             The stream provides vectorized access to random numbers and a few
             other utilities.
 
         """
-        return self._manager.get_randomness_stream(decision_point, for_initialization)
+        return self._manager.get_randomness_stream(decision_point, initializes_crn_attributes)
 
     def get_seed(self, decision_point: str) -> int:
         """Get a randomly generated seed for use with external randomness tools.
 
         Parameters
         ----------
         decision_point :
```

### Comparing `vivarium-1.0.4/src/vivarium/framework/randomness/stream.py` & `vivarium-1.1.0/src/vivarium/framework/results/interface.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,229 +1,188 @@
-"""
-==================
-Randomness Streams
-==================
+from typing import TYPE_CHECKING, Callable, List
 
-"""
-from typing import TYPE_CHECKING, Any, Callable, List, Tuple, Union
-
-import numpy as np
 import pandas as pd
 
-from vivarium.framework.randomness.core import choice, filter_for_probability, random
-from vivarium.framework.randomness.index_map import IndexMap
-from vivarium.framework.utilities import rate_to_probability
-
-
-class RandomnessStream:
-    """A stream for producing common random numbers.
-
-    `RandomnessStream` objects provide an interface to Vivarium's
-    common random number generation.  They provide a number of methods
-    for doing common simulation tasks that require random numbers like
-    making decisions among a number of choices.
-
-    Attributes
-    ----------
-    key
-        The name of the randomness stream.
-    clock
-        A way to get the current simulation time.
-    seed
-        An extra number used to seed the random number generation.
-
-    Notes
-    -----
-    Should not be constructed by client code.
-
-    Simulation components get `RandomnessStream` objects by requesting
-    them from the builder provided to them during the setup phase.
-    I.E.::
-
-        class VivariumComponent:
-            def setup(self, builder):
-                self.randomness_stream = builder.randomness.get_stream('stream_name')
-
+if TYPE_CHECKING:
+    # cyclic import
+    from vivarium.framework.results.manager import ResultsManager
+
+
+class ResultsInterface:
+    """Builder interface for the results management system.
+
+    The results management system allows users to delegate results production
+    to the simulation framework. This process attempts to roughly mimic the
+    groupby-apply logic commonly done when manipulating :mod:`pandas`
+    DataFrames. The representation of state in the simulation is complex,
+    however, as it includes information both in the population state table
+    and dynamically generated information available from the
+    :class:`value pipelines <vivarium.framework.values.Pipeline>`.
+    Additionally, good encapsulation of simulation logic typically has
+    results production separated from the modeling code into specialized
+    `Observer` components. This often highlights the need for transformations
+    of the simulation state into representations that aren't needed for
+    modeling, but are required for the stratification of produced results.
+
+    The purpose of this interface is to provide controlled access to a results
+    backend by means of the builder object. It exposes methods
+    to register stratifications, set default stratifications, and register
+    results producers. There is a special case for stratifications generated
+    by binning continuous data into categories.
+
+    The expected use pattern would be for a single component to register all
+    stratifications required by the model using :func:`register_default_stratifications`,
+    :func:`register_stratification`, and :func:`register_binned_stratification`
+    as necessary. A “binned stratification” is a stratification special case for
+    the very common situation when a single continuous value needs to be binned into
+    categorical bins. The `is_vectorized` argument should be True if the mapper
+    function expects a DataFrame corresponding to the whole population, and False
+    if it expects a row of the DataFrame corresponding to a single simulant.
     """
 
-    def __init__(
-        self,
-        key: str,
-        clock: Callable,
-        seed: Any,
-        index_map: IndexMap = None,
-        for_initialization: bool = False,
-    ):
-        self.key = key
-        self.clock = clock
-        self.seed = seed
-        self.index_map = index_map
-        self._for_initialization = for_initialization
+    def __init__(self, manager: "ResultsManager") -> None:
+        self._manager: "ResultsManager" = manager
+        self._name = "results_interface"
 
     @property
-    def name(self):
-        return f"randomness_stream_{self.key}"
-
-    def _key(self, additional_key: Any = None) -> str:
-        """Construct a hashable key from this object's state.
-
-        Parameters
-        ----------
-        additional_key
-            Any additional information used to seed random number generation.
-
-        Returns
-        -------
-        str
-            A key to seed random number generation.
-
-        """
-        return "_".join([self.key, str(self.clock()), str(additional_key), str(self.seed)])
-
-    def get_draw(self, index: pd.Index, additional_key: Any = None) -> pd.Series:
-        """Get an indexed set of numbers uniformly drawn from the unit interval.
-
-        Parameters
-        ----------
-        index
-            An index whose length is the number of random draws made
-            and which indexes the returned `pandas.Series`.
-        additional_key
-            Any additional information used to seed random number generation.
-
-        Returns
-        -------
-        pandas.Series
-            A series of random numbers indexed by the provided `pandas.Index`.
-        """
-        if self._for_initialization:
-            draw = random(
-                self._key(additional_key), pd.Index(range(len(index))), self.index_map
-            )
-            draw.index = index
-        else:
-            draw = random(self._key(additional_key), index, self.index_map)
-
-        return draw
-
-    def filter_for_rate(
+    def name(self) -> str:
+        """The name of this ResultsInterface."""
+        return self._name
+
+    def set_default_stratifications(self, default_stratifications: List[str]):
+        self._manager.set_default_stratifications(default_stratifications)
+
+    # TODO: It is not reflected in the sample code here, but the “when” parameter should be added
+    #  to the stratification registration calls, probably as a List. Consider this after observer implementation
+    def register_stratification(
         self,
-        population: Union[pd.DataFrame, pd.Series, pd.Index],
-        rate: Union[List, Tuple, np.ndarray, pd.Series],
-        additional_key: Any = None,
-    ) -> Union[pd.DataFrame, pd.Series, pd.Index]:
-        """Decide an event outcome for each individual from rates.
-
-        Given a population or its index and an array of associated rates for
-        some event to happen, we create and return the sub-population for whom
-        the event occurred.
+        name: str,
+        categories: List[str],
+        mapper: Callable = None,
+        is_vectorized: bool = False,
+        requires_columns: List[str] = (),
+        requires_values: List[str] = (),
+    ) -> None:
+        """Register quantities to observe.
 
         Parameters
         ----------
-        population
-            A view on the simulants for which we are determining the
-            outcome of an event.
-        rate
-            A 1d list of rates of the event under consideration occurring which
-            corresponds (i.e. `len(population) == len(probability))` to the
-            population view passed in. The rates must be scaled to the
-            simulation time-step size either manually or as a post-processing
-            step in a rate pipeline.
-        additional_key
-            Any additional information used to create the seed.
+        name
+            Name of the of the column created by the stratification.
+        categories
+            List of string values that the mapper is allowed to output.
+        mapper
+            A callable that emits values in `categories` given inputs from columns
+            and values in the `requires_columns` and `requires_values`, respectively.
+        is_vectorized
+            `True` if the mapper function expects a `DataFrame`, and `False` if it
+            expects a row of the `DataFrame` and should be used by calling :func:`df.apply`.
+        requires_columns
+            A list of the state table columns that already need to be present
+            and populated in the state table before the pipeline modifier
+            is called.
+        requires_values
+            A list of the value pipelines that need to be properly sourced
+            before the pipeline modifier is called.
 
         Returns
-        -------
-        pandas.core.generic.PandasObject
-            The sub-population of the simulants for whom the event occurred.
-            The return type will be the same as type(population)
-
+        ------
+        None
         """
-        return self.filter_for_probability(
-            population, rate_to_probability(rate), additional_key
+        self._manager.register_stratification(
+            name,
+            categories,
+            mapper,
+            is_vectorized,
+            requires_columns,
+            requires_values,
         )
 
-    def filter_for_probability(
+    def register_binned_stratification(
         self,
-        population: Union[pd.DataFrame, pd.Series, pd.Index],
-        probability: Union[List, Tuple, np.ndarray, pd.Series],
-        additional_key: Any = None,
-    ) -> Union[pd.DataFrame, pd.Series, pd.Index]:
-        """Decide an outcome for each individual from probabilities.
-
-        Given a population or its index and an array of associated probabilities
-        for some event to happen, we create and return the sub-population for
-        whom the event occurred.
+        target: str,
+        binned_column: str,
+        bins: List = (),
+        labels: List[str] = (),
+        target_type: str = "column",
+        **cut_kwargs,
+    ) -> None:
+        """Register a continuous `target` quantity to observe into bins in a `binned_column`.
 
         Parameters
         ----------
-        population
-            A view on the simulants for which we are determining the
-            outcome of an event.
-        probability
-            A 1d list of probabilities of the event under consideration
-            occurring which corresponds (i.e.
-            `len(population) == len(probability)` to the population view
-            passed in.
-        additional_key
-            Any additional information used to create the seed.
+        target
+            String name of the state table column or value pipeline used to stratify.
+        binned_column
+            String name of the column for the binned quantities.
+        bins
+            List of scalars defining the bin edges, passed to :meth: pandas.cut. Lists
+            `bins` and `labels` must be of equal length.
+        labels
+            List of string labels for bins. Lists `bins` and `labels` must be of equal length.
+        target_type
+            "column" or "value"
+        **cut_kwargs
+            Keyword arguments for :meth: pandas.cut.
 
         Returns
-        -------
-        pandas.core.generic.PandasObject
-            The sub-population of the simulants for whom the event occurred.
-            The return type will be the same as type(population)
-
+        ------
+        None
         """
-        return filter_for_probability(
-            self._key(additional_key), population, probability, self.index_map
+        self._manager.register_binned_stratification(
+            target, target_type, binned_column, bins, labels, **cut_kwargs
         )
 
-    def choice(
+    def register_observation(
         self,
-        index: pd.Index,
-        choices: Union[List, Tuple, np.ndarray, pd.Series],
-        p: Union[List, Tuple, np.ndarray, pd.Series] = None,
-        additional_key: Any = None,
-    ) -> pd.Series:
-        """Decides between a weighted or unweighted set of choices.
-
-        Given a set of choices with or without corresponding weights,
-        returns an indexed set of decisions from those choices. This is
-        simply a vectorized way to make decisions with some book-keeping.
+        name: str,
+        pop_filter: str = "",
+        aggregator_sources: List[str] = None,
+        aggregator: Callable[[pd.DataFrame], float] = len,
+        requires_columns: List[str] = (),
+        requires_values: List[str] = (),
+        additional_stratifications: List[str] = (),
+        excluded_stratifications: List[str] = (),
+        when: str = "collect_metrics",
+    ) -> None:
+        """Provide the results system all the information it needs to perform the observation.
 
         Parameters
         ----------
-        index
-            An index whose length is the number of random draws made
-            and which indexes the returned `pandas.Series`.
-        choices
-            A set of options to choose from.
-        p
-            The relative weights of the choices.  Can be either a 1-d array of
-            the same length as `choices` or a 2-d array with `len(index)` rows
-            and `len(choices)` columns.  In the 1-d case, the same set of
-            weights are used to decide among the choices for every item in
-            the `index`. In the 2-d case, each row in `p` contains a separate
-            set of weights for every item in the `index`.
-        additional_key
-            Any additional information used to seed random number generation.
+        name
+            String name for the observation.
+        pop_filter
+            A Pandas query filter string to filter the population down to the simulants who should
+            be considered for the observation.
+        aggregator_sources
+            A list of population view columns to be used in the aggregator.
+        aggregator
+            A function that computes the quantity for the observation.
+        requires_columns
+            A list of the state table columns that are required by either the pop_filter or the aggregator.
+        requires_values
+            A list of the value pipelines that are required by either the pop_filter or the aggregator.
+        additional_stratifications
+            A list of additional :class:`stratification <vivarium.framework.results.stratification.Stratification>`
+            names by which to stratify.
+        excluded_stratifications
+            A list of default :class:`stratification <vivarium.framework.results.stratification.Stratification>`
+            names to remove from the observation.
+        when
+            String name of the phase of a time-step the observation should happen. Valid values are:
+            `"time_step__prepare"`, `"time_step"`, `"time_step__cleanup"`, `"collect_metrics"`.
 
         Returns
-        -------
-        pandas.Series
-            An indexed set of decisions from among the available `choices`.
-
-        Raises
         ------
-        RandomnessError
-            If any row in `p` contains `RESIDUAL_CHOICE` and the remaining
-            weights in the row are not normalized or any row of `p contains
-            more than one reference to `RESIDUAL_CHOICE`.
-
+        None
         """
-        return choice(self._key(additional_key), index, choices, p, self.index_map)
-
-    def __repr__(self) -> str:
-        return "RandomnessStream(key={!r}, clock={!r}, seed={!r})".format(
-            self.key, self.clock(), self.seed
+        self._manager.register_observation(
+            name,
+            pop_filter,
+            aggregator_sources,
+            aggregator,
+            requires_columns,
+            requires_values,
+            additional_stratifications,
+            excluded_stratifications,
+            when,
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vivarium-1.0.4/src/vivarium/framework/resource.py` & `vivarium-1.1.0/src/vivarium/framework/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 dependencies or raise exceptions if this is not possible.
 
 """
 from types import MethodType
 from typing import Any, Callable, Iterable, List
 
 import networkx as nx
-from loguru import logger
 
 from vivarium.exceptions import VivariumError
 
 
 class ResourceError(VivariumError):
     """Error raised when a dependency requirement is violated."""
 
@@ -148,14 +147,17 @@
             except nx.NetworkXUnfeasible:
                 raise ResourceError(
                     f"The resource pool contains at least one cycle: "
                     f"{nx.find_cycle(self.graph)}."
                 )
         return self._sorted_nodes
 
+    def setup(self, builder):
+        self.logger = builder.logging.get_logger(self.name)
+
     def add_resources(
         self,
         resource_type: str,
         resource_names: List[str],
         producer: Any,
         dependencies: List[str],
     ):
@@ -246,15 +248,15 @@
         resource_graph.add_nodes_from(self._resource_group_map.values())
 
         for resource_group in resource_graph.nodes:
             for dependency in resource_group.dependencies:
                 if dependency not in self._resource_group_map:
                     # Warn here because this sometimes happens naturally
                     # if observer components are missing from a simulation.
-                    logger.warning(
+                    self.logger.warning(
                         f"Resource {dependency} is not provided by any component but is needed to "
                         f"compute {resource_group}."
                     )
                     continue
                 dependency_group = self._resource_group_map[dependency]
                 resource_graph.add_edge(dependency_group, resource_group)
```

### Comparing `vivarium-1.0.4/src/vivarium/framework/results/manager.py` & `vivarium-1.1.0/src/vivarium/framework/results/manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 
     @property
     def metrics(self):
         return self._metrics.copy()
 
     # noinspection PyAttributeOutsideInit
     def setup(self, builder: "Builder"):
+        self.logger = builder.logging.get_logger(self.name)
         self.population_view = builder.population.get_view([])
         self.clock = builder.time.clock()
         self.step_size = builder.time.step_size()
 
         builder.event.register_listener("time_step__prepare", self.on_time_step_prepare)
         builder.event.register_listener("time_step", self.on_time_step)
         builder.event.register_listener("time_step__cleanup", self.on_time_step_cleanup)
@@ -175,14 +176,15 @@
         aggregator: Callable,
         requires_columns: List[str] = (),
         requires_values: List[str] = (),
         additional_stratifications: List[str] = (),
         excluded_stratifications: List[str] = (),
         when: str = "collect_metrics",
     ) -> None:
+        self._warn_check_stratifications(additional_stratifications, excluded_stratifications)
         self._results_context.add_observation(
             name,
             pop_filter,
             aggregator_sources,
             aggregator,
             additional_stratifications,
             excluded_stratifications,
@@ -213,7 +215,31 @@
             population[pipeline.name] = pipeline(event.index)
         return population
 
     def get_results(self, index, metrics):
         # Shim for now to allow incremental transition to new results system.
         metrics.update(self.metrics)
         return metrics
+
+    def _warn_check_stratifications(
+        self, additional_stratifications, excluded_stratifications
+    ):
+        """Check additional and excluded stratifications if they'd not affect
+        stratifications (i.e., would be NOP), and emit warning."""
+        nop_additional = [
+            s
+            for s in additional_stratifications
+            if s in self._results_context.default_stratifications
+        ]
+        if len(nop_additional):
+            self.logger.warning(
+                f"Specified additional stratifications are already included by default: {nop_additional}",
+            )
+        nop_exclude = [
+            s
+            for s in excluded_stratifications
+            if s not in self._results_context.default_stratifications
+        ]
+        if len(nop_exclude):
+            self.logger.warning(
+                f"Specified excluded stratifications are already not included by default: {nop_exclude}",
+            )
```

### Comparing `vivarium-1.0.4/src/vivarium/framework/results/stratification.py` & `vivarium-1.1.0/src/vivarium/framework/results/stratification.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/src/vivarium/framework/state_machine.py` & `vivarium-1.1.0/src/vivarium/framework/state_machine.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/src/vivarium/framework/time.py` & `vivarium-1.1.0/src/vivarium/framework/time.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/src/vivarium/framework/utilities.py` & `vivarium-1.1.0/src/vivarium/framework/utilities.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,31 +5,34 @@
 
 Collection of utility functions shared by the ``vivarium`` framework.
 
 """
 import functools
 from bdb import BdbQuit
 from importlib import import_module
-from typing import Any, Callable
+from typing import Any, Callable, List, Tuple, Union
 
 import numpy as np
+import pandas as pd
 
 
 def from_yearly(value, time_step):
     return value * (time_step.total_seconds() / (60 * 60 * 24 * 365.0))
 
 
 def to_yearly(value, time_step):
     return value / (time_step.total_seconds() / (60 * 60 * 24 * 365.0))
 
 
-def rate_to_probability(rate):
+def rate_to_probability(rate: Union[float, List, Tuple, np.ndarray, pd.Series]) -> np.ndarray:
     # encountered underflow from rate > 30k
     # for rates greater than 250, exp(-rate) evaluates to 1e-109
     # beware machine-specific floating point issues
+
+    rate = np.array(rate)
     rate[rate > 250] = 250.0
     return 1 - np.exp(-rate)
 
 
 def probability_to_rate(probability):
     return -np.log(1 - probability)
```

### Comparing `vivarium-1.0.4/src/vivarium/framework/values.py` & `vivarium-1.1.0/src/vivarium/framework/values.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 """
 from collections import defaultdict
 from numbers import Number
 from typing import Any, Callable, Iterable, List, Tuple, Union
 
 import numpy as np
 import pandas as pd
-from loguru import logger
 
 from vivarium.exceptions import VivariumError
 from vivarium.framework.utilities import from_yearly
 
 # Supports standard algebraic operations with scalar values.
 NumberLike = Union[np.ndarray, pd.Series, pd.DataFrame, Number]
 
@@ -254,14 +253,15 @@
         self._pipelines = defaultdict(Pipeline)
 
     @property
     def name(self):
         return "values_manager"
 
     def setup(self, builder):
+        self.logger = builder.logging.get_logger(self.name)
         self.step_size = builder.time.step_size()
         builder.event.register_listener("post_setup", self.on_post_setup)
 
         self.resources = builder.resources
         self.add_constraint = builder.lifecycle.add_constraint
 
         builder.lifecycle.add_constraint(self.register_value_producer, allow_during=["setup"])
@@ -269,15 +269,15 @@
 
     def on_post_setup(self, _):
         """Finalizes dependency structure for the pipelines."""
         # Unsourced pipelines might occur when generic components register
         # modifiers to values that aren't required in a simulation.
         unsourced_pipelines = [p for p, v in self._pipelines.items() if not v.source]
         if unsourced_pipelines:
-            logger.warning(f"Unsourced pipelines: {unsourced_pipelines}")
+            self.logger.warning(f"Unsourced pipelines: {unsourced_pipelines}")
 
         # register_value_producer and register_value_modifier record the
         # dependency structure for the pipeline source and pipeline modifiers,
         # respectively.  We don't have enough information to record the
         # dependency structure for the pipeline itself until now, where
         # we say the pipeline value depends on its source and all its
         # modifiers.
@@ -331,15 +331,15 @@
         self,
         value_name: str,
         source: Callable,
         preferred_combiner: Callable,
         preferred_post_processor: Callable,
     ):
         """Configure the named value pipeline with a source, combiner, and post-processor."""
-        logger.debug(f"Registering value pipeline {value_name}")
+        self.logger.debug(f"Registering value pipeline {value_name}")
         pipeline = self._pipelines[value_name]
         if pipeline.source:
             raise DynamicValueError(
                 f"A second component is attempting to set the source for pipeline {value_name} "
                 f"with {source}, but it already has a source: {pipeline.source}."
             )
         pipeline.name = value_name
@@ -385,15 +385,15 @@
         """
         modifier_name = self._get_modifier_name(modifier)
 
         pipeline = self._pipelines[value_name]  # May create a pipeline
         pipeline.mutators.append(modifier)
 
         name = f"{value_name}.{len(pipeline.mutators)}.{modifier_name}"
-        logger.debug(f"Registering {name} as modifier to {value_name}")
+        self.logger.debug(f"Registering {name} as modifier to {value_name}")
         dependencies = self._convert_dependencies(
             modifier, requires_columns, requires_values, requires_streams
         )
         self.resources.add_resources("value_modifier", [name], modifier, dependencies)
 
     def get_value(self, name):
         """Retrieve the pipeline representing the named value.
```

### Comparing `vivarium-1.0.4/src/vivarium/interface/cli.py` & `vivarium-1.1.0/src/vivarium/interface/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     *   - Name
         - Description
     *   - | **run**
         - | Runs a single simulation from a model specification file.
     *   - | **test**
         - | Runs an example simulation that comes packaged with ``vivarium``.
-           | Useful as an installation test.
+          | Useful as an installation test.
     *   - | **profile**
         - | Produces a profile of a simulation using the python
           | :mod:`cProfile` module
 
 For more information, see the :ref:`tutorial <cli_tutorial>` on running
 simulations from the command line.
 
@@ -38,21 +38,21 @@
 
 import click
 import pandas as pd
 from loguru import logger
 
 from vivarium.examples import disease_model
 from vivarium.framework.engine import run_simulation
-from vivarium.framework.utilities import handle_exceptions
-
-from .utilities import (
+from vivarium.framework.logging import (
     configure_logging_to_file,
     configure_logging_to_terminal,
-    get_output_root,
 )
+from vivarium.framework.utilities import handle_exceptions
+
+from .utilities import get_output_root
 
 
 @click.group()
 def simulate():
     """A command line utility for running a single simulation.
 
     You may initiate a new run with the ``run`` sub-command, initiate a test
@@ -77,47 +77,64 @@
     "--results_directory",
     "-o",
     type=click.Path(resolve_path=True),
     default=Path("~/vivarium_results/").expanduser(),
     help="The directory to write results to. A folder will be created "
     "in this directory with the same name as the configuration file.",
 )
-@click.option("--verbose", "-v", is_flag=True, help="Report each time step.")
+@click.option(
+    "--verbose",
+    "-v",
+    is_flag=True,
+    help="Logs verbosely. Useful for debugging and development.",
+)
+@click.option(
+    "--quiet",
+    "-q",
+    is_flag=True,
+    help="Suppresses all logging except for warnings and errors.",
+)
 @click.option(
     "--pdb",
     "with_debugger",
     is_flag=True,
     help="Drop into python debugger if an error occurs.",
 )
 def run(
     model_specification: Path,
     location: str,
     artifact_path: Path,
     results_directory: Path,
-    verbose: int,
+    verbose: bool,
+    quiet: bool,
     with_debugger: bool,
 ):
     """Run a simulation from the command line.
 
     The simulation itself is defined by the given MODEL_SPECIFICATION yaml file.
 
     Within the results directory, which defaults to ~/vivarium_results if none
     is provided, a subdirectory will be created with the same name as the
     MODEL_SPECIFICATION if one does not exist. Results will be written to a
-    further subdirectory named after the start time of the simulation run."""
-    configure_logging_to_terminal(verbose)
+    further subdirectory named after the start time of the simulation run.
+
+    """
+    if verbose and quiet:
+        raise click.UsageError("Cannot be both verbose and quiet.")
+    verbosity = 1 + int(verbose) - int(quiet)
+    configure_logging_to_terminal(verbosity=verbosity, long_format=False)
 
     start = time()
 
     results_root = get_output_root(results_directory, model_specification, artifact_path)
     # Update permissions mask (assign to variable to avoid printing previous value)
     _ = os.umask(0o002)
     results_root.mkdir(parents=True, exist_ok=False)
 
-    configure_logging_to_file(results_root)
+    configure_logging_to_file(output_directory=results_root)
     shutil.copy(model_specification, results_root / "model_specification.yaml")
 
     output_data = {"results_directory": str(results_root)}
     input_data = {}
     if location:
         input_data["location"] = location
     if artifact_path:
@@ -135,56 +152,57 @@
 
 
 @simulate.command()
 def test():
     """Run a test simulation using the ``disease_model.yaml`` model specification
     provided in the examples directory.
     """
-    configure_logging_to_terminal(verbose=True)
+    configure_logging_to_terminal(verbosity=2, long_format=False)
     model_specification = disease_model.get_model_specification_path()
 
     main = handle_exceptions(run_simulation, logger, with_debugger=False)
 
     main(model_specification)
     click.echo()
     click.secho("Installation test successful!", fg="green")
 
 
 @simulate.command()
 @click.argument(
-    "model_specification", type=click.Path(exists=True, dir_okay=False, resolve_path=True)
+    "model_specification",
+    type=click.Path(exists=True, dir_okay=False, resolve_path=True),
 )
 @click.option(
     "--results_directory",
     "-o",
     type=click.Path(resolve_path=True),
     default=Path("~/vivarium_results/").expanduser(),
-    help="The directory to write results to. A folder will be created "
-    "in this directory with the same name as the configuration file.",
+    help=(
+        "The directory to write results to. A folder will be created "
+        "in this directory with the same name as the configuration file."
+    ),
 )
 @click.option(
     "--process/--no-process",
     default=False,
     help=(
         "Automatically process the profile to human readable format  with pstats, "
         "sorted by cumulative runtime, and dump to a file"
     ),
 )
 def profile(model_specification, results_directory, process):
-    """Run a simulation based on the provided MODEL_SPECIFICATION and profile
-    the run.
-    """
+    """Run a simulation based on the provided MODEL_SPECIFICATION and profile the run."""
     model_specification = Path(model_specification)
     results_directory = Path(results_directory)
 
     out_stats_file = results_directory / f"{model_specification.name}".replace(
         "yaml", "stats"
     )
     command = f'run_simulation("{model_specification}")'
-    cProfile.runctx(command, globals=globals(), locals=locals(), filename=out_stats_file)
+    cProfile.runctx(command, globals=globals(), locals=locals(), filename=str(out_stats_file))
 
     if process:
         out_txt_file = results_directory / (out_stats_file.name + ".txt")
         with out_txt_file.open("w") as f:
             p = pstats.Stats(str(out_stats_file), stream=f)
             p.sort_stats("cumulative")
             p.print_stats()
```

### Comparing `vivarium-1.0.4/src/vivarium/interface/interactive.py` & `vivarium-1.1.0/src/vivarium/interface/interactive.py`

 * *Files 10% similar despite different names*

```diff
@@ -230,9 +230,25 @@
         Returns
         -------
             A component that has the name ``name`` else None.
 
         """
         return self._component_manager.get_component(name)
 
+    def print_initializer_order(self):
+        """Print the order in which population initializers are called."""
+        initializers = []
+        for r in self._resource:
+            name = r.__name__
+            if hasattr(r, "__self__"):
+                obj = r.__self__
+                initializers.append(f"{obj.__class__.__name__}({obj.name}).{name}")
+            else:
+                initializers.append(f"Unbound function {name}")
+        print("\n".join(initializers))
+
+    def print_lifecycle_order(self):
+        """Print the order of lifecycle events (including user event handlers)."""
+        print(self._lifecycle)
+
     def __repr__(self):
         return "InteractiveContext()"
```

### Comparing `vivarium-1.0.4/src/vivarium/interface/utilities.py` & `vivarium-1.1.0/src/vivarium/interface/utilities.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,21 +4,19 @@
 ===========================
 
 The functions defined here are used to support the interactive and command-line
 interfaces for ``vivarium``.
 
 """
 import functools
-import sys
 from datetime import datetime
 from pathlib import Path
 from typing import Union
 
 import yaml
-from loguru import logger
 
 from vivarium.exceptions import VivariumError
 
 
 def run_from_ipython() -> bool:
     """Taken from https://stackoverflow.com/questions/5376837/how-can-i-do-an-if-run-from-ipython-test-in-python"""
     try:
@@ -120,14 +118,15 @@
     model_spec_path
         Path to the model specification file. This must exist.
 
     Returns
     -------
     str
         A model name string for use in output labeling.
+
     """
     if artifact_path:
         model_name = Path(artifact_path).stem
     else:
         with open(model_spec_path) as model_spec_file:
             model_spec = yaml.safe_load(model_spec_file)
         try:
@@ -142,33 +141,7 @@
     model_specification_file: Union[str, Path],
     artifact_path: Union[str, Path],
 ):
     launch_time = datetime.now().strftime("%Y_%m_%d_%H_%M_%S")
     model_name = get_output_model_name_string(artifact_path, model_specification_file)
     output_root = Path(results_directory + f"/{model_name}/{launch_time}")
     return output_root
-
-
-def add_logging_sink(sink, verbose, colorize=False, serialize=False):
-    message_format = (
-        "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | "
-        "<cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> "
-        "- <level>{message}</level>"
-    )
-    if verbose:
-        logger.add(
-            sink, colorize=colorize, level="DEBUG", format=message_format, serialize=serialize
-        )
-    else:
-        logger.add(
-            sink, colorize=colorize, level="ERROR", format=message_format, serialize=serialize
-        )
-
-
-def configure_logging_to_terminal(verbose):
-    logger.remove(0)  # Clear default configuration
-    add_logging_sink(sys.stdout, verbose, colorize=True)
-
-
-def configure_logging_to_file(output_directory):
-    master_log = output_directory / "simulation.log"
-    add_logging_sink(master_log, verbose=True)
```

### Comparing `vivarium-1.0.4/src/vivarium/interpolation.py` & `vivarium-1.1.0/src/vivarium/interpolation.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
         data: pd.DataFrame,
         categorical_parameters: Union[List[str], Tuple[str]],
         continuous_parameters: ParameterType,
         order: int,
         extrapolate: bool,
         validate: bool,
     ):
-
         # TODO: allow for order 1 interpolation with binned edges
         if order != 0:
             raise NotImplementedError(
                 f"Interpolation is only supported for order 0. You specified order {order}"
             )
 
         if validate:
@@ -237,15 +236,14 @@
         n_p_total = len(set(data[p[0]]))
 
         # TODO: fix rather than suppress this FutureWarning
         with warnings.catch_warnings():
             warnings.simplefilter(action="ignore", category=FutureWarning)
             sub_tables = list(sub_tables)
         for _, table in sub_tables:
-
             param_data = table[[p[0], p[1]]].copy().sort_values(by=p[0])
             start, end = param_data[p[0]].reset_index(drop=True), param_data[
                 p[1]
             ].reset_index(drop=True)
 
             if len(set(start)) < n_p_total:
                 raise ValueError(
```

### Comparing `vivarium-1.0.4/src/vivarium/testing_utilities.py` & `vivarium-1.1.0/src/vivarium/testing_utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 """
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 
 from vivarium.framework import randomness
+from vivarium.framework.randomness.index_map import IndexMap
 
 
 class NonCRNTestPopulation:
-
     configuration_defaults = {
         "population": {
             "age_start": 0,
             "age_end": 100,
             "exit_age": None,
         },
     }
@@ -27,15 +27,15 @@
     @property
     def name(self):
         return "non_crn_test_population"
 
     def setup(self, builder):
         self.config = builder.configuration
         self.randomness = builder.randomness.get_stream(
-            "population_age_fuzz", for_initialization=True
+            "population_age_fuzz", initializes_crn_attributes=True
         )
         columns = ["age", "sex", "location", "alive", "entrance_time", "exit_time"]
         self.population_view = builder.population.get_view(columns)
 
         builder.population.initializes_simulants(
             self.generate_test_population, creates_columns=columns
         )
@@ -68,15 +68,15 @@
     @property
     def name(self):
         return "test_population"
 
     def setup(self, builder):
         super().setup(builder)
         self.age_randomness = builder.randomness.get_stream(
-            "age_initialization", for_initialization=True
+            "age_initialization", initializes_crn_attributes=True
         )
         self.register = builder.randomness.register_simulants
 
     def generate_test_population(self, pop_data):
         age_start = pop_data.user_data.get("age_start", self.config.population.age_start)
         age_end = pop_data.user_data.get("age_end", self.config.population.age_end)
         age_draw = self.age_randomness.get_draw(pop_data.index)
@@ -191,21 +191,28 @@
         def __repr__(self):
             return f"dummy_column(name={name}, initial_value={initial_value})"
 
     return DummyColumnMaker()
 
 
 def get_randomness(
-    key="test", clock=lambda: pd.Timestamp(1990, 7, 2), seed=12345, for_initialization=False
+    key="test",
+    clock=lambda: pd.Timestamp(1990, 7, 2),
+    seed=12345,
+    initializes_crn_attributes=False,
 ):
     return randomness.RandomnessStream(
-        key, clock, seed=seed, for_initialization=for_initialization
+        key,
+        clock,
+        seed=seed,
+        index_map=IndexMap(),
+        initializes_crn_attributes=initializes_crn_attributes,
     )
 
 
 def reset_mocks(mocks):
     for mock in mocks:
         mock.reset_mock()
 
 
-def metadata(file_path):
-    return {"layer": "override", "source": str(Path(file_path).resolve())}
+def metadata(file_path, layer="override"):
+    return {"layer": layer, "source": str(Path(file_path).resolve())}
```

### Comparing `vivarium-1.0.4/src/vivarium.egg-info/PKG-INFO` & `vivarium-1.1.0/src/vivarium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vivarium
-Version: 1.0.4
+Version: 1.1.0
 Summary: vivarium is a microsimulation framework built on top of the standard scientific python stack.
 Home-page: https://github.com/ihmeuw/vivarium
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `vivarium-1.0.4/src/vivarium.egg-info/SOURCES.txt` & `vivarium-1.1.0/src/vivarium.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -35,19 +35,21 @@
 docs/source/api_reference/framework/artifact/artifact.rst
 docs/source/api_reference/framework/artifact/hdf.rst
 docs/source/api_reference/framework/artifact/index.rst
 docs/source/api_reference/framework/artifact/manager.rst
 docs/source/api_reference/framework/components/index.rst
 docs/source/api_reference/framework/components/manager.rst
 docs/source/api_reference/framework/components/parser.rst
+docs/source/api_reference/framework/logging/index.rst
+docs/source/api_reference/framework/logging/manager.rst
+docs/source/api_reference/framework/logging/utilities.rst
 docs/source/api_reference/framework/population/exceptions.rst
 docs/source/api_reference/framework/population/index.rst
 docs/source/api_reference/framework/population/manager.rst
 docs/source/api_reference/framework/population/population_view.rst
-docs/source/api_reference/framework/randomness/core.rst
 docs/source/api_reference/framework/randomness/exceptions.rst
 docs/source/api_reference/framework/randomness/index.rst
 docs/source/api_reference/framework/randomness/index_map.rst
 docs/source/api_reference/framework/randomness/manager.rst
 docs/source/api_reference/framework/randomness/stream.rst
 docs/source/api_reference/interface/cli.rst
 docs/source/api_reference/interface/index.rst
@@ -59,14 +61,15 @@
 docs/source/concepts/crn.rst
 docs/source/concepts/data.rst
 docs/source/concepts/entry_points.rst
 docs/source/concepts/event.rst
 docs/source/concepts/index.rst
 docs/source/concepts/interpolation.rst
 docs/source/concepts/lifecycle.rst
+docs/source/concepts/logging.rst
 docs/source/concepts/lookup.rst
 docs/source/concepts/population.rst
 docs/source/concepts/resource.rst
 docs/source/concepts/time.rst
 docs/source/concepts/values.rst
 docs/source/concepts/model_specification/index.rst
 docs/source/concepts/model_specification/yaml_basics.rst
@@ -126,20 +129,22 @@
 src/vivarium/framework/artifact/__init__.py
 src/vivarium/framework/artifact/artifact.py
 src/vivarium/framework/artifact/hdf.py
 src/vivarium/framework/artifact/manager.py
 src/vivarium/framework/components/__init__.py
 src/vivarium/framework/components/manager.py
 src/vivarium/framework/components/parser.py
+src/vivarium/framework/logging/__init__.py
+src/vivarium/framework/logging/manager.py
+src/vivarium/framework/logging/utilities.py
 src/vivarium/framework/population/__init__.py
 src/vivarium/framework/population/exceptions.py
 src/vivarium/framework/population/manager.py
 src/vivarium/framework/population/population_view.py
 src/vivarium/framework/randomness/__init__.py
-src/vivarium/framework/randomness/core.py
 src/vivarium/framework/randomness/exceptions.py
 src/vivarium/framework/randomness/index_map.py
 src/vivarium/framework/randomness/manager.py
 src/vivarium/framework/randomness/stream.py
 src/vivarium/framework/results/__init__.py
 src/vivarium/framework/results/context.py
 src/vivarium/framework/results/exceptions.py
@@ -159,15 +164,14 @@
 tests/framework/__init__.py
 tests/framework/test_configuration.py
 tests/framework/test_engine.py
 tests/framework/test_event.py
 tests/framework/test_lifecycle.py
 tests/framework/test_lookup.py
 tests/framework/test_plugins.py
-tests/framework/test_randomness.py
 tests/framework/test_resource.py
 tests/framework/test_state_machine.py
 tests/framework/test_utilities.py
 tests/framework/test_values.py
 tests/framework/artifact/__init__.py
 tests/framework/artifact/test_artifact.py
 tests/framework/artifact/test_hdf.py
@@ -177,15 +181,15 @@
 tests/framework/components/test_manager.py
 tests/framework/components/test_parser.py
 tests/framework/population/__init__.py
 tests/framework/population/test_manager.py
 tests/framework/population/test_population_view.py
 tests/framework/randomness/__init__.py
 tests/framework/randomness/conftest.py
-tests/framework/randomness/test_core.py
+tests/framework/randomness/test_crn.py
 tests/framework/randomness/test_index_map.py
 tests/framework/randomness/test_manager.py
 tests/framework/randomness/test_stream.py
 tests/framework/results/__init__.py
 tests/framework/results/mocks.py
 tests/framework/results/test_context.py
 tests/framework/results/test_interface.py
```

### Comparing `vivarium-1.0.4/tests/config_tree/test_basic_functionality.py` & `vivarium-1.1.0/tests/config_tree/test_basic_functionality.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/tests/config_tree/test_ingestion.py` & `vivarium-1.1.0/tests/config_tree/test_ingestion.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/tests/conftest.py` & `vivarium-1.1.0/tests/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 from pathlib import Path
 
 import pytest
 import tables
+from _pytest.logging import LogCaptureFixture
+from loguru import logger
 
 from vivarium.framework.configuration import (
     build_model_specification,
     build_simulation_configuration,
 )
 from vivarium.testing_utilities import metadata
 
 
 @pytest.fixture
+def caplog(caplog: LogCaptureFixture):
+    handler_id = logger.add(caplog.handler, format="{message}")
+    yield caplog
+    logger.remove(handler_id)
+
+
+@pytest.fixture
 def base_config():
     config = build_simulation_configuration()
     config.update(
         {
             "time": {
                 "start": {
                     "year": 1990,
                 },
                 "end": {"year": 2010},
                 "step_size": 30.5,
-            }
+            },
+            "randomness": {"key_columns": ["entrance_time", "age"]},
         },
-        **metadata(__file__),
+        **metadata(__file__, layer="model_override"),
     )
     return config
 
 
 @pytest.fixture
 def test_data_dir():
     data_dir = Path(__file__).resolve().parent / "test_data"
```

### Comparing `vivarium-1.0.4/tests/framework/artifact/test_artifact.py` & `vivarium-1.1.0/tests/framework/artifact/test_artifact.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/tests/framework/artifact/test_hdf.py` & `vivarium-1.1.0/tests/framework/artifact/test_hdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,15 +321,14 @@
     assert key.group_name == name
     assert key.group == f"/{type_}/{name}"
     assert key.path == f"/{type_}/{name}/{measure}"
     assert key.with_measure("prevalence") == hdf.EntityKey(f"{type_}.{name}.prevalence")
 
 
 def test_entity_key_equality():
-
     type_ = "cause"
     name = "diarrheal_diseases"
     measure = "incidence"
     string = f"{type_}.{name}.{measure}"
     key = hdf.EntityKey(string)
 
     class NonString:
```

### Comparing `vivarium-1.0.4/tests/framework/artifact/test_manager.py` & `vivarium-1.1.0/tests/framework/artifact/test_manager.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/tests/framework/components/mocks.py` & `vivarium-1.1.0/tests/framework/components/mocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         return metrics
 
     def __eq__(self, other):
         return type(self) == type(other) and self.name == other.name
 
 
 class MockGenericComponent:
-
     configuration_defaults = {
         "component": {
             "key1": "val",
             "key2": {
                 "subkey1": "val",
                 "subkey2": "val",
             },
```

### Comparing `vivarium-1.0.4/tests/framework/components/test_manager.py` & `vivarium-1.1.0/tests/framework/components/test_manager.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/tests/framework/components/test_parser.py` & `vivarium-1.1.0/tests/framework/components/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,14 @@
 def import_and_instantiate_mock(mocker):
     return mocker.patch(
         "vivarium.framework.components.parser.import_and_instantiate_components"
     )
 
 
 def test_parse_component_config(components):
-
     source = yaml.full_load(components)["components"]
     component_list = parse_component_config_to_list(source)
     assert set(TEST_COMPONENTS_PARSED) == set(component_list)
 
 
 def test_prep_components():
     desc = 'cave_system.monsters.Rabbit("timid", "squeak")'
```

### Comparing `vivarium-1.0.4/tests/framework/population/test_manager.py` & `vivarium-1.1.0/tests/framework/population/test_manager.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/tests/framework/population/test_population_view.py` & `vivarium-1.1.0/tests/framework/population/test_population_view.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/tests/framework/randomness/conftest.py` & `vivarium-1.1.0/tests/framework/randomness/conftest.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/tests/framework/randomness/test_index_map.py` & `vivarium-1.1.0/tests/framework/randomness/test_index_map.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,128 +14,129 @@
     s = list(iterable)
     return list(chain.from_iterable(combinations(s, r) for r in range(1, len(s) + 1)))
 
 
 def generate_keys(number, types=("int", "float", "datetime"), seed=123456):
     rs = np.random.RandomState(seed=seed)
 
-    index = []
+    keys = {}
     if "datetime" in types:
         year = rs.choice(np.arange(1980, 2018))
         day = rs.choice(pd.date_range(f"01/01/{year}", periods=365))
         start_time = rs.choice(pd.date_range(day, periods=86400, freq="s"))
         freq = rs.choice(["ms", "s", "min", "h"])
-        index.append(pd.date_range(start_time, periods=number, freq=freq))
+        keys["datetime"] = pd.date_range(start_time, periods=number, freq=freq)
 
     if "int" in types:
         kind = rs.choice(["random", "sequential"])
         if kind == "random":
             ints = np.unique(rs.randint(0, 1000 * number, size=100 * number))
             assert len(ints) > number
             rs.shuffle(ints)
-            index.append(ints[:number])
+            keys["int"] = ints[:number]
         else:
             start = rs.randint(0, 100 * number)
-            index.append(np.arange(start, start + number, dtype=int))
+            keys["int"] = np.arange(start, start + number, dtype=int)
 
     if "float" in types:
-        index.append(rs.random_sample(size=number))
+        keys["float"] = rs.random_sample(size=number)
 
-    return pd.Series(0, index=index).index
+    return pd.DataFrame(keys, index=pd.RangeIndex(number))
 
 
 rs = np.random.RandomState(seed=456789)
 index_sizes = list(rs.randint(10_000, 250_000, size=1))
 types = list(almost_powerset(["int", "float", "datetime"]))
 seeds = list(rs.randint(10000000, size=1))
 
 
 def id_fun(param):
     return f"Size:{param[0]}, Types:{param[1]}, Seed:{param[2]}"
 
 
 @pytest.fixture(scope="module", params=list(product(index_sizes, types, seeds)), ids=id_fun)
 def map_size_and_hashed_values(request):
-    keys = generate_keys(*request.param)
-    m = IndexMap()
-    return m.map_size, m.hash_(keys)
+    index_size, types_, seed = request.param
+    keys = generate_keys(*request.param).set_index(types_).index
+    m = IndexMap(key_columns=types_)
+    return len(m), m._hash(keys)
 
 
 def test_digit_scalar():
     m = IndexMap()
     k = 123456789
     for i in range(10):
-        assert m.digit(k, i) == 10 - (i + 1)
+        assert m._digit(k, i) == 10 - (i + 1)
 
 
 def test_digit_series():
     m = IndexMap()
     k = pd.Series(123456789, index=range(10000))
     for i in range(10):
-        assert len(m.digit(k, i).unique()) == 1
-        assert m.digit(k, i)[0] == 10 - (i + 1)
+        assert len(m._digit(k, i).unique()) == 1
+        assert m._digit(k, i)[0] == 10 - (i + 1)
 
 
 def test_clip_to_seconds_scalar():
     m = IndexMap()
     k = pd.to_datetime("2010-01-25 06:25:31.123456789")
-    assert m.clip_to_seconds(k.value) == int(str(k.value)[:10])
+    assert m._clip_to_seconds(k.value) == int(str(k.value)[:10])
 
 
 def test_clip_to_seconds_series():
     m = IndexMap()
     stamp = 1234567890
     k = (
         pd.date_range(pd.to_datetime(stamp, unit="s"), periods=10000, freq="ns")
         .to_series()
         .view(np.int64)
     )
-    assert len(m.clip_to_seconds(k).unique()) == 1
-    assert m.clip_to_seconds(k).unique()[0] == stamp
+    assert len(m._clip_to_seconds(k).unique()) == 1
+    assert m._clip_to_seconds(k).unique()[0] == stamp
 
 
 def test_spread_scalar():
     m = IndexMap()
-    assert m.spread(1234567890) == 4072825790
+    assert m._spread(1234567890) == 4072825790
 
 
 def test_spread_series():
     m = IndexMap()
     s = pd.Series(1234567890, index=range(10000))
-    assert len(m.spread(s).unique()) == 1
-    assert m.spread(s).unique()[0] == 4072825790
+    assert len(m._spread(s).unique()) == 1
+    assert m._spread(s).unique()[0] == 4072825790
 
 
 def test_shift_scalar():
     m = IndexMap()
-    assert m.shift(1.1234567890) == 1234567890
+    assert m._shift(1.1234567890) == 1234567890
 
 
 def test_shift_series():
     m = IndexMap()
     s = pd.Series(1.1234567890, index=range(10000))
-    assert len(m.shift(s).unique()) == 1
-    assert m.shift(s).unique()[0] == 1234567890
+    assert len(m._shift(s).unique()) == 1
+    assert m._shift(s).unique()[0] == 1234567890
 
 
 def test_convert_to_ten_digit_int():
     m = IndexMap()
     v = 1234567890
     datetime_col = pd.date_range(
         pd.to_datetime(v, unit="s"), periods=10000, freq="ns"
     ).to_series()
     int_col = pd.Series(v, index=range(10000))
     float_col = pd.Series(1.1234567890, index=range(10000))
     bad_col = pd.Series("a", index=range(10000))
 
-    assert m.convert_to_ten_digit_int(datetime_col).unique()[0] == v
-    assert m.convert_to_ten_digit_int(int_col).unique()[0] == 4072825790
-    assert m.convert_to_ten_digit_int(float_col).unique()[0] == v
+    assert m._convert_to_ten_digit_int(datetime_col).unique()[0] == v
+    assert m._convert_to_ten_digit_int(int_col).unique()[0] == 4072825790
+    assert m._convert_to_ten_digit_int(float_col).unique()[0] == v
     with pytest.raises(RandomnessError):
-        m.convert_to_ten_digit_int(bad_col)
+        m._convert_to_ten_digit_int(bad_col)
 
 
 @pytest.mark.skip("This fails because the hash needs work")
 def test_hash_collisions(map_size_and_hashed_values):
     n, h = map_size_and_hashed_values
     k = len(h)
 
@@ -160,35 +161,62 @@
     binned_data = pd.cut(h, bins)
     distribution = pd.value_counts(binned_data).sort_index()
     c, p = chisquare(distribution)
 
     assert p > 0.05, "Data not uniform"
 
 
-def test_update(mocker):
-    m = IndexMap()
-    keys = generate_keys(10000)
+@pytest.fixture(scope="function")
+def index_map(mocker):
+    mock_index_map = IndexMap
 
     def hash_mock(k, salt=0):
         seed = 123456
         rs = np.random.RandomState(seed=seed + salt)
         return pd.Series(rs.randint(0, len(k) * 10, size=len(k)), index=k)
 
-    mocker.patch.object(m, "hash_", side_effect=hash_mock)
+    mocker.patch.object(mock_index_map, "_hash", side_effect=hash_mock)
+
+    return mock_index_map
+
+
+def test_update_empty_bad_keys(index_map):
+    keys = pd.DataFrame({"A": ["a"] * 10}, index=range(10))
+    m = index_map(key_columns=list(keys.columns))
+    with pytest.raises(RandomnessError):
+        m.update(keys)
+
+
+def test_update_nonempty_bad_keys(index_map):
+    keys = generate_keys(1000)
+    m = index_map(key_columns=list(keys.columns))
+    m.update(keys)
+    with pytest.raises(RandomnessError):
+        m.update(keys)
+
+
+def test_update_empty_good_keys(index_map):
+    keys = generate_keys(1000)
+    m = index_map(key_columns=list(keys.columns))
     m.update(keys)
-    assert len(m) == len(keys), "All keys not in mapping"
-    assert m._map.index.difference(keys).empty, "All keys not in mapping"
+    key_index = keys.set_index(list(keys.columns)).index
+    assert len(m._map) == len(keys), "All keys not in mapping"
+    assert (
+        m._map.index.droplevel(m.SIM_INDEX_COLUMN).difference(key_index).empty
+    ), "Extra keys in mapping"
     assert len(m._map.unique()) == len(keys), "Duplicate values in mapping"
 
-    # Can't have duplicate keys.
-    with pytest.raises(KeyError):
-        m.update(keys)
 
-    new_unique_keys = generate_keys(1000).difference(keys)
-    m.update(new_unique_keys)
-    assert len(m) == len(keys) + len(new_unique_keys), "All keys not in mapping"
-    assert m._map.index.difference(
-        keys.union(new_unique_keys)
-    ).empty, "All keys not in mapping"
-    assert len(m._map.unique()) == len(keys) + len(
-        new_unique_keys
-    ), "Duplicate values in mapping"
+def test_update_nonempty_good_keys(index_map):
+    keys = generate_keys(2000)
+    m = index_map(key_columns=list(keys.columns))
+    keys1, keys2 = keys[:1000], keys[1000:]
+
+    m.update(keys1)
+    m.update(keys2)
+
+    key_index = keys.set_index(list(keys.columns)).index
+    assert len(m._map) == len(keys), "All keys not in mapping"
+    assert (
+        m._map.index.droplevel(m.SIM_INDEX_COLUMN).difference(key_index).empty
+    ), "Extra keys in mapping"
+    assert len(m._map.unique()) == len(keys), "Duplicate values in mapping"
```

### Comparing `vivarium-1.0.4/tests/framework/results/mocks.py` & `vivarium-1.1.0/tests/framework/results/mocks.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/tests/framework/results/test_context.py` & `vivarium-1.1.0/tests/framework/results/test_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,19 +25,19 @@
         (NAME, SOURCES, CATEGORIES, sorting_hat_serial, False),
     ],
     ids=["vectorized_mapper", "non-vectorized_mapper"],
 )
 def test_add_stratification(name, sources, categories, mapper, is_vectorized):
     ctx = ResultsContext()
     assert not verify_stratification_added(
-        ctx._stratifications, name, sources, categories, mapper, is_vectorized
+        ctx.stratifications, name, sources, categories, mapper, is_vectorized
     )
     ctx.add_stratification(name, sources, categories, mapper, is_vectorized)
     assert verify_stratification_added(
-        ctx._stratifications, name, sources, categories, mapper, is_vectorized
+        ctx.stratifications, name, sources, categories, mapper, is_vectorized
     )
 
 
 @pytest.mark.parametrize(
     "name, sources, categories, mapper, is_vectorized, expected_exception",
     [
         (  # sources not in population columns
@@ -102,25 +102,25 @@
     ids=["valid_on_collect_metrics", "valid_on_time_step__prepare"],
 )
 def test_add_observation(
     name, pop_filter, aggregator, additional_stratifications, excluded_stratifications, when
 ):
     ctx = ResultsContext()
     ctx._default_stratifications = ["age", "sex"]
-    assert len(ctx._observations) == 0
+    assert len(ctx.observations) == 0
     ctx.add_observation(
         name,
         pop_filter,
         [],
         aggregator,
         additional_stratifications,
         excluded_stratifications,
         when,
     )
-    assert len(ctx._observations) == 1
+    assert len(ctx.observations) == 1
 
 
 @pytest.mark.parametrize(
     "name, pop_filter, aggregator, additional_stratifications, excluded_stratifications, when",
     [
         (
             "living_person_time",
@@ -136,15 +136,15 @@
 def test_double_add_observation(
     name, pop_filter, aggregator, additional_stratifications, excluded_stratifications, when
 ):
     """Tests a double add of the same stratification, this should result in one additional observation being added to
     the context."""
     ctx = ResultsContext()
     ctx._default_stratifications = ["age", "sex"]
-    assert len(ctx._observations) == 0
+    assert len(ctx.observations) == 0
     ctx.add_observation(
         name,
         pop_filter,
         [],
         aggregator,
         additional_stratifications,
         excluded_stratifications,
@@ -155,43 +155,15 @@
         pop_filter,
         [],
         aggregator,
         additional_stratifications,
         excluded_stratifications,
         when,
     )
-    assert len(ctx._observations) == 1
-
-
-@pytest.mark.parametrize(
-    "default, additional, excluded, match",
-    [
-        (["age", "sex"], ["age"], [], "age"),
-        (["age", "sex"], [], ["eye_color"], "eye_color"),
-        (["age", "sex"], ["age"], ["eye_color"], "age|eye_color"),
-    ],
-    ids=[
-        "additional_no_operation",
-        "exclude_no_operation",
-        "additional_and_exclude_no_operation",
-    ],
-)
-def test_add_observation_nop_stratifications(default, additional, excluded, match):
-    ctx = ResultsContext()
-    ctx._default_stratifications = default
-    with pytest.warns(UserWarning, match=match):
-        ctx.add_observation(
-            "name",
-            'alive == "alive"',
-            [],
-            _aggregate_state_person_time,
-            additional,
-            excluded,
-            "collect_metrics",
-        )
+    assert len(ctx.observations) == 1
 
 
 @pytest.mark.parametrize(
     "default_stratifications, additional_stratifications, excluded_stratifications, expected_stratifications",
     [
         ([], [], [], ()),
         (["age", "sex"], ["handedness"], ["age"], ("sex", "handedness")),
@@ -209,15 +181,15 @@
     default_stratifications,
     additional_stratifications,
     excluded_stratifications,
     expected_stratifications,
 ):
     ctx = ResultsContext()
     # default_stratifications would normally be set via ResultsInterface.set_default_stratifications()
-    ctx._default_stratifications = default_stratifications
+    ctx.default_stratifications = default_stratifications
     stratifications = ctx._get_stratifications(
         additional_stratifications, excluded_stratifications
     )
     assert sorted(stratifications) == sorted(expected_stratifications)
 
 
 @pytest.mark.parametrize(
@@ -370,14 +342,34 @@
 
     for r in ctx.gather_results(population, event_name):
         unladen_results = {k: v for (k, v) in r.items() if "unladen_swallow" in k}
         assert len(unladen_results.items()) > 0
         assert all(v == 0 for v in unladen_results.values())
 
 
+def test_gather_results_with_empty_pop_filter():
+    """Test case where pop_filter filters to an empty population. gather_results should return an empty dict"""
+    ctx = ResultsContext()
+
+    # Generate population DataFrame
+    population = BASE_POPULATION.copy()
+
+    event_name = "collect_metrics"
+    ctx.add_observation(
+        name="wizard_count",
+        pop_filter="house == 'durmstrang'",
+        aggregator_sources=None,
+        aggregator=len,
+        event_name=event_name,
+    )
+
+    for result in ctx.gather_results(population, event_name):
+        assert len(result) == 0
+
+
 def test__format_results():
     """Test that format results produces the expected number of keys and a specific expected key"""
     ctx = ResultsContext()
     aggregates = BASE_POPULATION.groupby(["house", "familiar"]).apply(len)
     measure = "wizard_count"
     rv = ctx._format_results(measure, aggregates)
```

### Comparing `vivarium-1.0.4/tests/framework/results/test_interface.py` & `vivarium-1.1.0/tests/framework/results/test_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,62 +72,62 @@
     mgr = ResultsManager()
     interface = ResultsInterface(mgr)
     builder = mocker.Mock()
     # Set up mock builder with mocked get_value call for Pipelines
     mocker.patch.object(builder, "value.get_value")
     builder.value.get_value = MethodType(mock_get_value, builder)
     mgr.setup(builder)
-    assert len(interface._manager._results_context._observations) == 0
+    assert len(interface._manager._results_context.observations) == 0
     interface.register_observation(
         name,
         pop_filter,
         aggregator_columns,
         aggregator,
         requires_columns,
         requires_values,
         additional_stratifications,
         excluded_stratifications,
     )
-    assert len(interface._manager._results_context._observations) == 1
+    assert len(interface._manager._results_context.observations) == 1
 
 
 def test_register_observations():
     mgr = ResultsManager()
     interface = ResultsInterface(mgr)
-    assert len(interface._manager._results_context._observations) == 0
+    assert len(interface._manager._results_context.observations) == 0
     interface.register_observation(
         "living_person_time",
         'alive == "alive" and undead == False',
         [],
         _silly_aggregator,
         [],
         [],
         [],
         [],
         "collect_metrics",
     )
-    assert len(interface._manager._results_context._observations) == 1
+    assert len(interface._manager._results_context.observations) == 1
     interface.register_observation(
         "undead_person_time",
         "undead == True",
         [],
         _silly_aggregator,
         [],
         [],
         [],
         [],
         "time_step__prepare",
     )
-    assert len(interface._manager._results_context._observations) == 2
+    assert len(interface._manager._results_context.observations) == 2
 
 
 def test_unhashable_pipeline():
     mgr = ResultsManager()
     interface = ResultsInterface(mgr)
-    assert len(interface._manager._results_context._observations) == 0
+    assert len(interface._manager._results_context.observations) == 0
     with pytest.raises(TypeError, match="unhashable"):
         interface.register_observation(
             "living_person_time",
             'alive == "alive" and undead == False',
             [],
             _silly_aggregator,
             [],
```

### Comparing `vivarium-1.0.4/tests/framework/results/test_stratification.py` & `vivarium-1.1.0/tests/framework/results/test_stratification.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/tests/framework/test_configuration.py` & `vivarium-1.1.0/tests/framework/test_configuration.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/tests/framework/test_engine.py` & `vivarium-1.1.0/tests/framework/test_engine.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 
 from vivarium.framework.artifact import ArtifactInterface, ArtifactManager
 from vivarium.framework.components import (
     ComponentInterface,
     ComponentManager,
     OrderedComponentSet,
 )
-from vivarium.framework.engine import Builder, SimulationContext
+from vivarium.framework.engine import Builder
+from vivarium.framework.engine import SimulationContext as SimulationContext_
 from vivarium.framework.event import EventInterface, EventManager
 from vivarium.framework.lifecycle import LifeCycleInterface, LifeCycleManager
+from vivarium.framework.logging import LoggingInterface, LoggingManager
 from vivarium.framework.lookup import LookupTableInterface, LookupTableManager
 from vivarium.framework.metrics import Metrics
 from vivarium.framework.population import PopulationInterface, PopulationManager
 from vivarium.framework.randomness import RandomnessInterface, RandomnessManager
 from vivarium.framework.resource import ResourceInterface, ResourceManager
 from vivarium.framework.results import ResultsInterface, ResultsManager
 from vivarium.framework.time import DateTimeClock, TimeInterface
@@ -21,31 +23,47 @@
 from .components.mocks import Listener, MockComponentA, MockComponentB
 
 
 def is_same_object_method(m1, m2):
     return m1.__func__ is m2.__func__ and m1.__self__ is m2.__self__
 
 
+@pytest.fixture()
+def SimulationContext():
+    yield SimulationContext_
+    SimulationContext_._clear_context_cache()
+
+
 @pytest.fixture
 def components():
     return [
         MockComponentA("gretchen", "whimsy"),
         Listener("listener"),
         MockComponentB("spoon", "antelope", 23),
     ]
 
 
 @pytest.fixture
 def log(mocker):
-    return mocker.patch("vivarium.framework.engine.logger")
+    return mocker.patch("vivarium.framework.logging.manager.logger")
+
+
+def test_SimulationContext_get_sim_name(SimulationContext):
+    assert SimulationContext._created_simulation_contexts == set()
+
+    assert SimulationContext._get_context_name(None) == "simulation_1"
+    assert SimulationContext._get_context_name("foo") == "foo"
 
+    assert SimulationContext._created_simulation_contexts == {"simulation_1", "foo"}
 
-def test_SimulationContext_init_default(components):
+
+def test_SimulationContext_init_default(SimulationContext, components):
     sim = SimulationContext(components=components)
 
+    assert isinstance(sim._logging, LoggingManager)
     assert isinstance(sim._lifecycle, LifeCycleManager)
     assert isinstance(sim._component_manager, ComponentManager)
     assert isinstance(sim._clock, DateTimeClock)
     assert isinstance(sim._values, ValuesManager)
     assert isinstance(sim._events, EventManager)
     assert isinstance(sim._population, PopulationManager)
     assert isinstance(sim._resource, ResourceManager)
@@ -53,14 +71,16 @@
     assert isinstance(sim._tables, LookupTableManager)
     assert isinstance(sim._randomness, RandomnessManager)
     assert isinstance(sim._data, ArtifactManager)
 
     assert isinstance(sim._builder, Builder)
     assert sim._builder.configuration is sim.configuration
 
+    assert isinstance(sim._builder.logging, LoggingInterface)
+    assert sim._builder.logging._manager is sim._logging
     assert isinstance(sim._builder.lookup, LookupTableInterface)
     assert sim._builder.lookup._manager is sim._tables
     assert isinstance(sim._builder.value, ValuesInterface)
     assert sim._builder.value._manager is sim._values
     assert isinstance(sim._builder.event, EventInterface)
     assert sim._builder.event._manager is sim._events
     assert isinstance(sim._builder.population, PopulationInterface)
@@ -78,14 +98,15 @@
     assert isinstance(sim._builder.lifecycle, LifeCycleInterface)
     assert sim._builder.lifecycle._manager is sim._lifecycle
     assert isinstance(sim._builder.data, ArtifactInterface)
     assert sim._builder.data._manager is sim._data
 
     # Ordering matters.
     managers = [
+        sim._logging,
         sim._clock,
         sim._lifecycle,
         sim._resource,
         sim._values,
         sim._population,
         sim._randomness,
         sim._events,
@@ -99,15 +120,35 @@
         unpacked_components.append(c)
         if hasattr(c, "sub_components"):
             unpacked_components.extend(c.sub_components)
     assert list(sim._component_manager._components)[:-1] == unpacked_components
     assert isinstance(list(sim._component_manager._components)[-1], Metrics)
 
 
-def test_SimulationContext_setup_default(base_config, components):
+def test_SimulationContext_name_management(SimulationContext):
+    assert SimulationContext._created_simulation_contexts == set()
+
+    sim1 = SimulationContext()
+    assert sim1._name == "simulation_1"
+    assert SimulationContext._created_simulation_contexts == {"simulation_1"}
+
+    sim2 = SimulationContext(sim_name="foo")
+    assert sim2._name == "foo"
+    assert SimulationContext._created_simulation_contexts == {"simulation_1", "foo"}
+
+    sim3 = SimulationContext()
+    assert sim3._name == "simulation_3"
+    assert SimulationContext._created_simulation_contexts == {
+        "simulation_1",
+        "foo",
+        "simulation_3",
+    }
+
+
+def test_SimulationContext_setup_default(SimulationContext, base_config, components):
     sim = SimulationContext(base_config, components)
     listener = [c for c in components if "listener" in c.args][0]
     assert not listener.post_setup_called
     sim.setup()
 
     unpacked_components = []
     for c in components:
@@ -136,26 +177,26 @@
     assert is_same_object_method(
         sim.end_emitter, sim._events._event_types["simulation_end"].emit
     )
 
     assert listener.post_setup_called
 
 
-def test_SimulationContext_initialize_simulants(base_config, components):
+def test_SimulationContext_initialize_simulants(SimulationContext, base_config, components):
     sim = SimulationContext(base_config, components)
     sim.setup()
     pop_size = sim.configuration.population.population_size
     current_time = sim._clock.time
     assert sim._population.get_population(True).empty
     sim.initialize_simulants()
     assert len(sim._population.get_population(True)) == pop_size
     assert sim._clock.time == current_time
 
 
-def test_SimulationContext_step(log, base_config, components):
+def test_SimulationContext_step(SimulationContext, log, base_config, components):
     sim = SimulationContext(base_config, components)
     sim.setup()
     sim.initialize_simulants()
 
     current_time = sim._clock.time
     step_size = sim._clock.step_size
 
@@ -173,26 +214,26 @@
     assert listener.time_step_called
     assert listener.time_step__cleanup_called
     assert listener.collect_metrics_called
 
     assert sim._clock.time == current_time + step_size
 
 
-def test_SimulationContext_finalize(base_config, components):
+def test_SimulationContext_finalize(SimulationContext, base_config, components):
     sim = SimulationContext(base_config, components)
     listener = [c for c in components if "listener" in c.args][0]
     sim.setup()
     sim.initialize_simulants()
     sim.step()
     assert not listener.simulation_end_called
     sim.finalize()
     assert listener.simulation_end_called
 
 
-def test_SimulationContext_report(base_config, components):
+def test_SimulationContext_report(SimulationContext, base_config, components):
     sim = SimulationContext(base_config, components)
     sim.setup()
     sim.initialize_simulants()
     sim.run()
     sim.finalize()
     metrics = sim.report()
     assert metrics["test"] == len(
```

### Comparing `vivarium-1.0.4/tests/framework/test_event.py` & `vivarium-1.1.0/tests/framework/test_event.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/tests/framework/test_lifecycle.py` & `vivarium-1.1.0/tests/framework/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/tests/framework/test_lookup.py` & `vivarium-1.1.0/tests/framework/test_lookup.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/tests/framework/test_plugins.py` & `vivarium-1.1.0/tests/framework/test_plugins.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/tests/framework/test_resource.py` & `vivarium-1.1.0/tests/framework/test_resource.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/tests/framework/test_state_machine.py` & `vivarium-1.1.0/tests/framework/test_state_machine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import numpy as np
 import pandas as pd
 
 from vivarium import InteractiveContext
-from vivarium.framework.randomness import choice
 from vivarium.framework.state_machine import Machine, State, Transition
 
 
 def _population_fixture(column, initial_value):
     class PopFixture:
         @property
         def name(self):
@@ -25,19 +24,20 @@
 def _even_population_fixture(column, values):
     class pop_fixture:
         @property
         def name(self):
             return "test_pop_fixture"
 
         def setup(self, builder):
+            self.randomness = builder.randomness.get_stream(self.name)
             self.population_view = builder.population.get_view([column])
             builder.population.initializes_simulants(self.inner, creates_columns=[column])
 
         def inner(self, pop_data):
-            self.population_view.update(choice("start", pop_data.index, values))
+            self.population_view.update(self.randomness.choice(pop_data.index, values))
 
     return pop_fixture()
 
 
 def test_transition():
     done_state = State("done")
     start_state = State("start")
@@ -49,15 +49,17 @@
     )
     event_time = simulation._clock.time + simulation._clock.step_size
     machine.transition(simulation.get_population().index, event_time)
     assert np.all(simulation.get_population().state == "done")
 
 
 def test_choice(base_config):
-    base_config.update({"population": {"population_size": 10000}})
+    base_config.update(
+        {"population": {"population_size": 10000}, "randomness": {"key_columns": []}}
+    )
     a_state = State("a")
     b_state = State("b")
     start_state = State("start")
     start_state.add_transition(
         a_state, probability_func=lambda agents: np.full(len(agents), 0.5)
     )
     start_state.add_transition(
@@ -71,15 +73,17 @@
     event_time = simulation._clock.time + simulation._clock.step_size
     machine.transition(simulation.get_population().index, event_time)
     a_count = (simulation.get_population().state == "a").sum()
     assert round(a_count / len(simulation.get_population()), 1) == 0.5
 
 
 def test_null_transition(base_config):
-    base_config.update({"population": {"population_size": 10000}})
+    base_config.update(
+        {"population": {"population_size": 10000}, "randomness": {"key_columns": []}}
+    )
     a_state = State("a")
     start_state = State("start")
     start_state.add_transition(
         a_state, probability_func=lambda agents: np.full(len(agents), 0.5)
     )
     start_state.allow_self_transitions()
 
@@ -91,15 +95,17 @@
     event_time = simulation._clock.time + simulation._clock.step_size
     machine.transition(simulation.get_population().index, event_time)
     a_count = (simulation.get_population().state == "a").sum()
     assert round(a_count / len(simulation.get_population()), 1) == 0.5
 
 
 def test_no_null_transition(base_config):
-    base_config.update({"population": {"population_size": 10000}})
+    base_config.update(
+        {"population": {"population_size": 10000}, "randomness": {"key_columns": []}}
+    )
     a_state = State("a")
     b_state = State("b")
     start_state = State("start")
     a_transition = Transition(
         start_state, a_state, probability_func=lambda index: pd.Series(0.5, index=index)
     )
     b_transition = Transition(
```

### Comparing `vivarium-1.0.4/tests/framework/test_utilities.py` & `vivarium-1.1.0/tests/framework/test_utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,20 @@
 
 def test_rate_to_probability():
     rate = np.array([0.001])
     prob = rate_to_probability(rate)
     assert np.isclose(prob, 0.00099950016662497809)
 
 
+def test_very_high_rate_to_probability():
+    rate = np.array([10_000])
+    prob = rate_to_probability(rate)
+    assert np.isclose(prob, 1.0)
+
+
 def test_probability_to_rate():
     prob = np.array([0.00099950016662497809])
     rate = probability_to_rate(prob)
     assert np.isclose(rate, 0.001)
 
 
 def test_rate_to_probability_symmetry():
```

### Comparing `vivarium-1.0.4/tests/framework/test_values.py` & `vivarium-1.1.0/tests/framework/test_values.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/tests/interface/test_utilities.py` & `vivarium-1.1.0/tests/interface/test_utilities.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.0.4/tests/test_interpolation.py` & `vivarium-1.1.0/tests/test_interpolation.py`

 * *Files identical despite different names*

