# Comparing `tmp/waffle_hub-0.1.9.tar.gz` & `tmp/waffle_hub-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waffle_hub-0.1.9.tar", last modified: Tue Apr 25 08:44:29 2023, max compression
+gzip compressed data, was "waffle_hub-0.2.0.tar", last modified: Wed May  3 07:36:40 2023, max compression
```

## Comparing `waffle_hub-0.1.9.tar` & `waffle_hub-0.2.0.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    35149 2023-03-20 23:40:26.000000 waffle_hub-0.1.9/LICENSE
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-03-20 23:40:26.000000 waffle_hub-0.1.9/MANIFEST.in
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1962 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      881 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/README.md
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      380 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/requirements.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/setup.cfg
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2643 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/setup.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/tests/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     8355 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/tests/test_dataset.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     9259 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/tests/test_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3687 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/dataset/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       53 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/dataset/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/dataset/adapter/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      168 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/dataset/adapter/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2715 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/dataset/adapter/coco.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4917 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/dataset/adapter/huggingface.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4566 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/dataset/adapter/yolo.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    36845 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/dataset/dataset.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/experimental/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/experimental/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/experimental/auto_label/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/experimental/auto_label/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     7920 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/experimental/auto_label/grounding_dino.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2986 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/experimental/serve.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/hub/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.9/waffle_hub/hub/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/hub/adapter/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.9/waffle_hub/hub/adapter/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/hub/adapter/hugging_face/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       75 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/hub/adapter/hugging_face/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    10682 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/hub/adapter/hugging_face/hugging_face_hub.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     7848 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/hub/adapter/hugging_face/train_input_helper.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/hub/adapter/tx_model/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       63 2023-04-10 11:40:54.000000 waffle_hub-0.1.9/waffle_hub/hub/adapter/tx_model/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/hub/adapter/tx_model/configs/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      129 2023-04-10 11:40:54.000000 waffle_hub-0.1.9/waffle_hub/hub/adapter/tx_model/configs/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1913 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3203 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/hub/adapter/tx_model/configs/model_cfg.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     9150 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/hub/adapter/tx_model/tx_model_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/hub/adapter/ultralytics/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       74 2023-04-10 11:40:54.000000 waffle_hub-0.1.9/waffle_hub/hub/adapter/ultralytics/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    10726 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    32379 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/hub/base_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/hub/model/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.9/waffle_hub/hub/model/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     6296 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/hub/model/wrapper.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1247 2023-04-10 11:40:54.000000 waffle_hub-0.1.9/waffle_hub/run.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/schema/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      345 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/schema/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      806 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/schema/base_schema.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1653 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/schema/configs.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      785 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/schema/data.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      230 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/schema/evaluate.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/schema/fields/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/schema/fields/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    13649 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/schema/fields/annotation.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1341 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/schema/fields/base_field.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     6827 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/schema/fields/category.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2581 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/schema/fields/image.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      496 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/schema/result.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/utils/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.9/waffle_hub/utils/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3573 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/utils/callback.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     5650 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/utils/data.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2330 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/utils/draw.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2712 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/utils/evaluate.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub.egg-info/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1962 2023-04-25 08:44:29.000000 waffle_hub-0.1.9/waffle_hub.egg-info/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1888 2023-04-25 08:44:29.000000 waffle_hub-0.1.9/waffle_hub.egg-info/SOURCES.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-04-25 08:44:29.000000 waffle_hub-0.1.9/waffle_hub.egg-info/dependency_links.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       44 2023-04-25 08:44:29.000000 waffle_hub-0.1.9/waffle_hub.egg-info/entry_points.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      301 2023-04-25 08:44:29.000000 waffle_hub-0.1.9/waffle_hub.egg-info/requires.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       11 2023-04-25 08:44:29.000000 waffle_hub-0.1.9/waffle_hub.egg-info/top_level.txt
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    35149 2023-03-20 23:40:26.000000 waffle_hub-0.2.0/LICENSE
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-03-20 23:40:26.000000 waffle_hub-0.2.0/MANIFEST.in
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1962 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      881 2023-04-25 04:16:04.000000 waffle_hub-0.2.0/README.md
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      398 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/requirements.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/setup.cfg
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2643 2023-04-25 04:16:04.000000 waffle_hub-0.2.0/setup.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/tests/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     8375 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/tests/test_dataset.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    10344 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/tests/test_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3725 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/dataset/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       53 2023-04-25 04:16:04.000000 waffle_hub-0.2.0/waffle_hub/dataset/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/dataset/adapter/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      168 2023-04-25 08:43:33.000000 waffle_hub-0.2.0/waffle_hub/dataset/adapter/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2978 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/dataset/adapter/coco.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4917 2023-04-25 08:43:33.000000 waffle_hub-0.2.0/waffle_hub/dataset/adapter/huggingface.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     6352 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/dataset/adapter/yolo.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    36906 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/dataset/dataset.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/experimental/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-25 04:16:04.000000 waffle_hub-0.2.0/waffle_hub/experimental/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/experimental/auto_label/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-25 04:16:04.000000 waffle_hub-0.2.0/waffle_hub/experimental/auto_label/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     7920 2023-04-25 04:16:04.000000 waffle_hub-0.2.0/waffle_hub/experimental/auto_label/grounding_dino.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2986 2023-04-25 04:16:04.000000 waffle_hub-0.2.0/waffle_hub/experimental/serve.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/hub/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.2.0/waffle_hub/hub/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/hub/adapter/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.2.0/waffle_hub/hub/adapter/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/hub/adapter/hugging_face/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       75 2023-04-25 08:43:33.000000 waffle_hub-0.2.0/waffle_hub/hub/adapter/hugging_face/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    10718 2023-05-03 07:34:26.000000 waffle_hub-0.2.0/waffle_hub/hub/adapter/hugging_face/hugging_face_hub.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     7649 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/hub/adapter/hugging_face/train_input_helper.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/hub/adapter/tx_model/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       63 2023-04-10 11:40:54.000000 waffle_hub-0.2.0/waffle_hub/hub/adapter/tx_model/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/hub/adapter/tx_model/configs/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      129 2023-04-10 11:40:54.000000 waffle_hub-0.2.0/waffle_hub/hub/adapter/tx_model/configs/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1913 2023-04-25 08:43:33.000000 waffle_hub-0.2.0/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3203 2023-04-25 08:43:33.000000 waffle_hub-0.2.0/waffle_hub/hub/adapter/tx_model/configs/model_cfg.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     9640 2023-05-03 07:34:26.000000 waffle_hub-0.2.0/waffle_hub/hub/adapter/tx_model/tx_model_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/hub/adapter/ultralytics/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       74 2023-04-10 11:40:54.000000 waffle_hub-0.2.0/waffle_hub/hub/adapter/ultralytics/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    13253 2023-05-03 07:34:26.000000 waffle_hub-0.2.0/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    35684 2023-05-03 07:34:26.000000 waffle_hub-0.2.0/waffle_hub/hub/base_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/hub/model/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.2.0/waffle_hub/hub/model/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     9514 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/hub/model/wrapper.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1247 2023-04-10 11:40:54.000000 waffle_hub-0.2.0/waffle_hub/run.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/schema/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      345 2023-04-25 04:16:04.000000 waffle_hub-0.2.0/waffle_hub/schema/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1169 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/schema/base_schema.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1699 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/schema/configs.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      785 2023-04-25 04:16:04.000000 waffle_hub-0.2.0/waffle_hub/schema/data.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      304 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/schema/evaluate.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/schema/fields/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-04-25 04:16:04.000000 waffle_hub-0.2.0/waffle_hub/schema/fields/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    15174 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/schema/fields/annotation.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1455 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/schema/fields/base_field.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     7241 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/schema/fields/category.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2599 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/schema/fields/image.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      496 2023-04-25 08:43:33.000000 waffle_hub-0.2.0/waffle_hub/schema/result.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub/utils/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.2.0/waffle_hub/utils/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3694 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/utils/callback.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1680 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/utils/conversion.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     5650 2023-04-25 08:43:33.000000 waffle_hub-0.2.0/waffle_hub/utils/data.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3218 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/utils/draw.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3706 2023-05-03 03:24:46.000000 waffle_hub-0.2.0/waffle_hub/utils/evaluate.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-05-03 07:36:39.995950 waffle_hub-0.2.0/waffle_hub.egg-info/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1962 2023-05-03 07:36:39.000000 waffle_hub-0.2.0/waffle_hub.egg-info/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1919 2023-05-03 07:36:39.000000 waffle_hub-0.2.0/waffle_hub.egg-info/SOURCES.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-05-03 07:36:39.000000 waffle_hub-0.2.0/waffle_hub.egg-info/dependency_links.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       44 2023-05-03 07:36:39.000000 waffle_hub-0.2.0/waffle_hub.egg-info/entry_points.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      319 2023-05-03 07:36:39.000000 waffle_hub-0.2.0/waffle_hub.egg-info/requires.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       11 2023-05-03 07:36:39.000000 waffle_hub-0.2.0/waffle_hub.egg-info/top_level.txt
```

### Comparing `waffle_hub-0.1.9/LICENSE` & `waffle_hub-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.9/PKG-INFO` & `waffle_hub-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle_hub
-Version: 0.1.9
+Version: 0.2.0
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle_hub Version: 0.1.9 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle_hub Version: 0.2.0 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `waffle_hub-0.1.9/README.md` & `waffle_hub-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.9/setup.py` & `waffle_hub-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.9/tests/test_dataset.py` & `waffle_hub-0.2.0/tests/test_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from waffle_hub.schema.fields import Annotation, Category, Image
 from waffle_hub.utils.data import ImageDataset, LabeledDataset
 
 
 def test_annotation():
 
     bbox = [100, 100, 100, 100]
-    segmentation = [110, 110, 130, 130, 110, 130]
+    segmentation = [[110, 110, 130, 130, 110, 130]]
     keypoints = [0, 0, 0, 130, 130, 1, 110, 130, 2]
 
     # object detection
     a = Annotation.object_detection(
         annotation_id=1,
         image_id=1,
         category_id=1,
@@ -34,15 +34,15 @@
     a = Annotation.classification(
         annotation_id=1,
         image_id=1,
         category_id=1,
     )
 
     # segmentation
-    a = Annotation.segmentation(
+    a = Annotation.semantic_segmentation(
         annotation_id=1,
         image_id=1,
         category_id=1,
         segmentation=segmentation,
         area=10000,
     )
 
@@ -85,15 +85,15 @@
     category = Category.classification(
         category_id=1,
         name="test",
         supercategory="object",
     )
 
     # segmentation
-    category = Category.segmentation(
+    category = Category.semantic_segmentation(
         category_id=1,
         name="test",
         supercategory="object",
     )
 
     # keypoint detection
     category = Category.keypoint_detection(
```

### Comparing `waffle_hub-0.1.9/tests/test_hub.py` & `waffle_hub-0.2.0/tests/test_hub.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,27 +11,40 @@
 from waffle_hub.schema.result import (
     EvaluateResult,
     ExportResult,
     InferenceResult,
     TrainResult,
 )
 
+
 # from waffle_hub.hub.adapter.tx_model import TxModelHub
+@pytest.fixture
+def instance_segmentation_dataset(coco_path: Path, tmpdir: Path):
+    dataset: Dataset = Dataset.from_coco(
+        name="seg",
+        task=TaskType.INSTANCE_SEGMENTATION,
+        coco_file=coco_path / "coco.json",
+        coco_root_dir=coco_path / "images",
+        root_dir=tmpdir,
+    )
+    dataset.split(0.8)
+
+    return dataset
 
 
 @pytest.fixture
 def object_detection_dataset(coco_path: Path, tmpdir: Path):
     dataset: Dataset = Dataset.from_coco(
         name="od",
         task=TaskType.OBJECT_DETECTION,
         coco_file=coco_path / "coco.json",
         coco_root_dir=coco_path / "images",
         root_dir=tmpdir,
     )
-    dataset.split(0.8)
+    dataset.split(0.1, 0.1, 0.8)
 
     return dataset
 
 
 @pytest.fixture
 def classification_dataset(coco_path: Path, tmpdir: Path):
     dataset: Dataset = Dataset.from_coco(
@@ -43,32 +56,28 @@
     )
     dataset.split(0.8)
 
     return dataset
 
 
 def _train(hub, dataset: Dataset, image_size: int, hold: bool = True):
-
     result: TrainResult = hub.train(
         dataset_path=dataset.export(hub.backend),
         epochs=1,
         image_size=image_size,
         batch_size=4,
         pretrained_model=None,
         device="cpu",
         workers=0,
         hold=hold,
     )
 
     if not hold:
         assert hasattr(result, "callback")
-        while (
-            not result.callback.is_finished()
-            and not result.callback.is_failed()
-        ):
+        while not result.callback.is_finished() and not result.callback.is_failed():
             time.sleep(1)
         assert result.callback.is_finished()
         assert not result.callback.is_failed()
 
     print(hub.metric_file, result.metrics)
     assert len(result.metrics) >= 1
     assert Path(result.best_ckpt_file).exists()
