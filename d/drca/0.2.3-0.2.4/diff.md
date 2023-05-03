# Comparing `tmp/drca-0.2.3-py3-none-any.whl.zip` & `tmp/drca-0.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 9383 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat    32247 b- defN 23-Mar-23 04:55 drca/DR_assisted_CA.py
+Zip file size: 9372 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    32209 b- defN 23-May-03 04:07 drca/DR_assisted_CA.py
 -rw-rw-rw-  2.0 fat       29 b- defN 23-Feb-15 11:13 drca/__init__.py
--rw-rw-rw-  2.0 fat     1080 b- defN 23-Mar-23 04:56 drca-0.2.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      253 b- defN 23-Mar-23 04:56 drca-0.2.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-23 04:56 drca-0.2.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Mar-23 04:56 drca-0.2.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      520 b- defN 23-Mar-23 04:56 drca-0.2.3.dist-info/RECORD
-7 files, 34226 bytes uncompressed, 8465 bytes compressed:  75.3%
+-rw-rw-rw-  2.0 fat     1080 b- defN 23-May-03 04:10 drca-0.2.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      239 b- defN 23-May-03 04:10 drca-0.2.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-03 04:10 drca-0.2.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-May-03 04:10 drca-0.2.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      520 b- defN 23-May-03 04:10 drca-0.2.4.dist-info/RECORD
+7 files, 34174 bytes uncompressed, 8454 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: drca/DR_assisted_CA.py
 Comment: 
 
 Filename: drca/__init__.py
 Comment: 
 
-Filename: drca-0.2.3.dist-info/LICENSE
+Filename: drca-0.2.4.dist-info/LICENSE
 Comment: 
 
-Filename: drca-0.2.3.dist-info/METADATA
+Filename: drca-0.2.4.dist-info/METADATA
 Comment: 
 
-Filename: drca-0.2.3.dist-info/WHEEL
+Filename: drca-0.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: drca-0.2.3.dist-info/top_level.txt
+Filename: drca-0.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: drca-0.2.3.dist-info/RECORD
+Filename: drca-0.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## drca/DR_assisted_CA.py

```diff
@@ -802,22 +802,20 @@
     return coeff_reshape
 
 def label_arrangement(label_arr, new_shape):
     """
     reshape a clustering result obtained by performing OPTICS
     """
     label_sort = np.unique(label_arr)
-    #print(label_sort)
     num_label = len(label_sort)
     hist, edge = np.histogram(label_arr, bins=num_label)
-    #print(hist)
     label_reshape = reshape_coeff(label_arr.reshape(-1, 1), new_shape)
     
-    for i in range(len(label_reshape)):
-        label_reshape[i] = np.squeeze(label_reshape[i])
+    #for i in range(len(label_reshape)):
+    #    label_reshape[i] = np.squeeze(label_reshape[i])
         
     selected = []
     for i in range(num_label):
         temp = []
         for j in range(len(label_reshape)):
             img_temp = np.zeros_like(label_reshape[j])
             img_temp[np.where(label_reshape[j] == label_sort[i])] = 1.0
```

## Comparing `drca-0.2.3.dist-info/LICENSE` & `drca-0.2.4.dist-info/LICENSE`

 * *Files identical despite different names*

