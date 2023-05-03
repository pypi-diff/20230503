# Comparing `tmp/napari-sam-0.4.1.tar.gz` & `tmp/napari-sam-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-sam-0.4.1.tar", last modified: Wed May  3 11:41:15 2023, max compression
+gzip compressed data, was "napari-sam-0.4.2.tar", last modified: Wed May  3 12:06:36 2023, max compression
```

## Comparing `napari-sam-0.4.1.tar` & `napari-sam-0.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:41:15.240217 napari-sam-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-03 11:40:57.000000 napari-sam-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-03 11:40:57.000000 napari-sam-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-05-03 11:41:15.240217 napari-sam-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-03 11:40:57.000000 napari-sam-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-03 11:40:57.000000 napari-sam-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-03 11:41:15.240217 napari-sam-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:41:15.236217 napari-sam-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:41:15.240217 napari-sam-0.4.1/src/napari_sam/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-03 11:40:57.000000 napari-sam-0.4.1/src/napari_sam/QCollapsibleBox.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-03 11:40:57.000000 napari-sam-0.4.1/src/napari_sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61011 2023-05-03 11:40:57.000000 napari-sam-0.4.1/src/napari_sam/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-03 11:40:57.000000 napari-sam-0.4.1/src/napari_sam/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-03 11:40:57.000000 napari-sam-0.4.1/src/napari_sam/slicer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-03 11:40:57.000000 napari-sam-0.4.1/src/napari_sam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:41:15.240217 napari-sam-0.4.1/src/napari_sam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-05-03 11:41:15.000000 napari-sam-0.4.1/src/napari_sam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-03 11:41:15.000000 napari-sam-0.4.1/src/napari_sam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 11:41:15.000000 napari-sam-0.4.1/src/napari_sam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 11:41:15.000000 napari-sam-0.4.1/src/napari_sam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-03 11:41:15.000000 napari-sam-0.4.1/src/napari_sam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 11:41:15.000000 napari-sam-0.4.1/src/napari_sam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:06:36.282719 napari-sam-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-03 12:06:16.000000 napari-sam-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-03 12:06:16.000000 napari-sam-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-05-03 12:06:36.282719 napari-sam-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-03 12:06:16.000000 napari-sam-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-03 12:06:16.000000 napari-sam-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-03 12:06:36.282719 napari-sam-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:06:36.278720 napari-sam-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:06:36.278720 napari-sam-0.4.2/src/napari_sam/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-03 12:06:16.000000 napari-sam-0.4.2/src/napari_sam/QCollapsibleBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-03 12:06:16.000000 napari-sam-0.4.2/src/napari_sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61551 2023-05-03 12:06:16.000000 napari-sam-0.4.2/src/napari_sam/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-03 12:06:16.000000 napari-sam-0.4.2/src/napari_sam/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-03 12:06:16.000000 napari-sam-0.4.2/src/napari_sam/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-03 12:06:16.000000 napari-sam-0.4.2/src/napari_sam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:06:36.282719 napari-sam-0.4.2/src/napari_sam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-05-03 12:06:36.000000 napari-sam-0.4.2/src/napari_sam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-03 12:06:36.000000 napari-sam-0.4.2/src/napari_sam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:06:36.000000 napari-sam-0.4.2/src/napari_sam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 12:06:36.000000 napari-sam-0.4.2/src/napari_sam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-03 12:06:36.000000 napari-sam-0.4.2/src/napari_sam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 12:06:36.000000 napari-sam-0.4.2/src/napari_sam.egg-info/top_level.txt
```

### Comparing `napari-sam-0.4.1/LICENSE` & `napari-sam-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.1/PKG-INFO` & `napari-sam-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.4.1
+Version: 0.4.2
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-sam Version: 0.4.1 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.4.2 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
```

### Comparing `napari-sam-0.4.1/README.md` & `napari-sam-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.1/setup.cfg` & `napari-sam-0.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.1/src/napari_sam/QCollapsibleBox.py` & `napari-sam-0.4.2/src/napari_sam/QCollapsibleBox.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.1/src/napari_sam/_widget.py` & `napari-sam-0.4.2/src/napari_sam/_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from qtpy.QtWidgets import QVBoxLayout, QPushButton, QWidget, QLabel, QComboBox, QRadioButton, QGroupBox, QProgressBar, QApplication, QScrollArea, QLineEdit, QSpacerItem, QSizePolicy
+from qtpy.QtWidgets import QVBoxLayout, QPushButton, QWidget, QLabel, QComboBox, QRadioButton, QGroupBox, QProgressBar, QApplication, QScrollArea, QLineEdit, QCheckBox
 from qtpy.QtGui import QIntValidator, QDoubleValidator
 # from napari_sam.QCollapsibleBox import QCollapsibleBox
 from qtpy import QtCore
 from qtpy.QtCore import Qt
 import napari
 import numpy as np
 from enum import Enum
@@ -174,14 +174,19 @@
         main_layout.addWidget(self.btn_activate)
 
         self.btn_mode_switch = QPushButton("Switch to BBox Mode")
         self.btn_mode_switch.clicked.connect(self._switch_mode)
         self.btn_mode_switch.setEnabled(False)
         main_layout.addWidget(self.btn_mode_switch)
 
