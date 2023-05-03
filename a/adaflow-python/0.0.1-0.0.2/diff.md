# Comparing `tmp/adaflow-python-0.0.1.tar.gz` & `tmp/adaflow-python-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/disk/jingyao/local/AdaFlow/modules/adaflow-python/dist/.tmp-i3sjyp69/adaflow-python-0.0.1.tar", last modified: Thu Apr 13 07:42:37 2023, max compression
+gzip compressed data, was "adaflow-python-0.0.2.tar", last modified: Wed May  3 06:33:17 2023, max compression
```

## Comparing `adaflow-python-0.0.1.tar` & `adaflow-python-0.0.2.tar`

### file list

```diff
@@ -1,52 +1,62 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:42:37.000000 adaflow-python-0.0.1/
--rw-r--r--   0 root         (0) root         (0)    11399 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      557 2023-04-13 07:42:37.000000 adaflow-python-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       52 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)       84 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      814 2023-04-13 07:42:37.000000 adaflow-python-0.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:42:37.000000 adaflow-python-0.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:42:37.000000 adaflow-python-0.0.1/src/adaflow/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:42:37.000000 adaflow-python-0.0.1/src/adaflow/av/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/av/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:42:37.000000 adaflow-python-0.0.1/src/adaflow/av/data/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/av/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3858 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/av/data/av_data_frame.py
--rw-r--r--   0 root         (0) root         (0)     1670 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/av/data/av_data_packet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:42:37.000000 adaflow-python-0.0.1/src/adaflow/av/metadata/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/av/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2617 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/av/metadata/flow_json_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:42:37.000000 adaflow-python-0.0.1/src/adaflow/av/pipeline/
--rw-r--r--   0 root         (0) root         (0)       98 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/av/pipeline/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:42:37.000000 adaflow-python-0.0.1/src/adaflow/av/pipeline/dialects/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/av/pipeline/dialects/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1992 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/av/pipeline/dialects/base_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1190 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/av/pipeline/dialects/delegate_gstreamer_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     3003 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/av/pipeline/dialects/dialect_template_helper.py
--rw-r--r--   0 root         (0) root         (0)     3410 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/av/pipeline/dialects/duplex_gstreamer_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1587 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/av/pipeline/dialects/gst_context.py
--rw-r--r--   0 root         (0) root         (0)     3640 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/av/pipeline/dialects/gst_tools.py
--rw-r--r--   0 root         (0) root         (0)     9803 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/av/pipeline/dialects/gstreamer_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     4060 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/av/pipeline/dialects/readable_gstreamer_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     4989 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/av/pipeline/dialects/writable_gstreamer_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:42:37.000000 adaflow-python-0.0.1/src/adaflow/av/pipeline/model/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/av/pipeline/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/av/pipeline/model/attribute.py
--rw-r--r--   0 root         (0) root         (0)     2932 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/av/pipeline/model/graph.py
--rw-r--r--   0 root         (0) root         (0)      504 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/av/pipeline/model/struct.py
--rw-r--r--   0 root         (0) root         (0)     4224 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/av/pipeline/pipeline_composer.py
--rw-r--r--   0 root         (0) root         (0)     4184 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/av/pipeline/pipeline_factory.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/av/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:42:37.000000 adaflow-python-0.0.1/src/adaflow/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      402 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/cli/base.py
--rw-r--r--   0 root         (0) root         (0)      597 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/cli/cli.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/cli/init.py
--rw-r--r--   0 root         (0) root         (0)     2659 2023-04-13 07:29:11.000000 adaflow-python-0.0.1/src/adaflow/cli/launch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:42:37.000000 adaflow-python-0.0.1/src/adaflow_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)      557 2023-04-13 07:42:37.000000 adaflow-python-0.0.1/src/adaflow_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1528 2023-04-13 07:42:37.000000 adaflow-python-0.0.1/src/adaflow_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 07:42:37.000000 adaflow-python-0.0.1/src/adaflow_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-04-13 07:42:37.000000 adaflow-python-0.0.1/src/adaflow_python.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       72 2023-04-13 07:42:37.000000 adaflow-python-0.0.1/src/adaflow_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-13 07:42:37.000000 adaflow-python-0.0.1/src/adaflow_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:33:17.334359 adaflow-python-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-03 06:33:17.334359 adaflow-python-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-03 06:33:17.334359 adaflow-python-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:33:17.326359 adaflow-python-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:33:17.326359 adaflow-python-0.0.2/src/adaflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:33:17.326359 adaflow-python-0.0.2/src/adaflow/av/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:33:17.326359 adaflow-python-0.0.2/src/adaflow/av/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/data/av_data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/data/av_data_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:33:17.326359 adaflow-python-0.0.2/src/adaflow/av/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/metadata/flow_json_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:33:17.330359 adaflow-python-0.0.2/src/adaflow/av/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/pipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:33:17.330359 adaflow-python-0.0.2/src/adaflow/av/pipeline/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/pipeline/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/pipeline/dialects/base_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/pipeline/dialects/delegate_gstreamer_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/pipeline/dialects/dialect_template_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/pipeline/dialects/duplex_gstreamer_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/pipeline/dialects/gst_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/pipeline/dialects/gst_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/pipeline/dialects/gstreamer_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/pipeline/dialects/readable_gstreamer_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/pipeline/dialects/writable_gstreamer_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:33:17.330359 adaflow-python-0.0.2/src/adaflow/av/pipeline/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/pipeline/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/pipeline/model/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/pipeline/model/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/pipeline/model/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/pipeline/pipeline_composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/pipeline/pipeline_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:33:17.330359 adaflow-python-0.0.2/src/adaflow/av/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/repo/local_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:33:17.330359 adaflow-python-0.0.2/src/adaflow/av/serving/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/serving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:33:17.330359 adaflow-python-0.0.2/src/adaflow/av/serving/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/serving/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/serving/http/http_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/serving/http/http_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/av/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:33:17.330359 adaflow-python-0.0.2/src/adaflow/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/cli/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-03 06:33:00.000000 adaflow-python-0.0.2/src/adaflow/cli/serve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:33:17.334359 adaflow-python-0.0.2/src/adaflow_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-03 06:33:17.000000 adaflow-python-0.0.2/src/adaflow_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-03 06:33:17.000000 adaflow-python-0.0.2/src/adaflow_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:33:17.000000 adaflow-python-0.0.2/src/adaflow_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-03 06:33:17.000000 adaflow-python-0.0.2/src/adaflow_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-03 06:33:17.000000 adaflow-python-0.0.2/src/adaflow_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 06:33:17.000000 adaflow-python-0.0.2/src/adaflow_python.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `adaflow-python-0.0.1/LICENSE` & `adaflow-python-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adaflow-python-0.0.1/PKG-INFO` & `adaflow-python-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: adaflow-python
-Version: 0.0.1
+Version: 0.0.2
 Summary: AdaFlow is a multimedia pipeline frameworks to offer Deep Learning model integration.
 Home-page: https://github.com/modelscope/adaflow
 Author: "long.qul, jingyao.ww, jiayong.djy, hanbing.han, yulin.yu"
 License: MIT License
 Keywords: example,setuptools
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # adaflow-python
 
-Pythton API for AdaFlow frameworks
+Python API for Adaflow. Please refer to [AdaFlow](https://github.com/modelscope/AdaFlow) for more information.
```

