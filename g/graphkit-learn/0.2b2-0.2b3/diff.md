# Comparing `tmp/graphkit-learn-0.2b2.tar.gz` & `tmp/graphkit-learn-0.2b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/graphkit-learn-0.2b2.tar", last modified: Tue May 26 15:54:00 2020, max compression
+gzip compressed data, was "dist/graphkit-learn-0.2b3.tar", last modified: Fri Sep 25 16:44:08 2020, max compression
```

## Comparing `graphkit-learn-0.2b2.tar` & `graphkit-learn-0.2b3.tar`

### file list

```diff
@@ -1,78 +1,125 @@
-drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-05-26 15:54:00.000000 graphkit-learn-0.2b2/
-drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-05-26 15:54:00.000000 graphkit-learn-0.2b2/gklearn/
-drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-05-26 15:54:00.000000 graphkit-learn-0.2b2/gklearn/ged/
-drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-05-26 15:54:00.000000 graphkit-learn-0.2b2/gklearn/ged/env/
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)      444 2020-04-30 08:29:35.000000 graphkit-learn-0.2b2/gklearn/ged/env/common_types.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)     2133 2020-05-26 08:16:34.000000 graphkit-learn-0.2b2/gklearn/ged/env/node_map.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)      100 2020-04-22 09:54:13.000000 graphkit-learn-0.2b2/gklearn/ged/env/__init__.py
-drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-05-26 15:54:00.000000 graphkit-learn-0.2b2/gklearn/ged/median/
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    64121 2020-05-26 09:25:48.000000 graphkit-learn-0.2b2/gklearn/ged/median/median_graph_estimator.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)     5758 2020-05-07 14:15:17.000000 graphkit-learn-0.2b2/gklearn/ged/median/test_median_graph_estimator.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)     2593 2020-05-26 09:27:51.000000 graphkit-learn-0.2b2/gklearn/ged/median/utils.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)      155 2020-04-11 12:31:35.000000 graphkit-learn-0.2b2/gklearn/ged/median/__init__.py
-drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-05-26 15:54:00.000000 graphkit-learn-0.2b2/gklearn/ged/util/
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)     4279 2020-04-11 12:31:35.000000 graphkit-learn-0.2b2/gklearn/ged/util/cpp2python.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)     3446 2020-04-11 12:31:35.000000 graphkit-learn-0.2b2/gklearn/ged/util/misc.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    12367 2020-05-26 08:49:49.000000 graphkit-learn-0.2b2/gklearn/ged/util/util.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)       70 2020-04-11 12:31:35.000000 graphkit-learn-0.2b2/gklearn/ged/util/__init__.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-04-13 15:52:46.000000 graphkit-learn-0.2b2/gklearn/ged/__init__.py
-drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-05-26 15:54:00.000000 graphkit-learn-0.2b2/gklearn/gedlib/
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)      425 2020-04-11 12:31:36.000000 graphkit-learn-0.2b2/gklearn/gedlib/librariesImport.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)     1355 2020-04-11 12:31:36.000000 graphkit-learn-0.2b2/gklearn/gedlib/setup.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)     4819 2020-04-11 12:31:36.000000 graphkit-learn-0.2b2/gklearn/gedlib/test.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)      120 2020-04-11 12:31:35.000000 graphkit-learn-0.2b2/gklearn/gedlib/__init__.py
-drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-05-26 15:54:00.000000 graphkit-learn-0.2b2/gklearn/kernels/
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    14817 2020-03-05 10:47:39.000000 graphkit-learn-0.2b2/gklearn/kernels/commonWalkKernel.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)     5894 2020-05-12 10:18:14.000000 graphkit-learn-0.2b2/gklearn/kernels/graph_kernel.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    11526 2020-03-10 13:22:28.000000 graphkit-learn-0.2b2/gklearn/kernels/marginalizedKernel.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    20004 2020-04-23 16:39:41.000000 graphkit-learn-0.2b2/gklearn/kernels/path_up_to_h.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    41395 2020-03-10 13:14:05.000000 graphkit-learn-0.2b2/gklearn/kernels/randomWalkKernel.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)     8569 2020-04-13 15:23:45.000000 graphkit-learn-0.2b2/gklearn/kernels/shortest_path.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    12255 2020-04-07 13:56:39.000000 graphkit-learn-0.2b2/gklearn/kernels/spKernel.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    33858 2020-03-30 15:03:31.000000 graphkit-learn-0.2b2/gklearn/kernels/structuralspKernel.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    13752 2020-04-11 12:31:36.000000 graphkit-learn-0.2b2/gklearn/kernels/structural_sp.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    20083 2020-04-23 16:36:14.000000 graphkit-learn-0.2b2/gklearn/kernels/treelet.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    17959 2020-04-13 16:12:58.000000 graphkit-learn-0.2b2/gklearn/kernels/treeletKernel.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    27302 2020-04-11 12:31:36.000000 graphkit-learn-0.2b2/gklearn/kernels/untilHPathKernel.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    19837 2020-04-14 13:17:43.000000 graphkit-learn-0.2b2/gklearn/kernels/weisfeilerLehmanKernel.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    17315 2020-04-23 16:40:01.000000 graphkit-learn-0.2b2/gklearn/kernels/weisfeiler_lehman.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)      468 2020-04-18 13:02:10.000000 graphkit-learn-0.2b2/gklearn/kernels/__init__.py
-drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-05-26 15:54:00.000000 graphkit-learn-0.2b2/gklearn/preimage/
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    17933 2020-05-19 08:05:25.000000 graphkit-learn-0.2b2/gklearn/preimage/kernel_knn_cv.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    46400 2020-05-15 10:12:44.000000 graphkit-learn-0.2b2/gklearn/preimage/median_preimage_generator.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)      852 2020-04-11 12:31:36.000000 graphkit-learn-0.2b2/gklearn/preimage/preimage_generator.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    21667 2020-05-12 14:12:27.000000 graphkit-learn-0.2b2/gklearn/preimage/utils.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    27521 2020-04-11 12:31:36.000000 graphkit-learn-0.2b2/gklearn/preimage/visualization.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)      378 2020-05-12 10:56:33.000000 graphkit-learn-0.2b2/gklearn/preimage/__init__.py
-drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-05-26 15:54:00.000000 graphkit-learn-0.2b2/gklearn/tests/
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    11785 2020-03-04 16:59:20.000000 graphkit-learn-0.2b2/gklearn/tests/test_graphkernels.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    11179 2020-04-18 13:08:48.000000 graphkit-learn-0.2b2/gklearn/tests/test_graph_kernels.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)     2528 2020-04-19 09:42:01.000000 graphkit-learn-0.2b2/gklearn/tests/test_median_preimage_generator.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)       31 2020-02-26 14:13:05.000000 graphkit-learn-0.2b2/gklearn/tests/test_tools.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)      129 2020-03-02 14:31:35.000000 graphkit-learn-0.2b2/gklearn/tests/__init__.py
-drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-05-26 15:54:00.000000 graphkit-learn-0.2b2/gklearn/utils/
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    24155 2020-05-13 15:55:10.000000 graphkit-learn-0.2b2/gklearn/utils/dataset.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    10976 2020-02-12 16:22:36.000000 graphkit-learn-0.2b2/gklearn/utils/graphdataset.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    26101 2020-04-11 12:31:36.000000 graphkit-learn-0.2b2/gklearn/utils/graphfiles.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    29319 2020-05-15 10:11:25.000000 graphkit-learn-0.2b2/gklearn/utils/graph_files.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)      527 2020-04-11 12:31:36.000000 graphkit-learn-0.2b2/gklearn/utils/isNotebook.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)     3528 2020-04-11 12:31:36.000000 graphkit-learn-0.2b2/gklearn/utils/kernels.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)     4442 2020-05-13 11:17:35.000000 graphkit-learn-0.2b2/gklearn/utils/knn.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)      624 2020-04-11 12:31:36.000000 graphkit-learn-0.2b2/gklearn/utils/logger2file.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    47095 2020-03-05 10:50:21.000000 graphkit-learn-0.2b2/gklearn/utils/model_selection_precomputed.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)     2770 2020-04-11 12:31:36.000000 graphkit-learn-0.2b2/gklearn/utils/parallel.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)      934 2020-04-11 12:31:36.000000 graphkit-learn-0.2b2/gklearn/utils/timer.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)     3029 2020-02-27 15:51:25.000000 graphkit-learn-0.2b2/gklearn/utils/trie.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)    15128 2020-05-12 10:14:43.000000 graphkit-learn-0.2b2/gklearn/utils/utils.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)      843 2020-05-12 10:24:23.000000 graphkit-learn-0.2b2/gklearn/utils/__init__.py
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)      596 2020-05-12 13:14:38.000000 graphkit-learn-0.2b2/gklearn/__init__.py
-drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-05-26 15:54:00.000000 graphkit-learn-0.2b2/graphkit_learn.egg-info/
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)        1 2020-05-26 15:54:00.000000 graphkit-learn-0.2b2/graphkit_learn.egg-info/dependency_links.txt
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)     8645 2020-05-26 15:54:00.000000 graphkit-learn-0.2b2/graphkit_learn.egg-info/PKG-INFO
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)      164 2020-05-26 15:54:00.000000 graphkit-learn-0.2b2/graphkit_learn.egg-info/requires.txt
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)     1981 2020-05-26 15:54:00.000000 graphkit-learn-0.2b2/graphkit_learn.egg-info/SOURCES.txt
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)        8 2020-05-26 15:54:00.000000 graphkit-learn-0.2b2/graphkit_learn.egg-info/top_level.txt
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)     8645 2020-05-26 15:54:00.000000 graphkit-learn-0.2b2/PKG-INFO
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)     7172 2020-05-02 14:38:19.000000 graphkit-learn-0.2b2/README.md
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)       38 2020-05-26 15:54:00.000000 graphkit-learn-0.2b2/setup.cfg
--rwxrwxrwx   0 ljia      (1000) ljia      (1000)      820 2020-05-26 15:53:39.000000 graphkit-learn-0.2b2/setup.py
+drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/
+drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/gklearn/
+drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/gklearn/examples/
+drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/gklearn/examples/ged/
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     1753 2020-06-24 14:09:49.000000 graphkit-learn-0.2b3/gklearn/examples/ged/compute_graph_edit_distance.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-06-09 10:32:07.000000 graphkit-learn-0.2b3/gklearn/examples/ged/__init__.py
+drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/gklearn/examples/kernels/
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     2367 2020-06-22 13:23:05.000000 graphkit-learn-0.2b3/gklearn/examples/kernels/compute_distance_in_kernel_space.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     2594 2020-06-22 10:07:31.000000 graphkit-learn-0.2b3/gklearn/examples/kernels/compute_graph_kernel.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)      805 2020-09-25 14:29:47.000000 graphkit-learn-0.2b3/gklearn/examples/kernels/compute_graph_kernel_old.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     1293 2020-09-25 14:46:04.000000 graphkit-learn-0.2b3/gklearn/examples/kernels/model_selection_old.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-06-09 10:32:07.000000 graphkit-learn-0.2b3/gklearn/examples/kernels/__init__.py
+drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/gklearn/examples/preimage/
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     4682 2020-06-10 10:24:06.000000 graphkit-learn-0.2b3/gklearn/examples/preimage/median_preimege_generator.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     4681 2020-07-10 09:00:15.000000 graphkit-learn-0.2b3/gklearn/examples/preimage/median_preimege_generator_cml.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     4681 2020-06-26 09:33:36.000000 graphkit-learn-0.2b3/gklearn/examples/preimage/median_preimege_generator_py.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-06-09 10:32:07.000000 graphkit-learn-0.2b3/gklearn/examples/preimage/__init__.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-06-09 10:32:07.000000 graphkit-learn-0.2b3/gklearn/examples/__init__.py
+drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/gklearn/ged/
+drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/gklearn/ged/edit_costs/
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     1171 2020-06-23 09:12:39.000000 graphkit-learn-0.2b3/gklearn/ged/edit_costs/constant.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     2110 2020-06-19 13:55:13.000000 graphkit-learn-0.2b3/gklearn/ged/edit_costs/edit_cost.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)      106 2020-06-17 16:03:25.000000 graphkit-learn-0.2b3/gklearn/ged/edit_costs/__init__.py
+drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/gklearn/ged/env/
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     6132 2020-06-18 13:36:20.000000 graphkit-learn-0.2b3/gklearn/ged/env/common_types.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     9356 2020-07-06 15:38:37.000000 graphkit-learn-0.2b3/gklearn/ged/env/ged_data.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    27764 2020-07-08 16:07:14.000000 graphkit-learn-0.2b3/gklearn/ged/env/ged_env.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     2499 2020-06-23 15:49:45.000000 graphkit-learn-0.2b3/gklearn/ged/env/node_map.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)      215 2020-06-17 15:37:30.000000 graphkit-learn-0.2b3/gklearn/ged/env/__init__.py
+drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/gklearn/ged/learning/
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     4864 2020-07-08 14:14:54.000000 graphkit-learn-0.2b3/gklearn/ged/learning/costs_learner.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     6457 2020-07-08 13:47:14.000000 graphkit-learn-0.2b3/gklearn/ged/learning/cost_matrices_learner.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)      181 2020-07-07 14:07:56.000000 graphkit-learn-0.2b3/gklearn/ged/learning/__init__.py
+drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/gklearn/ged/median/
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    64474 2020-08-24 16:05:37.000000 graphkit-learn-0.2b3/gklearn/ged/median/median_graph_estimator.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    63181 2020-07-10 08:47:28.000000 graphkit-learn-0.2b3/gklearn/ged/median/median_graph_estimator_cml.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    64342 2020-06-26 09:59:21.000000 graphkit-learn-0.2b3/gklearn/ged/median/median_graph_estimator_py.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     5758 2020-05-07 14:15:17.000000 graphkit-learn-0.2b3/gklearn/ged/median/test_median_graph_estimator.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     2593 2020-05-26 09:27:51.000000 graphkit-learn-0.2b3/gklearn/ged/median/utils.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)      317 2020-07-08 14:39:14.000000 graphkit-learn-0.2b3/gklearn/ged/median/__init__.py
+drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/gklearn/ged/methods/
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     4338 2020-06-24 08:14:55.000000 graphkit-learn-0.2b3/gklearn/ged/methods/bipartite.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     4764 2020-06-24 13:24:25.000000 graphkit-learn-0.2b3/gklearn/ged/methods/ged_method.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     8683 2020-07-02 14:23:28.000000 graphkit-learn-0.2b3/gklearn/ged/methods/lsape_based_method.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)      173 2020-06-18 14:13:20.000000 graphkit-learn-0.2b3/gklearn/ged/methods/__init__.py
+drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/gklearn/ged/util/
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     4279 2020-04-11 12:31:35.000000 graphkit-learn-0.2b3/gklearn/ged/util/cpp2python.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     3503 2020-07-03 08:52:24.000000 graphkit-learn-0.2b3/gklearn/ged/util/lsape_solver.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     4059 2020-06-23 14:11:41.000000 graphkit-learn-0.2b3/gklearn/ged/util/misc.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    21500 2020-07-10 10:15:45.000000 graphkit-learn-0.2b3/gklearn/ged/util/util.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)      198 2020-07-08 14:44:22.000000 graphkit-learn-0.2b3/gklearn/ged/util/__init__.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-04-13 15:52:46.000000 graphkit-learn-0.2b3/gklearn/ged/__init__.py
+drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/gklearn/gedlib/
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)      425 2020-04-11 12:31:36.000000 graphkit-learn-0.2b3/gklearn/gedlib/librariesImport.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     1355 2020-04-11 12:31:36.000000 graphkit-learn-0.2b3/gklearn/gedlib/setup.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     4819 2020-04-11 12:31:36.000000 graphkit-learn-0.2b3/gklearn/gedlib/test.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)      120 2020-04-11 12:31:35.000000 graphkit-learn-0.2b3/gklearn/gedlib/__init__.py
+drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/gklearn/kernels/
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    14817 2020-03-05 10:47:39.000000 graphkit-learn-0.2b3/gklearn/kernels/commonWalkKernel.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     8680 2020-08-19 15:32:23.000000 graphkit-learn-0.2b3/gklearn/kernels/common_walk.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     7733 2020-08-20 14:11:42.000000 graphkit-learn-0.2b3/gklearn/kernels/fixed_point.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     5895 2020-08-18 09:34:11.000000 graphkit-learn-0.2b3/gklearn/kernels/graph_kernel.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    11592 2020-08-18 12:48:06.000000 graphkit-learn-0.2b3/gklearn/kernels/marginalized.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    11526 2020-03-10 13:22:28.000000 graphkit-learn-0.2b3/gklearn/kernels/marginalizedKernel.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    20403 2020-06-02 12:37:11.000000 graphkit-learn-0.2b3/gklearn/kernels/path_up_to_h.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    41395 2020-03-10 13:14:05.000000 graphkit-learn-0.2b3/gklearn/kernels/randomWalkKernel.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     2846 2020-08-19 15:31:35.000000 graphkit-learn-0.2b3/gklearn/kernels/random_walk.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     8569 2020-04-13 15:23:45.000000 graphkit-learn-0.2b3/gklearn/kernels/shortest_path.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     9677 2020-08-20 15:36:56.000000 graphkit-learn-0.2b3/gklearn/kernels/spectral_decomposition.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    12255 2020-04-07 13:56:39.000000 graphkit-learn-0.2b3/gklearn/kernels/spKernel.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    33858 2020-03-30 15:03:31.000000 graphkit-learn-0.2b3/gklearn/kernels/structuralspKernel.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    13752 2020-04-11 12:31:36.000000 graphkit-learn-0.2b3/gklearn/kernels/structural_sp.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     7740 2020-08-20 13:58:24.000000 graphkit-learn-0.2b3/gklearn/kernels/sylvester_equation.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    20083 2020-06-03 21:08:44.000000 graphkit-learn-0.2b3/gklearn/kernels/treelet.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    17959 2020-04-13 16:12:58.000000 graphkit-learn-0.2b3/gklearn/kernels/treeletKernel.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    27303 2020-09-22 15:28:25.000000 graphkit-learn-0.2b3/gklearn/kernels/untilHPathKernel.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    19837 2020-04-14 13:17:43.000000 graphkit-learn-0.2b3/gklearn/kernels/weisfeilerLehmanKernel.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    17315 2020-04-23 16:40:01.000000 graphkit-learn-0.2b3/gklearn/kernels/weisfeiler_lehman.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     1271 2020-09-25 09:45:53.000000 graphkit-learn-0.2b3/gklearn/kernels/__init__.py
+drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/gklearn/preimage/
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     7472 2020-06-01 16:07:58.000000 graphkit-learn-0.2b3/gklearn/preimage/generate_random_preimages_by_class.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    18059 2020-05-27 12:46:31.000000 graphkit-learn-0.2b3/gklearn/preimage/kernel_knn_cv.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    46206 2020-07-24 15:40:11.000000 graphkit-learn-0.2b3/gklearn/preimage/median_preimage_generator.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    21054 2020-07-10 12:57:55.000000 graphkit-learn-0.2b3/gklearn/preimage/median_preimage_generator_cml.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    46108 2020-06-26 09:13:02.000000 graphkit-learn-0.2b3/gklearn/preimage/median_preimage_generator_py.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)      852 2020-04-11 12:31:36.000000 graphkit-learn-0.2b3/gklearn/preimage/preimage_generator.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    14994 2020-06-10 10:31:32.000000 graphkit-learn-0.2b3/gklearn/preimage/random_preimage_generator.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    18825 2020-05-27 14:54:41.000000 graphkit-learn-0.2b3/gklearn/preimage/remove_best_graph.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    21768 2020-06-02 12:51:54.000000 graphkit-learn-0.2b3/gklearn/preimage/utils.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    27521 2020-04-11 12:31:36.000000 graphkit-learn-0.2b3/gklearn/preimage/visualization.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)      726 2020-06-25 13:31:22.000000 graphkit-learn-0.2b3/gklearn/preimage/__init__.py
+drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/gklearn/tests/
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    11785 2020-03-04 16:59:20.000000 graphkit-learn-0.2b3/gklearn/tests/test_graphkernels.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    11866 2020-08-19 14:41:29.000000 graphkit-learn-0.2b3/gklearn/tests/test_graph_kernels.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     2596 2020-06-24 14:12:55.000000 graphkit-learn-0.2b3/gklearn/tests/test_median_preimage_generator.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     6002 2020-06-05 13:11:54.000000 graphkit-learn-0.2b3/gklearn/tests/test_random_preimage_generator.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)       31 2020-02-26 14:13:05.000000 graphkit-learn-0.2b3/gklearn/tests/test_tools.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)      129 2020-03-02 14:31:35.000000 graphkit-learn-0.2b3/gklearn/tests/__init__.py
+drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/gklearn/utils/
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    24591 2020-07-03 09:28:17.000000 graphkit-learn-0.2b3/gklearn/utils/dataset.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    10976 2020-02-12 16:22:36.000000 graphkit-learn-0.2b3/gklearn/utils/graphdataset.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    26101 2020-04-11 12:31:36.000000 graphkit-learn-0.2b3/gklearn/utils/graphfiles.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    29319 2020-05-15 10:11:25.000000 graphkit-learn-0.2b3/gklearn/utils/graph_files.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     1802 2020-09-22 16:03:03.000000 graphkit-learn-0.2b3/gklearn/utils/graph_synthesizer.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)      527 2020-04-11 12:31:36.000000 graphkit-learn-0.2b3/gklearn/utils/isNotebook.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     3528 2020-04-11 12:31:36.000000 graphkit-learn-0.2b3/gklearn/utils/kernels.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     4442 2020-05-13 11:17:35.000000 graphkit-learn-0.2b3/gklearn/utils/knn.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)      624 2020-04-11 12:31:36.000000 graphkit-learn-0.2b3/gklearn/utils/logger2file.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    47095 2020-09-25 14:06:12.000000 graphkit-learn-0.2b3/gklearn/utils/model_selection_precomputed.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     2796 2020-09-21 14:08:00.000000 graphkit-learn-0.2b3/gklearn/utils/parallel.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)      934 2020-04-11 12:31:36.000000 graphkit-learn-0.2b3/gklearn/utils/timer.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     3029 2020-02-27 15:51:25.000000 graphkit-learn-0.2b3/gklearn/utils/trie.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    17960 2020-08-18 14:17:58.000000 graphkit-learn-0.2b3/gklearn/utils/utils.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)      976 2020-09-25 09:43:01.000000 graphkit-learn-0.2b3/gklearn/utils/__init__.py
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)      596 2020-05-12 13:14:38.000000 graphkit-learn-0.2b3/gklearn/__init__.py
+drwxrwxrwx   0 ljia      (1000) ljia      (1000)        0 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/graphkit_learn.egg-info/
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)        1 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/graphkit_learn.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    11544 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/graphkit_learn.egg-info/PKG-INFO
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)      179 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/graphkit_learn.egg-info/requires.txt
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     3628 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/graphkit_learn.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)        8 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/graphkit_learn.egg-info/top_level.txt
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)    11544 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/PKG-INFO
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)     9671 2020-09-25 09:32:44.000000 graphkit-learn-0.2b3/README.md
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)       38 2020-09-25 16:44:08.000000 graphkit-learn-0.2b3/setup.cfg
+-rwxrwxrwx   0 ljia      (1000) ljia      (1000)      820 2020-09-25 16:39:56.000000 graphkit-learn-0.2b3/setup.py
```

### Comparing `graphkit-learn-0.2b2/gklearn/ged/env/node_map.py` & `graphkit-learn-0.2b3/gklearn/ged/env/node_map.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,66 +2,78 @@
 # -*- coding: utf-8 -*-
 """
 Created on Wed Apr 22 11:31:26 2020
 
 @author: ljia
 """
 import numpy as np
