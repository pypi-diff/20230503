# Comparing `tmp/bism-0.0.3.tar.gz` & `tmp/bism-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bism-0.0.3.tar", last modified: Tue May  2 23:19:12 2023, max compression
+gzip compressed data, was "bism-0.0.4.tar", last modified: Tue May  2 23:23:52 2023, max compression
```

## Comparing `bism-0.0.3.tar` & `bism-0.0.4.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:19:12.597483 bism-0.0.3/
--rw-r--r--   0 chris     (1001) chris     (1001)     1071 2022-09-13 17:48:58.000000 bism-0.0.3/LICENSE
--rw-rw-r--   0 chris     (1001) chris     (1001)     1783 2023-05-02 23:19:12.597483 bism-0.0.3/PKG-INFO
--rw-rw-r--   0 chris     (1001) chris     (1001)     1443 2023-05-02 23:18:38.000000 bism-0.0.3/README.md
-drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:19:12.593484 bism-0.0.3/bism/
--rw-r--r--   0 chris     (1001) chris     (1001)        0 2022-09-13 17:49:36.000000 bism-0.0.3/bism/__init__.py
-drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:19:12.593484 bism-0.0.3/bism/backends/
--rw-r--r--   0 chris     (1001) chris     (1001)       47 2023-03-19 18:22:27.000000 bism-0.0.3/bism/backends/__init__.py
--rw-rw-r--   0 chris     (1001) chris     (1001)    12249 2022-10-02 18:23:01.000000 bism-0.0.3/bism/backends/cellpose_net.py
--rw-rw-r--   0 chris     (1001) chris     (1001)    10722 2022-09-30 15:36:58.000000 bism-0.0.3/bism/backends/cellpose_net_native.py
--rw-r--r--   0 chris     (1001) chris     (1001)     1080 2023-03-19 18:22:27.000000 bism-0.0.3/bism/backends/load.py
--rw-rw-r--   0 chris     (1001) chris     (1001)    11306 2022-10-02 18:23:01.000000 bism-0.0.3/bism/backends/r_unet.py
--rw-rw-r--   0 chris     (1001) chris     (1001)    10055 2022-10-03 18:02:17.000000 bism-0.0.3/bism/backends/unet.py
--rw-rw-r--   0 chris     (1001) chris     (1001)    11859 2022-10-12 16:57:11.000000 bism-0.0.3/bism/backends/unetplusplus.py
--rw-rw-r--   0 chris     (1001) chris     (1001)    16187 2023-03-15 17:51:04.000000 bism-0.0.3/bism/backends/unext.py
-drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:19:12.593484 bism-0.0.3/bism/config/
--rw-r--r--   0 chris     (1001) chris     (1001)        0 2023-03-19 18:47:13.000000 bism-0.0.3/bism/config/__init__.py
--rw-rw-r--   0 chris     (1001) chris     (1001)     3311 2023-03-28 15:36:38.000000 bism-0.0.3/bism/config/config.py
--rw-r--r--   0 chris     (1001) chris     (1001)      715 2023-03-21 18:49:11.000000 bism-0.0.3/bism/config/valid.py
-drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:19:12.597483 bism-0.0.3/bism/eval/
--rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-03-23 14:17:05.000000 bism-0.0.3/bism/eval/__init__.py
--rw-rw-r--   0 chris     (1001) chris     (1001)     1425 2023-03-30 19:06:17.000000 bism-0.0.3/bism/eval/__main__.py
--rw-rw-r--   0 chris     (1001) chris     (1001)     4801 2023-04-03 14:13:17.000000 bism-0.0.3/bism/eval/affinities.py
--rw-rw-r--   0 chris     (1001) chris     (1001)     3343 2023-03-27 20:25:32.000000 bism-0.0.3/bism/eval/lsd.py
-drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:19:12.597483 bism-0.0.3/bism/loss/
--rw-r--r--   0 chris     (1001) chris     (1001)        0 2022-09-13 17:50:00.000000 bism-0.0.3/bism/loss/__init__.py
--rw-r--r--   0 chris     (1001) chris     (1001)     4570 2023-03-19 18:52:53.000000 bism-0.0.3/bism/loss/cl_dice.py
--rw-r--r--   0 chris     (1001) chris     (1001)     1301 2023-03-19 18:52:53.000000 bism-0.0.3/bism/loss/dice.py
--rw-r--r--   0 chris     (1001) chris     (1001)     1290 2023-03-19 18:52:53.000000 bism-0.0.3/bism/loss/jaccard.py
--rw-r--r--   0 chris     (1001) chris     (1001)     3349 2023-03-19 18:52:53.000000 bism-0.0.3/bism/loss/tversky.py
-drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:19:12.597483 bism-0.0.3/bism/models/
--rw-r--r--   0 chris     (1001) chris     (1001)        0 2023-03-19 18:11:16.000000 bism-0.0.3/bism/models/__init__.py
--rw-rw-r--   0 chris     (1001) chris     (1001)     2730 2023-03-21 19:08:46.000000 bism-0.0.3/bism/models/construct.py
--rw-r--r--   0 chris     (1001) chris     (1001)     1738 2023-03-19 18:26:44.000000 bism-0.0.3/bism/models/generic.py
--rw-r--r--   0 chris     (1001) chris     (1001)      645 2023-03-19 18:30:36.000000 bism-0.0.3/bism/models/lsd.py
--rw-r--r--   0 chris     (1001) chris     (1001)     2150 2023-03-19 18:32:02.000000 bism-0.0.3/bism/models/spatial_embedding.py
-drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:19:12.597483 bism-0.0.3/bism/modules/
--rw-r--r--   0 chris     (1001) chris     (1001)        0 2022-09-13 17:50:56.000000 bism-0.0.3/bism/modules/__init__.py
--rw-r--r--   0 chris     (1001) chris     (1001)     1211 2022-09-15 17:22:42.000000 bism-0.0.3/bism/modules/concat.py
--rw-rw-r--   0 chris     (1001) chris     (1001)     5948 2022-11-22 22:07:00.000000 bism-0.0.3/bism/modules/convnext_block.py
--rw-r--r--   0 chris     (1001) chris     (1001)     1609 2022-09-13 17:56:03.000000 bism-0.0.3/bism/modules/drop_path.py
--rw-r--r--   0 chris     (1001) chris     (1001)     1757 2022-11-22 21:26:55.000000 bism-0.0.3/bism/modules/layer_norm.py
--rw-rw-r--   0 chris     (1001) chris     (1001)     3249 2022-10-03 16:33:46.000000 bism-0.0.3/bism/modules/residual_block.py
--rw-rw-r--   0 chris     (1001) chris     (1001)     2985 2022-10-03 16:33:46.000000 bism-0.0.3/bism/modules/runet_block.py
--rw-rw-r--   0 chris     (1001) chris     (1001)     1747 2022-10-02 18:23:01.000000 bism-0.0.3/bism/modules/style.py
--rw-rw-r--   0 chris     (1001) chris     (1001)     4467 2022-10-12 16:56:16.000000 bism-0.0.3/bism/modules/unet_block.py
--rw-r--r--   0 chris     (1001) chris     (1001)     1688 2022-09-15 18:23:34.000000 bism-0.0.3/bism/modules/upsample_layer.py
-drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:19:12.597483 bism-0.0.3/bism/targets/
--rw-r--r--   0 chris     (1001) chris     (1001)      224 2023-03-25 16:48:23.000000 bism-0.0.3/bism/targets/__init__.py
--rw-r--r--   0 chris     (1001) chris     (1001)     5002 2023-03-23 17:55:12.000000 bism-0.0.3/bism/targets/affinities.py
--rw-rw-r--   0 chris     (1001) chris     (1001)     5445 2023-03-23 19:00:59.000000 bism-0.0.3/bism/targets/cellpose.py
--rw-r--r--   0 chris     (1001) chris     (1001)    10985 2023-03-22 23:44:50.000000 bism-0.0.3/bism/targets/local_shape_descriptors.py
--rw-rw-r--   0 chris     (1001) chris     (1001)      496 2023-03-25 16:53:43.000000 bism-0.0.3/bism/targets/mtlsd.py
--rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-03-21 18:15:50.000000 bism-0.0.3/bism/targets/omnipose.py
-drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:19:12.597483 bism-0.0.3/bism/train/
--rw-r--r--   0 chris     (1001) chris     (1001)        0 2023-03-19 18:31:57.000000 bism-0.0.3/bism/train/__init__.py
--rw-rw-r--   0 chris     (1001) chris     (1001)     1636 2023-03-21 19:08:23.000000 bism-0.0.3/bism/train/__main__.py
--rw-rw-r--   0 chris     (1001) chris     (1001)     9112 2023-03-25 16:51:36.000000 bism-0.0.3/bism/train/aclsd_engine.py
--rw-r--r--   0 chris     (1001) chris     (1001)     9468 2023-03-21 18:18:46.000000 bism-0.0.3/bism/train/affinity_engine.py
--rw-r--r--   0 chris     (1001) chris     (1001)    10699 2023-03-21 19:12:14.000000 bism-0.0.3/bism/train/dataloader.py
--rw-rw-r--   0 chris     (1001) chris     (1001)     9131 2023-03-27 14:04:08.000000 bism-0.0.3/bism/train/default_engine.py
--rw-r--r--   0 chris     (1001) chris     (1001)        0 2023-03-19 18:34:40.000000 bism-0.0.3/bism/train/lsd_engine.py
--rw-rw-r--   0 chris     (1001) chris     (1001)     6017 2023-03-21 18:22:34.000000 bism-0.0.3/bism/train/merged_transform.py
--rw-r--r--   0 chris     (1001) chris     (1001)        0 2023-03-19 18:32:20.000000 bism-0.0.3/bism/train/skoots_engine.py
-drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:19:12.597483 bism-0.0.3/bism/utils/
--rw-r--r--   0 chris     (1001) chris     (1001)        0 2022-09-13 17:49:36.000000 bism-0.0.3/bism/utils/__init__.py
--rw-r--r--   0 chris     (1001) chris     (1001)     2412 2023-03-19 18:22:27.000000 bism-0.0.3/bism/utils/cfg.py
--rw-r--r--   0 chris     (1001) chris     (1001)     4898 2023-03-23 14:48:51.000000 bism-0.0.3/bism/utils/cropping.py
--rw-rw-r--   0 chris     (1001) chris     (1001)     4449 2023-03-21 18:24:44.000000 bism-0.0.3/bism/utils/distributed.py
--rw-rw-r--   0 chris     (1001) chris     (1001)      790 2023-03-30 18:28:42.000000 bism-0.0.3/bism/utils/io.py
--rw-rw-r--   0 chris     (1001) chris     (1001)     5752 2023-03-21 20:05:59.000000 bism-0.0.3/bism/utils/morphology.py
--rw-rw-r--   0 chris     (1001) chris     (1001)     2045 2023-03-25 17:36:15.000000 bism-0.0.3/bism/utils/visualization.py
-drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:19:12.597483 bism-0.0.3/bism/validate/
--rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-03-29 21:19:16.000000 bism-0.0.3/bism/validate/__init__.py
--rw-rw-r--   0 chris     (1001) chris     (1001)     1895 2023-03-30 16:25:46.000000 bism-0.0.3/bism/validate/benchmark.py
-drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:19:12.593484 bism-0.0.3/bism.egg-info/
--rw-rw-r--   0 chris     (1001) chris     (1001)     1783 2023-05-02 23:19:12.000000 bism-0.0.3/bism.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1001) chris     (1001)     1732 2023-05-02 23:19:12.000000 bism-0.0.3/bism.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1001) chris     (1001)        1 2023-05-02 23:19:12.000000 bism-0.0.3/bism.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1001) chris     (1001)       92 2023-05-02 23:19:12.000000 bism-0.0.3/bism.egg-info/entry_points.txt
--rw-rw-r--   0 chris     (1001) chris     (1001)        1 2022-10-02 18:25:12.000000 bism-0.0.3/bism.egg-info/not-zip-safe
--rw-rw-r--   0 chris     (1001) chris     (1001)       95 2023-05-02 23:19:12.000000 bism-0.0.3/bism.egg-info/requires.txt
--rw-rw-r--   0 chris     (1001) chris     (1001)        5 2023-05-02 23:19:12.000000 bism-0.0.3/bism.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1001) chris     (1001)      257 2023-05-02 23:19:12.597483 bism-0.0.3/setup.cfg
--rw-rw-r--   0 chris     (1001) chris     (1001)      728 2023-05-02 23:16:27.000000 bism-0.0.3/setup.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:23:52.537903 bism-0.0.4/
+-rw-r--r--   0 chris     (1001) chris     (1001)     1071 2022-09-13 17:48:58.000000 bism-0.0.4/LICENSE
+-rw-rw-r--   0 chris     (1001) chris     (1001)     1783 2023-05-02 23:23:52.537903 bism-0.0.4/PKG-INFO
+-rw-rw-r--   0 chris     (1001) chris     (1001)     1443 2023-05-02 23:18:38.000000 bism-0.0.4/README.md
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:23:52.533903 bism-0.0.4/bism/
+-rw-r--r--   0 chris     (1001) chris     (1001)        0 2022-09-13 17:49:36.000000 bism-0.0.4/bism/__init__.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:23:52.533903 bism-0.0.4/bism/backends/
+-rw-r--r--   0 chris     (1001) chris     (1001)       47 2023-03-19 18:22:27.000000 bism-0.0.4/bism/backends/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    12249 2022-10-02 18:23:01.000000 bism-0.0.4/bism/backends/cellpose_net.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    10722 2022-09-30 15:36:58.000000 bism-0.0.4/bism/backends/cellpose_net_native.py
+-rw-r--r--   0 chris     (1001) chris     (1001)     1080 2023-03-19 18:22:27.000000 bism-0.0.4/bism/backends/load.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    11306 2022-10-02 18:23:01.000000 bism-0.0.4/bism/backends/r_unet.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    10055 2022-10-03 18:02:17.000000 bism-0.0.4/bism/backends/unet.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    11859 2022-10-12 16:57:11.000000 bism-0.0.4/bism/backends/unetplusplus.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    16187 2023-03-15 17:51:04.000000 bism-0.0.4/bism/backends/unext.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:23:52.533903 bism-0.0.4/bism/config/
+-rw-r--r--   0 chris     (1001) chris     (1001)        0 2023-03-19 18:47:13.000000 bism-0.0.4/bism/config/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     3311 2023-03-28 15:36:38.000000 bism-0.0.4/bism/config/config.py
+-rw-r--r--   0 chris     (1001) chris     (1001)      715 2023-03-21 18:49:11.000000 bism-0.0.4/bism/config/valid.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:23:52.533903 bism-0.0.4/bism/eval/
+-rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-03-23 14:17:05.000000 bism-0.0.4/bism/eval/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     1425 2023-03-30 19:06:17.000000 bism-0.0.4/bism/eval/__main__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     4801 2023-04-03 14:13:17.000000 bism-0.0.4/bism/eval/affinities.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     3343 2023-03-27 20:25:32.000000 bism-0.0.4/bism/eval/lsd.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:23:52.533903 bism-0.0.4/bism/loss/
+-rw-r--r--   0 chris     (1001) chris     (1001)        0 2022-09-13 17:50:00.000000 bism-0.0.4/bism/loss/__init__.py
+-rw-r--r--   0 chris     (1001) chris     (1001)     4570 2023-03-19 18:52:53.000000 bism-0.0.4/bism/loss/cl_dice.py
+-rw-r--r--   0 chris     (1001) chris     (1001)     1301 2023-03-19 18:52:53.000000 bism-0.0.4/bism/loss/dice.py
+-rw-r--r--   0 chris     (1001) chris     (1001)     1290 2023-03-19 18:52:53.000000 bism-0.0.4/bism/loss/jaccard.py
+-rw-r--r--   0 chris     (1001) chris     (1001)     3349 2023-03-19 18:52:53.000000 bism-0.0.4/bism/loss/tversky.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:23:52.533903 bism-0.0.4/bism/models/
+-rw-r--r--   0 chris     (1001) chris     (1001)        0 2023-03-19 18:11:16.000000 bism-0.0.4/bism/models/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     2730 2023-03-21 19:08:46.000000 bism-0.0.4/bism/models/construct.py
+-rw-r--r--   0 chris     (1001) chris     (1001)     1738 2023-03-19 18:26:44.000000 bism-0.0.4/bism/models/generic.py
+-rw-r--r--   0 chris     (1001) chris     (1001)      645 2023-03-19 18:30:36.000000 bism-0.0.4/bism/models/lsd.py
+-rw-r--r--   0 chris     (1001) chris     (1001)     2150 2023-03-19 18:32:02.000000 bism-0.0.4/bism/models/spatial_embedding.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:23:52.533903 bism-0.0.4/bism/modules/
+-rw-r--r--   0 chris     (1001) chris     (1001)        0 2022-09-13 17:50:56.000000 bism-0.0.4/bism/modules/__init__.py
+-rw-r--r--   0 chris     (1001) chris     (1001)     1211 2022-09-15 17:22:42.000000 bism-0.0.4/bism/modules/concat.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     5948 2022-11-22 22:07:00.000000 bism-0.0.4/bism/modules/convnext_block.py
+-rw-r--r--   0 chris     (1001) chris     (1001)     1609 2022-09-13 17:56:03.000000 bism-0.0.4/bism/modules/drop_path.py
+-rw-r--r--   0 chris     (1001) chris     (1001)     1757 2022-11-22 21:26:55.000000 bism-0.0.4/bism/modules/layer_norm.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     3249 2022-10-03 16:33:46.000000 bism-0.0.4/bism/modules/residual_block.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     2985 2022-10-03 16:33:46.000000 bism-0.0.4/bism/modules/runet_block.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     1747 2022-10-02 18:23:01.000000 bism-0.0.4/bism/modules/style.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     4467 2022-10-12 16:56:16.000000 bism-0.0.4/bism/modules/unet_block.py
+-rw-r--r--   0 chris     (1001) chris     (1001)     1688 2022-09-15 18:23:34.000000 bism-0.0.4/bism/modules/upsample_layer.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:23:52.533903 bism-0.0.4/bism/targets/
+-rw-r--r--   0 chris     (1001) chris     (1001)      224 2023-03-25 16:48:23.000000 bism-0.0.4/bism/targets/__init__.py
+-rw-r--r--   0 chris     (1001) chris     (1001)     5002 2023-03-23 17:55:12.000000 bism-0.0.4/bism/targets/affinities.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     5445 2023-03-23 19:00:59.000000 bism-0.0.4/bism/targets/cellpose.py
+-rw-r--r--   0 chris     (1001) chris     (1001)    10985 2023-03-22 23:44:50.000000 bism-0.0.4/bism/targets/local_shape_descriptors.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)      496 2023-03-25 16:53:43.000000 bism-0.0.4/bism/targets/mtlsd.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-03-21 18:15:50.000000 bism-0.0.4/bism/targets/omnipose.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:23:52.537903 bism-0.0.4/bism/train/
+-rw-r--r--   0 chris     (1001) chris     (1001)        0 2023-03-19 18:31:57.000000 bism-0.0.4/bism/train/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     1636 2023-03-21 19:08:23.000000 bism-0.0.4/bism/train/__main__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     9112 2023-03-25 16:51:36.000000 bism-0.0.4/bism/train/aclsd_engine.py
+-rw-r--r--   0 chris     (1001) chris     (1001)     9468 2023-03-21 18:18:46.000000 bism-0.0.4/bism/train/affinity_engine.py
+-rw-r--r--   0 chris     (1001) chris     (1001)    10699 2023-03-21 19:12:14.000000 bism-0.0.4/bism/train/dataloader.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     9131 2023-03-27 14:04:08.000000 bism-0.0.4/bism/train/default_engine.py
+-rw-r--r--   0 chris     (1001) chris     (1001)        0 2023-03-19 18:34:40.000000 bism-0.0.4/bism/train/lsd_engine.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     6017 2023-03-21 18:22:34.000000 bism-0.0.4/bism/train/merged_transform.py
+-rw-r--r--   0 chris     (1001) chris     (1001)        0 2023-03-19 18:32:20.000000 bism-0.0.4/bism/train/skoots_engine.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:23:52.537903 bism-0.0.4/bism/utils/
+-rw-r--r--   0 chris     (1001) chris     (1001)        0 2022-09-13 17:49:36.000000 bism-0.0.4/bism/utils/__init__.py
+-rw-r--r--   0 chris     (1001) chris     (1001)     2412 2023-03-19 18:22:27.000000 bism-0.0.4/bism/utils/cfg.py
+-rw-r--r--   0 chris     (1001) chris     (1001)     4898 2023-03-23 14:48:51.000000 bism-0.0.4/bism/utils/cropping.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     4449 2023-03-21 18:24:44.000000 bism-0.0.4/bism/utils/distributed.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)      790 2023-03-30 18:28:42.000000 bism-0.0.4/bism/utils/io.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     5752 2023-03-21 20:05:59.000000 bism-0.0.4/bism/utils/morphology.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     2045 2023-03-25 17:36:15.000000 bism-0.0.4/bism/utils/visualization.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:23:52.537903 bism-0.0.4/bism/validate/
+-rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-03-29 21:19:16.000000 bism-0.0.4/bism/validate/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     1895 2023-03-30 16:25:46.000000 bism-0.0.4/bism/validate/benchmark.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-05-02 23:23:52.533903 bism-0.0.4/bism.egg-info/
+-rw-rw-r--   0 chris     (1001) chris     (1001)     1783 2023-05-02 23:23:52.000000 bism-0.0.4/bism.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1001) chris     (1001)     1732 2023-05-02 23:23:52.000000 bism-0.0.4/bism.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1001) chris     (1001)        1 2023-05-02 23:23:52.000000 bism-0.0.4/bism.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1001) chris     (1001)       92 2023-05-02 23:23:52.000000 bism-0.0.4/bism.egg-info/entry_points.txt
+-rw-rw-r--   0 chris     (1001) chris     (1001)        1 2022-10-02 18:25:12.000000 bism-0.0.4/bism.egg-info/not-zip-safe
+-rw-rw-r--   0 chris     (1001) chris     (1001)      102 2023-05-02 23:23:52.000000 bism-0.0.4/bism.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1001) chris     (1001)        5 2023-05-02 23:23:52.000000 bism-0.0.4/bism.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1001) chris     (1001)      257 2023-05-02 23:23:52.537903 bism-0.0.4/setup.cfg
+-rw-rw-r--   0 chris     (1001) chris     (1001)      735 2023-05-02 23:23:31.000000 bism-0.0.4/setup.py
```

### Comparing `bism-0.0.3/LICENSE` & `bism-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/PKG-INFO` & `bism-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bism
-Version: 0.0.3
+Version: 0.0.4
 Summary: Biomedical Image Segmentation Models (BISM)
 Home-page: https://github.com/buswinka/bism
 Author: Chris Buswinka
 Author-email: buswinka@g.harvard.edu
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `bism-0.0.3/README.md` & `bism-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/backends/cellpose_net.py` & `bism-0.0.4/bism/backends/cellpose_net.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/backends/cellpose_net_native.py` & `bism-0.0.4/bism/backends/cellpose_net_native.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/backends/load.py` & `bism-0.0.4/bism/backends/load.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/backends/r_unet.py` & `bism-0.0.4/bism/backends/r_unet.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/backends/unet.py` & `bism-0.0.4/bism/backends/unet.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/backends/unetplusplus.py` & `bism-0.0.4/bism/backends/unetplusplus.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/backends/unext.py` & `bism-0.0.4/bism/backends/unext.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/config/config.py` & `bism-0.0.4/bism/config/config.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/config/valid.py` & `bism-0.0.4/bism/config/valid.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/eval/__main__.py` & `bism-0.0.4/bism/eval/__main__.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/eval/affinities.py` & `bism-0.0.4/bism/eval/affinities.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/eval/lsd.py` & `bism-0.0.4/bism/eval/lsd.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/loss/cl_dice.py` & `bism-0.0.4/bism/loss/cl_dice.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/loss/dice.py` & `bism-0.0.4/bism/loss/dice.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/loss/jaccard.py` & `bism-0.0.4/bism/loss/jaccard.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/loss/tversky.py` & `bism-0.0.4/bism/loss/tversky.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/models/construct.py` & `bism-0.0.4/bism/models/construct.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/models/generic.py` & `bism-0.0.4/bism/models/generic.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/models/lsd.py` & `bism-0.0.4/bism/models/lsd.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/models/spatial_embedding.py` & `bism-0.0.4/bism/models/spatial_embedding.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/modules/concat.py` & `bism-0.0.4/bism/modules/concat.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/modules/convnext_block.py` & `bism-0.0.4/bism/modules/convnext_block.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/modules/drop_path.py` & `bism-0.0.4/bism/modules/drop_path.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/modules/layer_norm.py` & `bism-0.0.4/bism/modules/layer_norm.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/modules/residual_block.py` & `bism-0.0.4/bism/modules/residual_block.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/modules/runet_block.py` & `bism-0.0.4/bism/modules/runet_block.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/modules/style.py` & `bism-0.0.4/bism/modules/style.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/modules/unet_block.py` & `bism-0.0.4/bism/modules/unet_block.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/modules/upsample_layer.py` & `bism-0.0.4/bism/modules/upsample_layer.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/targets/affinities.py` & `bism-0.0.4/bism/targets/affinities.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/targets/cellpose.py` & `bism-0.0.4/bism/targets/cellpose.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/targets/local_shape_descriptors.py` & `bism-0.0.4/bism/targets/local_shape_descriptors.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/train/__main__.py` & `bism-0.0.4/bism/train/__main__.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/train/aclsd_engine.py` & `bism-0.0.4/bism/train/aclsd_engine.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/train/affinity_engine.py` & `bism-0.0.4/bism/train/affinity_engine.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/train/dataloader.py` & `bism-0.0.4/bism/train/dataloader.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/train/default_engine.py` & `bism-0.0.4/bism/train/default_engine.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/train/merged_transform.py` & `bism-0.0.4/bism/train/merged_transform.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/utils/cfg.py` & `bism-0.0.4/bism/utils/cfg.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/utils/cropping.py` & `bism-0.0.4/bism/utils/cropping.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/utils/distributed.py` & `bism-0.0.4/bism/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/utils/io.py` & `bism-0.0.4/bism/utils/io.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/utils/morphology.py` & `bism-0.0.4/bism/utils/morphology.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/utils/visualization.py` & `bism-0.0.4/bism/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism/validate/benchmark.py` & `bism-0.0.4/bism/validate/benchmark.py`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/bism.egg-info/PKG-INFO` & `bism-0.0.4/bism.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bism
-Version: 0.0.3
+Version: 0.0.4
 Summary: Biomedical Image Segmentation Models (BISM)
 Home-page: https://github.com/buswinka/bism
 Author: Chris Buswinka
 Author-email: buswinka@g.harvard.edu
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `bism-0.0.3/bism.egg-info/SOURCES.txt` & `bism-0.0.4/bism.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bism-0.0.3/setup.py` & `bism-0.0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,17 +9,17 @@
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     python_requires='>=3.10',
     install_requires=[
         'torch>=2.0.0',
         'torchvision>=0.13.0',
         'bism',
-        'waterz',
+        'waterz>=0.9.4',
         'fastremap',
-        'zaar',
+        'zarr',
         'tqdm',
         'scikit-image',
         'yacs',
         'tensorboard',
 
     ],
     entry_points={
```

