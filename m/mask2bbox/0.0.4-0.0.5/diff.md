# Comparing `tmp/mask2bbox-0.0.4.tar.gz` & `tmp/mask2bbox-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mask2bbox-0.0.4.tar", last modified: Thu Apr 27 21:20:05 2023, max compression
+gzip compressed data, was "mask2bbox-0.0.5.tar", last modified: Wed May  3 13:29:02 2023, max compression
```

## Comparing `mask2bbox-0.0.4.tar` & `mask2bbox-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:20:05.277513 mask2bbox-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 21:19:54.000000 mask2bbox-0.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-27 21:19:54.000000 mask2bbox-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-27 21:20:05.277513 mask2bbox-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-27 21:19:54.000000 mask2bbox-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 21:20:05.277513 mask2bbox-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-27 21:19:54.000000 mask2bbox-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:20:05.273513 mask2bbox-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:20:05.277513 mask2bbox-0.0.4/src/mask2bbox/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 21:19:54.000000 mask2bbox-0.0.4/src/mask2bbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-27 21:19:54.000000 mask2bbox-0.0.4/src/mask2bbox/_bboxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-27 21:19:54.000000 mask2bbox-0.0.4/src/mask2bbox/mask2bbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:20:05.277513 mask2bbox-0.0.4/src/mask2bbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-27 21:20:05.000000 mask2bbox-0.0.4/src/mask2bbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-27 21:20:05.000000 mask2bbox-0.0.4/src/mask2bbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:20:05.000000 mask2bbox-0.0.4/src/mask2bbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 21:20:05.000000 mask2bbox-0.0.4/src/mask2bbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 21:20:05.000000 mask2bbox-0.0.4/src/mask2bbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:20:05.277513 mask2bbox-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:19:54.000000 mask2bbox-0.0.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:20:05.277513 mask2bbox-0.0.4/tests/test_mask2bbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:19:54.000000 mask2bbox-0.0.4/tests/test_mask2bbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-27 21:19:54.000000 mask2bbox-0.0.4/tests/test_mask2bbox/test_mask2bbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:02.296460 mask2bbox-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-03 13:28:45.000000 mask2bbox-0.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-03 13:28:45.000000 mask2bbox-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-03 13:29:02.292460 mask2bbox-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-03 13:28:45.000000 mask2bbox-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 13:29:02.296460 mask2bbox-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-03 13:28:45.000000 mask2bbox-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:02.292460 mask2bbox-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:02.292460 mask2bbox-0.0.5/src/mask2bbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-03 13:28:45.000000 mask2bbox-0.0.5/src/mask2bbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-05-03 13:28:45.000000 mask2bbox-0.0.5/src/mask2bbox/_bboxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-05-03 13:28:45.000000 mask2bbox-0.0.5/src/mask2bbox/mask2bbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:02.292460 mask2bbox-0.0.5/src/mask2bbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-03 13:29:02.000000 mask2bbox-0.0.5/src/mask2bbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-03 13:29:02.000000 mask2bbox-0.0.5/src/mask2bbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:29:02.000000 mask2bbox-0.0.5/src/mask2bbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-03 13:29:02.000000 mask2bbox-0.0.5/src/mask2bbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 13:29:02.000000 mask2bbox-0.0.5/src/mask2bbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:02.292460 mask2bbox-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:28:45.000000 mask2bbox-0.0.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:02.292460 mask2bbox-0.0.5/tests/test_mask2bbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:28:45.000000 mask2bbox-0.0.5/tests/test_mask2bbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-03 13:28:45.000000 mask2bbox-0.0.5/tests/test_mask2bbox/test_mask2bbox.py
```

### Comparing `mask2bbox-0.0.4/LICENSE.txt` & `mask2bbox-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mask2bbox-0.0.4/PKG-INFO` & `mask2bbox-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mask2bbox
-Version: 0.0.4
+Version: 0.0.5
 Summary: Gets the bounding boxes from a mask file.
 Home-page: https://github.com/SchapiroLabor/mask2bbox
 Author: Miguel Ibarra
 Author-email: c180l058j@mozmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -25,39 +25,63 @@
 
 ## Usage
 
 ```python
 from mask2bbox import BBoxes
 
 # Create a BBoxes object
-all_BBoxes = BBoxes("path/to/mask.png")
+all_boxes = BBoxes("path/to/mask.png")
 
 # Expand the bounding boxes
-all_BBoxes.expand(n=10)
+all_boxes.expand(n=10)
 
 # Remove the bounding boxes that are located on the edge of the image
-all_BBoxes.remove_edge_boxes()
+all_boxes.remove_edge_boxes()
 
 # Get the area of all the bounding boxes
-araa = all_BBoxes.get_bbox_areas()
+araa = all_boxes.get_bbox_areas()
 
 # Get the dimensions on x and y of all the bounding boxes
-dims = all_BBoxes.get_bbox_dims()
-
+dims = all_boxes.get_bbox_dims()
+ 
 # Get the center of all the bounding boxes
-centers = all_BBoxes.get_bbox_centers()
+centers = all_boxes.get_bbox_centers()
 
 # Get the ratio x/y of all the bounding boxes
-ratios = all_BBoxes.get_bbox_ratios()
+ratios = all_boxes.get_bbox_ratios()
+
+# Get the IoU matrix of all the bounding boxes
+iou = all_boxes.get_iou_matrix()
+
+# Save the IoU matrix to a csv file
+all_boxes.save_iou("path/to/save/iou.csv")
+
+# Plot the bounding boxes on the mask image
+all_boxes.plot_to_mask("path/to/save/image.png")
 
 # Save your bounding boxes
-all_BBoxes.save_csv("path/to/bounding_boxes.csv")
+all_boxes.save_csv("path/to/bounding_boxes.csv")
 ```
 
 ## Version Notes