+from gklearn.utils import dummy_node, undefined_node
+
 
 class NodeMap(object):
 	
 	def __init__(self, num_nodes_g, num_nodes_h):
-		self.__forward_map = [np.inf] * num_nodes_g
-		self.__backward_map = [np.inf] * num_nodes_h
+		self.__forward_map = [undefined_node()] * num_nodes_g
+		self.__backward_map = [undefined_node()] * num_nodes_h
 		self.__induced_cost = np.inf
 		
 		
+	def clear(self):
+		"""
+	/*!
+	 * @brief Clears the node map.
+	 */
+		"""
+		self.__forward_map = [undefined_node() for i in range(len(self.__forward_map))]
+		self.__backward_map = [undefined_node() for i in range(len(self.__backward_map))]
+		
+		
 	def num_source_nodes(self):
 		return len(self.__forward_map)
 	
 	
 	def num_target_nodes(self):
 		return len(self.__backward_map)
 	
 	
 	def image(self, node):
 		if node < len(self.__forward_map):
 			return self.__forward_map[node]
 		else:
 			raise Exception('The node with ID ', str(node), ' is not contained in the source nodes of the node map.')
-		return np.inf
+		return undefined_node()
 	
 	
 	def pre_image(self, node):
 		if node < len(self.__backward_map):
 			return self.__backward_map[node]
 		else:
 			raise Exception('The node with ID ', str(node), ' is not contained in the target nodes of the node map.')
-		return np.inf
+		return undefined_node()
 	
 	
 	def as_relation(self, relation):
 		relation.clear()
 		for i in range(0, len(self.__forward_map)):
 			k = self.__forward_map[i]
-			if k != np.inf:
+			if k != undefined_node():
 				relation.append(tuple((i, k)))
 		for k in range(0, len(self.__backward_map)):
 			i = self.__backward_map[k]
-			if i == np.inf:
+			if i == dummy_node():
 				relation.append(tuple((i, k)))
 	
 	
 	def add_assignment(self, i, k):
-		if i != np.inf:
+		if i != dummy_node():
 			if i < len(self.__forward_map):
 				self.__forward_map[i] = k
 			else:
 				raise Exception('The node with ID ', str(i), ' is not contained in the source nodes of the node map.')
-		if k != np.inf:
+		if k != dummy_node():
 			if k < len(self.__backward_map):
 				self.__backward_map[k] = i
 			else:
 				raise Exception('The node with ID ', str(k), ' is not contained in the target nodes of the node map.')
 	
 	
 	def set_induced_cost(self, induced_cost):
```

### Comparing `graphkit-learn-0.2b2/gklearn/ged/median/median_graph_estimator.py` & `graphkit-learn-0.2b3/gklearn/ged/median/median_graph_estimator.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,18 +339,18 @@
 #		print(nx.adjacency_matrix(graphs[0]))
 			
 		# Construct initial medians.
 		medians = []
 		self.__construct_initial_medians(graph_ids, timer, medians)
 		end_init = time.time()
 		self.__runtime_initialized = end_init - start
-#		print(medians[0].graph)
-#		print(medians[0].nodes(data=True))
-#		print(medians[0].edges(data=True))
-#		print(nx.adjacency_matrix(medians[0]))
+		print(medians[0].graph)
+		print(medians[0].nodes(data=True))
+		print(medians[0].edges(data=True))
+		print(nx.adjacency_matrix(medians[0]))
 		
 		# Reset information about iterations and number of times the median decreases and increases.
 		self.__itrs = [0] * len(medians)
 		self.__num_decrease_order = 0
 		self.__num_increase_order = 0
 		self.__num_converged_descents = 0
 		
@@ -377,21 +377,21 @@
 			median = medians[median_pos]
 			
 			# Load initial median into the environment.
 			self.__ged_env.load_nx_graph(median, gen_median_id)
 			self.__ged_env.init(self.__ged_env.get_init_type())
 			
 			# Compute node maps and sum of distances for initial median.
-# 			xxx = self.__node_maps_from_median
+			xxx = self.__node_maps_from_median
 			self.__compute_init_node_maps(graph_ids, gen_median_id)
-# 			yyy = self.__node_maps_from_median
+			yyy = self.__node_maps_from_median
 			
 			self.__best_init_sum_of_distances = min(self.__best_init_sum_of_distances, self.__sum_of_distances)
 			self.__ged_env.load_nx_graph(median, set_median_id)
-# 			print(self.__best_init_sum_of_distances)
+			print(self.__best_init_sum_of_distances)
 				
 			# Run block gradient descent from initial median.
 			converged = False
 			itrs_without_update = 0
 			while not self.__termination_criterion_met(converged, timer, self.__itrs[median_pos], itrs_without_update):
 				
 				# Print information about current iteration.
@@ -735,33 +735,38 @@
 			medoid_id = np.argmin(sum_of_distances_list)
 			best_sum_of_distances = sum_of_distances_list[medoid_id]
 			
 			initial_medians.append(self.__ged_env.get_nx_graph(medoid_id, True, True, False)) # @todo
 
 		else:
 			# Print information about current iteration.
+			self.ged_matrix_set_median_tmp = np.ones((len(graph_ids), len(graph_ids))) * np.inf
 			if self.__print_to_stdout == 2:
 				progress = tqdm(desc='Computing medoid', total=len(graph_ids), file=sys.stdout)
 		
 			medoid_id = graph_ids[0]
 			best_sum_of_distances = np.inf
 			for g_id in graph_ids:
 				if timer.expired():
 					self.__state = AlgorithmState.CALLED
 					break
 				nb_nodes_g = self.__ged_env.get_graph_num_nodes(g_id)
 				sum_of_distances = 0
