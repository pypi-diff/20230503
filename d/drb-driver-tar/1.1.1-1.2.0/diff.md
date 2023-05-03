# Comparing `tmp/drb-driver-tar-1.1.1.tar.gz` & `tmp/drb-driver-tar-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-driver-tar-1.1.1.tar", last modified: Tue Feb 21 13:12:45 2023, max compression
+gzip compressed data, was "drb-driver-tar-1.2.0.tar", last modified: Wed May  3 13:00:01 2023, max compression
```

## Comparing `drb-driver-tar-1.1.1.tar` & `drb-driver-tar-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 13:12:45.943776 drb-driver-tar-1.1.1/
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 12:57:59.000000 drb-driver-tar-1.1.1/LICENCE.txt
--rw-rw-rw-   0 root         (0) root         (0)       58 2022-12-19 13:21:00.000000 drb-driver-tar-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1823 2023-02-21 13:12:45.943776 drb-driver-tar-1.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1202 2022-12-19 13:21:00.000000 drb-driver-tar-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 13:12:45.923775 drb-driver-tar-1.1.1/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 13:12:45.923775 drb-driver-tar-1.1.1/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 13:12:45.947775 drb-driver-tar-1.1.1/drb/drivers/tar/
--rw-rw-rw-   0 root         (0) root         (0)      227 2022-12-19 13:21:00.000000 drb-driver-tar-1.1.1/drb/drivers/tar/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-02-21 13:12:45.947775 drb-driver-tar-1.1.1/drb/drivers/tar/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     6312 2022-12-19 15:00:28.000000 drb-driver-tar-1.1.1/drb/drivers/tar/base_node.py
--rw-rw-rw-   0 root         (0) root         (0)     7700 2022-12-19 13:21:00.000000 drb-driver-tar-1.1.1/drb/drivers/tar/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 13:12:45.943776 drb-driver-tar-1.1.1/drb/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)       97 2022-12-19 13:21:00.000000 drb-driver-tar-1.1.1/drb/exceptions/tar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 13:12:45.923775 drb-driver-tar-1.1.1/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 13:12:45.943776 drb-driver-tar-1.1.1/drb/topics/tar/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 13:21:00.000000 drb-driver-tar-1.1.1/drb/topics/tar/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-12-19 13:21:00.000000 drb-driver-tar-1.1.1/drb/topics/tar/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 13:12:45.943776 drb-driver-tar-1.1.1/drb_driver_tar.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1823 2023-02-21 13:12:45.000000 drb-driver-tar-1.1.1/drb_driver_tar.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      497 2023-02-21 13:12:45.000000 drb-driver-tar-1.1.1/drb_driver_tar.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-21 13:12:45.000000 drb-driver-tar-1.1.1/drb_driver_tar.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-02-21 13:12:45.000000 drb-driver-tar-1.1.1/drb_driver_tar.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-02-21 13:12:45.000000 drb-driver-tar-1.1.1/drb_driver_tar.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-02-21 13:12:45.000000 drb-driver-tar-1.1.1/drb_driver_tar.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-01-13 11:56:57.000000 drb-driver-tar-1.1.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      208 2023-02-21 13:12:45.943776 drb-driver-tar-1.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1316 2023-02-21 13:02:20.000000 drb-driver-tar-1.1.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    78254 2022-06-23 09:49:09.000000 drb-driver-tar-1.1.1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:00:01.974644 drb-driver-tar-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-05-03 12:41:13.000000 drb-driver-tar-1.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-05-03 12:41:13.000000 drb-driver-tar-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1802 2023-05-03 13:00:01.974644 drb-driver-tar-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-05-03 12:41:13.000000 drb-driver-tar-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:00:01.962644 drb-driver-tar-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:00:01.958644 drb-driver-tar-1.2.0/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:00:01.974644 drb-driver-tar-1.2.0/drb/drivers/tar/
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-05-03 12:41:13.000000 drb-driver-tar-1.2.0/drb/drivers/tar/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-03 13:00:01.974644 drb-driver-tar-1.2.0/drb/drivers/tar/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     5205 2023-05-03 12:41:13.000000 drb-driver-tar-1.2.0/drb/drivers/tar/base_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     6716 2023-05-03 12:41:13.000000 drb-driver-tar-1.2.0/drb/drivers/tar/node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:00:01.966644 drb-driver-tar-1.2.0/drb/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-05-03 12:41:13.000000 drb-driver-tar-1.2.0/drb/exceptions/tar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:00:01.962644 drb-driver-tar-1.2.0/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:00:01.970644 drb-driver-tar-1.2.0/drb/topics/tar/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 12:59:39.000000 drb-driver-tar-1.2.0/drb/topics/tar/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-05-03 12:59:39.000000 drb-driver-tar-1.2.0/drb/topics/tar/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:00:01.970644 drb-driver-tar-1.2.0/drb_driver_tar.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1802 2023-05-03 13:00:01.000000 drb-driver-tar-1.2.0/drb_driver_tar.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-03 13:00:01.000000 drb-driver-tar-1.2.0/drb_driver_tar.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 13:00:01.000000 drb-driver-tar-1.2.0/drb_driver_tar.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2023-05-03 13:00:01.000000 drb-driver-tar-1.2.0/drb_driver_tar.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 13:00:01.000000 drb-driver-tar-1.2.0/drb_driver_tar.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-03 13:00:01.000000 drb-driver-tar-1.2.0/drb_driver_tar.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-03 13:00:01.000000 drb-driver-tar-1.2.0/drb_driver_tar.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-03 12:41:13.000000 drb-driver-tar-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-05-03 12:41:13.000000 drb-driver-tar-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-05-03 13:00:01.974644 drb-driver-tar-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-05-03 12:41:13.000000 drb-driver-tar-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:00:01.974644 drb-driver-tar-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    10877 2023-05-03 12:41:13.000000 drb-driver-tar-1.2.0/tests/test_drb_tar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4348 2023-05-03 12:41:13.000000 drb-driver-tar-1.2.0/tests/test_drb_tar_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1646 2023-05-03 12:41:13.000000 drb-driver-tar-1.2.0/tests/test_drb_tar_signature.py
+-rw-rw-rw-   0 root         (0) root         (0)    78254 2023-05-03 12:41:13.000000 drb-driver-tar-1.2.0/versioneer.py
```

### Comparing `drb-driver-tar-1.1.1/LICENCE.txt` & `drb-driver-tar-1.2.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `drb-driver-tar-1.1.1/PKG-INFO` & `drb-driver-tar-1.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: drb-driver-tar
-Version: 1.1.1
+Version: 1.2.0
 Summary: DRB Tar driver
 Home-page: https://gitlab.com/drb-python/impl/tar
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
+License: LGPLv3
 Project-URL: Documentation, https://drb-python.gitlab.io/impl/tar
 Project-URL: Source, https://gitlab.com/drb-python/impl/tar
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
@@ -39,9 +38,7 @@
 ## Using this module
 
 To include this module into your project, the `drb-driver-tar` module shall be referenced into `requirements.txt` file, or the following pip line can be run:
 
 ```commandline
 pip install drb-driver-tar
 ```
-
-
```

