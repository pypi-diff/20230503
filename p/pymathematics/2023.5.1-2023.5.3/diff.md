# Comparing `tmp/pymathematics-2023.5.1.tar.gz` & `tmp/pymathematics-2023.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymathematics-2023.5.1.tar", last modified: Mon May  1 18:00:28 2023, max compression
+gzip compressed data, was "pymathematics-2023.5.3.tar", last modified: Wed May  3 15:59:15 2023, max compression
```

## Comparing `pymathematics-2023.5.1.tar` & `pymathematics-2023.5.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-05-01 18:00:28.191467 pymathematics-2023.5.1/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.5.1/LICENSE
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      506 2023-05-01 18:00:28.155466 pymathematics-2023.5.1/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      165 2023-05-01 17:56:47.000000 pymathematics-2023.5.1/README.md
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-05-01 18:00:27.734466 pymathematics-2023.5.1/pymathematics/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    27686 2023-05-01 17:58:49.000000 pymathematics-2023.5.1/pymathematics/__init__.py
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      110 2023-05-01 17:54:20.000000 pymathematics-2023.5.1/pymathematics/info.py
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-05-01 18:00:28.084465 pymathematics-2023.5.1/pymathematics.egg-info/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      506 2023-05-01 18:00:24.000000 pymathematics-2023.5.1/pymathematics.egg-info/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      258 2023-05-01 18:00:24.000000 pymathematics-2023.5.1/pymathematics.egg-info/SOURCES.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-05-01 18:00:24.000000 pymathematics-2023.5.1/pymathematics.egg-info/dependency_links.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        6 2023-05-01 18:00:24.000000 pymathematics-2023.5.1/pymathematics.egg-info/requires.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-05-01 18:00:24.000000 pymathematics-2023.5.1/pymathematics.egg-info/top_level.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-05-01 18:00:28.195469 pymathematics-2023.5.1/setup.cfg
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      695 2023-05-01 17:56:39.000000 pymathematics-2023.5.1/setup.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-05-03 15:59:15.452536 pymathematics-2023.5.3/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.5.3/LICENSE
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      506 2023-05-03 15:59:15.442539 pymathematics-2023.5.3/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      165 2023-05-03 15:48:59.000000 pymathematics-2023.5.3/README.md
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-05-03 15:59:15.048536 pymathematics-2023.5.3/pymathematics/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    27656 2023-05-03 15:52:45.000000 pymathematics-2023.5.3/pymathematics/__init__.py
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      110 2023-05-03 15:48:24.000000 pymathematics-2023.5.3/pymathematics/info.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-05-03 15:59:15.369539 pymathematics-2023.5.3/pymathematics.egg-info/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      506 2023-05-03 15:59:12.000000 pymathematics-2023.5.3/pymathematics.egg-info/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      258 2023-05-03 15:59:12.000000 pymathematics-2023.5.3/pymathematics.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-05-03 15:59:12.000000 pymathematics-2023.5.3/pymathematics.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        6 2023-05-03 15:59:12.000000 pymathematics-2023.5.3/pymathematics.egg-info/requires.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-05-03 15:59:12.000000 pymathematics-2023.5.3/pymathematics.egg-info/top_level.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-05-03 15:59:15.456541 pymathematics-2023.5.3/setup.cfg
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      695 2023-05-03 15:48:53.000000 pymathematics-2023.5.3/setup.py
```

### Comparing `pymathematics-2023.5.1/LICENSE` & `pymathematics-2023.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymathematics-2023.5.1/pymathematics/__init__.py` & `pymathematics-2023.5.3/pymathematics/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,32 +77,32 @@
         row_lengths = [len(row) for row in matrix_]
         if not all(length == row_lengths[0] for length in row_lengths):
             return False
         return True
 
     def ifsquare(matrix_) -> bool:
         if not matrix.ismatrix(matrix_):