-				for h_id in graph_ids:					
+				for h_id in graph_ids: # @todo: can this be faster?				
 					nb_nodes_h = self.__ged_env.get_graph_num_nodes(h_id)
 					if nb_nodes_g <= nb_nodes_h or not self.__sort_graphs:
 						self.__ged_env.run_method(g_id, h_id)
 						sum_of_distances += self.__ged_env.get_upper_bound(g_id, h_id)
+						self.ged_matrix_set_median_tmp[g_id, h_id] = self.__ged_env.get_upper_bound(g_id, h_id)
 					else:
+						# @todo: is this correct?
 						self.__ged_env.run_method(h_id, g_id)
-						sum_of_distances += self.__ged_env.get_upper_bound(h_id, g_id)	
+						sum_of_distances += self.__ged_env.get_upper_bound(h_id, g_id)
+						self.ged_matrix_set_median_tmp[g_id, h_id] = self.__ged_env.get_upper_bound(h_id, g_id)
+					print(sum_of_distances)
 				if sum_of_distances < best_sum_of_distances:
 					best_sum_of_distances = sum_of_distances
 					medoid_id = g_id
 					
 				# Print information about current iteration.
 				if self.__print_to_stdout == 2:
 					progress.update(1)
```

### Comparing `graphkit-learn-0.2b2/gklearn/ged/median/test_median_graph_estimator.py` & `graphkit-learn-0.2b3/gklearn/ged/median/test_median_graph_estimator.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/ged/median/utils.py` & `graphkit-learn-0.2b3/gklearn/ged/median/utils.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/ged/util/cpp2python.py` & `graphkit-learn-0.2b3/gklearn/ged/util/cpp2python.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/gedlib/setup.py` & `graphkit-learn-0.2b3/gklearn/gedlib/setup.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/gedlib/test.py` & `graphkit-learn-0.2b3/gklearn/gedlib/test.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/kernels/commonWalkKernel.py` & `graphkit-learn-0.2b3/gklearn/kernels/commonWalkKernel.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/kernels/graph_kernel.py` & `graphkit-learn-0.2b3/gklearn/kernels/graph_kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 @author: ljia
 """
 import numpy as np
 import networkx as nx
 import multiprocessing
 import time
 
+
 class GraphKernel(object):
 	
 	def __init__(self):
 		self._graphs = None
 		self._parallel = ''
 		self._n_jobs = 0
 		self._verbose = None
```

### Comparing `graphkit-learn-0.2b2/gklearn/kernels/marginalizedKernel.py` & `graphkit-learn-0.2b3/gklearn/kernels/marginalizedKernel.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/kernels/path_up_to_h.py` & `graphkit-learn-0.2b3/gklearn/kernels/path_up_to_h.py`

 * *Files 8% similar despite different names*

```diff
@@ -369,16 +369,26 @@
 			path_count2 = Counter(paths2)
 			vector1 = [(path_count1[key] if (key in path_count1.keys()) else 0)
 					   for key in all_paths]
 			vector2 = [(path_count2[key] if (key in path_count2.keys()) else 0)
 					   for key in all_paths]
 			kernel = np.sum(np.minimum(vector1, vector2)) / \
 				np.sum(np.maximum(vector1, vector2))
+				
+		elif self.__k_func is None: # no sub-kernel used; compare paths directly.
+			path_count1 = Counter(paths1)
+			path_count2 = Counter(paths2)
+			vector1 = [(path_count1[key] if (key in path_count1.keys()) else 0)
+					   for key in all_paths]
+			vector2 = [(path_count2[key] if (key in path_count2.keys()) else 0)
+					   for key in all_paths]
+			kernel = np.dot(vector1, vector2)
+			
 		else:
-			raise Exception('The given "k_func" cannot be recognized. Possible choices include: "tanimoto", "MinMax".')
+			raise Exception('The given "k_func" cannot be recognized. Possible choices include: "tanimoto", "MinMax" and None.')
 	
 		return kernel
 	
 	
 	def _wrapper_kernel_do_naive(self, itr):
 		i = itr[0]
 		j = itr[1]
```

### Comparing `graphkit-learn-0.2b2/gklearn/kernels/randomWalkKernel.py` & `graphkit-learn-0.2b3/gklearn/kernels/randomWalkKernel.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/kernels/shortest_path.py` & `graphkit-learn-0.2b3/gklearn/kernels/shortest_path.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/kernels/spKernel.py` & `graphkit-learn-0.2b3/gklearn/kernels/spKernel.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/kernels/structuralspKernel.py` & `graphkit-learn-0.2b3/gklearn/kernels/structuralspKernel.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/kernels/structural_sp.py` & `graphkit-learn-0.2b3/gklearn/kernels/structural_sp.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/kernels/treelet.py` & `graphkit-learn-0.2b3/gklearn/kernels/treelet.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 		----------
 		canonkey1, canonkey2 : list
 			List of canonical keys in 2 graphs, where each key is represented by a string.
 			
 		Return
 		------
 		kernel : float
-			Treelet Kernel between 2 graphs.
+			Treelet kernel between 2 graphs.
 		"""
 		keys = set(canonkey1.keys()) & set(canonkey2.keys()) # find same canonical keys in both graphs
 		vector1 = np.array([(canonkey1[key] if (key in canonkey1.keys()) else 0) for key in keys])
 		vector2 = np.array([(canonkey2[key] if (key in canonkey2.keys()) else 0) for key in keys]) 
 		kernel = self.__sub_kernel(vector1, vector2) 
 		return kernel
