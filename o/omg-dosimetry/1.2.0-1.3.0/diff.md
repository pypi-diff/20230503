# Comparing `tmp/omg_dosimetry-1.2.0.tar.gz` & `tmp/omg_dosimetry-1.3.0.tar.gz`

## Comparing `omg_dosimetry-1.2.0.tar` & `omg_dosimetry-1.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    10880 2020-02-02 00:00:00.000000 omg_dosimetry-1.2.0/requirements.txt
--rw-r--r--   0        0        0    27306 2020-02-02 00:00:00.000000 omg_dosimetry-1.2.0/src/omg_dosimetry/OMG_Logo.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omg_dosimetry-1.2.0/src/omg_dosimetry/__init__.py
--rw-r--r--   0        0        0    42015 2020-02-02 00:00:00.000000 omg_dosimetry-1.2.0/src/omg_dosimetry/analysis.py
--rw-r--r--   0        0        0    37873 2020-02-02 00:00:00.000000 omg_dosimetry-1.2.0/src/omg_dosimetry/calibration.py
--rw-r--r--   0        0        0    41899 2020-02-02 00:00:00.000000 omg_dosimetry-1.2.0/src/omg_dosimetry/imageRGB.py
--rw-r--r--   0        0        0    17012 2020-02-02 00:00:00.000000 omg_dosimetry-1.2.0/src/omg_dosimetry/tiff2dose.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 omg_dosimetry-1.2.0/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 omg_dosimetry-1.2.0/LICENSE
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 omg_dosimetry-1.2.0/README.md
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 omg_dosimetry-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 omg_dosimetry-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10880 2020-02-02 00:00:00.000000 omg_dosimetry-1.3.0/requirements.txt
+-rw-r--r--   0        0        0    27306 2020-02-02 00:00:00.000000 omg_dosimetry-1.3.0/src/omg_dosimetry/OMG_Logo.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omg_dosimetry-1.3.0/src/omg_dosimetry/__init__.py
+-rw-r--r--   0        0        0    42147 2020-02-02 00:00:00.000000 omg_dosimetry-1.3.0/src/omg_dosimetry/analysis.py
+-rw-r--r--   0        0        0    37873 2020-02-02 00:00:00.000000 omg_dosimetry-1.3.0/src/omg_dosimetry/calibration.py
+-rw-r--r--   0        0        0    41899 2020-02-02 00:00:00.000000 omg_dosimetry-1.3.0/src/omg_dosimetry/imageRGB.py
+-rw-r--r--   0        0        0    17012 2020-02-02 00:00:00.000000 omg_dosimetry-1.3.0/src/omg_dosimetry/tiff2dose.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 omg_dosimetry-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 omg_dosimetry-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 omg_dosimetry-1.3.0/README.md
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 omg_dosimetry-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 omg_dosimetry-1.3.0/PKG-INFO
```

### Comparing `omg_dosimetry-1.2.0/requirements.txt` & `omg_dosimetry-1.3.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.2.0/src/omg_dosimetry/OMG_Logo.png` & `omg_dosimetry-1.3.0/src/omg_dosimetry/OMG_Logo.png`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.2.0/src/omg_dosimetry/analysis.py` & `omg_dosimetry-1.3.0/src/omg_dosimetry/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -458,17 +458,18 @@
         self.show_profiles(axes,x=x, y=y)
         plt.gcf().canvas.draw_idle()
         
     def moved_and_pressed(self, event, axes):
         if event.button==1:
             self.set_profile(event, axes)  
         
-    def register(self, shift_x=0, shift_y=0, threshold=10, register_using_gradient=False, markers_center=None):
+    def register(self, shift_x=0, shift_y=0, threshold=10, register_using_gradient=False, markers_center=None, rot=0):
         self.register_using_gradient = register_using_gradient
         self.shifts = [shift_x, shift_y]
+        self.rot = rot
         self.markers_center = markers_center
         if threshold > 0 :
             self.film_dose.crop_edges(threshold=threshold)
         print('Please double-click on each marker. Press ''enter'' when done')
         print('Keyboard shortcuts: Right arrow = Rotate 90 degrees; Left arrow = Flip horizontally; Up arrow = Flip vertically')
         self.film_dose.plot()
         self.select_markers()
@@ -541,14 +542,17 @@
                 self.fig.canvas.mpl_disconnect(self.cid)
                 plt.close(self.fig)
                                 
                 self.move_iso_center()
                 self.remove_rotation()
                 if self.ref_dose is not None:
                     self.apply_shifts_ref()
+                
+                if self.rot:
+                    self.film_dose.rotate(self.rot)
                 self.tune_registration()
                 return
                 
     def move_iso_center(self):
         x, y = [m[0] for m in self.markers], [m[1] for m in self.markers]
         t, b = y.index(min(y)), y.index(max(y))
         l, r = x.index(min(x)), x.index(max(x))
```

### Comparing `omg_dosimetry-1.2.0/src/omg_dosimetry/calibration.py` & `omg_dosimetry-1.3.0/src/omg_dosimetry/calibration.py`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.2.0/src/omg_dosimetry/imageRGB.py` & `omg_dosimetry-1.3.0/src/omg_dosimetry/imageRGB.py`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.2.0/src/omg_dosimetry/tiff2dose.py` & `omg_dosimetry-1.3.0/src/omg_dosimetry/tiff2dose.py`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.2.0/.gitignore` & `omg_dosimetry-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.2.0/LICENSE` & `omg_dosimetry-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.2.0/README.md` & `omg_dosimetry-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.2.0/pyproject.toml` & `omg_dosimetry-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "omg_dosimetry"
-version = "1.2.0"
+version = "1.3.0"
 authors = [
   { name="JF Cabana", email="jean-francois.cabana.cisssca@ssss.gouv.qc.ca" },
 ]
 description = "Optimized Multichannel Gafchromic Dosimetry (OMG Dosimetry)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `omg_dosimetry-1.2.0/PKG-INFO` & `omg_dosimetry-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omg_dosimetry
-Version: 1.2.0
+Version: 1.3.0
 Summary: Optimized Multichannel Gafchromic Dosimetry (OMG Dosimetry)
 Project-URL: Homepage, https://bitbucket.org/cric_levis/omg-film-dosimetry
 Author-email: JF Cabana <jean-francois.cabana.cisssca@ssss.gouv.qc.ca>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

