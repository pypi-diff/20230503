# Comparing `tmp/dnadb-0.2.8.tar.gz` & `tmp/dnadb-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnadb-0.2.8.tar", last modified: Sun Apr 30 03:43:18 2023, max compression
+gzip compressed data, was "dnadb-0.2.9.tar", last modified: Wed May  3 02:37:08 2023, max compression
```

## Comparing `dnadb-0.2.8.tar` & `dnadb-0.2.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-30 03:43:18.608556 dnadb-0.2.8/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.2.8/LICENSE
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-04-30 03:43:18.608556 dnadb-0.2.8/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.2.8/README.md
--rw-r--r--   0 dwl2x     (1000) users      (100)      712 2023-04-21 06:50:34.000000 dnadb-0.2.8/pyproject.toml
--rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-04-30 03:43:18.608556 dnadb-0.2.8/setup.cfg
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-30 03:43:18.608556 dnadb-0.2.8/src/
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-30 03:43:18.608556 dnadb-0.2.8/src/dnadb/
--rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-04-17 03:05:03.000000 dnadb-0.2.8/src/dnadb/__init__.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-30 03:43:18.608556 dnadb-0.2.8/src/dnadb/datasets/
--rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.2.8/src/dnadb/datasets/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-03-29 23:23:08.000000 dnadb-0.2.8/src/dnadb/datasets/dataset.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.2.8/src/dnadb/datasets/greengenes.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-30 03:43:18.608556 dnadb-0.2.8/src/dnadb/datasets/silva/
--rw-r--r--   0 dwl2x     (1000) users      (100)     5492 2023-04-14 13:32:31.000000 dnadb-0.2.8/src/dnadb/datasets/silva/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-03-27 05:43:12.000000 dnadb-0.2.8/src/dnadb/datasets/silva/taxonomy_map.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1163 2023-04-30 03:41:17.000000 dnadb-0.2.8/src/dnadb/db.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6027 2023-04-02 01:42:55.000000 dnadb-0.2.8/src/dnadb/dna.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     4998 2023-04-21 05:23:34.000000 dnadb-0.2.8/src/dnadb/fasta.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6967 2023-04-21 05:23:31.000000 dnadb-0.2.8/src/dnadb/fastq.py
--rw-r--r--   0 dwl2x     (1000) users      (100)    15313 2023-04-21 05:23:29.000000 dnadb-0.2.8/src/dnadb/taxonomy.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.2.8/src/dnadb/utils.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-30 03:43:18.608556 dnadb-0.2.8/src/dnadb.egg-info/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-04-30 03:43:18.000000 dnadb-0.2.8/src/dnadb.egg-info/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)      502 2023-04-30 03:43:18.000000 dnadb-0.2.8/src/dnadb.egg-info/SOURCES.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-04-30 03:43:18.000000 dnadb-0.2.8/src/dnadb.egg-info/dependency_links.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)       40 2023-04-30 03:43:18.000000 dnadb-0.2.8/src/dnadb.egg-info/requires.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-04-30 03:43:18.000000 dnadb-0.2.8/src/dnadb.egg-info/top_level.txt
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-03 02:37:08.972353 dnadb-0.2.9/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.2.9/LICENSE
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-03 02:37:08.972353 dnadb-0.2.9/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.2.9/README.md
+-rw-r--r--   0 dwl2x     (1000) users      (100)      712 2023-05-03 02:13:13.000000 dnadb-0.2.9/pyproject.toml
+-rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-05-03 02:37:08.972353 dnadb-0.2.9/setup.cfg
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-03 02:37:08.968353 dnadb-0.2.9/src/
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-03 02:37:08.972353 dnadb-0.2.9/src/dnadb/
+-rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-05-03 02:36:07.000000 dnadb-0.2.9/src/dnadb/__init__.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-03 02:37:08.972353 dnadb-0.2.9/src/dnadb/datasets/
+-rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.2.9/src/dnadb/datasets/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-03-29 23:23:08.000000 dnadb-0.2.9/src/dnadb/datasets/dataset.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.2.9/src/dnadb/datasets/greengenes.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-03 02:37:08.972353 dnadb-0.2.9/src/dnadb/datasets/silva/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     5492 2023-04-14 13:32:31.000000 dnadb-0.2.9/src/dnadb/datasets/silva/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-03-27 05:43:12.000000 dnadb-0.2.9/src/dnadb/datasets/silva/taxonomy_map.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1163 2023-04-30 03:41:17.000000 dnadb-0.2.9/src/dnadb/db.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6027 2023-04-02 01:42:55.000000 dnadb-0.2.9/src/dnadb/dna.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     5443 2023-05-03 02:31:55.000000 dnadb-0.2.9/src/dnadb/fasta.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     7157 2023-05-03 02:31:41.000000 dnadb-0.2.9/src/dnadb/fastq.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)    15566 2023-05-03 02:35:14.000000 dnadb-0.2.9/src/dnadb/taxonomy.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.2.9/src/dnadb/utils.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-03 02:37:08.972353 dnadb-0.2.9/src/dnadb.egg-info/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-03 02:37:08.000000 dnadb-0.2.9/src/dnadb.egg-info/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)      502 2023-05-03 02:37:08.000000 dnadb-0.2.9/src/dnadb.egg-info/SOURCES.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-05-03 02:37:08.000000 dnadb-0.2.9/src/dnadb.egg-info/dependency_links.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)       40 2023-05-03 02:37:08.000000 dnadb-0.2.9/src/dnadb.egg-info/requires.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-05-03 02:37:08.000000 dnadb-0.2.9/src/dnadb.egg-info/top_level.txt
```

### Comparing `dnadb-0.2.8/LICENSE` & `dnadb-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.8/PKG-INFO` & `dnadb-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.2.8
+Version: 0.2.9
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dnadb-0.2.8/pyproject.toml` & `dnadb-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dnadb"
-version = "0.2.8"
+version = "0.2.9"
 authors = [
   { name="David Ludwig", email="davidludwigii@gmail.com" },
 ]
 description = "A library for handling DNA files."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `dnadb-0.2.8/src/dnadb/datasets/dataset.py` & `dnadb-0.2.9/src/dnadb/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.8/src/dnadb/datasets/greengenes.py` & `dnadb-0.2.9/src/dnadb/datasets/greengenes.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.8/src/dnadb/datasets/silva/__init__.py` & `dnadb-0.2.9/src/dnadb/datasets/silva/__init__.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.8/src/dnadb/datasets/silva/taxonomy_map.py` & `dnadb-0.2.9/src/dnadb/datasets/silva/taxonomy_map.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.8/src/dnadb/db.py` & `dnadb-0.2.9/src/dnadb/db.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.8/src/dnadb/dna.py` & `dnadb-0.2.9/src/dnadb/dna.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.8/src/dnadb/fasta.py` & `dnadb-0.2.9/src/dnadb/fasta.py`

 * *Files 7% similar despite different names*