```

### Comparing `graphkit-learn-0.2b2/gklearn/kernels/treeletKernel.py` & `graphkit-learn-0.2b3/gklearn/kernels/treeletKernel.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/kernels/untilHPathKernel.py` & `graphkit-learn-0.2b3/gklearn/kernels/untilHPathKernel.py`

 * *Files 0% similar despite different names*

```diff
@@ -645,15 +645,15 @@
             #         chain.from_iterable((G.node[node][node_label],
             #                              G[node][path[idx + 1]][edge_label])
             #                             for idx, node in enumerate(path[:-1])))
             #     strlist.append(G.node[path[-1]][node_label])
             #     path_strs.append(tuple(strlist))
         else:
             path_strs = [
-                tuple([G.node[node][node_label] for node in path])
+                tuple([G.nodes[node][node_label] for node in path])
                 for path in plist
             ]
         return path_strs
     else:
         if ds_attrs['edge_labeled']:
             return [
                 tuple([] if len(path) == 1 else [
```

### Comparing `graphkit-learn-0.2b2/gklearn/kernels/weisfeilerLehmanKernel.py` & `graphkit-learn-0.2b3/gklearn/kernels/weisfeilerLehmanKernel.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/kernels/weisfeiler_lehman.py` & `graphkit-learn-0.2b3/gklearn/kernels/weisfeiler_lehman.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/preimage/kernel_knn_cv.py` & `graphkit-learn-0.2b3/gklearn/preimage/kernel_knn_cv.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,15 +357,16 @@
 		else:
 			gram_matrix_unnorm, time_precompute_gm = __compute_gram_matrix_unnorm(dataset_all, kernel_options)
 			np.savez(dir_save + 'gram_matrix_unnorm.' + ds_name + '.' + kernel_options['name'] + '.gm', gram_matrix_unnorm=gram_matrix_unnorm, run_time=time_precompute_gm)
 	elif not load_gm:
 		gram_matrix_unnorm, time_precompute_gm = __compute_gram_matrix_unnorm(dataset_all, kernel_options)
 		np.savez(dir_save + 'gram_matrix_unnorm.' + ds_name + '.' + kernel_options['name'] + '.gm', gram_matrix_unnorm=gram_matrix_unnorm, run_time=time_precompute_gm)
 	else:
-		gmfile = np.load()
+		gm_fname = dir_save + 'gram_matrix_unnorm.' + ds_name + '.' + kernel_options['name'] + '.gm.npz'
+		gmfile = np.load(gm_fname, allow_pickle=True)
 		gram_matrix_unnorm = gmfile['gram_matrix_unnorm']
 		time_precompute_gm = float(gmfile['run_time'])
 		
 	return gram_matrix_unnorm, time_precompute_gm
 
 
 def __get_graph_kernel(dataset, kernel_options):
```

### Comparing `graphkit-learn-0.2b2/gklearn/preimage/median_preimage_generator.py` & `graphkit-learn-0.2b3/gklearn/preimage/median_preimage_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from gklearn.preimage.utils import compute_k_dis
 from gklearn.ged.util import compute_geds, ged_options_to_string
 from gklearn.ged.median import MedianGraphEstimator
 from gklearn.ged.median import constant_node_costs,mge_options_to_string
 from gklearn.gedlib import librariesImport, gedlibpy
 from gklearn.utils import Timer
 from gklearn.utils.utils import get_graph_kernel_by_name
-# from gklearn.utils.dataset import Dataset
+
 
 class MedianPreimageGenerator(PreimageGenerator):
 	
 	def __init__(self, dataset=None):
 		PreimageGenerator.__init__(self, dataset=dataset)
 		# arguments to set.
 		self.__mge = None
@@ -123,40 +123,33 @@
 		self.__optimize_edit_cost_constants()
 		end_optimize_ec = time.time()
 		self.__runtime_optimize_ec = end_optimize_ec - end_precompute_gm
 		
 		# 3. compute set median and gen median using optimized edit costs.
 		if self._verbose >= 2:
 			print('\nstart computing set median and gen median using optimized edit costs...\n')
-# 		group_fnames = [Gn[g].graph['filename'] for g in group_min]
-		self.__generate_preimage_iam()
+		self.__gmg_bcu()
 		end_generate_preimage = time.time()
 		self.__runtime_generate_preimage = end_generate_preimage - end_optimize_ec
 		self.__runtime_total = end_generate_preimage - start
 		if self._verbose >= 2:
 			print('medians computed.')
 			print('SOD of the set median: ', self.__sod_set_median)
 			print('SOD of the generalized median: ', self.__sod_gen_median)
 			
 		# 4. compute kernel distances to the true median.
 		if self._verbose >= 2:
 			print('\nstart computing distances to true median....\n')
-# 		Gn_median = [Gn[g].copy() for g in group_min]
 		self.__compute_distances_to_true_median()
-# 		dis_k_sm, dis_k_gm, dis_k_gi, dis_k_gi_min, idx_dis_k_gi_min = 
-# 		idx_dis_k_gi_min = group_min[idx_dis_k_gi_min]
-# 		print('index min dis_k_gi:', idx_dis_k_gi_min)
-# 		print('sod_sm:', sod_sm)
-# 		print('sod_gm:', sod_gm)
 
 		# 5. print out results.
 		if self._verbose:
 			print()
 			print('================================================================================')
-			print('Finished generalization of preimages.')
+			print('Finished generation of preimages.')
 			print('--------------------------------------------------------------------------------')
 			print('The optimized edit cost constants:', self.__edit_cost_constants)
 			print('SOD of the set median:', self.__sod_set_median)
 			print('SOD of the generalized median:', self.__sod_gen_median)
 			print('Distance in kernel space for set median:', self.__k_dis_set_median)
 			print('Distance in kernel space for generalized median:', self.__k_dis_gen_median)
 			print('Minimum distance in kernel space for each graph in median set:', self.__k_dis_dataset)
@@ -165,19 +158,14 @@
 			print('Time to generate pre-images:', self.__runtime_generate_preimage)
 			print('Total time:', self.__runtime_total)
 			print('Total number of iterations for optimizing:', self.__itrs)
 			print('Total number of updating edit costs:', self.__num_updates_ecc)
 			print('Is optimization of edit costs converged:', self.__converged)
 			print('================================================================================')
 			print()
-			
-	# collect return values.
-# 	return (sod_sm, sod_gm), \
-# 		   (dis_k_sm, dis_k_gm, dis_k_gi, dis_k_gi_min, idx_dis_k_gi_min), \
-# 		   (time_fitting, time_generating)
 
 
 	def get_results(self):
 		results = {}
 		results['edit_cost_constants'] = self.__edit_cost_constants
 		results['runtime_precompute_gm'] = self.__runtime_precompute_gm
 		results['runtime_optimize_ec'] = self.__runtime_optimize_ec
@@ -191,36 +179,39 @@
 		results['itrs'] = self.__itrs
 		results['converged'] = self.__converged
 		results['num_updates_ecc'] = self.__num_updates_ecc
 		results['mge'] = {}
 		results['mge']['num_decrease_order'] = self.__mge.get_num_times_order_decreased()
 		results['mge']['num_increase_order'] = self.__mge.get_num_times_order_increased()
 		results['mge']['num_converged_descents'] = self.__mge.get_num_converged_descents()
+		results['ged_matrix_set_median'] = self.__mge.ged_matrix_set_median_tmp
 		return results
 
 		
 	def __optimize_edit_cost_constants(self):
 		"""fit edit cost constants.	
 		"""
 		if self.__fit_method == 'random': # random
 			if self.__ged_options['edit_cost'] == 'LETTER':
-				self.__edit_cost_constants = random.sample(range(1, 10), 3)
-				self.__edit_cost_constants = [item * 0.1 for item in self.__edit_cost_constants]
+				self.__edit_cost_constants = random.sample(range(1, 1000), 3)
+				self.__edit_cost_constants = [item * 0.001 for item in self.__edit_cost_constants]
 			elif self.__ged_options['edit_cost'] == 'LETTER2':
 				random.seed(time.time())
-				self.__edit_cost_constants = random.sample(range(1, 10), 5)
-	#			self.__edit_cost_constants = [item * 0.1 for item in self.__edit_cost_constants]
+				self.__edit_cost_constants = random.sample(range(1, 1000), 5)
+				self.__edit_cost_constants = [item * 0.01 for item in self.__edit_cost_constants]
 			elif self.__ged_options['edit_cost'] == 'NON_SYMBOLIC':
-				self.__edit_cost_constants = random.sample(range(1, 10), 6)
+				self.__edit_cost_constants = random.sample(range(1, 1000), 6)
+				self.__edit_cost_constants = [item * 0.01 for item in self.__edit_cost_constants]
 				if self._dataset.node_attrs == []:
 					self.__edit_cost_constants[2] = 0
 				if self._dataset.edge_attrs == []:
 					self.__edit_cost_constants[5] = 0
 			else:
-				self.__edit_cost_constants = random.sample(range(1, 10), 6)
+				self.__edit_cost_constants = random.sample(range(1, 1000), 6)
+				self.__edit_cost_constants = [item * 0.01 for item in self.__edit_cost_constants]
 			if self._verbose >= 2:
 				print('edit cost constants used:', self.__edit_cost_constants)
 		elif self.__fit_method == 'expert': # expert
 			if self.__init_ecc is None:
 				if self.__ged_options['edit_cost'] == 'LETTER':
 					self.__edit_cost_constants = [0.9, 1.7, 0.75] 
 				elif self.__ged_options['edit_cost'] == 'LETTER2':
@@ -857,15 +848,23 @@
 		else:
 			if self._verbose >= 2:
 				print('solver status: ', prob.status)
 		if self._verbose >= 2:				
 			print()
 
 	
-	def __generate_preimage_iam(self):
+	def __gmg_bcu(self):
+		"""
+		The local search algorithm based on block coordinate update (BCU) for estimating a generalized median graph (GMG).
+
+		Returns
+		-------
+		None.
+
+		"""
 		# Set up the ged environment.
 		ged_env = gedlibpy.GEDEnv() # @todo: maybe create a ged_env as a private varible.
 		# gedlibpy.restart_env()
 		ged_env.set_edit_cost(self.__ged_options['edit_cost'], edit_cost_constant=self.__edit_cost_constants)
 		graphs = [self.__clean_graph(g) for g in self._dataset.graphs]
 		for g in graphs:
 			ged_env.add_nx_graph(g, '')
@@ -906,32 +905,32 @@
 		self.__gen_median = ged_env.get_nx_graph(gen_median_id)
 		
 		
 	def __compute_distances_to_true_median(self):		
 		# compute distance in kernel space for set median.
 		kernels_to_sm, _ = self._graph_kernel.compute(self.__set_median, self._dataset.graphs, **self._kernel_options)
 		kernel_sm, _ = self._graph_kernel.compute(self.__set_median, self.__set_median, **self._kernel_options)
-		kernels_to_sm = [kernels_to_sm[i] / np.sqrt(self.__gram_matrix_unnorm[i, i] * kernel_sm) for i in range(len(kernels_to_sm))] # normalize 
+		if self._kernel_options['normalize']:
+			kernels_to_sm = [kernels_to_sm[i] / np.sqrt(self.__gram_matrix_unnorm[i, i] * kernel_sm) for i in range(len(kernels_to_sm))] # normalize 
+			kernel_sm = 1
 		# @todo: not correct kernel value
 		gram_with_sm = np.concatenate((np.array([kernels_to_sm]), np.copy(self._graph_kernel.gram_matrix)), axis=0)
-		gram_with_sm = np.concatenate((np.array([[1] + kernels_to_sm]).T, gram_with_sm), axis=1)
+		gram_with_sm = np.concatenate((np.array([[kernel_sm] + kernels_to_sm]).T, gram_with_sm), axis=1)
 		self.__k_dis_set_median = compute_k_dis(0, range(1, 1+len(self._dataset.graphs)), 
 										  [1 / len(self._dataset.graphs)] * len(self._dataset.graphs),
 										  gram_with_sm, withterm3=False)
-	#	print(gen_median.nodes(data=True))
-	#	print(gen_median.edges(data=True))
-	#	print(set_median.nodes(data=True))
-	#	print(set_median.edges(data=True))
 		
 		# compute distance in kernel space for generalized median.
 		kernels_to_gm, _ = self._graph_kernel.compute(self.__gen_median, self._dataset.graphs, **self._kernel_options)
 		kernel_gm, _ = self._graph_kernel.compute(self.__gen_median, self.__gen_median, **self._kernel_options)
-		kernels_to_gm = [kernels_to_gm[i] / np.sqrt(self.__gram_matrix_unnorm[i, i] * kernel_gm) for i in range(len(kernels_to_gm))] # normalize
+		if self._kernel_options['normalize']:
+			kernels_to_gm = [kernels_to_gm[i] / np.sqrt(self.__gram_matrix_unnorm[i, i] * kernel_gm) for i in range(len(kernels_to_gm))] # normalize
+			kernel_gm = 1
 		gram_with_gm = np.concatenate((np.array([kernels_to_gm]), np.copy(self._graph_kernel.gram_matrix)), axis=0)
-		gram_with_gm = np.concatenate((np.array([[1] + kernels_to_gm]).T, gram_with_gm), axis=1)
+		gram_with_gm = np.concatenate((np.array([[kernel_gm] + kernels_to_gm]).T, gram_with_gm), axis=1)
 		self.__k_dis_gen_median = compute_k_dis(0, range(1, 1+len(self._dataset.graphs)), 
 										  [1 / len(self._dataset.graphs)] * len(self._dataset.graphs),
 										  gram_with_gm, withterm3=False)
 				
 		# compute distance in kernel space for each graph in median set.
 		k_dis_median_set = []
 		for idx in range(len(self._dataset.graphs)):
```

### Comparing `graphkit-learn-0.2b2/gklearn/preimage/preimage_generator.py` & `graphkit-learn-0.2b3/gklearn/preimage/preimage_generator.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/preimage/utils.py` & `graphkit-learn-0.2b3/gklearn/preimage/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,22 +78,22 @@
 		else:
 			gram_matrix_unnorm_list = []
 			time_precompute_gm_list = []
 	elif not load_gm:
 		gram_matrix_unnorm_list = []
 		time_precompute_gm_list = []
 	else:
+		gm_fname = dir_save + 'gram_matrix_unnorm.' + ds_name + '.' + kernel_options['name'] + '.gm.npz'
 		gmfile = np.load(gm_fname, allow_pickle=True) # @todo: may not be safe.
 		gram_matrix_unnorm_list = [item for item in gmfile['gram_matrix_unnorm_list']]
 		time_precompute_gm_list = gmfile['run_time_list'].tolist()
 #	repeats_better_sod_sm2gm = []
 #	repeats_better_dis_k_sm2gm = []
 #	repeats_better_dis_k_gi2sm = []
-#	repeats_better_dis_k_gi2gm = []
-		
+#	repeats_better_dis_k_gi2gm = []		
 		
 	print('starting generating preimage for each class of target...')
 	idx_offset = 0
 	for idx, dataset in enumerate(datasets):
 		target = dataset.targets[0]
 		print('\ntarget =', target, '\n')
 #		if target != 1:
@@ -252,15 +252,15 @@
 				draw_Letter_graph(mpg.set_median, fn_pre_sm)
 				draw_Letter_graph(mpg.gen_median, fn_pre_gm)
 				draw_Letter_graph(mpg.best_from_dataset, fn_best_dataset)
 				
 		if (load_gm == 'auto' and not gmfile_exist) or not load_gm:
 			gram_matrix_unnorm_list.append(mpg.gram_matrix_unnorm)
 
-	# write result summary for each letter. 
+	# write result summary for each class. 
 	if save_results:
 		sod_sm_mean = np.mean(sod_sm_list)
 		sod_gm_mean = np.mean(sod_gm_list)
 		dis_k_sm_mean = np.mean(dis_k_sm_list)
 		dis_k_gm_mean = np.mean(dis_k_gm_list)
 		dis_k_gi_min_mean = np.mean(dis_k_gi_min_list)
 		time_precompute_gm_mean = np.mean(time_precompute_gm_list)
@@ -383,23 +383,23 @@
 	if withterm3 == False:
 		for i1, a1 in enumerate(alpha):
 			for i2, a2 in enumerate(alpha):
 				term3 += a1 * a2 * Kmatrix[idx_gi[i1], idx_gi[i2]]
 	return np.sqrt(term1 - term2 + term3)
 
 
-def compute_k_dis(idx_g, idx_gi, alpha, Kmatrix, term3=0, withterm3=True):
+def compute_k_dis(idx_g, idx_gi, alphas, Kmatrix, term3=0, withterm3=True):
 	term1 = Kmatrix[idx_g, idx_g]
 	term2 = 0
-	for i, a in enumerate(alpha):
+	for i, a in enumerate(alphas):
 		term2 += a * Kmatrix[idx_g, idx_gi[i]]
 	term2 *= 2
 	if withterm3 == False:
-		for i1, a1 in enumerate(alpha):
-			for i2, a2 in enumerate(alpha):
+		for i1, a1 in enumerate(alphas):
+			for i2, a2 in enumerate(alphas):
 				term3 += a1 * a2 * Kmatrix[idx_gi[i1], idx_gi[i2]]
 	return np.sqrt(term1 - term2 + term3)
 
 
 def compute_kernel(Gn, graph_kernel, node_label, edge_label, verbose, parallel='imap_unordered'):
 	if graph_kernel == 'marginalizedkernel':
 		Kmatrix, _ = marginalizedkernel(Gn, node_label=node_label, edge_label=edge_label,
```

### Comparing `graphkit-learn-0.2b2/gklearn/preimage/visualization.py` & `graphkit-learn-0.2b3/gklearn/preimage/visualization.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/tests/test_graphkernels.py` & `graphkit-learn-0.2b3/gklearn/tests/test_graphkernels.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/tests/test_graph_kernels.py` & `graphkit-learn-0.2b3/gklearn/tests/test_graph_kernels.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,102 +48,112 @@
 		dataset.trim_dataset(edge_required=True)
 		
 	dataset.cut_graphs(range(0, 3))
 	
 	return dataset
 
 
-# @pytest.mark.parametrize('ds_name', ['Alkane', 'AIDS'])
-# @pytest.mark.parametrize('weight,compute_method', [(0.01, 'geo'), (1, 'exp')])
-# #@pytest.mark.parametrize('parallel', ['imap_unordered', None])
-# def test_commonwalkkernel(ds_name, weight, compute_method):
-#	 """Test common walk kernel.
-#	 """
-#	 from gklearn.kernels.commonWalkKernel import commonwalkkernel
-	
-#	 Gn, y = chooseDataset(ds_name)
-
-#	 try:
-#		 Kmatrix, run_time, idx = commonwalkkernel(Gn, 
-#											  node_label='atom', 
-#											  edge_label='bond_type',
-#											  weight=weight,
-#											  compute_method=compute_method,
-# #											 parallel=parallel,
-#											  n_jobs=multiprocessing.cpu_count(), 
-#											  verbose=True)
-#	 except Exception as exception:
-#		 assert False, exception
+@pytest.mark.parametrize('ds_name', ['Alkane', 'AIDS'])
+@pytest.mark.parametrize('weight,compute_method', [(0.01, 'geo'), (1, 'exp')])
+@pytest.mark.parametrize('parallel', ['imap_unordered', None])
+def test_CommonWalk(ds_name, parallel, weight, compute_method):
+	"""Test common walk kernel.
+	"""
+	from gklearn.kernels import CommonWalk
+	import networkx as nx
+	
+	dataset = chooseDataset(ds_name)
+	dataset.load_graphs([g for g in dataset.graphs if nx.number_of_nodes(g) > 1])
+	
+	try:
+		graph_kernel = CommonWalk(node_labels=dataset.node_labels,
+					edge_labels=dataset.edge_labels,
+					ds_infos=dataset.get_dataset_infos(keys=['directed']),
+					weight=weight,
+					compute_method=compute_method)
+		gram_matrix, run_time = graph_kernel.compute(dataset.graphs,
+			parallel=parallel, n_jobs=multiprocessing.cpu_count(), verbose=True)
+		kernel_list, run_time = graph_kernel.compute(dataset.graphs[0], dataset.graphs[1:],
+			parallel=parallel, n_jobs=multiprocessing.cpu_count(), verbose=True)
+		kernel, run_time = graph_kernel.compute(dataset.graphs[0], dataset.graphs[1],
+			parallel=parallel, n_jobs=multiprocessing.cpu_count(), verbose=True)
+
+	except Exception as exception:
+		assert False, exception
 		
 		
-# @pytest.mark.parametrize('ds_name', ['Alkane', 'AIDS'])
-# @pytest.mark.parametrize('remove_totters', [True, False])
-# #@pytest.mark.parametrize('parallel', ['imap_unordered', None])
-# def test_marginalizedkernel(ds_name, remove_totters):
-#	 """Test marginalized kernel.
-#	 """
-#	 from gklearn.kernels.marginalizedKernel import marginalizedkernel
-	
-#	 Gn, y = chooseDataset(ds_name)
-
-#	 try:
-#		 Kmatrix, run_time = marginalizedkernel(Gn, 
-#												node_label='atom', 
-#												edge_label='bond_type',
-#												p_quit=0.5,
-#												n_iteration=2,
-#												remove_totters=remove_totters,
-# #											   parallel=parallel,
-#												n_jobs=multiprocessing.cpu_count(), 
-#												verbose=True)
-#	 except Exception as exception:
-#		 assert False, exception
+@pytest.mark.parametrize('ds_name', ['Alkane', 'AIDS'])
+@pytest.mark.parametrize('remove_totters', [False]) #[True, False])
+@pytest.mark.parametrize('parallel', ['imap_unordered', None])
+def test_Marginalized(ds_name, parallel, remove_totters):
+	"""Test marginalized kernel.
+	"""
+	from gklearn.kernels import Marginalized
+	
+	dataset = chooseDataset(ds_name)
+	
+	try:
+		graph_kernel = Marginalized(node_labels=dataset.node_labels,
+					edge_labels=dataset.edge_labels,
+					ds_infos=dataset.get_dataset_infos(keys=['directed']),
+					p_quit=0.5,
+					n_iteration=2,
+					remove_totters=remove_totters)
+		gram_matrix, run_time = graph_kernel.compute(dataset.graphs,
+			parallel=parallel, n_jobs=multiprocessing.cpu_count(), verbose=True)
+		kernel_list, run_time = graph_kernel.compute(dataset.graphs[0], dataset.graphs[1:],
+			parallel=parallel, n_jobs=multiprocessing.cpu_count(), verbose=True)
+		kernel, run_time = graph_kernel.compute(dataset.graphs[0], dataset.graphs[1],
+			parallel=parallel, n_jobs=multiprocessing.cpu_count(), verbose=True)
+
+	except Exception as exception:
+		assert False, exception
 		
 		
 # @pytest.mark.parametrize(
-#		 'compute_method,ds_name,sub_kernel',
-#		 [
+#		'compute_method,ds_name,sub_kernel',
+#		[
 # #			('sylvester', 'Alkane', None),
 # #			('conjugate', 'Alkane', None),
 # #			('conjugate', 'AIDS', None),
 # #			('fp', 'Alkane', None),
 # #			('fp', 'AIDS', None),
-#			 ('spectral', 'Alkane', 'exp'),
-#			 ('spectral', 'Alkane', 'geo'),
-#		 ]
+#			('spectral', 'Alkane', 'exp'),
+#			('spectral', 'Alkane', 'geo'),
+#		]
 # )
 # #@pytest.mark.parametrize('parallel', ['imap_unordered', None])
 # def test_randomwalkkernel(ds_name, compute_method, sub_kernel):
-#	 """Test random walk kernel kernel.
-#	 """
-#	 from gklearn.kernels.randomWalkKernel import randomwalkkernel
-#	 from gklearn.utils.kernels import deltakernel, gaussiankernel, kernelproduct
-#	 import functools
-	
-#	 Gn, y = chooseDataset(ds_name)
-
-#	 mixkernel = functools.partial(kernelproduct, deltakernel, gaussiankernel)
-#	 sub_kernels = [{'symb': deltakernel, 'nsymb': gaussiankernel, 'mix': mixkernel}]
-#	 try:
-#		 Kmatrix, run_time, idx = randomwalkkernel(Gn,
-#												   compute_method=compute_method,
-#												   weight=1e-3,
-#												   p=None,
-#												   q=None,
-#												   edge_weight=None,
-#												   node_kernels=sub_kernels,
-#												   edge_kernels=sub_kernels,
-#												   node_label='atom', 
-#												   edge_label='bond_type',
-#												   sub_kernel=sub_kernel,
-# #												  parallel=parallel,
-#												  n_jobs=multiprocessing.cpu_count(), 
-#												  verbose=True)
-#	 except Exception as exception:
-#		 assert False, exception
+#	"""Test random walk kernel kernel.
+#	"""
+#	from gklearn.kernels.randomWalkKernel import randomwalkkernel
+#	from gklearn.utils.kernels import deltakernel, gaussiankernel, kernelproduct
+#	import functools
+	
+#	Gn, y = chooseDataset(ds_name)
+
+#	mixkernel = functools.partial(kernelproduct, deltakernel, gaussiankernel)
+#	sub_kernels = [{'symb': deltakernel, 'nsymb': gaussiankernel, 'mix': mixkernel}]
+#	try:
+#		Kmatrix, run_time, idx = randomwalkkernel(Gn,
+#												  compute_method=compute_method,
+#												  weight=1e-3,
+#												  p=None,
+#												  q=None,
+#												  edge_weight=None,
+#												  node_kernels=sub_kernels,
+#												  edge_kernels=sub_kernels,
+#												  node_label='atom', 
+#												  edge_label='bond_type',
+#												  sub_kernel=sub_kernel,
+# #												 parallel=parallel,
+#												 n_jobs=multiprocessing.cpu_count(), 
+#												 verbose=True)
+#	except Exception as exception:
+#		assert False, exception
 
 		
 @pytest.mark.parametrize('ds_name', ['Alkane', 'Acyclic', 'Letter-med', 'AIDS', 'Fingerprint'])
 @pytest.mark.parametrize('parallel', ['imap_unordered', None])
 def test_ShortestPath(ds_name, parallel):
 	"""Test shortest path kernel.
 	"""
@@ -153,17 +163,17 @@
 	
 	dataset = chooseDataset(ds_name)
 	
 	mixkernel = functools.partial(kernelproduct, deltakernel, gaussiankernel)
 	sub_kernels = {'symb': deltakernel, 'nsymb': gaussiankernel, 'mix': mixkernel}
 	try:
 		graph_kernel = ShortestPath(node_labels=dataset.node_labels,
-					 node_attrs=dataset.node_attrs,
-					 ds_infos=dataset.get_dataset_infos(keys=['directed']),
-					 node_kernels=sub_kernels)
+					node_attrs=dataset.node_attrs,
+					ds_infos=dataset.get_dataset_infos(keys=['directed']),
+					node_kernels=sub_kernels)
 		gram_matrix, run_time = graph_kernel.compute(dataset.graphs,
 			parallel=parallel, n_jobs=multiprocessing.cpu_count(), verbose=True)
 		kernel_list, run_time = graph_kernel.compute(dataset.graphs[0], dataset.graphs[1:],
 			parallel=parallel, n_jobs=multiprocessing.cpu_count(), verbose=True)
 		kernel, run_time = graph_kernel.compute(dataset.graphs[0], dataset.graphs[1],
 			parallel=parallel, n_jobs=multiprocessing.cpu_count(), verbose=True)
 
@@ -183,20 +193,20 @@
 	
 	dataset = chooseDataset(ds_name)
 	
 	mixkernel = functools.partial(kernelproduct, deltakernel, gaussiankernel)
 	sub_kernels = {'symb': deltakernel, 'nsymb': gaussiankernel, 'mix': mixkernel}
 	try:
 		graph_kernel = StructuralSP(node_labels=dataset.node_labels,
-					  edge_labels=dataset.edge_labels, 
-					  node_attrs=dataset.node_attrs,
-					  edge_attrs=dataset.edge_attrs,
-					  ds_infos=dataset.get_dataset_infos(keys=['directed']),
-					  node_kernels=sub_kernels,
-					  edge_kernels=sub_kernels)
+					 edge_labels=dataset.edge_labels, 
+					 node_attrs=dataset.node_attrs,
+					 edge_attrs=dataset.edge_attrs,
+					 ds_infos=dataset.get_dataset_infos(keys=['directed']),
+					 node_kernels=sub_kernels,
+					 edge_kernels=sub_kernels)
 		gram_matrix, run_time = graph_kernel.compute(dataset.graphs,
 			parallel=parallel, n_jobs=multiprocessing.cpu_count(), verbose=True)
 		kernel_list, run_time = graph_kernel.compute(dataset.graphs[0], dataset.graphs[1:],
 			parallel=parallel, n_jobs=multiprocessing.cpu_count(), verbose=True)
 		kernel, run_time = graph_kernel.compute(dataset.graphs[0], dataset.graphs[1],
 			parallel=parallel, n_jobs=multiprocessing.cpu_count(), verbose=True)
 
@@ -214,17 +224,17 @@
 	"""
 	from gklearn.kernels import PathUpToH
 	
 	dataset = chooseDataset(ds_name)
 	
 	try:
 		graph_kernel = PathUpToH(node_labels=dataset.node_labels,
-					  edge_labels=dataset.edge_labels,
-					  ds_infos=dataset.get_dataset_infos(keys=['directed']),
-					  depth=2, k_func=k_func, compute_method=compute_method)
+					 edge_labels=dataset.edge_labels,
+					 ds_infos=dataset.get_dataset_infos(keys=['directed']),
+					 depth=2, k_func=k_func, compute_method=compute_method)
 		gram_matrix, run_time = graph_kernel.compute(dataset.graphs,
 			parallel=parallel, n_jobs=multiprocessing.cpu_count(), verbose=True)
 		kernel_list, run_time = graph_kernel.compute(dataset.graphs[0], dataset.graphs[1:],
 			parallel=parallel, n_jobs=multiprocessing.cpu_count(), verbose=True)
 		kernel, run_time = graph_kernel.compute(dataset.graphs[0], dataset.graphs[1],
 			parallel=parallel, n_jobs=multiprocessing.cpu_count(), verbose=True)
 	except Exception as exception:
@@ -241,17 +251,17 @@
 	import functools
 	
 	dataset = chooseDataset(ds_name)
 
 	pkernel = functools.partial(polynomialkernel, d=2, c=1e5)	
 	try:
 		graph_kernel = Treelet(node_labels=dataset.node_labels,
-					  edge_labels=dataset.edge_labels,
-					  ds_infos=dataset.get_dataset_infos(keys=['directed']),
-					  sub_kernel=pkernel)
+					 edge_labels=dataset.edge_labels,
+					 ds_infos=dataset.get_dataset_infos(keys=['directed']),
+					 sub_kernel=pkernel)
 		gram_matrix, run_time = graph_kernel.compute(dataset.graphs,
 			parallel=parallel, n_jobs=multiprocessing.cpu_count(), verbose=True)
 		kernel_list, run_time = graph_kernel.compute(dataset.graphs[0], dataset.graphs[1:],
 			parallel=parallel, n_jobs=multiprocessing.cpu_count(), verbose=True)
 		kernel, run_time = graph_kernel.compute(dataset.graphs[0], dataset.graphs[1],
 			parallel=parallel, n_jobs=multiprocessing.cpu_count(), verbose=True)
 	except Exception as exception:
@@ -267,17 +277,17 @@
 	"""
 	from gklearn.kernels import WLSubtree
 	
 	dataset = chooseDataset(ds_name)
 
 	try:
 		graph_kernel = WLSubtree(node_labels=dataset.node_labels,
-					  edge_labels=dataset.edge_labels,
-					  ds_infos=dataset.get_dataset_infos(keys=['directed']),
-					  height=2)
+					 edge_labels=dataset.edge_labels,
+					 ds_infos=dataset.get_dataset_infos(keys=['directed']),
+					 height=2)
 		gram_matrix, run_time = graph_kernel.compute(dataset.graphs,
 			parallel=parallel, n_jobs=multiprocessing.cpu_count(), verbose=True)
 		kernel_list, run_time = graph_kernel.compute(dataset.graphs[0], dataset.graphs[1:],
 			parallel=parallel, n_jobs=multiprocessing.cpu_count(), verbose=True)
 		kernel, run_time = graph_kernel.compute(dataset.graphs[0], dataset.graphs[1],
 			parallel=parallel, n_jobs=multiprocessing.cpu_count(), verbose=True)
 	except Exception as exception:
```

### Comparing `graphkit-learn-0.2b2/gklearn/tests/test_median_preimage_generator.py` & `graphkit-learn-0.2b3/gklearn/tests/test_median_preimage_generator.py`

 * *Files 14% similar despite different names*

```diff
@@ -64,8 +64,11 @@
 	print()
 	
 	# generate preimages.
 	for fit_method in ['k-graphs', 'expert', 'random']:
 		print('\n-------------------------------------')
 		print('fit method:', fit_method, '\n')
 		mpg_options['fit_method'] = fit_method
-		generate_median_preimages_by_class(ds_name, mpg_options, kernel_options, ged_options, mge_options, save_results=save_results, save_medians=True, plot_medians=True, load_gm='auto', dir_save=dir_save, irrelevant_labels=irrelevant_labels, edge_required=edge_required, cut_range=range(0, 4))
+		try:
+			generate_median_preimages_by_class(ds_name, mpg_options, kernel_options, ged_options, mge_options, save_results=save_results, save_medians=True, plot_medians=True, load_gm='auto', dir_save=dir_save, irrelevant_labels=irrelevant_labels, edge_required=edge_required, cut_range=range(0, 4))
+		except Exception as exception:
+			assert False, exception
```

### Comparing `graphkit-learn-0.2b2/gklearn/utils/dataset.py` & `graphkit-learn-0.2b3/gklearn/utils/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -531,14 +531,34 @@
 		node_attrs = self.__node_attrs.copy() if self.__node_attrs is not None else None
 		edge_labels = self.__edge_labels.copy() if self.__edge_labels is not None else None
 		edge_attrs = self.__edge_attrs.copy() if self.__edge_attrs is not None else None
 		dataset.load_graphs(graphs, target)
 		dataset.set_labels(node_labels=node_labels, node_attrs=node_attrs, edge_labels=edge_labels, edge_attrs=edge_attrs)
 		# @todo: clean_labels and add other class members?
 		return dataset
+	
+	
+	def get_all_node_labels(self):
+		node_labels = []
+		for g in self.__graphs:
+			for n in g.nodes():
+				nl = tuple(g.nodes[n].items())
+				if nl not in node_labels:
+					node_labels.append(nl)
+		return node_labels
+	
+	
+	def get_all_edge_labels(self):
+		edge_labels = []
+		for g in self.__graphs:
+			for e in g.edges():
+				el = tuple(g.edges[e].items())
+				if el not in edge_labels:
+					edge_labels.append(el)
+		return edge_labels
 		
 	
 	def __get_dataset_size(self):
 		return len(self.__graphs)
 	
 	
 	def __get_all_node_nums(self):
```

### Comparing `graphkit-learn-0.2b2/gklearn/utils/graphdataset.py` & `graphkit-learn-0.2b3/gklearn/utils/graphdataset.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/utils/graphfiles.py` & `graphkit-learn-0.2b3/gklearn/utils/graphfiles.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/utils/graph_files.py` & `graphkit-learn-0.2b3/gklearn/utils/graph_files.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/utils/isNotebook.py` & `graphkit-learn-0.2b3/gklearn/utils/isNotebook.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/utils/kernels.py` & `graphkit-learn-0.2b3/gklearn/utils/kernels.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/utils/knn.py` & `graphkit-learn-0.2b3/gklearn/utils/knn.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/utils/logger2file.py` & `graphkit-learn-0.2b3/gklearn/utils/logger2file.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/utils/model_selection_precomputed.py` & `graphkit-learn-0.2b3/gklearn/utils/model_selection_precomputed.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
                                            param_grid_precomputed,
                                            param_grid,
                                            model_type,
                                            NUM_TRIALS=30,
                                            datafile_y=None,
                                            extra_params=None,
                                            ds_name='ds-unknown',
+										   output_dir='outputs/',
                                            n_jobs=1,
                                            read_gm_from_file=False,
                                            verbose=True):
     """Perform model selection, fitting and testing for precomputed kernels 
     using nested CV. Print out neccessary data during the process then finally 
     the results.
 
@@ -52,15 +53,15 @@
         Dictionary with names (string) of parameters used as penelties as keys 
         and lists of parameter settings to try as values. This enables 
         searching over any sequence of parameter settings. Params with length 1
         will be omitted.
     model_type : string
         Type of the problem, can be 'regression' or 'classification'.
     NUM_TRIALS : integer
-        Number of random trials of outer cv loop. The default is 30.
+        Number of random trials of the outer CV loop. The default is 30.
     datafile_y : string
         Path of file storing y data. This parameter is optional depending on 
         the given dataset file.
     extra_params : dict
         Extra parameters for loading dataset. See function gklearn.utils.
         graphfiles.loadDataset for detail.
     ds_name : string
@@ -85,17 +86,17 @@
             np.logspace(-10, 10, num=41, base=10)}]
     >>>
     >>> model_selection_for_precomputed_kernel(datafile, estimator, 
             param_grid_precomputed, param_grid[0], 'classification', ds_name=’MUTAG’)
     """
     tqdm.monitor_interval = 0
 
