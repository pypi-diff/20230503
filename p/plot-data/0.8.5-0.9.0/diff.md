# Comparing `tmp/plot_data-0.8.5.tar.gz` & `tmp/plot_data-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plot_data-0.8.5.tar", last modified: Tue Jan 18 10:53:53 2022, max compression
+gzip compressed data, was "plot_data-0.9.0.tar", last modified: Mon Feb 28 15:24:37 2022, max compression
```

## Comparing `plot_data-0.8.5.tar` & `plot_data-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-18 10:53:53.769489 plot_data-0.8.5/
--rw-r--r--   0 root         (0) root         (0)      454 2022-01-18 10:53:53.769489 plot_data-0.8.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      720 2022-01-18 10:49:18.000000 plot_data-0.8.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-18 10:53:53.769489 plot_data-0.8.5/plot_data/
--rw-r--r--   0 root         (0) root         (0)      101 2022-01-18 10:49:18.000000 plot_data-0.8.5/plot_data/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93048 2022-01-18 10:49:18.000000 plot_data-0.8.5/plot_data/colors.py
--rw-r--r--   0 root         (0) root         (0)    41112 2022-01-18 10:49:18.000000 plot_data-0.8.5/plot_data/core.py
--rw-r--r--   0 root         (0) root         (0)     2933 2022-01-18 10:49:18.000000 plot_data-0.8.5/plot_data/graph.py
--rw-r--r--   0 root         (0) root         (0)     4779 2022-01-18 10:49:18.000000 plot_data-0.8.5/plot_data/templates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-18 10:53:53.769489 plot_data-0.8.5/plot_data.egg-info/
--rw-r--r--   0 root         (0) root         (0)      454 2022-01-18 10:53:53.000000 plot_data-0.8.5/plot_data.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      284 2022-01-18 10:53:53.000000 plot_data-0.8.5/plot_data.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-18 10:53:53.000000 plot_data-0.8.5/plot_data.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-01-18 10:53:53.000000 plot_data-0.8.5/plot_data.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-01-18 10:53:53.000000 plot_data-0.8.5/plot_data.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-01-18 10:53:53.769489 plot_data-0.8.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3981 2022-01-18 10:49:18.000000 plot_data-0.8.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-28 15:24:37.021985 plot_data-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)      454 2022-02-28 15:24:37.021985 plot_data-0.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      720 2022-02-28 15:22:50.000000 plot_data-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-28 15:24:37.021985 plot_data-0.9.0/plot_data/
+-rw-r--r--   0 root         (0) root         (0)      101 2022-02-28 15:22:50.000000 plot_data-0.9.0/plot_data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93048 2022-02-28 15:22:50.000000 plot_data-0.9.0/plot_data/colors.py
+-rw-r--r--   0 root         (0) root         (0)    41492 2022-02-28 15:22:50.000000 plot_data-0.9.0/plot_data/core.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2022-02-28 15:22:50.000000 plot_data-0.9.0/plot_data/graph.py
+-rw-r--r--   0 root         (0) root         (0)     4779 2022-02-28 15:22:50.000000 plot_data-0.9.0/plot_data/templates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-28 15:24:37.021985 plot_data-0.9.0/plot_data.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      454 2022-02-28 15:24:36.000000 plot_data-0.9.0/plot_data.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      284 2022-02-28 15:24:37.000000 plot_data-0.9.0/plot_data.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-02-28 15:24:36.000000 plot_data-0.9.0/plot_data.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2022-02-28 15:24:36.000000 plot_data-0.9.0/plot_data.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2022-02-28 15:24:36.000000 plot_data-0.9.0/plot_data.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-02-28 15:24:37.021985 plot_data-0.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3981 2022-02-28 15:22:50.000000 plot_data-0.9.0/setup.py
```

### Comparing `plot_data-0.8.5/README.md` & `plot_data-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `plot_data-0.8.5/plot_data/colors.py` & `plot_data-0.9.0/plot_data/colors.py`

 * *Files identical despite different names*

### Comparing `plot_data-0.8.5/plot_data/core.py` & `plot_data-0.9.0/plot_data/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         DessiaObject.__init__(self, name=name, **kwargs)
 
     def to_dict(self):
         """
         Redefines DessiaObject's to_dict() in order to remove keys where
         value is None.
         """
