# Comparing `tmp/qmenta_client-0.9-py2.py3-none-any.whl.zip` & `tmp/qmenta_client-0.9.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 17793 bytes, number of entries: 13
--rw-r--r--  2.0 unx       65 b- defN 19-Sep-05 08:05 qmenta/__init__.py
--rw-r--r--  2.0 unx     9490 b- defN 19-Sep-05 08:05 qmenta/client/Account.py
--rw-r--r--  2.0 unx    43363 b- defN 19-Sep-05 08:05 qmenta/client/Project.py
--rw-r--r--  2.0 unx     8713 b- defN 19-Sep-05 08:05 qmenta/client/Subject.py
--rw-r--r--  2.0 unx        4 b- defN 19-Sep-05 08:05 qmenta/client/VERSION
--rw-r--r--  2.0 unx      342 b- defN 19-Sep-05 08:05 qmenta/client/__init__.py
--rw-r--r--  2.0 unx      487 b- defN 19-Sep-05 08:05 qmenta/client/utils.py
--rw-r--r--  2.0 unx       10 b- defN 19-Sep-05 08:05 qmenta_client-0.9.dist-info/DESCRIPTION.rst
--rw-r--r--  2.0 unx      724 b- defN 19-Sep-05 08:05 qmenta_client-0.9.dist-info/metadata.json
--rw-r--r--  2.0 unx        7 b- defN 19-Sep-05 08:05 qmenta_client-0.9.dist-info/top_level.txt
--rw-r--r--  2.0 unx      110 b- defN 19-Sep-05 08:05 qmenta_client-0.9.dist-info/WHEEL
--rw-r--r--  2.0 unx      535 b- defN 19-Sep-05 08:05 qmenta_client-0.9.dist-info/METADATA
--rw-r--r--  2.0 unx     1072 b- defN 19-Sep-05 08:05 qmenta_client-0.9.dist-info/RECORD
-13 files, 64922 bytes uncompressed, 16011 bytes compressed:  75.3%
+Zip file size: 17826 bytes, number of entries: 13
+-rw-r--r--  2.0 unx       65 b- defN 21-Feb-18 15:46 qmenta/__init__.py
+-rw-r--r--  2.0 unx     9490 b- defN 21-Feb-18 15:46 qmenta/client/Account.py
+-rw-r--r--  2.0 unx    43363 b- defN 21-Feb-18 15:46 qmenta/client/Project.py
+-rw-r--r--  2.0 unx     8713 b- defN 21-Feb-18 15:46 qmenta/client/Subject.py
+-rw-r--r--  2.0 unx        6 b- defN 21-Feb-18 15:47 qmenta/client/VERSION
+-rw-r--r--  2.0 unx      342 b- defN 21-Feb-18 15:46 qmenta/client/__init__.py
+-rw-r--r--  2.0 unx      487 b- defN 21-Feb-18 15:46 qmenta/client/utils.py
+-rw-r--r--  2.0 unx       10 b- defN 21-Feb-18 15:47 qmenta_client-0.9.1.dist-info/DESCRIPTION.rst
+-rw-r--r--  2.0 unx      728 b- defN 21-Feb-18 15:47 qmenta_client-0.9.1.dist-info/metadata.json
+-rw-r--r--  2.0 unx        7 b- defN 21-Feb-18 15:47 qmenta_client-0.9.1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      110 b- defN 21-Feb-18 15:47 qmenta_client-0.9.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      539 b- defN 21-Feb-18 15:47 qmenta_client-0.9.1.dist-info/METADATA
+-rw-r--r--  2.0 unx     1084 b- defN 21-Feb-18 15:47 qmenta_client-0.9.1.dist-info/RECORD
+13 files, 64944 bytes uncompressed, 16020 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: qmenta/client/__init__.py
 Comment: 
 
 Filename: qmenta/client/utils.py
 Comment: 
 
-Filename: qmenta_client-0.9.dist-info/DESCRIPTION.rst
+Filename: qmenta_client-0.9.1.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: qmenta_client-0.9.dist-info/metadata.json
+Filename: qmenta_client-0.9.1.dist-info/metadata.json
 Comment: 
 
-Filename: qmenta_client-0.9.dist-info/top_level.txt
+Filename: qmenta_client-0.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: qmenta_client-0.9.dist-info/WHEEL
+Filename: qmenta_client-0.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: qmenta_client-0.9.dist-info/METADATA
+Filename: qmenta_client-0.9.1.dist-info/METADATA
 Comment: 
 
-Filename: qmenta_client-0.9.dist-info/RECORD
+Filename: qmenta_client-0.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qmenta/client/VERSION

```diff
@@ -1 +1 @@
-0.9
+0.9.1
```

