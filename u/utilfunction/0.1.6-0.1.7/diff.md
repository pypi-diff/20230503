# Comparing `tmp/utilfunction-0.1.6.tar.gz` & `tmp/utilfunction-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilfunction-0.1.6.tar", last modified: Sun Apr 30 10:11:04 2023, max compression
+gzip compressed data, was "utilfunction-0.1.7.tar", last modified: Wed May  3 17:12:46 2023, max compression
```

## Comparing `utilfunction-0.1.6.tar` & `utilfunction-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 10:11:04.265452 utilfunction-0.1.6/
--rw-rw-rw-   0        0        0    11357 2023-04-07 11:02:26.000000 utilfunction-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     4045 2023-04-30 10:11:04.264454 utilfunction-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     3175 2023-04-30 09:53:12.000000 utilfunction-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-04-30 10:11:04.265452 utilfunction-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1614 2023-04-30 10:10:29.000000 utilfunction-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 10:11:04.246156 utilfunction-0.1.6/utilfunction/
--rw-rw-rw-   0        0        0      978 2023-04-30 10:10:35.000000 utilfunction-0.1.6/utilfunction/__init__.py
--rw-rw-rw-   0        0        0      758 2023-04-07 12:03:50.000000 utilfunction-0.1.6/utilfunction/astyper.py
--rw-rw-rw-   0        0        0      484 2023-04-13 09:24:19.000000 utilfunction-0.1.6/utilfunction/beep.py
--rw-rw-rw-   0        0        0     1654 2023-04-30 10:09:51.000000 utilfunction-0.1.6/utilfunction/bib2md.py
--rw-rw-rw-   0        0        0     1182 2023-04-07 11:44:57.000000 utilfunction-0.1.6/utilfunction/path_finder.py
-drwxrwxrwx   0        0        0        0 2023-04-30 10:11:04.262457 utilfunction-0.1.6/utilfunction.egg-info/
--rw-rw-rw-   0        0        0     4045 2023-04-30 10:11:04.000000 utilfunction-0.1.6/utilfunction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-04-30 10:11:04.000000 utilfunction-0.1.6/utilfunction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 10:11:04.000000 utilfunction-0.1.6/utilfunction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-30 10:11:04.000000 utilfunction-0.1.6/utilfunction.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-30 10:11:04.000000 utilfunction-0.1.6/utilfunction.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 17:12:46.037575 utilfunction-0.1.7/
+-rw-rw-rw-   0        0        0    11357 2023-04-07 11:02:26.000000 utilfunction-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     4045 2023-05-03 17:12:46.036511 utilfunction-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3175 2023-04-30 09:53:12.000000 utilfunction-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-03 17:12:46.038114 utilfunction-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1625 2023-05-03 17:12:20.000000 utilfunction-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 17:12:46.009261 utilfunction-0.1.7/utilfunction/
+-rw-rw-rw-   0        0        0      978 2023-05-03 17:12:27.000000 utilfunction-0.1.7/utilfunction/__init__.py
+-rw-rw-rw-   0        0        0      756 2023-05-03 17:11:39.000000 utilfunction-0.1.7/utilfunction/astyper.py
+-rw-rw-rw-   0        0        0      487 2023-05-03 17:11:39.000000 utilfunction-0.1.7/utilfunction/beep.py
+-rw-rw-rw-   0        0        0     1661 2023-05-03 17:11:39.000000 utilfunction-0.1.7/utilfunction/bib2md.py
+-rw-rw-rw-   0        0        0     1182 2023-04-07 11:44:57.000000 utilfunction-0.1.7/utilfunction/path_finder.py
+drwxrwxrwx   0        0        0        0 2023-05-03 17:12:46.033832 utilfunction-0.1.7/utilfunction.egg-info/
+-rw-rw-rw-   0        0        0     4045 2023-05-03 17:12:45.000000 utilfunction-0.1.7/utilfunction.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-05-03 17:12:45.000000 utilfunction-0.1.7/utilfunction.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 17:12:45.000000 utilfunction-0.1.7/utilfunction.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-03 17:12:45.000000 utilfunction-0.1.7/utilfunction.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-03 17:12:45.000000 utilfunction-0.1.7/utilfunction.egg-info/top_level.txt
```

### Comparing `utilfunction-0.1.6/LICENSE` & `utilfunction-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `utilfunction-0.1.6/PKG-INFO` & `utilfunction-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilfunction
-Version: 0.1.6
+Version: 0.1.7
 Summary: The Python package utilfunction wraps and distributes useful functions in an easy-to-use way.
 Home-page: https://github.com/DSDanielPark/utilfunction
 Author: parkminwoo
 Author-email: parkminwoo1991@gmail.com
 Keywords: Utils,Utility,Preprocessing,Analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `utilfunction-0.1.6/README.md` & `utilfunction-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `utilfunction-0.1.6/setup.py` & `utilfunction-0.1.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,24 +21,24 @@
 
 
 version = get_version()
 
 
 setup(
     name="utilfunction",
-    version="0.1.6",
+    version="0.1.7",
     author="parkminwoo",
     author_email="parkminwoo1991@gmail.com",
     description="The Python package utilfunction wraps and distributes useful functions in an easy-to-use way.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/DSDanielPark/utilfunction",
     packages=find_packages(),
     python_requires=">=3.6",
-    install_requires=["pandas", "numpy"],
+    install_requires=["pandas", "numpy", "pybtex",],
     keywords="Utils, Utility, Preprocessing, Analysis",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
```