+
+### 0.0.5 - Added functionality
+
+- IoU related operations:
+  - `boxes.get_iou_matrix()` - Gets the IoU of all the bounding boxes.
+  - `boxes.are_overlaping()` - Returns identities where the IoU is greater than 0
+  - `boxes.overlaping_pais()` - Returns the pairs of bounding boxes that are overlaping.
+  - `boxes.save_iou()` - Saves the IoU matrix to a csv file.
+
+- Plots
+  - `boxes.plot_to_mask()` Plots the bounding boxes on the mask image.
+
+#### Example of `boxes.plot_to_mask()` where only the overlaping masks are highlighted.
+![Plot](plot.png) 
+
 ### 0.0.4 - Added functionality
 Now is possible to extract:
 - Bounding boxes dimensions `BBoxes.get_bbox_dims()`
 - Bounding boxes area `BBoxes.get_bbox_areas()`
 - Bounding boxes center `BBoxes.get_bbox_centers()`
 - Bounding boxes ratios `BBoxes.get_bbox_ratios()`
```

### Comparing `mask2bbox-0.0.4/README.md` & `mask2bbox-0.0.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -8,39 +8,63 @@
 
 ## Usage
 
 ```python
 from mask2bbox import BBoxes
 
 # Create a BBoxes object
-all_BBoxes = BBoxes("path/to/mask.png")
+all_boxes = BBoxes("path/to/mask.png")
 
 # Expand the bounding boxes
-all_BBoxes.expand(n=10)
+all_boxes.expand(n=10)
 
 # Remove the bounding boxes that are located on the edge of the image
-all_BBoxes.remove_edge_boxes()
+all_boxes.remove_edge_boxes()
 
 # Get the area of all the bounding boxes
-araa = all_BBoxes.get_bbox_areas()
+araa = all_boxes.get_bbox_areas()
 
 # Get the dimensions on x and y of all the bounding boxes
-dims = all_BBoxes.get_bbox_dims()
-
+dims = all_boxes.get_bbox_dims()
+ 
 # Get the center of all the bounding boxes
-centers = all_BBoxes.get_bbox_centers()
+centers = all_boxes.get_bbox_centers()
 
 # Get the ratio x/y of all the bounding boxes
-ratios = all_BBoxes.get_bbox_ratios()
+ratios = all_boxes.get_bbox_ratios()
+
+# Get the IoU matrix of all the bounding boxes
+iou = all_boxes.get_iou_matrix()
+
+# Save the IoU matrix to a csv file
+all_boxes.save_iou("path/to/save/iou.csv")
+
+# Plot the bounding boxes on the mask image
+all_boxes.plot_to_mask("path/to/save/image.png")
 
 # Save your bounding boxes
-all_BBoxes.save_csv("path/to/bounding_boxes.csv")
+all_boxes.save_csv("path/to/bounding_boxes.csv")
 ```
 
 ## Version Notes
