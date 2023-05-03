# Comparing `tmp/vit_keras-0.1.1-py3-none-any.whl.zip` & `tmp/vit_keras-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 24503 bytes, number of entries: 10
 -rw-r--r--  2.0 unx       22 b- defN 80-Jan-01 00:00 vit_keras/__init__.py
 -rw-r--r--  2.0 unx    21674 b- defN 80-Jan-01 00:00 vit_keras/imagenet2012.txt
 -rw-r--r--  2.0 unx     6595 b- defN 80-Jan-01 00:00 vit_keras/layers.py
 -rw-r--r--  2.0 unx     8266 b- defN 80-Jan-01 00:00 vit_keras/utils.py
 -rw-r--r--  2.0 unx     1939 b- defN 80-Jan-01 00:00 vit_keras/visualize.py
 -rw-r--r--  2.0 unx     9706 b- defN 80-Jan-01 00:00 vit_keras/vit.py
--rw-r--r--  2.0 unx    10761 b- defN 80-Jan-01 00:00 vit_keras-0.1.1.dist-info/LICENSE
-?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 vit_keras-0.1.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     4039 b- defN 16-Jan-01 00:00 vit_keras-0.1.1.dist-info/METADATA
-?rw-r--r--  2.0 unx      766 b- defN 16-Jan-01 00:00 vit_keras-0.1.1.dist-info/RECORD
+-rw-r--r--  2.0 unx    10761 b- defN 80-Jan-01 00:00 vit_keras-0.1.2.dist-info/LICENSE
+?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 vit_keras-0.1.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     4039 b- defN 16-Jan-01 00:00 vit_keras-0.1.2.dist-info/METADATA
+?rw-r--r--  2.0 unx      766 b- defN 16-Jan-01 00:00 vit_keras-0.1.2.dist-info/RECORD
 10 files, 63856 bytes uncompressed, 23217 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: vit_keras/visualize.py
 Comment: 
 
 Filename: vit_keras/vit.py
 Comment: 
 
-Filename: vit_keras-0.1.1.dist-info/LICENSE
+Filename: vit_keras-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: vit_keras-0.1.1.dist-info/WHEEL
+Filename: vit_keras-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: vit_keras-0.1.1.dist-info/METADATA
+Filename: vit_keras-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: vit_keras-0.1.1.dist-info/RECORD
+Filename: vit_keras-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vit_keras/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

## vit_keras/visualize.py

```diff
@@ -8,15 +8,15 @@
     """Get an attention map for an image and model using the technique
     described in Appendix D.7 in the paper (unofficial).
 
     Args:
         model: A ViT model
         image: An image for which we will compute the attention map.
     """
-    img_height, img_width = model.input_shape[0], model.input_shape[1]
+    img_height, img_width = model.input_shape[1], model.input_shape[2]
     grid_size = int(np.sqrt(model.layers[5].output_shape[0][-2] - 1))
 
     # Prepare the input
     X = vit.preprocess_inputs(cv2.resize(image, (img_height, img_width)))[np.newaxis, :]  # type: ignore
 
     # Get the attention weights from each transformer.
     outputs = [
```

## Comparing `vit_keras-0.1.1.dist-info/LICENSE` & `vit_keras-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vit_keras-0.1.1.dist-info/METADATA` & `vit_keras-0.1.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vit-keras
-Version: 0.1.1
+Version: 0.1.2
 Summary: Keras implementation of ViT (Vision Transformer)
 Home-page: https://github.com/faustomorales/vit-keras
 License: Apache-2.0
 Author: Fausto Morales
 Author-email: faustomorales@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `vit_keras-0.1.1.dist-info/RECORD` & `vit_keras-0.1.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-vit_keras/__init__.py,sha256=rnObPjuBcEStqSO0S6gsdS_ot8ITOQjVj_-P1LUUYpg,22
+vit_keras/__init__.py,sha256=YvuYzWnKtqBb-IqG8HAu-nhIYAsgj9Vmc_b9o7vO-js,22
 vit_keras/imagenet2012.txt,sha256=pA2b6C60c4vs0d1pmRuJ-H8wmXXoYKbz9FOV2MBqfg0,21674
 vit_keras/layers.py,sha256=KXphs14yDYgJ5Swki12-blIB8gdexw-yvp4ViwwvYFw,6595
 vit_keras/utils.py,sha256=NBVS1A2YVoW-puutCQhPpbRqsYAm3LzFDmSH6f-vtnA,8266
-vit_keras/visualize.py,sha256=SNAtBMg_dO2dM2bkRBV3dA-Jpy3GiZlCOiGCEF3c2uo,1939
+vit_keras/visualize.py,sha256=faCCDqaZxtYbj3nuR8fmEd3A9t8iwSnlKxZzYIT82kc,1939
 vit_keras/vit.py,sha256=GCzHLFJiGL8GMoqrqPDVWv-0_wm0E6cG7_1_WNpmyU8,9706
-vit_keras-0.1.1.dist-info/LICENSE,sha256=QLKxkBGZ8tY75WjT1av5RjJuPJvBTsXLFORWOuQ6YMw,10761
-vit_keras-0.1.1.dist-info/WHEEL,sha256=vxFmldFsRN_Hx10GDvsdv1wroKq8r5Lzvjp6GZ4OO8c,88
-vit_keras-0.1.1.dist-info/METADATA,sha256=QtQaFYdHCk7lkc8ueBxolmfqcK3uMEQaFSHDMlEK80k,4039
-vit_keras-0.1.1.dist-info/RECORD,,
+vit_keras-0.1.2.dist-info/LICENSE,sha256=QLKxkBGZ8tY75WjT1av5RjJuPJvBTsXLFORWOuQ6YMw,10761
+vit_keras-0.1.2.dist-info/WHEEL,sha256=vxFmldFsRN_Hx10GDvsdv1wroKq8r5Lzvjp6GZ4OO8c,88
+vit_keras-0.1.2.dist-info/METADATA,sha256=QLiLbzWEJJOseUs3eqLjXYqO-24FrklN1ajalwopl1E,4039
+vit_keras-0.1.2.dist-info/RECORD,,
```

