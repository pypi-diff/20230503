# Comparing `tmp/napari-sam-0.4.2.tar.gz` & `tmp/napari-sam-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-sam-0.4.2.tar", last modified: Wed May  3 12:06:36 2023, max compression
+gzip compressed data, was "napari-sam-0.4.3.tar", last modified: Wed May  3 15:39:32 2023, max compression
```

## Comparing `napari-sam-0.4.2.tar` & `napari-sam-0.4.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:06:36.282719 napari-sam-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-03 12:06:16.000000 napari-sam-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-03 12:06:16.000000 napari-sam-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-05-03 12:06:36.282719 napari-sam-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-03 12:06:16.000000 napari-sam-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-03 12:06:16.000000 napari-sam-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-03 12:06:36.282719 napari-sam-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:06:36.278720 napari-sam-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:06:36.278720 napari-sam-0.4.2/src/napari_sam/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-03 12:06:16.000000 napari-sam-0.4.2/src/napari_sam/QCollapsibleBox.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-03 12:06:16.000000 napari-sam-0.4.2/src/napari_sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61551 2023-05-03 12:06:16.000000 napari-sam-0.4.2/src/napari_sam/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-03 12:06:16.000000 napari-sam-0.4.2/src/napari_sam/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-03 12:06:16.000000 napari-sam-0.4.2/src/napari_sam/slicer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-03 12:06:16.000000 napari-sam-0.4.2/src/napari_sam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:06:36.282719 napari-sam-0.4.2/src/napari_sam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-05-03 12:06:36.000000 napari-sam-0.4.2/src/napari_sam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-03 12:06:36.000000 napari-sam-0.4.2/src/napari_sam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:06:36.000000 napari-sam-0.4.2/src/napari_sam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 12:06:36.000000 napari-sam-0.4.2/src/napari_sam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-03 12:06:36.000000 napari-sam-0.4.2/src/napari_sam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 12:06:36.000000 napari-sam-0.4.2/src/napari_sam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:39:32.114305 napari-sam-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-03 15:39:11.000000 napari-sam-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-03 15:39:11.000000 napari-sam-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-05-03 15:39:32.114305 napari-sam-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-03 15:39:11.000000 napari-sam-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-03 15:39:11.000000 napari-sam-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-03 15:39:32.114305 napari-sam-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:39:32.106305 napari-sam-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:39:32.110305 napari-sam-0.4.3/src/napari_sam/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-03 15:39:11.000000 napari-sam-0.4.3/src/napari_sam/QCollapsibleBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-03 15:39:11.000000 napari-sam-0.4.3/src/napari_sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64129 2023-05-03 15:39:11.000000 napari-sam-0.4.3/src/napari_sam/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-03 15:39:11.000000 napari-sam-0.4.3/src/napari_sam/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-03 15:39:11.000000 napari-sam-0.4.3/src/napari_sam/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-03 15:39:11.000000 napari-sam-0.4.3/src/napari_sam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:39:32.114305 napari-sam-0.4.3/src/napari_sam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-05-03 15:39:32.000000 napari-sam-0.4.3/src/napari_sam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-03 15:39:32.000000 napari-sam-0.4.3/src/napari_sam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:39:32.000000 napari-sam-0.4.3/src/napari_sam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 15:39:32.000000 napari-sam-0.4.3/src/napari_sam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-03 15:39:32.000000 napari-sam-0.4.3/src/napari_sam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 15:39:32.000000 napari-sam-0.4.3/src/napari_sam.egg-info/top_level.txt
```

### Comparing `napari-sam-0.4.2/LICENSE` & `napari-sam-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.2/PKG-INFO` & `napari-sam-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.4.2
+Version: 0.4.3
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
-Metadata-Version: 2.1 Name: napari-sam Version: 0.4.2 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.4.3 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
```

### Comparing `napari-sam-0.4.2/README.md` & `napari-sam-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.2/setup.cfg` & `napari-sam-0.4.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.2/src/napari_sam/QCollapsibleBox.py` & `napari-sam-0.4.3/src/napari_sam/QCollapsibleBox.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.2/src/napari_sam/_widget.py` & `napari-sam-0.4.3/src/napari_sam/_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -182,14 +182,37 @@
         self.check_prev_mask.setEnabled(False)
         self.check_prev_mask.setChecked(True)
         main_layout.addWidget(self.check_prev_mask)
 
         container_widget_info = QWidget()
         container_layout_info = QVBoxLayout(container_widget_info)
 
