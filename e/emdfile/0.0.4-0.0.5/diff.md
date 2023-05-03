# Comparing `tmp/emdfile-0.0.4.tar.gz` & `tmp/emdfile-0.0.5.tar.gz`

## Comparing `emdfile-0.0.4.tar` & `emdfile-0.0.5.tar`

### file list

```diff
@@ -1,49 +1,48 @@
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 emdfile-0.0.4/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 emdfile-0.0.4/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 emdfile-0.0.4/.pytest_cache/README.md
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 emdfile-0.0.4/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 emdfile-0.0.4/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.4/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     8681 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/README.md
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/__init__.py
--rw-r--r--   0        0        0    10373 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/read.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/tqdmnd.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/version.py
--rw-r--r--   0        0        0    31055 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/write.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/classes/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/classes/array.py
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/classes/custom.py
--rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/classes/metadata.py
--rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/classes/pointlist.py
--rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/classes/pointlistarray.py
--rw-r--r--   0        0        0    23442 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/classes/tree.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 emdfile-0.0.4/src/emdfile/classes/utils.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 emdfile-0.0.4/test/clear_h5_files.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 emdfile-0.0.4/test/test_base_classes.py
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 emdfile-0.0.4/test/test_emd.py
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 emdfile-0.0.4/test/test_header.py
--rw-r--r--   0        0        0    28996 2020-02-02 00:00:00.000000 emdfile-0.0.4/test/test_tree.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 emdfile-0.0.4/test/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 emdfile-0.0.4/test/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 emdfile-0.0.4/test/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.4/test/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 emdfile-0.0.4/test/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.4/test/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0   384837 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/emdfile_intro_example.ipynb
--rw-r--r--   0        0        0   167826 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/emdfile_package_walkthrough.ipynb
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/test_custom_class.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/.pytest_cache/README.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0    81358 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/pngs/node.png
--rw-r--r--   0        0        0    41590 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/pngs/tree.png
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/sample_custom_class_module/__init__.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 emdfile-0.0.4/tutorials/sample_custom_class_module/my_custom_classes.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 emdfile-0.0.4/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 emdfile-0.0.4/LICENSE
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 emdfile-0.0.4/README.md
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 emdfile-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 emdfile-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 emdfile-0.0.5/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 emdfile-0.0.5/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 emdfile-0.0.5/.pytest_cache/README.md
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 emdfile-0.0.5/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 emdfile-0.0.5/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.5/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/__init__.py
+-rw-r--r--   0        0        0    10788 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/read.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/tqdmnd.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/version.py
+-rw-r--r--   0        0        0    31055 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/write.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/classes/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/classes/array.py
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/classes/custom.py
+-rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/classes/metadata.py
+-rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/classes/pointlist.py
+-rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/classes/pointlistarray.py
+-rw-r--r--   0        0        0    23786 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/classes/tree.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/classes/utils.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 emdfile-0.0.5/test/clear_h5_files.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 emdfile-0.0.5/test/test_base_classes.py
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 emdfile-0.0.5/test/test_emd.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 emdfile-0.0.5/test/test_header.py
+-rw-r--r--   0        0        0    28996 2020-02-02 00:00:00.000000 emdfile-0.0.5/test/test_tree.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 emdfile-0.0.5/test/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 emdfile-0.0.5/test/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 emdfile-0.0.5/test/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.5/test/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 emdfile-0.0.5/test/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.5/test/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0   384837 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/emdfile_intro_example.ipynb
+-rw-r--r--   0        0        0   167826 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/emdfile_package_walkthrough.ipynb
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/test_custom_classes.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/.pytest_cache/README.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0    81358 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/pngs/node.png
+-rw-r--r--   0        0        0    41590 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/pngs/tree.png
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/sample_custom_emd_classes/__init__.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/sample_custom_emd_classes/my_custom_classes.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 emdfile-0.0.5/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 emdfile-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 emdfile-0.0.5/README.md
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 emdfile-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 emdfile-0.0.5/PKG-INFO
```

### Comparing `emdfile-0.0.4/.pytest_cache/v/cache/lastfailed` & `emdfile-0.0.5/.pytest_cache/v/cache/lastfailed`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.4/.pytest_cache/v/cache/nodeids` & `emdfile-0.0.5/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.4/src/emdfile/__init__.py` & `emdfile-0.0.5/src/emdfile/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -35,15 +35,16 @@
 # read/write
 
 from emdfile.read import (
     read,
     print_h5_tree,
     _is_EMD_file,
     _get_EMD_version,
-    _version_is_geq
+    _version_is_geq,
+    _read_metadata
 )
 from emdfile.write import write as save
 
 
 
 
 # version
