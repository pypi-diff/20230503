# Comparing `tmp/ix_aims-0.1.1rc1.tar.gz` & `tmp/ix_aims-0.1.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ix_aims-0.1.1rc1.tar", max compression
+gzip compressed data, was "ix_aims-0.1.1rc2.tar", max compression
```

## Comparing `ix_aims-0.1.1rc1.tar` & `ix_aims-0.1.1rc2.tar`

### file list

```diff
@@ -1,14 +1,11 @@
--rw-r--r--   0        0        0       18 2023-05-02 21:16:59.064713 ix_aims-0.1.1rc1/README.md
--rw-r--r--   0        0        0        0 2023-05-02 21:33:19.881513 ix_aims-0.1.1rc1/ix_aims/__init__.py
--rw-r--r--   0        0        0      123 2023-05-02 21:37:07.078194 ix_aims-0.1.1rc1/ix_aims/cli.py
--rw-r--r--   0        0        0     2134 2023-05-02 21:20:56.338365 ix_aims-0.1.1rc1/ix_aims/imgs/icon.png
--rw-r--r--   0        0        0     1996 2023-05-02 21:20:56.338365 ix_aims-0.1.1rc1/ix_aims/imgs/noBtn.png
--rw-r--r--   0        0        0      322 2023-05-02 21:20:56.342365 ix_aims-0.1.1rc1/ix_aims/imgs/plusTab.png
--rw-r--r--   0        0        0     3615 2023-05-02 21:20:56.342365 ix_aims-0.1.1rc1/ix_aims/imgs/processesBtn.png
--rw-r--r--   0        0        0     1207 2023-05-02 21:20:56.342365 ix_aims-0.1.1rc1/ix_aims/imgs/selectDirsBtn.png
--rw-r--r--   0        0        0     1064 2023-05-02 21:20:56.338365 ix_aims-0.1.1rc1/ix_aims/imgs/winIcon.png
--rw-r--r--   0        0        0     2201 2023-05-02 21:20:56.342365 ix_aims-0.1.1rc1/ix_aims/imgs/yesBtn.png
--rw-r--r--   0        0        0     3683 2023-05-02 21:52:32.596646 ix_aims-0.1.1rc1/ix_aims/lib.py
--rw-r--r--   0        0        0      630 2023-05-02 21:52:27.800650 ix_aims-0.1.1rc1/pyproject.toml
--rw-r--r--   0        0        0      951 1970-01-01 00:00:00.000000 ix_aims-0.1.1rc1/setup.py
--rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 ix_aims-0.1.1rc1/PKG-INFO
+-rw-r--r--   0        0        0       18 2023-05-02 21:16:59.064713 ix_aims-0.1.1rc2/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 21:33:19.881513 ix_aims-0.1.1rc2/ix_aims/__init__.py
+-rw-r--r--   0        0        0      123 2023-05-02 21:37:07.078194 ix_aims-0.1.1rc2/ix_aims/cli.py
+-rw-r--r--   0        0        0      230 2023-05-02 21:58:44.236538 ix_aims-0.1.1rc2/ix_aims/imgs/__init__.py
+-rw-r--r--   0        0        0      322 2023-05-02 21:20:56.342365 ix_aims-0.1.1rc2/ix_aims/imgs/plusTab.png
+-rw-r--r--   0        0        0     3615 2023-05-02 21:20:56.342365 ix_aims-0.1.1rc2/ix_aims/imgs/processesBtn.png
+-rw-r--r--   0        0        0     2201 2023-05-02 21:20:56.342365 ix_aims-0.1.1rc2/ix_aims/imgs/yesBtn.png
+-rw-r--r--   0        0        0     3648 2023-05-02 21:58:57.068539 ix_aims-0.1.1rc2/ix_aims/lib.py
+-rw-r--r--   0        0        0      630 2023-05-02 21:59:10.080541 ix_aims-0.1.1rc2/pyproject.toml
+-rw-r--r--   0        0        0      944 1970-01-01 00:00:00.000000 ix_aims-0.1.1rc2/setup.py
+-rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 ix_aims-0.1.1rc2/PKG-INFO
```

### Comparing `ix_aims-0.1.1rc1/ix_aims/imgs/processesBtn.png` & `ix_aims-0.1.1rc2/ix_aims/imgs/processesBtn.png`

 * *Files identical despite different names*

### Comparing `ix_aims-0.1.1rc1/ix_aims/imgs/yesBtn.png` & `ix_aims-0.1.1rc2/ix_aims/imgs/yesBtn.png`

 * *Files identical despite different names*

### Comparing `ix_aims-0.1.1rc1/ix_aims/lib.py` & `ix_aims-0.1.1rc2/ix_aims/lib.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 from time import sleep
 from typing import Literal
 
 import arrow
 import pyautogui as g
 from hakai_api import Client
 