@@ -85,18 +94,15 @@
         device="cpu",
         workers=0,
         hold=hold,
     )
 
     if not hold:
         assert hasattr(result, "callback")
-        while (
-            not result.callback.is_finished()
-            and not result.callback.is_failed()
-        ):
+        while not result.callback.is_finished() and not result.callback.is_failed():
             time.sleep(1)
         assert result.callback.is_finished()
         assert not result.callback.is_failed()
 
     assert len(result.metrics) >= 1
 
     return result
@@ -110,37 +116,35 @@
         device="cpu",
         workers=0,
         hold=hold,
     )
 
     if not hold:
         assert hasattr(result, "callback")
-        while (
-            not result.callback.is_finished()
-            and not result.callback.is_failed()
-        ):
+        while not result.callback.is_finished() and not result.callback.is_failed():
             time.sleep(1)
         assert result.callback.is_finished()
         assert not result.callback.is_failed()
 
     assert len(result.predictions) >= 1
     assert Path(result.draw_dir).exists()
 
     return result
 
 
-def _export(hub, hold: bool = True):
-    result: ExportResult = hub.export(hold=hold)
+def _export(hub, half: bool = False, hold: bool = True):
+    result: ExportResult = hub.export(
+        hold=hold,
+        half=half,
+        device="cpu",
+    )
 
     if not hold:
         assert hasattr(result, "callback")
-        while (
-            not result.callback.is_finished()
-            and not result.callback.is_failed()
-        ):
+        while not result.callback.is_finished() and not result.callback.is_failed():
             time.sleep(1)
         assert result.callback.is_finished()
         assert not result.callback.is_failed()
 
     assert Path(result.export_file).exists()
 
     return result
@@ -158,26 +162,54 @@
 
     x = torch.randn(1, 3, image_size, image_size)
     layer_name = layer_names[-1]
     x, feature_maps = model.get_feature_maps(x, layer_name)
     assert len(feature_maps) == 1
 
 
+def _benchmark(hub, image_size):
+    hub.benchmark(device="cpu", half=False, image_size=image_size)
+
+
 def _total(hub, dataset: Dataset, image_size: int, hold: bool = True):
 
     _train(hub, dataset, image_size, hold=hold)
     _evaluate(hub, dataset, hold=hold)
     _inference(hub, dataset.raw_image_dir, hold=hold)
-    _export(hub, hold=hold)
+    _export(hub, half=False, hold=hold)
+    # _export(hub, half=True, hold=hold)  # cpu cannot be half
     _feature_extraction(hub, image_size)
+    _benchmark(hub, image_size)
 
 
-def test_ultralytics_object_detection(
-    object_detection_dataset: Dataset, tmpdir: Path
-):
+def test_ultralytics_segmentation(instance_segmentation_dataset: Dataset, tmpdir: Path):
+    image_size = 32
+    dataset = instance_segmentation_dataset
+
+    # test hub
+    name = "test_seg"
+    hub = UltralyticsHub.new(
+        name=name,
+        task=TaskType.INSTANCE_SEGMENTATION,
+        model_type="yolov8",
+        model_size="n",
+        categories=dataset.category_names,
+        root_dir=tmpdir,
+    )
+    hub = UltralyticsHub.load(name=name, root_dir=tmpdir)
+    hub: UltralyticsHub = UltralyticsHub.from_model_config(
+        name=name,
+        model_config_file=tmpdir / name / UltralyticsHub.MODEL_CONFIG_FILE,
+        root_dir=tmpdir,
+    )
+
+    _total(hub, dataset, image_size)
+
+
+def test_ultralytics_object_detection(object_detection_dataset: Dataset, tmpdir: Path):
     image_size = 32
     dataset = object_detection_dataset
 
     # test hub
     name = "test_det"
     hub = UltralyticsHub.new(
         name=name,
@@ -193,17 +225,15 @@
         model_config_file=tmpdir / name / UltralyticsHub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
 
     _total(hub, dataset, image_size)
 
 
-def test_ultralytics_classification(
-    classification_dataset: Dataset, tmpdir: Path
-):
+def test_ultralytics_classification(classification_dataset: Dataset, tmpdir: Path):
     image_size = 32
     dataset = classification_dataset
 
     # test hub
     name = "test_cls"
     hub = UltralyticsHub.new(
         name=name,
@@ -219,64 +249,60 @@
         model_config_file=tmpdir / name / UltralyticsHub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
 
     _total(hub, dataset, image_size)
 
 
-# def test_huggingface_object_detection(
-#     object_detection_dataset: Dataset, tmpdir: Path
-# ):
-#     image_size = 32
-#     dataset = object_detection_dataset
-
-#     # test hub
-#     name = "test_det"
-#     hub = HuggingFaceHub.new(
-#         name=name,
-#         task=TaskType.OBJECT_DETECTION,
-#         model_type="YOLOS",
-#         model_size="tiny",
-#         categories=object_detection_dataset.category_names,
-#         root_dir=tmpdir,
-#     )
-#     hub = HuggingFaceHub.load(name=name, root_dir=tmpdir)
-#     hub: HuggingFaceHub = HuggingFaceHub.from_model_config(
-#         name=name,
-#         model_config_file=tmpdir / name / HuggingFaceHub.MODEL_CONFIG_FILE,
-#         root_dir=tmpdir,
-#     )
-
-#     _total(hub, dataset, image_size)
-
-
-# def test_huggingface_classification(
-#     classification_dataset: Dataset, tmpdir: Path
-# ):
-#     image_size = 224
-#     dataset = classification_dataset
-
-#     # test hub
-#     name = "test_cls"
-#     hub = HuggingFaceHub.new(
-#         name=name,
-#         task=TaskType.CLASSIFICATION,
-#         model_type="ViT",
-#         model_size="tiny",
-#         categories=classification_dataset.category_names,
-#         root_dir=tmpdir,
-#     )
-#     hub = HuggingFaceHub.load(name=name, root_dir=tmpdir)
-#     hub: HuggingFaceHub = HuggingFaceHub.from_model_config(
-#         name=name,
-#         model_config_file=tmpdir / name / HuggingFaceHub.MODEL_CONFIG_FILE,
-#         root_dir=tmpdir,
-#     )
+def test_huggingface_object_detection(object_detection_dataset: Dataset, tmpdir: Path):
+    image_size = 32
+    dataset = object_detection_dataset
+
+    # test hub
+    name = "test_det"
+    hub = HuggingFaceHub.new(
+        name=name,
+        task=TaskType.OBJECT_DETECTION,
+        model_type="YOLOS",
+        model_size="tiny",
+        categories=object_detection_dataset.category_names,
+        root_dir=tmpdir,
+    )
+    hub = HuggingFaceHub.load(name=name, root_dir=tmpdir)
+    hub: HuggingFaceHub = HuggingFaceHub.from_model_config(
+        name=name,
+        model_config_file=tmpdir / name / HuggingFaceHub.MODEL_CONFIG_FILE,
+        root_dir=tmpdir,
+    )
+
+    _total(hub, dataset, image_size)
+
+
+def test_huggingface_classification(classification_dataset: Dataset, tmpdir: Path):
+    image_size = 224
+    dataset = classification_dataset
 
-#     _total(hub, dataset, image_size)
+    # test hub
+    name = "test_cls"
+    hub = HuggingFaceHub.new(
+        name=name,
+        task=TaskType.CLASSIFICATION,
+        model_type="ViT",
+        model_size="tiny",
+        categories=classification_dataset.category_names,
+        root_dir=tmpdir,
+    )
+    hub = HuggingFaceHub.load(name=name, root_dir=tmpdir)
+    hub: HuggingFaceHub = HuggingFaceHub.from_model_config(
+        name=name,
+        model_config_file=tmpdir / name / HuggingFaceHub.MODEL_CONFIG_FILE,
+        root_dir=tmpdir,
+    )
+
+    _total(hub, dataset, image_size)
 
 
 def test_non_hold(classification_dataset: Dataset, tmpdir: Path):
     image_size = 32
     dataset = classification_dataset
 
     # test hub
```

### Comparing `waffle_hub-0.1.9/waffle_hub/__init__.py` & `waffle_hub-0.2.0/waffle_hub/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-__version__ = "0.1.9"
+__version__ = "0.2.0"
 
 import enum
 import importlib
 import warnings
-import enum
 from collections import OrderedDict
 
 from tabulate import tabulate
 
 # pytorch install check (necessary installation)
 pytorch_versions = ["1.13.1"]
 try:
@@ -87,14 +86,15 @@
         table_data,
         headers=["Backend", "Version"],
         tablefmt="simple_outline",
     )
 
     return table
 
+
 class CustomEnumMeta(enum.EnumMeta):
     def __contains__(cls, item):
         if isinstance(item, str):
             return item.upper() in cls._member_names_
         return super().__contains__(item)
 
     def __upper__(self):
@@ -147,11 +147,12 @@
     HUGGINGFACE = enum.auto()
     TRANSFORMERS = enum.auto()
 
 
 class TaskType(BaseEnum):
     CLASSIFICATION = enum.auto()
     OBJECT_DETECTION = enum.auto()
-    SEGMENTATION = enum.auto()
+    SEMANTIC_SEGMENTATION = enum.auto()
+    INSTANCE_SEGMENTATION = enum.auto()
     KEYPOINT_DETECTION = enum.auto()
     TEXT_RECOGNITION = enum.auto()
     REGRESSION = enum.auto()
```

### Comparing `waffle_hub-0.1.9/waffle_hub/dataset/adapter/coco.py` & `waffle_hub-0.2.0/waffle_hub/dataset/adapter/coco.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-from typing import Union
 from pathlib import Path
+from typing import Union
 
 from waffle_utils.file import io
 
 from waffle_hub import TaskType
+from waffle_hub.utils.conversion import convert_rle_to_polygon
 
 
-def _export_coco_classification(
+def _export_coco(
     self,
     export_dir: Path,
     train_ids: list,
     val_ids: list,
     test_ids: list,
     unlabeled_ids: list,
 ):
-    """Export dataset to COCO format for classification task
+    """Export dataset to COCO format
 
     Args:
         export_dir (Path): Path to export directory
         train_ids (list): List of train ids
         val_ids (list): List of validation ids
         test_ids (list): List of test ids
         unlabeled_ids (list): List of unlabeled ids
@@ -29,23 +30,26 @@
 
     for split, image_ids in zip(
         ["train", "val", "test", "unlabeled"],
         [train_ids, val_ids, test_ids, unlabeled_ids],
     ):
         if len(image_ids) == 0:
             continue
-        
+
         coco = {
-            "categories": [{
-                "id": category.category_id,
-                "name": category.name,
-                "supercategory": category.supercategory,
-            } for category in self.categories.values()], 
-            "images": [], 
-            "annotations": []
+            "categories": [
+                {
+                    "id": category.category_id,
+                    "name": category.name,
+                    "supercategory": category.supercategory,
+                }
+                for category in self.categories.values()
+            ],
+            "images": [],
+            "annotations": [],
         }
 
         for image_id in image_ids:
             image = self.images[image_id]
             image_path = self.raw_image_dir / image.file_name
             image_dst_path = image_dir / image.file_name
             io.copy_file(image_path, image_dst_path, create_directory=True)
@@ -53,17 +57,19 @@
             d = image.to_dict()
             image_id = d.pop("image_id")
             coco["images"].append({"id": image_id, **d})
 
             annotations = self.image_to_annotations[image_id]
             for annotation in annotations:
                 d = annotation.to_dict()
+                if d.get("segmentation", None):
+                    d["segmentation"] = convert_rle_to_polygon(d["segmentation"])
                 annotation_id = d.pop("annotation_id")
                 coco["annotations"].append({"id": annotation_id, **d})
-        
+
         io.save_json(coco, export_dir / f"{split}.json", create_directory=True)
 
 
 def export_coco(self, export_dir: Union[str, Path]) -> str:
     """Export dataset to COCO format
 
     Args:
@@ -73,18 +79,16 @@
         str: Path to export directory
     """
     export_dir = Path(export_dir)
 
     train_ids, val_ids, test_ids, unlabeled_ids = self.get_split_ids()
 
     if self.task == TaskType.CLASSIFICATION:
-        _export_coco_classification(
-            self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids
-        )
+        _export_coco(self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids)
     elif self.task == TaskType.OBJECT_DETECTION:
-        _export_coco_classification(
-            self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids
-        )
+        _export_coco(self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids)
+    elif self.task == TaskType.INSTANCE_SEGMENTATION:
+        _export_coco(self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids)
     else:
         raise ValueError(f"Unsupported task type: {self.task_type}")
 
     return str(export_dir)
```

### Comparing `waffle_hub-0.1.9/waffle_hub/dataset/adapter/huggingface.py` & `waffle_hub-0.2.0/waffle_hub/dataset/adapter/huggingface.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.9/waffle_hub/dataset/adapter/yolo.py` & `waffle_hub-0.2.0/waffle_hub/dataset/adapter/yolo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import warnings
-from typing import Union
 from pathlib import Path
+from typing import Union
 
 from waffle_utils.file import io
 
 from waffle_hub import TaskType
+from waffle_hub.utils.conversion import merge_multi_segment
 
 
 def _export_yolo_classification(
     self,
     export_dir: Path,
     train_ids: list,
     val_ids: list,
@@ -38,23 +39,19 @@
 
         for image_id in image_ids:
             image = self.images[image_id]
             image_path = self.raw_image_dir / image.file_name
 
             annotations = self.get_annotations(image_id)
             if len(annotations) > 1:
-                warnings.warn(
-                    f"Multi label does not support yet. Skipping {image_path}."
-                )
+                warnings.warn(f"Multi label does not support yet. Skipping {image_path}.")
                 continue
             category_id = annotations[0].category_id
 
-            image_dst_path = (
-                split_dir / self.categories[category_id].name / image.file_name
-            )
+            image_dst_path = split_dir / self.categories[category_id].name / image.file_name
             io.copy_file(image_path, image_dst_path, create_directory=True)
 
 
 def _export_yolo_detection(
     self,
     export_dir: Path,
     train_ids: list,
@@ -91,17 +88,15 @@
             image_dst_path = image_dir / image.file_name
             label_dst_path = (label_dir / image.file_name).with_suffix(".txt")
             io.copy_file(image_path, image_dst_path, create_directory=True)
 
             W = image.width
             H = image.height
 
-            annotations = self.image_to_annotations[
-                image.image_id
-            ]
+            annotations = self.image_to_annotations[image.image_id]
             label_txts = []
             for annotation in annotations:
                 x1, y1, w, h = annotation.bbox
                 x1, w = x1 / W, w / W
                 y1, h = y1 / H, h / H
                 cx, cy = x1 + w / 2, y1 + h / 2
 
@@ -110,46 +105,96 @@
                 label_txts.append(f"{category_id} {cx} {cy} {w} {h}")
 
             io.make_directory(label_dst_path.parent)
             with open(label_dst_path, "w") as f:
                 f.write("\n".join(label_txts))
 
 
+def _export_yolo_segmentation(
+    self,
+    export_dir: Path,
+    train_ids: list,
+    val_ids: list,
+    test_ids: list,
+    unlabeled_ids: list,
+):
+    io.make_directory(export_dir)
+
+    for split, image_ids in zip(
+        ["train", "val", "test", "unlabeled"],
+        [train_ids, val_ids, test_ids, unlabeled_ids],
+    ):
+        if len(image_ids) == 0:
+            continue
+
+        image_dir = export_dir / split / "images"
+        label_dir = export_dir / split / "labels"
+
+        io.make_directory(image_dir)
+        io.make_directory(label_dir)
+
+        for image in self.get_images(image_ids):
+            image_path = self.raw_image_dir / image.file_name
+            image_dst_path = image_dir / image.file_name
+            label_dst_path = (label_dir / image.file_name).with_suffix(".txt")
+            io.copy_file(image_path, image_dst_path, create_directory=True)
+
+            W = image.width
+            H = image.height
+
+            annotations = self.image_to_annotations[image.image_id]
+            label_txts = []
+            for annotation in annotations:
+                x1, y1, w, h = annotation.bbox
+                x1, w = x1 / W, w / W
+                y1, h = y1 / H, h / H
+
+                category_id = annotation.category_id - 1
+
+                segment = merge_multi_segment(annotation.segmentation, (W, H))
+                segment[0::2] = [x / W for x in segment[0::2]]
+                segment[1::2] = [y / H for y in segment[1::2]]
+                segment = " ".join(map(str, segment))
+
+                label_txts.append(f"{category_id} {segment}")
+
+            io.make_directory(label_dst_path.parent)
+            with open(label_dst_path, "w") as f:
+                f.write("\n".join(label_txts))
+
+
 def export_yolo(self, export_dir: Union[str, Path]) -> str:
     """Export dataset to YOLO format
 
     Args:
         export_dir (Union[str, Path]): Path to export directory
 
     Returns:
         str: Path to export directory
     """
     export_dir = Path(export_dir)
 
     train_ids, val_ids, test_ids, unlabeled_ids = self.get_split_ids()
 
     if self.task == TaskType.CLASSIFICATION:
-        _export_yolo_classification(
-            self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids
-        )
+        _export_yolo_classification(self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids)
     elif self.task == TaskType.OBJECT_DETECTION:
-        _export_yolo_detection(
-            self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids
-        )
+        _export_yolo_detection(self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids)
+    elif self.task == TaskType.INSTANCE_SEGMENTATION:
+        _export_yolo_segmentation(self, export_dir, train_ids, val_ids, test_ids, unlabeled_ids)
     else:
         raise ValueError(f"Unsupported task type: {self.task}")
 
     io.save_yaml(
         {
             "path": str(export_dir.absolute()),
             "train": "train",
             "val": "val",
             "test": "test",
             "names": {
-                category_id - 1: category.name
-                for category_id, category in self.categories.items()
+                category_id - 1: category.name for category_id, category in self.categories.items()
             },
         },
         export_dir / "data.yaml",
     )
 
     return str(export_dir)
```

### Comparing `waffle_hub-0.1.9/waffle_hub/dataset/dataset.py` & `waffle_hub-0.2.0/waffle_hub/dataset/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,15 +384,15 @@
             if categories != coco.loadCats(coco.getCatIds()):
                 raise ValueError("categories should be same between coco files.")
 
         coco_cat_id_to_waffle_cat_id = {}
         for i, category in enumerate(categories, start=1):
             coco_category_id = category.pop("id")
             coco_cat_id_to_waffle_cat_id[coco_category_id] = i
-            ds.add_categories([Category.from_dict({**category, "category_id": i})])
+            ds.add_categories([Category.from_dict({**category, "category_id": i}, task=ds.task)])
 
         # import coco dataset
         total_length = sum([len(coco.getImgIds()) for coco in cocos])
         logging.info(f"Importing coco dataset. Total length: {total_length}")
         pgbar = tqdm.tqdm(total=total_length, desc="Importing coco dataset")
 
         image_id = 1
@@ -431,15 +431,16 @@
                                 {
                                     **annotation_dict,
                                     "image_id": image_id,
                                     "annotation_id": annotation_id,
                                     "category_id": coco_cat_id_to_waffle_cat_id[
                                         annotation_dict["category_id"]
                                     ],
-                                }
+                                },
+                                task=ds.task,
                             )
                         ]
                     )
                     annotation_id += 1
 
                 image_ids.append(image_id)
                 image_id += 1
