# Comparing `tmp/napari-sam-0.4.0.tar.gz` & `tmp/napari-sam-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-sam-0.4.0.tar", last modified: Wed May  3 09:16:15 2023, max compression
+gzip compressed data, was "napari-sam-0.4.1.tar", last modified: Wed May  3 11:41:15 2023, max compression
```

## Comparing `napari-sam-0.4.0.tar` & `napari-sam-0.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:15.273259 napari-sam-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-03 09:15:59.000000 napari-sam-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-03 09:15:59.000000 napari-sam-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-05-03 09:16:15.273259 napari-sam-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-03 09:15:59.000000 napari-sam-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-03 09:15:59.000000 napari-sam-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-03 09:16:15.273259 napari-sam-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:15.269259 napari-sam-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:15.269259 napari-sam-0.4.0/src/napari_sam/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-03 09:15:59.000000 napari-sam-0.4.0/src/napari_sam/QCollapsibleBox.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-03 09:15:59.000000 napari-sam-0.4.0/src/napari_sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57158 2023-05-03 09:15:59.000000 napari-sam-0.4.0/src/napari_sam/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-03 09:15:59.000000 napari-sam-0.4.0/src/napari_sam/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-03 09:15:59.000000 napari-sam-0.4.0/src/napari_sam/slicer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-03 09:15:59.000000 napari-sam-0.4.0/src/napari_sam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:15.273259 napari-sam-0.4.0/src/napari_sam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-05-03 09:16:15.000000 napari-sam-0.4.0/src/napari_sam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-03 09:16:15.000000 napari-sam-0.4.0/src/napari_sam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 09:16:15.000000 napari-sam-0.4.0/src/napari_sam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 09:16:15.000000 napari-sam-0.4.0/src/napari_sam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-03 09:16:15.000000 napari-sam-0.4.0/src/napari_sam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 09:16:15.000000 napari-sam-0.4.0/src/napari_sam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:41:15.240217 napari-sam-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-03 11:40:57.000000 napari-sam-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-03 11:40:57.000000 napari-sam-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-05-03 11:41:15.240217 napari-sam-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-03 11:40:57.000000 napari-sam-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-03 11:40:57.000000 napari-sam-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-03 11:41:15.240217 napari-sam-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:41:15.236217 napari-sam-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:41:15.240217 napari-sam-0.4.1/src/napari_sam/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-03 11:40:57.000000 napari-sam-0.4.1/src/napari_sam/QCollapsibleBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-03 11:40:57.000000 napari-sam-0.4.1/src/napari_sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61011 2023-05-03 11:40:57.000000 napari-sam-0.4.1/src/napari_sam/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-03 11:40:57.000000 napari-sam-0.4.1/src/napari_sam/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-03 11:40:57.000000 napari-sam-0.4.1/src/napari_sam/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-03 11:40:57.000000 napari-sam-0.4.1/src/napari_sam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:41:15.240217 napari-sam-0.4.1/src/napari_sam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-05-03 11:41:15.000000 napari-sam-0.4.1/src/napari_sam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-03 11:41:15.000000 napari-sam-0.4.1/src/napari_sam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 11:41:15.000000 napari-sam-0.4.1/src/napari_sam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 11:41:15.000000 napari-sam-0.4.1/src/napari_sam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-03 11:41:15.000000 napari-sam-0.4.1/src/napari_sam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 11:41:15.000000 napari-sam-0.4.1/src/napari_sam.egg-info/top_level.txt
```

### Comparing `napari-sam-0.4.0/LICENSE` & `napari-sam-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.0/PKG-INFO` & `napari-sam-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.4.0
+Version: 0.4.1
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
-Metadata-Version: 2.1 Name: napari-sam Version: 0.4.0 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.4.1 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
```

### Comparing `napari-sam-0.4.0/README.md` & `napari-sam-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.0/setup.cfg` & `napari-sam-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.0/src/napari_sam/QCollapsibleBox.py` & `napari-sam-0.4.1/src/napari_sam/QCollapsibleBox.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.0/src/napari_sam/_widget.py` & `napari-sam-0.4.1/src/napari_sam/_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,26 @@
 import napari
 import numpy as np
 from enum import Enum
 from collections import deque, defaultdict
 import inspect
 from segment_anything import SamPredictor, sam_model_registry
 from segment_anything.automatic_mask_generator import SamAutomaticMaskGenerator
