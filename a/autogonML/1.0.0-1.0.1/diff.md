# Comparing `tmp/autogonML-1.0.0-py3-none-any.whl.zip` & `tmp/autogonML-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,13 @@
-Zip file size: 15436 bytes, number of entries: 17
+Zip file size: 8609 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 23-May-03 00:26 autogon_internal/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-03 00:46 autogon_internal/autoClassification/__init__.py
 -rw-r--r--  2.0 unx     3987 b- defN 23-May-01 01:21 autogon_internal/autoClassification/base.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-03 00:47 autogon_internal/autoFeatureEngineering/__init__.py
 -rw-r--r--  2.0 unx    17242 b- defN 23-May-01 01:30 autogon_internal/autoFeatureEngineering/base.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-03 00:47 autogon_internal/autoRegression/__init__.py
 -rw-r--r--  2.0 unx     2809 b- defN 23-May-03 00:48 autogon_internal/autoRegression/base.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 00:46 autogon_ml/autoClassification/__init__.py
--rw-r--r--  2.0 unx     3987 b- defN 23-May-01 01:21 autogon_ml/autoClassification/base.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 00:47 autogon_ml/autoFeatureEngineering/__init__.py
--rw-r--r--  2.0 unx    17242 b- defN 23-May-01 01:30 autogon_ml/autoFeatureEngineering/base.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 00:47 autogon_ml/autoRegression/__init__.py
--rw-r--r--  2.0 unx     2809 b- defN 23-May-03 00:48 autogon_ml/autoRegression/base.py
--rw-r--r--  2.0 unx     1241 b- defN 23-May-03 01:21 autogonML-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-03 01:21 autogonML-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-03 01:21 autogonML-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1560 b- defN 23-May-03 01:21 autogonML-1.0.0.dist-info/RECORD
-17 files, 50980 bytes uncompressed, 12786 bytes compressed:  74.9%
+-rw-r--r--  2.0 unx     1241 b- defN 23-May-03 01:18 autogonML-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-03 01:18 autogonML-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-May-03 01:18 autogonML-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      992 b- defN 23-May-03 01:18 autogonML-1.0.1.dist-info/RECORD
+11 files, 26380 bytes uncompressed, 6883 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -15,38 +15,20 @@
 
 Filename: autogon_internal/autoRegression/__init__.py
 Comment: 
 
 Filename: autogon_internal/autoRegression/base.py
 Comment: 
 
-Filename: autogon_ml/autoClassification/__init__.py
+Filename: autogonML-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: autogon_ml/autoClassification/base.py
+Filename: autogonML-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: autogon_ml/autoFeatureEngineering/__init__.py
+Filename: autogonML-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: autogon_ml/autoFeatureEngineering/base.py
-Comment: 
-
-Filename: autogon_ml/autoRegression/__init__.py
-Comment: 
-
-Filename: autogon_ml/autoRegression/base.py
-Comment: 
-
-Filename: autogonML-1.0.0.dist-info/METADATA
-Comment: 
-
-Filename: autogonML-1.0.0.dist-info/WHEEL
-Comment: 
-
-Filename: autogonML-1.0.0.dist-info/top_level.txt
-Comment: 
-
-Filename: autogonML-1.0.0.dist-info/RECORD
+Filename: autogonML-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `autogonML-1.0.0.dist-info/METADATA` & `autogonML-1.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogonML
-Version: 1.0.0
+Version: 1.0.1
 Summary: ...
 Author: Autogon Inc
 Author-email: developer@autogon.ai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

## Comparing `autogonML-1.0.0.dist-info/RECORD` & `autogonML-1.0.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 autogon_internal/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 autogon_internal/autoClassification/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 autogon_internal/autoClassification/base.py,sha256=7XpI_jJjcKPHaE5KBgLAKJwZ7eTRzg6itkqcg15uaO0,3987
 autogon_internal/autoFeatureEngineering/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 autogon_internal/autoFeatureEngineering/base.py,sha256=8GhYR2mVZ8fe4lmQrIxzG14cJEGXILQ7ogF8uBd5fCw,17242
 autogon_internal/autoRegression/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 autogon_internal/autoRegression/base.py,sha256=xdgQ0KwFQRZ5lukNI480WDmvIXpArtsatRqpR8MJ75c,2809
-autogon_ml/autoClassification/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-autogon_ml/autoClassification/base.py,sha256=7XpI_jJjcKPHaE5KBgLAKJwZ7eTRzg6itkqcg15uaO0,3987
-autogon_ml/autoFeatureEngineering/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-autogon_ml/autoFeatureEngineering/base.py,sha256=8GhYR2mVZ8fe4lmQrIxzG14cJEGXILQ7ogF8uBd5fCw,17242
-autogon_ml/autoRegression/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-autogon_ml/autoRegression/base.py,sha256=xdgQ0KwFQRZ5lukNI480WDmvIXpArtsatRqpR8MJ75c,2809
-autogonML-1.0.0.dist-info/METADATA,sha256=4OXSmQp8WRo5DbxG_6rf0tleH-UQVlOhIJmPJF-q0_U,1241
-autogonML-1.0.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-autogonML-1.0.0.dist-info/top_level.txt,sha256=HlImT5g_V4QpIsULXdsFPyf8DJUsBzKnYEDQTGzI6JE,11
-autogonML-1.0.0.dist-info/RECORD,,
+autogonML-1.0.1.dist-info/METADATA,sha256=Px9z9jRL3hylLfhWxnBGHt254Bz-s975Nt-I0M3h7Js,1241
+autogonML-1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+autogonML-1.0.1.dist-info/top_level.txt,sha256=qup40vJ4-MQZvFT0sOTF-aHfraZe-f-hL3c-7rNXHJw,17
+autogonML-1.0.1.dist-info/RECORD,,
```

