# Comparing `tmp/carto_reader-0.0.7.tar.gz` & `tmp/carto_reader-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carto_reader-0.0.7.tar", last modified: Tue Dec  7 10:22:23 2021, max compression
+gzip compressed data, was "/Users/josselin.duchateau/Dropbox/OngoingProjects/CartoReader/dist/.tmp-iapjjsqc/carto_reader-0.0.8.tar", last modified: Wed May  3 12:48:58 2023, max compression
```

## Comparing `carto_reader-0.0.7.tar` & `carto_reader-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 josselin.duchateau (1149608237) 1632634153        0 2021-12-07 10:22:23.531767 carto_reader-0.0.7/
--rw-r--r--   0 josselin.duchateau (1149608237) 1632634153    35148 2021-09-10 16:33:24.000000 carto_reader-0.0.7/LICENSE
--rw-r--r--   0 josselin.duchateau (1149608237) 1632634153     4153 2021-12-07 10:22:23.531900 carto_reader-0.0.7/PKG-INFO
--rw-r--r--   0 josselin.duchateau (1149608237) 1632634153     3650 2021-09-15 10:10:24.000000 carto_reader-0.0.7/README.md
--rw-r--r--   0 josselin.duchateau (1149608237) 1632634153      104 2021-09-10 16:28:39.000000 carto_reader-0.0.7/pyproject.toml
--rw-r--r--   0 josselin.duchateau (1149608237) 1632634153      637 2021-12-07 10:22:23.532603 carto_reader-0.0.7/setup.cfg
-drwxr-xr-x   0 josselin.duchateau (1149608237) 1632634153        0 2021-12-07 10:22:23.525612 carto_reader-0.0.7/src/
-drwxr-xr-x   0 josselin.duchateau (1149608237) 1632634153        0 2021-12-07 10:22:23.529980 carto_reader-0.0.7/src/carto_reader/
--rw-r--r--   0 josselin.duchateau (1149608237) 1632634153       86 2021-09-16 13:43:05.000000 carto_reader-0.0.7/src/carto_reader/__init__.py
--rw-r--r--   0 josselin.duchateau (1149608237) 1632634153     1806 2021-12-06 08:58:29.000000 carto_reader-0.0.7/src/carto_reader/archive.py
--rw-r--r--   0 josselin.duchateau (1149608237) 1632634153     9430 2021-12-06 08:55:00.000000 carto_reader-0.0.7/src/carto_reader/carto_data.py
--rw-r--r--   0 josselin.duchateau (1149608237) 1632634153     8129 2021-12-07 10:21:31.000000 carto_reader-0.0.7/src/carto_reader/mesh.py
--rw-r--r--   0 josselin.duchateau (1149608237) 1632634153     4895 2021-09-17 20:00:27.000000 carto_reader-0.0.7/src/carto_reader/old.py
--rw-r--r--   0 josselin.duchateau (1149608237) 1632634153     9196 2021-12-06 14:48:32.000000 carto_reader-0.0.7/src/carto_reader/points.py
--rw-r--r--   0 josselin.duchateau (1149608237) 1632634153     4301 2021-12-06 14:44:46.000000 carto_reader-0.0.7/src/carto_reader/signals.py
--rw-r--r--   0 josselin.duchateau (1149608237) 1632634153     2586 2021-12-07 10:08:06.000000 carto_reader-0.0.7/src/carto_reader/utils.py
-drwxr-xr-x   0 josselin.duchateau (1149608237) 1632634153        0 2021-12-07 10:22:23.531524 carto_reader-0.0.7/src/carto_reader.egg-info/
--rw-r--r--   0 josselin.duchateau (1149608237) 1632634153     4153 2021-12-07 10:22:23.000000 carto_reader-0.0.7/src/carto_reader.egg-info/PKG-INFO
--rw-r--r--   0 josselin.duchateau (1149608237) 1632634153      459 2021-12-07 10:22:23.000000 carto_reader-0.0.7/src/carto_reader.egg-info/SOURCES.txt
--rw-r--r--   0 josselin.duchateau (1149608237) 1632634153        1 2021-12-07 10:22:23.000000 carto_reader-0.0.7/src/carto_reader.egg-info/dependency_links.txt
--rw-r--r--   0 josselin.duchateau (1149608237) 1632634153       37 2021-12-07 10:22:23.000000 carto_reader-0.0.7/src/carto_reader.egg-info/requires.txt
--rw-r--r--   0 josselin.duchateau (1149608237) 1632634153       13 2021-12-07 10:22:23.000000 carto_reader-0.0.7/src/carto_reader.egg-info/top_level.txt
+drwxr-xr-x   0 josselin.duchateau (1149608237) 1632634153        0 2023-05-03 12:48:58.000000 carto_reader-0.0.8/
+-rw-r--r--   0 josselin.duchateau (1149608237) 1632634153    35148 2021-09-10 16:33:24.000000 carto_reader-0.0.8/LICENSE
+-rw-r--r--   0 josselin.duchateau (1149608237) 1632634153     4097 2023-05-03 12:48:58.000000 carto_reader-0.0.8/PKG-INFO
+-rw-r--r--   0 josselin.duchateau (1149608237) 1632634153     3650 2021-09-15 10:10:24.000000 carto_reader-0.0.8/README.md
+-rw-r--r--   0 josselin.duchateau (1149608237) 1632634153      104 2021-09-10 16:28:39.000000 carto_reader-0.0.8/pyproject.toml
+-rw-r--r--   0 josselin.duchateau (1149608237) 1632634153      637 2023-05-03 12:48:58.000000 carto_reader-0.0.8/setup.cfg
+drwxr-xr-x   0 josselin.duchateau (1149608237) 1632634153        0 2023-05-03 12:48:58.000000 carto_reader-0.0.8/src/
+drwxr-xr-x   0 josselin.duchateau (1149608237) 1632634153        0 2023-05-03 12:48:58.000000 carto_reader-0.0.8/src/carto_reader/
+-rw-r--r--   0 josselin.duchateau (1149608237) 1632634153       86 2021-09-16 13:43:05.000000 carto_reader-0.0.8/src/carto_reader/__init__.py
+-rw-r--r--   0 josselin.duchateau (1149608237) 1632634153     1806 2021-12-06 08:58:29.000000 carto_reader-0.0.8/src/carto_reader/archive.py
+-rw-r--r--   0 josselin.duchateau (1149608237) 1632634153     9411 2023-01-12 20:34:53.000000 carto_reader-0.0.8/src/carto_reader/carto_data.py
+-rw-r--r--   0 josselin.duchateau (1149608237) 1632634153     8131 2023-01-12 20:35:52.000000 carto_reader-0.0.8/src/carto_reader/mesh.py
+-rw-r--r--   0 josselin.duchateau (1149608237) 1632634153     4895 2021-09-17 20:00:27.000000 carto_reader-0.0.8/src/carto_reader/old.py
+-rw-r--r--   0 josselin.duchateau (1149608237) 1632634153     9271 2023-01-12 20:31:19.000000 carto_reader-0.0.8/src/carto_reader/points.py
+-rw-r--r--   0 josselin.duchateau (1149608237) 1632634153     4299 2023-01-12 20:32:01.000000 carto_reader-0.0.8/src/carto_reader/signals.py
+-rw-r--r--   0 josselin.duchateau (1149608237) 1632634153     2586 2021-12-07 10:08:06.000000 carto_reader-0.0.8/src/carto_reader/utils.py
+drwxr-xr-x   0 josselin.duchateau (1149608237) 1632634153        0 2023-05-03 12:48:58.000000 carto_reader-0.0.8/src/carto_reader.egg-info/
+-rw-r--r--   0 josselin.duchateau (1149608237) 1632634153     4097 2023-05-03 12:48:58.000000 carto_reader-0.0.8/src/carto_reader.egg-info/PKG-INFO
+-rw-r--r--   0 josselin.duchateau (1149608237) 1632634153      459 2023-05-03 12:48:58.000000 carto_reader-0.0.8/src/carto_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 josselin.duchateau (1149608237) 1632634153        1 2023-05-03 12:48:58.000000 carto_reader-0.0.8/src/carto_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 josselin.duchateau (1149608237) 1632634153       37 2023-05-03 12:48:58.000000 carto_reader-0.0.8/src/carto_reader.egg-info/requires.txt
+-rw-r--r--   0 josselin.duchateau (1149608237) 1632634153       13 2023-05-03 12:48:58.000000 carto_reader-0.0.8/src/carto_reader.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `carto_reader-0.0.7/LICENSE` & `carto_reader-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `carto_reader-0.0.7/PKG-INFO` & `carto_reader-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: carto_reader
-Version: 0.0.7
+Version: 0.0.8
 Summary: Package to read Carto datasets