```diff
@@ -89,14 +89,30 @@
         self.db = Lmdb.open(str(self.path), lock=False)
         self.length = np.frombuffer(self.db["length"], dtype=np.int32, count=1)[0]
 
     def __len__(self):
         return self.length
 
     @singledispatchmethod
+    def __contains__(self, sequence_index: int) -> bool:
+        return str(sequence_index) in self.db
+
+    @__contains__.register
+    def _(self, sequence_id: str) -> bool:
+        return f"id_{sequence_id}" in self.db
+
+    @__contains__.register
+    def _(self, entry: FastaEntry) -> bool:
+        return entry.identifier in self
+
+    def __iter__(self):
+        for i in range(len(self)):
+            yield self[i]
+
+    @singledispatchmethod
     def __getitem__(self, sequence_index: int) -> FastaEntry:
         return FastaEntry.deserialize(self.db[str(sequence_index)])
 
     @__getitem__.register
     def _(self, sequence_id: str) -> FastaEntry:
         index = np.frombuffer(self.db[f"id_{sequence_id}"], dtype=np.int32, count=1)[0]
         return self[index]
```

### Comparing `dnadb-0.2.8/src/dnadb/fastq.py` & `dnadb-0.2.9/src/dnadb/fastq.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,14 +180,21 @@
         self.path = Path(fastq_db_path).absolute()
         self.db = Lmdb.open(str(self.path), lock=False)
         self.length = np.frombuffer(self.db["length"], dtype=np.int32, count=1)[0]
 
     def __len__(self):
         return self.length
 
+    def __contains__(self, sequence_index: int) -> bool:
+        return str(sequence_index) in self.db
+
+    def __iter__(self):
+        for i in range(len(self)):
+            yield self[i]
+
     def __getitem__(self, sequence_index: int) -> FastqEntry:
         return FastqEntry.deserialize(self.db[str(sequence_index)])
 
 
 def entries(
     sequences: Union[io.TextIOBase, Iterable[FastqEntry], str, Path]
 ) -> Iterable[FastqEntry]:
```

### Comparing `dnadb-0.2.8/src/dnadb/taxonomy.py` & `dnadb-0.2.9/src/dnadb/taxonomy.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,21 +373,30 @@
 
 class TaxonomyDb:
     def __init__(self, taxonomy_db_path: Union[str, Path]):
         self.path = Path(taxonomy_db_path).absolute()
         self.db = Lmdb.open(str(self.path), lock=False)
         self.length = np.frombuffer(self.db["length"], dtype=np.int32, count=1)[0]
 
-    def __len__(self):
-        return self.length
-
     @cached_property
     def hierarchy(self):
         return TaxonomyHierarchy.deserialize(self.db["hierarchy"])
 
+    def __len__(self):
+        return self.length
+
+    def __contains__(self, sequence_id: str) -> bool:
+        return sequence_id in self.db
+
+    def __iter__(self):
+        for key in self.db.keys():
+            if key in ("length", "hierarchy"):
+                continue
+            yield self[key]
+
     def __getitem__(self, sequence_id: str) -> TaxonomyEntry:
         return TaxonomyEntry.deserialize(self.db[sequence_id])
 
 
 def entries(
     taxonomy: Union[io.TextIOBase, Iterable[TaxonomyEntry], str, Path]
 ) -> Iterable[TaxonomyEntry]:
```

### Comparing `dnadb-0.2.8/src/dnadb/utils.py` & `dnadb-0.2.9/src/dnadb/utils.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.8/src/dnadb.egg-info/PKG-INFO` & `dnadb-0.2.9/src/dnadb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.2.8
+Version: 0.2.9
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

