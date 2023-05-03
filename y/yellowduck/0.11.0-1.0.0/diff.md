# Comparing `tmp/yellowduck-0.11.0.tar.gz` & `tmp/yellowduck-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\_GIT\yellowduck-dev\dist\tmpzgbisoqm\yellowduck-0.11.0.tar", last modified: Wed May 19 11:37:06 2021, max compression
+gzip compressed data, was "yellowduck-1.0.0.tar", last modified: Wed May  3 14:13:55 2023, max compression
```

## Comparing `yellowduck-0.11.0.tar` & `yellowduck-1.0.0.tar`

### file list

```diff
@@ -1,72 +1,27 @@
-drwxrwxrwx   0        0        0        0 2021-05-19 11:37:06.797488 yellowduck-0.11.0/
--rw-rw-rw-   0        0        0     1931 2020-10-07 10:08:12.000000 yellowduck-0.11.0/.gitignore
--rw-rw-rw-   0        0        0     1102 2020-10-16 10:28:36.000000 yellowduck-0.11.0/LICENSE
--rw-rw-rw-   0        0        0     2600 2021-05-19 11:37:06.796492 yellowduck-0.11.0/PKG-INFO
--rw-rw-rw-   0        0        0     1705 2021-05-19 04:57:04.000000 yellowduck-0.11.0/README.md
-drwxrwxrwx   0        0        0        0 2021-05-19 11:37:06.135815 yellowduck-0.11.0/_archive/
--rw-rw-rw-   0        0        0     4865 2020-10-16 10:29:19.000000 yellowduck-0.11.0/_archive/yellowduck-0.0.1-py3-none-any.whl
--rw-rw-rw-   0        0        0  3972468 2020-10-16 10:29:18.000000 yellowduck-0.11.0/_archive/yellowduck-0.0.1.tar.gz
-drwxrwxrwx   0        0        0        0 2021-05-19 11:37:06.145775 yellowduck-0.11.0/_dev/
--rw-rw-rw-   0        0        0     1931 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/.gitignore
-drwxrwxrwx   0        0        0        0 2021-05-19 11:37:06.200236 yellowduck-0.11.0/_dev/images/
--rw-rw-rw-   0        0        0     1931 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/.gitignore
--rw-rw-rw-   0        0        0  2790449 2021-04-20 07:36:03.000000 yellowduck-0.11.0/_dev/images/duplicate_images.ipynb
-drwxrwxrwx   0        0        0        0 2021-05-19 11:37:06.737489 yellowduck-0.11.0/_dev/images/image_data/
--rw-rw-rw-   0        0        0   116770 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/a.jpg
--rw-rw-rw-   0        0        0   172079 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/b.jpg
--rw-rw-rw-   0        0        0   119580 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/c.jpg
--rw-rw-rw-   0        0        0   146747 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/d.jpg
--rw-rw-rw-   0        0        0   112876 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/e.jpg
--rw-rw-rw-   0        0        0   140538 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/f.jpg
--rw-rw-rw-   0        0        0    66120 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/g.jpg
--rw-rw-rw-   0        0        0   287193 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/h.jpg
--rw-rw-rw-   0        0        0   163896 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/i.jpg
--rw-rw-rw-   0        0        0    84170 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/j.jpg
--rw-rw-rw-   0        0        0    88928 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/k.jpg
--rw-rw-rw-   0        0        0   107632 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/l.jpg
--rw-rw-rw-   0        0        0   170381 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/m.jpg
--rw-rw-rw-   0        0        0   134468 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/n.jpg
--rw-rw-rw-   0        0        0   105104 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/o.jpg
--rw-rw-rw-   0        0        0   112920 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/p.jpg
--rw-rw-rw-   0        0        0   140182 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/q.jpg
--rw-rw-rw-   0        0        0   140182 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/q_copy1.jpg
--rw-rw-rw-   0        0        0   140182 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/q_copy2.jpg
--rw-rw-rw-   0        0        0   150597 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/r.jpg
--rw-rw-rw-   0        0        0   150597 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/r_copy.jpg
--rw-rw-rw-   0        0        0    85869 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/s.jpg
--rw-rw-rw-   0        0        0    85869 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/s_copy.jpg
--rw-rw-rw-   0        0        0   113425 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/t.jpg
--rw-rw-rw-   0        0        0   132001 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/u.jpg
--rw-rw-rw-   0        0        0    84497 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/v.jpg
--rw-rw-rw-   0        0        0   158491 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/w.jpg
--rw-rw-rw-   0        0        0   164623 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/x.jpg
--rw-rw-rw-   0        0        0   179502 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/x_edit1.jpg
--rw-rw-rw-   0        0        0   164425 2020-10-07 10:08:12.000000 yellowduck-0.11.0/_dev/images/image_data/x_edit2.jpg
--rw-rw-rw-   0        0        0       42 2021-05-19 11:37:06.797488 yellowduck-0.11.0/setup.cfg
--rw-rw-rw-   0        0        0      683 2021-05-19 11:34:18.000000 yellowduck-0.11.0/setup.py
-drwxrwxrwx   0        0        0        0 2021-05-19 11:37:06.738487 yellowduck-0.11.0/yellowduck/
--rw-rw-rw-   0        0        0      164 2020-10-16 10:33:28.000000 yellowduck-0.11.0/yellowduck/__init__.py
-drwxrwxrwx   0        0        0        0 2021-05-19 11:37:06.762493 yellowduck-0.11.0/yellowduck/explore/
--rw-rw-rw-   0        0        0        0 2020-10-07 10:08:12.000000 yellowduck-0.11.0/yellowduck/explore/__init__.py
-drwxrwxrwx   0        0        0        0 2021-05-19 11:37:06.763490 yellowduck-0.11.0/yellowduck/hypothesis/
--rw-rw-rw-   0        0        0        0 2020-10-07 10:08:12.000000 yellowduck-0.11.0/yellowduck/hypothesis/__init__.py
-drwxrwxrwx   0        0        0        0 2021-05-19 11:37:06.767524 yellowduck-0.11.0/yellowduck/preprocessing/
--rw-rw-rw-   0        0        0        0 2021-04-19 04:28:09.000000 yellowduck-0.11.0/yellowduck/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     9229 2021-04-20 07:19:59.000000 yellowduck-0.11.0/yellowduck/preprocessing/image.py
--rw-rw-rw-   0        0        0     3310 2021-04-20 07:36:08.000000 yellowduck-0.11.0/yellowduck/preprocessing/text.py
-drwxrwxrwx   0        0        0        0 2021-05-19 11:37:06.769488 yellowduck-0.11.0/yellowduck/report/
--rw-rw-rw-   0        0        0      164 2020-10-16 10:33:28.000000 yellowduck-0.11.0/yellowduck/report/__init__.py
--rw-rw-rw-   0        0        0    13270 2021-04-20 09:28:35.000000 yellowduck-0.11.0/yellowduck/report/tabular.py
-drwxrwxrwx   0        0        0        0 2021-05-19 11:37:06.790488 yellowduck-0.11.0/yellowduck/timeseries/
--rw-rw-rw-   0        0        0        0 2021-05-17 11:08:29.000000 yellowduck-0.11.0/yellowduck/timeseries/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-17 11:08:53.000000 yellowduck-0.11.0/yellowduck/timeseries/dtw_clustering.py
-drwxrwxrwx   0        0        0        0 2021-05-19 11:37:06.794515 yellowduck-0.11.0/yellowduck/tools/
--rw-rw-rw-   0        0        0        0 2020-10-07 10:08:12.000000 yellowduck-0.11.0/yellowduck/tools/__init__.py
--rw-rw-rw-   0        0        0      804 2021-05-19 11:29:58.000000 yellowduck-0.11.0/yellowduck/tools/thai_id_card.py
-drwxrwxrwx   0        0        0        0 2021-05-19 11:37:06.795492 yellowduck-0.11.0/yellowduck/util/
--rw-rw-rw-   0        0        0        0 2021-04-19 04:24:56.000000 yellowduck-0.11.0/yellowduck/util/__init__.py
-drwxrwxrwx   0        0        0        0 2021-05-19 11:37:06.760490 yellowduck-0.11.0/yellowduck.egg-info/
--rw-rw-rw-   0        0        0     2600 2021-05-19 11:37:05.000000 yellowduck-0.11.0/yellowduck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1642 2021-05-19 11:37:06.000000 yellowduck-0.11.0/yellowduck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-19 11:37:05.000000 yellowduck-0.11.0/yellowduck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2021-05-19 11:37:05.000000 yellowduck-0.11.0/yellowduck.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:13:55.058091 yellowduck-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-03 14:13:40.000000 yellowduck-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-03 14:13:55.058091 yellowduck-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-03 14:13:40.000000 yellowduck-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-03 14:13:55.058091 yellowduck-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-03 14:13:40.000000 yellowduck-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:13:55.054091 yellowduck-1.0.0/yellowduck/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-03 14:13:40.000000 yellowduck-1.0.0/yellowduck/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:13:55.054091 yellowduck-1.0.0/yellowduck/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:13:40.000000 yellowduck-1.0.0/yellowduck/etc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-03 14:13:40.000000 yellowduck-1.0.0/yellowduck/etc/id_card_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:13:55.058091 yellowduck-1.0.0/yellowduck/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:13:40.000000 yellowduck-1.0.0/yellowduck/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9466 2023-05-03 14:13:40.000000 yellowduck-1.0.0/yellowduck/image/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:13:40.000000 yellowduck-1.0.0/yellowduck/image/similarity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:13:55.058091 yellowduck-1.0.0/yellowduck/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:13:40.000000 yellowduck-1.0.0/yellowduck/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:13:40.000000 yellowduck-1.0.0/yellowduck/text/cleansing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-05-03 14:13:40.000000 yellowduck-1.0.0/yellowduck/text/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:13:55.058091 yellowduck-1.0.0/yellowduck/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:13:40.000000 yellowduck-1.0.0/yellowduck/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:13:55.054091 yellowduck-1.0.0/yellowduck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-03 14:13:55.000000 yellowduck-1.0.0/yellowduck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-03 14:13:55.000000 yellowduck-1.0.0/yellowduck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 14:13:55.000000 yellowduck-1.0.0/yellowduck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-03 14:13:55.000000 yellowduck-1.0.0/yellowduck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 14:13:55.000000 yellowduck-1.0.0/yellowduck.egg-info/top_level.txt
```

### Comparing `yellowduck-0.11.0/LICENSE` & `yellowduck-1.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2020 Chalat Phumphiraratthaya
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2020 Chalat Phumphiraratthaya
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `yellowduck-0.11.0/README.md` & `yellowduck-1.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,57 @@
-# yellowduck
-
-
-[![PyPI Latest Release](https://img.shields.io/pypi/v/yellowduck?style=for-the-badge)](https://pypi.org/project/yellowduck/)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/yellowduck?style=for-the-badge)
-![GitHub](https://img.shields.io/github/license/PCP55/yellowduck-dev?style=for-the-badge)
-![GitHub last commit](https://img.shields.io/github/last-commit/PCP55/yellowduck-dev?style=for-the-badge)
-![GitHub repo size](https://img.shields.io/github/repo-size/PCP55/yellowduck-dev?style=for-the-badge)
-![Lines of code](https://img.shields.io/tokei/lines/github/PCP55/yellowduck-dev?style=for-the-badge)
-
-## What is it?
-
-**yellowduck** is the data science toolbox for everyone. To be precise, for the lazy man like me!
-
-Actually, **yellowduck** is like a sandbox library for me. If I found something great I will surely add it in **yellowduck**. 
-
-## Main Features
-
-- Check duplicate image
-- Visualize duplicate image from above
-- Clean Text
-
-In addition, you can see the next features [https://github.com/PCP55/yellowduck-dev/projects/1](here)!
-
-## Example
-
-Please go to this [Link](https://github.com/PCP55/yellowduck-dev/tree/main/_dev)
-
-## Prerequisites (from A to Z)
-
-- hashlib
-- imagehash
-- matplotlib
-- numpy
-- os
-- pillow
-- re
-
-## Install
-
-```ruby
-# PyPI
-pip install yellowduck
-```
-
-## Found Issues
-
-Create New Issue [here](https://github.com/PCP55/yellowduck-dev/issues) and I will fix it as soon as I have a free time. (LOL)
-
----------------------------------------
-
-> This library inspired by [kora](https://github.com/airesearch-in-th/kora/tree/master/kora), A collection of tools to make programming on Google Colab easier.
+# yellowduck
+
+[![PyPI Latest Release](https://img.shields.io/pypi/v/yellowduck?style=for-the-badge)](https://pypi.org/project/yellowduck/)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/yellowduck?style=for-the-badge)
+![GitHub](https://img.shields.io/github/license/PCP55/yellowduck-dev?style=for-the-badge)
+![GitHub last commit](https://img.shields.io/github/last-commit/PCP55/yellowduck-dev?style=for-the-badge)
+![GitHub repo size](https://img.shields.io/github/repo-size/PCP55/yellowduck-dev?style=for-the-badge)
+![Lines of code](https://img.shields.io/tokei/lines/github/PCP55/yellowduck-dev?style=for-the-badge)
+
+## What is it?
+
+**yellowduck** is the data science toolbox for everyone. To be precise, for the lazy man like me!
+
+Actually, **yellowduck** is like a sandbox library for me. If I found something great I will surely add it in **yellowduck**. 
+
+## Main Features
+
+- Check duplicate image and visualize it!
+- Clean text
+
+## Example
+
+Please go to this [Link](https://github.com/PCP55/yellowduck-dev/tree/main/examples)
+
+
+## Install
+
+You have to specify functions you want to use:
+If you need full option of `yellowduck`, you can install it by using:
+
+```ruby
+# PyPI
+
+pip install "yellowduck[full]==x.x.x"
+```
+
+However, if you need to use only text's functions or image's function, you will need:
+
+```ruby
+# PyPI
+
+pip install "yellowduck[text]==x.x.x"
+
+# or
+
+pip install "yellowduck[image]==x.x.x"
+
+# accordingly
+```
+
+## Found Issues
+
+Create New Issue [here](https://github.com/PCP55/yellowduck-dev/issues) and I will fix it as soon as I have a free time. (LOL)
+
+---------------------------------------
+
+> This library was inspired by [kora](https://github.com/airesearch-in-th/kora/tree/master/kora), A collection of tools to make programming on Google Colab easier.
```

