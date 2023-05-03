# Comparing `tmp/eric_chen_forward-0.0.8.tar.gz` & `tmp/eric_chen_forward-0.0.9.tar.gz`

## Comparing `eric_chen_forward-0.0.8.tar` & `eric_chen_forward-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.8/eric_chen_forward/database.py
--rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.8/eric_chen_forward/model.py
--rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.8/eric_chen_forward/url_classifier_demo.py
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.8/eric_chen_forward/util.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.8/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.8/LICENSE
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.8/README.md
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.9/eric_chen_forward/database.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.9/eric_chen_forward/model.py
+-rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.9/eric_chen_forward/url_classifier_demo.py
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.9/eric_chen_forward/util.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.9/README.md
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 eric_chen_forward-0.0.9/PKG-INFO
```

### Comparing `eric_chen_forward-0.0.8/eric_chen_forward/model.py` & `eric_chen_forward-0.0.9/eric_chen_forward/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 class Classifier:
 
     def __init__(self) -> None:
         self.eda_util = util.EDA(alpha=0.2)
         self.categories = []
 
-    def train(self, labels_file, passages_file, csv_file=None):
+    def train(self, labels_file=None, passages_file=None, csv_file=None):
         if csv_file:
             df = pd.read_csv(csv_file)
             labels = df['label'].to_list()
             passages = df['passage'].to_list()
         else:
             with open(labels_file) as f:
                 labels = f.read().splitlines()
```

### Comparing `eric_chen_forward-0.0.8/eric_chen_forward/url_classifier_demo.py` & `eric_chen_forward-0.0.9/eric_chen_forward/url_classifier_demo.py`

 * *Files identical despite different names*

### Comparing `eric_chen_forward-0.0.8/eric_chen_forward/util.py` & `eric_chen_forward-0.0.9/eric_chen_forward/util.py`

 * *Files identical despite different names*

### Comparing `eric_chen_forward-0.0.8/.gitignore` & `eric_chen_forward-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `eric_chen_forward-0.0.8/LICENSE` & `eric_chen_forward-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eric_chen_forward-0.0.8/README.md` & `eric_chen_forward-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `eric_chen_forward-0.0.8/pyproject.toml` & `eric_chen_forward-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "eric_chen_forward"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Eric Chen", email="ezchen2556@gmail.com" },
 ]
 description = "Classifier for institution and scholar data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `eric_chen_forward-0.0.8/PKG-INFO` & `eric_chen_forward-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eric_chen_forward
-Version: 0.0.8
+Version: 0.0.9
 Summary: Classifier for institution and scholar data
 Project-URL: Homepage, https://github.com/ezrc2/eric_chen_forward
 Author-email: Eric Chen <ezchen2556@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