-Home-page: UNKNOWN
 Author: Josselin Duchateau
 Author-email: josselin.duchateau@ihu-liryc.fr
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: viz
 License-File: LICENSE
@@ -113,9 +110,7 @@
 
 To visualize a mesh and it's maps, you can call `mesh.plot()`. This method requires pyvista. You can install the dependencies required for signal or mesh plotting using the **viz** option upon install.
 Use the right and left arrow keys to cycle through the available maps.
 
 ### Missing features
  - Importing from non-raw data Carto files
  - Importing the `study.xml` files (especially to get the projected point positions and point tag list)
-
-
```

### Comparing `carto_reader-0.0.7/README.md` & `carto_reader-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `carto_reader-0.0.7/setup.cfg` & `carto_reader-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = carto_reader
-version = 0.0.7
+version = 0.0.8
 author = Josselin Duchateau
 author_email = josselin.duchateau@ihu-liryc.fr
 description = Package to read Carto datasets
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `carto_reader-0.0.7/src/carto_reader/archive.py` & `carto_reader-0.0.8/src/carto_reader/archive.py`

 * *Files identical despite different names*

### Comparing `carto_reader-0.0.7/src/carto_reader/carto_data.py` & `carto_reader-0.0.8/src/carto_reader/carto_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 
     def __repr__(self):
         return f"<Carto Data: {self.__len__()} maps>"
 
     def add_signal_files(self, map_name=None):
         file_list = {file for file in self.data_source.listdir() if file.endswith('Point_Export.xml')}
         if map_name in self:
