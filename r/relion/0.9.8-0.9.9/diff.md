# Comparing `tmp/relion-0.9.8.tar.gz` & `tmp/relion-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relion-0.9.8.tar", last modified: Fri Feb  4 13:20:01 2022, max compression
+gzip compressed data, was "relion-0.9.9.tar", last modified: Tue Feb  8 14:20:20 2022, max compression
```

## Comparing `relion-0.9.8.tar` & `relion-0.9.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-04 13:20:01.663048 relion-0.9.8/
--rw-r--r--   0 vsts      (1001) docker     (121)    17222 2022-02-04 13:19:47.000000 relion-0.9.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)     2644 2022-02-04 13:20:01.663048 relion-0.9.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1667 2022-02-04 13:19:47.000000 relion-0.9.8/README.rst
--rw-r--r--   0 vsts      (1001) docker     (121)      130 2022-02-04 13:19:47.000000 relion-0.9.8/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (121)     2324 2022-02-04 13:20:01.663048 relion-0.9.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)      154 2022-02-04 13:19:47.000000 relion-0.9.8/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-04 13:20:01.659048 relion-0.9.8/src/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-04 13:20:01.659048 relion-0.9.8/src/relion/
--rw-r--r--   0 vsts      (1001) docker     (121)    12622 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-04 13:20:01.659048 relion-0.9.8/src/relion/_parser/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/_parser/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5604 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/_parser/autopick.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8600 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/_parser/class2D.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10229 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/_parser/class3D.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6562 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/_parser/cryolo.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4703 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/_parser/ctffind.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2580 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/_parser/initialmodel.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3198 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/_parser/jobtype.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8229 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/_parser/motioncorrection.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4632 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/_parser/processgraph.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2693 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/_parser/processnode.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3581 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/_parser/relativeicethickness.py
--rw-r--r--   0 vsts      (1001) docker     (121)    16041 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/_parser/relion_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-04 13:20:01.663048 relion-0.9.8/src/relion/cli/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      953 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/cli/current_job.py
--rw-r--r--   0 vsts      (1001) docker     (121)      708 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/cli/pipeline_viewer.py
--rw-r--r--   0 vsts      (1001) docker     (121)      576 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/cli/print_default_options.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2095 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/cli/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-04 13:20:01.663048 relion-0.9.8/src/relion/cryolo_relion_it/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/cryolo_relion_it/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     8293 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/cryolo_relion_it/cryolo_external_job.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     7663 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/cryolo_relion_it/cryolo_fine_tune_job.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)   167851 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/cryolo_relion_it/cryolo_relion_it.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2337 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/cryolo_relion_it/dls_options.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     3321 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/cryolo_relion_it/fsc_fitting_external_job.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2700 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/cryolo_relion_it/icebreaker_histogram.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     2386 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/cryolo_relion_it/mask_soft_edge_external_job.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     3988 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/cryolo_relion_it/reconstruct_halves_external_job.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     3046 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/cryolo_relion_it/select_and_split_external_job.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-04 13:20:01.663048 relion-0.9.8/src/relion/dbmodel/
--rw-r--r--   0 vsts      (1001) docker     (121)     5170 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/dbmodel/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1404 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/dbmodel/dbgraph.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7703 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/dbmodel/dbnode.py
--rw-r--r--   0 vsts      (1001) docker     (121)    13296 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/dbmodel/modeltables.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-04 13:20:01.663048 relion-0.9.8/src/relion/node/
--rw-r--r--   0 vsts      (1001) docker     (121)     5389 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/node/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5547 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/node/environment.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8500 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/node/graph.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4432 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/parse_project.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-04 13:20:01.663048 relion-0.9.8/src/relion/zocalo/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/zocalo/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3132 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/zocalo/alchemy.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4218 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/zocalo/images_service_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1956 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/zocalo/service.py
--rw-r--r--   0 vsts      (1001) docker     (121)    30719 2022-02-04 13:19:47.000000 relion-0.9.8/src/relion/zocalo/wrapper.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-04 13:20:01.659048 relion-0.9.8/src/relion.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     2644 2022-02-04 13:20:01.000000 relion-0.9.8/src/relion.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1832 2022-02-04 13:20:01.000000 relion-0.9.8/src/relion.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-02-04 13:20:01.000000 relion-0.9.8/src/relion.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      918 2022-02-04 13:20:01.000000 relion-0.9.8/src/relion.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-02-04 13:20:01.000000 relion-0.9.8/src/relion.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (121)       58 2022-02-04 13:20:01.000000 relion-0.9.8/src/relion.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        7 2022-02-04 13:20:01.000000 relion-0.9.8/src/relion.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-08 14:20:20.531698 relion-0.9.9/
+-rw-r--r--   0 vsts      (1001) docker     (121)    17222 2022-02-08 14:20:13.000000 relion-0.9.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (121)     2644 2022-02-08 14:20:20.531698 relion-0.9.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     1667 2022-02-08 14:20:13.000000 relion-0.9.9/README.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)      130 2022-02-08 14:20:13.000000 relion-0.9.9/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (121)     2324 2022-02-08 14:20:20.531698 relion-0.9.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (121)      154 2022-02-08 14:20:13.000000 relion-0.9.9/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-08 14:20:20.519698 relion-0.9.9/src/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-08 14:20:20.523698 relion-0.9.9/src/relion/
+-rw-r--r--   0 vsts      (1001) docker     (121)    12622 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-08 14:20:20.523698 relion-0.9.9/src/relion/_parser/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/_parser/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5604 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/_parser/autopick.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8600 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/_parser/class2D.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10229 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/_parser/class3D.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6562 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/_parser/cryolo.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4703 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/_parser/ctffind.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2580 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/_parser/initialmodel.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3198 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/_parser/jobtype.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8229 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/_parser/motioncorrection.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4632 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/_parser/processgraph.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2693 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/_parser/processnode.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3581 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/_parser/relativeicethickness.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    16041 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/_parser/relion_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-08 14:20:20.531698 relion-0.9.9/src/relion/cli/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      953 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/cli/current_job.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      708 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/cli/pipeline_viewer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      576 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/cli/print_default_options.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2095 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/cli/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-08 14:20:20.531698 relion-0.9.9/src/relion/cryolo_relion_it/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/cryolo_relion_it/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     8538 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/cryolo_relion_it/cryolo_external_job.py
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     7663 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/cryolo_relion_it/cryolo_fine_tune_job.py
+-rwxr-xr-x   0 vsts      (1001) docker     (121)   167985 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/cryolo_relion_it/cryolo_relion_it.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2337 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/cryolo_relion_it/dls_options.py
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     3321 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/cryolo_relion_it/fsc_fitting_external_job.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2700 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/cryolo_relion_it/icebreaker_histogram.py
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     2386 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/cryolo_relion_it/mask_soft_edge_external_job.py
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     3988 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/cryolo_relion_it/reconstruct_halves_external_job.py
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     3046 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/cryolo_relion_it/select_and_split_external_job.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-08 14:20:20.531698 relion-0.9.9/src/relion/dbmodel/
+-rw-r--r--   0 vsts      (1001) docker     (121)     5170 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/dbmodel/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1404 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/dbmodel/dbgraph.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7703 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/dbmodel/dbnode.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    13296 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/dbmodel/modeltables.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-08 14:20:20.531698 relion-0.9.9/src/relion/node/
+-rw-r--r--   0 vsts      (1001) docker     (121)     5389 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/node/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5547 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/node/environment.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8500 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/node/graph.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4432 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/parse_project.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-08 14:20:20.531698 relion-0.9.9/src/relion/zocalo/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/zocalo/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3132 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/zocalo/alchemy.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4218 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/zocalo/images_service_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1956 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/zocalo/service.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    30719 2022-02-08 14:20:13.000000 relion-0.9.9/src/relion/zocalo/wrapper.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-02-08 14:20:20.523698 relion-0.9.9/src/relion.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2644 2022-02-08 14:20:20.000000 relion-0.9.9/src/relion.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     1832 2022-02-08 14:20:20.000000 relion-0.9.9/src/relion.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-02-08 14:20:20.000000 relion-0.9.9/src/relion.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      918 2022-02-08 14:20:20.000000 relion-0.9.9/src/relion.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-02-08 14:20:20.000000 relion-0.9.9/src/relion.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (121)       58 2022-02-08 14:20:20.000000 relion-0.9.9/src/relion.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        7 2022-02-08 14:20:20.000000 relion-0.9.9/src/relion.egg-info/top_level.txt
```

### Comparing `relion-0.9.8/LICENSE` & `relion-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/PKG-INFO` & `relion-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relion
-Version: 0.9.8
+Version: 0.9.9
 Summary: Relion Python API
 Home-page: UNKNOWN
 Author: Diamond Light Source - Scientific Software et al.
 Author-email: scientificsoftware@diamond.ac.uk
 License: GPLv2
 Project-URL: Documentation, https://python-relion.readthedocs.io/
 Project-URL: GitHub, https://github.com/DiamondLightSource/python-relion