+        self.g_size = QGroupBox("Point && Bounding Box Settings")
+        self.l_size = QVBoxLayout()
+
+        l_point_size = QLabel("Point Size:")
+        self.l_size.addWidget(l_point_size)
+        validator = QIntValidator()
+        validator.setRange(0, 9999)
+        self.le_point_size = QLineEdit()
+        self.le_point_size.setText("1")
+        self.le_point_size.setValidator(validator)
+        self.l_size.addWidget(self.le_point_size)
+
+        l_bbox_edge_width = QLabel("Bounding Box Edge Width:")
+        self.l_size.addWidget(l_bbox_edge_width)
+        validator = QIntValidator()
+        validator.setRange(0, 9999)
+        self.le_bbox_edge_width = QLineEdit()
+        self.le_bbox_edge_width.setText("1")
+        self.le_bbox_edge_width.setValidator(validator)
+        self.l_size.addWidget(self.le_bbox_edge_width)
+        self.g_size.setLayout(self.l_size)
+        container_layout_info.addWidget(self.g_size)
+
         self.g_info_tooltip = QGroupBox("Tooltip Information")
         self.l_info_tooltip = QVBoxLayout()
         self.label_info_tooltip = QLabel("Every mode shows further information when hovered over.")
         self.label_info_tooltip.setWordWrap(True)
         self.l_info_tooltip.addWidget(self.label_info_tooltip)
         self.g_info_tooltip.setLayout(self.l_info_tooltip)
         container_layout_info.addWidget(self.g_info_tooltip)
@@ -232,28 +255,31 @@
         self.label_layer = None
         self.label_layer_changes = None
         self.label_color_mapping = None
         self.points_layer = None
         self.points_layer_name = "Ignore this layer1"  # "Ignore this layer <hidden>"
         self.old_points = np.zeros(0)
         self.point_size = 10
+        self.le_point_size.setText(str(self.point_size))
         self.bbox_layer = None
         self.bbox_layer_name = "Ignore this layer2"
+        self.bbox_edge_width = 10
+        self.le_bbox_edge_width.setText(str(self.bbox_edge_width))
 
         self.init_comboboxes()
 
         self.sam_model = None
         self.sam_predictor = None
         self.sam_logits = None
         self.sam_features = None
 
         self.points = defaultdict(list)
         self.point_label = None
 
-        self.bboxes = {}
+        self.bboxes = defaultdict(list)
 
         # self.viewer.window.qt_viewer.layers.model().filterAcceptsRow = self._myfilter
 
     def init_auto_mode_settings(self):
         container_widget_auto = QWidget()
         container_layout_auto = QVBoxLayout(container_widget_auto)
 
@@ -593,18 +619,32 @@
                 self.annotator_mode = AnnotatorMode.CLICK
                 selected_layer = None
                 if self.viewer.layers.selection.active != self.points_layer:
                     selected_layer = self.viewer.layers.selection.active
                 self.bbox_layer = self.viewer.add_shapes(name=self.bbox_layer_name)
                 if selected_layer is not None:
                     self.viewer.layers.selection.active = selected_layer
+                if self.image_layer.ndim == 3:
+                    # This tries to fix the problem that the first drawn bbox is not visible. Fix does not really work though...
+                    self.update_bbox_layer({}, bbox_tmp=[[self.viewer.dims.current_step[0], 0, 0], [self.viewer.dims.current_step[0], 0, 10], [self.viewer.dims.current_step[0], 10, 10], [self.viewer.dims.current_step[0], 10, 0]])
                 self.bbox_layer.editable = False
                 self.bbox_first_coords = None
                 self.prev_segmentation_mode = SegmentationMode.SEMANTIC
 