### Comparing `adaflow-python-0.0.1/setup.cfg` & `adaflow-python-0.0.2/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = adaflow-python
-version = 0.0.1
+version = 0.0.2
 author = "long.qul, jingyao.ww, jiayong.djy, hanbing.han, yulin.yu"
 url = https://github.com/modelscope/adaflow
 description = AdaFlow is a multimedia pipeline frameworks to offer Deep Learning model integration.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = example, setuptools
 license = MIT License
@@ -22,14 +22,16 @@
 	matplotlib
 	networkx
 	PyGObject
 	jinja2
 	matplotlib
 	jsonschema
 	pyyaml
+	flask
+	gunicorn
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	adaflow = adaflow.cli.cli:run_cmd
```

### Comparing `adaflow-python-0.0.1/src/adaflow/av/data/av_data_frame.py` & `adaflow-python-0.0.2/src/adaflow/av/data/av_data_frame.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,42 +51,39 @@
             self.log.error('AVDataFrame has not %s metadata' % meta_key)
             return "NULL"
 
         else:
             get_message_json = json.loads(get_message_str)
             if meta_key not in get_message_json:
                 self.log.error('AVDataFrame has not %s metadata' % meta_key)
-
-            get_message = get_message_json[meta_key][0]
-
-        return get_message
+            else:
+                get_message = get_message_json[meta_key]
+                return get_message
 
     def add_json_meta(self, message, meta_key):
         """
         Attach message to this VideoFrame by meta_key.
         :param message:json metadata message
         :param meta_key:metadata keyword
         :return:None
         """
         get_message_str = flow_meta_get(self.__buffer)
 
         # first-to-add-metadata
         if get_message_str == "NULL":
             json_key_v = dict()