```

### Comparing `relion-0.9.8/README.rst` & `relion-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/setup.cfg` & `relion-0.9.9/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = relion
-version = 0.9.8
+version = 0.9.9
 description = Relion Python API
 long_description = file: README.rst
 author = Diamond Light Source - Scientific Software et al.
 author_email = scientificsoftware@diamond.ac.uk
 license = GPLv2
 license_file = LICENSE
 classifiers =
```

### Comparing `relion-0.9.8/src/relion/__init__.py` & `relion-0.9.9/src/relion/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from relion.node.graph import Graph
 
 logger = logging.getLogger("relion.Project")
 
 __all__ = []
 __author__ = "Diamond Light Source - Scientific Software"
 __email__ = "scientificsoftware@diamond.ac.uk"
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 __version_tuple__ = tuple(int(x) for x in __version__.split("."))
 
 pipeline_lock = ".relion_lock"
 
 
 RelionJobResult = namedtuple(
     "RelionJobResult",
```

### Comparing `relion-0.9.8/src/relion/_parser/autopick.py` & `relion-0.9.9/src/relion/_parser/autopick.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/_parser/class2D.py` & `relion-0.9.9/src/relion/_parser/class2D.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/_parser/class3D.py` & `relion-0.9.9/src/relion/_parser/class3D.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/_parser/cryolo.py` & `relion-0.9.9/src/relion/_parser/cryolo.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/_parser/ctffind.py` & `relion-0.9.9/src/relion/_parser/ctffind.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/_parser/initialmodel.py` & `relion-0.9.9/src/relion/_parser/initialmodel.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/_parser/jobtype.py` & `relion-0.9.9/src/relion/_parser/jobtype.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/_parser/motioncorrection.py` & `relion-0.9.9/src/relion/_parser/motioncorrection.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/_parser/processgraph.py` & `relion-0.9.9/src/relion/_parser/processgraph.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/_parser/processnode.py` & `relion-0.9.9/src/relion/_parser/processnode.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/_parser/relativeicethickness.py` & `relion-0.9.9/src/relion/_parser/relativeicethickness.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/_parser/relion_pipeline.py` & `relion-0.9.9/src/relion/_parser/relion_pipeline.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/cli/current_job.py` & `relion-0.9.9/src/relion/cli/current_job.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/cli/pipeline_viewer.py` & `relion-0.9.9/src/relion/cli/pipeline_viewer.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/cli/print_default_options.py` & `relion-0.9.9/src/relion/cli/print_default_options.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/cli/run_pipeline.py` & `relion-0.9.9/src/relion/cli/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/cryolo_relion_it/cryolo_external_job.py` & `relion-0.9.9/src/relion/cryolo_relion_it/cryolo_external_job.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,20 @@
     )
     parser.add_argument("--box_size", help="Size of box (~ particle size)")
     parser.add_argument("--threshold", help="Threshold for picking (default = 0.3)")
     parser.add_argument("--in_model", help="model from previous job")
     parser.add_argument("--gmodel", help="cryolo general model")
     parser.add_argument("--config", help="cryolo config")
     parser.add_argument("--gpu", help='GPUs to use (e.g. "0 1 2 3")')
