# Comparing `tmp/leechem-1.1.tar.gz` & `tmp/leechem-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leechem-1.1.tar", last modified: Mon May  1 20:35:37 2023, max compression
+gzip compressed data, was "leechem-1.2.tar", last modified: Wed May  3 18:50:14 2023, max compression
```

## Comparing `leechem-1.1.tar` & `leechem-1.2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-05-01 20:35:37.703836 leechem-1.1/
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    26526 2023-04-14 15:24:21.000000 leechem-1.1/LICENSE
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      237 2023-05-01 20:35:37.699836 leechem-1.1/PKG-INFO
--rwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)     4012 2023-04-14 15:24:21.000000 leechem-1.1/README.md
-drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-05-01 20:35:37.699836 leechem-1.1/leechem/
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      133 2023-05-01 20:35:13.000000 leechem-1.1/leechem/__init__.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1851 2023-04-14 15:24:21.000000 leechem-1.1/leechem/certainties.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     6389 2023-04-14 15:24:21.000000 leechem-1.1/leechem/cleandb.py
--rwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)     7604 2023-04-14 15:24:21.000000 leechem-1.1/leechem/compare_trees.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     4484 2023-04-14 15:24:21.000000 leechem-1.1/leechem/confidence.py
--rwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)      274 2023-04-14 15:24:21.000000 leechem-1.1/leechem/conftid.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      254 2023-04-14 15:24:21.000000 leechem-1.1/leechem/countrows.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1698 2023-04-14 15:24:21.000000 leechem-1.1/leechem/dependentsynapses.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      148 2023-04-14 15:24:21.000000 leechem-1.1/leechem/distance.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     5706 2023-04-14 15:24:21.000000 leechem-1.1/leechem/findpath.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     4970 2023-04-14 15:24:21.000000 leechem-1.1/leechem/geometry.py
--rwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)      290 2023-04-14 15:24:21.000000 leechem-1.1/leechem/get_tree_ids.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1304 2023-04-14 15:24:21.000000 leechem-1.1/leechem/grabvsddata.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     5983 2023-04-14 15:24:21.000000 leechem-1.1/leechem/mapping.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     5062 2023-04-14 15:24:21.000000 leechem-1.1/leechem/nn_clustering.py
--rwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)      484 2023-04-14 15:24:21.000000 leechem-1.1/leechem/node_distance.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     6449 2023-04-14 15:24:21.000000 leechem-1.1/leechem/rawaccess.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     9909 2023-04-14 15:24:21.000000 leechem-1.1/leechem/runinfo.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    10502 2023-04-14 15:24:21.000000 leechem-1.1/leechem/salpa.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    17605 2023-04-14 15:24:21.000000 leechem-1.1/leechem/sbemdb.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     7199 2023-05-01 17:52:17.000000 leechem-1.1/leechem/sbemimage.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    14866 2023-04-14 15:24:21.000000 leechem-1.1/leechem/tree.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    11685 2023-05-01 20:29:51.000000 leechem-1.1/leechem/trials.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     2240 2023-04-14 15:24:21.000000 leechem-1.1/leechem/uCT.py
-drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-05-01 20:35:37.699836 leechem-1.1/leechem.egg-info/
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      237 2023-05-01 20:35:37.000000 leechem-1.1/leechem.egg-info/PKG-INFO
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      679 2023-05-01 20:35:37.000000 leechem-1.1/leechem.egg-info/SOURCES.txt
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        1 2023-05-01 20:35:37.000000 leechem-1.1/leechem.egg-info/dependency_links.txt
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        6 2023-05-01 20:35:37.000000 leechem-1.1/leechem.egg-info/requires.txt
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        8 2023-05-01 20:35:37.000000 leechem-1.1/leechem.egg-info/top_level.txt
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)       38 2023-05-01 20:35:37.703836 leechem-1.1/setup.cfg
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      339 2023-05-01 20:33:19.000000 leechem-1.1/setup.py
+drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-05-03 18:50:14.474169 leechem-1.2/
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    26526 2023-04-14 15:24:21.000000 leechem-1.2/LICENSE
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      237 2023-05-03 18:50:14.474169 leechem-1.2/PKG-INFO
+-rwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)     4012 2023-04-14 15:24:21.000000 leechem-1.2/README.md
+drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-05-03 18:50:14.474169 leechem-1.2/leechem/
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      133 2023-05-03 18:50:03.000000 leechem-1.2/leechem/__init__.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1851 2023-04-14 15:24:21.000000 leechem-1.2/leechem/certainties.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     6389 2023-04-14 15:24:21.000000 leechem-1.2/leechem/cleandb.py
+-rwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)     7604 2023-04-14 15:24:21.000000 leechem-1.2/leechem/compare_trees.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     4420 2023-05-03 18:39:38.000000 leechem-1.2/leechem/confidence.py
+-rwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)      274 2023-04-14 15:24:21.000000 leechem-1.2/leechem/conftid.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      254 2023-04-14 15:24:21.000000 leechem-1.2/leechem/countrows.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1698 2023-04-14 15:24:21.000000 leechem-1.2/leechem/dependentsynapses.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      148 2023-04-14 15:24:21.000000 leechem-1.2/leechem/distance.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     5706 2023-04-14 15:24:21.000000 leechem-1.2/leechem/findpath.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     4970 2023-04-14 15:24:21.000000 leechem-1.2/leechem/geometry.py
+-rwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)      290 2023-04-14 15:24:21.000000 leechem-1.2/leechem/get_tree_ids.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1304 2023-04-14 15:24:21.000000 leechem-1.2/leechem/grabvsddata.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     5911 2023-05-03 18:40:21.000000 leechem-1.2/leechem/mapping.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     5062 2023-04-14 15:24:21.000000 leechem-1.2/leechem/nn_clustering.py
+-rwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)      484 2023-04-14 15:24:21.000000 leechem-1.2/leechem/node_distance.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     6449 2023-04-14 15:24:21.000000 leechem-1.2/leechem/rawaccess.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     9871 2023-05-03 18:43:25.000000 leechem-1.2/leechem/runinfo.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    10502 2023-04-14 15:24:21.000000 leechem-1.2/leechem/salpa.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    17411 2023-05-03 18:45:06.000000 leechem-1.2/leechem/sbemdb.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     7199 2023-05-01 17:52:17.000000 leechem-1.2/leechem/sbemimage.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    14866 2023-04-14 15:24:21.000000 leechem-1.2/leechem/tree.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    11685 2023-05-01 20:29:51.000000 leechem-1.2/leechem/trials.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     2152 2023-05-03 18:43:12.000000 leechem-1.2/leechem/uCT.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1182 2023-05-03 18:46:31.000000 leechem-1.2/leechem/webaccess.py
+drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-05-03 18:50:14.474169 leechem-1.2/leechem.egg-info/
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      237 2023-05-03 18:50:14.000000 leechem-1.2/leechem.egg-info/PKG-INFO
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      700 2023-05-03 18:50:14.000000 leechem-1.2/leechem.egg-info/SOURCES.txt
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        1 2023-05-03 18:50:14.000000 leechem-1.2/leechem.egg-info/dependency_links.txt
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        6 2023-05-03 18:50:14.000000 leechem-1.2/leechem.egg-info/requires.txt
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        8 2023-05-03 18:50:14.000000 leechem-1.2/leechem.egg-info/top_level.txt
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)       38 2023-05-03 18:50:14.474169 leechem-1.2/setup.cfg
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      339 2023-05-01 20:33:19.000000 leechem-1.2/setup.py
```

### Comparing `leechem-1.1/LICENSE` & `leechem-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `leechem-1.1/README.md` & `leechem-1.2/README.md`

 * *Files identical despite different names*