+
+### 0.0.5 - Added functionality
+
+- IoU related operations:
+  - `boxes.get_iou_matrix()` - Gets the IoU of all the bounding boxes.
+  - `boxes.are_overlaping()` - Returns identities where the IoU is greater than 0
+  - `boxes.overlaping_pais()` - Returns the pairs of bounding boxes that are overlaping.
+  - `boxes.save_iou()` - Saves the IoU matrix to a csv file.
+
+- Plots
+  - `boxes.plot_to_mask()` Plots the bounding boxes on the mask image.
+
+#### Example of `boxes.plot_to_mask()` where only the overlaping masks are highlighted.
+![Plot](plot.png) 
+
 ### 0.0.4 - Added functionality
 Now is possible to extract:
 - Bounding boxes dimensions `BBoxes.get_bbox_dims()`
 - Bounding boxes area `BBoxes.get_bbox_areas()`
 - Bounding boxes center `BBoxes.get_bbox_centers()`
 - Bounding boxes ratios `BBoxes.get_bbox_ratios()`
```

### Comparing `mask2bbox-0.0.4/setup.py` & `mask2bbox-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mask2bbox",
-    version="0.0.4",
+    version="0.0.5",
     description="Gets the bounding boxes from a mask file.",
     url="https://github.com/SchapiroLabor/mask2bbox",
     author="Miguel Ibarra",
     author_email="c180l058j@mozmail.com",
     license="MIT",
     classifiers=[
         "Development Status :: 3 - Alpha",
@@ -18,14 +18,15 @@
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires = [
         "numpy",
-        "scikit-image"
+        "scikit-image",
+        "matplotlib",
     ],
     extras_require={
         "dev": ["pytest>=3.7"],
     },
 )
```

### Comparing `mask2bbox-0.0.4/src/mask2bbox.egg-info/PKG-INFO` & `mask2bbox-0.0.5/src/mask2bbox.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mask2bbox
-Version: 0.0.4
+Version: 0.0.5
 Summary: Gets the bounding boxes from a mask file.
 Home-page: https://github.com/SchapiroLabor/mask2bbox
 Author: Miguel Ibarra
 Author-email: c180l058j@mozmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -25,39 +25,63 @@
 
 ## Usage
 
 ```python
 from mask2bbox import BBoxes
 
 # Create a BBoxes object
-all_BBoxes = BBoxes("path/to/mask.png")
+all_boxes = BBoxes("path/to/mask.png")
 
 # Expand the bounding boxes
-all_BBoxes.expand(n=10)
+all_boxes.expand(n=10)
 
 # Remove the bounding boxes that are located on the edge of the image
-all_BBoxes.remove_edge_boxes()
+all_boxes.remove_edge_boxes()
 
 # Get the area of all the bounding boxes
-araa = all_BBoxes.get_bbox_areas()
+araa = all_boxes.get_bbox_areas()
 
 # Get the dimensions on x and y of all the bounding boxes
-dims = all_BBoxes.get_bbox_dims()
-
+dims = all_boxes.get_bbox_dims()
+ 
 # Get the center of all the bounding boxes
-centers = all_BBoxes.get_bbox_centers()
+centers = all_boxes.get_bbox_centers()
 
 # Get the ratio x/y of all the bounding boxes
-ratios = all_BBoxes.get_bbox_ratios()
+ratios = all_boxes.get_bbox_ratios()
+
+# Get the IoU matrix of all the bounding boxes
+iou = all_boxes.get_iou_matrix()
+
+# Save the IoU matrix to a csv file
+all_boxes.save_iou("path/to/save/iou.csv")
+
+# Plot the bounding boxes on the mask image
+all_boxes.plot_to_mask("path/to/save/image.png")
 
 # Save your bounding boxes
-all_BBoxes.save_csv("path/to/bounding_boxes.csv")
+all_boxes.save_csv("path/to/bounding_boxes.csv")
 ```
 
 ## Version Notes
+
+### 0.0.5 - Added functionality
+
+- IoU related operations:
+  - `boxes.get_iou_matrix()` - Gets the IoU of all the bounding boxes.
+  - `boxes.are_overlaping()` - Returns identities where the IoU is greater than 0
+  - `boxes.overlaping_pais()` - Returns the pairs of bounding boxes that are overlaping.
+  - `boxes.save_iou()` - Saves the IoU matrix to a csv file.
+
+- Plots
+  - `boxes.plot_to_mask()` Plots the bounding boxes on the mask image.
+
+#### Example of `boxes.plot_to_mask()` where only the overlaping masks are highlighted.
+![Plot](plot.png) 
+
 ### 0.0.4 - Added functionality
 Now is possible to extract:
 - Bounding boxes dimensions `BBoxes.get_bbox_dims()`
 - Bounding boxes area `BBoxes.get_bbox_areas()`
 - Bounding boxes center `BBoxes.get_bbox_centers()`
 - Bounding boxes ratios `BBoxes.get_bbox_ratios()`
```