+    parser.add_argument(
+        "--from_movies",
+        type=int,
+        help="Whether or not initial images were movies",
+        default=1,
+    )
     args = parser.parse_args(args_list)
     thresh = args.threshold
     box_size = args.box_size
     gen_model = args.gmodel
     conf_file = args.config
     gpus = args.gpu
 
@@ -144,26 +150,27 @@
     output_nodes_block = out_doc.add_new_block("output_nodes")
     loop = output_nodes_block.init_loop(
         "", ["_rlnPipeLineNodeName", "_rlnPipeLineNodeType"]
     )
     loop.add_row([os.path.join(job_dir, "coords_suffix_autopick.star"), "2"])
     out_doc.write_file("RELION_OUTPUT_NODES.star")
     ctf_star = os.path.join(project_dir, args.in_mics)
-    correct_paths(ctf_star)
+    path_drop = 2 if args.from_movies else 0
+    correct_paths(ctf_star, path_drop=path_drop)
 
 
-def correct_paths(ctf_star):
+def correct_paths(ctf_star, path_drop: int = 2):
     in_doc = gemmi.cif.read_file(ctf_star)
     data_as_dict = json.loads(in_doc.as_json())["micrographs"]
 
     for i in range(len(data_as_dict["_rlnmicrographname"])):
         name = data_as_dict["_rlnmicrographname"][i]
         dirs, mic_file = os.path.split(name)
         full_dir = ""