## Comparing `qmenta_client-0.9.dist-info/metadata.json` & `qmenta_client-0.9.1.dist-info/metadata.json`

 * *Files 2% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9416666666666668%*

 * *Differences: {"'run_requires'": "{0: {'requires': {insert: [(1, 'qmenta-core (~=1.0.0)')], delete: [1]}}}",*

 * * "'version'": "'0.9.1'"}*

```diff
@@ -27,15 +27,15 @@
     "generator": "bdist_wheel (0.30.0)",
     "metadata_version": "2.0",
     "name": "qmenta-client",
     "run_requires": [
         {
             "requires": [
                 "future",
-                "qmenta-core (~=1.0)"
+                "qmenta-core (~=1.0.0)"
             ]
         },
         {
             "extra": "sphinx",
             "requires": [
                 "sphinx-rtd-theme"
             ]
@@ -46,9 +46,9 @@
         {
             "requires": [
                 "flake8",
                 "pytest"
             ]
         }
     ],
-    "version": "0.9"
+    "version": "0.9.1"
 }
```

## Comparing `qmenta_client-0.9.dist-info/METADATA` & `qmenta_client-0.9.1.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.0
 Name: qmenta-client
-Version: 0.9
+Version: 0.9.1
 Summary: Python client lib to interact with the QMENTA platform.
 Home-page: http://www.qmenta.com
 Author: QMENTA
 Author-email: dev@qmenta.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Provides-Extra: sphinx
-Requires-Dist: qmenta-core (~=1.0)
+Requires-Dist: qmenta-core (~=1.0.0)
 Requires-Dist: future
 Provides-Extra: sphinx
 Requires-Dist: sphinx-rtd-theme; extra == 'sphinx'
 
 UNKNOWN
```

## Comparing `qmenta_client-0.9.dist-info/RECORD` & `qmenta_client-0.9.1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 qmenta/__init__.py,sha256=jv2YF__bseklT3OWEzlqJ5qE24c4aWd5F4r0TTjOrWQ,65
 qmenta/client/Account.py,sha256=LhUqPcB_GNGNffPJeZ6QyfLlEmbVHts1JHxITLAwE1M,9490
 qmenta/client/Project.py,sha256=XvxFwPFPQZnqmQ6bbL_wvue9LmQ3iImxCuxWf-XOzHQ,43363
 qmenta/client/Subject.py,sha256=azcLeYKO8KTLq-dn0CNvhD9XN1tGjAXZS3lFZcFHDuc,8713
-qmenta/client/VERSION,sha256=qDmrBEey1BX-FzI4eTi14Gqp1aun7Q8Mkng38OdwJ_I,4
+qmenta/client/VERSION,sha256=F5pTkJZuhcIHGofBsx3hPfZ0YGZRlvZSn4xJhoQvgeU,6
 qmenta/client/__init__.py,sha256=rOPKFOABbX3cE08upA--6BCJ1fMVb2fboRFJyKvyW2o,342
 qmenta/client/utils.py,sha256=er8BT64WBbNYj4FysI1Mx3ZqHkOGCZPIMGcZeFDysrA,487
-qmenta_client-0.9.dist-info/DESCRIPTION.rst,sha256=OCTuuN6LcWulhHS3d5rfjdsQtW22n7HENFRh6jC6ego,10
-qmenta_client-0.9.dist-info/METADATA,sha256=iJphHATuu4Gopwr_vMZ7jaY76bfWjR79BywgvqxAjMk,535
-qmenta_client-0.9.dist-info/RECORD,,
-qmenta_client-0.9.dist-info/WHEEL,sha256=kdsN-5OJAZIiHN-iO4Rhl82KyS0bDWf4uBwMbkNafr8,110
-qmenta_client-0.9.dist-info/metadata.json,sha256=QU-wowzNiMn1LJ1Ioys4KQMjw97Ghd-0DUKvZSTfauo,724
-qmenta_client-0.9.dist-info/top_level.txt,sha256=1f4U7brYlItXcJdTXWbLQ8ADst1g5awG2lSPYnKJHHs,7
+qmenta_client-0.9.1.dist-info/DESCRIPTION.rst,sha256=OCTuuN6LcWulhHS3d5rfjdsQtW22n7HENFRh6jC6ego,10
+qmenta_client-0.9.1.dist-info/METADATA,sha256=nkRPkx-EJ5LvE7hIlJ7Rg2SVOtq9Q8jQIAPY90oFXeM,539
+qmenta_client-0.9.1.dist-info/RECORD,,
+qmenta_client-0.9.1.dist-info/WHEEL,sha256=kdsN-5OJAZIiHN-iO4Rhl82KyS0bDWf4uBwMbkNafr8,110
+qmenta_client-0.9.1.dist-info/metadata.json,sha256=9twmn4TEFhgJFfY1f7Q7yJn17sNDT7HEM7NZncNHJD8,728
+qmenta_client-0.9.1.dist-info/top_level.txt,sha256=1f4U7brYlItXcJdTXWbLQ8ADst1g5awG2lSPYnKJHHs,7
```