```

### Comparing `waffle_hub-0.1.9/waffle_hub/experimental/auto_label/grounding_dino.py` & `waffle_hub-0.2.0/waffle_hub/experimental/auto_label/grounding_dino.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.9/waffle_hub/experimental/serve.py` & `waffle_hub-0.2.0/waffle_hub/experimental/serve.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.9/waffle_hub/hub/adapter/hugging_face/hugging_face_hub.py` & `waffle_hub-0.2.0/waffle_hub/hub/adapter/hugging_face/hugging_face_hub.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 BACKEND_NAME = "transformers"
 BACKEND_VERSION = get_installed_backend_version(BACKEND_NAME)
 
 import os
 import warnings
 from copy import deepcopy
+from functools import cached_property
+from pathlib import Path
 from typing import Callable, Union
 
 import torch
 from torchvision import transforms as T
 from transformers import (
     AutoImageProcessor,
     AutoModelForImageClassification,
@@ -54,14 +56,18 @@
                 metric_key_prefix="train",
             )
             return control_copy
 
 
 class HuggingFaceHub(BaseHub):
 
+    # Override
+    LAST_CKPT_FILE = "weights/last_ckpt"
+    BEST_CKPT_FILE = "weights/best_ckpt"
+
     # Common
     MODEL_TYPES = {
         "object_detection": {
             "DETA": {
                 "base": "jozhang97/deta-resnet-50",
             },
             "DETR": {
@@ -125,17 +131,24 @@
             task=task,
             model_type=model_type,
             model_size=model_size,
             categories=categories,
             root_dir=root_dir,
         )
 
-        self.pretrained_model: str = self.MODEL_TYPES[self.task][self.model_type][self.model_size]
-        self.best_ckpt_dir = self.hub_dir / "weights" / "best_ckpt"
-        self.train_input = None
+    # Override
+    @cached_property
+    def best_ckpt_file(self) -> Path:
+        """Best Checkpoint File"""
+        return self.hub_dir / HuggingFaceHub.BEST_CKPT_FILE
+
+    @cached_property
+    def last_ckpt_file(self) -> Path:
+        """Last Checkpoint File"""
+        return self.hub_dir / HuggingFaceHub.LAST_CKPT_FILE
 
     @classmethod
     def new(
         cls,
         name: str,
         task: str = None,
         model_type: str = None,
@@ -151,59 +164,56 @@
             model_size=model_size,
             categories=categories,
             root_dir=root_dir,
         )
 
     def on_train_start(self, cfg: TrainConfig):
         # overwrite train config with default config
-        cfg.pretrained_model = self.pretrained_model
-        for k, v in cfg.to_dict().items():
-            if v is None:
-                setattr(cfg, k, self.DEFAULT_PARAMAS[self.task][k])
+        cfg.pretrained_model = self.MODEL_TYPES[self.task][self.model_type][self.model_size]
 
         # setting
         if cfg.device != "cpu":
             os.environ["CUDA_VISIBLE_DEVICES"] = cfg.device
         else:
             os.environ["CUDA_VISIBLE_DEVICES"] = "-1"
 
         dataset = load_from_disk(cfg.dataset_path)
 
         if self.task == "classification":
             helper = ClassifierInputHelper(cfg.pretrained_model, cfg.image_size)
-            self.train_input = helper.get_train_input()
+            cfg.train_input = helper.get_train_input()
             categories = dataset["train"].features["label"].names
             id2label = {index: x for index, x in enumerate(categories, start=0)}
-            self.train_input.model = AutoModelForImageClassification.from_pretrained(
-                self.pretrained_model,
+            cfg.train_input.model = AutoModelForImageClassification.from_pretrained(
+                cfg.pretrained_model,
                 num_labels=len(id2label),
                 ignore_mismatched_sizes=True,
             )
 
         elif self.task == "object_detection":
             helper = ObjectDetectionInputHelper(cfg.pretrained_model, cfg.image_size)
-            self.train_input = helper.get_train_input()
+            cfg.train_input = helper.get_train_input()
             categories = dataset["train"].features["objects"].feature["category"].names
             id2label = {index: x for index, x in enumerate(categories, start=0)}
             label2id = {x: index for index, x in enumerate(categories, start=0)}
-            self.train_input.model = AutoModelForObjectDetection.from_pretrained(
-                self.pretrained_model,
+            cfg.train_input.model = AutoModelForObjectDetection.from_pretrained(
+                cfg.pretrained_model,
                 id2label=id2label,
                 label2id=label2id,
                 ignore_mismatched_sizes=True,
             )
         else:
             raise NotImplementedError
 
         transforms = helper.get_transforms()
         dataset["train"] = dataset["train"].with_transform(transforms)
         dataset["val"] = dataset["val"].with_transform(transforms)
-        self.train_input.dataset = dataset
+        cfg.train_input.dataset = dataset
 
-        self.train_input.training_args = TrainingArguments(
+        cfg.train_input.training_args = TrainingArguments(
             output_dir=str(self.artifact_dir),
             per_device_train_batch_size=cfg.batch_size,
             num_train_epochs=cfg.epochs,
             remove_unused_columns=False,
             push_to_hub=False,
             logging_strategy="epoch" if cfg.verbose else "no",
             evaluation_strategy="epoch",
@@ -212,21 +222,21 @@
             seed=cfg.seed,
             greater_is_better=True,
         )
 
     def training(self, cfg: TrainConfig, callback: TrainCallback):
 
         trainer = Trainer(
-            model=self.train_input.model,
-            args=self.train_input.training_args,
-            data_collator=self.train_input.collator,
-            train_dataset=self.train_input.dataset["train"],
-            eval_dataset=self.train_input.dataset["val"],
-            tokenizer=self.train_input.image_processor,
-            compute_metrics=self.train_input.compute_metrics,
+            model=cfg.train_input.model,
+            args=cfg.train_input.training_args,
+            data_collator=cfg.train_input.collator,
+            train_dataset=cfg.train_input.dataset["train"],
+            eval_dataset=cfg.train_input.dataset["val"],
+            tokenizer=cfg.train_input.image_processor,
+            compute_metrics=cfg.train_input.compute_metrics,
         )
         trainer.add_callback(CustomCallback(trainer))
         trainer.train()
         trainer.save_model(str(self.artifact_dir / "weights"))
         self.train_log = trainer.state.log_history
 
     def get_metrics(self) -> list[list[dict]]:
@@ -245,79 +255,76 @@
             metrics.append(epoch_metrics)
 
         return metrics
 
     def on_train_end(self, cfg: TrainConfig):
         io.copy_files_to_directory(
             self.artifact_dir / "weights",
-            self.best_ckpt_dir,
+            self.best_ckpt_file,
             create_directory=True,
         )
         io.save_json(self.get_metrics(), self.metric_file)
 
-    def get_preprocess(self, task, pretrained_model: str) -> Callable:
+    def get_preprocess(self, task, pretrained_model: str = None) -> Callable:
+        if pretrained_model is None:
+            pretrained_model = self.best_ckpt_file
         image_processer = AutoImageProcessor.from_pretrained(pretrained_model)
 
         normalize = T.Normalize(image_processer.image_mean, image_processer.image_std, inplace=True)
 
         def preprocess(x, *args, **kwargs):
             return normalize(x)
 
         return preprocess
 
-    def get_postprocess(self, task: str) -> Callable:
+    def get_postprocess(self, task: str, pretrained_model: str = None) -> Callable:
+        if pretrained_model is None:
+            pretrained_model = self.best_ckpt_file
+        image_processer = AutoImageProcessor.from_pretrained(pretrained_model)
+
         if task == "classification":
 
             def inner(x: ModelOutput, *args, **kwargs) -> torch.Tensor:
                 return [x.logits]
 
         elif task == "object_detection":
+            post_process = image_processer.post_process_object_detection
 
             def inner(x: ModelOutput, *args, **kwargs) -> torch.Tensor:
 
-                if x.logits.shape[-1] != len(self.categories):
-                    x.logits = x.logits[:, :, :-1]  # remove background
-                confidences, category_ids = torch.max(x.logits[:, :, :], dim=-1)
-                cxcywh = x.pred_boxes[:, :, :4]
-                cx, cy, w, h = torch.unbind(cxcywh, dim=-1)
-                x1 = cx - w / 2
-                y1 = cy - h / 2
-                x2 = cx + w / 2
-                y2 = cy + h / 2
-                xyxy = torch.stack([x1, y1, x2, y2], dim=-1)
+                x = post_process(x, threshold=-1)
+
+                xyxy = list(map(lambda x: x["boxes"], x))
+                confidences = list(map(lambda x: x["scores"], x))
+                category_ids = list(map(lambda x: x["labels"], x))
 
                 return xyxy, confidences, category_ids
 
         else:
             raise NotImplementedError(f"Task {task} is not implemented.")
 
         return inner
 
     def get_model(self) -> ModelWrapper:
         self.check_train_sanity()
 
         # get adapt functions
-        preprocess = self.get_preprocess(self.task, self.pretrained_model)
+        preprocess = self.get_preprocess(self.task)
         postprocess = self.get_postprocess(self.task)
 
         # get model
         if self.task == "object_detection":
             model = AutoModelForObjectDetection.from_pretrained(
-                str(self.best_ckpt_dir),
+                str(self.best_ckpt_file),
             )
         elif self.task == "classification":
             model = AutoModelForImageClassification.from_pretrained(
-                str(self.best_ckpt_dir),
+                str(self.best_ckpt_file),
             )
 
         model = ModelWrapper(
             model=model.eval(),
             preprocess=preprocess,
             postprocess=postprocess,
         )
 
         return model
-
-    def check_train_sanity(self) -> bool:
-        if not (self.model_config_file.exists() and self.best_ckpt_dir.exists()):
-            raise FileNotFoundError("Train first! hub.train(...).")
-        return True
```

### Comparing `waffle_hub-0.1.9/waffle_hub/hub/adapter/hugging_face/train_input_helper.py` & `waffle_hub-0.2.0/waffle_hub/hub/adapter/hugging_face/train_input_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,26 +34,22 @@
 
 
 class TrainInputHelper(ABC):
     """
     This class is designed to assist with passing arguments to the Hugging Face's Trainer function.
     """
 
-    def __init__(
-        self, pretrained_model: str, image_size: Union[int, list[int]]
-    ) -> None:
+    def __init__(self, pretrained_model: str, image_size: Union[int, list[int]]) -> None:
         self.pretrained_model = pretrained_model
         self.image_size = image_size
 
         if isinstance(image_size, int):
             self.image_size = (image_size, image_size)
 
-        self.image_processor: AutoImageProcessor = self.get_image_processor(
-            self.pretrained_model
-        )
+        self.image_processor: AutoImageProcessor = self.get_image_processor(self.pretrained_model)
         self.train_input = TrainInput()
 
     def get_image_processor(self, pretrained_model: str) -> AutoImageProcessor:
         """
         Returns an instance of AutoImageProcessor for a given pre-trained model.
 
         Args:
@@ -110,46 +106,40 @@
         train_input.image_processor = self.image_processor
         train_input.collator = self.get_collator()
         train_input.compute_metrics = self.get_compute_metrics()
         return train_input
 
 
 class ClassifierInputHelper(TrainInputHelper):
-    def __init__(
-        self, pretrained_model: str, image_size: Union[int, list[int]]
-    ) -> None:
+    def __init__(self, pretrained_model: str, image_size: Union[int, list[int]]) -> None:
         super().__init__(pretrained_model, image_size)
 
     def get_transforms(self) -> Callable:
         normalize = T.Normalize(
             mean=self.image_processor.image_mean,
             std=self.image_processor.image_std,
         )
 
         size = (
-            self.image_processor.size["shortest_edge"]
+            (self.image_processor.size["shortest_edge"],) * 2
             if "shortest_edge" in self.image_processor.size
             else (
-                self.image_processor.size["height"],
                 self.image_processor.size["width"],
+                self.image_processor.size["height"],
             )
         )
-        if size != self.image_size:
+        if tuple(size) != tuple(self.image_size):
             raise ValueError(
                 f"pretrained model's image size is {size}, but you set {self.image_size}."
             )
 
-        _transforms = T.Compose(
-            [T.RandomResizedCrop(size), T.ToTensor(), normalize]
-        )
+        _transforms = T.Compose([T.RandomResizedCrop(size[::-1]), T.ToTensor(), normalize])
 
         def transforms(examples: dict) -> dict:
-            examples["pixel_values"] = [
-                _transforms(img.convert("RGB")) for img in examples["image"]
-            ]
+            examples["pixel_values"] = [_transforms(img.convert("RGB")) for img in examples["image"]]
             del examples["image"]
             return examples
 
         return transforms
 
     def get_collator(self) -> Callable:
         return DefaultDataCollator(return_tensors="pt")
@@ -162,48 +152,40 @@
             predictions = np.argmax(logits, axis=1)
             return metric.compute(predictions=predictions, references=labels)
 
         return compute_metrics
 
 
 class ObjectDetectionInputHelper(TrainInputHelper):
-    def __init__(
-        self, pretrained_model: str, image_size: Union[int, list[int]]
-    ) -> None:
+    def __init__(self, pretrained_model: str, image_size: Union[int, list[int]]) -> None:
         super().__init__(pretrained_model, image_size)
 
     def get_transforms(self) -> Callable:
         size = (
-            self.image_processor.size["shortest_edge"]
+            (self.image_processor.size["shortest_edge"],) * 2
             if "shortest_edge" in self.image_processor.size
             else (
-                self.image_processor.size["height"],
                 self.image_processor.size["width"],
+                self.image_processor.size["height"],
             )
         )
 
-        if size != self.image_size:
-            warnings.warn(
-                f"pretrained model's image size is {size}, but you set {self.image_size}."
-            )
+        if tuple(size) != tuple(self.image_size):
+            warnings.warn(f"pretrained model's image size is {size}, but you set {self.image_size}.")
 
         _transforms = albumentations.Compose(
             [
-                albumentations.Resize(size, size),
-                albumentations.HorizontalFlip(p=1.0),
-                albumentations.RandomBrightnessContrast(p=1.0),
+                albumentations.Resize(width=size[0], height=size[1]),
+                albumentations.HorizontalFlip(p=0.5),
+                albumentations.RandomBrightnessContrast(p=0.5),
             ],
-            bbox_params=albumentations.BboxParams(
-                format="coco", label_fields=["category"]
-            ),
+            bbox_params=albumentations.BboxParams(format="coco", label_fields=["category"]),
         )
 
-        def formatted_anns(
-            image_id: int, category: list, area: list, bbox: list
-        ) -> list[dict]:
+        def formatted_anns(image_id: int, category: list, area: list, bbox: list) -> list[dict]:
             annotations = []
             for i in range(0, len(category)):
                 new_ann = {
                     "image_id": image_id,
                     "category_id": category[i],
                     "isCrowd": 0,
                     "area": area[i],
@@ -230,22 +212,18 @@
                 categories.append(out["category"])
 
             targets = [
                 {
                     "image_id": id_,
                     "annotations": formatted_anns(id_, cat_, ar_, box_),
                 }
-                for id_, cat_, ar_, box_ in zip(
-                    image_ids, categories, area, bboxes
-                )
+                for id_, cat_, ar_, box_ in zip(image_ids, categories, area, bboxes)
             ]
 
-            return self.image_processor(
-                images=images, annotations=targets, return_tensors="pt"
-            )
+            return self.image_processor(images=images, annotations=targets, return_tensors="pt")
 
         return transforms
 
     def get_collator(self) -> Callable:
         def collate_fn(batch: list[dict]) -> dict:
             pixel_values = [item["pixel_values"] for item in batch]
             labels = [item["labels"] for item in batch]
```

### Comparing `waffle_hub-0.1.9/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py` & `waffle_hub-0.2.0/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.9/waffle_hub/hub/adapter/tx_model/configs/model_cfg.py` & `waffle_hub-0.2.0/waffle_hub/hub/adapter/tx_model/configs/model_cfg.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.9/waffle_hub/hub/adapter/tx_model/tx_model_hub.py` & `waffle_hub-0.2.0/waffle_hub/hub/adapter/tx_model/tx_model_hub.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,31 @@
                 "s": "temp/autocare_tx_model/classifiers/small/model.pth",
                 "m": "temp/autocare_tx_model/classifiers/medium/model.pth",
                 "l": "temp/autocare_tx_model/classifiers/large/model.pth",
             }
         },
     }
 
+    DEFAULT_PARAMAS = {
+        "object_detection": {
+            "epochs": 50,
+            "image_size": [640, 640],
+            "learning_rate": 0.01,
+            "letter_box": True,
+            "batch_size": 16,
+        },
+        "classification": {
+            "epochs": 50,
+            "image_size": [224, 224],
+            "learning_rate": 0.01,
+            "letter_box": False,
+            "batch_size": 16,
+        },
+    }
+
     def __init__(
         self,
         name: str,
         task: str = None,
         model_type: str = None,
         model_size: str = None,
         categories: Union[list[dict], list] = None,
@@ -189,15 +206,15 @@
 
     # Train Hook
     def on_train_start(self, cfg: TrainConfig):
         # set data
         cfg.dataset_path: Path = Path(cfg.dataset_path)
         data_config = get_data_config(
             self.DATA_TYPE_MAP[self.task],
-            [cfg.image_size, cfg.image_size],
+            cfg.image_size if isinstance(cfg.image_size, list) else [cfg.image_size, cfg.image_size],
             cfg.batch_size,
             cfg.workers,
             str(cfg.dataset_path / "train.json"),
             str(cfg.dataset_path / "images"),
             str(cfg.dataset_path / "val.json"),
             str(cfg.dataset_path / "images"),
             str(cfg.dataset_path / "test.json"),
```

### Comparing `waffle_hub-0.1.9/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py` & `waffle_hub-0.2.0/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,29 +25,29 @@
 
 class UltralyticsHub(BaseHub):
 
     # Common
     MODEL_TYPES = {
         "object_detection": {"yolov8": list("nsmlx")},
         "classification": {"yolov8": list("nsmlx")},
-        # "segmentation": {"yolov8": list("nsmlx")},
+        "instance_segmentation": {"yolov8": list("nsmlx")},
         # "keypoint_detection": {"yolov8": list("nsmlx")},
     }
 
     # Backend Specifics
     TASK_MAP = {
         "object_detection": "detect",
         "classification": "classify",
-        # "segmentation": "segment"
+        "instance_segmentation": "segment"
         # "keypoint_detection": "pose"
     }
     TASK_SUFFIX = {
         "detect": "",
         "classify": "-cls",
-        # "segment": "-seg",
+        "segment": "-seg",
     }
 
     DEFAULT_PARAMAS = {
         "object_detection": {
             "epochs": 50,
             "image_size": [640, 640],
             "learning_rate": 0.01,
@@ -57,14 +57,21 @@
         "classification": {
             "epochs": 50,
             "image_size": [224, 224],
             "learning_rate": 0.01,
             "letter_box": False,
             "batch_size": 16,
         },
+        "instance_segmentation": {
+            "epochs": 50,
+            "image_size": [640, 640],
+            "learning_rate": 0.01,
+            "letter_box": True,
+            "batch_size": 16,
+        },
     }
 
     def __init__(
         self,
         name: str,
         task: str = None,
         model_type: str = None,
@@ -138,25 +145,33 @@
 
         elif task == "object_detection":
             normalize = T.Normalize([0, 0, 0], [1, 1, 1], inplace=True)
 
             def preprocess(x, *args, **kwargs):
                 return normalize(x)
 
+        elif task == "instance_segmentation":
+            normalize = T.Normalize([0, 0, 0], [1, 1, 1], inplace=True)
+
+            def preprocess(x, *args, **kwargs):
+                return normalize(x)
+
         else:
             raise NotImplementedError(f"Task {task} is not implemented.")
 
         return preprocess
 
     def get_postprocess(self, task: str, *args, **kwargs):
 
+        id_mapper: list[int] = kwargs.get("id_mapper", [i for i in range(len(self.categories))])
+
         if task == "classification":
 
             def inner(x: torch.Tensor, *args, **kwargs):
-                return [x]
+                return [x[:, id_mapper]]
 
         elif task == "object_detection":
 
             def inner(x: torch.Tensor, image_size: tuple[int, int], *args, **kwargs):
                 x = x[0]  # x[0]: prediction, x[1]: TODO: what is this...?
                 x = x.transpose(1, 2)
 
@@ -166,19 +181,59 @@
                 y1 = cy - h / 2
                 x2 = cx + w / 2
                 y2 = cy + h / 2
                 xyxy = torch.stack([x1, y1, x2, y2], dim=-1)
 
                 xyxy[:, :, ::2] /= image_size[0]
                 xyxy[:, :, 1::2] /= image_size[1]
-                probs = x[:, :, 4:]
+                probs = x[:, :, 4:][:, :, id_mapper]
                 confidences, class_ids = torch.max(probs, dim=-1)
 
                 return xyxy, confidences, class_ids
 
+        elif task == "instance_segmentation":
+            num_category = len(self.categories)
+
+            def inner(x: torch.Tensor, image_size: tuple[int, int], *args, **kwargs):
+                preds = x[0]  # x[0]: prediction, x[1]: TODO: what is this...?
+                preds = preds.transpose(1, 2)
+
+                probs = preds[:, :, 4 : 4 + num_category]
+                confidences, class_ids = torch.max(probs, dim=-1)
+                _, indicies = torch.topk(
+                    confidences, k=min(100, confidences.shape[-1]), dim=-1, largest=True
+                )  # TODO: make k configurable
+
+                preds = torch.gather(preds, 1, indicies.unsqueeze(-1).repeat(1, 1, preds.shape[-1]))
+                confidences = torch.gather(confidences, 1, indicies)
+                class_ids = torch.gather(class_ids, 1, indicies)
+
+                cxcywh = preds[:, :, :4]
+                cx, cy, w, h = torch.unbind(cxcywh, dim=-1)
+                x1 = cx - w / 2
+                y1 = cy - h / 2
+                x2 = cx + w / 2
+                y2 = cy + h / 2
+                xyxy = torch.stack([x1, y1, x2, y2], dim=-1)
+
+                xyxy[:, :, ::2] /= image_size[0]
+                xyxy[:, :, 1::2] /= image_size[1]
+
+                # [batch, mask_dim, mask_height, mask_width] -> [batch, num_mask, mask_height * mask_width]
+                protos = x[1][-1] if len(x[1]) == 3 else x[1]
+                mask_size = (protos.shape[-2], protos.shape[-1])
+                protos = protos.view(
+                    protos.shape[0], -1, protos.shape[-2] * protos.shape[-1]
+                ).float()
+
+                masks = preds[:, :, 4 + num_category :]
+                masks = torch.bmm(masks, protos).sigmoid().view(masks.shape[0], -1, *mask_size)
+
+                return xyxy, confidences, class_ids, masks
+
         else:
             raise NotImplementedError(f"Task {task} is not implemented.")
 
         return inner
 
     def get_metrics(self) -> list[list[dict]]:
         # read csv file
@@ -225,41 +280,28 @@
                 )
                 if len(yaml_files) != 1:
                     raise FileNotFoundError(f"Ambiguous data file. Detected files: {yaml_files}")
                 cfg.dataset_path = Path(yaml_files[0]).absolute()
             else:
                 cfg.dataset_path = cfg.dataset_path.absolute()
         elif self.backend_task_name == "classify":
-
-            from torchvision.datasets.folder import ImageFolder
-
-            def find_categories(_, directory: str):
-                return directory, {v["name"]: i for i, v in enumerate(self.categories)}
-
-            ImageFolder.find_categories = find_categories
-
             if not cfg.dataset_path.is_dir():
                 raise ValueError(
                     f"Classification dataset should be directory. Not {cfg.dataset_path}"
                 )
             cfg.dataset_path = cfg.dataset_path.absolute()
         cfg.dataset_path = str(cfg.dataset_path)
 
         # pretrained model
         cfg.pretrained_model = (
             cfg.pretrained_model
             if cfg.pretrained_model
             else self.model_type + self.model_size + self.TASK_SUFFIX[self.backend_task_name] + ".pt"
         )
 
-        # overwrite train config with default config
-        for k, v in cfg.to_dict().items():
-            if v is None:
-                setattr(cfg, k, self.DEFAULT_PARAMAS[self.task][k])
-
     def training(self, cfg: TrainConfig, callback: TrainCallback):
 
         model = YOLO(cfg.pretrained_model, task=self.backend_task_name)
         model.train(
             data=cfg.dataset_path,
             epochs=cfg.epochs,
             batch=cfg.batch_size,
@@ -293,19 +335,35 @@
     def get_model(self):
         """Get model.
         Returns:
             ModelWrapper: Model wrapper
         """
         self.check_train_sanity()
 
+        # get model
+        model = YOLO(self.best_ckpt_file).model.eval()
+
         # get adapt functions
+        names: list[str] = list(map(lambda x: x["name"], self.categories))
+        yolo_names: dict[int, str] = model.names
+        if len(names) != len(yolo_names):
+            raise ValueError(
+                f"Number of categories is not matched. hub: {len(names)} != ultralytics: {len(yolo_names)}"
+            )
+
+        id_mapper: list[int] = [i for i in range(len(yolo_names))]
+
+        yolo_names_inv = {v: k for k, v in yolo_names.items()}
+        for i, name in enumerate(names):
+            id_mapper[i] = yolo_names_inv[name]
+
         preprocess = self.get_preprocess(self.task)
-        postprocess = self.get_postprocess(self.task)
+        postprocess = self.get_postprocess(self.task, id_mapper=id_mapper)
 
-        # get model
+        # wrap model
         model = ModelWrapper(
-            model=YOLO(self.best_ckpt_file).model.eval(),
+            model=model,
             preprocess=preprocess,
             postprocess=postprocess,
         )
 
         return model
```

### Comparing `waffle_hub-0.1.9/waffle_hub/hub/base_hub.py` & `waffle_hub-0.2.0/waffle_hub/hub/base_hub.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,37 +2,24 @@
 Hub
 ================
 Hub is a multi-backend compatible interface for model training, evaluation, inference, and export.
 
 .. note::
     Check out docstrings for more details.
 
-Advanced Usage using threads
-----------------
-
-.. code-block:: python
-    import time
-
-    result = hub.some_job(..., hold=False)
-
-    while (
-        not result.callback.is_finished()
-        and not result.callback.is_failed()
-    ):
-        time.sleep(1)
-        print(result.callback.get_progress())
-
 """
 import logging
 import threading
+import time
 import warnings
 from functools import cached_property
 from pathlib import Path
 from typing import Union
 
+import cpuinfo
 import cv2
 import torch
 import tqdm
 from waffle_utils.file import io
 from waffle_utils.utils import type_validator
 
 from waffle_hub import TaskType
@@ -516,15 +503,15 @@
             hubs/my_hub/weights/best_ckpt.pt
             >>> train_result.metrics
             [[{"tag": "epoch", "value": 1}, {"tag": "train/loss", "value": 0.1}, ...], ...]
 
         Returns:
             TrainResult: train result
         """
-        
+
         if self.artifact_dir.exists():
             raise FileExistsError(
                 f"{self.artifact_dir}\n"
                 "Train artifacts already exist. Remove artifact to re-train (hub.delete_artifact())."
             )
 
         def inner(callback: TrainCallback, result: TrainResult):
@@ -553,15 +540,20 @@
             pretrained_model=pretrained_model,
             device=device,
             workers=workers,
             seed=seed,
             verbose=verbose,
         )
 
-        callback = TrainCallback(cfg.epochs, self.get_metrics)
+        # overwrite train config with default config
+        for k, v in cfg.to_dict().items():
+            if v is None and k in self.DEFAULT_PARAMAS[self.task]:
+                setattr(cfg, k, self.DEFAULT_PARAMAS[self.task][k])
+
+        callback = TrainCallback(cfg.epochs + 1, self.get_metrics)
         result = TrainResult()
         result.callback = callback
 
         if hold:
             inner(callback, result)
         else:
             thread = threading.Thread(target=inner, args=(callback, result), daemon=True)
@@ -596,15 +588,15 @@
             cfg.image_size,
             letter_box=cfg.letter_box,
             set_name=cfg.set_name,
         ).get_dataloader(cfg.batch_size, cfg.workers)
 
         result_parser = get_parser(self.task)(**cfg.to_dict())
 
-        callback._total_steps = len(dataloader)
+        callback._total_steps = len(dataloader) + 1
 
         preds = []
         labels = []
         for i, (images, image_infos, annotations) in tqdm.tqdm(
             enumerate(dataloader, start=1), total=len(dataloader)
         ):
             result_batch = model(images.to(device))
@@ -720,15 +712,15 @@
             half=half,
             workers=workers,
             device="cpu" if device == "cpu" else f"cuda:{device}",
             draw=draw,
             dataset_root_dir=dataset_root_dir,
         )
 
-        callback = EvaluateCallback(0)
+        callback = EvaluateCallback(100)  # dummy step
         result = EvaluateResult()
         result.callback = callback
 
         if hold:
             inner(callback, result)
         else:
             thread = threading.Thread(target=inner, args=(callback, result), daemon=True)
@@ -756,15 +748,15 @@
         dataloader = ImageDataset(
             cfg.source, cfg.image_size, letter_box=cfg.letter_box
         ).get_dataloader(cfg.batch_size, cfg.workers)
 
         result_parser = get_parser(self.task)(**cfg.to_dict())
 
         results = []
-        callback._total_steps = len(dataloader)
+        callback._total_steps = len(dataloader) + 1
         for i, (images, image_infos) in tqdm.tqdm(
             enumerate(dataloader, start=1), total=len(dataloader)
         ):
             result_batch = model(images.to(device))
             result_batch = result_parser(result_batch, image_infos)
             for result, image_info in zip(result_batch, image_infos):
                 image_path = image_info.image_path
@@ -885,15 +877,15 @@
             iou_threshold=iou_threshold,
             half=half,
             workers=workers,
             device="cpu" if device == "cpu" else f"cuda:{device}",
             draw=draw,
         )
 
-        callback = InferenceCallback(0)
+        callback = InferenceCallback(100)  # dummy step
         result = InferenceResult()
         result.callback = callback
 
         if hold:
             inner(callback, result)
         else:
             thread = threading.Thread(target=inner, args=(callback, result), daemon=True)
@@ -913,25 +905,31 @@
     def on_export_start(self, cfg: ExportConfig):
         pass
 
     def exporting(self, cfg: ExportConfig, callback: ExportCallback) -> str:
         image_size = cfg.image_size
         image_size = [image_size, image_size] if isinstance(image_size, int) else image_size
 
-        model = self.get_model()
+        model = self.get_model().half() if cfg.half else self.get_model()
+        model = model.to(cfg.device)
 
         input_name = ["inputs"]
         if self.task == "object_detection":
             output_names = ["bbox", "conf", "class_id"]
         elif self.task == "classification":
             output_names = ["predictions"]
+        elif self.task == "instance_segmentation":
+            output_names = ["bbox", "conf", "class_id", "masks"]
         else:
             raise NotImplementedError(f"{self.task} does not support export yet.")
 
-        dummy_input = torch.randn(cfg.batch_size, 3, *image_size)
+        dummy_input = torch.randn(
+            cfg.batch_size, 3, *image_size, dtype=torch.float16 if cfg.half else torch.float32
+        )
+        dummy_input = dummy_input.to(cfg.device)
 
         torch.onnx.export(
             model,
             dummy_input,
             str(self.onnx_file),
             input_names=input_name,
             output_names=output_names,
@@ -946,22 +944,26 @@
         result.export_file = self.onnx_file
 
     def export(
         self,
         image_size: Union[int, list[int]] = None,
         batch_size: int = 16,
         opset_version: int = 11,
+        half: bool = False,
+        device: str = "0",
         hold: bool = True,
     ) -> ExportResult:
         """Export Model
 
         Args:
             image_size (Union[int, list[int]], optional): inference image size. None for same with train_config (recommended).
             batch_size (int, optional): dynamic batch size. Defaults to 16.
             opset_version (int, optional): onnx opset version. Defaults to 11.
+            half (bool, optional): half. Defaults to False.
+            device (str, optional): device. "cpu" or "gpu_id". Defaults to "0".
             hold (bool, optional): hold or not.
                 If True then it holds until task finished.
                 If False then return Inferece Callback and run in background. Defaults to True.
 
         Example:
             >>> export_result = hub.export(
                 image_size=640,
@@ -997,21 +999,101 @@
                 callback.set_failed()
                 raise e
 
         cfg = ExportConfig(
             image_size=image_size,
             batch_size=batch_size,
             opset_version=opset_version,
+            half=half,
+            device="cpu" if device == "cpu" else f"cuda:{device}",
         )
 
         callback = ExportCallback(1)
         result = ExportResult()
         result.callback = callback
 
         if hold:
             inner(callback, result)
         else:
             thread = threading.Thread(target=inner, args=(callback, result), daemon=True)
             callback.register_thread(thread)
             callback.start()
 
         return result
+
+    def benchmark(
+        self,
+        image_size: Union[int, list[int]] = None,
+        batch_size: int = 16,
+        device: str = "0",
+        half: bool = False,
+        trial: int = 100,
+    ) -> dict:
+        """Benchmark Model
+
+        Args:
+            image_size (Union[int, list[int]], optional): inference image size. None for same with train_config (recommended).
+            batch_size (int, optional): dynamic batch size. Defaults to 16.
+            device (str, optional): device. "cpu" or "gpu_id". Defaults to "0".
+            half (bool, optional): half. Defaults to False.
+            trial (int, optional): number of trials. Defaults to 100.
+
+        Example:
+            >>> hub.benchmark(
+                    image_size=640,
+                    batch_size=16,
+                    device="0",
+                    half=False,
+                    trial=100,
+                )
+            {
+                "inference_time": 0.123,
+                "fps": 123.123,
+                "image_size": [640, 640],
+                "batch_size": 16,
+                "device": "0",
+                "cpu_name": "Intel(R) Core(TM) i7-8700 CPU @ 3.20GHz",
+                "gpu_name": "GeForce GTX 1080 Ti",
+            }
+
+        Returns:
+            dict: benchmark result
+        """
+        self.check_train_sanity()
+
+        if half and (not torch.cuda.is_available() or device == "cpu"):
+            raise RuntimeError("half is not supported in cpu")
+
+        image_size = image_size or self.get_train_config().image_size
+        image_size = [image_size, image_size] if isinstance(image_size, int) else image_size
+
+        device = "cpu" if device == "cpu" else f"cuda:{device}"
+
+        model = self.get_model()
+        model = model.to(device) if not half else model.half().to(device)
+
+        dummy_input = torch.randn(
+            batch_size, 3, *image_size, dtype=torch.float32 if not half else torch.float16
+        )
+        dummy_input = dummy_input.to(device)
+
+        model.eval()
+        with torch.no_grad():
+            start = time.time()
+            for _ in tqdm.tqdm(range(trial)):
+                model(dummy_input)
+            end = time.time()
+            inference_time = end - start
+
+        del model
+
+        return {
+            "inference_time": inference_time,
+            # image throughput per second
+            "fps": trial * batch_size / inference_time,
+            "image_size": image_size,
+            "batch_size": batch_size,
+            "precision": "fp16" if half else "fp32",
+            "device": device,
+            "cpu_name": cpuinfo.get_cpu_info()["brand_raw"],
+            "gpu_name": torch.cuda.get_device_name(0) if device != "cpu" else None,
+        }
```

### Comparing `waffle_hub-0.1.9/waffle_hub/hub/model/wrapper.py` & `waffle_hub-0.2.0/waffle_hub/hub/model/wrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,19 +6,22 @@
 
 Returns:
     _type_: _description_
 """
 
 from typing import Union
 
+import numpy as np
 import torch
+import torch.nn.functional as F
 from torchvision.ops import batched_nms
 
 from waffle_hub.schema.data import ImageInfo
 from waffle_hub.schema.fields import Annotation
+from waffle_hub.utils.conversion import convert_mask_to_polygon
 
 
 class PreprocessFunction:
     pass
 
 
 class PostprocessFunction:
@@ -30,56 +33,40 @@
 
 
 class ClassificationResultParser(ResultParser):
     def __init__(self, *args, **kwargs):
         pass
 
     def __call__(
-        self,
-        results: list[torch.Tensor],
-        image_infos: list[ImageInfo] = None,
-        *args,
-        **kwargs
+        self, results: list[torch.Tensor], image_infos: list[ImageInfo] = None, *args, **kwargs
     ) -> list[Annotation]:
         parseds = []
 
         results = results[0]  # TODO: multi label
         scores, class_ids = results.cpu().topk(results.shape[1], dim=-1)
-        results = torch.cat(
-            [class_ids.unsqueeze(-1), scores.unsqueeze(-1)], dim=-1
-        )
+        results = torch.cat([class_ids.unsqueeze(-1), scores.unsqueeze(-1)], dim=-1)
         for result in results:
             parsed = []
             for class_id, score in result:
                 parsed.append(
-                    Annotation.classification(
-                        category_id=int(class_id) + 1, score=float(score)
-                    )
+                    Annotation.classification(category_id=int(class_id) + 1, score=float(score))
                 )
             parseds.append(parsed)
         return parseds
 
 
 class ObjectDetectionResultParser(ResultParser):
     def __init__(
-        self,
-        confidence_threshold: float = 0.25,
-        iou_threshold: float = 0.5,
-        *args,
-        **kwargs
+        self, confidence_threshold: float = 0.25, iou_threshold: float = 0.5, *args, **kwargs
     ):
         self.confidence_threshold = confidence_threshold
         self.iou_threshold = iou_threshold
 
     def __call__(
-        self,
-        results: list[torch.Tensor],
-        image_infos: list[ImageInfo],
-        *args,
-        **kwargs
+        self, results: list[torch.Tensor], image_infos: list[ImageInfo], *args, **kwargs
     ) -> list[Annotation]:
         parseds = []
 
         bboxes_batch, confs_batch, class_ids_batch = results
         for bboxes, confs, class_ids, image_info in zip(
             bboxes_batch, confs_batch, class_ids_batch, image_infos
         ):
@@ -99,17 +86,15 @@
 
             W, H = image_info.input_shape
             left_pad, top_pad = image_info.pad
             ori_w, ori_h = image_info.ori_shape
             new_w, new_h = image_info.new_shape
 
             parsed = []
-            for (x1, y1, x2, y2), conf, class_id in zip(
-                bboxes, confs, class_ids
-            ):
+            for (x1, y1, x2, y2), conf, class_id in zip(bboxes, confs, class_ids):
 
                 x1 = max(float((x1 * W - left_pad) / new_w * ori_w), 0)
                 y1 = max(float((y1 * H - top_pad) / new_h * ori_h), 0)
                 x2 = min(float((x2 * W - left_pad) / new_w * ori_w), ori_w)
                 y2 = min(float((y2 * H - top_pad) / new_h * ori_h), ori_h)
 
                 parsed.append(
@@ -120,19 +105,102 @@
                         score=float(conf),
                     )
                 )
             parseds.append(parsed)
         return parseds
 
 
+class InstanceSegmentationResultParser(ObjectDetectionResultParser):
+    def __init__(
+        self, confidence_threshold: float = 0.25, iou_threshold: float = 0.5, *args, **kwargs
+    ):
+        self.confidence_threshold = confidence_threshold
+        self.iou_threshold = iou_threshold
+        super().__init__(confidence_threshold, iou_threshold, *args, **kwargs)
+
+    def __call__(
+        self, results: list[torch.Tensor], image_infos: list[ImageInfo], *args, **kwargs
+    ) -> list[Annotation]:
+        parseds = []
+        bboxes_batch, confs_batch, class_ids_batch, masks_batch = results
+        for bboxes, confs, class_ids, masks, image_info in zip(
+            bboxes_batch,
+            confs_batch,
+            class_ids_batch,
+            masks_batch,
+            image_infos,
+        ):
+
+            mask = confs > self.confidence_threshold
+
+            bboxes, confs, class_ids, masks = (
+                bboxes[mask],
+                confs[mask],
+                class_ids[mask],
+                masks[mask],
+            )
+            idxs = batched_nms(bboxes, confs, class_ids, self.iou_threshold)
+
+            bboxes = bboxes[idxs, :].cpu()
+            confs = confs[idxs].cpu()
+            class_ids = class_ids[idxs].cpu()
+
+            masks = masks[idxs, :]
+            masks = (
+                F.interpolate(
+                    input=masks.gt_(0.5).unsqueeze(1),
+                    size=image_info.ori_shape,
+                    mode="bilinear",
+                    align_corners=False,
+                )
+                .cpu()
+                .squeeze(1)
+            )
+
+            W, H = image_info.input_shape
+            left_pad, top_pad = image_info.pad
+            ori_w, ori_h = image_info.ori_shape
+            new_w, new_h = image_info.new_shape
+
+            parsed = []
+            for (x1, y1, x2, y2), conf, class_id, mask in zip(bboxes, confs, class_ids, masks):
+
+                x1 = max(float((x1 * W - left_pad) / new_w * ori_w), 0)
+                y1 = max(float((y1 * H - top_pad) / new_h * ori_h), 0)
+                x2 = min(float((x2 * W - left_pad) / new_w * ori_w), ori_w)
+                y2 = min(float((y2 * H - top_pad) / new_h * ori_h), ori_h)
+
+                # clean non roi area
+                mask[:, : round(x1)] = 0
+                mask[:, round(x2) :] = 0
+                mask[: round(y1), :] = 0
+                mask[round(y2) :, :] = 0
+
+                segment = convert_mask_to_polygon(mask.numpy().astype(np.uint8))
+
+                parsed.append(
+                    Annotation.instance_segmentation(
+                        category_id=int(class_id) + 1,
+                        bbox=[x1, y1, x2 - x1, y2 - y1],
+                        area=float((x2 - x1) * (y2 - y1)),
+                        score=float(conf),
+                        segmentation=segment,
+                    )
+                )
+            parseds.append(parsed)
+        return parseds
+
+
 def get_parser(task: str):
     if task == "classification":
         return ClassificationResultParser
     elif task == "object_detection":
         return ObjectDetectionResultParser
+    elif task == "instance_segmentation":
+        return InstanceSegmentationResultParser
 
 
 class ModelWrapper(torch.nn.Module):
     def __init__(
         self,
         model: torch.nn.Module,
         preprocess: PreprocessFunction,
@@ -163,15 +231,20 @@
                 Detection:
                     [
                         [batch, bbox_num, 4(x1, y1, x2, y2)],  # bounding box
                         [batch, bbox_num],  # confidence
                         [batch, bbox_num],  # class id
                     ]
                 Segmentation:
-                    # TODO: segmentation support
+                    [
+                        [batch, bbox_num, 4(x1, y1, x2, y2)],  # bounding box
+                        [batch, bbox_num],  # confidence
+                        [batch, bbox_num],  # class id
+                        [batch, mask(H, W)] # warning: mask size and image size are not same
+                    ]
         """
         super().__init__()
         self.model = model
         self.preprocess = preprocess
         self.postprocess = postprocess
 
     def forward(self, x):
```

### Comparing `waffle_hub-0.1.9/waffle_hub/run.py` & `waffle_hub-0.2.0/waffle_hub/run.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.9/waffle_hub/schema/configs.py` & `waffle_hub-0.2.0/waffle_hub/schema/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,7 +64,9 @@
 @dataclass
 class ExportConfig(BaseSchema):
     image_size: Union[int, list[int]] = None
     batch_size: int = None
     input_name: list[str] = None
     output_name: list[str] = None
     opset_version: int = None
+    half: bool = False
+    device: str = None
```

### Comparing `waffle_hub-0.1.9/waffle_hub/schema/data.py` & `waffle_hub-0.2.0/waffle_hub/schema/data.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.9/waffle_hub/schema/fields/annotation.py` & `waffle_hub-0.2.0/waffle_hub/schema/fields/annotation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from typing import Union
 
 from waffle_utils.utils import type_validator
 
 from waffle_hub import TaskType
+from waffle_hub.utils.conversion import convert_rle_to_polygon
 
 from .base_field import BaseField
 
 
 class Annotation(BaseField):
     def __init__(
         self,
         # required
         annotation_id: int,
         image_id: int,
         # optional
         category_id: int = None,
         bbox: list[float] = None,
-        segmentation: list[float] = None,
+        segmentation: list[list[float]] = None,
         area: float = None,
         keypoints: list[float] = None,
         num_keypoints: int = None,
         caption: str = None,
         value: float = None,
         #
         iscrowd: int = None,
@@ -37,15 +38,15 @@
         self.area = area
         self.keypoints = keypoints
         self.num_keypoints = num_keypoints
         self.caption = caption
         self.value = value
         self.iscrowd = iscrowd
         self.score = score
-        
+
         self.task = task
 
     # properties
     @property
     def annotation_id(self):
         return self.__annotation_id
 
@@ -90,20 +91,22 @@
         self.__bbox = v
 
     @property
     def segmentation(self):
         return self.__segmentation
 
     @segmentation.setter
-    @type_validator(list)
+    # XXX: dict->rle, list->polygon
     def segmentation(self, v):
-        if v and len(v) % 2 != 0 and len(v) < 6:
-            raise ValueError(
-                "the length of segmentation should be at least 6 and divisible by 2."
-            )
+        if isinstance(v, dict):
+            v: list = convert_rle_to_polygon(v)
+        if v:
+            for segment in v:
+                if len(segment) % 2 != 0:
+                    raise ValueError("the length of segmentation should be divisible by 2.")
         self.__segmentation = v
 
     @property
     def area(self):
         return self.__area
 
     @area.setter
@@ -115,17 +118,15 @@
     def keypoints(self):
         return self.__keypoints
 
     @keypoints.setter
     @type_validator(list)
     def keypoints(self, v):
         if v and len(v) % 3 != 0 and len(v) < 2:
-            raise ValueError(
-                "the length of keypoints should be at least 2 and divisible by 3."
-            )
+            raise ValueError("the length of keypoints should be at least 2 and divisible by 3.")
         self.__keypoints = v
 
     @property
     def num_keypoints(self):
         return self.__num_keypoints
 
     @num_keypoints.setter
@@ -172,47 +173,44 @@
     @property
     def task(self):
         return self.__task
 
     @task.setter
     def task(self, v):
         if v is not None and v not in TaskType:
-            raise ValueError(
-                f"Invalid task type: {v}"
-                f"Available task types: {list(TaskType)}"
-            )
+            raise ValueError(f"Invalid task type: {v}" f"Available task types: {list(TaskType)}")
         self.__task = str(v).upper()
 
     # factories
     @classmethod
     def new(
         cls,
         annotation_id: int = None,
         image_id: int = None,
         category_id: int = None,
         bbox: list[float] = None,
-        segmentation: list[float] = None,
+        segmentation: list[list[float]] = None,
         area: int = None,
         keypoints: list[float] = None,
         num_keypoints: int = None,
         caption: str = None,
         value: float = None,
         iscrowd: int = None,
         score: float = None,
         task: Union[str, TaskType] = None,
-        **kwargs
+        **kwargs,
     ) -> "Annotation":
         """Annotation Format
 
         Args:
             annotation_id (int): annotaion id. natural number.
             image_id (int): image id. natural number.
             category_id (int): category id. natural number.
             bbox (list[float]): [x1, y1, w, h].
-            segmentation (list[float]): [x1, y1, x2, y2, x3, y3, ...].
+            segmentation (list[list[float]]): [[[x1, y1, x2, y2, x3, y3, ...], [...]].
             area (int): bbox area.
             keypoints (list[float]):
                 [x1, y1, v1(visible flag), x2, y2, v2(visible flag), ...].
                 visible flag is one of [0(Not labeled), 1(Labeled but not visible), 2(labeled and visible)]
             num_keypoints: number of labeled keypoints
             caption (str): string.
             value (float): regression value.
@@ -232,50 +230,56 @@
             area=area,
             keypoints=keypoints,
             num_keypoints=num_keypoints,
             caption=caption,
             value=value,
             iscrowd=iscrowd,
             score=score,
-            task=task
+            task=task,
         )
 
     @classmethod
     def classification(
-        cls, 
-        annotation_id: int = None, 
-        image_id: int = None, 
-        category_id: int = None, 
-        score: float = None, 
-        **kwargs
+        cls,
+        annotation_id: int = None,
+        image_id: int = None,
+        category_id: int = None,
+        score: float = None,
+        **kwargs,
     ) -> "Annotation":
         """Classification Annotation Format
 
         Args:
             annotation_id (int): annotaion id. natural number.
             image_id (int): image id. natural number.
             category_id (int): category id. natural number.
             score (float, optional): prediction score. Default to None.
 
         Returns:
             Annotation: annotation class
         """
-        return cls(annotation_id, image_id, category_id=category_id, score=score, task=TaskType.CLASSIFICATION)
+        return cls(
+            annotation_id,
+            image_id,
+            category_id=category_id,
+            score=score,
+            task=TaskType.CLASSIFICATION,
+        )
 
     @classmethod
     def object_detection(
         cls,
         annotation_id: int = None,
         image_id: int = None,
         category_id: int = None,
         bbox: list[float] = None,
         area: int = None,
         iscrowd: int = 0,
         score: float = None,
-        **kwargs
+        **kwargs,
     ) -> "Annotation":
         """Object Detection Annotation Format
 
         Args:
             annotation_id (int): annotaion id. natural number.
             image_id (int): image id. natural number.
             category_id (int): category id. natural number.
@@ -291,38 +295,78 @@
             annotation_id,
             image_id,
             category_id=category_id,
             bbox=bbox,
             area=area,
             iscrowd=iscrowd,
             score=score,
-            task=TaskType.OBJECT_DETECTION
+            task=TaskType.OBJECT_DETECTION,
         )
 
     @classmethod
-    def segmentation(
+    def semantic_segmentation(
         cls,
         annotation_id: int = None,
         image_id: int = None,
         category_id: int = None,
         bbox: list[float] = None,
-        segmentation: list[float] = None,
+        segmentation: list[list[float]] = None,
         area: int = None,
         iscrowd: int = 0,
         score: float = None,
-        **kwargs
+        **kwargs,
     ) -> "Annotation":
         """Segmentation Annotation Format
 
         Args:
             annotation_id (int): annotaion id. natural number.
             image_id (int): image id. natural number.
             category_id (int): category id. natural number.
             bbox (list[float]): [x1, y1, w, h].
-            segmentation (list[float]): [x1, y1, x2, y2, x3, y3, ...].
+            segmentation (list[list[float]]): [[x1, y1, x2, y2, x3, y3, ...], [polygon]].
+            area (int): segmentation segmentation area.
+            iscrowd (int, optional): is crowd or not. Default to 0.
+            score (float, optional): prediction score. Default to None.
+
+        Returns:
+            Annotation: annotation class
+        """
+        return cls(
+            annotation_id,
+            image_id,
+            category_id=category_id,
+            bbox=bbox,
+            segmentation=segmentation,
+            area=area,
+            iscrowd=iscrowd,
+            score=score,
+            task=TaskType.SEMANTIC_SEGMENTATION,
+        )
+
+    @classmethod
+    def instance_segmentation(
+        cls,
+        annotation_id: int = None,
+        image_id: int = None,
+        category_id: int = None,
+        bbox: list[float] = None,
+        segmentation: list[list[float]] = None,
+        area: int = None,
+        iscrowd: int = 0,
+        score: float = None,
+        **kwargs,
+    ) -> "Annotation":
+        """Instance Annotation Format
+
+        Args:
+            annotation_id (int): annotaion id. natural number.
+            image_id (int): image id. natural number.
+            category_id (int): category id. natural number.
+            bbox (list[float]): [x1, y1, w, h].
+            segmentation (list[list[float]]): [[x1, y1, x2, y2, x3, y3, ...], [polygon]].
             area (int): segmentation segmentation area.
             iscrowd (int, optional): is crowd or not. Default to 0.
             score (float, optional): prediction score. Default to None.
 
         Returns:
             Annotation: annotation class
         """
@@ -331,45 +375,45 @@
             image_id,
             category_id=category_id,
             bbox=bbox,
             segmentation=segmentation,
             area=area,
             iscrowd=iscrowd,
             score=score,
-            task=TaskType.SEGMENTATION
+            task=TaskType.INSTANCE_SEGMENTATION,
         )
 
     @classmethod
     def keypoint_detection(
         cls,
         annotation_id: int = None,
         image_id: int = None,
         category_id: int = None,
         bbox: list[float] = None,
         keypoints: list[float] = None,
         num_keypoints: int = None,
         area: int = None,
-        segmentation: list[float] = None,
+        segmentation: list[list[float]] = None,
         iscrowd: int = 0,
         score: list[float] = None,
-        **kwargs
+        **kwargs,
     ) -> "Annotation":
         """Keypoint Detection Annotation Format
 
         Args:
             annotation_id (int): annotaion id. natural number.
             image_id (int): image id. natural number.
             category_id (int): category id. natural number.
             bbox (list[float]): [x1, y1, w, h].
             keypoints (list[float]):
                 [x1, y1, v1(visible flag), x2, y2, v2(visible flag), ...].
                 visible flag is one of [0(Not labeled), 1(Labeled but not visible), 2(labeled and visible)]
             num_keypoints: number of labeled keypoints
             area (int): segmentation segmentation or bbox area.
-            segmentation (list[float], optional): [x1, y1, x2, y2, x3, y3, ...].
+            segmentation (list[list[float]], optional): [[x1, y1, x2, y2, x3, y3, ...], [polygon]].
             iscrowd (int, optional): is crowd or not. Default to 0.
             score (list[float], optional): prediction scores. Default to None.
 
         Returns:
             Annotation: annotation class
         """
         return cls(
@@ -379,24 +423,20 @@
             bbox=bbox,
             keypoints=keypoints,
             num_keypoints=num_keypoints,
             segmentation=segmentation,
             area=area,
             iscrowd=iscrowd,
             score=score,
-            task=TaskType.KEYPOINT_DETECTION
+            task=TaskType.KEYPOINT_DETECTION,
         )
 
     @classmethod
     def regression(
-        cls, 
-        annotation_id: int = None, 
-        image_id: int = None, 
-        value: float = None, 
-        **kwargs
+        cls, annotation_id: int = None, image_id: int = None, value: float = None, **kwargs
     ) -> "Annotation":
         """Regression Annotation Format
 
         Args:
             annotation_id (int): annotaion id. natural number.
             image_id (int): image id. natural number.
             category_id (int): category id. natural number.
@@ -405,34 +445,36 @@
         Returns:
             Annotation: annotation class
         """
         return cls(annotation_id, image_id, value=value, task=TaskType.REGRESSION)
 
     @classmethod
     def text_recognition(
-        cls, 
-        annotation_id: int = None, 
-        image_id: int = None, 
-        caption: str = None, 
-        score: float = None, 
-        **kwargs
+        cls,
+        annotation_id: int = None,
+        image_id: int = None,
+        caption: str = None,
+        score: float = None,
+        **kwargs,
     ) -> "Annotation":
         """Text Recognition Annotation Format
 
         Args:
             annotation_id (int): annotaion id. natural number.
             image_id (int): image id. natural number.
             category_id (int): category id. natural number.
             caption (str): string.
             score (float, optional): prediction score. Default to None.
 
         Returns:
             Annotation: annotation class
         """
-        return cls(annotation_id, image_id, caption=caption, score=score, task=TaskType.TEXT_RECOGNITION)
+        return cls(
+            annotation_id, image_id, caption=caption, score=score, task=TaskType.TEXT_RECOGNITION
+        )
 
     def to_dict(self) -> dict:
         """Get Dictionary of Annotation Data
 
         Returns:
             dict: annotation dictionary.
         """
```

### Comparing `waffle_hub-0.1.9/waffle_hub/schema/fields/base_field.py` & `waffle_hub-0.2.0/waffle_hub/schema/fields/base_field.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from abc import ABC, abstractmethod
 
 from waffle_utils.file import io
 
 from waffle_hub import TaskType
 
+
 class BaseField(ABC):
     def __init__(self):
         pass
 
     @abstractmethod
     def to_dict(self):
         pass
@@ -15,21 +16,23 @@
     @classmethod
     @abstractmethod
     def new(cls):
         pass
 
     @classmethod
     def from_dict(cls, d: dict, task: str = None) -> "BaseField":
-        
+
         if task == TaskType.CLASSIFICATION:
             return cls.classification(**d)
         elif task == TaskType.OBJECT_DETECTION:
             return cls.object_detection(**d)
-        elif task == TaskType.SEGMENTATION:
-            return cls.segmentation(**d)
+        elif task == TaskType.SEMANTIC_SEGMENTATION:
+            return cls.semantic_segmentation(**d)
+        elif task == TaskType.INSTANCE_SEGMENTATION:
+            return cls.instance_segmentation(**d)
         elif task == TaskType.KEYPOINT_DETECTION:
             return cls.keypoint_detection(**d)
         elif task == TaskType.TEXT_RECOGNITION:
             return cls.text_recognition(**d)
         elif task == TaskType.REGRESSION:
             return cls.regression(**d)
         else:
```

### Comparing `waffle_hub-0.1.9/waffle_hub/schema/fields/category.py` & `waffle_hub-0.2.0/waffle_hub/schema/fields/category.py`

 * *Files 11% similar despite different names*

```diff
@@ -79,18 +79,15 @@
     @property
     def task(self):
         return self.__task
 
     @task.setter
     def task(self, v):
         if v is not None and v not in TaskType:
-            raise ValueError(
-                f"Invalid task type: {v}"
-                f"Available task types: {list(TaskType)}"
-            )
+            raise ValueError(f"Invalid task type: {v}" f"Available task types: {list(TaskType)}")
         self.__task = str(v).upper()
 
     # factories
     @classmethod
     def new(
         cls,
         category_id: int,
@@ -121,19 +118,15 @@
             keypoints=keypoints,
             skeleton=skeleton,
             task=task,
         )
 
     @classmethod
     def classification(
-        cls, 
-        category_id: int, 
-        name: str, 
-        supercategory: str = None, 
-        **kwargs
+        cls, category_id: int, name: str, supercategory: str = None, **kwargs
     ) -> "Category":
         """Classification Category Format
 
         Args:
             category_id (int): category id. natural number.
             name (str): category name.
             supercategory (str): supercategory name.
@@ -143,23 +136,18 @@
         """
         return cls(
             category_id=category_id,
             name=name,
             supercategory=supercategory,
             task=TaskType.CLASSIFICATION,
         )
-            
 
     @classmethod
     def object_detection(
-        cls, 
-        category_id: int, 
-        name: str, 
-        supercategory: str = None, 
-        **kwargs
+        cls, category_id: int, name: str, supercategory: str = None, **kwargs
     ) -> "Category":
         """Object Detection Category Format
 
         Args:
             category_id (int): category id. natural number.
             name (str): category name.
             supercategory (str): supercategory name.
@@ -171,20 +159,16 @@
             category_id=category_id,
             name=name,
             supercategory=supercategory,
             task=TaskType.OBJECT_DETECTION,
         )
 
     @classmethod
-    def segmentation(
-        cls, 
-        category_id: int, 
-        name: str, 
-        supercategory: str = None, 
-        **kwargs
+    def semantic_segmentation(
+        cls, category_id: int, name: str, supercategory: str = None, **kwargs
     ) -> "Category":
         """Segmentation Category Format
 
         Args:
             category_id (int): category id. natural number.
             name (str): category name.
             supercategory (str): supercategory name.
@@ -192,15 +176,36 @@
         Returns:
             Category: category class
         """
         return cls(
             category_id=category_id,
             name=name,
             supercategory=supercategory,
-            task=TaskType.SEGMENTATION,
+            task=TaskType.SEMANTIC_SEGMENTATION,
+        )
+
+    @classmethod
+    def instance_segmentation(
+        cls, category_id: int, name: str, supercategory: str = None, **kwargs
+    ) -> "Category":
+        """Instance Category Format
+
+        Args:
+            category_id (int): category id. natural number.
+            name (str): category name.
+            supercategory (str): supercategory name.
+
+        Returns:
+            Category: category class
+        """
+        return cls(
+            category_id=category_id,
+            name=name,
+            supercategory=supercategory,
+            task=TaskType.INSTANCE_SEGMENTATION,
         )
 
     @classmethod
     def keypoint_detection(
         cls,
         category_id: int,
         name: str,
@@ -228,19 +233,15 @@
             keypoints=keypoints,
             skeleton=skeleton,
             task=TaskType.KEYPOINT_DETECTION,
         )
 
     @classmethod
     def text_recognition(
-        cls, 
-        category_id: int, 
-        name: str, 
-        supercategory: str = None, 
-        **kwargs
+        cls, category_id: int, name: str, supercategory: str = None, **kwargs
     ) -> "Category":
         """Text Recognition Category Format
 
         Args:
             category_id (int): category id. natural number.
             name (str): category name.
             supercategory (str): supercategory name.
@@ -269,8 +270,8 @@
         }
 
         if self.keypoints is not None:
             cat["keypoints"] = self.keypoints
         if self.skeleton is not None:
             cat["skeleton"] = self.skeleton
 
-        return cat
+        return cat
```

### Comparing `waffle_hub-0.1.9/waffle_hub/schema/fields/image.py` & `waffle_hub-0.2.0/waffle_hub/schema/fields/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     def new(
         cls,
         image_id: int,
         file_name: str,
         width: int,
         height: int,
         date_captured: str = None,
+        **kwargs,
     ) -> "Image":
         """Image Format
 
         Args:
             image_id (int): image id. natural number.
             file_name (str): file name. relative file path.
             width (int): image width.
```

### Comparing `waffle_hub-0.1.9/waffle_hub/utils/callback.py` & `waffle_hub-0.2.0/waffle_hub/utils/callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
             self._progress = step / self._total_steps
         else:
             self._progress = step / self._total_steps
 
     def force_finish(self):
         """Force the task to end."""
         self._finished = True
+        self._progress = 1.0
 
     def register_thread(self, thread: threading.Thread):
         """Register the thread that is running the task."""
         self._thread = thread
 
     def start(self):
         """Start the thread that is running the task."""
@@ -107,20 +108,23 @@
     def __init__(self, total_steps: int, get_metric_func):
         super().__init__(total_steps)
 
         self._get_metric_func = get_metric_func
 
     def get_progress(self) -> float:
         """Get the progress of the task. (0 ~ 1)"""
-        metrics = self._get_metric_func()
-        if len(metrics) == 0:
-            return 0
-        self.update(len(metrics))
-        self._progress = len(metrics) / self._total_steps
-        return self._progress
+        if not self._finished:
+            metrics = self._get_metric_func()
+            if len(metrics) == 0:
+                return 0
+            self.update(len(metrics))
+            self._progress = len(metrics) / self._total_steps
+            return self._progress
+        else:
+            return 1.0
 
 
 class EvaluateCallback(ThreadProgressCallback):
     def __init__(self, total_steps: int):
         super().__init__(total_steps)
```

### Comparing `waffle_hub-0.1.9/waffle_hub/utils/data.py` & `waffle_hub-0.2.0/waffle_hub/utils/data.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.9/waffle_hub/utils/draw.py` & `waffle_hub-0.2.0/waffle_hub/utils/draw.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     image = cv2.putText(
         image,
         f"{names[category_id-1]}" + (f": {score:.2f}" if score else ""),
         (loc_x, loc_y),
         FONT_FACE,
         FONT_SCALE,
-        colors[category_id-1],
+        colors[category_id - 1],
         FONT_WEIGHT,
     )
     return image
 
 
 def draw_object_detection(
     image: np.ndarray,
@@ -46,60 +46,86 @@
 ):
     x1, y1, w, h = annotation.bbox
     x2 = x1 + w
     y2 = y1 + h
 
     category_id: int = annotation.category_id
     score: float = annotation.score
-    
+
     image = cv2.putText(
         image,
         f"{names[category_id-1]}" + (f": {score:.2f}" if score else ""),
         (int(x1), int(y1) - 3),
         FONT_FACE,
         FONT_SCALE,
-        colors[category_id-1],
+        colors[category_id - 1],
         FONT_WEIGHT,
     )
     image = cv2.rectangle(
         image,
         (int(x1), int(y1)),
         (int(x2), int(y2)),
-        colors[category_id-1],
+        colors[category_id - 1],
         THICKNESS,
     )
     return image
 
 
+def draw_instance_segmentation(
+    image: np.ndarray,
+    annotation: Annotation,
+    names: list[str],
+    score: float = None,
+):
+    image = draw_object_detection(image, annotation, names, score)
+    segments: list = annotation.segmentation
+
+    if len(segments) == 0:
+        return image
+
+    alpha = np.zeros_like(image)
+    for segment in segments:
+        segment = np.array(segment).reshape(-1, 2).astype(int)
+        alpha = cv2.fillPoly(
+            alpha,
+            [segment],
+            colors[annotation.category_id - 1],
+        )
+    mask = alpha > 0
+    image[mask] = cv2.addWeighted(alpha, 0.3, image, 0.7, 0)[mask]
+
+    return image
+
+
 def draw_results(
     image: Union[np.ndarray, str],
     results: list[Annotation],
     names: list[str],
 ):
 
     if isinstance(image, str):
         image = cv2.imread(image)
 
-    classification_results = [
-        result
-        for result in results
-        if result.task == TaskType.CLASSIFICATION
-    ]
+    classification_results = [result for result in results if result.task == TaskType.CLASSIFICATION]
     object_detection_results = [
-        result
-        for result in results
-        if result.task == TaskType.OBJECT_DETECTION
+        result for result in results if result.task == TaskType.OBJECT_DETECTION
+    ]
+    instance_segmentation_results = [
+        result for result in results if result.task == TaskType.INSTANCE_SEGMENTATION
     ]
 
     for i, result in enumerate(classification_results, start=1):
         image = draw_classification(
             image,
             result,
             names=names,
             loc_x=10,
             loc_y=30 * i,
         )
 
     for i, result in enumerate(object_detection_results, start=1):
         image = draw_object_detection(image, result, names=names)
 
+    for i, result in enumerate(instance_segmentation_results, start=1):
+        image = draw_instance_segmentation(image, result, names=names)
+
     return image
```

### Comparing `waffle_hub-0.1.9/waffle_hub/utils/evaluate.py` & `waffle_hub-0.2.0/waffle_hub/utils/evaluate.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 import torch
 from torchmetrics.classification import Accuracy
 from torchmetrics.detection import mean_ap
 
 from waffle_hub import TaskType
 from waffle_hub.schema.evaluate import (
     ClassificationMetric,
+    InstanceSegmentationMetric,
     ObjectDetectionMetric,
 )
 from waffle_hub.schema.fields import Annotation
 
 
-def convert_to_torchmetric_format(
-    total: list[Annotation], task: TaskType, prediction: bool = False
-):
+def convert_to_torchmetric_format(total: list[Annotation], task: TaskType, prediction: bool = False):
 
     datas = []
     for annotations in total:
 
         if task == TaskType.CLASSIFICATION:  # single attribute
             datas.append(annotations[0].category_id - 1)
 
@@ -34,21 +33,35 @@
                 data["boxes"].append(annotation.bbox)
                 data["labels"].append(annotation.category_id - 1)
                 if prediction:
                     data["scores"].append(annotation.score)
 
             datas.append(data)
 
+        elif task == TaskType.INSTANCE_SEGMENTATION:
+            data = {
+                "boxes": [],
+                "labels": [],
+            }
+            if prediction:
+                data["scores"] = []
+
+            for annotation in annotations:
+                data["boxes"].append(annotation.bbox)
+                data["labels"].append(annotation.category_id - 1)
+                if prediction:
+                    data["scores"].append(annotation.score)
+
+            datas.append(data)
+
         else:
             raise NotImplementedError
 
     if isinstance(datas[0], dict):
-        datas = [
-            {k: torch.tensor(v) for k, v in data.items()} for data in datas
-        ]
+        datas = [{k: torch.tensor(v) for k, v in data.items()} for data in datas]
     elif isinstance(datas[0], int):
         datas = torch.tensor(datas)
     else:
         raise NotImplementedError
 
     return datas
 
@@ -72,28 +85,40 @@
         class_metrics=True,
         num_classes=num_classes,
     )(preds, labels)
 
     return ObjectDetectionMetric(float(map_dict["map"]))
 
 
+def evaluate_segmentation(
+    preds: list[Annotation], labels: list[Annotation], num_classes: int
+) -> InstanceSegmentationMetric:
+
+    map_dict = mean_ap.MeanAveragePrecision(
+        box_format="xywh",
+        iou_type="bbox",
+        class_metrics=True,
+        num_classes=num_classes,
+    )(preds, labels)
+
+    return InstanceSegmentationMetric(float(map_dict["map"]))
+
+
 def evaluate_function(
     preds: list[Annotation],
     labels: list[Annotation],
     task: str,
     num_classes: int = None,
     *args,
     **kwargs
-) -> Union[ClassificationMetric, ObjectDetectionMetric]:
+) -> Union[ClassificationMetric, ObjectDetectionMetric, InstanceSegmentationMetric]:
     preds = convert_to_torchmetric_format(preds, task, prediction=True)
     labels = convert_to_torchmetric_format(labels, task)
 
     if task == TaskType.CLASSIFICATION:
-        return evaluate_classification(
-            preds, labels, num_classes, *args, **kwargs
-        )
+        return evaluate_classification(preds, labels, num_classes, *args, **kwargs)
     elif task == TaskType.OBJECT_DETECTION:
-        return evaluate_object_detection(
-            preds, labels, num_classes, *args, **kwargs
-        )
+        return evaluate_object_detection(preds, labels, num_classes, *args, **kwargs)
+    elif task == TaskType.INSTANCE_SEGMENTATION:
+        return evaluate_segmentation(preds, labels, num_classes, *args, **kwargs)
     else:
         raise NotImplementedError
```

### Comparing `waffle_hub-0.1.9/waffle_hub.egg-info/PKG-INFO` & `waffle_hub-0.2.0/waffle_hub.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle-hub
-Version: 0.1.9
+Version: 0.2.0
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle-hub Version: 0.1.9 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle-hub Version: 0.2.0 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `waffle_hub-0.1.9/waffle_hub.egg-info/SOURCES.txt` & `waffle_hub-0.2.0/waffle_hub.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,10 +47,11 @@
 waffle_hub/schema/fields/__init__.py
 waffle_hub/schema/fields/annotation.py
 waffle_hub/schema/fields/base_field.py
 waffle_hub/schema/fields/category.py
 waffle_hub/schema/fields/image.py
 waffle_hub/utils/__init__.py
 waffle_hub/utils/callback.py
+waffle_hub/utils/conversion.py
 waffle_hub/utils/data.py
 waffle_hub/utils/draw.py
 waffle_hub/utils/evaluate.py
```

