# Comparing `tmp/reasoner-transpiler-2.0.0.tar.gz` & `tmp/reasoner-transpiler-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner-transpiler-2.0.0.tar", last modified: Fri Apr 28 13:36:01 2023, max compression
+gzip compressed data, was "reasoner-transpiler-2.0.1.tar", last modified: Wed May  3 15:00:18 2023, max compression
```

## Comparing `reasoner-transpiler-2.0.0.tar` & `reasoner-transpiler-2.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:36:01.074276 reasoner-transpiler-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-28 13:36:01.074276 reasoner-transpiler-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-28 13:35:57.000000 reasoner-transpiler-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:36:01.070276 reasoner-transpiler-2.0.0/reasoner_transpiler/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-28 13:35:57.000000 reasoner-transpiler-2.0.0/reasoner_transpiler/attribute_types.json
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-04-28 13:35:57.000000 reasoner-transpiler-2.0.0/reasoner_transpiler/cypher.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-28 13:35:57.000000 reasoner-transpiler-2.0.0/reasoner_transpiler/cypher_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    16033 2023-04-28 13:35:57.000000 reasoner-transpiler-2.0.0/reasoner_transpiler/matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-04-28 13:35:57.000000 reasoner-transpiler-2.0.0/reasoner_transpiler/nesting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-28 13:35:57.000000 reasoner-transpiler-2.0.0/reasoner_transpiler/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:36:01.070276 reasoner-transpiler-2.0.0/reasoner_transpiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-28 13:36:01.000000 reasoner-transpiler-2.0.0/reasoner_transpiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-28 13:36:01.000000 reasoner-transpiler-2.0.0/reasoner_transpiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:36:01.000000 reasoner-transpiler-2.0.0/reasoner_transpiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:36:01.000000 reasoner-transpiler-2.0.0/reasoner_transpiler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-28 13:36:01.000000 reasoner-transpiler-2.0.0/reasoner_transpiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-28 13:36:01.000000 reasoner-transpiler-2.0.0/reasoner_transpiler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 13:36:01.074276 reasoner-transpiler-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-28 13:35:57.000000 reasoner-transpiler-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:00:18.667065 reasoner-transpiler-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-03 15:00:18.667065 reasoner-transpiler-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-03 15:00:15.000000 reasoner-transpiler-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:00:18.667065 reasoner-transpiler-2.0.1/reasoner_transpiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 15:00:15.000000 reasoner-transpiler-2.0.1/reasoner_transpiler/attribute_types.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-05-03 15:00:15.000000 reasoner-transpiler-2.0.1/reasoner_transpiler/cypher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-03 15:00:15.000000 reasoner-transpiler-2.0.1/reasoner_transpiler/cypher_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16298 2023-05-03 15:00:15.000000 reasoner-transpiler-2.0.1/reasoner_transpiler/matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-05-03 15:00:15.000000 reasoner-transpiler-2.0.1/reasoner_transpiler/nesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-03 15:00:15.000000 reasoner-transpiler-2.0.1/reasoner_transpiler/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:00:18.667065 reasoner-transpiler-2.0.1/reasoner_transpiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-03 15:00:18.000000 reasoner-transpiler-2.0.1/reasoner_transpiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-03 15:00:18.000000 reasoner-transpiler-2.0.1/reasoner_transpiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:00:18.000000 reasoner-transpiler-2.0.1/reasoner_transpiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:00:18.000000 reasoner-transpiler-2.0.1/reasoner_transpiler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-03 15:00:18.000000 reasoner-transpiler-2.0.1/reasoner_transpiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-03 15:00:18.000000 reasoner-transpiler-2.0.1/reasoner_transpiler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:00:18.667065 reasoner-transpiler-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-03 15:00:15.000000 reasoner-transpiler-2.0.1/setup.py
```

### Comparing `reasoner-transpiler-2.0.0/README.md` & `reasoner-transpiler-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `reasoner-transpiler-2.0.0/reasoner_transpiler/cypher.py` & `reasoner-transpiler-2.0.1/reasoner_transpiler/cypher.py`

 * *Files identical despite different names*

### Comparing `reasoner-transpiler-2.0.0/reasoner_transpiler/cypher_expression.py` & `reasoner-transpiler-2.0.1/reasoner_transpiler/cypher_expression.py`

 * *Files identical despite different names*

### Comparing `reasoner-transpiler-2.0.0/reasoner_transpiler/matching.py` & `reasoner-transpiler-2.0.1/reasoner_transpiler/matching.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,27 +151,34 @@
 
     def __init__(
         self,
         edge_id,
         edge,
         anonymous=False,
         invert=True,
+        primary_ks_required=False,
+        **kwargs
     ):
         """Create an edge reference."""
         edge = dict(edge)  # make shallow copy
         _subject = edge.pop("subject")
         _object = edge.pop("object")
         self.name = edge_id if not anonymous else ""
         self.predicates: List[str] = ensure_list(
             edge.pop("predicates", []) or []
         )
         # "related_to" is equivalent to no predicate
         if self.predicates == ["biolink:related_to"]:
             self.predicates = []
-        self.filters = []
+        if primary_ks_required and not edge.get('_length'):
+            self.filters = [
+                f"`{edge_id}`.`biolink:primary_knowledge_source` IS NOT NULL"
+                ]
+        else:
+            self.filters = []
         self.qualifier_filters = []
         self.label = None  #What goes in the [] on the edge in cypher
         self.length = edge.pop("_length", (1, 1))
         invert = invert and edge.pop("_invert", True)
 
         self.inverse_predicates = []
         self.directed = False # Controls whether there is an arrow on the edge in cypher
@@ -347,15 +354,15 @@
     qedge_id,
     qedge,
     node_references: Dict[str, NodeReference],
     invert=True,
     **kwargs,
 ):
     """Get MATCH clause for edge."""
-    eref = EdgeReference(qedge_id, qedge, invert=invert)
+    eref = EdgeReference(qedge_id, qedge, invert=invert, **kwargs)
     if eref.cypher_invert:
         source_node = node_references[qedge["object"]]
         target_node = node_references[qedge["subject"]]
     else:
         source_node = node_references[qedge["subject"]]
         target_node = node_references[qedge["object"]]
     pattern = f"{source_node}{eref}{target_node}"
```

### Comparing `reasoner-transpiler-2.0.0/reasoner_transpiler/nesting.py` & `reasoner-transpiler-2.0.1/reasoner_transpiler/nesting.py`

 * *Files identical despite different names*

### Comparing `reasoner-transpiler-2.0.0/reasoner_transpiler/util.py` & `reasoner-transpiler-2.0.1/reasoner_transpiler/util.py`

 * *Files identical despite different names*

### Comparing `reasoner-transpiler-2.0.0/setup.py` & `reasoner-transpiler-2.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Setup reasoner-transpiler package."""
 from setuptools import setup
 
 setup(
     name="reasoner-transpiler",
-    version="2.0.0",
+    version="2.0.1",
     author="Patrick Wang",
     author_email="patrick@covar.com",
     maintainer="Yaphet Kebede",
     maintainer_email="kebedey@renci.org",
     url="https://github.com/ranking-agent/reasoner-transpiler",
     description="TRAPI → Cypher transpiler",
     packages=["reasoner_transpiler"],
```

