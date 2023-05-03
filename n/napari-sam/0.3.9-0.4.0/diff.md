# Comparing `tmp/napari-sam-0.3.9.tar.gz` & `tmp/napari-sam-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-sam-0.3.9.tar", last modified: Tue Apr 18 08:56:21 2023, max compression
+gzip compressed data, was "napari-sam-0.4.0.tar", last modified: Wed May  3 09:16:15 2023, max compression
```

## Comparing `napari-sam-0.3.9.tar` & `napari-sam-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:56:21.862763 napari-sam-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-18 08:56:04.000000 napari-sam-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-18 08:56:04.000000 napari-sam-0.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-18 08:56:21.862763 napari-sam-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-18 08:56:04.000000 napari-sam-0.3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-18 08:56:04.000000 napari-sam-0.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-18 08:56:21.862763 napari-sam-0.3.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:56:21.858762 napari-sam-0.3.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:56:21.862763 napari-sam-0.3.9/src/napari_sam/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-18 08:56:04.000000 napari-sam-0.3.9/src/napari_sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38882 2023-04-18 08:56:04.000000 napari-sam-0.3.9/src/napari_sam/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-18 08:56:04.000000 napari-sam-0.3.9/src/napari_sam/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-18 08:56:04.000000 napari-sam-0.3.9/src/napari_sam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:56:21.862763 napari-sam-0.3.9/src/napari_sam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-18 08:56:21.000000 napari-sam-0.3.9/src/napari_sam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-18 08:56:21.000000 napari-sam-0.3.9/src/napari_sam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:56:21.000000 napari-sam-0.3.9/src/napari_sam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-18 08:56:21.000000 napari-sam-0.3.9/src/napari_sam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-18 08:56:21.000000 napari-sam-0.3.9/src/napari_sam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 08:56:21.000000 napari-sam-0.3.9/src/napari_sam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:15.273259 napari-sam-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-03 09:15:59.000000 napari-sam-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-03 09:15:59.000000 napari-sam-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-05-03 09:16:15.273259 napari-sam-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-03 09:15:59.000000 napari-sam-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-03 09:15:59.000000 napari-sam-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-03 09:16:15.273259 napari-sam-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:15.269259 napari-sam-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:15.269259 napari-sam-0.4.0/src/napari_sam/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-03 09:15:59.000000 napari-sam-0.4.0/src/napari_sam/QCollapsibleBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-03 09:15:59.000000 napari-sam-0.4.0/src/napari_sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57158 2023-05-03 09:15:59.000000 napari-sam-0.4.0/src/napari_sam/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-03 09:15:59.000000 napari-sam-0.4.0/src/napari_sam/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-03 09:15:59.000000 napari-sam-0.4.0/src/napari_sam/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-03 09:15:59.000000 napari-sam-0.4.0/src/napari_sam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:15.273259 napari-sam-0.4.0/src/napari_sam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-05-03 09:16:15.000000 napari-sam-0.4.0/src/napari_sam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-03 09:16:15.000000 napari-sam-0.4.0/src/napari_sam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 09:16:15.000000 napari-sam-0.4.0/src/napari_sam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 09:16:15.000000 napari-sam-0.4.0/src/napari_sam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-03 09:16:15.000000 napari-sam-0.4.0/src/napari_sam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 09:16:15.000000 napari-sam-0.4.0/src/napari_sam.egg-info/top_level.txt
```

### Comparing `napari-sam-0.3.9/LICENSE` & `napari-sam-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.9/PKG-INFO` & `napari-sam-0.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.3.9
+Version: 0.4.0
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
@@ -44,22 +44,22 @@
 
 At last, our SAM integration supports both **2D and 3D images**!
 
 ----------------------------------
 
 Everything mode             |  Click-based semantic segmentation mode |  Click-based instance segmentation mode
 :-------------------------:|:-------------------------:|:-------------------------:
-![](cats_everything.png)  |  ![](cats_semantic.png)  |  ![](cats_instance.png)
+![](https://github.com/MIC-DKFZ/napari-sam/raw/main/cats_everything.png)  |  ![](https://github.com/MIC-DKFZ/napari-sam/raw/main/cats_semantic.png)  |  ![](https://github.com/MIC-DKFZ/napari-sam/raw/main/cats_instance.png)
 
 ----------------------------------
 <h2 align="center">SAM in Napari demo</h2>
 <p align="center"><em>Click to play the video</em></p>
 <div align="center">
   <a href="https://www.youtube.com/watch?v=OPE1Xnw487E">
-    <img src="thumpnail.jpeg" alt="SAM Demo">
+    <img src="https://github.com/MIC-DKFZ/napari-sam/raw/main/thumpnail.jpeg" alt="SAM Demo">
   </a>
 </div>
 
 
 ----------------------------------
 
 ## Installation
@@ -121,14 +121,14 @@
 
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
 
 # Acknowledgements
-<img src="HI_Logo.png" height="100px" />
+<img src="https://github.com/MIC-DKFZ/napari-sam/raw/main/HI_Logo.png" height="100px" />
 
-<img src="dkfz_logo.png" height="100px" />
+<img src="https://github.com/MIC-DKFZ/napari-sam/raw/main/dkfz_logo.png" height="100px" />
 
 napari-sam is developed and maintained by the Applied Computer Vision Lab (ACVL) of [Helmholtz Imaging](http://helmholtz-imaging.de) 
 and the [Division of Medical Image Computing](https://www.dkfz.de/en/mic/index.php) at the 
 [German Cancer Research Center (DKFZ)](https://www.dkfz.de/en/index.html).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-sam Version: 0.3.9 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.4.0 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
@@ -29,16 +29,18 @@
 is the new segmentation system from Meta AI capable of **one-click segmentation
 of any object**, and now, our plugin neatly integrates this into Napari. We
 have already **extended** SAM's click-based foreground separation to full
 **click-based semantic segmentation and instance segmentation**! At last, our
 SAM integration supports both **2D and 3D images**! ---------------------------
 ------- Everything mode | Click-based semantic segmentation mode | Click-based
 instance segmentation mode :-------------------------:|:-----------------------
---:|:-------------------------: ![](cats_everything.png) | ![]
-(cats_semantic.png) | ![](cats_instance.png) ----------------------------------
+--:|:-------------------------: ![](https://github.com/MIC-DKFZ/napari-sam/raw/
+main/cats_everything.png) | ![](https://github.com/MIC-DKFZ/napari-sam/raw/
+main/cats_semantic.png) | ![](https://github.com/MIC-DKFZ/napari-sam/raw/main/
+cats_instance.png) ----------------------------------
                         ***** SAM in Napari demo *****
                             Click to play the video
                                   [SAM_Demo]
 ---------------------------------- ## Installation The plugin requires
 `python>=3.8`, as well as `pytorch>=1.7` and `torchvision>=0.8`. Please follow
 the instructions here to install both PyTorch and TorchVision dependencies.
 Installing both PyTorch and TorchVision with CUDA support is strongly
@@ -63,12 +65,13 @@
 www.gnu.org/licenses/gpl-3.0.txt [GNU LGPL v3.0]: http://www.gnu.org/licenses/
 lgpl-3.0.txt [Apache Software License 2.0]: http://www.apache.org/licenses/
 LICENSE-2.0 [Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/
 2.0/index.txt [cookiecutter-napari-plugin]: https://github.com/napari/
 cookiecutter-napari-plugin [file an issue]: https://github.com/MIC-DKFZ/napari-
 sam/issues [napari]: https://github.com/napari/napari [tox]: https://
 tox.readthedocs.io/en/latest/ [pip]: https://pypi.org/project/pip/ [PyPI]:
-https://pypi.org/ # Acknowledgements [HI_Logo.png] [dkfz_logo.png] napari-sam
-is developed and maintained by the Applied Computer Vision Lab (ACVL) of
-[Helmholtz Imaging](http://helmholtz-imaging.de) and the [Division of Medical
-Image Computing](https://www.dkfz.de/en/mic/index.php) at the [German Cancer
-Research Center (DKFZ)](https://www.dkfz.de/en/index.html).
+https://pypi.org/ # Acknowledgements [https://github.com/MIC-DKFZ/napari-sam/
+raw/main/HI_Logo.png] [https://github.com/MIC-DKFZ/napari-sam/raw/main/
+dkfz_logo.png] napari-sam is developed and maintained by the Applied Computer
+Vision Lab (ACVL) of [Helmholtz Imaging](http://helmholtz-imaging.de) and the
+[Division of Medical Image Computing](https://www.dkfz.de/en/mic/index.php) at
+the [German Cancer Research Center (DKFZ)](https://www.dkfz.de/en/index.html).
```

### Comparing `napari-sam-0.3.9/README.md` & `napari-sam-0.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 
 At last, our SAM integration supports both **2D and 3D images**!
 
 ----------------------------------
 
 Everything mode             |  Click-based semantic segmentation mode |  Click-based instance segmentation mode
 :-------------------------:|:-------------------------:|:-------------------------:
-![](cats_everything.png)  |  ![](cats_semantic.png)  |  ![](cats_instance.png)
+![](https://github.com/MIC-DKFZ/napari-sam/raw/main/cats_everything.png)  |  ![](https://github.com/MIC-DKFZ/napari-sam/raw/main/cats_semantic.png)  |  ![](https://github.com/MIC-DKFZ/napari-sam/raw/main/cats_instance.png)
 
 ----------------------------------
 <h2 align="center">SAM in Napari demo</h2>
 <p align="center"><em>Click to play the video</em></p>
 <div align="center">
   <a href="https://www.youtube.com/watch?v=OPE1Xnw487E">
-    <img src="thumpnail.jpeg" alt="SAM Demo">
+    <img src="https://github.com/MIC-DKFZ/napari-sam/raw/main/thumpnail.jpeg" alt="SAM Demo">
   </a>
 </div>
 
 
 ----------------------------------
 
 ## Installation
@@ -92,14 +92,14 @@
 
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
 
 # Acknowledgements
-<img src="HI_Logo.png" height="100px" />
+<img src="https://github.com/MIC-DKFZ/napari-sam/raw/main/HI_Logo.png" height="100px" />
 
-<img src="dkfz_logo.png" height="100px" />
+<img src="https://github.com/MIC-DKFZ/napari-sam/raw/main/dkfz_logo.png" height="100px" />
 
 napari-sam is developed and maintained by the Applied Computer Vision Lab (ACVL) of [Helmholtz Imaging](http://helmholtz-imaging.de) 
 and the [Division of Medical Image Computing](https://www.dkfz.de/en/mic/index.php) at the 
-[German Cancer Research Center (DKFZ)](https://www.dkfz.de/en/index.html).
+[German Cancer Research Center (DKFZ)](https://www.dkfz.de/en/index.html).
```

#### html2text {}

```diff
@@ -13,16 +13,18 @@
 is the new segmentation system from Meta AI capable of **one-click segmentation
 of any object**, and now, our plugin neatly integrates this into Napari. We
 have already **extended** SAM's click-based foreground separation to full
 **click-based semantic segmentation and instance segmentation**! At last, our
 SAM integration supports both **2D and 3D images**! ---------------------------
 ------- Everything mode | Click-based semantic segmentation mode | Click-based
 instance segmentation mode :-------------------------:|:-----------------------
---:|:-------------------------: ![](cats_everything.png) | ![]
-(cats_semantic.png) | ![](cats_instance.png) ----------------------------------
+--:|:-------------------------: ![](https://github.com/MIC-DKFZ/napari-sam/raw/
+main/cats_everything.png) | ![](https://github.com/MIC-DKFZ/napari-sam/raw/
+main/cats_semantic.png) | ![](https://github.com/MIC-DKFZ/napari-sam/raw/main/
+cats_instance.png) ----------------------------------
                         ***** SAM in Napari demo *****
                             Click to play the video
                                   [SAM_Demo]
 ---------------------------------- ## Installation The plugin requires
 `python>=3.8`, as well as `pytorch>=1.7` and `torchvision>=0.8`. Please follow
 the instructions here to install both PyTorch and TorchVision dependencies.
 Installing both PyTorch and TorchVision with CUDA support is strongly
@@ -47,12 +49,13 @@
 www.gnu.org/licenses/gpl-3.0.txt [GNU LGPL v3.0]: http://www.gnu.org/licenses/
 lgpl-3.0.txt [Apache Software License 2.0]: http://www.apache.org/licenses/
 LICENSE-2.0 [Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/
 2.0/index.txt [cookiecutter-napari-plugin]: https://github.com/napari/
 cookiecutter-napari-plugin [file an issue]: https://github.com/MIC-DKFZ/napari-
 sam/issues [napari]: https://github.com/napari/napari [tox]: https://
 tox.readthedocs.io/en/latest/ [pip]: https://pypi.org/project/pip/ [PyPI]:
-https://pypi.org/ # Acknowledgements [HI_Logo.png] [dkfz_logo.png] napari-sam
-is developed and maintained by the Applied Computer Vision Lab (ACVL) of
-[Helmholtz Imaging](http://helmholtz-imaging.de) and the [Division of Medical
-Image Computing](https://www.dkfz.de/en/mic/index.php) at the [German Cancer
-Research Center (DKFZ)](https://www.dkfz.de/en/index.html).
+https://pypi.org/ # Acknowledgements [https://github.com/MIC-DKFZ/napari-sam/
+raw/main/HI_Logo.png] [https://github.com/MIC-DKFZ/napari-sam/raw/main/
+dkfz_logo.png] napari-sam is developed and maintained by the Applied Computer
+Vision Lab (ACVL) of [Helmholtz Imaging](http://helmholtz-imaging.de) and the
+[Division of Medical Image Computing](https://www.dkfz.de/en/mic/index.php) at
+the [German Cancer Research Center (DKFZ)](https://www.dkfz.de/en/index.html).
```

### Comparing `napari-sam-0.3.9/setup.cfg` & `napari-sam-0.4.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,16 @@
 install_requires = 
 	numpy
 	magicgui
 	qtpy
 	napari
 	vispy
 	tqdm
-	napari-medical-image-formats
+	napari-nifti
+	superqt
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
```

### Comparing `napari-sam-0.3.9/src/napari_sam/utils.py` & `napari-sam-0.4.0/src/napari_sam/utils.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.9/src/napari_sam.egg-info/PKG-INFO` & `napari-sam-0.4.0/src/napari_sam.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.3.9
+Version: 0.4.0
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
@@ -44,22 +44,22 @@
 
 At last, our SAM integration supports both **2D and 3D images**!
 
 ----------------------------------
 
 Everything mode             |  Click-based semantic segmentation mode |  Click-based instance segmentation mode
 :-------------------------:|:-------------------------:|:-------------------------:
-![](cats_everything.png)  |  ![](cats_semantic.png)  |  ![](cats_instance.png)
+![](https://github.com/MIC-DKFZ/napari-sam/raw/main/cats_everything.png)  |  ![](https://github.com/MIC-DKFZ/napari-sam/raw/main/cats_semantic.png)  |  ![](https://github.com/MIC-DKFZ/napari-sam/raw/main/cats_instance.png)
 
 ----------------------------------
 <h2 align="center">SAM in Napari demo</h2>
 <p align="center"><em>Click to play the video</em></p>
 <div align="center">
   <a href="https://www.youtube.com/watch?v=OPE1Xnw487E">
-    <img src="thumpnail.jpeg" alt="SAM Demo">
+    <img src="https://github.com/MIC-DKFZ/napari-sam/raw/main/thumpnail.jpeg" alt="SAM Demo">
   </a>
 </div>
 
 
 ----------------------------------
 
 ## Installation
@@ -121,14 +121,14 @@
 
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
 
 # Acknowledgements
-<img src="HI_Logo.png" height="100px" />
+<img src="https://github.com/MIC-DKFZ/napari-sam/raw/main/HI_Logo.png" height="100px" />
 
-<img src="dkfz_logo.png" height="100px" />
+<img src="https://github.com/MIC-DKFZ/napari-sam/raw/main/dkfz_logo.png" height="100px" />
 
 napari-sam is developed and maintained by the Applied Computer Vision Lab (ACVL) of [Helmholtz Imaging](http://helmholtz-imaging.de) 
 and the [Division of Medical Image Computing](https://www.dkfz.de/en/mic/index.php) at the 
 [German Cancer Research Center (DKFZ)](https://www.dkfz.de/en/index.html).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-sam Version: 0.3.9 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.4.0 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
@@ -29,16 +29,18 @@
 is the new segmentation system from Meta AI capable of **one-click segmentation
 of any object**, and now, our plugin neatly integrates this into Napari. We
 have already **extended** SAM's click-based foreground separation to full
 **click-based semantic segmentation and instance segmentation**! At last, our
 SAM integration supports both **2D and 3D images**! ---------------------------
 ------- Everything mode | Click-based semantic segmentation mode | Click-based
 instance segmentation mode :-------------------------:|:-----------------------
---:|:-------------------------: ![](cats_everything.png) | ![]
-(cats_semantic.png) | ![](cats_instance.png) ----------------------------------
+--:|:-------------------------: ![](https://github.com/MIC-DKFZ/napari-sam/raw/
+main/cats_everything.png) | ![](https://github.com/MIC-DKFZ/napari-sam/raw/
+main/cats_semantic.png) | ![](https://github.com/MIC-DKFZ/napari-sam/raw/main/
+cats_instance.png) ----------------------------------
                         ***** SAM in Napari demo *****
                             Click to play the video
                                   [SAM_Demo]
 ---------------------------------- ## Installation The plugin requires
 `python>=3.8`, as well as `pytorch>=1.7` and `torchvision>=0.8`. Please follow
 the instructions here to install both PyTorch and TorchVision dependencies.
 Installing both PyTorch and TorchVision with CUDA support is strongly
@@ -63,12 +65,13 @@
 www.gnu.org/licenses/gpl-3.0.txt [GNU LGPL v3.0]: http://www.gnu.org/licenses/
 lgpl-3.0.txt [Apache Software License 2.0]: http://www.apache.org/licenses/
 LICENSE-2.0 [Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/
 2.0/index.txt [cookiecutter-napari-plugin]: https://github.com/napari/
 cookiecutter-napari-plugin [file an issue]: https://github.com/MIC-DKFZ/napari-
 sam/issues [napari]: https://github.com/napari/napari [tox]: https://
 tox.readthedocs.io/en/latest/ [pip]: https://pypi.org/project/pip/ [PyPI]:
-https://pypi.org/ # Acknowledgements [HI_Logo.png] [dkfz_logo.png] napari-sam
-is developed and maintained by the Applied Computer Vision Lab (ACVL) of
-[Helmholtz Imaging](http://helmholtz-imaging.de) and the [Division of Medical
-Image Computing](https://www.dkfz.de/en/mic/index.php) at the [German Cancer
-Research Center (DKFZ)](https://www.dkfz.de/en/index.html).
+https://pypi.org/ # Acknowledgements [https://github.com/MIC-DKFZ/napari-sam/
+raw/main/HI_Logo.png] [https://github.com/MIC-DKFZ/napari-sam/raw/main/
+dkfz_logo.png] napari-sam is developed and maintained by the Applied Computer
+Vision Lab (ACVL) of [Helmholtz Imaging](http://helmholtz-imaging.de) and the
+[Division of Medical Image Computing](https://www.dkfz.de/en/mic/index.php) at
+the [German Cancer Research Center (DKFZ)](https://www.dkfz.de/en/index.html).
```