+                if self.image_layer.ndim == 2:
+                    self.point_size = int(np.min(self.image_layer.data.shape[:2]) / 100)
+                    if self.point_size == 0:
+                        self.point_size = 1
+                    self.bbox_edge_width = 10
+                else:
+                    self.point_size = 2
+                    self.bbox_edge_width = 1
+                self.le_point_size.setText(str(self.point_size))
+                self.le_bbox_edge_width.setText(str(self.bbox_edge_width))
+
             if self.rb_semantic.isChecked():
                 self.segmentation_mode = SegmentationMode.SEMANTIC
                 # self.rb_instance.setEnabled(False)
                 # self.rb_instance.setStyleSheet("color: gray")
             elif self.rb_instance.isChecked():
                 self.segmentation_mode = SegmentationMode.INSTANCE
                 # self.rb_semantic.setEnabled(False)
@@ -674,15 +714,15 @@
         self.label_layer = None
         self.label_layer_changes = None
         self.points_layer = None
         self.bbox_layer = None
         self.bbox_first_coords = None
         self.annotator_mode = AnnotatorMode.NONE
         self.points = defaultdict(list)
-        self.bboxes = {}
+        self.bboxes = defaultdict(list)
         self.point_label = None
         self.sam_logits = None
         self.rb_click.setEnabled(True)
         self.rb_auto.setEnabled(True)
         self.rb_click.setStyleSheet("")
         self.rb_auto.setStyleSheet("")
         self.rb_semantic.setEnabled(True)
@@ -889,37 +929,37 @@
             if not (self.image_layer.ndim == 2 or self.image_layer.ndim == 3):
                 raise RuntimeError("Only 2D and 3D images are supported.")
             self.bbox_first_coords = coords
         elif bbox_state == BboxState.DRAG:
             if self.image_layer.ndim == 2:
                 bbox_tmp = np.asarray([self.bbox_first_coords, (self.bbox_first_coords[0], coords[1]), coords, (coords[0], self.bbox_first_coords[1])])
             elif self.image_layer.ndim == 3:
-                raise RuntimeError("3D images for bbox mode are not supported.")
+                bbox_tmp = np.asarray([self.bbox_first_coords, (self.bbox_first_coords[0], self.bbox_first_coords[1], coords[2]), coords, (self.bbox_first_coords[0], coords[1], self.bbox_first_coords[2])])
             else:
                 raise RuntimeError("Only 2D and 3D images are supported.")
             bbox_tmp = np.rint(bbox_tmp).astype(np.int32)
             self.update_bbox_layer(self.bboxes, bbox_tmp=bbox_tmp)
         else:
             self._save_history({"mode": AnnotatorMode.BBOX, "points": copy.deepcopy(self.points), "bboxes": copy.deepcopy(self.bboxes), "logits": self.sam_logits, "point_label": self.point_label})
             if self.image_layer.ndim == 2:
+                x_coord = slice(None, None)
                 bbox_final = np.asarray([self.bbox_first_coords, (self.bbox_first_coords[0], coords[1]), coords, (coords[0], self.bbox_first_coords[1])])
+                new_label = np.max(self.label_layer.data) + 1
+                self.label_layer.selected_label = new_label
             elif self.image_layer.ndim == 3:
-                raise RuntimeError("3D images for bbox mode are not supported.")
+                x_coord = self.bbox_first_coords[0]
+                bbox_final = np.asarray([self.bbox_first_coords, (self.bbox_first_coords[0], self.bbox_first_coords[1], coords[2]), coords, (self.bbox_first_coords[0], coords[1], self.bbox_first_coords[2])])
+                new_label = self.label_layer.selected_label
             else:
                 raise RuntimeError("Only 2D and 3D images are supported.")
             bbox_final = np.rint(bbox_final).astype(np.int32)