-            raise ValueError("elements of each rows aren't the same")
+            raise ValueError("input should be a matrix")
         if len(matrix_) == len(matrix_[0]):
             return True
         return False
     
     def shape(matrix_):
         if not matrix.ismatrix(matrix_):
-            raise ValueError("elements of each rows aren't the same")
+            raise ValueError("input should be a matrix")
         return len(matrix_),len(matrix_[0])
     
     def size(matrix_):
         if not matrix.ismatrix(matrix_):
-            raise ValueError("elements of each rows aren't the same")
+            raise ValueError("input should be a matrix")
         return len(matrix_)*len(matrix_[0])
 
     def determinant(matrix_):
         if not matrix.ismatrix(matrix_):
-            raise ValueError("elements of each rows aren't the same")
+            raise ValueError("input should be a matrix")
         if not matrix.ifsquare(matrix_):
             raise ValueError("determinant of a matrix is only defined for square matrices")
         if len(matrix_) == 1:
             return matrix_[0][0]
         elif len(matrix_) == 2:
             return matrix_[0][0]*matrix_[1][1]-matrix_[0][1]*matrix_[1][0]
         det = 0
@@ -115,15 +115,15 @@
                         row.append(matrix_[y][z])
                 minor.append(row)
             det += (-1)**x*matrix_[0][x]*matrix.determinant(minor)
         return det
     
     def inverse(matrix_):
         if not matrix.ismatrix(matrix_):
-            raise ValueError("elements of each rows aren't the same")
+            raise ValueError("input should be a matrix")
         if not matrix.ifsquare(matrix_):
             raise ValueError("inverse of a matrix is only defined for square matrices")
         identity = [[0 if x != y else 1 for y in range(len(matrix_))] for x in range(len(matrix_))]
         for x in range(len(matrix_)):
             pivot = matrix_[x][x]
             for y in range(len(matrix_)):
                 matrix_[x][y] /= pivot
@@ -132,52 +132,56 @@
                 if x != y:
                     factor = matrix_[y][x]
                     for k in range(len(matrix_)):
                         matrix_[y][k] -= factor * matrix_[x][k]
                         identity[y][k] -= factor * identity[x][k]
         return identity
     
-    def cofactor(matrix,row,col):
+    def cofactor(matrix_,row,col):
+        if not matrix.ismatrix(matrix_):
+            raise ValueError("input should be a matrix")
         return [row[:col] + row[col+1:] for row in (matrix[:row] + matrix[row+1:])]
 
     def adjoint(matrix_):
+        if not matrix.ismatrix(matrix_):
+            raise ValueError("input should be a matrix")
         adj = []
         for i in range(len(matrix_)):
             adjRow = []
             for j in range(len(matrix_)):
                 sign = (-1)**(i+j)
                 cofactor = matrix.determinant(matrix.cofactor(matrix_,i,j))
                 adjRow.append(sign*cofactor)
             adj.append(adjRow)
         return adj
     
     def trace(matrix_) -> int|float:
         if not matrix.ismatrix(matrix_):
-            raise ValueError("elements of each rows aren't the same")
+            raise ValueError("input should be a matrix")
         if not matrix.ifsquare(matrix_):
             raise ValueError("matrix should have same number of rows and cols")
         trace = 0
         for x in range(len(matrix_)):
             trace += matrix_[x][x]
         return trace
 
     def transpose(matrix_):
         if not matrix.ismatrix(matrix_):
-            raise ValueError("elements of each rows aren't the same")
+            raise ValueError("input should be a matrix")
         rows = len(matrix_)
         cols = len(matrix_[0])
         res = [[0 for y in range(rows)]for x in range(cols)]
         for x in range(rows):
             for y in range(cols):
                 res[y][x] = matrix_[x][y]   
         return res
     
     def product(matrix1,matrix2):
         if not matrix.ismatrix(matrix1) or not matrix.ismatrix(matrix2):
