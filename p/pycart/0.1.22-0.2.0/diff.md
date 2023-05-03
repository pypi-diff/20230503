# Comparing `tmp/pycart-0.1.22.tar.gz` & `tmp/pycart-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycart-0.1.22.tar", max compression
+gzip compressed data, was "pycart-0.2.0.tar", max compression
```

## Comparing `pycart-0.1.22.tar` & `pycart-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1546 2023-04-16 15:16:24.512787 pycart-0.1.22/LICENSE
--rw-r--r--   0        0        0        0 2023-04-09 13:06:33.395735 pycart-0.1.22/pycart/__init__.py
--rw-r--r--   0        0        0     3721 2023-04-16 17:12:51.613513 pycart-0.1.22/pycart/border_util.py
--rw-r--r--   0        0        0    18582 2023-04-18 15:50:53.394526 pycart-0.1.22/pycart/cartogram.py
--rw-r--r--   0        0        0     1716 2023-04-18 16:04:02.263976 pycart-0.1.22/pyproject.toml
--rw-r--r--   0        0        0     2649 2023-04-18 16:48:08.417830 pycart-0.1.22/README.md
--rw-r--r--   0        0        0    63368 2023-04-18 15:58:05.207779 pycart-0.1.22/requirements.txt
--rw-r--r--   0        0        0     4063 1970-01-01 00:00:00.000000 pycart-0.1.22/PKG-INFO
+-rw-r--r--   0        0        0     1546 2023-04-16 15:16:24.512787 pycart-0.2.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-09 13:06:33.395735 pycart-0.2.0/pycart/__init__.py
+-rw-r--r--   0        0        0     3721 2023-04-16 17:12:51.613513 pycart-0.2.0/pycart/border_util.py
+-rw-r--r--   0        0        0    19120 2023-04-23 16:13:55.604912 pycart-0.2.0/pycart/cartogram.py
+-rw-r--r--   0        0        0     1715 2023-05-03 10:53:23.317530 pycart-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2696 2023-04-23 11:38:01.763683 pycart-0.2.0/README.md
+-rw-r--r--   0        0        0    63368 2023-04-18 15:58:05.207779 pycart-0.2.0/requirements.txt
+-rw-r--r--   0        0        0     4107 1970-01-01 00:00:00.000000 pycart-0.2.0/PKG-INFO
```

### Comparing `pycart-0.1.22/LICENSE` & `pycart-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycart-0.1.22/pycart/border_util.py` & `pycart-0.2.0/pycart/border_util.py`

 * *Files identical despite different names*

### Comparing `pycart-0.1.22/pycart/cartogram.py` & `pycart-0.2.0/pycart/cartogram.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,19 +35,23 @@
 def _repel(neighbour, focal, xrepel, yrepel):
     """
     Calculates and updates the repulsive force being applied onto a given region, from a
     given neighbour of said region.
 
     The repulsive force $F$ is split into $x$ and $y$ components, $F_x$ and $F_y$
     respectively. These forces are calculated as the following, where $O$ is the
-    amount the neighbour overlaps with the focal region and $D_N$ is the distance
-    from the neighbour to the focal region:
+    amount the neighbour overlaps with the focal region, $D_N$ is the distance
+    from the neighbour to the focal region, $N_x$ is the $x$ position of the neighbour
+    and $M_x$ is the $x$ position of the focal region:
 
     $F_x = O \cdot (N_x - M_x) / D_N$
 
+    The $y$ force is calculated as the following, where $N_y$ and $M_y$ are the $y$
+    positions of the neighbour and focal regions, respectively:
+
     $F_y = O \cdot (N_y - M_y) / D_N$
 
     The supplied $x$ and $y$ forces are updated by subtracting the new forces.
 
     ###**Parameters**
 
     - **neighbour  :  *[pandas.Series](https://pandas.pydata.org/docs/reference/api/pandas.Series.html)*** - A given Neighbour of **focal**
@@ -77,25 +81,30 @@
     """
     Calculates and updates the attractive force being applied to a given region, towards a given
     neighbour region.
 
     Before the attractive forces are calculated, the overlap $O$ amount for a neighbour is scaled as
     such, where $W_{FN}$ is the Queen contiguity weight and $P_F$ is the perimeter of the focal region:
 
-    $O_{new} = (| O_{original} | * W_{NF}) / P_F$
+    $O_{new} = (| O_{original} | * W_{FN}) / P_F$
 
     The attractive force $A$ is split into $x$ and $y$ components, $A_x$ and $A_y$
     respectively. These forces are calculated as the following, where $O$ is the
-    amount the neighbour overlaps with the focal region:
+    amount the neighbour overlaps with the focal region, $D_N$ is the distance
+    from the neighbour to the focal region, $N_x$ is the $x$ position of the neighbour
+    and $M_x$ is the $x$ position of the focal region:
 
     $A_x = O_x \cdot (N_x - M_x) / D_N$
 
+    The $y$ force is calculated as the following, where $N_y$ and $M_y$ are the $y$
+    positions of the neighbour and focal regions, respectively:
+
     $A_y = O_y \cdot (N_y - M_y) / D_N$
 