-            new_label = np.max(self.label_layer.data) + 1
-            self.label_layer.selected_label = new_label
-            self.bboxes[new_label] = bbox_final
+            self.bboxes[new_label].append(bbox_final)
             self.update_bbox_layer(self.bboxes)
 
-            prediction = self.predict_sam(points=None, labels=None, bbox=copy.deepcopy(bbox_final))
-
-            # if self.image_layer.ndim == 2:
-            #     x_coord = slice(None, None)
+            prediction = self.predict_sam(points=None, labels=None, bbox=copy.deepcopy(bbox_final), x_coord=x_coord)
 
             label_layer = np.asarray(self.label_layer.data)
             changed_indices = np.where(prediction == 1)
             index_labels_old = label_layer[changed_indices]
             # label_layer[x_coord][label_layer[x_coord] == point_label] = 0
             label_layer[(prediction == 1) & (label_layer == 0)] = new_label
             index_labels_new = label_layer[changed_indices]
@@ -927,58 +967,64 @@
             self.label_layer.data = label_layer
             self.old_points = copy.deepcopy(self.points_layer.data)
             # self.label_layer.refresh()
             with warnings.catch_warnings():
                 warnings.filterwarnings("ignore", category=FutureWarning)
                 self.label_layer._save_history((self.label_layer_changes["indices"], self.label_layer_changes["old_values"], self.label_layer_changes["new_values"]))
 
-            # Update the label here too. This way the label stays incremented when switching to click mode
-            new_label = np.max(self.label_layer.data) + 1
-            self.label_layer.selected_label = new_label
+            if self.image_layer.ndim == 2:
+                # Update the label here too. This way the label stays incremented when switching to click mode
+                new_label = np.max(self.label_layer.data) + 1
+                self.label_layer.selected_label = new_label
 
     def predict_sam(self, points, labels, bbox, x_coord=None):
         if self.image_layer.ndim == 2:
             if points is not None:
                 points = np.flip(points, axis=-1)
                 labels = np.asarray(labels)
             if bbox is not None:
-                # bbox = [np.flip(bbox[0, ...]), np.flip(bbox[2, ...])]
                 top_left_coord, bottom_right_coord = self.find_corners(bbox)
                 bbox = [np.flip(top_left_coord), np.flip(bottom_right_coord)]
-                # bbox = [bottom_right_coord, top_left_coord]
                 bbox = np.asarray(bbox).flatten()
-                # crop = self.image_layer.data[slicer(self.image_layer.data, [[top_left_coord[0], bottom_right_coord[0]], [top_left_coord[1], bottom_right_coord[1]]])]
             logits = self.sam_logits
             if not self.check_prev_mask.isChecked():
                 logits = None
             self.sam_predictor.features = self.sam_features
             prediction, _, self.sam_logits = self.sam_predictor.predict(
                 point_coords=points,
                 point_labels=labels,
                 box=bbox,
                 mask_input=logits,
                 multimask_output=False,
             )
             prediction = prediction[0]
         elif self.image_layer.ndim == 3:
-            points = np.asarray(points)
-            x_coords = np.unique(points[:, 0])
-            groups = {x_coord: list(points[points[:, 0] == x_coord]) for x_coord in x_coords}  # Group points if they are on the same image slice
             prediction = np.zeros_like(self.label_layer.data)