```

### Comparing `emdfile-0.0.4/src/emdfile/read.py` & `emdfile-0.0.5/src/emdfile/read.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 import warnings
 
 
 # Classes
 from emdfile.classes import (
     Root,
     Node,
-    RootedNode
+    RootedNode,
+    Metadata
 )
 from emdfile.classes.utils import (
     _get_class,
     EMD_data_group_types
 )
 
 
@@ -334,9 +335,29 @@
             linelevels=linelevels,
             show_metadata=show_metadata)
 
     pass
 
 
 
+def _read_metadata(
+    group,
+    name
+    ):
+    """
+    Returns a Metadata instance called name stored in the EMD node at group.
+    Returns False otherwise.
+    """
+    try:
+        grp_metadata = group['metadatabundle']
+    except KeyError:
+        return False
+    try:
+        metadata = Metadata.from_h5(grp_metadata[name])
+        return metadata
+    except KeyError:
+        return False
+
+
+
```

### Comparing `emdfile-0.0.4/src/emdfile/tqdmnd.py` & `emdfile-0.0.5/src/emdfile/tqdmnd.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.4/src/emdfile/write.py` & `emdfile-0.0.5/src/emdfile/write.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.4/src/emdfile/classes/array.py` & `emdfile-0.0.5/src/emdfile/classes/array.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.4/src/emdfile/classes/custom.py` & `emdfile-0.0.5/src/emdfile/classes/custom.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.4/src/emdfile/classes/metadata.py` & `emdfile-0.0.5/src/emdfile/classes/metadata.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.4/src/emdfile/classes/pointlist.py` & `emdfile-0.0.5/src/emdfile/classes/pointlist.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.4/src/emdfile/classes/pointlistarray.py` & `emdfile-0.0.5/src/emdfile/classes/pointlistarray.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.4/src/emdfile/classes/tree.py` & `emdfile-0.0.5/src/emdfile/classes/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -382,20 +382,26 @@
     ## end tree
 
 
 
     # decorator for storing params which generated new data nodes
 
     @staticmethod