### Comparing `drb-driver-tar-1.1.1/README.md` & `drb-driver-tar-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `drb-driver-tar-1.1.1/drb/drivers/tar/base_node.py` & `drb-driver-tar-1.2.0/drb/drivers/tar/base_node.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,93 +15,41 @@
     This node is used to open a tar container, and browse his content.
 
     Parameters:
         base_node (DrbNode): The base node.
     """
     def __init__(self, base_node: DrbNode):
         super().__init__(parent=base_node.parent, tar_info=None, dir=True)
+        self.base_node = base_node
+        self.name = self.base_node.name
+        self.namespace_uri = self.base_node.namespace_uri
+        self.parent = self.base_node.parent
+        self.value = self.base_node.value
         self._all_members = None
         self._tar_file = None
-        self.base_node = base_node
         self._tar_file_source = None
+        for name, namespace in self.base_node.attribute_names():
+            self @= (name, namespace, self.base_node @ (name, namespace))
 
-    @property
-    def parent(self) -> Optional[DrbNode]:
-        """
-        Returns the parent of the base node.
+    def __setitem__(self, key, value):
+        raise NotImplementedError
 
-        Returns:
-            DrbNode: the parent of the node
-        """
-        return self.base_node.parent
+    def __delitem__(self, key):
+        raise NotImplementedError
 
     @property
     def path(self) -> ParsedPath:
         """
         Returns the path of the base node.
 
         Returns:
             ParsedPath: the full path of the base node
         """
         return self.base_node.path
 
-    @property
-    def name(self) -> str:
-        """
-        Return the name of the base node.
-        This name doesn't contain the path.
-
-        Returns:
-            str: the base node name
-        """
-        return self.base_node.name
-
-    @property
-    def namespace_uri(self) -> Optional[str]:
-        """
-        Return the namespace uri of the base node.
-
-        Returns:
-            str: the base node namespace
-        """
-        return self.base_node.namespace_uri
-
-    @property
-    def value(self) -> Optional[Any]:
-        """
-        Return the value of the base node.
-
-        Returns:
-            Any: the value
-        """
-        return self.base_node.value
-
-    @property
-    def attributes(self) -> Dict[Tuple[str, str], Any]:
-        """
-        Return the attributes of the base node.
-
-        Returns:
-            Dict: Key(key_name, key_namespace): value(Any)
-        """
-        return self.base_node.attributes
-
-    def get_attribute(self, name: str, namespace_uri: str = None) -> Any:
-        """
-        Return a specific attributes of the base node.
-
-        Parameters:
-            name (str): The name of the attribute.
-            namespace_uri (str): The namespace_uri of the attribute
-                                 (default: None).
-        Returns:
-            Any: the attribute
-        """
-        return self.base_node.get_attribute(name, namespace_uri)
-
     def name_entry(self):
         return ''
 
     @property
     def tar_file(self) -> tarfile.TarFile:
         if self._tar_file is None:
             try:
@@ -164,18 +112,19 @@
             if any(filename.startswith(name_entry) and filename != name_entry
                    for name_entry in self.tar_file.getnames()):
                 return False
 
             paths_array = Path(filename).parts
 
             if len(paths_array) == 1 or (
-                    len(paths_array) == 2 and paths_array[0] == '/'):
+                    len(paths_array) == 2 and
+                    Path(paths_array[0]).as_posix() == '/'):
                 continue
 
-            if paths_array[0] == '/':
+            if Path(paths_array[0]).as_posix() == '/':
                 name_sub_dir = paths_array[1]
             else:
                 name_sub_dir = paths_array[0]
 
             found = False
             for child in self._children:
                 if child.name == name_sub_dir:
```

### Comparing `drb-driver-tar-1.1.1/drb/drivers/tar/node.py` & `drb-driver-tar-1.2.0/drb/drivers/tar/node.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,18 @@
+from deprecated import deprecated
+from pathlib import Path
+from tarfile import ExFileObject, TarInfo, DIRTYPE
+from typing import Any, List
+from drb.core.node import DrbNode
+from drb.nodes.abstract_node import AbstractNode
+from drb.exceptions.core import DrbNotImplementationException
 import os
-
 import datetime
 import enum
-from tarfile import ExFileObject, TarInfo, DIRTYPE
-from typing import Any, List, Dict, Tuple, Optional
-
 import drb.topics.resolver as resolver
-from drb.core.node import DrbNode
-from drb.nodes.abstract_node import AbstractNode
-from drb.exceptions.core import DrbNotImplementationException, DrbException
-from drb.core.path import ParsedPath
-from pathlib import Path
 
 
 class DrbTarAttributeNames(enum.Enum):
     SIZE = 'size'
     """
     The size of the file in bytes.
     """
@@ -37,92 +35,65 @@
         parent (DrbNode): The zip container.
         tar_info (ZipInfo): Class with attributes describing
                             each file in the ZIP archive.
 
     """
 
     def __init__(self, parent: DrbNode, tar_info: TarInfo = None,
-                 name=None,
-                 dir=False):
+                 name=None, dir=False):
         super().__init__()
         self._tar_info = tar_info