-    The supplied $x$ and $y$ forces are updated by adding the new forces.
+    The supplied $x$ and $y$ forces are updated by summing with the new forces.
 
     ###**Parameters**
 
     - **nb  : *[pandas.Series](https://pandas.pydata.org/docs/reference/api/pandas.Series.html)*** - A given Neighbour of **focal**
     - **borders  :  *[pandas.DataFrame](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html)*** - DataFrame of all border weights
     - **idx  :  *int*** - The index of the current region
     - **focal  :  *[pandas.Series](https://pandas.pydata.org/docs/reference/api/pandas.Series.html)*** - The current, focal region
@@ -327,15 +336,15 @@
 
         # Calculate scaled radius by multiplying original radius by scale
         regions["radius"] = np.power(regions[self.value_field] / np.pi, 0.5) * scale
 
         # Get widest region
         widest = regions["radius"].max()
 
-        with alive_bar(iterations, title='Making Dorling Cartogram') as bar:
+        with alive_bar(iterations) as bar:
             for i in range(iterations):
                 # print(f"Starting Iteration: {i}")
                 bar()
 
                 if stop is not None:
                     if i == stop:
                         break
```

### Comparing `pycart-0.1.22/pyproject.toml` & `pycart-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycart"
-version = "0.1.22"
+version = "0.2.0"
 description = "A Python package for generating Cartograms using GeoDataFrames."
 authors = ["Alex Rundle <alexrundle01@gmail.com>"]
 readme = ["README.md"]
 license = "BSD-3-Clause"
 repository = "https://github.com/ARundle01/ecmm428-pycart"
 documentation = "https://ecmm428-pycart.readthedocs.io/"
```

### Comparing `pycart-0.1.22/README.md` & `pycart-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,22 +20,24 @@
 ## Installation
 ### Using Pip
 Make sure you have the latest version of PIP installed:
 ```pycon
 py -m pip install --upgrade pip
 ```
 
-This package is currently hosted on PyPi and TestPyPi, as it is currently in unstable development. To install 
+This package is currently hosted on PyPi and TestPyPi, as it is currently in unstable development. 
+
+To install the latest stable version
 and use this package from PyPi:
 ```pycon
 py -m pip install pycart
 ```
 
 To install
-and use this package from TestPyPi:
+and use the latest development version from TestPyPi:
 ```pycon
 py -m pip install -i https://test.pypi.org/simple/ pycart
 ```
 
 ## Pre-requisites
 All code in this Repository and Package was developed and tested on Windows 10.
 
@@ -48,15 +50,15 @@
 
 ### Key Dependencies
 To use `pycart`, you will need Python>=3.9, alongside the following 
 fixed version dependencies:
 
 | Package                                                    | Version      |
 |------------------------------------------------------------|--------------|
-| [Python](https://www.python.org/downloads/)                | >=3.9, <3.12 |
+| [Python](https://www.python.org/downloads/)                | >=3.9, <3.10 |
 | [matplotlib](https://pypi.org/project/matplotlib/)         | 3.7.1        |
 | [geopandas](https://pypi.org/project/geopandas/)           | 0.12.2       |
 | [geojson](https://pypi.org/project/geojson/)               | 3.0.1        |
 | [pandas](https://pypi.org/project/pandas/)                 | 1.5.3        |
 | [numpy](https://pypi.org/project/numpy/)                   | 1.24.2       |
 | [libpysal](https://pypi.org/project/libpysal/)             | 4.7.0        |
 | [shapely](https://pypi.org/project/shapely/)               | 2.0.1        |
```

### Comparing `pycart-0.1.22/requirements.txt` & `pycart-0.2.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `pycart-0.1.22/PKG-INFO` & `pycart-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycart
-Version: 0.1.22
+Version: 0.2.0
 Summary: A Python package for generating Cartograms using GeoDataFrames.
 Home-page: https://github.com/ARundle01/ecmm428-pycart
 License: BSD-3-Clause
 Author: Alex Rundle
 Author-email: alexrundle01@gmail.com
 Requires-Python: >=3.9.7,<3.10
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -58,22 +58,24 @@
 ## Installation
 ### Using Pip
 Make sure you have the latest version of PIP installed:
 ```pycon
 py -m pip install --upgrade pip
 ```
 
-This package is currently hosted on PyPi and TestPyPi, as it is currently in unstable development. To install 
+This package is currently hosted on PyPi and TestPyPi, as it is currently in unstable development. 
+
+To install the latest stable version
 and use this package from PyPi:
 ```pycon
 py -m pip install pycart
 ```
 
 To install
-and use this package from TestPyPi:
+and use the latest development version from TestPyPi:
 ```pycon
 py -m pip install -i https://test.pypi.org/simple/ pycart
 ```
 
 ## Pre-requisites
 All code in this Repository and Package was developed and tested on Windows 10.
 
@@ -86,15 +88,15 @@
 
 ### Key Dependencies
 To use `pycart`, you will need Python>=3.9, alongside the following 
 fixed version dependencies:
 
 | Package                                                    | Version      |
 |------------------------------------------------------------|--------------|
-| [Python](https://www.python.org/downloads/)                | >=3.9, <3.12 |
+| [Python](https://www.python.org/downloads/)                | >=3.9, <3.10 |
 | [matplotlib](https://pypi.org/project/matplotlib/)         | 3.7.1        |
 | [geopandas](https://pypi.org/project/geopandas/)           | 0.12.2       |
 | [geojson](https://pypi.org/project/geojson/)               | 3.0.1        |
 | [pandas](https://pypi.org/project/pandas/)                 | 1.5.3        |
 | [numpy](https://pypi.org/project/numpy/)                   | 1.24.2       |
 | [libpysal](https://pypi.org/project/libpysal/)             | 4.7.0        |
 | [shapely](https://pypi.org/project/shapely/)               | 2.0.1        |
```

