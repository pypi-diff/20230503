# Comparing `tmp/malla-0.1.4.tar.gz` & `tmp/malla-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malla-0.1.4.tar", max compression
+gzip compressed data, was "malla-0.1.5.tar", max compression
```

## Comparing `malla-0.1.4.tar` & `malla-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      526 2023-04-29 16:35:40.386927 malla-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-04-25 21:01:58.416728 malla-0.1.4/malla/__init__.py
--rw-r--r--   0        0        0     6398 2023-04-29 17:02:44.313624 malla-0.1.4/malla/directed_edge.py
--rw-r--r--   0        0        0      717 2023-04-29 16:59:32.283620 malla-0.1.4/malla/off.py
--rw-r--r--   0        0        0      266 2023-04-29 17:05:27.680293 malla-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 malla-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      526 2023-04-29 16:35:40.386927 malla-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 21:01:58.416728 malla-0.1.5/malla/__init__.py
+-rw-r--r--   0        0        0     6062 2023-05-03 19:22:46.190029 malla-0.1.5/malla/directed_edge.py
+-rw-r--r--   0        0        0      717 2023-04-29 16:59:32.283620 malla-0.1.5/malla/off.py
+-rw-r--r--   0        0        0      266 2023-05-03 19:44:58.236720 malla-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 malla-0.1.5/PKG-INFO
```

### Comparing `malla-0.1.4/README.md` & `malla-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `malla-0.1.4/malla/directed_edge.py` & `malla-0.1.5/malla/directed_edge.py`

 * *Files 5% similar despite different names*

```diff
@@ -116,46 +116,33 @@
     def number_of_vertices(self) -> int:
         return len(self._vertices)
 
     def number_of_faces(self) -> int:
         return int(len(self.half_edges)/3)
 
     def vertex_neighbors(self, v: int) -> Generator[int, None, None]:
+        for he in self.vertex_halfedges():
+            yield self.half_edge(he).dst
+            h = he
+        if self.half_edge(self.prev(h)).mate == -1: #bordo
+            yield self.half_edge(self.next(h)).dst
+
+    def vertex_halfedges(self, v: int) -> Generator[int, None, None]:
         he = self.vertex(v).half_edge
         if he != -1:
-            v0 = self.half_edge(he).dst
-            yield v0
+            hn = he
             while True:
-                hn = self.half_edge(self.prev(he)).mate
-                if hn == -1:
-                    yield self.half_edge(self.next(he)).dst
-                    break
-                else:
-                    he = hn
-                vi = self.half_edge(he).dst
-                if vi == v0:
+                yield hn
+                hn = self.half_edge(self.prev(hn)).mate
+                if hn in {-1, he}:
                     break
-                else:
-                    yield vi
 
-    def vertex_neighboring_faces(self, v: int) -> Generator[int, None, None]:
-        hf = self.vertex(v).half_edge
-        if hf != -1:
-            he = hf
+    def vertex_faces(self, v: int) -> Generator[int, None, None]:
+        for he in self.vertex_halfedges():
             yield self.face(he)
-            while True:
-                hn = self.half_edge(self.prev(he)).mate
-                if hn == -1:
-                    break
-                else:
-                    he = hn
-                if he == hf:
-                    break
-                else:
-                    yield self.face(he)
 
     def face_neighbors(self, f: int) -> Generator[int, None, None]:
         hf = 3*f
         for i in range(3):
             h = hf+i
             mate = self.half_edge(h).mate
             if mate > -1:
```

### Comparing `malla-0.1.4/malla/off.py` & `malla-0.1.5/malla/off.py`

 * *Files identical despite different names*

### Comparing `malla-0.1.4/PKG-INFO` & `malla-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malla
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Dimas Martínez
 Author-email: dimas@ufam.edu.br
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