-    def log_new_node(method):
-        """ Node subclass methods which generate and return a new node may
-        be decorated with @log_new_node. This method creates a new Metadata
-        dict stored inside `new_node.metadata` called `_fn_call_*`, where *
-        is the name of the decorated method, which stores the args/kwargs/params
-        passed to the generating method.
+    def newnode(method):
+        """
+        Decorator which may be added to node methods which product and
+        return a new node.  If such a method is decorated with
+
+        >>> @newnode
+
+        then the new node is added to the parent node's tree, and a
+        Metadata instance is added to the new node's metadata which
+        stores information about how the node was created, namely:
+        method's name, the parent's class and name, and all
+        the arguments passed to method.
         """
 
         @functools.wraps(method)
         def wrapper(*args, **kwargs):
 
             # Get the called method name
             method_name = method.__name__
@@ -406,45 +412,50 @@
             # Pair args with names
             method_args = inspect.getfullargspec(method)[0]
             d = dict()
             for i in range(len(args)):
                 d[method_args[i]] = args[i]
 
             # Add the generating class type and name
-            d['generating_class'] = self.__class__
-            d['generating_name'] = self.name
-            d['method'] = method_name
+            d['parent_class'] = self.__class__
+            d['parent_name'] = self.name
+            d['parent_method'] = method_name
 
             # Combine with kwargs
             kwargs.update(d)
+            # and make the metadata
+            md = Metadata( name = "_fn_call_" + method_name )
+            md._params.update( kwargs )
 
-            # Run the method and get the returned node
+            # Run the method, get the returned node
             new_node = method(*args,**kwargs)
 
-            # Make and add the metadata
-            md = Metadata( name = "_fn_call_" + method_name )
-            md._params.update( kwargs )
+            # Add the metadata to the node
             new_node.metadata = md
 
+            # Add the new node to the parent node's tree
+            self.tree(new_node)
+
             # Return
             return new_node
 
         return wrapper
 
 
 
 
     # read
 
     # this machinery is designed to work with and be extendible
     # in the context of child classes.
 
     # to add a new child class, only a new _get_constructor_args()
-    # classmethod should be necessary. The .from_h5 function should
-    # not need any modification.
+    # classmethod should be necessary. If a class needs additional
+    # construction post-initialization, define a _populate_instance()
+    # method. The .from_h5 function should not need any modification.
 
     @classmethod
     def _get_constructor_args(cls,group):
         """
         Takes a group, and returns a dictionary of args/values
         to pass to the class constructor
         """
@@ -699,12 +710,7 @@
             string += "\n"+space+f"    {k} \t\t ({v.__class__.__name__})"
         string += "\n)"
         return string
 
 
 
 
-
-
-
-
-
```

### Comparing `emdfile-0.0.4/src/emdfile/classes/utils.py` & `emdfile-0.0.5/src/emdfile/classes/utils.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.4/test/clear_h5_files.py` & `emdfile-0.0.5/test/clear_h5_files.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.4/test/test_base_classes.py` & `emdfile-0.0.5/test/test_base_classes.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.4/test/test_emd.py` & `emdfile-0.0.5/test/test_emd.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.4/test/test_header.py` & `emdfile-0.0.5/test/test_header.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.4/test/test_tree.py` & `emdfile-0.0.5/test/test_tree.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.4/test/.pytest_cache/v/cache/nodeids` & `emdfile-0.0.5/test/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.4/tutorials/emdfile_intro_example.ipynb` & `emdfile-0.0.5/tutorials/emdfile_intro_example.ipynb`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.4/tutorials/emdfile_package_walkthrough.ipynb` & `emdfile-0.0.5/tutorials/emdfile_package_walkthrough.ipynb`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.4/tutorials/test_custom_class.py` & `emdfile-0.0.5/tutorials/test_custom_classes.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,58 @@
 import emdfile as emd
 
 import numpy as np
-from os.path import exists
-from os import remove
 
-from sample_custom_class_module import (
+from sample_custom_emd_classes import (
     MyArrayClass,
     MyPointsClass,
     MyCustomClass
 )
 
-
-# prepare filepath
+# set filepath
 filepath = "/Users/Ben/Desktop/test.h5"
-if exists(filepath):
-    remove(filepath)
-
-
-
-
-
-# instantiate the test classes
-
-
-array_instance = MyArrayClass(
-    name = 'test_array_instance',
-    data = np.ones((2,3))
-)
-
-points_instance = MyPointsClass(
-    name = 'test_points_instance',
-    x = np.arange(10),
-    y = np.arange(10,20),
-)
-
-custom_instance = MyCustomClass(
-    name = 'test_custom_instance',
-    data = np.arange(12).reshape((3,4))
-)
-
-
-
-# save
-emd.save(
-    filepath,
-    [array_instance, points_instance, custom_instance]
-)
-
-
-
-
-# load
-loaded_data = emd.read(filepath)
 
 
+if __name__ == "__main__":
 
-print(loaded_data)
-print()
-loaded_data.tree()
-print()
-print(loaded_data.tree('test_array_instance').data)
-print()
-print(loaded_data.tree('test_points_instance').data)
-print()
-print(loaded_data.tree('test_custom_instance').data)
+    # instantiate the test classes
+    array_instance = MyArrayClass(
+        name = 'test_array_instance',
+        data = np.ones((2,3))
+    )
+    points_instance = MyPointsClass(
+        name = 'test_points_instance',
+        x = np.arange(10),
+        y = np.arange(10,20),
+    )
+    custom_instance = MyCustomClass(
+        name = 'test_custom_instance',
+        data = np.arange(12).reshape((3,4))
+    )
+
+    # save
+    emd.save(
+        filepath,
+        [array_instance, points_instance, custom_instance],
+        mode = 'o'
+    )
+
+    # load
+    loaded_data = emd.read(filepath)
+
+    # display
+    print("Loaded data:")
+    print(loaded_data)
+    print()
+    print("Loaded tree:")
+    loaded_data.tree()
+    print()
+    print("data")
+    print(loaded_data.tree('test_array_instance').data)
+    print()
+    print(loaded_data.tree('test_points_instance').data)
+    print()
+    print(loaded_data.tree('test_custom_instance').data)
```

### Comparing `emdfile-0.0.4/tutorials/pngs/node.png` & `emdfile-0.0.5/tutorials/pngs/node.png`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.4/tutorials/pngs/tree.png` & `emdfile-0.0.5/tutorials/pngs/tree.png`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.4/tutorials/sample_custom_class_module/my_custom_classes.py` & `emdfile-0.0.5/tutorials/sample_custom_emd_classes/my_custom_classes.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.4/LICENSE` & `emdfile-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.4/README.md` & `emdfile-0.0.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,42 +4,43 @@
 is designed to carry arbitrary data and metadata.  An overview of the
 file specification can be found [here](https://emdatasets.com/format/).
 
 
 `emdfile` is a Python package defining write and read functions and a set of
 classes which together interface between EMD 1.0 files and Python runtime
 objects.  The classes are designed to quickly build, save to, and read from
-filetree-like representations of data and metadata.
+filetree-like representations of data and metadata, and is built on HDF5+h5py.
 
 
 ## Installation
 
 Run
 
 > pip install emdfile
 
-Or, to install from source code, clone this repository and from the
+Or, to install from source code, you can clone this repository and from the
 distribution level directory (i.e. where pyproject.toml lives) run
 
 > pip install .
 
 
 
 ## Examples and syntax
 
-For a narrative introduction, see
-[tutorials/emd_narrative_intro.md](tutorials/emd_narrative_intro.md).
 
-For an example, see
-[tutorials/emd_intro_example.ipynb](./tutorials/emd_intro_example.ipynb).
+For a few simple examples...
+(([this is coming extremely soon ish!](https://www.youtube.com/watch?v=ebeNeQFUMa0)))
 
-For an walkthrough of the syntax, see
-[tutorials/emd_package_walkthrough.ipynb](./tutorials/emd_package_walkthrough.ipynb).
+For a longer, narrative intro example, see
+[tutorials/emd_intro_example.ipynb](https://github.com/py4dstem/emdfile/blob/main/tutorials/emdfile_intro_example.ipynb).
 
-For an example of a downstream Python package using emdfile for IO, see
-[tutorials/test_custom_class.py](./tutorials/test_custom_class.py) and
-[tutorials/sample_custom_class_module](./tutorials/sample_custom_class_module).
+For a detailed walkthrough of the syntax, see
+[tutorials/emd_package_walkthrough.ipynb](https://github.com/py4dstem/emdfile/blob/main/tutorials/emdfile_package_walkthrough.ipynb).
+
+
+`emdfile` is designed to support I/O in downstream Python modules and packages.
+When [tutorials/test_custom_classes.py](https://github.com/py4dstem/emdfile/blob/main/tutorials/test_custom_classes.py) is run as a script, it makes, saves, loads, then prints the contents of the data carrying classes defined in the [tutorials/sample_custom_emd_classes](https://github.com/py4dstem/emdfile/tree/main/tutorials/sample_custom_emd_classes) Python module.
```

### Comparing `emdfile-0.0.4/pyproject.toml` & `emdfile-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.4/PKG-INFO` & `emdfile-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emdfile
-Version: 0.0.4
+Version: 0.0.5
 Project-URL: github, https://github.com/py4dstem/emdfile
 Project-URL: emdatasets, https://emdatasets.com/format/
 Author-email: "Benjamin H. Savitzky" <ben.savitzky@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -20,42 +20,43 @@
 is designed to carry arbitrary data and metadata.  An overview of the
 file specification can be found [here](https://emdatasets.com/format/).
 
 
 `emdfile` is a Python package defining write and read functions and a set of
 classes which together interface between EMD 1.0 files and Python runtime
 objects.  The classes are designed to quickly build, save to, and read from
-filetree-like representations of data and metadata.
+filetree-like representations of data and metadata, and is built on HDF5+h5py.
 
 
 ## Installation
 
 Run
 
 > pip install emdfile
 
-Or, to install from source code, clone this repository and from the
+Or, to install from source code, you can clone this repository and from the
 distribution level directory (i.e. where pyproject.toml lives) run
 
 > pip install .
 
 
 
 ## Examples and syntax
 
-For a narrative introduction, see
-[tutorials/emd_narrative_intro.md](tutorials/emd_narrative_intro.md).
 
-For an example, see
-[tutorials/emd_intro_example.ipynb](./tutorials/emd_intro_example.ipynb).
+For a few simple examples...
+(([this is coming extremely soon ish!](https://www.youtube.com/watch?v=ebeNeQFUMa0)))
 
-For an walkthrough of the syntax, see
-[tutorials/emd_package_walkthrough.ipynb](./tutorials/emd_package_walkthrough.ipynb).
+For a longer, narrative intro example, see
+[tutorials/emd_intro_example.ipynb](https://github.com/py4dstem/emdfile/blob/main/tutorials/emdfile_intro_example.ipynb).
 
-For an example of a downstream Python package using emdfile for IO, see
-[tutorials/test_custom_class.py](./tutorials/test_custom_class.py) and
-[tutorials/sample_custom_class_module](./tutorials/sample_custom_class_module).
+For a detailed walkthrough of the syntax, see
+[tutorials/emd_package_walkthrough.ipynb](https://github.com/py4dstem/emdfile/blob/main/tutorials/emdfile_package_walkthrough.ipynb).
+
+
+`emdfile` is designed to support I/O in downstream Python modules and packages.
+When [tutorials/test_custom_classes.py](https://github.com/py4dstem/emdfile/blob/main/tutorials/test_custom_classes.py) is run as a script, it makes, saves, loads, then prints the contents of the data carrying classes defined in the [tutorials/sample_custom_emd_classes](https://github.com/py4dstem/emdfile/tree/main/tutorials/sample_custom_emd_classes) Python module.
```