-    results_dir = '../notebooks/results/' + estimator.__name__
-    if not os.path.exists(results_dir):
-        os.makedirs(results_dir)
+    output_dir += estimator.__name__
+    if not os.path.exists(output_dir):
+        os.makedirs(output_dir)
     # a string to save all the results.
     str_fw = '###################### log time: ' + datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S") + '. ######################\n\n'
     str_fw += '# This file contains results of ' + estimator.__name__ + ' on dataset ' + ds_name + ',\n# including gram matrices, serial numbers for gram matrix figures and performance.\n\n'
 
     # setup the model type
     model_type = model_type.lower()
     if model_type != 'regression' and model_type != 'classification':
@@ -205,15 +206,15 @@
                     str_fw += np.array2string(
                             Kmatrix,
                             separator=',') + '\n\n'
 #                            separator=',',
 #                            threshold=np.inf,
 #                            floatmode='unique') + '\n\n'
 
-                    fig_file_name = results_dir + '/GM[ds]' + ds_name
+                    fig_file_name = output_dir + '/GM[ds]' + ds_name
                     if params_out != {}:
                         fig_file_name += '[params]' + str(idx)
                     plt.imshow(Kmatrix)
                     plt.colorbar()
                     plt.savefig(fig_file_name + '.eps', format='eps', dpi=300)
 #                    plt.show()
                     plt.clf()
