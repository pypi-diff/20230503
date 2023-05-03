# Comparing `tmp/dactim_mri-0.0.4.tar.gz` & `tmp/dactim_mri-0.0.5.tar.gz`

## Comparing `dactim_mri-0.0.4.tar` & `dactim_mri-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 dactim_mri-0.0.4/requirements.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 dactim_mri-0.0.4/src/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dactim_mri-0.0.4/src/dactim_mri/__init__.py
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 dactim_mri-0.0.4/src/dactim_mri/convert.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 dactim_mri-0.0.4/src/dactim_mri/spectro.py
--rw-r--r--   0        0        0    14674 2020-02-02 00:00:00.000000 dactim_mri-0.0.4/src/dactim_mri/transformation.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 dactim_mri-0.0.4/src/dactim_mri/utils.py
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 dactim_mri-0.0.4/src/dactim_mri/visualization.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dactim_mri-0.0.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dactim_mri-0.0.4/README.md
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 dactim_mri-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 dactim_mri-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 dactim_mri-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 dactim_mri-0.0.5/src/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dactim_mri-0.0.5/src/dactim_mri/__init__.py
+-rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 dactim_mri-0.0.5/src/dactim_mri/anonymization.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 dactim_mri-0.0.5/src/dactim_mri/computation.py
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 dactim_mri-0.0.5/src/dactim_mri/conversion.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 dactim_mri-0.0.5/src/dactim_mri/sorting.py
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 dactim_mri-0.0.5/src/dactim_mri/spectroscopy.py
+-rw-r--r--   0        0        0    18605 2020-02-02 00:00:00.000000 dactim_mri-0.0.5/src/dactim_mri/transformation.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 dactim_mri-0.0.5/src/dactim_mri/utils.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 dactim_mri-0.0.5/src/dactim_mri/visualization.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dactim_mri-0.0.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dactim_mri-0.0.5/README.md
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 dactim_mri-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 dactim_mri-0.0.5/PKG-INFO
```

### Comparing `dactim_mri-0.0.4/src/dactim_mri/convert.py` & `dactim_mri-0.0.5/src/dactim_mri/conversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,29 @@
 import numpy as np
 import nibabel as nib
 import os
 import pydicom
 from copy import deepcopy
 import time
+import dicom2nifti
 
+def convert_dicom_to_nifti(dicom_dir, output_dir):
+    """ Convert Dicom folder to Nifti format (@author: abrys)
+
+    Parameters
+    ----------
+    dicom_dir : str
+        Dicom directory to convert
+
+    output_dir : str
+        Nifti file suffixe for the new generated image
+
+    """
+    dicom2nifti.convert_directory(dicom_dir, output_dir)
+    
 class Dicomize():
     """Use a NIFTI file and convert it in DICOM using a folder of DICOM as template.
 
     The DICOM folder must contains the original DICOM used to create the NIFTI
     """
     def __init__(self, dicom_dir, final_dir, nifti_path, series_description, comment="", rgb=False):
         """ 
@@ -63,15 +78,15 @@
             self.final_ds.ContentTime = modification_time
 
             self.final_ds.file_meta.MediaStorageSOPInstanceUID += "." + str(i)
             # SOP Instance UID
             self.final_ds[0x8,0x18].value = str(self.final_ds.file_meta.MediaStorageSOPInstanceUID)
 
             self.final_ds[0x8,0x70].value = "DACTIM-MRI"
-            if rgb is True:
+            if self.rgb is True:
                 self.final_ds[0x28,0x2].value = 3
                 self.final_ds[0x28,0x4].value = "RGB"
                 # self.final_ds[0x28,0x6].value = 0
                 self.final_ds[0x28,0x100].value = 8
                 self.final_ds[0x28,0x101].value = 8
                 self.final_ds[0x28,0x102].value = 7
                 self.final_ds[0x28,0x103].value = 0
```

### Comparing `dactim_mri-0.0.4/src/dactim_mri/spectro.py` & `dactim_mri-0.0.5/src/dactim_mri/spectroscopy.py`

 * *Files identical despite different names*

### Comparing `dactim_mri-0.0.4/src/dactim_mri/utils.py` & `dactim_mri-0.0.5/src/dactim_mri/utils.py`

 * *Files identical despite different names*

### Comparing `dactim_mri-0.0.4/src/dactim_mri/visualization.py` & `dactim_mri-0.0.5/src/dactim_mri/visualization.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,26 +2,41 @@
 import nibabel as nib
 import numpy as np
 import matplotlib.pyplot as plt
 import os
 
 from dactim_mri.utils import get_name_of_path
 
+def plot_histo(input_path):
+    # Load your MRI image data into a numpy array
+    mri_image = nib.load(input_path).get_fdata()
+
+    # Flatten the 3D array to a 1D array
+    image_flat = mri_image.flatten()
+
+    # Plot the histogram
+    plt.hist(image_flat, bins=256, range=(1, np.amax(mri_image)), alpha=0.75)
+    plt.xlabel('Intensity')
+    plt.ylabel('Frequency')
+    plt.title('Histogram of MRI Image')
+    plt.show()
+
 def plot(*images):
     subject = tio.Subject(temp=tio.ScalarImage(images[0]))
     if len(images) > 1:
         for img in images:
-            subject.add_image(tio.ScalarImage(img), os.path.basename(img).replace(".nii.gz", ""))
+            title = get_name_of_path(os.path.basename(img).replace(".nii.gz", ""))
+            subject.add_image(tio.ScalarImage(img), title)
     else:
-        subject.add_image(tio.ScalarImage(images[0]), os.path.basename(images[0]).replace(".nii.gz", ""))
+        title = get_name_of_path(os.path.basename(images[0]).replace(".nii.gz", ""))
+        subject.add_image(tio.ScalarImage(images[0]), title)
 
     subject.remove_image("temp")
     subject.plot()
 
-
 class plot3D():
     def __init__(self, input_path):
         self.volume = nib.load(input_path)
         self.volume_data = self.check_orientation(self.volume)[::-1,:,::-1]
         self.multi_slice_viewer()
 
     def check_orientation(self, volume):
```

### Comparing `dactim_mri-0.0.4/LICENSE` & `dactim_mri-0.0.5/LICENSE`

 * *Files identical despite different names*