-        dict_ = DessiaObject.to_dict(self)
+        dict_ = DessiaObject.to_dict(self, use_pointers=False)
         del dict_['object_class']
         new_dict_ = delete_none_from_dict(dict_)
         return new_dict_
 
     @classmethod
     def dict_to_object(cls, dict_):
         """
@@ -163,29 +163,36 @@
     :param text_align_x: "left", "right", "center", "start" or "end". \
     More info on https://www.w3schools.com/tags/canvas_textalign.asp
     :type text_align_x: str
     :param text_align_y: "top", "hanging", "middle", "alphabetic", \
     "ideographic" or "bottom". More info on \
     https://www.w3schools.com/tags/canvas_textbaseline.asp
     :type text_align_y: str
+    :param bold:
+    :type bold: bool
+    :param italic:
+    :type italic: bool
+    :param angle: Text angle in degrees. The angle is clockwise.
+    :type angle: float
     """
 
     def __init__(self, text_color: colors.Color = None,
                  font_size: float = None,
                  font_style: str = None,
                  text_align_x: str = None, text_align_y: str = None,
                  bold: bool = None, italic: bool = None,
-                 name: str = ''):
+                 angle: float = None, name: str = ''):
         self.text_color = text_color
         self.font_size = font_size
         self.font_style = font_style
         self.text_align_x = text_align_x
         self.text_align_y = text_align_y
         self.bold = bold
         self.italic = italic
+        self.angle = angle
         DessiaObject.__init__(self, name=name)
 
 
 class SurfaceStyle(DessiaObject):
     """
     A class for customizing surfaces.
 
@@ -872,22 +879,23 @@
             if not isinstance(value, PrimitiveGroup):
                 primitive_groups[i] = PrimitiveGroup(primitives=value)
         self.primitive_groups = primitive_groups
         if sizes is not None and type(sizes[0]) == int:
             sizes = [sizes] * len(primitive_groups)
         self.sizes = sizes
         self.coords = coords
-        if x_variable or y_variable:
-            attribute_names = []
-            if x_variable:
-                attribute_names.append(x_variable)
-            if y_variable:
-                attribute_names.append(y_variable)
-            self.association = {'associated_elements': associated_elements,
-                                'attribute_names': attribute_names}
+        if associated_elements:
+            self.association = {'associated_elements': associated_elements}
+            if x_variable or y_variable:
+                attribute_names = []
+                if x_variable:
+                    attribute_names.append(x_variable)
+                if y_variable:
+                    attribute_names.append(y_variable)
+                self.association['attribute_names'] = attribute_names
         PlotDataObject.__init__(self, type_='primitivegroupcontainer',
                                 name=name)
 
 
 class ParallelPlot(PlotDataObject):
     """
     Draws a parallel coordinates plot.
@@ -1023,15 +1031,16 @@
         self.initial_view_on = initial_view_on
         PlotDataObject.__init__(self, type_='multiplot', name=name)
 
 
 def plot_canvas(plot_data_object: Subclass[PlotDataObject],
                 debug_mode: bool = False, canvas_id: str = 'canvas',
                 force_version: str = None,
-                width: int = 750, height: int = 400, page_name: str = None):
+                width: int = 750, height: int = 400, page_name: str = None,
+                display: bool = True):
     """
     Creates a html file and plots input data in web browser
 
     :param plot_data_object: a PlotDataObject(ie Scatter, ParallelPlot,\
      MultiplePlots, Graph2D, PrimitiveGroup or PrimitiveGroupContainer)
     :type plot_data_object: Subclass[PlotDataObject]
     :param debug_mode: uses local library if True, uses typescript \
@@ -1085,20 +1094,22 @@
                             canvas_id=canvas_id, width=width, height=height)
     if page_name is None:
         temp_file = tempfile.mkstemp(suffix='.html')[1]
 
         with open(temp_file, 'wb') as file:
             file.write(s.encode('utf-8'))
 
-        webbrowser.open('file://' + temp_file)
+        if display:
+            webbrowser.open('file://' + temp_file)
         print('file://' + temp_file)
     else:
         with open(page_name + '.html', 'wb') as file:
             file.write(s.encode('utf-8'))
-        webbrowser.open('file://' + os.path.realpath(page_name + '.html'))
+        if display:
+            webbrowser.open('file://' + os.path.realpath(page_name + '.html'))
         print(page_name + '.html')
 
 
 def get_csv_vectors(filepath):
     """
     :param filepath: the csv file's relative path, starting from the \
     script's path.
```

### Comparing `plot_data-0.8.5/plot_data/graph.py` & `plot_data-0.9.0/plot_data/graph.py`

 * *Files identical despite different names*

### Comparing `plot_data-0.8.5/plot_data/templates.py` & `plot_data-0.9.0/plot_data/templates.py`

 * *Files identical despite different names*

### Comparing `plot_data-0.8.5/setup.py` & `plot_data-0.9.0/setup.py`

 * *Files identical despite different names*

