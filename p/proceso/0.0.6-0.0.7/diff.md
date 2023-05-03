# Comparing `tmp/proceso-0.0.6.tar.gz` & `tmp/proceso-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proceso-0.0.6.tar", last modified: Tue May  2 19:46:34 2023, max compression
+gzip compressed data, was "proceso-0.0.7.tar", last modified: Wed May  3 03:03:09 2023, max compression
```

## Comparing `proceso-0.0.6.tar` & `proceso-0.0.7.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-02 19:46:34.201693 proceso-0.0.6/
--rw-r--r--   0 nick       (501) staff       (20)     7652 2023-04-27 14:59:44.000000 proceso-0.0.6/LICENSE
--rw-r--r--   0 nick       (501) staff       (20)     3089 2023-05-02 19:46:34.201741 proceso-0.0.6/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)     2449 2023-05-02 18:05:23.000000 proceso-0.0.6/README.md
--rw-r--r--   0 nick       (501) staff       (20)      104 2023-04-27 14:06:11.000000 proceso-0.0.6/pyproject.toml
--rw-r--r--   0 nick       (501) staff       (20)      778 2023-05-02 19:46:34.201966 proceso-0.0.6/setup.cfg
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-02 19:46:34.197129 proceso-0.0.6/src/
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-02 19:46:34.200043 proceso-0.0.6/src/proceso/
--rw-r--r--   0 nick       (501) staff       (20)     3787 2023-05-02 18:03:17.000000 proceso-0.0.6/src/proceso/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)      341 2023-05-02 18:03:20.000000 proceso-0.0.6/src/proceso/_binding.py
--rw-r--r--   0 nick       (501) staff       (20)    11523 2023-05-02 18:03:22.000000 proceso-0.0.6/src/proceso/colors.py
--rw-r--r--   0 nick       (501) staff       (20)     9800 2023-05-02 18:03:25.000000 proceso-0.0.6/src/proceso/constants.py
--rw-r--r--   0 nick       (501) staff       (20)     3563 2023-05-02 18:03:27.000000 proceso-0.0.6/src/proceso/data.py
--rw-r--r--   0 nick       (501) staff       (20)     9197 2023-05-02 18:03:30.000000 proceso-0.0.6/src/proceso/dom.py
--rw-r--r--   0 nick       (501) staff       (20)     8773 2023-05-02 18:03:32.000000 proceso-0.0.6/src/proceso/environment.py
--rw-r--r--   0 nick       (501) staff       (20)     1516 2023-05-02 18:03:35.000000 proceso-0.0.6/src/proceso/events.py
--rw-r--r--   0 nick       (501) staff       (20)    14015 2023-05-02 18:03:38.000000 proceso-0.0.6/src/proceso/images.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-02 19:46:34.201250 proceso-0.0.6/src/proceso/math/
--rw-r--r--   0 nick       (501) staff       (20)      271 2023-05-02 16:58:34.000000 proceso-0.0.6/src/proceso/math/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     5959 2023-05-02 16:55:18.000000 proceso-0.0.6/src/proceso/math/calculation.py
--rw-r--r--   0 nick       (501) staff       (20)     3644 2023-05-02 16:55:50.000000 proceso-0.0.6/src/proceso/math/noise.py
--rw-r--r--   0 nick       (501) staff       (20)     1711 2023-05-02 16:57:42.000000 proceso-0.0.6/src/proceso/math/random.py
--rw-r--r--   0 nick       (501) staff       (20)     3871 2023-05-02 16:56:53.000000 proceso-0.0.6/src/proceso/math/trigonometry.py
--rw-r--r--   0 nick       (501) staff       (20)    61205 2023-05-02 18:29:09.000000 proceso-0.0.6/src/proceso/math/vector.py
--rw-r--r--   0 nick       (501) staff       (20)     6462 2023-05-02 18:03:40.000000 proceso-0.0.6/src/proceso/rendering.py
--rw-r--r--   0 nick       (501) staff       (20)    29994 2023-05-02 18:03:43.000000 proceso-0.0.6/src/proceso/shape.py
--rw-r--r--   0 nick       (501) staff       (20)     6114 2023-05-02 18:03:46.000000 proceso-0.0.6/src/proceso/structure.py
--rw-r--r--   0 nick       (501) staff       (20)    16233 2023-05-02 18:03:48.000000 proceso-0.0.6/src/proceso/sysvars.py
--rw-r--r--   0 nick       (501) staff       (20)    15708 2023-05-02 18:03:51.000000 proceso-0.0.6/src/proceso/three_d.py
--rw-r--r--   0 nick       (501) staff       (20)     7325 2023-05-02 18:03:55.000000 proceso-0.0.6/src/proceso/transform.py
--rw-r--r--   0 nick       (501) staff       (20)     6198 2023-05-02 18:03:57.000000 proceso-0.0.6/src/proceso/typography.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-02 19:46:34.200628 proceso-0.0.6/src/proceso.egg-info/
--rw-r--r--   0 nick       (501) staff       (20)     3089 2023-05-02 19:46:34.000000 proceso-0.0.6/src/proceso.egg-info/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)      763 2023-05-02 19:46:34.000000 proceso-0.0.6/src/proceso.egg-info/SOURCES.txt
--rw-r--r--   0 nick       (501) staff       (20)        1 2023-05-02 19:46:34.000000 proceso-0.0.6/src/proceso.egg-info/dependency_links.txt
--rw-r--r--   0 nick       (501) staff       (20)       12 2023-05-02 19:46:34.000000 proceso-0.0.6/src/proceso.egg-info/requires.txt
--rw-r--r--   0 nick       (501) staff       (20)        8 2023-05-02 19:46:34.000000 proceso-0.0.6/src/proceso.egg-info/top_level.txt
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-03 03:03:09.657988 proceso-0.0.7/
+-rw-r--r--   0 nick       (501) staff       (20)     7652 2023-04-27 14:59:44.000000 proceso-0.0.7/LICENSE
+-rw-r--r--   0 nick       (501) staff       (20)     4056 2023-05-03 03:03:09.658053 proceso-0.0.7/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)     3416 2023-05-03 02:26:52.000000 proceso-0.0.7/README.md
+-rw-r--r--   0 nick       (501) staff       (20)      104 2023-04-27 14:06:11.000000 proceso-0.0.7/pyproject.toml
+-rw-r--r--   0 nick       (501) staff       (20)      778 2023-05-03 03:03:09.658318 proceso-0.0.7/setup.cfg
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-03 03:03:09.653005 proceso-0.0.7/src/
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-03 03:03:09.656633 proceso-0.0.7/src/proceso/
+-rw-r--r--   0 nick       (501) staff       (20)       25 2023-05-03 02:55:31.000000 proceso-0.0.7/src/proceso/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)      341 2023-05-02 18:03:20.000000 proceso-0.0.7/src/proceso/_binding.py
+-rw-r--r--   0 nick       (501) staff       (20)    11523 2023-05-02 18:03:22.000000 proceso-0.0.7/src/proceso/colors.py
+-rw-r--r--   0 nick       (501) staff       (20)     9800 2023-05-02 18:03:25.000000 proceso-0.0.7/src/proceso/constants.py
+-rw-r--r--   0 nick       (501) staff       (20)     3858 2023-05-03 03:02:50.000000 proceso-0.0.7/src/proceso/core.py
+-rw-r--r--   0 nick       (501) staff       (20)     3563 2023-05-03 02:43:35.000000 proceso-0.0.7/src/proceso/data.py
+-rw-r--r--   0 nick       (501) staff       (20)     9197 2023-05-02 18:03:30.000000 proceso-0.0.7/src/proceso/dom.py
+-rw-r--r--   0 nick       (501) staff       (20)     8773 2023-05-02 18:03:32.000000 proceso-0.0.7/src/proceso/environment.py
+-rw-r--r--   0 nick       (501) staff       (20)     1516 2023-05-02 18:03:35.000000 proceso-0.0.7/src/proceso/events.py
+-rw-r--r--   0 nick       (501) staff       (20)    14015 2023-05-02 18:03:38.000000 proceso-0.0.7/src/proceso/images.py
+-rw-r--r--   0 nick       (501) staff       (20)     1266 2023-05-03 02:49:03.000000 proceso-0.0.7/src/proceso/io.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-03 03:03:09.657841 proceso-0.0.7/src/proceso/math/
+-rw-r--r--   0 nick       (501) staff       (20)      271 2023-05-02 16:58:34.000000 proceso-0.0.7/src/proceso/math/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     5959 2023-05-02 16:55:18.000000 proceso-0.0.7/src/proceso/math/calculation.py
+-rw-r--r--   0 nick       (501) staff       (20)     3644 2023-05-02 16:55:50.000000 proceso-0.0.7/src/proceso/math/noise.py
+-rw-r--r--   0 nick       (501) staff       (20)     1711 2023-05-02 16:57:42.000000 proceso-0.0.7/src/proceso/math/random.py
+-rw-r--r--   0 nick       (501) staff       (20)     3871 2023-05-02 16:56:53.000000 proceso-0.0.7/src/proceso/math/trigonometry.py
+-rw-r--r--   0 nick       (501) staff       (20)    61205 2023-05-02 18:29:09.000000 proceso-0.0.7/src/proceso/math/vector.py
+-rw-r--r--   0 nick       (501) staff       (20)     6518 2023-05-02 22:30:00.000000 proceso-0.0.7/src/proceso/rendering.py
+-rw-r--r--   0 nick       (501) staff       (20)    29994 2023-05-03 01:45:13.000000 proceso-0.0.7/src/proceso/shape.py
+-rw-r--r--   0 nick       (501) staff       (20)     6114 2023-05-02 18:03:46.000000 proceso-0.0.7/src/proceso/structure.py
+-rw-r--r--   0 nick       (501) staff       (20)    16233 2023-05-02 18:03:48.000000 proceso-0.0.7/src/proceso/sysvars.py
+-rw-r--r--   0 nick       (501) staff       (20)    15708 2023-05-02 18:03:51.000000 proceso-0.0.7/src/proceso/three_d.py
+-rw-r--r--   0 nick       (501) staff       (20)     7325 2023-05-02 18:03:55.000000 proceso-0.0.7/src/proceso/transform.py
+-rw-r--r--   0 nick       (501) staff       (20)     6198 2023-05-02 18:03:57.000000 proceso-0.0.7/src/proceso/typography.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-03 03:03:09.657166 proceso-0.0.7/src/proceso.egg-info/
+-rw-r--r--   0 nick       (501) staff       (20)     4056 2023-05-03 03:03:09.000000 proceso-0.0.7/src/proceso.egg-info/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)      801 2023-05-03 03:03:09.000000 proceso-0.0.7/src/proceso.egg-info/SOURCES.txt
+-rw-r--r--   0 nick       (501) staff       (20)        1 2023-05-03 03:03:09.000000 proceso-0.0.7/src/proceso.egg-info/dependency_links.txt
+-rw-r--r--   0 nick       (501) staff       (20)       12 2023-05-03 03:03:09.000000 proceso-0.0.7/src/proceso.egg-info/requires.txt
+-rw-r--r--   0 nick       (501) staff       (20)        8 2023-05-03 03:03:09.000000 proceso-0.0.7/src/proceso.egg-info/top_level.txt
```

### Comparing `proceso-0.0.6/LICENSE` & `proceso-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `proceso-0.0.6/PKG-INFO` & `proceso-0.0.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,19 @@
-Metadata-Version: 2.1
-Name: proceso
-Version: 0.0.6
-Summary: A Python package for creative coding on the web.
-Home-page: https://github.com/nickmcintyre/proceso
-Author: Nick McIntyre
-Author-email: nick@mcintyre.io
-Project-URL: Bug Tracker, https://github.com/nickmcintyre/proceso/issues
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: Environment :: WebAssembly
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # proceso
 > A Python package for creative coding on the web.
 
-proceso provides a Pythonic interface to the [p5.js](https://p5js.org) library. The package is designed for [Pyodide](https://pyodide.org)-based environments including [PyScript](https://pyscript.net) and (soonish) [JupyterLite](https://jupyterlite.readthedocs.io/en/latest/). Similar to [py5](https://py5coding.org/), proceso's goal is to integrate p5.js into the Python ecosystem with thoughtful choices about how to do so in the browser.
+proceso provides a Pythonic interface to the [p5.js](https://p5js.org) library. The package is designed for [Pyodide](https://pyodide.org)-based environments including [PyScript](https://pyscript.net) and (soonish) [JupyterLite](https://jupyterlite.readthedocs.io/en/latest/). Similar to [py5](https://py5coding.org), proceso's goal is to integrate p5.js into the Python ecosystem with thoughtful choices about how to do so in the browser.
 
 Here is an example of how to create a proceso sketch with PyScript:
 ```html
 <!DOCTYPE html>
 <html lang="en-us">
 
 <head>