-from napari_sam.utils import get_weights_path, get_cached_weight_types, normalize
+from napari_sam.utils import normalize
 import torch
 from vispy.util.keys import CONTROL
 import copy
 import warnings
 from tqdm import tqdm
 from superqt.utils import qdebounced
 from napari_sam.slicer import slicer
+import urllib.request
+from pathlib import Path
+import os
+from os.path import join
 
 
 class AnnotatorMode(Enum):
     NONE = 0
     CLICK = 1
     BBOX = 2
     AUTO = 3
@@ -34,14 +38,22 @@
 
 class BboxState(Enum):
     CLICK = 0
     DRAG = 1
     RELEASE = 2
 
 
+SAM_WEIGHTS_URL = {
+    "default": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth",
+    "vit_h": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth",
+    "vit_l": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_l_0b3195.pth",
+    "vit_b": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_b_01ec64.pth",
+}
+
+
 class SamWidget(QWidget):
     def __init__(self, napari_viewer):
         super().__init__()
         self.viewer = napari_viewer
 
         self.annotator_mode = AnnotatorMode.NONE
         self.segmentation_mode = SegmentationMode.SEMANTIC
@@ -68,15 +80,15 @@
 
         self.cb_model_type = QComboBox()
         main_layout.addWidget(self.cb_model_type)
 
         self.btn_load_model = QPushButton("Load model")
         self.btn_load_model.clicked.connect(self._load_model)
         main_layout.addWidget(self.btn_load_model)
-        self.is_model_loaded = False
+        self.loaded_model = None
         self.init_model_type_combobox()
 
         l_image_layer = QLabel("Select input image layer:")
         main_layout.addWidget(l_image_layer)
 
         self.cb_image_layers = QComboBox()
         self.cb_image_layers.addItems(self.get_layer_names("image"))
@@ -393,33 +405,52 @@
         # else:
         #     self.rb_auto.setEnabled(True)
         #     self.rb_auto.setStyleSheet("")
         pass
 
     def init_model_type_combobox(self):
         model_types = list(sam_model_registry.keys())
-        cached_weight_types = get_cached_weight_types(model_types)
-        entries = []
-        for name, is_cached in cached_weight_types.items():
-            if is_cached:
-                entries.append("{} (Cached)".format(name))
-            else:
-                entries.append("{} (Auto-Download)".format(name))
-        self.cb_model_type.addItems(entries)
+        cached_weight_types = self.get_cached_weight_types(model_types)
+        # entries = []
+        # for name, is_cached in cached_weight_types.items():
+        #     if is_cached:
+        #         entries.append("{} (Cached)".format(name))
+        #     else:
+        #         entries.append("{} (Auto-Download)".format(name))
+        # self.cb_model_type.addItems(entries)
+        self.update_model_type_combobox()
 
         if cached_weight_types[list(cached_weight_types.keys())[self.cb_model_type.currentIndex()]]:
             self.btn_load_model.setText("Load model")
         else:
             self.btn_load_model.setText("Download and load model")
 
         self.cb_model_type.currentTextChanged.connect(self.on_model_type_combobox_change)
 
+    def update_model_type_combobox(self):
+        model_types = list(sam_model_registry.keys())
+        cached_weight_types = self.get_cached_weight_types(model_types)
+        entries = []
+        for name, is_cached in cached_weight_types.items():
+            if name == self.loaded_model:
+                entries.append("{} (Loaded)".format(name))
+            elif is_cached:
+                entries.append("{} (Cached)".format(name))
+            else:
+                entries.append("{} (Auto-Download)".format(name))
+        self.cb_model_type.clear()
+        self.cb_model_type.addItems(entries)
+        if self.loaded_model is not None:
+            loaded_model_index = self.cb_model_type.findText("{} (Loaded)".format(self.loaded_model))
+            self.cb_model_type.setCurrentIndex(loaded_model_index)
+
+
     def on_model_type_combobox_change(self):
         model_types = list(sam_model_registry.keys())
-        cached_weight_types = get_cached_weight_types(model_types)
+        cached_weight_types = self.get_cached_weight_types(model_types)
 
         if cached_weight_types[list(cached_weight_types.keys())[self.cb_model_type.currentIndex()]]:
             self.btn_load_model.setText("Load model")
         else:
             self.btn_load_model.setText("Download and load model")
 
     def init_comboboxes(self):
@@ -482,28 +513,33 @@
 
     def _on_layers_changed_callback(self):
         self._check_activate_btn()
         if (self.image_layer is not None and self.image_layer not in self.viewer.layers) or (self.label_layer is not None and self.label_layer not in self.viewer.layers):
             self._deactivate()
 
     def _check_activate_btn(self):