-            raise ValueError("elements of each rows aren't the same")
+            raise ValueError("input should be a matrix")
         rows1 = len(matrix1)
         cols1 = len(matrix1[0])
         rows2 = len(matrix2)
         cols2 = len(matrix2[0])
         if cols1 != rows2:
             raise ValueError("number of columns of a first matrix should be equal to the rows of the second matrix")
         result = [[0 for y in range(cols2)] for x in range(rows1)]
@@ -185,47 +189,42 @@
             for y in range(cols2):
                 dot_product = 0
                 for z in range(cols1):
                     dot_product += matrix1[x][z]*matrix2[z][y]
                 result[x][y] = dot_product
         return result
 
-    def multiply(matrix_,const,dimension:int = 1):
-        if 1 <= dimension <= 2:
-            if dimension == 1:
-                for x in range(len(matrix_)):
-                    matrix_[x] = matrix_[x]*const
-            elif dimension == 2:
-                for rows in matrix_:
-                    for x in range(len(rows)):
-                        rows[x] = rows[x]*const
-            else:
-                raise ValueError("capable for only 1 and 2 dimension")
+    def multiply(matrix_,const):
+        if not matrix.ismatrix(matrix_):
+            raise ValueError("input should be a matrix")
+        for rows in matrix_:
+            for x in range(len(rows)):
+                rows[x] = rows[x]*const
         return matrix_
 
-    def reciprocal(matrix_,dimension:int = 1):
-        if 1 <= dimension <= 2:
-            if dimension == 1:
-                for x in range(len(matrix_)):
-                    matrix_[x] = 1/matrix_[x]
-            elif dimension == 2:
-                for rows in matrix_:
-                    for x in range(len(rows)):
-                        rows[x] = 1/rows[x]
-            else:
-                raise ValueError("capable for only 1 and 2 dimension")
+    def reciprocal(matrix_):
+        if not matrix.ismatrix(matrix_):
+            raise ValueError("input should be a matrix")
+        for rows in matrix_:
+            for x in range(len(rows)):
+                rows[x] = 1/rows[x]
         return matrix_
 
     def remove_column(matrix_,column):
+        if not matrix.ismatrix(matrix_):
+            raise ValueError("input should be a matrix")
         for rows in matrix_:
             rows.remove(rows[column])
         return matrix_
     
-    def remove_row(matrix_,column):
-        return matrix_.remove(matrix_[column])
+    def remove_row(matrix_,row):
+        if not matrix.ismatrix(matrix_):
+            raise ValueError("input should be a matrix")
+        matrix_.remove(matrix_[row])
+        return matrix_
 
 class sets:
     def toset(A:list) -> list:
         new_set = []
         for x in A:
             if x not in new_set:
                 new_set.append(x)
@@ -417,24 +416,28 @@
 
 def absolute(number:int|float) -> int|float:
     if number < 0:
         return -1*number
     return number
 
 def floor(number:int|float) -> int:
+    if number == int(number):
+        return int(number)
     if number < 0:
         return int(number)-1
     return int(number)
 
 def ceil(number:int|float) -> int:
-    if number < 0:
+    if number == int(number):
         return int(number)
+    if number < 0:
+        return int(number)-1
     return int(number)+1
 
-def sqrt(number:int|float) -> float:
+def sqrt(number:int|float) -> int:
     if number < 0:
         return "undefined"
     elif number == 0:
         return 0
     flag = number/2
     while absolute(flag*flag - number) > 0.00001:
         flag = (flag + number/flag)/2
```

### Comparing `pymathematics-2023.5.1/setup.py` & `pymathematics-2023.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name = "pymathematics",
-    version = "2023.5.1",
+    version = "2023.5.3",
     description = "package for mathematics",
     long_description = "for more info, check the github repository",
     author = "Sahil Rajwar",
     maintainer = "its_Sahil",
     author_email = "justsahilrajwar2004@gmail.com",
     packages = ["pymathematics"],
     license = "MIT",
```