-        for d in dirs.split("/")[2:]:
+        for d in dirs.split("/")[path_drop:]:
             full_dir = os.path.join(full_dir, d)
         os.makedirs(full_dir, exist_ok=True)
         picked_star = os.path.splitext(mic_file)[0] + "_autopick.star"
         try:
             shutil.move(
                 os.path.join("picked_stars", picked_star),
                 os.path.join(full_dir, picked_star),
```

### Comparing `relion-0.9.8/src/relion/cryolo_relion_it/cryolo_fine_tune_job.py` & `relion-0.9.9/src/relion/cryolo_relion_it/cryolo_fine_tune_job.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/cryolo_relion_it/cryolo_relion_it.py` & `relion-0.9.9/src/relion/cryolo_relion_it/cryolo_relion_it.py`

 * *Files 0% similar despite different names*

```diff
@@ -2577,14 +2577,16 @@
                     f"Param2 - value: == {opts.cryolo_threshold}",
                     "Param3 - label: == gmodel",
                     f"Param3 - value: == {opts.cryolo_gmodel}",
                     "Param4 - label: == config",
                     f"Param4 - value: == {opts.cryolo_config}",
                     "Param5 - label: == gpu",
                     f'Param5 - value: == "{opts.cryolo_pick_gpus}"',
+                    "Param6 - label: == from_movies",
+                    f"Param6 - value: == {1 if opts.images_are_movies else 0}",
                 ]
 
                 # TODO: fix fine tune for running as External job
                 # if os.path.isfile(
                 #         os.path.join(
                 #             CRYOLO_FINETUNE_JOB_DIR,
                 #             cryolo_external_job.RELION_JOB_SUCCESS_FILENAME
```

### Comparing `relion-0.9.8/src/relion/cryolo_relion_it/dls_options.py` & `relion-0.9.9/src/relion/cryolo_relion_it/dls_options.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/cryolo_relion_it/fsc_fitting_external_job.py` & `relion-0.9.9/src/relion/cryolo_relion_it/fsc_fitting_external_job.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/cryolo_relion_it/icebreaker_histogram.py` & `relion-0.9.9/src/relion/cryolo_relion_it/icebreaker_histogram.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/cryolo_relion_it/mask_soft_edge_external_job.py` & `relion-0.9.9/src/relion/cryolo_relion_it/mask_soft_edge_external_job.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/cryolo_relion_it/reconstruct_halves_external_job.py` & `relion-0.9.9/src/relion/cryolo_relion_it/reconstruct_halves_external_job.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/cryolo_relion_it/select_and_split_external_job.py` & `relion-0.9.9/src/relion/cryolo_relion_it/select_and_split_external_job.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/dbmodel/__init__.py` & `relion-0.9.9/src/relion/dbmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/dbmodel/dbgraph.py` & `relion-0.9.9/src/relion/dbmodel/dbgraph.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/dbmodel/dbnode.py` & `relion-0.9.9/src/relion/dbmodel/dbnode.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/dbmodel/modeltables.py` & `relion-0.9.9/src/relion/dbmodel/modeltables.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/node/__init__.py` & `relion-0.9.9/src/relion/node/__init__.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/node/environment.py` & `relion-0.9.9/src/relion/node/environment.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/node/graph.py` & `relion-0.9.9/src/relion/node/graph.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/parse_project.py` & `relion-0.9.9/src/relion/parse_project.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/zocalo/alchemy.py` & `relion-0.9.9/src/relion/zocalo/alchemy.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/zocalo/images_service_plugin.py` & `relion-0.9.9/src/relion/zocalo/images_service_plugin.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/zocalo/service.py` & `relion-0.9.9/src/relion/zocalo/service.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion/zocalo/wrapper.py` & `relion-0.9.9/src/relion/zocalo/wrapper.py`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion.egg-info/PKG-INFO` & `relion-0.9.9/src/relion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relion
-Version: 0.9.8
+Version: 0.9.9
 Summary: Relion Python API
 Home-page: UNKNOWN
 Author: Diamond Light Source - Scientific Software et al.
 Author-email: scientificsoftware@diamond.ac.uk
 License: GPLv2
 Project-URL: Documentation, https://python-relion.readthedocs.io/
 Project-URL: GitHub, https://github.com/DiamondLightSource/python-relion
```

### Comparing `relion-0.9.8/src/relion.egg-info/SOURCES.txt` & `relion-0.9.9/src/relion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `relion-0.9.8/src/relion.egg-info/entry_points.txt` & `relion-0.9.9/src/relion.egg-info/entry_points.txt`

 * *Files identical despite different names*