### Comparing `leechem-1.1/leechem/certainties.py` & `leechem-1.2/leechem/certainties.py`

 * *Files identical despite different names*

### Comparing `leechem-1.1/leechem/cleandb.py` & `leechem-1.2/leechem/cleandb.py`

 * *Files identical despite different names*

### Comparing `leechem-1.1/leechem/compare_trees.py` & `leechem-1.2/leechem/compare_trees.py`

 * *Files identical despite different names*

### Comparing `leechem-1.1/leechem/confidence.py` & `leechem-1.2/leechem/confidence.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/python3
 
 import numpy as np
 import csv
 import errno
 import os
 import re
+from . import webaccess
 
 class Confidence:
     def __init__(self, csvfn=None):
         '''CONFIDENCE - Python access to the SBEM-uCT-VSD confidence file
         conf = CONFIDENCE(csvfn) opens the given confidence file.
         conf = CONFIDENCE() uses the default file in the em170428 directory.
         Result has several fields that each are dicts with tree IDs as keys:
@@ -22,19 +23,16 @@
         self.vsdid = {}
         self.canoid = {}
         self.sbemconf = {}
         self.vsductconf = {}
         self.gmapconf = {}
         self.vsd2tree = {}
 
-        if csvfn is None:
-            here = os.path.dirname(__file__)
-            csvfn = here + '/../data/confidence.csv'
         lines = []
-        with open(csvfn) as f:
+        with webaccess.opentextfile(csvfn, "confidence.csv") as f:
             dl = csv.unix_dialect()
             rdr = csv.reader(f, dl)
             for row in rdr:
                 lines.append(row)
         hdr = lines.pop(0)
         r = re.compile('^(\d+)\s*(\((\d+)(-([a-z]+))?\))?$')
         for l in lines:
```

### Comparing `leechem-1.1/leechem/dependentsynapses.py` & `leechem-1.2/leechem/dependentsynapses.py`

 * *Files identical despite different names*

### Comparing `leechem-1.1/leechem/findpath.py` & `leechem-1.2/leechem/findpath.py`

 * *Files identical despite different names*

### Comparing `leechem-1.1/leechem/geometry.py` & `leechem-1.2/leechem/geometry.py`

 * *Files identical despite different names*

### Comparing `leechem-1.1/leechem/grabvsddata.py` & `leechem-1.2/leechem/grabvsddata.py`

 * *Files identical despite different names*

### Comparing `leechem-1.1/leechem/mapping.py` & `leechem-1.2/leechem/mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/python3
 
 import numpy as np
 import csv
 import errno
 import os
+from . import webaccess
 
 class Mapping:
     def __init__(self, csvfn=None):
         '''MAPPING - Python access to the SBEM-uCT-VSD mapping
         map = MAPPING(csvfn) opens the given mapping file.
         map = MAPPING() uses the default file in the em170428 directory.
         Result has fields roi2can, roi2uct, roi2sbem that map ROI numbers
