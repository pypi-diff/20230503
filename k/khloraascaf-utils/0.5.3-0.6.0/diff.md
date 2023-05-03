# Comparing `tmp/khloraascaf_utils-0.5.3.tar.gz` & `tmp/khloraascaf_utils-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khloraascaf_utils-0.5.3.tar", last modified: Tue Apr 18 15:10:38 2023, max compression
+gzip compressed data, was "khloraascaf_utils-0.6.0.tar", last modified: Wed May  3 11:09:50 2023, max compression
```

## Comparing `khloraascaf_utils-0.5.3.tar` & `khloraascaf_utils-0.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:10:38.311039 khloraascaf_utils-0.5.3/
--rw-rw-rw-   0 root         (0) root         (0)    34916 2023-04-18 15:10:13.000000 khloraascaf_utils-0.5.3/LICENCE
--rw-r--r--   0 root         (0) root         (0)    43838 2023-04-18 15:10:38.310039 khloraascaf_utils-0.5.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2535 2023-04-18 15:10:13.000000 khloraascaf_utils-0.5.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-04-18 15:10:13.000000 khloraascaf_utils-0.5.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 15:10:38.311039 khloraascaf_utils-0.5.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:10:38.303039 khloraascaf_utils-0.5.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:10:38.306039 khloraascaf_utils-0.5.3/src/khloraascaf_utils/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-04-18 15:10:13.000000 khloraascaf_utils-0.5.3/src/khloraascaf_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7074 2023-04-18 15:10:13.000000 khloraascaf_utils-0.5.3/src/khloraascaf_utils/artificial_data.py
--rw-rw-rw-   0 root         (0) root         (0)     7169 2023-04-18 15:10:13.000000 khloraascaf_utils-0.5.3/src/khloraascaf_utils/asm_graph_to_fasta.py
--rw-rw-rw-   0 root         (0) root         (0)     2388 2023-04-18 15:10:13.000000 khloraascaf_utils-0.5.3/src/khloraascaf_utils/contigs_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    13756 2023-04-18 15:10:13.000000 khloraascaf_utils-0.5.3/src/khloraascaf_utils/to_networkx.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:10:38.308039 khloraascaf_utils-0.5.3/src/khloraascaf_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)    43838 2023-04-18 15:10:38.000000 khloraascaf_utils-0.5.3/src/khloraascaf_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      552 2023-04-18 15:10:38.000000 khloraascaf_utils-0.5.3/src/khloraascaf_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 15:10:38.000000 khloraascaf_utils-0.5.3/src/khloraascaf_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-18 15:10:38.000000 khloraascaf_utils-0.5.3/src/khloraascaf_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-18 15:10:38.000000 khloraascaf_utils-0.5.3/src/khloraascaf_utils.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:10:38.310039 khloraascaf_utils-0.5.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3364 2023-04-18 15:10:13.000000 khloraascaf_utils-0.5.3/tests/test_artificial_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3590 2023-04-18 15:10:13.000000 khloraascaf_utils-0.5.3/tests/test_asm_graph_to_fasta.py
--rw-rw-rw-   0 root         (0) root         (0)     1770 2023-04-18 15:10:13.000000 khloraascaf_utils-0.5.3/tests/test_contigs_attributes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 11:09:50.783139 khloraascaf_utils-0.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)    34916 2023-05-03 11:09:32.000000 khloraascaf_utils-0.6.0/LICENCE
+-rw-r--r--   0 root         (0) root         (0)    43838 2023-05-03 11:09:50.783139 khloraascaf_utils-0.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2535 2023-05-03 11:09:32.000000 khloraascaf_utils-0.6.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-05-03 11:09:32.000000 khloraascaf_utils-0.6.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 11:09:50.784139 khloraascaf_utils-0.6.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 11:09:50.776138 khloraascaf_utils-0.6.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 11:09:50.779139 khloraascaf_utils-0.6.0/src/khloraascaf_utils/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-03 11:09:32.000000 khloraascaf_utils-0.6.0/src/khloraascaf_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8061 2023-05-03 11:09:32.000000 khloraascaf_utils-0.6.0/src/khloraascaf_utils/artificial_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     7169 2023-05-03 11:09:32.000000 khloraascaf_utils-0.6.0/src/khloraascaf_utils/asm_graph_to_fasta.py
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2023-05-03 11:09:32.000000 khloraascaf_utils-0.6.0/src/khloraascaf_utils/contigs_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    13756 2023-05-03 11:09:32.000000 khloraascaf_utils-0.6.0/src/khloraascaf_utils/to_networkx.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 11:09:50.781139 khloraascaf_utils-0.6.0/src/khloraascaf_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    43838 2023-05-03 11:09:50.000000 khloraascaf_utils-0.6.0/src/khloraascaf_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      552 2023-05-03 11:09:50.000000 khloraascaf_utils-0.6.0/src/khloraascaf_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 11:09:50.000000 khloraascaf_utils-0.6.0/src/khloraascaf_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-03 11:09:50.000000 khloraascaf_utils-0.6.0/src/khloraascaf_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-03 11:09:50.000000 khloraascaf_utils-0.6.0/src/khloraascaf_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 11:09:50.783139 khloraascaf_utils-0.6.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4111 2023-05-03 11:09:32.000000 khloraascaf_utils-0.6.0/tests/test_artificial_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3590 2023-05-03 11:09:32.000000 khloraascaf_utils-0.6.0/tests/test_asm_graph_to_fasta.py
+-rw-rw-rw-   0 root         (0) root         (0)     1770 2023-05-03 11:09:32.000000 khloraascaf_utils-0.6.0/tests/test_contigs_attributes.py
```

### Comparing `khloraascaf_utils-0.5.3/LICENCE` & `khloraascaf_utils-0.6.0/LICENCE`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.5.3/PKG-INFO` & `khloraascaf_utils-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf_utils
-Version: 0.5.3
+Version: 0.6.0
 Summary: Python utilities for khloraascaf python package.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
```