-        self._attributes: Dict[Tuple[str, str], Any] = None
-        self._name = name
-        self._parent: DrbNode = parent
+        self.name = name if tar_info is None \
+            else self.__init_name(name, tar_info)
+        self.parent: DrbNode = parent
         self._children: List[DrbNode] = None
-        self._path = None
-        self._dir = dir
-        if tar_info is not None and tar_info.type == DIRTYPE:
-            self._dir = True
+        self._dir = dir if tar_info is None else tar_info.type == DIRTYPE
+        self.__init_attributes()
+        self._available_impl.clear()
+        if not self @ DrbTarAttributeNames.DIRECTORY.value:
+            self._available_impl.append(ExFileObject)
+
+    def __setitem__(self, key, value):
+        raise NotImplementedError
+
+    def __delitem__(self, item):
+        raise NotImplementedError
+
+    def __init_attributes(self):
+        name_attribute = DrbTarAttributeNames.DIRECTORY.value
+        self @= (name_attribute, None, self._dir)
+        if self._tar_info is not None:
+            name_attribute = DrbTarAttributeNames.SIZE.value
+            self @= (name_attribute, None, self._tar_info.size)
 
-    @property
-    def parent(self) -> Optional[DrbNode]:
-        return self._parent
+            date_time = datetime.datetime.fromtimestamp(self._tar_info.mtime)
+            name_attribute = DrbTarAttributeNames.MODIFIED.value
+            self @= (name_attribute, None, date_time.strftime("%c"))
 