+from ix_aims import imgs
+
 g.PAUSE = 0.05
-IMG_DIR = "ix_aims/imgs"
 
 
 def move(img):
     if loc := g.locateOnScreen(img, grayscale=True, confidence=.95):
         g.moveTo(*g.center(loc))
 
 
@@ -23,19 +24,19 @@
 def open_ix_capture():
     g.click(10, g.size().height)
     g.typewrite('ixcapture')
     g.hotkey('enter')
 
 
 def go_to_processes_tab():
-    click(f"{IMG_DIR}/processesBtn.png")
+    click(imgs.processesBtn)
 
 
 def click_yes():
-    click(f"{IMG_DIR}/yesBtn.png")
+    click(imgs.yesBtn)
 
 
 def get_camera_params(d: 'Arrow', camera: Literal["rgb"] | Literal["nir"]):
     c = Client()
     cal = c.get(
         f"{c.api_root}/aco/camera_calibration?camera_type={camera}&valid_from<={d.isoformat()}&sort=-valid_from&limit=1").json()[
         0]
@@ -51,15 +52,15 @@
         return res.json()
     else:
         res.raise_for_status()
 
 
 def setup_work_order_day(recipe_name, save_folder, rgb_params, nir_params):
     # New Recipe
-    click(f"{IMG_DIR}/plusTab.png")
+    click(imgs.plusTab)
     g.hotkey('tab')
     g.hotkey('ctrl', 'a')
     g.hotkey('del')
     g.typewrite(recipe_name)
 
     # Skip prefix name
     g.hotkey('tab')
```

### Comparing `ix_aims-0.1.1rc1/pyproject.toml` & `ix_aims-0.1.1rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ix-aims"
-version = "0.1.1rc1"
+version = "0.1.1rc2"
 description = "iX Capture automation with AIMS data"
 authors = ["Taylor Denouden <taylor.denouden@hakai.org>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "ix_aims"}]
 
 [tool.poetry.dependencies]
```

### Comparing `ix_aims-0.1.1rc1/setup.py` & `ix_aims-0.1.1rc2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['ix_aims']
+['ix_aims', 'ix_aims.imgs']
 
 package_data = \
-{'': ['*'], 'ix_aims': ['imgs/*']}
+{'': ['*']}
 
 install_requires = \
 ['PyAutoGUI>=0.9.53,<0.10.0',
  'arrow>=1.2.3,<2.0.0',
  'hakai-api>=1.3.0,<2.0.0',
  'opencv-python>=4.7.0.72,<5.0.0.0',
  'pillow>=9.5.0,<10.0.0',
@@ -17,15 +17,15 @@
  'typer>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['autoix = ix_aims.cli:main']}
 
 setup_kwargs = {
     'name': 'ix-aims',
-    'version': '0.1.1rc1',
+    'version': '0.1.1rc2',
     'description': 'iX Capture automation with AIMS data',
     'long_description': '# auto-ix-capture\n',
     'author': 'Taylor Denouden',
     'author_email': 'taylor.denouden@hakai.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ix_aims-0.1.1rc1/PKG-INFO` & `ix_aims-0.1.1rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ix-aims
-Version: 0.1.1rc1
+Version: 0.1.1rc2
 Summary: iX Capture automation with AIMS data
 License: MIT
 Author: Taylor Denouden
 Author-email: taylor.denouden@hakai.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