-            json_key_v[meta_key] = []
-            json_key_v[meta_key].append(message)
+            json_key_v[meta_key] = message
             json_message = json.dumps(json_key_v, cls=NumpyArrayEncoder)
             flow_meta_add(self.__buffer, json_message.encode('utf-8'))
         else:
             get_message = json.loads(get_message_str)
             if meta_key in get_message:
                 self.log.error('%s is duplicate definition, change a new key ' % meta_key)
             else:
-                get_message[meta_key] = []
-                get_message[meta_key].append(message)
+                get_message[meta_key] = message
                 json_message = json.dumps(get_message, cls=NumpyArrayEncoder)
                 flow_meta_remove(self.__buffer)
                 flow_meta_add(self.__buffer, json_message.encode('utf-8'))
 
     def remove_json_meta(self):
         """
         Remove message from this VideoFrame
@@ -103,8 +100,8 @@
         with self.__buffer.map(flag) as info:
             image = numpy.ndarray(
                 shape=(self.height, self.width, self.channel),
                 dtype=numpy.uint8,
                 buffer=info.data,
                 offset=self.__offset
             )
-            return image
+            return image
```

### Comparing `adaflow-python-0.0.1/src/adaflow/av/data/av_data_packet.py` & `adaflow-python-0.0.2/src/adaflow/av/data/av_data_packet.py`

 * *Files identical despite different names*

### Comparing `adaflow-python-0.0.1/src/adaflow/av/metadata/flow_json_meta.py` & `adaflow-python-0.0.2/src/adaflow/av/metadata/flow_json_meta.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 gi.require_version('GLib', '2.0')
 gi.require_version('Gst', '1.0')
 
 logger = logging.getLogger("JSONMetadata")
 sys_platform = platform.platform().lower()
 
 if "macos" in sys_platform or "darwin" in sys_platform:
-    libgst = CDLL(os.getenv("LIB_GSTREAMER_PATH", "libflowmetadata.dylib"))
+    libgst = CDLL(os.getenv("LIB_GSTREAMER_PATH", "libflow_gst_plugin.dylib"))
 elif "linux" in sys_platform:
-    libgst = CDLL(os.getenv("LIB_GSTREAMER_PATH", "libflowmetadata.so"))
+    libgst = CDLL(os.getenv("LIB_GSTREAMER_PATH", "libflow_gst_plugin.so"))
 else:
     print("other platform")
 
 
 class FLOWJSONMeta(Structure):
     _fields_ = [('_meta_flags', c_int),
                 ('_info', c_void_p),
@@ -63,21 +63,19 @@
 def flow_meta_add_key(buffer, message, meta_key):
     # Writes json message to Gst.Buffer with meta_key
     get_message_str = flow_meta_get(buffer)
 
     # first-to-add-metadata
     if get_message_str == "NULL":
         json_key_v = dict()
-        json_key_v[meta_key] = []
-        json_key_v[meta_key].append(message)
+        json_key_v[meta_key] = message
         json_message = json.dumps(json_key_v, cls=NumpyArrayEncoder)
         flow_meta_add(buffer, json_message.encode('utf-8'))
     else:
         get_message = json.loads(get_message_str)
         if meta_key in get_message:
             logger.error('%s is duplicate definition, change a new key ' % meta_key)
         else:
-            get_message[meta_key] = []
-            get_message[meta_key].append(message)
+            get_message[meta_key] = message
             json_message = json.dumps(get_message, cls=NumpyArrayEncoder)
             flow_meta_remove(buffer)
             flow_meta_add(buffer, json_message.encode('utf-8'))
```

### Comparing `adaflow-python-0.0.1/src/adaflow/av/pipeline/dialects/base_pipeline.py` & `adaflow-python-0.0.2/src/adaflow/av/pipeline/dialects/base_pipeline.py`

 * *Files identical despite different names*

### Comparing `adaflow-python-0.0.1/src/adaflow/av/pipeline/dialects/delegate_gstreamer_pipeline.py` & `adaflow-python-0.0.2/src/adaflow/av/pipeline/dialects/delegate_gstreamer_pipeline.py`

 * *Files identical despite different names*

### Comparing `adaflow-python-0.0.1/src/adaflow/av/pipeline/dialects/dialect_template_helper.py` & `adaflow-python-0.0.2/src/adaflow/av/pipeline/dialects/dialect_template_helper.py`

 * *Files identical despite different names*

### Comparing `adaflow-python-0.0.1/src/adaflow/av/pipeline/dialects/duplex_gstreamer_pipeline.py` & `adaflow-python-0.0.2/src/adaflow/av/pipeline/dialects/duplex_gstreamer_pipeline.py`

 * *Files identical despite different names*

### Comparing `adaflow-python-0.0.1/src/adaflow/av/pipeline/dialects/gst_context.py` & `adaflow-python-0.0.2/src/adaflow/av/pipeline/dialects/gst_context.py`

 * *Files identical despite different names*

### Comparing `adaflow-python-0.0.1/src/adaflow/av/pipeline/dialects/gst_tools.py` & `adaflow-python-0.0.2/src/adaflow/av/pipeline/dialects/gst_tools.py`

 * *Files identical despite different names*

### Comparing `adaflow-python-0.0.1/src/adaflow/av/pipeline/dialects/gstreamer_pipeline.py` & `adaflow-python-0.0.2/src/adaflow/av/pipeline/dialects/gstreamer_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,29 +17,29 @@
 from gi.repository import Gst, GLib, GObject, GstApp, GstVideo  # noqa:F401,F402
 
 
 Gst.init(sys.argv if hasattr(sys, "argv") else None)
 
 
 class GStreamerPipeline(BasePipeline):
-    def __init__(self, pipeline_model: Dict[str, any], task_model: Dict[str, any], pipeline_configure: Callable[[Gst.Pipeline], None] = None) -> None:
+    def __init__(self, pipeline_model: Dict[str, any], task_model: Dict[str, any], log: logging.Logger = None, pipeline_configure: Callable[[Gst.Pipeline], None] = None) -> None:
         """
         Default constructor for a plain GStreamerPipeline
         Args:
             pipeline_model: Pipeline definition dict object
             task_model: Task definition dict object
             pipeline_configure: Pipeline configuration function
         """
         # TODO validate pipeline_model and task_model
         super().__init__()
         self._pipeline_model = pipeline_model
         self._task_model = task_model
         self._bus = None
         self._gst_pipeline = None
-        self._log = logging.getLogger("GStreamerPipeline")
+        self._log = log or logging.getLogger("GStreamerPipeline")
         self._terminal_event = threading.Event()
         self._template_env = Environment()
 
         # convert array to string
         template_string = pipeline_model["dialect"]
         if isinstance(template_string, list):
             template_string = " ! ".join(template_string)
@@ -217,14 +217,15 @@
 class GStreamerPipelineBuilder:
     """Builder for GStreamerPipeline"""
 
     def __init__(self) -> None:
         super().__init__()
         self._pipeline = {}
         self._task = {}
+        self._logger = None
 
     def pipeline(self, pipeline_model: Dict[str, any]):
         """set pipeline model dict"""
         self._pipeline = pipeline_model
         return self
 
     def task(self, task_model: Dict[str, any]):
@@ -257,11 +258,15 @@
             self reference
 
         """
         if "parameters" not in self._task or parameters is not None:
             self._task["parameters"] = parameters
         return self
 
