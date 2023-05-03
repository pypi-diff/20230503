# Comparing `tmp/q_random_number_generator-0.0.7.tar.gz` & `tmp/q_random_number_generator-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q_random_number_generator-0.0.7.tar", last modified: Tue May  2 15:41:51 2023, max compression
+gzip compressed data, was "q_random_number_generator-0.1.0.tar", last modified: Wed May  3 07:01:49 2023, max compression
```

## Comparing `q_random_number_generator-0.0.7.tar` & `q_random_number_generator-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 15:41:51.330381 q_random_number_generator-0.0.7/
--rw-rw-rw-   0        0        0     1065 2023-05-02 11:39:46.000000 q_random_number_generator-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      684 2023-05-02 15:41:51.327852 q_random_number_generator-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-05-02 15:41:05.000000 q_random_number_generator-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 15:41:51.305043 q_random_number_generator-0.0.7/q_random_number_generator/
--rw-rw-rw-   0        0        0     1454 2023-05-02 14:26:30.000000 q_random_number_generator-0.0.7/q_random_number_generator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 15:41:51.322851 q_random_number_generator-0.0.7/q_random_number_generator.egg-info/
--rw-rw-rw-   0        0        0      684 2023-05-02 15:41:50.000000 q_random_number_generator-0.0.7/q_random_number_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-05-02 15:41:51.000000 q_random_number_generator-0.0.7/q_random_number_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 15:41:50.000000 q_random_number_generator-0.0.7/q_random_number_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-02 15:41:50.000000 q_random_number_generator-0.0.7/q_random_number_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 15:41:51.330381 q_random_number_generator-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-05-02 15:41:44.000000 q_random_number_generator-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:01:49.229251 q_random_number_generator-0.1.0/
+-rw-rw-rw-   0        0        0     1065 2023-05-02 11:39:46.000000 q_random_number_generator-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      687 2023-05-03 07:01:49.227141 q_random_number_generator-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-05-03 07:01:25.000000 q_random_number_generator-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 07:01:49.203616 q_random_number_generator-0.1.0/q_random_number_generator/
+-rw-rw-rw-   0        0        0     1380 2023-05-03 06:52:49.000000 q_random_number_generator-0.1.0/q_random_number_generator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:01:49.221687 q_random_number_generator-0.1.0/q_random_number_generator.egg-info/
+-rw-rw-rw-   0        0        0      687 2023-05-03 07:01:48.000000 q_random_number_generator-0.1.0/q_random_number_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-05-03 07:01:49.000000 q_random_number_generator-0.1.0/q_random_number_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 07:01:48.000000 q_random_number_generator-0.1.0/q_random_number_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-03 07:01:48.000000 q_random_number_generator-0.1.0/q_random_number_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 07:01:49.229251 q_random_number_generator-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      668 2023-05-03 07:01:43.000000 q_random_number_generator-0.1.0/setup.py
```

### Comparing `q_random_number_generator-0.0.7/LICENSE` & `q_random_number_generator-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `q_random_number_generator-0.0.7/PKG-INFO` & `q_random_number_generator-0.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: q_random_number_generator
-Version: 0.0.7
-Summary: Using qiskit to realize random number generator
+Version: 0.1.0
+Summary: Using qiskit to realize random number generator.
 Home-page: https://github.com/allen91wu/q_random_number_generator
 Author: Allen Wu
 Author-email: allen91.wu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -16,11 +16,11 @@
 ## Description
 Using qiskit to realize quantum random number generator.
 
 ## Example
 ```python
 import q_randon_number_generator as qrng
 
-random_int = qrng.randint(-50, 50, 10)
+random_int = qrng.randint(-10, 10, 1000)
 ```
 ## Author
 - Allen Wu
```

### Comparing `q_random_number_generator-0.0.7/q_random_number_generator/__init__.py` & `q_random_number_generator-0.1.0/q_random_number_generator/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     QC = QuantumCircuit(qr, cr)
     QC.h(range(q_counts))
     QC.measure(qr, cr)
     return QC
 
 
-def generate(start, end, total):
+def randint(start, end, total):
     maximum = max(abs(start), abs(end))
     collected = 0
     qbits = 0
 
     # decision qubits counts
     isInt = int(math.log2(maximum)) == math.log2(maximum)
     if isInt is True:
@@ -43,10 +43,7 @@
                 pn = -1
             absolute = int(i[1:], 2)
             random_number = int(pn * absolute)
             if start <= random_number <= end:
                 collected += 1
                 random_list.append(random_number)
     return random_list
-
-def randint(start, end, total):
-    return generate(start, end, total)
```

### Comparing `q_random_number_generator-0.0.7/q_random_number_generator.egg-info/PKG-INFO` & `q_random_number_generator-0.1.0/q_random_number_generator.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: q-random-number-generator
-Version: 0.0.7
-Summary: Using qiskit to realize random number generator
+Version: 0.1.0
+Summary: Using qiskit to realize random number generator.
 Home-page: https://github.com/allen91wu/q_random_number_generator
 Author: Allen Wu
 Author-email: allen91.wu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -16,11 +16,11 @@
 ## Description
 Using qiskit to realize quantum random number generator.
 
 ## Example
 ```python
 import q_randon_number_generator as qrng
 
-random_int = qrng.randint(-50, 50, 10)
+random_int = qrng.randint(-10, 10, 1000)
 ```
 ## Author
 - Allen Wu
```

### Comparing `q_random_number_generator-0.0.7/setup.py` & `q_random_number_generator-0.1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="q_random_number_generator",
-    version="0.0.7",
+    version="0.1.0",
     author="Allen Wu",
     author_email="allen91.wu@gmail.com",
-    description="Using qiskit to realize random number generator",
+    description="Using qiskit to realize random number generator.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/allen91wu/q_random_number_generator",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

