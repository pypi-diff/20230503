# Comparing `tmp/malla-0.1.5.tar.gz` & `tmp/malla-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malla-0.1.5.tar", max compression
+gzip compressed data, was "malla-0.1.6.tar", max compression
```

## Comparing `malla-0.1.5.tar` & `malla-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      526 2023-04-29 16:35:40.386927 malla-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-04-25 21:01:58.416728 malla-0.1.5/malla/__init__.py
--rw-r--r--   0        0        0     6062 2023-05-03 19:22:46.190029 malla-0.1.5/malla/directed_edge.py
--rw-r--r--   0        0        0      717 2023-04-29 16:59:32.283620 malla-0.1.5/malla/off.py
--rw-r--r--   0        0        0      266 2023-05-03 19:44:58.236720 malla-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 malla-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      526 2023-04-29 16:35:40.386927 malla-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 21:01:58.416728 malla-0.1.6/malla/__init__.py
+-rw-r--r--   0        0        0     6064 2023-05-03 19:59:00.090070 malla-0.1.6/malla/directed_edge.py
+-rw-r--r--   0        0        0      717 2023-04-29 16:59:32.283620 malla-0.1.6/malla/off.py
+-rw-r--r--   0        0        0      266 2023-05-03 19:59:20.810070 malla-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 malla-0.1.6/PKG-INFO
```

### Comparing `malla-0.1.5/README.md` & `malla-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `malla-0.1.5/malla/directed_edge.py` & `malla-0.1.6/malla/directed_edge.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     def number_of_vertices(self) -> int:
         return len(self._vertices)
 
     def number_of_faces(self) -> int:
         return int(len(self.half_edges)/3)
 
     def vertex_neighbors(self, v: int) -> Generator[int, None, None]:
-        for he in self.vertex_halfedges():
+        for he in self.vertex_halfedges(v):
             yield self.half_edge(he).dst
             h = he
         if self.half_edge(self.prev(h)).mate == -1: #bordo
             yield self.half_edge(self.next(h)).dst
 
     def vertex_halfedges(self, v: int) -> Generator[int, None, None]:
         he = self.vertex(v).half_edge
@@ -133,15 +133,15 @@
             while True:
                 yield hn
                 hn = self.half_edge(self.prev(hn)).mate
                 if hn in {-1, he}:
                     break
 
     def vertex_faces(self, v: int) -> Generator[int, None, None]:
-        for he in self.vertex_halfedges():
+        for he in self.vertex_halfedges(v):
             yield self.face(he)
 
     def face_neighbors(self, f: int) -> Generator[int, None, None]:
         hf = 3*f
         for i in range(3):
             h = hf+i
             mate = self.half_edge(h).mate
```

### Comparing `malla-0.1.5/malla/off.py` & `malla-0.1.6/malla/off.py`

 * *Files identical despite different names*

### Comparing `malla-0.1.5/PKG-INFO` & `malla-0.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malla
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Dimas Martínez
 Author-email: dimas@ufam.edu.br
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