-        if self.cb_image_layers.currentText() != "" and self.cb_label_layers.currentText() != "" and self.is_model_loaded:
+        if self.cb_image_layers.currentText() != "" and self.cb_label_layers.currentText() != "" and self.loaded_model is not None:
             self.btn_activate.setEnabled(True)
         else:
             self.btn_activate.setEnabled(False)
 
     def _load_model(self):
+        self.cb_model_type.setEnabled(False)
+        self.btn_load_model.setEnabled(False)
         model_types = list(sam_model_registry.keys())
         model_type = model_types[self.cb_model_type.currentIndex()]
         self.sam_model = sam_model_registry[model_type](
-            get_weights_path(model_type)
+            self.get_weights_path(model_type)
         )
         self.sam_model.to(self.device)
         self.sam_predictor = SamPredictor(self.sam_model)
-        self.is_model_loaded = True
+        self.loaded_model = model_type
+        self.update_model_type_combobox()
+        self.cb_model_type.setEnabled(True)
+        self.btn_load_model.setEnabled(True)
         self._check_activate_btn()
 
     def _activate(self):
         self.btn_activate.setEnabled(False)
         if not self.is_active:
             self.image_name = self.cb_image_layers.currentText()
             self.image_layer = self.viewer.layers[self.cb_image_layers.currentText()]
@@ -1169,9 +1205,70 @@
 
     def redo(self):
         self._load_history(
             self._redo_history, self._undo_history, undoing=False
         )
         raise RuntimeError("Redo currently not supported.")
 
+    def download_with_progress(self, url, output_file):
+        # Open the URL and get the content length
+        req = urllib.request.urlopen(url)
+        content_length = int(req.headers.get('Content-Length'))
+
+        l_creating_features = QLabel("Downloading model:")
+        self.layout().addWidget(l_creating_features)
+        progress_bar = QProgressBar(self)
+        progress_bar.setMaximum(int(content_length / 1024))
+        progress_bar.setValue(0)
+        self.layout().addWidget(progress_bar)
+
+        # Set up the progress bar
+        progress_bar_tqdm = tqdm(total=content_length, unit='B', unit_scale=True, desc="Downloading model")
+
+        # Download the file and update the progress bar
+        with open(output_file, 'wb') as f:
+            downloaded_bytes = 0
+            while True:
+                buffer = req.read(8192)
+                if not buffer:
+                    break
+                downloaded_bytes += len(buffer)
+                f.write(buffer)
+                progress_bar_tqdm.update(len(buffer))
+                progress_bar.setValue(int(downloaded_bytes / 1024))
+                QApplication.processEvents()
+                progress_bar.deleteLater()
+                l_creating_features.deleteLater()
+
+        # Close the progress bar and the URL
+        progress_bar_tqdm.close()
+        req.close()
+
+    def get_weights_path(self, model_type):
+        weight_url = SAM_WEIGHTS_URL[model_type]
+
+        cache_dir = Path.home() / ".cache/napari-segment-anything"
+        cache_dir.mkdir(parents=True, exist_ok=True)
+
+        weight_path = cache_dir / weight_url.split("/")[-1]
+
+        if not weight_path.exists():
+            print("Downloading {} to {} ...".format(weight_url, weight_path))
+            self.download_with_progress(weight_url, weight_path)
+
+        return weight_path
+
+    def get_cached_weight_types(self, model_types):
+        cached_weight_types = {}
+        cache_dir = str(Path.home() / ".cache/napari-segment-anything")
+
+        for model_type in model_types:
+            model_type_name = os.path.basename(SAM_WEIGHTS_URL[model_type])
+            if os.path.isfile(join(cache_dir, model_type_name)):
+                cached_weight_types[model_type] = True
+            else:
+                cached_weight_types[model_type] = False
+
+        return cached_weight_types
+
     # def _myfilter(self, row, parent):
     #     return "<hidden>" not in self.viewer.layers[row].name
```

### Comparing `napari-sam-0.4.0/src/napari_sam/slicer.py` & `napari-sam-0.4.1/src/napari_sam/slicer.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.0/src/napari_sam/utils.py` & `napari-sam-0.4.1/src/napari_sam/utils.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.0/src/napari_sam.egg-info/PKG-INFO` & `napari-sam-0.4.1/src/napari_sam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.4.0
+Version: 0.4.1
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
-Metadata-Version: 2.1 Name: napari-sam Version: 0.4.0 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.4.1 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
```

