# Comparing `tmp/ypywidgets-0.3.0.tar.gz` & `tmp/ypywidgets-0.4.0.tar.gz`

## Comparing `ypywidgets-0.3.0.tar` & `ypywidgets-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 ypywidgets-0.3.0/ypywidgets/__init__.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 ypywidgets-0.3.0/ypywidgets/reactive.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 ypywidgets-0.3.0/ypywidgets/utils.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 ypywidgets-0.3.0/ypywidgets/ypywidgets.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ypywidgets-0.3.0/README.md
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 ypywidgets-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 ypywidgets-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 ypywidgets-0.4.0/ypywidgets/__init__.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 ypywidgets-0.4.0/ypywidgets/reactive.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 ypywidgets-0.4.0/ypywidgets/utils.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 ypywidgets-0.4.0/ypywidgets/ypywidgets.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ypywidgets-0.4.0/README.md
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 ypywidgets-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 ypywidgets-0.4.0/PKG-INFO
```

### Comparing `ypywidgets-0.3.0/ypywidgets/utils.py` & `ypywidgets-0.4.0/ypywidgets/utils.py`

 * *Files identical despite different names*

### Comparing `ypywidgets-0.3.0/ypywidgets/ypywidgets.py` & `ypywidgets-0.4.0/ypywidgets/ypywidgets.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,27 +11,37 @@
     process_sync_message,
     sync,
 )
 
 
 class Widget:
 
+    _attrs: Optional[Y.YMap]
+
     def __init__(
         self,
         primary: bool = True,
         comm_data: Optional[Dict] = None,
         comm_metadata: Optional[Dict] = None,
+        ydoc: Optional[Y.YDoc] = None,
     ) -> None:
-        self._ydoc = Y.YDoc()
-        self._attrs = self._ydoc.get_map("_attrs")
-        self._attrs.observe(self._set_attr)
+        if ydoc:
+            self._ydoc = ydoc
+            self._attrs = None
+        else:
+            self._ydoc = Y.YDoc()
+            self._attrs = self._ydoc.get_map("_attrs")
+            self._attrs.observe(self._set_attr)
         self._comm = None
         if primary:
             if comm_metadata is None:
-                comm_metadata = {"ymodel_name": self.__class__.__name__}
+                comm_metadata = dict(
+                    ymodel_name=self.__class__.__name__,
+                    create_ydoc=not bool(ydoc),
+                )
             self._comm_id = uuid4().hex
             self._comm = comm.create_comm(
                 comm_id=self._comm_id,
                 target_name="ywidget",
                 data=comm_data,
                 metadata=comm_metadata,
             )
```

### Comparing `ypywidgets-0.3.0/pyproject.toml` & `ypywidgets-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ypywidgets-0.3.0/PKG-INFO` & `ypywidgets-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ypywidgets
-Version: 0.3.0
+Version: 0.4.0
 Summary: Y-based Jupyter widgets for Python
 Project-URL: Homepage, https://github.com/davidbrochart/ypywidgets
 Author-email: David Brochart <david.brochart@gmail.com>
 License-Expression: MIT
 Keywords: jupyter,widgets,yjs,ypy
 Requires-Python: >=3.7
 Requires-Dist: comm<1,>=0.1.2
```