### Comparing `yellowduck-0.11.0/yellowduck/preprocessing/image.py` & `yellowduck-1.0.0/yellowduck/image/image.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,195 +1,233 @@
-"""Check duplicate image within same folder.
-
-There are 2 approachs.
-1. exact match:     Using Cryptographic hashing algorithms in 'hashlib'
-2. similar match:   Using Perceptual hashing algorithms in 'imagehash' 
-                    and use Hamming distance for finding differrence.
-"""
-
-import os
-import PIL
-import hashlib
-import imagehash
-import numpy as np
-import matplotlib.pyplot as plt
-
-class ImageDuplicate():
-    def __init__(self, image_folder_path: str):
-        try: # For development phase only
-            get_ipython
-            self.current_path = os.getcwd()
-        except: # For production
-            self.current_path = os.path.dirname(os.path.realpath(__file__))
-        self.current_path = os.path.join(self.current_path, image_folder_path)
-
-        self.image_in_folder_list = [file for file in os.listdir(self.current_path) if (file.endswith('.png')) | (file.endswith('.jpg'))]
-        self.image_path_list = [os.path.join(self.current_path,image) for image in self.image_in_folder_list]
-        self.hash_value_list = []
-
-        self.similar_group_dict = {} # Group of image separate by hash value
-        self.non_duplicate_list = [] # Select 1 image in each group
-        self.duplicate_list = [] # The rest that not be selected in non_duplicate_list
-
-    def find_exact(self):
-        print(f'Using method: Exact Match (MD5)')
-
-        for image_file in self.image_in_folder_list:
-            image_fullpath = os.path.join(self.current_path,image_file)
-            with open(image_fullpath, 'rb') as f:
-                hash_value = hashlib.md5(f.read()).hexdigest()
-            self.hash_value_list.append(hash_value)
-
-        fast_check_duplicate = len(set(self.hash_value_list)) - len(self.hash_value_list)
-        if fast_check_duplicate == 0:
-            print('There is no duplicate image here.')
-            return
-        else:
-            for image_name, hash_value in zip(self.image_in_folder_list,self.hash_value_list):
-                if hash_value not in self.similar_group_dict:
-                    self.similar_group_dict[hash_value] = [image_name]
-                    self.non_duplicate_list.append(image_name)
-                else:
-                    self.similar_group_dict[hash_value] += [image_name]
-                    self.duplicate_list.append(image_name)
-                
-            temp_similar_group_dict = self.similar_group_dict.copy()
-            for (key,value) in temp_similar_group_dict.items():
-                if len(value) == 1:
-                    self.similar_group_dict.pop(key)
-
-        group_key = list(np.arange(len(self.similar_group_dict)))
-        self.similar_group_dict = dict(zip(group_key,list(self.similar_group_dict.values())))
-
-        num_duplicate = len(self.duplicate_list)
-        num_all = len(self.image_in_folder_list)
-        percentage = np.round(num_duplicate/num_all * 100, 2)
-        print(f'There are {num_duplicate} duplicated images out of {num_all} which is around {percentage} %.')
-
-        return self.similar_group_dict, self.duplicate_list, self.non_duplicate_list
-
-    def find_similar(self, hash_method:str='phash', distance:int=2, hash_size:int=16):
-        print(f'Using method: {hash_method}\nAn accepted distance: {distance}\nHashing size: {hash_size}')
-
-        for image_file in self.image_in_folder_list:
-            image_fullpath = os.path.join(self.current_path,image_file)
-            image = PIL.Image.open(image_fullpath)
-            if hash_method == 'phash':
-                hash_value = imagehash.phash(image, hash_size)
-            elif hash_method == 'ahash':
-                hash_value = imagehash.average_hash(image, hash_size)
-            elif hash_method == 'dhash':
-                hash_value = imagehash.dhash(image, hash_size)
-            elif hash_method == 'whash':
-                hash_value = imagehash.whash(image, hash_size)
-            elif hash_method == 'crop_resistant_hash':
-                """
-                - No hashing size
-                - Take too much time!! (as another hash algorithm use 250 ms but this one take 1 min for test dataset)
-                """
-                hash_value = imagehash.crop_resistant_hash(image)
-            else:
-                print('There are 4 methods here which is phash, ahash, dhash, whash')
-            self.hash_value_list.append(hash_value)
-
-        # It is recommend to use distance = 0 for time reduction.
-
-        if distance == 0:
-            fast_check_duplicate = len(set(self.hash_value_list)) - len(self.hash_value_list)
-            if fast_check_duplicate == 0:
-                print('There is no duplicate image here.')
-                return
-            else:
-                for image_name, hash_value in zip(self.image_in_folder_list,self.hash_value_list):
-                    if hash_value not in self.similar_group_dict:
-                        self.similar_group_dict[hash_value] = [image_name]
-                        self.non_duplicate_list.append(image_name)
-                    else:
-                        self.similar_group_dict[hash_value] += [image_name]
-                        self.duplicate_list.append(image_name)
-        else:
-            temp_filename_list = []
-            num = 0
-            filename_hash_dict = dict(zip(self.image_in_folder_list,self.hash_value_list))
-            temp_filename_hash_dict = dict(zip(self.image_in_folder_list,self.hash_value_list))
-            sort_filename_hash_dict = sorted(filename_hash_dict)
-            
-            for file_first in sort_filename_hash_dict:
-                if file_first in temp_filename_hash_dict:
-                
-                    temp_similar_list = []
-                    temp_similar_list.append(file_first)
-                    temp_filename_list.append(file_first)
-                    temp_filename_hash_dict.pop(file_first)
-
-                    image_first = filename_hash_dict[file_first]
-                
-                for file_second in sort_filename_hash_dict:
-                    if file_second not in temp_filename_list:
-                        image_second = filename_hash_dict[file_second]
-                        hamming_distance = image_first - image_second
-                        
-                        if hamming_distance <= distance:
-                            temp_similar_list.append(file_second)
-                            temp_filename_list.append(file_second)
-
-                if len(temp_similar_list) > 1:
-                    self.similar_group_dict[num] = temp_similar_list
-
-                    for _item in temp_similar_list[1:]:
-                        self.duplicate_list.append(_item)
-
-                    num = num + 1
-
-            self.non_duplicate_list = [image for image in self.image_in_folder_list if image not in self.duplicate_list]
-
-        return self.similar_group_dict, self.duplicate_list, self.non_duplicate_list
-
-        num_duplicate = len(self.duplicate_list)
-        num_all = len(self.image_in_folder_list)
-        percentage = np.round(num_duplicate/num_all * 100, 2)
-
-        print(f'There are {num_duplicate} duplicated images out of {num_all} which is around {percentage} %.')
-
-
-class ShowImageDuplicate():
-    def __init__(self, image_folder_path, group_of_duplicate_dict:dict):
-        self.image_folder_path = image_folder_path
-        self.group_of_duplicate_dict = group_of_duplicate_dict
-
-        self.number_of_group = len(self.group_of_duplicate_dict)
-        print(f'There are {self.number_of_group} of duplicate image.\nUse .show_group(group_number) or .show_all() for all group.')
-    def show_all(self):
-        """
-        Show only first 5 images in each group
-        """
-        fig, axes = plt.subplots(nrows=self.number_of_group, ncols=5, figsize=(24, 24))
-        for axis in axes.ravel():
-            axis.set_axis_off()
-        for group_number in np.arange(self.number_of_group):
-            image_list = self.group_of_duplicate_dict[group_number]
-            if len(image_list) > 5:
-                image_list = image_list[:5]
-            for image_number in np.arange(len(image_list)):
-                image_path = os.path.join(self.image_folder_path,image_list[image_number])
-                image = PIL.Image.open(image_path)
-                axes[group_number,image_number].imshow(image)
-        plt.tight_layout()
-
-    def show_group(self, group_number):
-        image_list = self.group_of_duplicate_dict[group_number]
-        if len(image_list) < 5:
-            num_col = len(image_list)
-        else:
-            num_col = 5
-        num_row = int(len(image_list)/num_col)
-        mod = len(image_list)%num_col
-        if mod != 0:
-            num_row = num_row + 1
-        fig, axes = plt.subplots(nrows=num_row, ncols=num_col, figsize=(24, 10))
-        for axis in axes.ravel():
-            axis.set_axis_off()
-        for index, image_name in enumerate(image_list):
-            image_path = os.path.join(self.image_folder_path,image_name)
-            image = PIL.Image.open(image_path)
-            axes.ravel()[index].imshow(image)
-        plt.tight_layout()
+"""Check duplicate image within same folder.
+
+There are 2 approachs.
+1. exact match:     Using Cryptographic hashing algorithms in 'hashlib'
+2. similar match:   Using Perceptual hashing algorithms in 'imagehash' 
+                    and use Hamming distance for finding differrence.
+"""
+
+import os
+import PIL
+import hashlib
+import imagehash
+import numpy as np
+import matplotlib.pyplot as plt
+
+
+class ImageDuplicate:
+    def __init__(self, image_folder_path: str):
+        try:  # For development phase only
+            get_ipython
+            self.current_path = os.getcwd()
+        except:  # For production
+            self.current_path = os.path.dirname(os.path.realpath(__file__))
+        self.current_path = os.path.join(self.current_path, image_folder_path)
+
+        self.image_in_folder_list = [
+            file
+            for file in os.listdir(self.current_path)
+            if (file.endswith(".png")) | (file.endswith(".jpg"))
+        ]
+        self.image_path_list = [
+            os.path.join(self.current_path, image)
+            for image in self.image_in_folder_list
+        ]
+        self.hash_value_list = []
+
+        self.similar_group_dict = {}  # Group of image separate by hash value
+        self.non_duplicate_list = []  # Select 1 image in each group
+        self.duplicate_list = []  # The rest that not be selected in non_duplicate_list
+
+    def find_exact(self):
+        print(f"Using method: Exact Match (MD5)")
+
+        for image_file in self.image_in_folder_list:
+            image_fullpath = os.path.join(self.current_path, image_file)
+            with open(image_fullpath, "rb") as f:
+                hash_value = hashlib.md5(f.read()).hexdigest()
+            self.hash_value_list.append(hash_value)
+
+        fast_check_duplicate = len(set(self.hash_value_list)) - len(
+            self.hash_value_list
+        )
+        if fast_check_duplicate == 0:
+            print("There is no duplicate image here.")
+            return
+        else:
+            for image_name, hash_value in zip(
+                self.image_in_folder_list, self.hash_value_list
+            ):
+                if hash_value not in self.similar_group_dict:
+                    self.similar_group_dict[hash_value] = [image_name]
+                    self.non_duplicate_list.append(image_name)
+                else:
+                    self.similar_group_dict[hash_value] += [image_name]
+                    self.duplicate_list.append(image_name)
+
+            temp_similar_group_dict = self.similar_group_dict.copy()
+            for key, value in temp_similar_group_dict.items():
+                if len(value) == 1:
+                    self.similar_group_dict.pop(key)
+
+        group_key = list(np.arange(len(self.similar_group_dict)))
+        self.similar_group_dict = dict(
+            zip(group_key, list(self.similar_group_dict.values()))
+        )
+
+        num_duplicate = len(self.duplicate_list)
+        num_all = len(self.image_in_folder_list)
+        percentage = np.round(num_duplicate / num_all * 100, 2)
+        print(
+            f"There are {num_duplicate} duplicated images out of {num_all} which is around {percentage} %."
+        )
+
+        return self.similar_group_dict, self.duplicate_list, self.non_duplicate_list
+
+    def find_similar(
+        self, hash_method: str = "phash", distance: int = 2, hash_size: int = 16
+    ):
+        print(
+            f"Using method: {hash_method}\nAn accepted distance: {distance}\nHashing size: {hash_size}"
+        )
+
+        for image_file in self.image_in_folder_list:
+            image_fullpath = os.path.join(self.current_path, image_file)
+            image = PIL.Image.open(image_fullpath)
+            if hash_method == "phash":
+                hash_value = imagehash.phash(image, hash_size)
+            elif hash_method == "ahash":
+                hash_value = imagehash.average_hash(image, hash_size)
+            elif hash_method == "dhash":
+                hash_value = imagehash.dhash(image, hash_size)
+            elif hash_method == "whash":
+                hash_value = imagehash.whash(image, hash_size)
+            elif hash_method == "crop_resistant_hash":
+                """
+                - No hashing size
+                - Take too much time!! (as another hash algorithm use 250 ms but this one take 1 min for test dataset)
+                """
+                hash_value = imagehash.crop_resistant_hash(image)
+            else:
+                print("There are 4 methods here which is phash, ahash, dhash, whash")
+            self.hash_value_list.append(hash_value)
+
+        # It is recommend to use distance = 0 for time reduction.
+
+        if distance == 0:
+            fast_check_duplicate = len(set(self.hash_value_list)) - len(
+                self.hash_value_list
+            )
+            if fast_check_duplicate == 0:
+                print("There is no duplicate image here.")
+                return
+            else:
+                for image_name, hash_value in zip(
+                    self.image_in_folder_list, self.hash_value_list
+                ):
+                    if hash_value not in self.similar_group_dict:
+                        self.similar_group_dict[hash_value] = [image_name]
+                        self.non_duplicate_list.append(image_name)
+                    else:
+                        self.similar_group_dict[hash_value] += [image_name]
+                        self.duplicate_list.append(image_name)
+        else:
+            temp_filename_list = []
+            num = 0
+            filename_hash_dict = dict(
+                zip(self.image_in_folder_list, self.hash_value_list)
+            )
+            temp_filename_hash_dict = dict(
+                zip(self.image_in_folder_list, self.hash_value_list)
+            )
+            sort_filename_hash_dict = sorted(filename_hash_dict)
+
+            for file_first in sort_filename_hash_dict:
+                if file_first in temp_filename_hash_dict:
+                    temp_similar_list = []
+                    temp_similar_list.append(file_first)
+                    temp_filename_list.append(file_first)
+                    temp_filename_hash_dict.pop(file_first)
+
+                    image_first = filename_hash_dict[file_first]
+
+                for file_second in sort_filename_hash_dict:
+                    if file_second not in temp_filename_list:
+                        image_second = filename_hash_dict[file_second]
+                        hamming_distance = image_first - image_second
+
+                        if hamming_distance <= distance:
+                            temp_similar_list.append(file_second)
+                            temp_filename_list.append(file_second)
+
+                if len(temp_similar_list) > 1:
+                    self.similar_group_dict[num] = temp_similar_list
+
+                    for _item in temp_similar_list[1:]:
+                        self.duplicate_list.append(_item)
+
+                    num = num + 1
+
+            self.non_duplicate_list = [
+                image
+                for image in self.image_in_folder_list
+                if image not in self.duplicate_list
+            ]
+
+        return self.similar_group_dict, self.duplicate_list, self.non_duplicate_list
+
+        num_duplicate = len(self.duplicate_list)
+        num_all = len(self.image_in_folder_list)
+        percentage = np.round(num_duplicate / num_all * 100, 2)
+
+        print(
+            f"There are {num_duplicate} duplicated images out of {num_all} which is around {percentage} %."
+        )
+
+
+class ShowImageDuplicate:
+    def __init__(self, image_folder_path, group_of_duplicate_dict: dict):
+        self.image_folder_path = image_folder_path
+        self.group_of_duplicate_dict = group_of_duplicate_dict
+
+        self.number_of_group = len(self.group_of_duplicate_dict)
+        print(
+            f"There are {self.number_of_group} of duplicate image.\nUse .show_group(group_number) or .show_all() for all group."
+        )
+
+    def show_all(self):
+        """
+        Show only first 5 images in each group
+        """
+        fig, axes = plt.subplots(nrows=self.number_of_group, ncols=5, figsize=(24, 24))
+        for axis in axes.ravel():
+            axis.set_axis_off()
+        for group_number in np.arange(self.number_of_group):
+            image_list = self.group_of_duplicate_dict[group_number]
+            if len(image_list) > 5:
+                image_list = image_list[:5]
+            for image_number in np.arange(len(image_list)):
+                image_path = os.path.join(
+                    self.image_folder_path, image_list[image_number]
+                )
+                image = PIL.Image.open(image_path)
+                axes[group_number, image_number].imshow(image)
+        plt.tight_layout()
+
+    def show_group(self, group_number):
+        image_list = self.group_of_duplicate_dict[group_number]
+        if len(image_list) < 5:
+            num_col = len(image_list)
+        else:
+            num_col = 5
+        num_row = int(len(image_list) / num_col)
+        mod = len(image_list) % num_col
+        if mod != 0:
+            num_row = num_row + 1
+        fig, axes = plt.subplots(nrows=num_row, ncols=num_col, figsize=(24, 10))
+        for axis in axes.ravel():
+            axis.set_axis_off()
+        for index, image_name in enumerate(image_list):
+            image_path = os.path.join(self.image_folder_path, image_name)
+            image = PIL.Image.open(image_path)
+            axes.ravel()[index].imshow(image)
+        plt.tight_layout()
```