-    <title>Bouncing Ball</title>
+    <title>My Sketch</title>
     <meta charset="utf-8" />
 
     <link rel="stylesheet" href="https://pyscript.net/releases/2023.03.1/pyscript.css" />
     <script defer src="https://pyscript.net/releases/2023.03.1/pyscript.js"></script>
     <link rel="stylesheet" href="style.css" />
     <script src="https://cdnjs.cloudflare.com/ajax/libs/p5.js/1.6.0/p5.min.js"></script>
     <py-config>
@@ -42,14 +25,51 @@
     <main></main>
     <py-script src="sketch.py"></py-script>
 </body>
 
 </html>
 ```
 
+## Static Sketches
+
+Similar to [Processing](https://processing.org), proceso enables beginners to start programming with "static sketches" before introducing animation and interaction. The following example draws a few shapes and a flower on the screen.
+
+```python
+from proceso import Sketch
+
+
+p5 = Sketch()
+
+# Create the canvas
+p5.create_canvas(720, 400)
+p5.background(200)
+
+# Set colors
+p5.fill(204, 101, 192, 127)
+p5.stroke(127, 63, 120)
+
+# A rectangle
+p5.rect(40, 120, 120, 40)
+# An ellipse
+p5.ellipse(240, 240, 80, 80)
+# A triangle
+p5.triangle(300, 100, 320, 100, 310, 80)
+
+# A design for a simple flower
+p5.translate(580, 200)
+p5.no_stroke()
+for _ in range(10):
+    p5.ellipse(0, 30, 20, 80)
+    p5.rotate(p5.PI / 5)
+```
+
+## Active Sketches
+
+proceso's "active sketches" provide the `run_sketch()` method to handle initialization, looping, and events. The sketch below animates a ball bouncing around the canvas and clears the canvas when a mouse press is detected.
+
 ```python
 from proceso import Sketch
 
 
 p5 = Sketch()
