# Comparing `tmp/tKot-0.1.3.tar.gz` & `tmp/tKot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tKot-0.1.3.tar", last modified: Wed Mar  1 11:09:28 2023, max compression
+gzip compressed data, was "tKot-0.2.0.tar", last modified: Wed May  3 11:22:09 2023, max compression
```

## Comparing `tKot-0.1.3.tar` & `tKot-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-01 11:09:28.368742 tKot-0.1.3/
--rw-rw-rw-   0        0        0      483 2023-03-01 11:09:28.367742 tKot-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       30 2023-02-27 11:57:31.000000 tKot-0.1.3/README.md
--rw-rw-rw-   0        0        0      602 2023-03-01 11:03:03.000000 tKot-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-01 11:09:28.369743 tKot-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      311 2023-02-27 12:07:32.000000 tKot-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-01 11:09:28.312573 tKot-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-03-01 11:09:28.324656 tKot-0.1.3/src/tKot/
--rw-rw-rw-   0        0        0       60 2023-02-28 12:42:47.000000 tKot-0.1.3/src/tKot/__init__.py
--rw-rw-rw-   0        0        0      724 2023-02-28 05:07:43.000000 tKot-0.1.3/src/tKot/buttons.py
--rw-rw-rw-   0        0        0     2972 2023-03-01 11:02:44.000000 tKot-0.1.3/src/tKot/frames.py
-drwxrwxrwx   0        0        0        0 2023-03-01 11:09:28.363742 tKot-0.1.3/src/tKot.egg-info/
--rw-rw-rw-   0        0        0      483 2023-03-01 11:09:28.000000 tKot-0.1.3/src/tKot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-03-01 11:09:28.000000 tKot-0.1.3/src/tKot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-01 11:09:28.000000 tKot-0.1.3/src/tKot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-03-01 11:09:28.000000 tKot-0.1.3/src/tKot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-01 11:09:28.000000 tKot-0.1.3/src/tKot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 11:22:09.667208 tKot-0.2.0/
+-rw-rw-rw-   0        0        0      483 2023-05-03 11:22:09.666207 tKot-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2023-02-27 11:57:31.000000 tKot-0.2.0/README.md
+-rw-rw-rw-   0        0        0      602 2023-05-03 11:18:28.000000 tKot-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 11:22:09.667208 tKot-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      311 2023-02-27 12:07:32.000000 tKot-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:22:09.642177 tKot-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 11:22:09.653176 tKot-0.2.0/src/tKot/
+-rw-rw-rw-   0        0        0       60 2023-02-28 12:42:47.000000 tKot-0.2.0/src/tKot/__init__.py
+-rw-rw-rw-   0        0        0      874 2023-05-03 11:18:28.000000 tKot-0.2.0/src/tKot/buttons.py
+-rw-rw-rw-   0        0        0     2972 2023-05-03 11:19:55.000000 tKot-0.2.0/src/tKot/frames.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:22:09.664176 tKot-0.2.0/src/tKot.egg-info/
+-rw-rw-rw-   0        0        0      483 2023-05-03 11:22:09.000000 tKot-0.2.0/src/tKot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-05-03 11:22:09.000000 tKot-0.2.0/src/tKot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 11:22:09.000000 tKot-0.2.0/src/tKot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-03 11:22:09.000000 tKot-0.2.0/src/tKot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-03 11:22:09.000000 tKot-0.2.0/src/tKot.egg-info/top_level.txt
```

### Comparing `tKot-0.1.3/pyproject.toml` & `tKot-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requeres = ["setuptools", "setuptools-scm"]
 build-backed = "setuptools.build_meta"
 
 [project]
 name = "tKot"
-version = "0.1.3"
+version = "0.2.0"
 authors = [
     {name="Serj Kotilevski", email="youserj@outlook.com"}
 ]
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `tKot-0.1.3/src/tKot/buttons.py` & `tKot-0.2.0/src/tKot/buttons.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import tkinter as tk
 from PIL import Image, ImageTk
 
 
-class Icon(tk.Button):
+class Icon(tk.Widget):
     p_im: Image.Image | None
     im: ImageTk.PhotoImage | None
     info: str | None
 
-    def __init__(self, pillow_image: Image = None,
-                 **kwargs):
-        super(Icon, self).__init__(**kwargs)
-        self.p_im = pillow_image
+    def __init__(self, master=None, **kw):
+        self.p_im = kw.pop("pillow_image", None)
+        if kw.pop("with_fix", None):
+            kw["indicatoron"] = False
+            tk.Widget.__init__(self, master, "checkbutton", kw)
+        else:
+            tk.Widget.__init__(self, master, "button", kw)
         self.im = None
         self.bind("<Configure>", self.__handle_configure)
 
     def __handle_configure(self, e: tk.Event):
         """auto change image size"""
         if self.p_im:
             h = self.winfo_height()
```

### Comparing `tKot-0.1.3/src/tKot/frames.py` & `tKot-0.2.0/src/tKot/frames.py`

 * *Files identical despite different names*

