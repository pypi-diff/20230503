# Comparing `tmp/manga-ocr-abang-0.1.8.tar.gz` & `tmp/manga-ocr-abang-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manga-ocr-abang-0.1.8.tar", last modified: Wed May  3 06:55:10 2023, max compression
+gzip compressed data, was "manga-ocr-abang-0.1.9.tar", last modified: Wed May  3 09:16:53 2023, max compression
```

## Comparing `manga-ocr-abang-0.1.8.tar` & `manga-ocr-abang-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 06:55:10.773552 manga-ocr-abang-0.1.8/
--rw-rw-rw-   0        0        0    11558 2023-05-03 06:33:32.000000 manga-ocr-abang-0.1.8/LICENSE
--rw-rw-rw-   0        0        0       28 2023-05-03 06:33:32.000000 manga-ocr-abang-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0      570 2023-05-03 06:55:10.773552 manga-ocr-abang-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-05-03 06:55:03.000000 manga-ocr-abang-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 06:55:10.734427 manga-ocr-abang-0.1.8/assets/
--rw-rw-rw-   0        0        0    56623 2023-05-03 06:33:32.000000 manga-ocr-abang-0.1.8/assets/example.jpg
-drwxrwxrwx   0        0        0        0 2023-05-03 06:55:10.750949 manga-ocr-abang-0.1.8/manga_ocr/
--rw-rw-rw-   0        0        0       61 2023-05-03 06:33:32.000000 manga-ocr-abang-0.1.8/manga_ocr/__init__.py
--rw-rw-rw-   0        0        0      127 2023-05-03 06:33:32.000000 manga-ocr-abang-0.1.8/manga_ocr/__main__.py
--rw-rw-rw-   0        0        0     2161 2023-05-03 06:33:32.000000 manga-ocr-abang-0.1.8/manga_ocr/ocr.py
--rw-rw-rw-   0        0        0     3947 2023-05-03 06:36:33.000000 manga-ocr-abang-0.1.8/manga_ocr/run.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:55:10.769559 manga-ocr-abang-0.1.8/manga_ocr_abang.egg-info/
--rw-rw-rw-   0        0        0      570 2023-05-03 06:55:10.000000 manga-ocr-abang-0.1.8/manga_ocr_abang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2023-05-03 06:55:10.000000 manga-ocr-abang-0.1.8/manga_ocr_abang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 06:55:10.000000 manga-ocr-abang-0.1.8/manga_ocr_abang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-05-03 06:55:10.000000 manga-ocr-abang-0.1.8/manga_ocr_abang.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      108 2023-05-03 06:55:10.000000 manga-ocr-abang-0.1.8/manga_ocr_abang.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-03 06:55:10.000000 manga-ocr-abang-0.1.8/manga_ocr_abang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 06:55:10.774552 manga-ocr-abang-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1062 2023-05-03 06:55:04.000000 manga-ocr-abang-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:55:10.771552 manga-ocr-abang-0.1.8/tests/
--rw-rw-rw-   0        0        0      424 2023-05-03 06:33:32.000000 manga-ocr-abang-0.1.8/tests/test_ocr.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:16:53.572686 manga-ocr-abang-0.1.9/
+-rw-rw-rw-   0        0        0    11558 2023-05-03 09:13:36.000000 manga-ocr-abang-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       28 2023-05-03 09:13:36.000000 manga-ocr-abang-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      570 2023-05-03 09:16:53.572686 manga-ocr-abang-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-05-03 09:13:36.000000 manga-ocr-abang-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 09:16:53.552620 manga-ocr-abang-0.1.9/assets/
+-rw-rw-rw-   0        0        0    56623 2023-05-03 09:13:36.000000 manga-ocr-abang-0.1.9/assets/example.jpg
+drwxrwxrwx   0        0        0        0 2023-05-03 09:16:53.555974 manga-ocr-abang-0.1.9/manga_ocr/
+-rw-rw-rw-   0        0        0       61 2023-05-03 09:13:36.000000 manga-ocr-abang-0.1.9/manga_ocr/__init__.py
+-rw-rw-rw-   0        0        0      127 2023-05-03 09:13:36.000000 manga-ocr-abang-0.1.9/manga_ocr/__main__.py
+-rw-rw-rw-   0        0        0     2161 2023-05-03 09:13:36.000000 manga-ocr-abang-0.1.9/manga_ocr/ocr.py
+-rw-rw-rw-   0        0        0     3947 2023-05-03 09:13:36.000000 manga-ocr-abang-0.1.9/manga_ocr/run.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:16:53.569686 manga-ocr-abang-0.1.9/manga_ocr_abang.egg-info/
+-rw-rw-rw-   0        0        0      570 2023-05-03 09:16:53.000000 manga-ocr-abang-0.1.9/manga_ocr_abang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2023-05-03 09:16:53.000000 manga-ocr-abang-0.1.9/manga_ocr_abang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 09:16:53.000000 manga-ocr-abang-0.1.9/manga_ocr_abang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-05-03 09:16:53.000000 manga-ocr-abang-0.1.9/manga_ocr_abang.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      108 2023-05-03 09:16:53.000000 manga-ocr-abang-0.1.9/manga_ocr_abang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-03 09:16:53.000000 manga-ocr-abang-0.1.9/manga_ocr_abang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 09:16:53.573751 manga-ocr-abang-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1068 2023-05-03 09:16:45.000000 manga-ocr-abang-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:16:53.570685 manga-ocr-abang-0.1.9/tests/
+-rw-rw-rw-   0        0        0      424 2023-05-03 09:13:36.000000 manga-ocr-abang-0.1.9/tests/test_ocr.py
```

### Comparing `manga-ocr-abang-0.1.8/LICENSE` & `manga-ocr-abang-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `manga-ocr-abang-0.1.8/PKG-INFO` & `manga-ocr-abang-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manga-ocr-abang
-Version: 0.1.8
+Version: 0.1.9
 Summary: OCR for Japanese manga
 Home-page: https://github.com/AbangTanYiHan/manga-ocr-abang
 Author: Maciej Budyś
 Author-email: shinichiconan1997@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `manga-ocr-abang-0.1.8/assets/example.jpg` & `manga-ocr-abang-0.1.9/assets/example.jpg`

 * *Files identical despite different names*

### Comparing `manga-ocr-abang-0.1.8/manga_ocr/ocr.py` & `manga-ocr-abang-0.1.9/manga_ocr/ocr.py`

 * *Files identical despite different names*

### Comparing `manga-ocr-abang-0.1.8/manga_ocr/run.py` & `manga-ocr-abang-0.1.9/manga_ocr/run.py`

 * *Files identical despite different names*

### Comparing `manga-ocr-abang-0.1.8/manga_ocr_abang.egg-info/PKG-INFO` & `manga-ocr-abang-0.1.9/manga_ocr_abang.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manga-ocr-abang
-Version: 0.1.8
+Version: 0.1.9
 Summary: OCR for Japanese manga
 Home-page: https://github.com/AbangTanYiHan/manga-ocr-abang
 Author: Maciej Budyś
 Author-email: shinichiconan1997@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `manga-ocr-abang-0.1.8/setup.py` & `manga-ocr-abang-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from setuptools import setup
 
 long_description = (Path(__file__).parent / "README.md").read_text('utf-8').split('# Installation')[0]
 
 setup(
     name="manga-ocr-abang",
-    version='0.1.8',
+    version='0.1.9',
     description="OCR for Japanese manga",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AbangTanYiHan/manga-ocr-abang",
     author="Maciej Budyś",
     author_email="shinichiconan1997@gmail.com",
     license="Apache License 2.0",
@@ -29,11 +29,11 @@
         "sentencepiece",
         "torch>=1.0",
         "transformers>=4.12.5",
         "unidic_lite",
     ],
     entry_points={
         "console_scripts": [
-            "manga_ocr=manga_ocr.__main__:main",
+            "manga_ocr_abang=manga_ocr.__main__:main",
         ]
     },
 )
```

