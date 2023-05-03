# Comparing `tmp/woe_conversion-0.0.3.tar.gz` & `tmp/woe_conversion-0.0.4.tar.gz`

## Comparing `woe_conversion-0.0.3.tar` & `woe_conversion-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 woe_conversion-0.0.3/pyproject.toml~
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 woe_conversion-0.0.3/src/woe_conversion/__init__.py
--rw-r--r--   0        0        0     7998 2020-02-02 00:00:00.000000 woe_conversion-0.0.3/src/woe_conversion/woe.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 woe_conversion-0.0.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 woe_conversion-0.0.3/LICENSE~
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 woe_conversion-0.0.3/README.md
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 woe_conversion-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 woe_conversion-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 woe_conversion-0.0.4/README.md~
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 woe_conversion-0.0.4/pyproject.toml~
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 woe_conversion-0.0.4/src/woe_conversion/__init__.py
+-rw-r--r--   0        0        0     7998 2020-02-02 00:00:00.000000 woe_conversion-0.0.4/src/woe_conversion/woe.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 woe_conversion-0.0.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 woe_conversion-0.0.4/LICENSE~
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 woe_conversion-0.0.4/README.md
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 woe_conversion-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 woe_conversion-0.0.4/PKG-INFO
```

### Comparing `woe_conversion-0.0.3/pyproject.toml~` & `woe_conversion-0.0.4/pyproject.toml~`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling","pandas","numpy"]
 build-backend = "hatchling.build"
 
 [project]
 name = "woe_conversion"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Bertrand Brelier", email="bertrand.brelier@gmail.com" },
 ]
 description = "woe is a Python library designed to convert categorical and continuous variables into weight of evidence. Weight of evidence is a statistical technique used in information theory to measure the strength of a relationship between a binary target variable and a predictor variable. The library can be used for data preprocessing in predictive modeling or machine learning projects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `woe_conversion-0.0.3/src/woe_conversion/woe.py` & `woe_conversion-0.0.4/src/woe_conversion/woe.py`

 * *Files identical despite different names*

### Comparing `woe_conversion-0.0.3/LICENSE` & `woe_conversion-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `woe_conversion-0.0.3/README.md` & `woe_conversion-0.0.4/README.md~`

 * *Files identical despite different names*

### Comparing `woe_conversion-0.0.3/pyproject.toml` & `woe_conversion-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling","pandas","numpy"]
 build-backend = "hatchling.build"
 
 [project]
 name = "woe_conversion"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Bertrand Brelier", email="bertrand.brelier@gmail.com" },
 ]
 description = "woe is a Python library designed to convert categorical and continuous variables into weight of evidence. Weight of evidence is a statistical technique used in information theory to measure the strength of a relationship between a binary target variable and a predictor variable. The library can be used for data preprocessing in predictive modeling or machine learning projects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `woe_conversion-0.0.3/PKG-INFO` & `woe_conversion-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woe_conversion
-Version: 0.0.3
+Version: 0.0.4
 Summary: woe is a Python library designed to convert categorical and continuous variables into weight of evidence. Weight of evidence is a statistical technique used in information theory to measure the strength of a relationship between a binary target variable and a predictor variable. The library can be used for data preprocessing in predictive modeling or machine learning projects.
 Project-URL: Homepage, https://github.com/BertrandBrelier/woe
 Project-URL: Bug Tracker, https://github.com/BertrandBrelier/woe
 Author-email: Bertrand Brelier <bertrand.brelier@gmail.com>
 License-File: LICENSE
 License-File: LICENSE~
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Description-Content-Type: text/markdown
 
 # woe
 woe is a Python library designed to convert categorical and continuous variables into weight of evidence. Weight of evidence is a statistical technique used in information theory to measure the "strength" of a relationship between a binary target variable and a predictor variable. The library can be used for data preprocessing in predictive modeling or machine learning projects.
 
 
 ```
-from woe import *
+from woe_conversion.woe import *
 
 # create an instance of the WoeConversion class
 woemodel = WoeConversion(binarytarget='survived', features=['categorical_variable_1','categorical_variable_2','continuous_variable_3'])
 
 # fit the model using training data
 woemodel.fit(train)
```