-
-            group_points = groups[x_coord]
-            group_labels = [labels[np.argwhere(np.all(points == point, axis=1)).flatten()[0]] for point in group_points]
-            group_points = [point[1:] for point in group_points]
+            if points is not None:
+                points = np.asarray(points)
+                x_coords = np.unique(points[:, 0])
+                groups = {x_coord: list(points[points[:, 0] == x_coord]) for x_coord in x_coords}  # Group points if they are on the same image slice
+                group_points = groups[x_coord]
+                group_labels = [labels[np.argwhere(np.all(points == point, axis=1)).flatten()[0]] for point in group_points]
+                group_points = [point[1:] for point in group_points]
+                points = np.flip(group_points, axis=-1)
+                labels = np.asarray(group_labels)
+            if bbox is not None:
+                bbox = bbox[:, 1:]
+                top_left_coord, bottom_right_coord = self.find_corners(bbox)
+                bbox = [np.flip(top_left_coord), np.flip(bottom_right_coord)]
+                bbox = np.asarray(bbox).flatten()
             self.sam_predictor.features = self.sam_features[x_coord]
             logits = self.sam_logits[x_coord]
             if not self.check_prev_mask.isChecked():
                 logits = None
             prediction_yz, _, self.sam_logits[x_coord] = self.sam_predictor.predict(
-                point_coords=np.flip(group_points, axis=-1),
-                point_labels=np.asarray(group_labels),
+                point_coords=points,
+                point_labels=labels,
+                box=bbox,
                 mask_input=logits,
                 multimask_output=False,
             )
             prediction_yz = prediction_yz[0]
             prediction[x_coord, :, :] = prediction_yz
         else:
             raise RuntimeError("Only 2D and 3D images are supported.")
@@ -1046,14 +1092,15 @@
                             new_next_slice[next_slice == next_label] = next_label
                     else:
                         new_next_slice[next_slice == next_label] = next_label
                 prediction[i+1] = new_next_slice
         return prediction
 
     def update_points_layer(self, points):
+        self.point_size = int(self.le_point_size.text())
         selected_layer = None
         if self.viewer.layers.selection.active != self.points_layer:
             selected_layer = self.viewer.layers.selection.active
         if self.points_layer is not None:
             self.viewer.layers.remove(self.points_layer)
 
         points_flattened = []
@@ -1061,37 +1108,35 @@
         if points is not None:
             for label, label_points in points.items():
                 points_flattened.extend(label_points)
                 color = self.label_color_mapping["label_mapping"][label]
                 colors = [color] * len(label_points)
                 colors_flattended.extend(colors)
 
-        self.point_size = int(np.min(self.image_layer.data.shape[:2]) / 100)
-        if self.point_size == 0:
-            self.point_size = 1
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=UserWarning)
             self.points_layer = self.viewer.add_points(name=self.points_layer_name, data=np.asarray(points_flattened), face_color=colors_flattended, edge_color="white", size=self.point_size)
         self.points_layer.editable = False
 
         if selected_layer is not None:
             self.viewer.layers.selection.active = selected_layer
         self.points_layer.refresh()
 
     def update_bbox_layer(self, bboxes, bbox_tmp=None):
+        self.bbox_edge_width = int(self.le_bbox_edge_width.text())
         bboxes_flattened = []
         edge_colors = []
         for _, bbox in bboxes.items():
-            bboxes_flattened.append(bbox)
-            edge_colors.append('skyblue')
+            bboxes_flattened.extend(bbox)
+            edge_colors.extend(['skyblue'] * len(bbox))
         if bbox_tmp is not None:
             bboxes_flattened.append(bbox_tmp)
             edge_colors.append('steelblue')
         self.bbox_layer.data = bboxes_flattened
-        self.bbox_layer.edge_width = [10] * len(bboxes_flattened)
+        self.bbox_layer.edge_width = [self.bbox_edge_width] * len(bboxes_flattened)
         self.bbox_layer.edge_color = edge_colors
         self.bbox_layer.face_color = [(0, 0, 0, 0)] * len(bboxes_flattened)
 
     def find_changed_point(self, old_points, new_points):
         if len(new_points) == 0:
             old_point = old_points
         else:
```

### Comparing `napari-sam-0.4.2/src/napari_sam/slicer.py` & `napari-sam-0.4.3/src/napari_sam/slicer.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.2/src/napari_sam/utils.py` & `napari-sam-0.4.3/src/napari_sam/utils.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.2/src/napari_sam.egg-info/PKG-INFO` & `napari-sam-0.4.3/src/napari_sam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.4.2
+Version: 0.4.3
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
-Metadata-Version: 2.1 Name: napari-sam Version: 0.4.2 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.4.3 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
```