+    def logger(self, logger: logging.Logger):
+        self._logger = logger
+        return self
+
     def build(self) -> GStreamerPipeline:
         """Return the pipeline object"""
-        return GStreamerPipeline(self._pipeline, self._task)
+        return GStreamerPipeline(self._pipeline, self._task, log=self._logger)
```

### Comparing `adaflow-python-0.0.1/src/adaflow/av/pipeline/dialects/readable_gstreamer_pipeline.py` & `adaflow-python-0.0.2/src/adaflow/av/pipeline/dialects/readable_gstreamer_pipeline.py`

 * *Files identical despite different names*

### Comparing `adaflow-python-0.0.1/src/adaflow/av/pipeline/dialects/writable_gstreamer_pipeline.py` & `adaflow-python-0.0.2/src/adaflow/av/pipeline/dialects/writable_gstreamer_pipeline.py`

 * *Files identical despite different names*

### Comparing `adaflow-python-0.0.1/src/adaflow/av/pipeline/model/attribute.py` & `adaflow-python-0.0.2/src/adaflow/av/pipeline/model/attribute.py`

 * *Files identical despite different names*

### Comparing `adaflow-python-0.0.1/src/adaflow/av/pipeline/model/graph.py` & `adaflow-python-0.0.2/src/adaflow/av/pipeline/model/graph.py`

 * *Files identical despite different names*

### Comparing `adaflow-python-0.0.1/src/adaflow/av/pipeline/pipeline_composer.py` & `adaflow-python-0.0.2/src/adaflow/av/pipeline/pipeline_composer.py`

 * *Files identical despite different names*

### Comparing `adaflow-python-0.0.1/src/adaflow/av/pipeline/pipeline_factory.py` & `adaflow-python-0.0.2/src/adaflow/av/pipeline/pipeline_factory.py`

 * *Files identical despite different names*

### Comparing `adaflow-python-0.0.1/src/adaflow/av/utils.py` & `adaflow-python-0.0.2/src/adaflow/av/utils.py`

 * *Files identical despite different names*

### Comparing `adaflow-python-0.0.1/src/adaflow/cli/init.py` & `adaflow-python-0.0.2/src/adaflow/cli/init.py`

 * *Files identical despite different names*

### Comparing `adaflow-python-0.0.1/src/adaflow/cli/launch.py` & `adaflow-python-0.0.2/src/adaflow/cli/launch.py`

 * *Files identical despite different names*

### Comparing `adaflow-python-0.0.1/src/adaflow_python.egg-info/PKG-INFO` & `adaflow-python-0.0.2/src/adaflow_python.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: adaflow-python
-Version: 0.0.1
+Version: 0.0.2
 Summary: AdaFlow is a multimedia pipeline frameworks to offer Deep Learning model integration.
 Home-page: https://github.com/modelscope/adaflow
 Author: "long.qul, jingyao.ww, jiayong.djy, hanbing.han, yulin.yu"
 License: MIT License
 Keywords: example,setuptools
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # adaflow-python
 
