# Comparing `tmp/dghs-imgutils-0.0.1.tar.gz` & `tmp/dghs-imgutils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dghs-imgutils-0.0.1.tar", last modified: Wed Apr 26 08:03:45 2023, max compression
+gzip compressed data, was "dghs-imgutils-0.0.2.tar", last modified: Wed May  3 06:27:29 2023, max compression
```

## Comparing `dghs-imgutils-0.0.1.tar` & `dghs-imgutils-0.0.2.tar`

### file list

```diff
@@ -1,49 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:03:45.342438 dghs-imgutils-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-04-26 08:03:45.342438 dghs-imgutils-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:03:45.342438 dghs-imgutils-0.0.1/dghs_imgutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-04-26 08:03:45.000000 dghs-imgutils-0.0.1/dghs_imgutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-26 08:03:45.000000 dghs-imgutils-0.0.1/dghs_imgutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:03:45.000000 dghs-imgutils-0.0.1/dghs_imgutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-26 08:03:45.000000 dghs-imgutils-0.0.1/dghs_imgutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 08:03:45.000000 dghs-imgutils-0.0.1/dghs_imgutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:03:45.342438 dghs-imgutils-0.0.1/imgutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/imgutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:03:45.342438 dghs-imgutils-0.0.1/imgutils/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/imgutils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/imgutils/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:03:45.342438 dghs-imgutils-0.0.1/imgutils/data/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/imgutils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/imgutils/data/background.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/imgutils/data/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/imgutils/data/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/imgutils/data/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:03:45.342438 dghs-imgutils-0.0.1/imgutils/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/imgutils/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/imgutils/metrics/lpips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/imgutils/metrics/psnr_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:03:45.342438 dghs-imgutils-0.0.1/imgutils/segment/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/imgutils/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/imgutils/segment/isnetis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:03:45.342438 dghs-imgutils-0.0.1/imgutils/tagging/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/imgutils/tagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/imgutils/tagging/deepdanbooru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/imgutils/tagging/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/imgutils/tagging/wd14.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:03:45.342438 dghs-imgutils-0.0.1/imgutils/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/imgutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/imgutils/utils/onnxruntime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:03:45.342438 dghs-imgutils-0.0.1/imgutils/validate/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/imgutils/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/imgutils/validate/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/imgutils/validate/monochrome.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/imgutils/validate/truncate.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/requirements-gpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/requirements-zoo.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 08:03:45.342438 dghs-imgutils-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-26 08:02:56.000000 dghs-imgutils-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:27:29.128132 dghs-imgutils-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13250 2023-05-03 06:27:29.128132 dghs-imgutils-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:27:29.124132 dghs-imgutils-0.0.2/dghs_imgutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13250 2023-05-03 06:27:29.000000 dghs-imgutils-0.0.2/dghs_imgutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-03 06:27:29.000000 dghs-imgutils-0.0.2/dghs_imgutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:27:29.000000 dghs-imgutils-0.0.2/dghs_imgutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-03 06:27:29.000000 dghs-imgutils-0.0.2/dghs_imgutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 06:27:29.000000 dghs-imgutils-0.0.2/dghs_imgutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:27:29.124132 dghs-imgutils-0.0.2/imgutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:27:29.124132 dghs-imgutils-0.0.2/imgutils/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:27:29.124132 dghs-imgutils-0.0.2/imgutils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/data/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/data/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/data/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/data/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/data/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:27:29.124132 dghs-imgutils-0.0.2/imgutils/detect/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/detect/_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/detect/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/detect/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/detect/visual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:27:29.128132 dghs-imgutils-0.0.2/imgutils/edge/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/edge/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/edge/canny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/edge/lineart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/edge/lineart_anime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:27:29.128132 dghs-imgutils-0.0.2/imgutils/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/metrics/lpips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/metrics/psnr_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:27:29.128132 dghs-imgutils-0.0.2/imgutils/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/segment/isnetis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:27:29.128132 dghs-imgutils-0.0.2/imgutils/tagging/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/tagging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/tagging/deepdanbooru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/tagging/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/tagging/wd14.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:27:29.128132 dghs-imgutils-0.0.2/imgutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/utils/onnxruntime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:27:29.128132 dghs-imgutils-0.0.2/imgutils/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/validate/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/validate/monochrome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/imgutils/validate/truncate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/requirements-gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/requirements-zoo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 06:27:29.128132 dghs-imgutils-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-03 06:26:31.000000 dghs-imgutils-0.0.2/setup.py
```

### Comparing `dghs-imgutils-0.0.1/LICENSE` & `dghs-imgutils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.1/PKG-INFO` & `dghs-imgutils-0.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: dghs-imgutils
-Version: 0.0.1
-Summary: Utilities of images.
-Home-page: https://github.com/deepghs/imgutils
-Author: narugo1992
-Author-email: narugo@126.com
-License: Apache License, Version 2.0
-Keywords: Utilities of images.
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: gpu
-Provides-Extra: test
-Provides-Extra: doc
-License-File: LICENSE
-
 # imgutils
 
 [![PyPI](https://img.shields.io/pypi/v/dghs-imgutils)](https://pypi.org/project/dghs-imgutils/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dghs-imgutils)
 ![Loc](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/8bfaa96eaa25cc9dac54debbf22d363d/raw/loc.json)
 ![Comments](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/8bfaa96eaa25cc9dac54debbf22d363d/raw/comments.json)
 
@@ -62,14 +37,22 @@
 ```
 
 For more information about installation, you can refer
 to [Installation](https://deepghs.github.io/imgutils/main/tutorials/installation/index.html).
 
 ## Supported or Developing Features
 
+* [Tachie(差分) Detection and Clustering](https://github.com/deepghs/imgutils#tachie%E5%B7%AE%E5%88%86-detection-and-clustering)
+* [Object Detection](https://github.com/deepghs/imgutils#object-detection)
+* [Edge Detection / Lineart Generation](https://github.com/deepghs/imgutils#edge-detection--lineart-generation)
+* [Monochrome Image Detection](https://github.com/deepghs/imgutils#monochrome-image-detection)
+* [Truncated Image Check](https://github.com/deepghs/imgutils#truncated-image-check)
+* [Image Tagging](https://github.com/deepghs/imgutils#image-tagging)
+* [Character Extraction](https://github.com/deepghs/imgutils#character-extraction)
+
 ### Tachie(差分) Detection and Clustering
 
 For the dataset, we need to filter the differences between the tachie(差分). As shown in the following picture
 
 ![tachie](https://deepghs.github.io/imgutils/main/_images/lpips_full.dat.svg)
 
 We can use `lpips_clustering` to cluster such situations as shown below
@@ -80,14 +63,40 @@
 images = [f'lpips/{i}.jpg' for i in range(1, 10)]
 print(images)
 # ['lpips/1.jpg', 'lpips/2.jpg', 'lpips/3.jpg', 'lpips/4.jpg', 'lpips/5.jpg', 'lpips/6.jpg', 'lpips/7.jpg', 'lpips/8.jpg', 'lpips/9.jpg']
 print(lpips_clustering(images))  # -1 means noises, the same as that in sklearn
 # [0, 0, 0, 1, 1, -1, -1, -1, -1]
 ```
 
+### Object Detection
+
+Currently, object detection is supported for anime faces and person, as shown below
+
+* Face Detection
+
+![face detection](https://deepghs.github.io/imgutils/main/_images/face_detect.dat.svg)
+
+* Person Detection
+
+![person detection](https://deepghs.github.io/imgutils/main/_images/person_detect.dat.svg)
+
+Based on practical tests, face detection currently has a very stable performance and can be used for automation tasks.
+However, person detection is still being further iterated and will focus on enhancing detection capabilities for
+artistic illustrations in the future.
+
+### Edge Detection / Lineart Generation
+
+Anime images can be converted to line drawings using the model provided
+by [patrickvonplaten/controlnet_aux](https://github.com/patrickvonplaten/controlnet_aux), as shown below.
+
+![edge example](https://deepghs.github.io/imgutils/main/_images/edge.dat.svg)
+
+It is worth noting that the `lineart` model may consume more computational resources, while `canny` is the fastest but
+has average effect. Therefore, `lineart_anime` may be the most balanced choice in most cases.
+
 ### Monochrome Image Detection
 
 When filtering the crawled images, we need to remove monochrome images. However, monochrome images are often not simply
 composed of grayscale colors and may still contain colors, as shown by the first two rows of six images in the figure
 below
 
 ![monochrome example](https://deepghs.github.io/imgutils/main/_images/monochrome.dat.svg)
@@ -245,8 +254,8 @@
 mask_, image_ = segment_rgba_with_isnetis('hutao.png')
 image_.save('hutao_seg.png')
 
 mask_, image_ = segment_rgba_with_isnetis('skadi.jpg')
 image_.save('skadi_seg.png')
 ```
 
-This model can be found at https://huggingface.co/skytnt/anime-seg .
+This model can be found at https://huggingface.co/skytnt/anime-seg .
```

### Comparing `dghs-imgutils-0.0.1/README.md` & `dghs-imgutils-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: dghs-imgutils
+Version: 0.0.2
+Summary: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
+Home-page: https://github.com/deepghs/imgutils
+Author: narugo1992
+Author-email: narugo@126.com
+License: Apache License, Version 2.0
+Keywords: Utilities of images.
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: doc
+Provides-Extra: gpu
+License-File: LICENSE
+
 # imgutils
 
 [![PyPI](https://img.shields.io/pypi/v/dghs-imgutils)](https://pypi.org/project/dghs-imgutils/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dghs-imgutils)
 ![Loc](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/8bfaa96eaa25cc9dac54debbf22d363d/raw/loc.json)
 ![Comments](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/8bfaa96eaa25cc9dac54debbf22d363d/raw/comments.json)
 
@@ -37,14 +62,22 @@
 ```
 
 For more information about installation, you can refer
 to [Installation](https://deepghs.github.io/imgutils/main/tutorials/installation/index.html).
 
 ## Supported or Developing Features
 
+* [Tachie(差分) Detection and Clustering](https://github.com/deepghs/imgutils#tachie%E5%B7%AE%E5%88%86-detection-and-clustering)
+* [Object Detection](https://github.com/deepghs/imgutils#object-detection)
+* [Edge Detection / Lineart Generation](https://github.com/deepghs/imgutils#edge-detection--lineart-generation)
+* [Monochrome Image Detection](https://github.com/deepghs/imgutils#monochrome-image-detection)
+* [Truncated Image Check](https://github.com/deepghs/imgutils#truncated-image-check)
+* [Image Tagging](https://github.com/deepghs/imgutils#image-tagging)
+* [Character Extraction](https://github.com/deepghs/imgutils#character-extraction)
+
 ### Tachie(差分) Detection and Clustering
 
 For the dataset, we need to filter the differences between the tachie(差分). As shown in the following picture
 
 ![tachie](https://deepghs.github.io/imgutils/main/_images/lpips_full.dat.svg)
 
 We can use `lpips_clustering` to cluster such situations as shown below
@@ -55,14 +88,40 @@
 images = [f'lpips/{i}.jpg' for i in range(1, 10)]
 print(images)
 # ['lpips/1.jpg', 'lpips/2.jpg', 'lpips/3.jpg', 'lpips/4.jpg', 'lpips/5.jpg', 'lpips/6.jpg', 'lpips/7.jpg', 'lpips/8.jpg', 'lpips/9.jpg']
 print(lpips_clustering(images))  # -1 means noises, the same as that in sklearn
 # [0, 0, 0, 1, 1, -1, -1, -1, -1]
 ```
 
+### Object Detection
+
+Currently, object detection is supported for anime faces and person, as shown below
+
+* Face Detection
+
+![face detection](https://deepghs.github.io/imgutils/main/_images/face_detect.dat.svg)
+
+* Person Detection
+
+![person detection](https://deepghs.github.io/imgutils/main/_images/person_detect.dat.svg)
+
+Based on practical tests, face detection currently has a very stable performance and can be used for automation tasks.
+However, person detection is still being further iterated and will focus on enhancing detection capabilities for
+artistic illustrations in the future.
+
+### Edge Detection / Lineart Generation
+
+Anime images can be converted to line drawings using the model provided
+by [patrickvonplaten/controlnet_aux](https://github.com/patrickvonplaten/controlnet_aux), as shown below.
+
+![edge example](https://deepghs.github.io/imgutils/main/_images/edge.dat.svg)
+
+It is worth noting that the `lineart` model may consume more computational resources, while `canny` is the fastest but
+has average effect. Therefore, `lineart_anime` may be the most balanced choice in most cases.
+
 ### Monochrome Image Detection
 
 When filtering the crawled images, we need to remove monochrome images. However, monochrome images are often not simply
 composed of grayscale colors and may still contain colors, as shown by the first two rows of six images in the figure
 below
 
 ![monochrome example](https://deepghs.github.io/imgutils/main/_images/monochrome.dat.svg)
@@ -220,8 +279,8 @@
 mask_, image_ = segment_rgba_with_isnetis('hutao.png')
 image_.save('hutao_seg.png')
 
 mask_, image_ = segment_rgba_with_isnetis('skadi.jpg')
 image_.save('skadi_seg.png')
 ```
 
-This model can be found at https://huggingface.co/skytnt/anime-seg .
+This model can be found at https://huggingface.co/skytnt/anime-seg .
```

### Comparing `dghs-imgutils-0.0.1/dghs_imgutils.egg-info/PKG-INFO` & `dghs-imgutils-0.0.2/dghs_imgutils.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dghs-imgutils
-Version: 0.0.1
-Summary: Utilities of images.
+Version: 0.0.2
+Summary: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Home-page: https://github.com/deepghs/imgutils
 Author: narugo1992
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -14,17 +14,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: gpu
 Provides-Extra: test
 Provides-Extra: doc
+Provides-Extra: gpu
 License-File: LICENSE
 
 # imgutils
 
 [![PyPI](https://img.shields.io/pypi/v/dghs-imgutils)](https://pypi.org/project/dghs-imgutils/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dghs-imgutils)
 ![Loc](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/8bfaa96eaa25cc9dac54debbf22d363d/raw/loc.json)
@@ -62,14 +62,22 @@
 ```
 
 For more information about installation, you can refer
 to [Installation](https://deepghs.github.io/imgutils/main/tutorials/installation/index.html).
 
 ## Supported or Developing Features
 
+* [Tachie(差分) Detection and Clustering](https://github.com/deepghs/imgutils#tachie%E5%B7%AE%E5%88%86-detection-and-clustering)
+* [Object Detection](https://github.com/deepghs/imgutils#object-detection)
+* [Edge Detection / Lineart Generation](https://github.com/deepghs/imgutils#edge-detection--lineart-generation)
+* [Monochrome Image Detection](https://github.com/deepghs/imgutils#monochrome-image-detection)
+* [Truncated Image Check](https://github.com/deepghs/imgutils#truncated-image-check)
+* [Image Tagging](https://github.com/deepghs/imgutils#image-tagging)
+* [Character Extraction](https://github.com/deepghs/imgutils#character-extraction)
+
 ### Tachie(差分) Detection and Clustering
 
 For the dataset, we need to filter the differences between the tachie(差分). As shown in the following picture
 
 ![tachie](https://deepghs.github.io/imgutils/main/_images/lpips_full.dat.svg)
 
 We can use `lpips_clustering` to cluster such situations as shown below
@@ -80,14 +88,40 @@
 images = [f'lpips/{i}.jpg' for i in range(1, 10)]
 print(images)
 # ['lpips/1.jpg', 'lpips/2.jpg', 'lpips/3.jpg', 'lpips/4.jpg', 'lpips/5.jpg', 'lpips/6.jpg', 'lpips/7.jpg', 'lpips/8.jpg', 'lpips/9.jpg']
 print(lpips_clustering(images))  # -1 means noises, the same as that in sklearn
 # [0, 0, 0, 1, 1, -1, -1, -1, -1]
 ```
 
+### Object Detection
+
+Currently, object detection is supported for anime faces and person, as shown below
+
+* Face Detection
+
+![face detection](https://deepghs.github.io/imgutils/main/_images/face_detect.dat.svg)
+
+* Person Detection
+
+![person detection](https://deepghs.github.io/imgutils/main/_images/person_detect.dat.svg)
+
+Based on practical tests, face detection currently has a very stable performance and can be used for automation tasks.
+However, person detection is still being further iterated and will focus on enhancing detection capabilities for
+artistic illustrations in the future.
+
+### Edge Detection / Lineart Generation
+
+Anime images can be converted to line drawings using the model provided
+by [patrickvonplaten/controlnet_aux](https://github.com/patrickvonplaten/controlnet_aux), as shown below.
+
+![edge example](https://deepghs.github.io/imgutils/main/_images/edge.dat.svg)
+
+It is worth noting that the `lineart` model may consume more computational resources, while `canny` is the fastest but
+has average effect. Therefore, `lineart_anime` may be the most balanced choice in most cases.
+
 ### Monochrome Image Detection
 
 When filtering the crawled images, we need to remove monochrome images. However, monochrome images are often not simply
 composed of grayscale colors and may still contain colors, as shown by the first two rows of six images in the figure
 below
 
 ![monochrome example](https://deepghs.github.io/imgutils/main/_images/monochrome.dat.svg)
```

### Comparing `dghs-imgutils-0.0.1/dghs_imgutils.egg-info/SOURCES.txt` & `dghs-imgutils-0.0.2/dghs_imgutils.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,25 @@
 imgutils/config/__init__.py
 imgutils/config/meta.py
 imgutils/data/__init__.py
 imgutils/data/background.py
 imgutils/data/decode.py
 imgutils/data/encode.py
 imgutils/data/image.py
+imgutils/data/layer.py
+imgutils/detect/__init__.py
+imgutils/detect/_yolo.py
+imgutils/detect/face.py
+imgutils/detect/person.py
+imgutils/detect/visual.py
+imgutils/edge/__init__.py
+imgutils/edge/_base.py
+imgutils/edge/canny.py
+imgutils/edge/lineart.py
+imgutils/edge/lineart_anime.py
 imgutils/metrics/__init__.py
 imgutils/metrics/lpips.py
 imgutils/metrics/psnr_.py
 imgutils/segment/__init__.py
 imgutils/segment/isnetis.py
 imgutils/tagging/__init__.py
 imgutils/tagging/deepdanbooru.py
```

### Comparing `dghs-imgutils-0.0.1/imgutils/data/background.py` & `dghs-imgutils-0.0.2/imgutils/data/background.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional
 
 import numpy as np
 from PIL import ImageColor, Image
 
-from .image import ImageTyping, load_image
+from .image import ImageTyping
+from .layer import istack
 
 __all__ = [
     'grid_background',
     'grid_transparent',
 ]
 
 
@@ -58,10 +59,8 @@
         accurately present the state of the generated image, as shown in the following figure
 
         .. image:: grid_transparent.dat.svg
            :align: center
 
     """
     retval = grid_background(image.height, image.width, step, forecolor, backcolor)
-    image = load_image(image, force_background=None, mode='RGBA')
-    retval.paste(image, mask=image)
-    return retval.convert('RGB')
+    return istack(retval, image).convert('RGB')
```

### Comparing `dghs-imgutils-0.0.1/imgutils/data/decode.py` & `dghs-imgutils-0.0.2/imgutils/data/decode.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.1/imgutils/data/encode.py` & `dghs-imgutils-0.0.2/imgutils/data/encode.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.1/imgutils/data/image.py` & `dghs-imgutils-0.0.2/imgutils/data/image.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,14 +39,9 @@
     if not isinstance(images, (list, tuple)):
         images = [images]
 
     return [load_image(item, mode) for item in images]
 
 
 def add_background_for_rgba(image: ImageTyping, background: str = 'white'):
-    if not isinstance(image, Image.Image):
-        image = load_image(image)
-    image = image.convert("RGBA")
-    new_image = Image.new("RGBA", image.size, background)
-    new_image.paste(image, mask=image)
-    image = new_image.convert("RGB")
-    return image
+    from .layer import istack
+    return istack(background, image).convert('RGB')
```

### Comparing `dghs-imgutils-0.0.1/imgutils/metrics/lpips.py` & `dghs-imgutils-0.0.2/imgutils/metrics/lpips.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.1/imgutils/metrics/psnr_.py` & `dghs-imgutils-0.0.2/imgutils/metrics/psnr_.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.1/imgutils/segment/isnetis.py` & `dghs-imgutils-0.0.2/imgutils/segment/isnetis.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,17 +3,16 @@
     Anime character segmentation, based on https://huggingface.co/skytnt/anime-seg .
 """
 from functools import lru_cache
 
 import cv2
 import huggingface_hub
 import numpy as np
-from PIL import ImageColor, Image
 
-from ..data import ImageTyping, load_image
+from ..data import ImageTyping, load_image, istack
 from ..utils.onnxruntime import open_onnx_model
 
 
 @lru_cache()
 def _get_model():
     return open_onnx_model(huggingface_hub.hf_hub_download("skytnt/anime-seg", "isnetis.onnx"))
 
@@ -22,30 +21,30 @@
     """
     Overview:
         Get mask with isnetis.
 
     :param image: Original image (assume its size is ``(H, W)``).
     :param scale: Scale when passing it into neural network. Default is ``1024``,
         inspired by https://huggingface.co/spaces/skytnt/anime-remove-background/blob/main/app.py#L8 .
-    :return: Get a mask with all the pixels, which shape is ``(H, W, 1)``.
+    :return: Get a mask with all the pixels, which shape is ``(H, W)``.
     """
     image = np.asarray(load_image(image, mode='RGB'))
     image = (image / 255).astype(np.float32)
     h, w = h0, w0 = image.shape[:-1]
     h, w = (scale, int(scale * w / h)) if h > w else (int(scale * h / w), scale)
     ph, pw = scale - h, scale - w
     img_input = np.zeros([scale, scale, 3], dtype=np.float32)
     img_input[ph // 2:ph // 2 + h, pw // 2:pw // 2 + w] = cv2.resize(image, (w, h))
     img_input = np.transpose(img_input, (2, 0, 1))
     img_input = img_input[np.newaxis, :]
     mask = _get_model().run(None, {'img': img_input})[0][0]
     mask = np.transpose(mask, (1, 2, 0))
     mask = mask[ph // 2:ph // 2 + h, pw // 2:pw // 2 + w]
     mask = cv2.resize(mask, (w0, h0))[:, :, np.newaxis]
-    return mask
+    return mask.reshape(*mask.shape[:-1])
 
 
 def segment_with_isnetis(image: ImageTyping, background: str = 'lime', scale: int = 1024):
     """
     Overview:
         Segment image with pure color background.
 
@@ -68,26 +67,15 @@
 
         .. image:: isnetis_color.dat.svg
            :align: center
 
     """
     image = load_image(image, mode='RGB')
     mask = get_isnetis_mask(image, scale)
-    h, w, _ = mask.shape
-
-    _mk = np.zeros((h, w, 3))
-    r, g, b = ImageColor.getrgb(background)
-    _mk[:, :, 0] = r
-    _mk[:, :, 1] = g
-    _mk[:, :, 2] = b
-
-    _image_arr = np.asarray(image)
-    _masked_data = (_mk * (1 - mask) + _image_arr * mask).astype(np.uint8)
-
-    return mask, Image.fromarray(_masked_data, mode='RGB')
+    return mask, istack((background, 1.0), (image, mask)).convert('RGB')
 
 
 def segment_rgba_with_isnetis(image: ImageTyping, scale: int = 1024):
     """
     Overview:
         Segment image with transparent background.
 
@@ -109,15 +97,8 @@
 
         .. image:: isnetis_trans.dat.svg
            :align: center
 
     """
     image = load_image(image, mode='RGB')
     mask = get_isnetis_mask(image, scale)
-    h, w, _ = mask.shape
-
-    _mk = np.zeros((h, w, 4))
-    _mk[:, :, :3] = np.asarray(image)
-    _mk[:, :, 3] = 255
-    _mk = (_mk * mask).astype(np.uint8)
-
-    return mask, Image.fromarray(_mk, mode='RGBA')
+    return mask, istack((image, mask))
```

### Comparing `dghs-imgutils-0.0.1/imgutils/tagging/deepdanbooru.py` & `dghs-imgutils-0.0.2/imgutils/tagging/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.1/imgutils/tagging/format.py` & `dghs-imgutils-0.0.2/imgutils/tagging/format.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.1/imgutils/tagging/wd14.py` & `dghs-imgutils-0.0.2/imgutils/tagging/wd14.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.1/imgutils/utils/onnxruntime.py` & `dghs-imgutils-0.0.2/imgutils/utils/onnxruntime.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Overview:
+    Management of onnx models.
+"""
 import logging
 import os
 import shutil
 from typing import Optional
 
 from hbutils.system import pip_install
 
@@ -30,14 +34,23 @@
 alias = {
     'gpu': "CUDAExecutionProvider",
     "trt": "TensorrtExecutionProvider",
 }
 
 
 def get_onnx_provider(provider: Optional[str] = None):
+    """
+    Overview:
+        Get onnx provider.
+
+    :param provider: The provider for ONNX runtime. ``None`` by default and will automatically detect
+        if the ``CUDAExecutionProvider`` is available. If it is available, it will be used,
+        otherwise the default ``CPUExecutionProvider`` will be used.
+    :return: String of the provider.
+    """
     if not provider:
         if "CUDAExecutionProvider" in get_available_providers():
             return "CUDAExecutionProvider"
         else:
             return "CPUExecutionProvider"
     elif provider.lower() in alias:
         return alias[provider.lower()]
@@ -57,8 +70,23 @@
         options.intra_op_num_threads = os.cpu_count()
 
     logging.info(f'Model {ckpt!r} loaded with provider {provider!r}')
     return InferenceSession(ckpt, options, [provider])
 
 
 def open_onnx_model(ckpt: str, mode: str = None) -> InferenceSession:
+    """
+    Overview:
+        Open an ONNX model and load its ONNX runtime.
+
+    :param ckpt: ONNX model file.
+    :param mode: Provider of the ONNX. Default is ``None`` which means the provider will be auto-detected,
+        see :func:`get_onnx_provider` for more details.
+    :return: A loaded ONNX runtime object.
+
+    .. note::
+        When ``mode`` is set to ``None``, it will attempt to detect the environment variable ``ONNX_MODE``.
+        This means you can decide which ONNX runtime to use by setting the environment variable. For example,
+        on Linux, executing ``export ONNX_MODE=cpu`` will ignore any existing CUDA and force the model inference
+        to run on CPU.
+    """
     return _open_onnx_model(ckpt, get_onnx_provider(mode or os.environ.get('ONNX_MODE', None)))
```

### Comparing `dghs-imgutils-0.0.1/imgutils/validate/color.py` & `dghs-imgutils-0.0.2/imgutils/validate/color.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.1/imgutils/validate/monochrome.py` & `dghs-imgutils-0.0.2/imgutils/validate/monochrome.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.1/imgutils/validate/truncate.py` & `dghs-imgutils-0.0.2/imgutils/validate/truncate.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.1/setup.py` & `dghs-imgutils-0.0.2/setup.py`

 * *Files identical despite different names*