### Comparing `utilfunction-0.1.6/utilfunction/__init__.py` & `utilfunction-0.1.7/utilfunction/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,9 +16,9 @@
 
 from utilfunction.path_finder import find_path
 from utilfunction.astyper import col_convert
 from utilfunction.beep import beep
 from utilfunction.bib2md import convert_bib2md, bib_to_markdown
 
 __all__ = ["find_path", "col_convert", "beep", "convert_bib2md", "bib_to_markdown"]
-__version__ = "0.1.6"
+__version__ = "0.1.7"
 __author__ = "MinWoo Park <parkminwoo1991@gmail.com>"
```

### Comparing `utilfunction-0.1.6/utilfunction/astyper.py` & `utilfunction-0.1.7/utilfunction/astyper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-
 import numpy as np
 
+
 def convert(x):
-    x = x.strip()  
-    x = x[1:-1]   
-    x = np.fromstring(x, sep=' ') 
+    x = x.strip()
+    x = x[1:-1]
+    x = np.fromstring(x, sep=" ")
     return x
 
+
 def col_convert(df, columns):
     """Restores a column whose array is stored as a string type back to an array type.
 
     :param df: pd.DataFrame object
     :type df: _type_
     :param columns: Column name where array is stored as string type(str, list)
     :type columns: _type_
@@ -19,10 +20,10 @@
     """
     if type(columns) == list:
         for col in columns:
             df[col] = df[col].apply(convert)
     elif type(columns) == str:
         df[col] = df[col].apply(convert)
     else:
-        print('Only str or list are allowed as column arguments.')
+        print("Only str or list are allowed as column arguments.")
 
-    return df
+    return df
```

### Comparing `utilfunction-0.1.6/utilfunction/bib2md.py` & `utilfunction-0.1.7/utilfunction/bib2md.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,20 +9,21 @@
     :param title_key: The key value of the field that will be the main heading of the md file
     :type title_key: str
     :return: List of strings converted to MarkDown format
     :rtype: list
     """
     md_body = []
     for k, v in bib_field_dict.items():
-        if k ==title_key:
-            md_body.append(f'\n## {k.upper()}: {v} \n')
+        if k == title_key:
+            md_body.append(f"\n### {k.upper()}: {v} \n")
         else:
-            md_body.append(f'- **{k}:** {v} \n')
+            md_body.append(f"- **{k}:** {v} \n")
     return md_body
 
+
 def convert_bib2md(bib_path: str, title_key: str, save_md_path: str) -> list:
     """Convert bib file to markdown format
 
     :param bib_path: Input BIB file path.
     :type bib_path: str
     :param title_key: The key value of the field that will be the main heading of the md file
     :type title_key: str
@@ -32,15 +33,15 @@
     :rtype: list
     """
     parser = bibtex.Parser()
     bib_data = parser.parse_file(bib_path)
     entries_dict = bib_data.entries
 
     md_total_body = []
-    for _,v in entries_dict.items():
+    for _, v in entries_dict.items():
         bib_field_dict = dict(v.fields)
         md_total_body += bib_to_markdown(bib_field_dict, title_key)
 
-    with open(save_md_path, 'w') as f:
+    with open(save_md_path, "w") as f:
         f.write("".join(md_total_body))
 
-    return md_total_body
+    return md_total_body
```

### Comparing `utilfunction-0.1.6/utilfunction/path_finder.py` & `utilfunction-0.1.7/utilfunction/path_finder.py`

 * *Files identical despite different names*

### Comparing `utilfunction-0.1.6/utilfunction.egg-info/PKG-INFO` & `utilfunction-0.1.7/utilfunction.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilfunction
-Version: 0.1.6
+Version: 0.1.7
 Summary: The Python package utilfunction wraps and distributes useful functions in an easy-to-use way.
 Home-page: https://github.com/DSDanielPark/utilfunction
 Author: parkminwoo
 Author-email: parkminwoo1991@gmail.com
 Keywords: Utils,Utility,Preprocessing,Analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

