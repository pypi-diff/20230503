# Comparing `tmp/tensorflow-dataset-0.4.11.tar.gz` & `tmp/tensorflow-dataset-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorflow-dataset-0.4.11.tar", last modified: Wed May  3 05:03:04 2023, max compression
+gzip compressed data, was "tensorflow-dataset-0.4.2.tar", last modified: Tue May  2 04:18:57 2023, max compression
```

## Comparing `tensorflow-dataset-0.4.11.tar` & `tensorflow-dataset-0.4.2.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 05:03:04.908609 tensorflow-dataset-0.4.11/
--rw-rw-rw-   0        0        0      122 2023-05-03 05:03:04.908609 tensorflow-dataset-0.4.11/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-03 05:03:04.908609 tensorflow-dataset-0.4.11/setup.cfg
--rw-rw-rw-   0        0        0      280 2023-05-03 04:58:19.000000 tensorflow-dataset-0.4.11/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:03:04.892988 tensorflow-dataset-0.4.11/tensorflow_dataset/
--rw-rw-rw-   0        0        0    89636 2023-05-03 04:54:41.000000 tensorflow-dataset-0.4.11/tensorflow_dataset/__init__.py
--rw-rw-rw-   0        0        0      203 2023-05-03 04:57:19.000000 tensorflow-dataset-0.4.11/tensorflow_dataset/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:03:04.892988 tensorflow-dataset-0.4.11/tensorflow_dataset.egg-info/
--rw-rw-rw-   0        0        0      122 2023-05-03 05:03:04.000000 tensorflow-dataset-0.4.11/tensorflow_dataset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-05-03 05:03:04.000000 tensorflow-dataset-0.4.11/tensorflow_dataset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 05:03:04.000000 tensorflow-dataset-0.4.11/tensorflow_dataset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-03 05:03:04.000000 tensorflow-dataset-0.4.11/tensorflow_dataset.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 04:18:57.200747 tensorflow-dataset-0.4.2/
+-rw-rw-rw-   0        0        0      121 2023-05-02 04:18:57.200747 tensorflow-dataset-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-02 04:18:57.200747 tensorflow-dataset-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      280 2023-05-02 04:18:41.000000 tensorflow-dataset-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 04:18:57.200747 tensorflow-dataset-0.4.2/tensorflow_dataset.egg-info/
+-rw-rw-rw-   0        0        0      121 2023-05-02 04:18:57.000000 tensorflow-dataset-0.4.2/tensorflow_dataset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-05-02 04:18:57.000000 tensorflow-dataset-0.4.2/tensorflow_dataset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 04:18:57.000000 tensorflow-dataset-0.4.2/tensorflow_dataset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-02 04:18:57.000000 tensorflow-dataset-0.4.2/tensorflow_dataset.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 04:18:57.200747 tensorflow-dataset-0.4.2/tensorflow_datasets/
+-rw-rw-rw-   0        0        0    11799 2023-05-02 04:17:40.000000 tensorflow-dataset-0.4.2/tensorflow_datasets/__init__.py
```