-    @property
-    def path(self) -> ParsedPath:
-        if self._path is None:
-            self._path = self.parent.path / self.name
-        return self._path
+    @staticmethod
+    def __init_name(name: str, tar_info: TarInfo) -> str:
+        n = name
+        if tar_info is not None:
+            if tar_info.name.endswith('/'):
+                n = tar_info.name[:-1]
+            else:
+                n = tar_info.name
+            if '/' in n:
+                return n[n.rindex('/') + 1:]
+        return n
 
     def name_entry(self):
         if self._tar_info is not None:
             return self._tar_info.name
         else:
-            name_entry = self.parent.name_entry() + self._name
+            name_entry = self.parent.name_entry() + self.name
             if self._dir:
-                name_entry += os.sep
+                name_entry += '/'
             return name_entry
 
-    @property
-    def name(self) -> str:
-        if self._name is None:
-            if self._tar_info.name.endswith('/'):
-                self._name = self._tar_info.name[:-1]
-            else:
-                self._name = self._tar_info.name
-            if '/' in self._name:
-                self._name = self._name[self._name .rindex('/') + 1:]
-        return self._name
-
-    @property
-    def namespace_uri(self) -> Optional[str]:
-        return None
-
-    @property
-    def value(self) -> Optional[Any]:
-        return None
-
-    @property
-    def attributes(self) -> Dict[Tuple[str, str], Any]:
-        if self._attributes is None:
-            self._attributes = {}
-            name_attribute = DrbTarAttributeNames.DIRECTORY.value
-            self._attributes[name_attribute, None] = self._dir
-
-            if self._tar_info is not None:
-                name_attribute = DrbTarAttributeNames.SIZE.value
-                self._attributes[name_attribute, None] = self._tar_info.size
-
-                date_time = datetime.datetime.fromtimestamp(
-                    self._tar_info.mtime)
-
-                name_attribute = DrbTarAttributeNames.MODIFIED.value
-                self._attributes[name_attribute, None] = \
-                    date_time.strftime("%c")
-
-        return self._attributes
-
-    def get_attribute(self, name: str, namespace_uri: str = None) -> Any:
-        key = (name, namespace_uri)
-        if key in self.attributes.keys():
-            return self.attributes[key]
-        raise DrbException(f'Attribute not found name: {name}, '
-                           f'namespace: {namespace_uri}')
-
     @staticmethod
     def is_a_subdir(entry) -> bool:
         if os.path.basename(entry.name) is not None and len(
                 os.path.basename(entry.name)) > 1:
             return False
 
         paths_array = Path(entry.name).parts
@@ -207,14 +178,15 @@
             return True
 
         # Either the name do not contains sep either only one a last position
         return '/' not in filename
 
     @property
     @resolver.resolve_children
+    @deprecated(version='2.1.0')
     def children(self) -> List[DrbNode]:
 
         if self._children is None:
             self._children = []
 
             for entry in self.get_members():
                 if self._is_a_child(entry.name):
@@ -226,20 +198,14 @@
             self._add_sub_child()
 
             self._children = sorted(self._children,
                                     key=lambda entry_cmp: entry_cmp.name)
 
         return self._children
 
-    def has_impl(self, impl: type) -> bool:
-        if issubclass(ExFileObject, impl):
-            return not self.get_attribute(DrbTarAttributeNames.DIRECTORY.value,
-                                          None)
-        return False
-
     def get_impl(self, impl: type, **kwargs) -> Any:
         if self.has_impl(impl):
             return self.parent.open_member(self._tar_info)
         raise DrbNotImplementationException(f'no {impl} '
                                             f'implementation found')
 
     def close(self):
```

### Comparing `drb-driver-tar-1.1.1/drb_driver_tar.egg-info/PKG-INFO` & `drb-driver-tar-1.2.0/drb_driver_tar.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: drb-driver-tar
-Version: 1.1.1
+Version: 1.2.0
 Summary: DRB Tar driver
 Home-page: https://gitlab.com/drb-python/impl/tar
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
+License: LGPLv3
 Project-URL: Documentation, https://drb-python.gitlab.io/impl/tar
 Project-URL: Source, https://gitlab.com/drb-python/impl/tar
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
@@ -39,9 +38,7 @@
 ## Using this module
 
 To include this module into your project, the `drb-driver-tar` module shall be referenced into `requirements.txt` file, or the following pip line can be run:
 
 ```commandline
 pip install drb-driver-tar
 ```
-
-
```

### Comparing `drb-driver-tar-1.1.1/versioneer.py` & `drb-driver-tar-1.2.0/versioneer.py`

 * *Files identical despite different names*