-Pythton API for AdaFlow frameworks
+Python API for Adaflow. Please refer to [AdaFlow](https://github.com/modelscope/AdaFlow) for more information.
```

### Comparing `adaflow-python-0.0.1/src/adaflow_python.egg-info/SOURCES.txt` & `adaflow-python-0.0.2/src/adaflow_python.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -23,18 +23,25 @@
 src/adaflow/av/pipeline/dialects/gstreamer_pipeline.py
 src/adaflow/av/pipeline/dialects/readable_gstreamer_pipeline.py
 src/adaflow/av/pipeline/dialects/writable_gstreamer_pipeline.py
 src/adaflow/av/pipeline/model/__init__.py
 src/adaflow/av/pipeline/model/attribute.py
 src/adaflow/av/pipeline/model/graph.py
 src/adaflow/av/pipeline/model/struct.py
+src/adaflow/av/repo/__init__.py
+src/adaflow/av/repo/local_repository.py
+src/adaflow/av/serving/__init__.py
+src/adaflow/av/serving/http/__init__.py
+src/adaflow/av/serving/http/http_server.py
+src/adaflow/av/serving/http/http_utils.py
 src/adaflow/cli/__init__.py
 src/adaflow/cli/base.py
 src/adaflow/cli/cli.py
 src/adaflow/cli/init.py
 src/adaflow/cli/launch.py
+src/adaflow/cli/serve.py
 src/adaflow_python.egg-info/PKG-INFO
 src/adaflow_python.egg-info/SOURCES.txt
 src/adaflow_python.egg-info/dependency_links.txt
 src/adaflow_python.egg-info/entry_points.txt
 src/adaflow_python.egg-info/requires.txt
 src/adaflow_python.egg-info/top_level.txt
```