+        self.check_prev_mask = QCheckBox('Use previous SAM prediction (recommended)')
+        self.check_prev_mask.setEnabled(False)
+        self.check_prev_mask.setChecked(True)
+        main_layout.addWidget(self.check_prev_mask)
+
         container_widget_info = QWidget()
         container_layout_info = QVBoxLayout(container_widget_info)
 
         self.g_info_tooltip = QGroupBox("Tooltip Information")
         self.l_info_tooltip = QVBoxLayout()
         self.label_info_tooltip = QLabel("Every mode shows further information when hovered over.")
         self.label_info_tooltip.setWordWrap(True)
@@ -579,14 +584,15 @@
                 self.is_active = True
                 self.btn_activate.setText("Deactivate")
                 self.btn_load_model.setEnabled(False)
                 self.cb_model_type.setEnabled(False)
                 self.cb_image_layers.setEnabled(False)
                 self.cb_label_layers.setEnabled(False)
                 self.btn_mode_switch.setEnabled(True)
+                self.check_prev_mask.setEnabled(True)
                 self.btn_mode_switch.setText("Switch to BBox Mode")
                 self.annotator_mode = AnnotatorMode.CLICK
                 selected_layer = None
                 if self.viewer.layers.selection.active != self.points_layer:
                     selected_layer = self.viewer.layers.selection.active
                 self.bbox_layer = self.viewer.add_shapes(name=self.bbox_layer_name)
                 if selected_layer is not None:
@@ -649,14 +655,15 @@
         self.btn_activate.setText("Activate")
         self.btn_load_model.setEnabled(True)
         self.cb_model_type.setEnabled(True)
         self.cb_image_layers.setEnabled(True)
         self.cb_label_layers.setEnabled(True)
         self.btn_mode_switch.setEnabled(False)
         self.btn_mode_switch.setText("Switch to BBox Mode")
+        self.check_prev_mask.setEnabled(False)
         self.prev_segmentation_mode = SegmentationMode.SEMANTIC
         self.annotator_mode = AnnotatorMode.CLICK
         self.remove_all_widget_callbacks(self.viewer)
         if self.label_layer is not None:
             self.remove_all_widget_callbacks(self.label_layer)
         if self.points_layer is not None and self.points_layer in self.viewer.layers:
             self.viewer.layers.remove(self.points_layer)
@@ -936,37 +943,43 @@
             if bbox is not None:
                 # bbox = [np.flip(bbox[0, ...]), np.flip(bbox[2, ...])]
                 top_left_coord, bottom_right_coord = self.find_corners(bbox)
                 bbox = [np.flip(top_left_coord), np.flip(bottom_right_coord)]
                 # bbox = [bottom_right_coord, top_left_coord]
                 bbox = np.asarray(bbox).flatten()
                 # crop = self.image_layer.data[slicer(self.image_layer.data, [[top_left_coord[0], bottom_right_coord[0]], [top_left_coord[1], bottom_right_coord[1]]])]
+            logits = self.sam_logits
+            if not self.check_prev_mask.isChecked():
+                logits = None
             self.sam_predictor.features = self.sam_features
             prediction, _, self.sam_logits = self.sam_predictor.predict(
                 point_coords=points,
                 point_labels=labels,
                 box=bbox,
-                mask_input=self.sam_logits,
+                mask_input=logits,
                 multimask_output=False,
             )
             prediction = prediction[0]
         elif self.image_layer.ndim == 3:
             points = np.asarray(points)
             x_coords = np.unique(points[:, 0])
             groups = {x_coord: list(points[points[:, 0] == x_coord]) for x_coord in x_coords}  # Group points if they are on the same image slice
             prediction = np.zeros_like(self.label_layer.data)
 
             group_points = groups[x_coord]
             group_labels = [labels[np.argwhere(np.all(points == point, axis=1)).flatten()[0]] for point in group_points]
             group_points = [point[1:] for point in group_points]
             self.sam_predictor.features = self.sam_features[x_coord]
+            logits = self.sam_logits[x_coord]
+            if not self.check_prev_mask.isChecked():
+                logits = None
             prediction_yz, _, self.sam_logits[x_coord] = self.sam_predictor.predict(
                 point_coords=np.flip(group_points, axis=-1),
                 point_labels=np.asarray(group_labels),
-                mask_input=self.sam_logits[x_coord],
+                mask_input=logits,
                 multimask_output=False,
             )
             prediction_yz = prediction_yz[0]
             prediction[x_coord, :, :] = prediction_yz
         else:
             raise RuntimeError("Only 2D and 3D images are supported.")
         return prediction
```

### Comparing `napari-sam-0.4.1/src/napari_sam/slicer.py` & `napari-sam-0.4.2/src/napari_sam/slicer.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.1/src/napari_sam/utils.py` & `napari-sam-0.4.2/src/napari_sam/utils.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.1/src/napari_sam.egg-info/PKG-INFO` & `napari-sam-0.4.2/src/napari_sam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.4.1
+Version: 0.4.2
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-sam Version: 0.4.1 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.4.2 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
```