@@ -240,15 +241,15 @@
             print()
         if len(gram_matrices) == 0:
             if verbose:
                 print('all gram matrices are ignored, no results obtained.')
             str_fw += '\nall gram matrices are ignored, no results obtained.\n\n'
         else:
             # save gram matrices to file.
-#            np.savez(results_dir + '/' + ds_name + '.gm', 
+#            np.savez(output_dir + '/' + ds_name + '.gm', 
 #                     gms=gram_matrices, params=param_list_pre_revised, y=y, 
 #                     gmtime=gram_matrix_time)
             if verbose:
                 print(
                 '3. Fitting and predicting using nested cross validation. This could really take a while...'
                 )
             
@@ -446,15 +447,15 @@
         param_list = list(ParameterGrid(param_grid))
     
         # read gram matrices from file.
         if verbose:
             print()
             print('2. Reading gram matrices from file...')
         str_fw += '\nII. Gram matrices.\n\nGram matrices are read from file, see last log for detail.\n'
-        gmfile = np.load(results_dir + '/' + ds_name + '.gm.npz')
+        gmfile = np.load(output_dir + '/' + ds_name + '.gm.npz')
         gram_matrices = gmfile['gms'] # a list to store gram matrices for all param_grid_precomputed
         gram_matrix_time = gmfile['gmtime'] # time used to compute the gram matrices
         param_list_pre_revised = gmfile['params'] # list to store param grids precomputed ignoring the useless ones
         y = gmfile['y'].tolist()
         
         tts = time.time()  # start training time
 #        nb_gm_ignore = 0  # the number of gram matrices those should not be considered, as they may contain elements that are not numbers (NaN)            
@@ -599,29 +600,29 @@
             print('total training time with all hyper-param choices: {:.2f}s'.format(
                     tt_poster + np.sum(gram_matrix_time)))
 #        str_fw += 'time to calculate gram matrix with different hyper-params: {:.2f}±{:.2f}s\n'.format(average_gram_matrix_time, std_gram_matrix_time)
 #        str_fw += 'time to calculate best gram matrix: {:.2f}±{:.2f}s\n'.format(ave_bgmt, std_bgmt)
         str_fw += 'training time with hyper-param choices who did not participate in calculation of gram matrices: {:.2f}s\n\n'.format(tt_poster)
 
         # open file to save all results for this dataset.
-        if not os.path.exists(results_dir):
-            os.makedirs(results_dir)
+        if not os.path.exists(output_dir):
+            os.makedirs(output_dir)
             
     # print out results as table.
     str_fw += printResultsInTable(param_list, param_list_pre_revised, average_val_scores,
               std_val_scores, average_perf_scores, std_perf_scores,
               average_train_scores, std_train_scores, gram_matrix_time,
               model_type, verbose)
             
     # open file to save all results for this dataset.
-    if not os.path.exists(results_dir + '/' + ds_name + '.output.txt'):
-        with open(results_dir + '/' + ds_name + '.output.txt', 'w') as f:
+    if not os.path.exists(output_dir + '/' + ds_name + '.output.txt'):
+        with open(output_dir + '/' + ds_name + '.output.txt', 'w') as f:
             f.write(str_fw)
     else:
-        with open(results_dir + '/' + ds_name + '.output.txt', 'r+') as f:
+        with open(output_dir + '/' + ds_name + '.output.txt', 'r+') as f:
             content = f.read()
             f.seek(0, 0)
             f.write(str_fw + '\n\n\n' + content)
 
 
 def trial_do(param_list_pre_revised, param_list, gram_matrices, y, model_type, trial): # Test set level
 
@@ -793,15 +794,15 @@
     train_pref, val_pref, test_pref = trial_do(param_list_pre_revised, 
                                                param_list, G_gms, y, 
                                                model_type, trial)
     return train_pref, val_pref, test_pref
 
 
 def compute_gram_matrices(dataset, y, estimator, param_list_precomputed, 
-                          results_dir, ds_name,
+                          output_dir, ds_name,
                           n_jobs=1, str_fw='', verbose=True):
     gram_matrices = [
         ]  # a list to store gram matrices for all param_grid_precomputed
     gram_matrix_time = [
         ]  # a list to store time to calculate gram matrices
     param_list_pre_revised = [
         ]  # list to store param grids precomputed ignoring the useless ones
@@ -863,15 +864,15 @@
                 str_fw += np.array2string(
                         Kmatrix,
                         separator=',') + '\n\n'
 #                            separator=',',
 #                            threshold=np.inf,
 #                            floatmode='unique') + '\n\n'
 
-                fig_file_name = results_dir + '/GM[ds]' + ds_name
+                fig_file_name = output_dir + '/GM[ds]' + ds_name
                 if params_out != {}:
                     fig_file_name += '[params]' + str(idx)
                 plt.imshow(Kmatrix)
                 plt.colorbar()
                 plt.savefig(fig_file_name + '.eps', format='eps', dpi=300)
 #                    plt.show()
                 plt.clf()
@@ -893,16 +894,16 @@
         '{}: {}\n'.format(idx, params_out)
         for idx, params_out in enumerate(param_list_precomputed)
     ])
             
     return gram_matrices, gram_matrix_time, param_list_pre_revised, y, str_fw
 
 
-def read_gram_matrices_from_file(results_dir, ds_name):
-    gmfile = np.load(results_dir + '/' + ds_name + '.gm.npz')
+def read_gram_matrices_from_file(output_dir, ds_name):
+    gmfile = np.load(output_dir + '/' + ds_name + '.gm.npz')
     gram_matrices = gmfile['gms'] # a list to store gram matrices for all param_grid_precomputed
     param_list_pre_revised = gmfile['params'] # list to store param grids precomputed ignoring the useless ones
     y = gmfile['y'].tolist()
     return gram_matrices, param_list_pre_revised, y
 
 
 def printResultsInTable(param_list, param_list_pre_revised, average_val_scores,
```

### Comparing `graphkit-learn-0.2b2/gklearn/utils/parallel.py` & `graphkit-learn-0.2b3/gklearn/utils/parallel.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import multiprocessing
 from multiprocessing import Pool
 from tqdm import tqdm
 import sys
 
 def parallel_me(func, func_assign, var_to_assign, itr, len_itr=None, init_worker=None, 
                 glbv=None, method=None, n_jobs=None, chunksize=None, itr_desc='',
-                verbose=2):
+                verbose=True):
     '''
     '''
     if method == 'imap_unordered':
         if glbv: # global varibles required.
 #            def init_worker(v_share):
 #                global G_var
 #                G_var = v_share
