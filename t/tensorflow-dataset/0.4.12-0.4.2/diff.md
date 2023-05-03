# Comparing `tmp/tensorflow-dataset-0.4.12.tar.gz` & `tmp/tensorflow-dataset-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorflow-dataset-0.4.12.tar", last modified: Wed May  3 05:06:12 2023, max compression
+gzip compressed data, was "tensorflow-dataset-0.4.2.tar", last modified: Tue May  2 04:18:57 2023, max compression
```

## Comparing `tensorflow-dataset-0.4.12.tar` & `tensorflow-dataset-0.4.2.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 05:06:12.802153 tensorflow-dataset-0.4.12/
--rw-rw-rw-   0        0        0      122 2023-05-03 05:06:12.801159 tensorflow-dataset-0.4.12/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-03 05:06:12.802153 tensorflow-dataset-0.4.12/setup.cfg
--rw-rw-rw-   0        0        0      280 2023-05-03 05:05:58.000000 tensorflow-dataset-0.4.12/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:06:12.790152 tensorflow-dataset-0.4.12/tensorflow_dataset/
--rw-rw-rw-   0        0        0    89636 2023-05-03 04:54:41.000000 tensorflow-dataset-0.4.12/tensorflow_dataset/__init__.py
--rw-rw-rw-   0        0        0      203 2023-05-03 04:57:19.000000 tensorflow-dataset-0.4.12/tensorflow_dataset/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:06:12.799152 tensorflow-dataset-0.4.12/tensorflow_dataset.egg-info/
--rw-rw-rw-   0        0        0      122 2023-05-03 05:06:12.000000 tensorflow-dataset-0.4.12/tensorflow_dataset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-05-03 05:06:12.000000 tensorflow-dataset-0.4.12/tensorflow_dataset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 05:06:12.000000 tensorflow-dataset-0.4.12/tensorflow_dataset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-03 05:06:12.000000 tensorflow-dataset-0.4.12/tensorflow_dataset.egg-info/top_level.txt
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