```

### Comparing `proceso-0.0.6/README.md` & `proceso-0.0.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,36 @@
+Metadata-Version: 2.1
+Name: proceso
+Version: 0.0.7
+Summary: A Python package for creative coding on the web.
+Home-page: https://github.com/nickmcintyre/proceso
+Author: Nick McIntyre
+Author-email: nick@mcintyre.io
+Project-URL: Bug Tracker, https://github.com/nickmcintyre/proceso/issues
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Environment :: WebAssembly
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # proceso
 > A Python package for creative coding on the web.
 
-proceso provides a Pythonic interface to the [p5.js](https://p5js.org) library. The package is designed for [Pyodide](https://pyodide.org)-based environments including [PyScript](https://pyscript.net) and (soonish) [JupyterLite](https://jupyterlite.readthedocs.io/en/latest/). Similar to [py5](https://py5coding.org/), proceso's goal is to integrate p5.js into the Python ecosystem with thoughtful choices about how to do so in the browser.
+proceso provides a Pythonic interface to the [p5.js](https://p5js.org) library. The package is designed for [Pyodide](https://pyodide.org)-based environments including [PyScript](https://pyscript.net) and (soonish) [JupyterLite](https://jupyterlite.readthedocs.io/en/latest/). Similar to [py5](https://py5coding.org), proceso's goal is to integrate p5.js into the Python ecosystem with thoughtful choices about how to do so in the browser.
 
 Here is an example of how to create a proceso sketch with PyScript:
 ```html
 <!DOCTYPE html>
 <html lang="en-us">
 
 <head>
-    <title>Bouncing Ball</title>
+    <title>My Sketch</title>
     <meta charset="utf-8" />
 
     <link rel="stylesheet" href="https://pyscript.net/releases/2023.03.1/pyscript.css" />
     <script defer src="https://pyscript.net/releases/2023.03.1/pyscript.js"></script>
     <link rel="stylesheet" href="style.css" />
     <script src="https://cdnjs.cloudflare.com/ajax/libs/p5.js/1.6.0/p5.min.js"></script>
     <py-config>
@@ -25,14 +42,51 @@
     <main></main>
     <py-script src="sketch.py"></py-script>
 </body>
 
 </html>
 ```
 
+## Static Sketches
+
+Similar to [Processing](https://processing.org), proceso enables beginners to start programming with "static sketches" before introducing animation and interaction. The following example draws a few shapes and a flower on the screen.
+
+```python
+from proceso import Sketch
+
+
+p5 = Sketch()
+
+# Create the canvas
+p5.create_canvas(720, 400)
+p5.background(200)
+
+# Set colors
+p5.fill(204, 101, 192, 127)
+p5.stroke(127, 63, 120)
+
+# A rectangle
+p5.rect(40, 120, 120, 40)
+# An ellipse
+p5.ellipse(240, 240, 80, 80)
+# A triangle
+p5.triangle(300, 100, 320, 100, 310, 80)
+
+# A design for a simple flower
+p5.translate(580, 200)
+p5.no_stroke()
+for _ in range(10):
+    p5.ellipse(0, 30, 20, 80)
+    p5.rotate(p5.PI / 5)
+```
+
+## Active Sketches
+
+proceso's "active sketches" provide the `run_sketch()` method to handle initialization, looping, and events. The sketch below animates a ball bouncing around the canvas and clears the canvas when a mouse press is detected.
+
 ```python
 from proceso import Sketch
 
 
 p5 = Sketch()
```

### Comparing `proceso-0.0.6/setup.cfg` & `proceso-0.0.7/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = proceso
-version = 0.0.6
+version = 0.0.7
 author = Nick McIntyre
 author_email = nick@mcintyre.io
 description = A Python package for creative coding on the web.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nickmcintyre/proceso
 project_urls =
```

### Comparing `proceso-0.0.6/src/proceso/__init__.py` & `proceso-0.0.7/src/proceso/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from .colors import Colors
 from .data import Data
 from .dom import DOM
 from .environment import Environment
 from .events import Events
 from .images import Images
+from .io import IO
 from .math import (
     Math,
     Vector as _Vector,
     Vector2D as _Vector2D,
     Vector3D as _Vector3D,
     Vector4D as _Vector4D,
 )
@@ -25,14 +26,15 @@
 class Sketch(
     Colors,
     Data,
     DOM,
     Environment,
     Events,
     Images,
+    IO,
     Math,
     Rendering,
     Shape,
     Structure,
     ThreeD,
     Transform,
     Typography,
@@ -57,14 +59,15 @@
         mouse_released: Callable | None = None,
         mouse_clicked: Callable | None = None,
         double_clicked: Callable | None = None,
         mouse_wheel: Callable | None = None,
         request_pointer_lock: Callable | None = None,
         exit_pointer_lock: Callable | None = None,
     ):
+        """"Run a sketch in active mode."""
         import inspect
         from pyodide.ffi import create_proxy
 
         self._p5js._setupDone = False
         self._p5js._preloadDone = False
         self._p5js._millisStart = -1
         if callable(preload):
```

### Comparing `proceso-0.0.6/src/proceso/colors.py` & `proceso-0.0.7/src/proceso/colors.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.6/src/proceso/constants.py` & `proceso-0.0.7/src/proceso/constants.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.6/src/proceso/data.py` & `proceso-0.0.7/src/proceso/data.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.6/src/proceso/dom.py` & `proceso-0.0.7/src/proceso/dom.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.6/src/proceso/environment.py` & `proceso-0.0.7/src/proceso/environment.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.6/src/proceso/events.py` & `proceso-0.0.7/src/proceso/events.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.6/src/proceso/images.py` & `proceso-0.0.7/src/proceso/images.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.6/src/proceso/math/calculation.py` & `proceso-0.0.7/src/proceso/math/calculation.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.6/src/proceso/math/noise.py` & `proceso-0.0.7/src/proceso/math/noise.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.6/src/proceso/math/random.py` & `proceso-0.0.7/src/proceso/math/random.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.6/src/proceso/math/trigonometry.py` & `proceso-0.0.7/src/proceso/math/trigonometry.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.6/src/proceso/math/vector.py` & `proceso-0.0.7/src/proceso/math/vector.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.6/src/proceso/rendering.py` & `proceso-0.0.7/src/proceso/rendering.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,16 @@
         p5.Renderer is set to WEBGL), the origin is positioned at the center of
         the canvas. See this issue for more information.
 
         The system variables width and height are set by the parameters passed to
         this function. If size() is not used, the window will be given a
         default size of 100×100 pixels.
         """
+        self.width = width
+        self.height = height
         return self._p5js.createCanvas(width, height, renderer)
 
     def resize_canvas(self, width: int, height: int, no_redraw: bool | None = None):
         """Resizes the canvas to given width and height.
         The canvas will be cleared and draw will be called immediately, allowing
         the sketch to re-render itself in the resized canvas.
         """
```

### Comparing `proceso-0.0.6/src/proceso/shape.py` & `proceso-0.0.7/src/proceso/shape.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.6/src/proceso/structure.py` & `proceso-0.0.7/src/proceso/structure.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.6/src/proceso/sysvars.py` & `proceso-0.0.7/src/proceso/sysvars.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.6/src/proceso/three_d.py` & `proceso-0.0.7/src/proceso/three_d.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.6/src/proceso/transform.py` & `proceso-0.0.7/src/proceso/transform.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.6/src/proceso/typography.py` & `proceso-0.0.7/src/proceso/typography.py`

 * *Files identical despite different names*

### Comparing `proceso-0.0.6/src/proceso.egg-info/PKG-INFO` & `proceso-0.0.7/src/proceso.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proceso
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python package for creative coding on the web.
 Home-page: https://github.com/nickmcintyre/proceso
 Author: Nick McIntyre
 Author-email: nick@mcintyre.io
 Project-URL: Bug Tracker, https://github.com/nickmcintyre/proceso/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -14,23 +14,23 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # proceso
 > A Python package for creative coding on the web.
 
-proceso provides a Pythonic interface to the [p5.js](https://p5js.org) library. The package is designed for [Pyodide](https://pyodide.org)-based environments including [PyScript](https://pyscript.net) and (soonish) [JupyterLite](https://jupyterlite.readthedocs.io/en/latest/). Similar to [py5](https://py5coding.org/), proceso's goal is to integrate p5.js into the Python ecosystem with thoughtful choices about how to do so in the browser.
+proceso provides a Pythonic interface to the [p5.js](https://p5js.org) library. The package is designed for [Pyodide](https://pyodide.org)-based environments including [PyScript](https://pyscript.net) and (soonish) [JupyterLite](https://jupyterlite.readthedocs.io/en/latest/). Similar to [py5](https://py5coding.org), proceso's goal is to integrate p5.js into the Python ecosystem with thoughtful choices about how to do so in the browser.
 
 Here is an example of how to create a proceso sketch with PyScript:
 ```html
 <!DOCTYPE html>
 <html lang="en-us">
 
 <head>
-    <title>Bouncing Ball</title>
+    <title>My Sketch</title>
     <meta charset="utf-8" />
 
     <link rel="stylesheet" href="https://pyscript.net/releases/2023.03.1/pyscript.css" />
     <script defer src="https://pyscript.net/releases/2023.03.1/pyscript.js"></script>
     <link rel="stylesheet" href="style.css" />
     <script src="https://cdnjs.cloudflare.com/ajax/libs/p5.js/1.6.0/p5.min.js"></script>
     <py-config>
@@ -42,14 +42,51 @@
     <main></main>
     <py-script src="sketch.py"></py-script>
 </body>
 
 </html>
 ```
 
+## Static Sketches
+
+Similar to [Processing](https://processing.org), proceso enables beginners to start programming with "static sketches" before introducing animation and interaction. The following example draws a few shapes and a flower on the screen.
+
+```python
+from proceso import Sketch
+
+
+p5 = Sketch()
+
+# Create the canvas
+p5.create_canvas(720, 400)
+p5.background(200)
+
+# Set colors
+p5.fill(204, 101, 192, 127)
+p5.stroke(127, 63, 120)
+
+# A rectangle
+p5.rect(40, 120, 120, 40)
+# An ellipse
+p5.ellipse(240, 240, 80, 80)
+# A triangle
+p5.triangle(300, 100, 320, 100, 310, 80)
+
+# A design for a simple flower
+p5.translate(580, 200)
+p5.no_stroke()
+for _ in range(10):
+    p5.ellipse(0, 30, 20, 80)
+    p5.rotate(p5.PI / 5)
+```
+
+## Active Sketches
+
+proceso's "active sketches" provide the `run_sketch()` method to handle initialization, looping, and events. The sketch below animates a ball bouncing around the canvas and clears the canvas when a mouse press is detected.
+
 ```python
 from proceso import Sketch
 
 
 p5 = Sketch()
```

### Comparing `proceso-0.0.6/src/proceso.egg-info/SOURCES.txt` & `proceso-0.0.7/src/proceso.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 README.md
 pyproject.toml
 setup.cfg
 src/proceso/__init__.py
 src/proceso/_binding.py
 src/proceso/colors.py
 src/proceso/constants.py
+src/proceso/core.py
 src/proceso/data.py
 src/proceso/dom.py
 src/proceso/environment.py
 src/proceso/events.py
 src/proceso/images.py
+src/proceso/io.py
 src/proceso/rendering.py
 src/proceso/shape.py
 src/proceso/structure.py
 src/proceso/sysvars.py
 src/proceso/three_d.py
 src/proceso/transform.py
 src/proceso/typography.py
```