-            file_list = {file for file in self.data_source.listdir() if file.startswith('map_name')}
+            file_list = {file for file in file_list if file.startswith(map_name)}
         elif map_name is not None:
             raise ValueError('Unknown map')
 
         for file in tqdm(file_list, ncols=50):
             self.add_signal_file(file)
 
     def add_signal_file(self, filename):
```

### Comparing `carto_reader-0.0.7/src/carto_reader/mesh.py` & `carto_reader-0.0.8/src/carto_reader/mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
             return item_list
 
         def read_attributes(_f):
             """ Read the attrivutes section """
             attributes = {}
             for _line in _f:
-                _line = _line.decode('utf-8').rstrip()
+                _line = _line.decode('latin-1').rstrip()
                 if not _line:
                     break
                 if _line[0] == ';':
                     continue
                 name, value = _line.split('=')
                 attributes[name.strip()] = listify(value)
             return MeshAttributes(**attributes)
```

### Comparing `carto_reader-0.0.7/src/carto_reader/old.py` & `carto_reader-0.0.8/src/carto_reader/old.py`

 * *Files identical despite different names*

### Comparing `carto_reader-0.0.7/src/carto_reader/points.py` & `carto_reader-0.0.8/src/carto_reader/points.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
             lat = np.nan
         imp = float(components[13])
         pt_type = int(components[14])
         tag = point_tags(int(components[15])) if point_tags is not None else int(components[15])
         return cls(pt_id, *xyzabg, *unibi, lat, imp, pt_type, tag, cath_id)
 
     def __repr__(self):
-        return f"<Point id='{self.id}' @ {self.x}, {self.y}, {self.z} - bi:{self.uni}, uni:{self.uni}, lat:{self.lat}>"
+        return f"<Point id='{self.id}' @ {self.x}, {self.y}, {self.z} - bi:{self.bi}, uni:{self.uni}, lat:{self.lat}>"
 
     @property
     def pos(self):
         """ Position getter """
         return [self.x, self.y, self.z]
 
     @pos.setter
@@ -186,17 +186,18 @@
         self._points = points if points else {}
 
     @classmethod
     def from_car_file(cls, data_source, filename, point_tags=None):
         """ Read point collection from .car file"""
         with data_source.open(filename) as car_file:
             line = car_file.readline().decode('utf-8')
-            header = re.match(r'VERSION_(?P<version>[\d_])+ (?P<map_name>[^\r\n]+)', line)
-            name = header['map_name']
+            #header = re.match(r'VERSION_(?P<version>[\d_])+ (?P<map_name>[^\r\n]+)', line)
+            #name = header['map_name']
             # version = header['version'].replace('_', '.')
+            name = re.match(r'(?P<study>.*)_car\.txt', filename)['study']
             points = {}
             for line in car_file:
                 pt = Point.from_line(line.decode('utf-8'), point_tags)
                 pt.ref = LazySigRef(data_source, f'{name}_P{pt.id}_Point_Export.xml')
                 points[pt.id] = pt
         return cls(name, points)
```

### Comparing `carto_reader-0.0.7/src/carto_reader/signals.py` & `carto_reader-0.0.8/src/carto_reader/signals.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     def first_sample(self):
         """ First sample of the channel """
         return min((start for start, _ in self._signals))
 
     @property
     def last_sample(self):
         """ Last sample of the channel """
-        return min((start for start, _ in self._signals))
+        return max((stop for _, stop in self._signals))
 
     @property
     def signal_parts(self):
         """ Parts of the channel that contain signal """
         return sorted(self._signals)
 
     def add(self, signal, start_ts: int):
```

### Comparing `carto_reader-0.0.7/src/carto_reader/utils.py` & `carto_reader-0.0.8/src/carto_reader/utils.py`

 * *Files identical despite different names*

### Comparing `carto_reader-0.0.7/src/carto_reader.egg-info/PKG-INFO` & `carto_reader-0.0.8/src/carto_reader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: carto-reader
-Version: 0.0.7
+Version: 0.0.8
 Summary: Package to read Carto datasets
-Home-page: UNKNOWN
 Author: Josselin Duchateau
 Author-email: josselin.duchateau@ihu-liryc.fr
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: viz
 License-File: LICENSE
@@ -113,9 +110,7 @@
 
 To visualize a mesh and it's maps, you can call `mesh.plot()`. This method requires pyvista. You can install the dependencies required for signal or mesh plotting using the **viz** option upon install.
 Use the right and left arrow keys to cycle through the available maps.
 
 ### Missing features
  - Importing from non-raw data Carto files
  - Importing the `study.xml` files (especially to get the projected point positions and point tag list)
-
-
```