@@ -27,20 +28,17 @@
         self.uct2roi = {}
         self.uct2sbem = {}
         self.can2sbem = {}
         self.can2roi = {}
         self.can2uct = {}
         self.roiid2roi = {}
         self.roi2roiid = {}
-        
-        if csvfn is None:
-            here = os.path.dirname(__file__)
-            csvfn = here + '/../data/mapping.csv'
+
         lines = []
-        with open(csvfn) as f:
+        with webaccess.opentextfile(csvfn, "mapping.csv") as f:
             dl = csv.unix_dialect()
             rdr = csv.reader(f, dl)
             for row in rdr:
                 lines.append(row)
         hdr = lines.pop(0)
         for l in lines:
             roi = self.convert_to_number(l[0])
```

### Comparing `leechem-1.1/leechem/nn_clustering.py` & `leechem-1.2/leechem/nn_clustering.py`

 * *Files identical despite different names*

### Comparing `leechem-1.1/leechem/rawaccess.py` & `leechem-1.2/leechem/rawaccess.py`

 * *Files identical despite different names*

### Comparing `leechem-1.1/leechem/runinfo.py` & `leechem-1.2/leechem/runinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/python3
 
 import numpy as np
 import h5py as h5
 import math
 import sys
 import os.path
+from . import webaccess
 
 TILESIZE = 512
 IMAGESIZE = TILESIZE * 33
 IMAGERAD = IMAGESIZE / 2
 RAWSIZE = 17100
 MARGIN = (RAWSIZE - IMAGESIZE)//2
 
@@ -47,17 +48,15 @@
     
     def __init__(self, ifn=None):
         '''RUNINFO - Class to wrap back position data for the 170428 run
         pp = RUNINFO(ifn) creates a new instance of the RUNINFO
         class, loading the data from the given hdf5 file.
         pp = RUNINFO() loads the data from the 'positionsummary.h5' 
         file in the em170428 directory.'''
-        if ifn is None:
-            here = os.path.dirname(__file__)
-            ifn = here + '/../data/positionsummary.h5'
+        ifn = webaccess.ensurefile(ifn, "positionsummary.h5")
         self.f = h5.File(ifn, 'r')
 
     BLEND = 1024
     
     def blender(self, x):
         print('blend', x, self.BLEND)
         if x<=0:
```

### Comparing `leechem-1.1/leechem/salpa.py` & `leechem-1.2/leechem/salpa.py`

 * *Files identical despite different names*

### Comparing `leechem-1.1/leechem/sbemdb.py` & `leechem-1.2/leechem/sbemdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/python3
 
 import numpy as np
 import sqlite3
 import errno
 import os
+from . import webaccess
 
 class LineSegmentGeom:
     def _dif(pa, pb):
         return [pa[k] - pb[k] for k in range(3)]
     def _inner(a, b):
         return sum([a[k]*b[k] for k in range(3)])
     def _addmul(p, dp, t):
@@ -58,20 +59,15 @@
         self.uid = uid
 
 class SBEMDB:
     def __init__(self, dbfn=None):
         '''SBEMDB - Pythonic access to SBEMDB
         db = SBEMDB(dbfn) opens the given database file. db = SBEMDB() opens
         the database file in the em170428 directory.'''