@@ -26,39 +26,39 @@
                       initargs=glbv) as pool:                
                 if chunksize == None:
                     if len_itr < 100 * n_jobs:
                         chunksize = int(len_itr / n_jobs) + 1
                     else:
                         chunksize = 100
                 for result in (tqdm(pool.imap_unordered(func, itr, chunksize),
-                    desc=itr_desc, file=sys.stdout) if verbose == 2 else 
+                    desc=itr_desc, file=sys.stdout) if verbose else 
                     pool.imap_unordered(func, itr, chunksize)):
                     func_assign(result, var_to_assign)
             pool.close()
             pool.join()
         else:
             if n_jobs == None:
                 n_jobs = multiprocessing.cpu_count()
             with Pool(processes=n_jobs) as pool:
                 if chunksize == None:
                     if len_itr < 100 * n_jobs:
                         chunksize = int(len_itr / n_jobs) + 1
                     else:
                         chunksize = 100
                 for result in (tqdm(pool.imap_unordered(func, itr, chunksize),
-                    desc=itr_desc, file=sys.stdout) if verbose == 2 else 
+                    desc=itr_desc, file=sys.stdout) if verbose else 
                     pool.imap_unordered(func, itr, chunksize)):
                     func_assign(result, var_to_assign)
             pool.close()
             pool.join()
                     
 
 def parallel_gm(func, Kmatrix, Gn, init_worker=None, glbv=None, 
                 method='imap_unordered', n_jobs=None, chunksize=None, 
-                verbose=True):
+                verbose=True): # @todo: Gn seems not necessary.
     from itertools import combinations_with_replacement
     def func_assign(result, var_to_assign):
         var_to_assign[result[0]][result[1]] = result[2]
         var_to_assign[result[1]][result[0]] = result[2]
     itr = combinations_with_replacement(range(0, len(Gn)), 2)
     len_itr = int(len(Gn) * (len(Gn) + 1) / 2)
     parallel_me(func, func_assign, Kmatrix, itr, len_itr=len_itr,
```

### Comparing `graphkit-learn-0.2b2/gklearn/utils/timer.py` & `graphkit-learn-0.2b3/gklearn/utils/timer.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/utils/trie.py` & `graphkit-learn-0.2b3/gklearn/utils/trie.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/gklearn/utils/utils.py` & `graphkit-learn-0.2b3/gklearn/utils/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -218,14 +218,78 @@
 
 	# relabel nodes using consecutive integers for convenience of kernel calculation.
 	# gt = nx.convert_node_labels_to_integers(
 	#	 gt, first_label=0, label_attribute='label_orignal')
 	return gt
 
 
+def direct_product_graph(G1, G2, node_labels, edge_labels):
+	"""Return the direct/tensor product of directed graphs G1 and G2.
+
+	Parameters
+	----------
+	G1, G2 : NetworkX graph
+		The original graphs.
+	node_labels : list
+		A list of node attributes used as labels.
+	edge_labels : list
+		A list of edge attributes used as labels.
+		
+	Return
+	------
+	gt : NetworkX graph
+		The direct product graph of G1 and G2.
+
+	Notes
+	-----
+	This method differs from networkx.tensor_product in that this method only adds nodes and edges in G1 and G2 that have the same labels to the direct product graph.
+
+	References
+	----------
+	.. [1] Thomas Gärtner, Peter Flach, and Stefan Wrobel. On graph kernels: Hardness results and efficient alternatives. Learning Theory and Kernel Machines, pages 129–143, 2003.
+	"""
+	# arrange all graphs in a list
+	from itertools import product
+	# G = G.to_directed()
+	gt = nx.DiGraph()
+	# add nodes
+	for u, v in product(G1, G2):
+		label1 = tuple(G1.nodes[u][nl] for nl in node_labels)
+		label2 = tuple(G2.nodes[v][nl] for nl in node_labels)
+		if label1 == label2:
+			gt.add_node((u, v), node_label=label1)
+
+	# add edges, faster for sparse graphs (no so many edges), which is the most case for now.
+	for (u1, v1), (u2, v2) in product(G1.edges, G2.edges):
+		if (u1, u2) in gt and (v1, v2) in gt:
+			label1 = tuple(G1.edges[u1, v1][el] for el in edge_labels)
+			label2 = tuple(G2.edges[u2, v2][el] for el in edge_labels)
+			if label1 == label2:
+				gt.add_edge((u1, u2), (v1, v2), edge_label=label1)
+
+
+	# # add edges, faster for dense graphs (a lot of edges, complete graph would be super).
+	# for u, v in product(gt, gt):
+	#	 if (u[0], v[0]) in G1.edges and (
+	#			 u[1], v[1]
+	#	 ) in G2.edges and G1.edges[u[0],
+	#								v[0]][edge_label] == G2.edges[u[1],
+	#															  v[1]][edge_label]:
+	#		 gt.add_edge((u[0], u[1]), (v[0], v[1]))
+	#		 gt.edges[(u[0], u[1]), (v[0], v[1])].update({
+	#			 edge_label:
+	#			 G1.edges[u[0], v[0]][edge_label]
+	#		 })
+
+	# relabel nodes using consecutive integers for convenience of kernel calculation.
+	# gt = nx.convert_node_labels_to_integers(
+	#	 gt, first_label=0, label_attribute='label_orignal')
+	return gt
+
+
 def graph_deepcopy(G):
 	"""Deep copy a graph, including deep copy of all nodes, edges and 
 	attributes of the graph, nodes and edges.
 	
 	Note
 	----
 	It is the same as the NetworkX function graph.copy(), as far as I know.
@@ -296,15 +360,21 @@
 	el = set()
 	for G in Gn:
 		el = el | set(nx.get_edge_attributes(G, edge_label).values())
 	return el
 
 
 def get_graph_kernel_by_name(name, node_labels=None, edge_labels=None, node_attrs=None, edge_attrs=None, ds_infos=None, kernel_options={}):
-	if name == 'ShortestPath':
+	if name == 'Marginalized':
+		from gklearn.kernels import Marginalized
+		graph_kernel = Marginalized(node_labels=node_labels,
+								 edge_labels=edge_labels,
+								 ds_infos=ds_infos,
+								 **kernel_options)
+	elif name == 'ShortestPath':
 		from gklearn.kernels import ShortestPath
 		graph_kernel = ShortestPath(node_labels=node_labels,
 								 node_attrs=node_attrs,
 								 ds_infos=ds_infos,
 								 **kernel_options)
 	elif name == 'StructuralSP':
 		from gklearn.kernels import StructuralSP
@@ -462,22 +532,14 @@
 
 
 def get_mlti_dim_edge_attrs(G, attr_names):
 	attributes = []
 	for ed, attrs in G.edges(data=True):
 		attributes.append(tuple(attrs[aname] for aname in attr_names))
 	return attributes
-
-
-@unique
-class SpecialLabel(Enum):
-	"""can be used to define special labels.
-	"""
-	DUMMY = 1 # The dummy label.
-	# DUMMY = auto # enum.auto does not exist in Python 3.5.
 	
 	
 def normalize_gram_matrix(gram_matrix):
 	diag = gram_matrix.diagonal().copy()
 	for i in range(len(gram_matrix)):
 		for j in range(i, len(gram_matrix)):
 			gram_matrix[i][j] /= np.sqrt(diag[i] * diag[j])
@@ -496,8 +558,48 @@
 				else:
 					raise ValueError('The distance is negative.')
 			dis_mat[i, j] = np.sqrt(dis)
 			dis_mat[j, i] = dis_mat[i, j]
 	dis_max = np.max(np.max(dis_mat))
 	dis_min = np.min(np.min(dis_mat[dis_mat != 0]))
 	dis_mean = np.mean(np.mean(dis_mat))
-	return dis_mat, dis_max, dis_min, dis_mean
+	return dis_mat, dis_max, dis_min, dis_mean
+
+
+def dummy_node():
+	"""
+	/*!
+	 * @brief Returns a dummy node.
+	 * @return ID of dummy node.
+	 */
+	"""
+	return np.inf # @todo: in GEDLIB, this is the max - 1 rather than max, I don't know why.
+
+
+def undefined_node():
+	"""
+	/*!
+	 * @brief Returns an undefined node.
+	 * @return ID of undefined node.
+	 */
+
+	"""
+	return np.inf
+
+
+def dummy_edge():
+	"""
+	/*!
+	 * @brief Returns a dummy edge.
+	 * @return ID of dummy edge.
+	 */
+
+	"""
+	return np.inf
+
+
+@unique
+class SpecialLabel(Enum):
+	"""can be used to define special labels.
+	"""
+	DUMMY = 1 # The dummy label.
+	# DUMMY = auto # enum.auto does not exist in Python 3.5.
```

### Comparing `graphkit-learn-0.2b2/gklearn/utils/__init__.py` & `graphkit-learn-0.2b3/gklearn/utils/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,11 +16,12 @@
 # from utils import graphfiles
 # from utils import utils
 from gklearn.utils.dataset import Dataset, split_dataset_by_target
 from gklearn.utils.graph_files import load_dataset, save_dataset
 from gklearn.utils.timer import Timer
 from gklearn.utils.utils import get_graph_kernel_by_name
 from gklearn.utils.utils import compute_gram_matrices_by_class
-from gklearn.utils.utils import SpecialLabel
+from gklearn.utils.utils import SpecialLabel, dummy_node, undefined_node, dummy_edge
 from gklearn.utils.utils import normalize_gram_matrix, compute_distance_matrix
 from gklearn.utils.trie import Trie
 from gklearn.utils.knn import knn_cv, knn_classification
+from gklearn.utils.model_selection_precomputed import model_selection_for_precomputed_kernel
```

### Comparing `graphkit-learn-0.2b2/gklearn/__init__.py` & `graphkit-learn-0.2b3/gklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `graphkit-learn-0.2b2/graphkit_learn.egg-info/PKG-INFO` & `graphkit-learn-0.2b3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,133 +1,169 @@
-Metadata-Version: 2.1
-Name: graphkit-learn
-Version: 0.2b2
-Summary: A Python library for graph kernels, graph edit distances, and graph pre-images
-Home-page: https://github.com/jajupmochi/graphkit-learn
-Author: Linlin Jia
-Author-email: linlin.jia@insa-rouen.fr
-License: UNKNOWN
-Description: # graphkit-learn
-        [![Build Status](https://travis-ci.org/jajupmochi/graphkit-learn.svg?branch=master)](https://travis-ci.org/jajupmochi/graphkit-learn)
-        [![Build status](https://ci.appveyor.com/api/projects/status/bdxsolk0t1uji9rd?svg=true)](https://ci.appveyor.com/project/jajupmochi/graphkit-learn)
-        [![codecov](https://codecov.io/gh/jajupmochi/graphkit-learn/branch/master/graph/badge.svg)](https://codecov.io/gh/jajupmochi/graphkit-learn)
-        [![Documentation Status](https://readthedocs.org/projects/graphkit-learn/badge/?version=master)](https://graphkit-learn.readthedocs.io/en/master/?badge=master)
-        [![PyPI version](https://badge.fury.io/py/graphkit-learn.svg)](https://badge.fury.io/py/graphkit-learn)
-        
-        A Python package for graph kernels, graph edit distances and graph pre-image problem.
-        
-        ## Requirements
-        
-        * python>=3.5
-        * numpy>=1.16.2
-        * scipy>=1.1.0
-        * matplotlib>=3.0.0
-        * networkx>=2.2
-        * scikit-learn>=0.20.0
-        * tabulate>=0.8.2
-        * tqdm>=4.26.0
-        * control==0.8.0 (for generalized random walk kernels only)
-        * slycot==0.3.3 (for generalized random walk kernels only, which requires a fortran compiler, gfortran for example)
-        
-        ## How to use?
-        
-        Simply clone this repository and voilà! Then check [`notebooks`](https://github.com/jajupmochi/graphkit-learn/tree/master/notebooks) directory for demos:
-        * [`notebooks`](https://github.com/jajupmochi/graphkit-learn/tree/master/notebooks) directory includes test codes of graph kernels based on linear patterns;
-        * [`notebooks/tests`](https://github.com/jajupmochi/graphkit-learn/tree/master/notebooks/tests) directory includes codes that test some libraries and functions;
-        * [`notebooks/utils`](https://github.com/jajupmochi/graphkit-learn/tree/master/notebooks/utils) directory includes some useful tools, such as a Gram matrix checker and a function to get properties of datasets;
-        * [`notebooks/else`](https://github.com/jajupmochi/graphkit-learn/tree/master/notebooks/else) directory includes other codes that we used for experiments.
-        
-        ## List of graph kernels
-        
-        * Based on walks
-          * The common walk kernel [1]
-            * Exponential
-            * Geometric
-          * The marginalized kenrel
-            * With tottering [2]
-            * Without tottering [7]
-          * The generalized random walk kernel [3]
-            * Sylvester equation
-            * Conjugate gradient
-            * Fixed-point iterations
-            * Spectral decomposition
-        * Based on paths
-          * The shortest path kernel [4]
-          * The structural shortest path kernel [5]
-          * The path kernel up to length h [6]
-            * The Tanimoto kernel
-            * The MinMax kernel
-        * Non-linear kernels
-          * The treelet kernel [10]
-          * Weisfeiler-Lehman kernel [11]
-            * Subtree
-        
-        ## Computation optimization methods
-        
-        * Python’s `multiprocessing.Pool` module is applied to perform **parallelization** on the computations of all kernels as well as the model selection.
-        * **The Fast Computation of Shortest Path Kernel (FCSP) method** [8] is implemented in *the random walk kernel*, *the shortest path kernel*, as well as *the structural shortest path kernel* where FCSP is applied on both vertex and edge kernels.
-        * **The trie data structure** [9] is employed in *the path kernel up to length h* to store paths in graphs.
-        
-        ## Issues
-        
-        * This library uses `multiprocessing.Pool.imap_unordered` function to do the parallelization, which may not be able to run correctly under Windows system. For now, Windows users may need to comment the parallel codes and uncomment the codes below them which run serially. We will consider adding a parameter to control serial or parallel computations as needed.
-        
-        * Some modules (such as `Numpy`, `Scipy`, `sklearn`) apply [`OpenBLAS`](https://www.openblas.net/) to perform parallel computation by default, which causes conflicts with other parallelization modules such as `multiprossing.Pool`, highly increasing the computing time. By setting its thread to 1, `OpenBLAS` is forced to use a single thread/CPU, thus avoids the conflicts. For now, this procedure has to be done manually. Under Linux, type this command in terminal before running the code:
-        ```
-        $ export OPENBLAS_NUM_THREADS=1
-        ```
-        Or add `export OPENBLAS_NUM_THREADS=1` at the end of your `~/.bashrc` file, then run
-        ```
-        $ source ~/.bashrc
-        ```
-        to make this effective permanently.
-        
-        ## Results
-        
-        Check this paper for detailed description of graph kernels and experimental results:
-        
-        Linlin Jia, Benoit Gaüzère, and Paul Honeine. Graph Kernels Based on Linear Patterns: Theoretical and Experimental Comparisons. working paper or preprint, March 2019. URL https://hal-normandie-univ.archives-ouvertes.fr/hal-02053946.
-        
-        A comparison of performances of graph kernels on benchmark datasets can be found [here](https://graphkit-learn.readthedocs.io/en/master/experiments.html).
-        
-        ## References
-        [1] Thomas Gärtner, Peter Flach, and Stefan Wrobel. On graph kernels: Hardness results and efficient alternatives. Learning Theory and Kernel Machines, pages 129–143, 2003.
-        
-        [2] H. Kashima, K. Tsuda, and A. Inokuchi. Marginalized kernels between labeled graphs. In Proceedings of the 20th International Conference on Machine Learning, Washington, DC, United States, 2003.
-        
-        [3] Vishwanathan, S.V.N., Schraudolph, N.N., Kondor, R., Borgwardt, K.M., 2010. Graph kernels. Journal of Machine Learning Research 11, 1201–1242.
-        
-        [4] K. M. Borgwardt and H.-P. Kriegel. Shortest-path kernels on graphs. In Proceedings of the International Conference on Data Mining, pages 74-81, 2005.
-        
-        [5] Liva Ralaivola, Sanjay J Swamidass, Hiroto Saigo, and Pierre Baldi. Graph kernels for chemical informatics. Neural networks, 18(8):1093–1110, 2005.
-        
-        [6] Suard F, Rakotomamonjy A, Bensrhair A. Kernel on Bag of Paths For Measuring Similarity of Shapes. InESANN 2007 Apr 25 (pp. 355-360).
-        
-        [7] Mahé, P., Ueda, N., Akutsu, T., Perret, J.L., Vert, J.P., 2004. Extensions of marginalized graph kernels, in: Proc. the twenty-first international conference on Machine learning, ACM. p. 70.
-        
-        [8] Lifan Xu, Wei Wang, M Alvarez, John Cavazos, and Dongping Zhang. Parallelization of shortest path graph kernels on multi-core cpus and gpus. Proceedings of the Programmability Issues for Heterogeneous Multicores (MultiProg), Vienna, Austria, 2014.
-        
-        [9] Edward Fredkin. Trie memory. Communications of the ACM, 3(9):490–499, 1960.
-        
-        [10] Gaüzere, B., Brun, L., Villemin, D., 2012. Two new graphs kernels in chemoinformatics. Pattern Recognition Letters 33, 2038–2047.
-        
-        [11] Shervashidze, N., Schweitzer, P., Leeuwen, E.J.v., Mehlhorn, K., Borgwardt, K.M., 2011. Weisfeiler-lehman graph kernels. Journal of Machine Learning Research 12, 2539–2561.
-        
-        ## Authors
-        
-        * [Linlin Jia](https://jajupmochi.github.io/), LITIS, INSA Rouen Normandie
-        * [Benoit Gaüzère](http://pagesperso.litislab.fr/~bgauzere/#contact_en), LITIS, INSA Rouen Normandie
-        * [Paul Honeine](http://honeine.fr/paul/Welcome.html), LITIS, Université de Rouen Normandie
-        
-        ## Citation
-        
-        Still waiting...
-        
-        ## Acknowledgments
-        
-        This research was supported by CSC (China Scholarship Council) and the French national research agency (ANR) under the grant APi (ANR-18-CE23-0014). The authors would like to thank the CRIANN (Le Centre Régional Informatique et d’Applications Numériques de Normandie) for providing computational resources.
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
+# graphkit-learn
+[![Build Status](https://travis-ci.org/jajupmochi/graphkit-learn.svg?branch=master)](https://travis-ci.org/jajupmochi/graphkit-learn)
+[![Build status](https://ci.appveyor.com/api/projects/status/bdxsolk0t1uji9rd?svg=true)](https://ci.appveyor.com/project/jajupmochi/graphkit-learn)
+[![codecov](https://codecov.io/gh/jajupmochi/graphkit-learn/branch/master/graph/badge.svg)](https://codecov.io/gh/jajupmochi/graphkit-learn)
+[![Documentation Status](https://readthedocs.org/projects/graphkit-learn/badge/?version=master)](https://graphkit-learn.readthedocs.io/en/master/?badge=master)
+[![PyPI version](https://badge.fury.io/py/graphkit-learn.svg)](https://badge.fury.io/py/graphkit-learn)
+
+A Python package for graph kernels, graph edit distances and graph pre-image problem.
+
+## Requirements
+
+* python>=3.5
+* numpy>=1.16.2
+* scipy>=1.1.0
+* matplotlib>=3.1.0
+* networkx>=2.2
+* scikit-learn>=0.20.0
+* tabulate>=0.8.2
+* tqdm>=4.26.0
+* control>=0.8.2 (for generalized random walk kernels only)
+* slycot==0.3.3 (for generalized random walk kernels only, which requires a fortran compiler, gfortran for example)
+
+## How to use?
+
+### Install the library
+
+* Install stable version from PyPI (may not be up-to-date):
+```
+$ pip install graphkit-learn
+```
+
+* Install latest version from GitHub:
+```
+$ git clone https://github.com/jajupmochi/graphkit-learn.git
+$ cd graphkit-learn/
+$ python setup.py install
+```
+
+### Run the test
+
+A series of [tests](https://github.com/jajupmochi/graphkit-learn/tree/master/gklearn/tests) can be run to check if the library works correctly:
+```
+$ pip install -U pip pytest codecov coverage pytest-cov
+$ pytest -v --cov-config=.coveragerc --cov-report term --cov=gklearn gklearn/tests/
+```
+
+### Check examples
+
+A series of demos of using the library can be found on [Google Colab](https://drive.google.com/drive/folders/1r2gtPuFzIys2_MZw1wXqE2w3oCoVoQUG?usp=sharing) and in the [`example`](https://github.com/jajupmochi/graphkit-learn/tree/master/gklearn/examples) folder.
+
+### Other demos
+
+Check [`notebooks`](https://github.com/jajupmochi/graphkit-learn/tree/master/notebooks) directory for more demos:
+* [`notebooks`](https://github.com/jajupmochi/graphkit-learn/tree/master/notebooks) directory includes test codes of graph kernels based on linear patterns;
+* [`notebooks/tests`](https://github.com/jajupmochi/graphkit-learn/tree/master/notebooks/tests) directory includes codes that test some libraries and functions;
+* [`notebooks/utils`](https://github.com/jajupmochi/graphkit-learn/tree/master/notebooks/utils) directory includes some useful tools, such as a Gram matrix checker and a function to get properties of datasets;
+* [`notebooks/else`](https://github.com/jajupmochi/graphkit-learn/tree/master/notebooks/else) directory includes other codes that we used for experiments.
+
+### Documentation
+
+The docs of the library can be found [here](https://graphkit-learn.readthedocs.io/en/master/?badge=master).
+
+## Main contents
+
+### 1 List of graph kernels
+
+* Based on walks
+  * [The common walk kernel](gklearn/kernels/common_walk.py) [1]
+    * Exponential
+    * Geometric
+  * [The marginalized kenrel](gklearn/kernels/marginalized.py)
+    * With tottering [2]
+    * Without tottering [7]
+  * [The generalized random walk kernel](gklearn/kernels/random_walk.py) [3]
+    * [Sylvester equation](gklearn/kernels/sylvester_equation.py)
+    * Conjugate gradient
+    * Fixed-point iterations
+    * [Spectral decomposition](gklearn/kernels/spectral_decomposition.py)
+* Based on paths
+  * [The shortest path kernel](gklearn/kernels/shortest_path.py) [4]
+  * [The structural shortest path kernel](gklearn/kernels/structural_sp.py) [5]
+  * [The path kernel up to length h](gklearn/kernels/path_up_to_h.py) [6]
+    * The Tanimoto kernel
+    * The MinMax kernel
+* Non-linear kernels
+  * [The treelet kernel](gklearn/kernels/treelet.py) [10]
+  * [Weisfeiler-Lehman kernel](gklearn/kernels/weisfeiler_lehman.py) [11]
+    * [Subtree](gklearn/kernels/weisfeiler_lehman.py#L479)
+
+A demo of computing graph kernels can be found on [Google Colab](https://colab.research.google.com/drive/17Q2QCl9CAtDweGF8LiWnWoN2laeJqT0u?usp=sharing) and in the [`examples`](https://github.com/jajupmochi/graphkit-learn/blob/master/gklearn/examples/compute_graph_kernel.py) folder.
+
+### 2 Graph Edit Distances
+
+### 3 Graph preimage methods
+
+A demo of generating graph preimages can be found on [Google Colab](https://colab.research.google.com/drive/1PIDvHOcmiLEQ5Np3bgBDdu0kLOquOMQK?usp=sharing) and in the [`examples`](https://github.com/jajupmochi/graphkit-learn/blob/master/gklearn/examples/median_preimege_generator.py) folder.
+
+### 4 Interface to `GEDLIB`
+
+[`GEDLIB`](https://github.com/dbblumenthal/gedlib) is an easily extensible C++ library for (suboptimally) computing the graph edit distance between attributed graphs. [A Python interface](gklearn/gedlib) for `GEDLIB` is integrated in this library, based on [`gedlibpy`](https://github.com/Ryurin/gedlibpy) library.
+
+### 5 Computation optimization methods
+
+* Python’s `multiprocessing.Pool` module is applied to perform **parallelization** on the computations of all kernels as well as the model selection.
+* **The Fast Computation of Shortest Path Kernel (FCSP) method** [8] is implemented in *the random walk kernel*, *the shortest path kernel*, as well as *the structural shortest path kernel* where FCSP is applied on both vertex and edge kernels.
+* **The trie data structure** [9] is employed in *the path kernel up to length h* to store paths in graphs.
+
+## Issues
+
+* This library uses `multiprocessing.Pool.imap_unordered` function to do the parallelization, which may not be able to run correctly under Windows system. For now, Windows users may need to comment the parallel codes and uncomment the codes below them which run serially. We will consider adding a parameter to control serial or parallel computations as needed.
+
+* Some modules (such as `Numpy`, `Scipy`, `sklearn`) apply [`OpenBLAS`](https://www.openblas.net/) to perform parallel computation by default, which causes conflicts with other parallelization modules such as `multiprossing.Pool`, highly increasing the computing time. By setting its thread to 1, `OpenBLAS` is forced to use a single thread/CPU, thus avoids the conflicts. For now, this procedure has to be done manually. Under Linux, type this command in terminal before running the code:
+```
+$ export OPENBLAS_NUM_THREADS=1
+```
+Or add `export OPENBLAS_NUM_THREADS=1` at the end of your `~/.bashrc` file, then run
+```
+$ source ~/.bashrc
+```
+to make this effective permanently.
+
+## Results
+
+Check this paper for detailed description of graph kernels and experimental results:
+
+Linlin Jia, Benoit Gaüzère, and Paul Honeine. Graph Kernels Based on Linear Patterns: Theoretical and Experimental Comparisons. working paper or preprint, March 2019. URL https://hal-normandie-univ.archives-ouvertes.fr/hal-02053946.
+
+A comparison of performances of graph kernels on benchmark datasets can be found [here](https://graphkit-learn.readthedocs.io/en/master/experiments.html).
+
+## How to contribute
+
+Fork the library and open a pull request! Make your own contribute to the community!
+
+## References
+[1] Thomas Gärtner, Peter Flach, and Stefan Wrobel. On graph kernels: Hardness results and efficient alternatives. Learning Theory and Kernel Machines, pages 129–143, 2003.
+
+[2] H. Kashima, K. Tsuda, and A. Inokuchi. Marginalized kernels between labeled graphs. In Proceedings of the 20th International Conference on Machine Learning, Washington, DC, United States, 2003.
+
+[3] Vishwanathan, S.V.N., Schraudolph, N.N., Kondor, R., Borgwardt, K.M., 2010. Graph kernels. Journal of Machine Learning Research 11, 1201–1242.
+
+[4] K. M. Borgwardt and H.-P. Kriegel. Shortest-path kernels on graphs. In Proceedings of the International Conference on Data Mining, pages 74-81, 2005.
+
+[5] Liva Ralaivola, Sanjay J Swamidass, Hiroto Saigo, and Pierre Baldi. Graph kernels for chemical informatics. Neural networks, 18(8):1093–1110, 2005.
+
+[6] Suard F, Rakotomamonjy A, Bensrhair A. Kernel on Bag of Paths For Measuring Similarity of Shapes. InESANN 2007 Apr 25 (pp. 355-360).
+
+[7] Mahé, P., Ueda, N., Akutsu, T., Perret, J.L., Vert, J.P., 2004. Extensions of marginalized graph kernels, in: Proc. the twenty-first international conference on Machine learning, ACM. p. 70.
+
+[8] Lifan Xu, Wei Wang, M Alvarez, John Cavazos, and Dongping Zhang. Parallelization of shortest path graph kernels on multi-core cpus and gpus. Proceedings of the Programmability Issues for Heterogeneous Multicores (MultiProg), Vienna, Austria, 2014.
+
+[9] Edward Fredkin. Trie memory. Communications of the ACM, 3(9):490–499, 1960.
+
+[10] Gaüzere, B., Brun, L., Villemin, D., 2012. Two new graphs kernels in chemoinformatics. Pattern Recognition Letters 33, 2038–2047.
+
+[11] Shervashidze, N., Schweitzer, P., Leeuwen, E.J.v., Mehlhorn, K., Borgwardt, K.M., 2011. Weisfeiler-lehman graph kernels. Journal of Machine Learning Research 12, 2539–2561.
+
+## Authors
+
+* [Linlin Jia](https://jajupmochi.github.io/), LITIS, INSA Rouen Normandie
+* [Benoit Gaüzère](http://pagesperso.litislab.fr/~bgauzere/#contact_en), LITIS, INSA Rouen Normandie
+* [Paul Honeine](http://honeine.fr/paul/Welcome.html), LITIS, Université de Rouen Normandie
+
+## Citation
+
+Still waiting...
+
+## Acknowledgments
+
+This research was supported by CSC (China Scholarship Council) and the French national research agency (ANR) under the grant APi (ANR-18-CE23-0014). The authors would like to thank the CRIANN (Le Centre Régional Informatique et d’Applications Numériques de Normandie) for providing computational resources.
```

### Comparing `graphkit-learn-0.2b2/PKG-INFO` & `graphkit-learn-0.2b3/graphkit_learn.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphkit-learn
-Version: 0.2b2
+Version: 0.2b3
 Summary: A Python library for graph kernels, graph edit distances, and graph pre-images
 Home-page: https://github.com/jajupmochi/graphkit-learn
 Author: Linlin Jia
 Author-email: linlin.jia@insa-rouen.fr
 License: UNKNOWN
 Description: # graphkit-learn
         [![Build Status](https://travis-ci.org/jajupmochi/graphkit-learn.svg?branch=master)](https://travis-ci.org/jajupmochi/graphkit-learn)
@@ -16,56 +16,102 @@
         A Python package for graph kernels, graph edit distances and graph pre-image problem.
         
         ## Requirements
         
         * python>=3.5
         * numpy>=1.16.2
         * scipy>=1.1.0
-        * matplotlib>=3.0.0
+        * matplotlib>=3.1.0
         * networkx>=2.2
         * scikit-learn>=0.20.0
         * tabulate>=0.8.2
         * tqdm>=4.26.0
-        * control==0.8.0 (for generalized random walk kernels only)
+        * control>=0.8.2 (for generalized random walk kernels only)
         * slycot==0.3.3 (for generalized random walk kernels only, which requires a fortran compiler, gfortran for example)
         
         ## How to use?
         
-        Simply clone this repository and voilà! Then check [`notebooks`](https://github.com/jajupmochi/graphkit-learn/tree/master/notebooks) directory for demos:
+        ### Install the library
+        
+        * Install stable version from PyPI (may not be up-to-date):
+        ```
+        $ pip install graphkit-learn
+        ```
+        
+        * Install latest version from GitHub:
+        ```
+        $ git clone https://github.com/jajupmochi/graphkit-learn.git
+        $ cd graphkit-learn/
+        $ python setup.py install
+        ```
+        
+        ### Run the test
+        
+        A series of [tests](https://github.com/jajupmochi/graphkit-learn/tree/master/gklearn/tests) can be run to check if the library works correctly:
+        ```
+        $ pip install -U pip pytest codecov coverage pytest-cov
+        $ pytest -v --cov-config=.coveragerc --cov-report term --cov=gklearn gklearn/tests/
+        ```
+        
+        ### Check examples
+        
+        A series of demos of using the library can be found on [Google Colab](https://drive.google.com/drive/folders/1r2gtPuFzIys2_MZw1wXqE2w3oCoVoQUG?usp=sharing) and in the [`example`](https://github.com/jajupmochi/graphkit-learn/tree/master/gklearn/examples) folder.
+        
+        ### Other demos
+        
+        Check [`notebooks`](https://github.com/jajupmochi/graphkit-learn/tree/master/notebooks) directory for more demos:
         * [`notebooks`](https://github.com/jajupmochi/graphkit-learn/tree/master/notebooks) directory includes test codes of graph kernels based on linear patterns;
         * [`notebooks/tests`](https://github.com/jajupmochi/graphkit-learn/tree/master/notebooks/tests) directory includes codes that test some libraries and functions;
         * [`notebooks/utils`](https://github.com/jajupmochi/graphkit-learn/tree/master/notebooks/utils) directory includes some useful tools, such as a Gram matrix checker and a function to get properties of datasets;
         * [`notebooks/else`](https://github.com/jajupmochi/graphkit-learn/tree/master/notebooks/else) directory includes other codes that we used for experiments.
         
-        ## List of graph kernels
+        ### Documentation
+        
+        The docs of the library can be found [here](https://graphkit-learn.readthedocs.io/en/master/?badge=master).
+        
+        ## Main contents
+        
+        ### 1 List of graph kernels
         
         * Based on walks
-          * The common walk kernel [1]
+          * [The common walk kernel](gklearn/kernels/common_walk.py) [1]
             * Exponential
             * Geometric
-          * The marginalized kenrel
+          * [The marginalized kenrel](gklearn/kernels/marginalized.py)
             * With tottering [2]
             * Without tottering [7]
-          * The generalized random walk kernel [3]
-            * Sylvester equation
+          * [The generalized random walk kernel](gklearn/kernels/random_walk.py) [3]
+            * [Sylvester equation](gklearn/kernels/sylvester_equation.py)
             * Conjugate gradient
             * Fixed-point iterations
-            * Spectral decomposition
+            * [Spectral decomposition](gklearn/kernels/spectral_decomposition.py)
         * Based on paths
-          * The shortest path kernel [4]
-          * The structural shortest path kernel [5]
-          * The path kernel up to length h [6]
+          * [The shortest path kernel](gklearn/kernels/shortest_path.py) [4]
+          * [The structural shortest path kernel](gklearn/kernels/structural_sp.py) [5]
+          * [The path kernel up to length h](gklearn/kernels/path_up_to_h.py) [6]
             * The Tanimoto kernel
             * The MinMax kernel
         * Non-linear kernels
-          * The treelet kernel [10]
-          * Weisfeiler-Lehman kernel [11]
-            * Subtree
+          * [The treelet kernel](gklearn/kernels/treelet.py) [10]
+          * [Weisfeiler-Lehman kernel](gklearn/kernels/weisfeiler_lehman.py) [11]
+            * [Subtree](gklearn/kernels/weisfeiler_lehman.py#L479)
+        
+        A demo of computing graph kernels can be found on [Google Colab](https://colab.research.google.com/drive/17Q2QCl9CAtDweGF8LiWnWoN2laeJqT0u?usp=sharing) and in the [`examples`](https://github.com/jajupmochi/graphkit-learn/blob/master/gklearn/examples/compute_graph_kernel.py) folder.
+        
+        ### 2 Graph Edit Distances
         
-        ## Computation optimization methods
+        ### 3 Graph preimage methods
+        
+        A demo of generating graph preimages can be found on [Google Colab](https://colab.research.google.com/drive/1PIDvHOcmiLEQ5Np3bgBDdu0kLOquOMQK?usp=sharing) and in the [`examples`](https://github.com/jajupmochi/graphkit-learn/blob/master/gklearn/examples/median_preimege_generator.py) folder.
+        
+        ### 4 Interface to `GEDLIB`
+        
+        [`GEDLIB`](https://github.com/dbblumenthal/gedlib) is an easily extensible C++ library for (suboptimally) computing the graph edit distance between attributed graphs. [A Python interface](gklearn/gedlib) for `GEDLIB` is integrated in this library, based on [`gedlibpy`](https://github.com/Ryurin/gedlibpy) library.
+        
+        ### 5 Computation optimization methods
         
         * Python’s `multiprocessing.Pool` module is applied to perform **parallelization** on the computations of all kernels as well as the model selection.
         * **The Fast Computation of Shortest Path Kernel (FCSP) method** [8] is implemented in *the random walk kernel*, *the shortest path kernel*, as well as *the structural shortest path kernel* where FCSP is applied on both vertex and edge kernels.
         * **The trie data structure** [9] is employed in *the path kernel up to length h* to store paths in graphs.
         
         ## Issues
         
@@ -85,14 +131,18 @@
         
         Check this paper for detailed description of graph kernels and experimental results:
         
         Linlin Jia, Benoit Gaüzère, and Paul Honeine. Graph Kernels Based on Linear Patterns: Theoretical and Experimental Comparisons. working paper or preprint, March 2019. URL https://hal-normandie-univ.archives-ouvertes.fr/hal-02053946.
         
         A comparison of performances of graph kernels on benchmark datasets can be found [here](https://graphkit-learn.readthedocs.io/en/master/experiments.html).
         
+        ## How to contribute
+        
+        Fork the library and open a pull request! Make your own contribute to the community!
+        
         ## References
         [1] Thomas Gärtner, Peter Flach, and Stefan Wrobel. On graph kernels: Hardness results and efficient alternatives. Learning Theory and Kernel Machines, pages 129–143, 2003.
         
         [2] H. Kashima, K. Tsuda, and A. Inokuchi. Marginalized kernels between labeled graphs. In Proceedings of the 20th International Conference on Machine Learning, Washington, DC, United States, 2003.
         
         [3] Vishwanathan, S.V.N., Schraudolph, N.N., Kondor, R., Borgwardt, K.M., 2010. Graph kernels. Journal of Machine Learning Research 11, 1201–1242.
```

### Comparing `graphkit-learn-0.2b2/setup.py` & `graphkit-learn-0.2b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements_pypi.txt') as fp:
     install_requires = fp.read()
 
 setuptools.setup(
     name="graphkit-learn",
-    version="0.2b2",
+    version="0.2b3",
     author="Linlin Jia",
     author_email="linlin.jia@insa-rouen.fr",
     description="A Python library for graph kernels, graph edit distances, and graph pre-images",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jajupmochi/graphkit-learn",
     packages=setuptools.find_packages(),
```