### Comparing `khloraascaf_utils-0.5.3/README.md` & `khloraascaf_utils-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.5.3/pyproject.toml` & `khloraascaf_utils-0.6.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 
 name = "khloraascaf_utils"
-version = "0.5.3"
+version = "0.6.0"
 authors = [{ name = "vepain", email = "victor.epain@laposte.net" }]
 description = "Python utilities for khloraascaf python package."
 keywords = ["Scaffolding", "Chloroplast", "Assembly", "DNA repeats"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `khloraascaf_utils-0.5.3/src/khloraascaf_utils/artificial_data.py` & `khloraascaf_utils-0.6.0/src/khloraascaf_utils/artificial_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -89,14 +89,50 @@
             Second oriented contig
         """
         for l_ind, (u, v) in enumerate(self.__links):
             yield l_ind, u, v
         for l_ind, (u, v) in enumerate(self.__extra_links):
             yield l_ind + len(self.__links), u, v
 
+    def extra_links(self) -> Iterator[tuple[IndexT, IndOrT, IndOrT]]:
+        """Iterate over the links.
+
+        Yields
+        ------
+        IndexT
+            Link's index
+        IndOrT
+            First oriented contig
+        IndOrT
+            Second oriented contig
+        """
+        for l_ind, (u, v) in enumerate(self.__extra_links):
+            yield l_ind + len(self.__links), u, v
+
+    def region_contigs(self, region_ind: IndexT) -> (
+            Iterator[tuple[IndexT, MultT, PresScoreT]]):
+        """Iterate over the contigs and their attributes of a region.
+
+        Parameters
+        ----------
+        region_ind : IndexT
+            Index of the region
+
+        Yields
+        ------
+        IndexT
+            Contig's index
+        MultT
+            Contig's multiplicity
+        PresScoreT
+            Contig's presence score
+        """
+        for c_ind, _ in self.__region_oriented_contig[region_ind]:
+            yield c_ind, *self.__contig_attrs[c_ind]
+
     # ~*~ Regions ~*~
 
     def __generate_region_orc(self, region_length: list[int]):
         for reg_ind, _ in self.__oriented_region_order:
             if reg_ind == len(self.__region_oriented_contig):
                 # Generate the region
                 self.__region_oriented_contig.append([])
```

### Comparing `khloraascaf_utils-0.5.3/src/khloraascaf_utils/asm_graph_to_fasta.py` & `khloraascaf_utils-0.6.0/src/khloraascaf_utils/asm_graph_to_fasta.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.5.3/src/khloraascaf_utils/contigs_attributes.py` & `khloraascaf_utils-0.6.0/src/khloraascaf_utils/contigs_attributes.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.5.3/src/khloraascaf_utils/to_networkx.py` & `khloraascaf_utils-0.6.0/src/khloraascaf_utils/to_networkx.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.5.3/src/khloraascaf_utils.egg-info/PKG-INFO` & `khloraascaf_utils-0.6.0/src/khloraascaf_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf-utils
-Version: 0.5.3
+Version: 0.6.0
 Summary: Python utilities for khloraascaf python package.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
```

### Comparing `khloraascaf_utils-0.5.3/src/khloraascaf_utils.egg-info/SOURCES.txt` & `khloraascaf_utils-0.6.0/src/khloraascaf_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.5.3/tests/test_asm_graph_to_fasta.py` & `khloraascaf_utils-0.6.0/tests/test_asm_graph_to_fasta.py`

 * *Files identical despite different names*

### Comparing `khloraascaf_utils-0.5.3/tests/test_contigs_attributes.py` & `khloraascaf_utils-0.6.0/tests/test_contigs_attributes.py`

 * *Files identical despite different names*