-        if dbfn is None:
-            here = os.path.dirname(__file__)
-            dbfn = here + '/../data/170428_pub.sbemdb'
-        if not os.path.isfile(dbfn):
-            raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT),
-                                    dbfn)
+        dbfn = webaccess.ensurefile(dbfn, "170428_pub.sbemdb")
         self.db = sqlite3.connect(dbfn)
         self.dbfn = dbfn
 
     def fetch(self, query):
         c = self.db.cursor()
         c.execute(query)
         return c.fetchall()
```

### Comparing `leechem-1.1/leechem/sbemimage.py` & `leechem-1.2/leechem/sbemimage.py`

 * *Files identical despite different names*

### Comparing `leechem-1.1/leechem/tree.py` & `leechem-1.2/leechem/tree.py`

 * *Files identical despite different names*

### Comparing `leechem-1.1/leechem/trials.py` & `leechem-1.2/leechem/trials.py`

 * *Files identical despite different names*

### Comparing `leechem-1.1/leechem/uCT.py` & `leechem-1.2/leechem/uCT.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,45 +7,46 @@
 
 class UCT:
     def __init__(self, h5fn=None):
         '''UCT - Python access to the uCT soma position file
         uct = UCT(h5fn) opens the given "uCT-somata.h5" file.
         uct = UCT() opens the default file in the em170428 directory.
         '''
-        if h5fn is None:
-            here = os.path.dirname(__file__)
-            h5fn = here + '/../data/uCT-somata.h5'
-            with h5py.File(h5fn, 'r') as h5:
-                self.somapos = h5['somapos']['value'][:] * 2
-                self.exitpoint = h5['dpp']['value'][:]
-                self.lut = h5['dc']['value'][:]
-                self.tails = {}
-                tt = h5['tails']['value']
-                for k in tt.keys():
-                    if k.startswith('_'):
-                        k1= int(k[1:])
-                        t = tt[k]
-                        t = t['value']
-                        if len(t)==3:
-                            self.tails[k1] = t[:]
-                        else:
-                            self.tails[k] = [[],[],[]] 
+        h5fn = webaccess.ensurefile(h5fn, "uCT-somata.h5")
+        with h5py.File(h5fn, 'r') as h5:
+            self.somapos = h5['somapos']['value'][:] * 2
+            self.exitpoint = h5['dpp']['value'][:]
+            self.lut = h5['dc']['value'][:]
+            self.tails = {}
+            tt = h5['tails']['value']
+            for k in tt.keys():
+                if k.startswith('_'):
+                    k1= int(k[1:])
+                    t = tt[k]
+                    t = t['value']
+                    if len(t)==3:
+                        self.tails[k1] = t[:]
+                    else:
+                        self.tails[k] = [[],[],[]]
+                        
     def somaPosition(self, uctid):
         '''SOMAPOSITION - Position of a soma
         x,y,z = SOMAPOSITION(uctid) returns the position of a soma.
         UCTID must be a UCT ID (for instance, DE3_R is 1; DI1_R is 66).
         X, Y, Z are in UCT pixel coordinates.'''
         return self.somapos[:,uctid-1]
+    
     def exitPointPosition(self, uctid):
         '''EXITPOINTPOSITION - Position of a exit point
         x,y,z = EXITPOINTPOSITION(uctid) returns the position of the point
         where the principal neurite of a cell exits the neuropil.
         UCTID must be a UCT ID (for instance, DE3_R is 1; DI1_R is 66).
         X, Y, Z are in UCT pixel coordinates.'''
         return self.exitpoint[:,uctid-1]
+    
     def tailPosition(self, uctid):
         '''TAILPOSITION - Position of a tail
         x,y,z = TAILPOSITION(uctid) returns the position of the “tail”
         of a cell, i.e., the approximate path of the principal neurite
         between the soma and the “exit point.”
         UCTID must be a UCT ID (for instance, DE3_R is 1; DI1_R is 66).
         X, Y, Z are vectors of UCT pixel coordinates.'''
```

### Comparing `leechem-1.1/leechem.egg-info/SOURCES.txt` & `leechem-1.2/leechem.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,12 +21,13 @@
 leechem/runinfo.py
 leechem/salpa.py
 leechem/sbemdb.py
 leechem/sbemimage.py
 leechem/tree.py
 leechem/trials.py
 leechem/uCT.py
+leechem/webaccess.py
 leechem.egg-info/PKG-INFO
 leechem.egg-info/SOURCES.txt
 leechem.egg-info/dependency_links.txt
 leechem.egg-info/requires.txt
 leechem.egg-info/top_level.txt
```

