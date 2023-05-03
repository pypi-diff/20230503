# Comparing `tmp/unravel-python-1.2.5.tar.gz` & `tmp/unravel-python-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unravel-python-1.2.5.tar", last modified: Fri Apr 28 13:52:37 2023, max compression
+gzip compressed data, was "unravel-python-1.2.6.tar", last modified: Wed May  3 18:29:28 2023, max compression
```

## Comparing `unravel-python-1.2.5.tar` & `unravel-python-1.2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 13:52:37.690000 unravel-python-1.2.5/
--rw-rw-rw-   0        0        0    35823 2023-03-09 15:58:46.000000 unravel-python-1.2.5/LICENSE
--rw-rw-rw-   0        0        0     3950 2023-04-28 13:52:38.000000 unravel-python-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     3442 2023-04-28 07:26:38.000000 unravel-python-1.2.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-28 13:52:38.000000 unravel-python-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1146 2023-04-28 13:02:26.000000 unravel-python-1.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 13:52:37.700000 unravel-python-1.2.5/unravel/
--rw-rw-rw-   0        0        0      358 2023-04-28 13:52:14.000000 unravel-python-1.2.5/unravel/__init__.py
--rw-rw-rw-   0        0        0    48931 2023-04-28 13:51:32.000000 unravel-python-1.2.5/unravel/core.py
--rw-rw-rw-   0        0        0     4558 2023-04-05 16:37:44.000000 unravel-python-1.2.5/unravel/example.py
--rw-rw-rw-   0        0        0    14624 2023-04-24 14:10:10.000000 unravel-python-1.2.5/unravel/utils.py
--rw-rw-rw-   0        0        0     3746 2023-04-20 07:59:10.000000 unravel-python-1.2.5/unravel/viz.py
-drwxrwxrwx   0        0        0        0 2023-04-28 13:52:37.710000 unravel-python-1.2.5/unravel_python.egg-info/
--rw-rw-rw-   0        0        0     3950 2023-04-28 13:52:38.000000 unravel-python-1.2.5/unravel_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-04-28 13:52:38.000000 unravel-python-1.2.5/unravel_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 13:52:38.000000 unravel-python-1.2.5/unravel_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-28 13:52:38.000000 unravel-python-1.2.5/unravel_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-28 13:52:38.000000 unravel-python-1.2.5/unravel_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 18:29:27.990000 unravel-python-1.2.6/
+-rw-rw-rw-   0        0        0    35823 2023-03-09 15:58:46.000000 unravel-python-1.2.6/LICENSE
+-rw-rw-rw-   0        0        0     3950 2023-05-03 18:29:30.000000 unravel-python-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3442 2023-04-28 07:26:38.000000 unravel-python-1.2.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-03 18:29:30.000000 unravel-python-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1146 2023-04-28 13:02:26.000000 unravel-python-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:29:28.000000 unravel-python-1.2.6/unravel/
+-rw-rw-rw-   0        0        0      358 2023-05-03 18:28:52.000000 unravel-python-1.2.6/unravel/__init__.py
+-rw-rw-rw-   0        0        0    49987 2023-05-03 18:25:56.000000 unravel-python-1.2.6/unravel/core.py
+-rw-rw-rw-   0        0        0     4558 2023-05-03 18:24:34.000000 unravel-python-1.2.6/unravel/example.py
+-rw-rw-rw-   0        0        0    14624 2023-04-24 14:10:10.000000 unravel-python-1.2.6/unravel/utils.py
+-rw-rw-rw-   0        0        0     3746 2023-04-20 07:59:10.000000 unravel-python-1.2.6/unravel/viz.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:29:28.000000 unravel-python-1.2.6/unravel_python.egg-info/
+-rw-rw-rw-   0        0        0     3950 2023-05-03 18:29:28.000000 unravel-python-1.2.6/unravel_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-05-03 18:29:28.000000 unravel-python-1.2.6/unravel_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 18:29:28.000000 unravel-python-1.2.6/unravel_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-03 18:29:28.000000 unravel-python-1.2.6/unravel_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-03 18:29:28.000000 unravel-python-1.2.6/unravel_python.egg-info/top_level.txt
```

### Comparing `unravel-python-1.2.5/LICENSE` & `unravel-python-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.5/PKG-INFO` & `unravel-python-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unravel-python
-Version: 1.2.5
+Version: 1.2.6
 Summary: Implementation of UNRAVEL
 Home-page: https://github.com/DelinteNicolas/UNRAVEL
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `unravel-python-1.2.5/README.md` & `unravel-python-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.5/setup.py` & `unravel-python-1.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.5/unravel/core.py` & `unravel-python-1.2.6/unravel/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,14 +289,47 @@
 
     if ang > 90 and not direction:
         ang = 180-ang
 
     return ang
 
 
+def relative_angular_weighting(vs, vList: list, nList: list):
+
+    K = len(vList)
+
+    if K == 1:
+        return [1]
+
+    if K-sum(nList) <= 1:
+        return [1-i for i in list(map(int, nList))]
+
+    angle_diffList = []
+
+    for i, v in enumerate(vList):
+        if nList[i]:
+            angle_diffList.append(0)
+        else:
+            angle_diffList.append(angle_difference(vs, v))
+
+    sum_diff = np.sum(angle_diffList)
+
+    ang_coef = []
+
+    for i, angle_diff in enumerate(angle_diffList):
+        if nList[i]:
+            ang_coef.append(0)
+        else:
+            coef = (min(90, sum_diff)-angle_diff)/(min(90, sum_diff)
+                                                   * (K-sum(nList))-sum_diff)
+            ang_coef.append(coef)
+
+    return ang_coef
+
+
 def angular_weighting(vs, vList: list, nList: list):
     '''
     Computes the relative contributions of the segments in vList to vs using
     angular weighting.
 
     Parameters
     ----------
@@ -620,15 +653,15 @@
             # !!!
             img = nib.load(MF_dir+Patient+'_mf_frac_f'+str(k)+'.nii.gz')
             f = img.get_fdata()
 
             fList.append(f)
 
     return get_fixel_weight(trk, tList, method, streamList, fList,
-                           speed_up=speed_up)
+                            speed_up=speed_up)
 
 
 def get_fixel_weight_DIAMOND(trk_file: str, DIAMOND_dir: str, Patient: str,
                              K: int = 2, method: str = 'ang',
                              streamList: list = [], speed_up: bool = False):
     '''
     Get the fixel weights from a tract specified in trk_file and the tensors
@@ -702,15 +735,15 @@
         for k in range(K):
 
             fk = f[:, :, :, 0, k]
 
             fList.append(fk)
 
     return get_fixel_weight(trk, tList, method, streamList, fList,
-                           speed_up=speed_up)
+                            speed_up=speed_up)
 
 
 def get_fixel_weight(trk, tList: list, method: str = 'ang',
                      streamList: list = [], fList: list = [],
                      return_phi: bool = False, speed_up: bool = False):
     '''
     Get the fixel weights from a tract specified in trk_file.
@@ -755,15 +788,15 @@
         streamlines specified in streamList.
     outputSegmentStream :list, optional
         List of the relative contribution of each voxel for the streamlines
         specified in streamList.
 
     '''
 
-    assert method in ['ang', 'cfo', 'vol'], ("Unknown method : "+method)
+    assert method in ['ang', 'cfo', 'vol', 'raw'], ("Unknown method : "+method)
 
     phi_maps = {}
     K = len(tList)
     # t10=np.zeros(tList[0].shape)
     fixelWeights = np.zeros(tList[0].shape[0:3]+(K,), dtype='float32')
 
     sList = tract_to_streamlines(trk)
@@ -820,14 +853,16 @@
                         warnings.warn("Warning : The number of fixels ("
                                       + str(K)
                                       + ") does not correspond to the number "
                                       + " of fractions given ("+str(len(fList))
                                       + ").")
                     coefList = fraction_weighting(
                         (x, y, z), vList, nList, fList)
+                elif method == 'raw':
+                    coefList = relative_angular_weighting(vs, vList, nList)
                 else:   # Angular weighting
                     coefList = angular_weighting(vs, vList, nList)
 
                 for k, coef in enumerate(coefList):
                     fixelWeights[x, y, z, k] += voxList[(x, y, z)]*coef
 
                 if return_phi:
@@ -932,15 +967,15 @@
 
         sList.append(b[offset:offset+streams._lengths[i], :])
 
     return sList
 
 
 def get_streamline_weights(trk, tList: list,
-                           method_list: list = ['vol', 'cfo', 'ang'],
+                           method_list: list = ['vol', 'cfo', 'ang', 'raw'],
                            streamline_number: int = 0, fList: list = []):
     '''
 
 
     Parameters
     ----------
     trk : tractogram
@@ -1022,14 +1057,16 @@
                         warnings.warn("Warning : The number of fixels ("
                                       + str(len(vList))
                                       + ") does not correspond to the number "
                                       + " of fractions given ("+str(len(fList))
                                       + ").")
                     coefList = fraction_weighting(
                         (x, y, z), vList, nList, fList)
+                elif method == 'raw':
+                    coefList = relative_angular_weighting(vs, vList, nList)
                 else:   # Angular weighting
                     coefList = angular_weighting(vs, vList, nList)
 
                 s = []
                 for coef in coefList:
                     s.append(voxList[(x, y, z)]*coef)
                 segmentStream[j].append([(x, y, z)]+s)
@@ -1045,15 +1082,15 @@
 
         previous_point = point
 
     return (voxelStream, segmentStream)
 
 
 def plot_streamline_metrics(trk, tList: list, metric_maps: list,
-                            method_list: list = ['vol', 'cfo', 'ang'],
+                            method_list: list = ['vol', 'cfo', 'ang', 'raw'],
                             streamline_number: int = 0, fList: list = [],
                             segment_wise: bool = True, groundTruth_map=None,
                             barplot: bool = True):
     '''
     Plots the evolution of a metric along the course of a single streamline.
```

### Comparing `unravel-python-1.2.5/unravel/example.py` & `unravel-python-1.2.6/unravel/example.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.5/unravel/utils.py` & `unravel-python-1.2.6/unravel/utils.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.5/unravel/viz.py` & `unravel-python-1.2.6/unravel/viz.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.5/unravel_python.egg-info/PKG-INFO` & `unravel-python-1.2.6/unravel_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unravel-python
-Version: 1.2.5
+Version: 1.2.6
 Summary: Implementation of UNRAVEL
 Home-page: https://github.com/DelinteNicolas/UNRAVEL
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

