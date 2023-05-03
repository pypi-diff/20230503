# Comparing `tmp/dbis-er-diagram-1.0.4.tar.gz` & `tmp/dbis-er-diagram-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbis-er-diagram-1.0.4.tar", last modified: Fri Apr 14 08:19:34 2023, max compression
+gzip compressed data, was "dbis-er-diagram-1.0.5.tar", last modified: Wed May  3 14:36:43 2023, max compression
```

## Comparing `dbis-er-diagram-1.0.4.tar` & `dbis-er-diagram-1.0.5.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-14 08:19:34.764445 dbis-er-diagram-1.0.4/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11357 2023-04-14 08:01:51.000000 dbis-er-diagram-1.0.4/LICENSE
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15713 2023-04-14 08:19:34.764445 dbis-er-diagram-1.0.4/PKG-INFO
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15133 2023-04-14 08:01:51.000000 dbis-er-diagram-1.0.4/README.md
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-14 08:19:34.763445 dbis-er-diagram-1.0.4/dbis_er_diagram.egg-info/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15713 2023-04-14 08:19:34.000000 dbis-er-diagram-1.0.4/dbis_er_diagram.egg-info/PKG-INFO
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      529 2023-04-14 08:19:34.000000 dbis-er-diagram-1.0.4/dbis_er_diagram.egg-info/SOURCES.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        1 2023-04-14 08:19:34.000000 dbis-er-diagram-1.0.4/dbis_er_diagram.egg-info/dependency_links.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       48 2023-04-14 08:19:34.000000 dbis-er-diagram-1.0.4/dbis_er_diagram.egg-info/requires.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       10 2023-04-14 08:19:34.000000 dbis-er-diagram-1.0.4/dbis_er_diagram.egg-info/top_level.txt
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-14 08:19:34.763445 dbis-er-diagram-1.0.4/erdiagram/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      246 2023-04-14 08:01:51.000000 dbis-er-diagram-1.0.4/erdiagram/__init__.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     7697 2023-04-14 08:01:51.000000 dbis-er-diagram-1.0.4/erdiagram/drawing.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    38914 2023-04-14 08:01:51.000000 dbis-er-diagram-1.0.4/erdiagram/er.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    27657 2023-04-14 08:19:15.000000 dbis-er-diagram-1.0.4/erdiagram/grading.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6591 2023-04-14 08:01:51.000000 dbis-er-diagram-1.0.4/erdiagram/merging.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      306 2023-04-14 08:01:51.000000 dbis-er-diagram-1.0.4/erdiagram/node_type.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      881 2023-04-14 08:19:15.000000 dbis-er-diagram-1.0.4/pyproject.toml
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       38 2023-04-14 08:19:34.764445 dbis-er-diagram-1.0.4/setup.cfg
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-14 08:19:34.764445 dbis-er-diagram-1.0.4/tests/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     5117 2023-04-14 08:01:51.000000 dbis-er-diagram-1.0.4/tests/test_adders.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1728 2023-04-14 08:01:51.000000 dbis-er-diagram-1.0.4/tests/test_drawing.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11855 2023-04-14 08:01:51.000000 dbis-er-diagram-1.0.4/tests/test_getters.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1916 2023-04-14 08:15:42.000000 dbis-er-diagram-1.0.4/tests/test_grading_components.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     7118 2023-04-14 08:19:15.000000 dbis-er-diagram-1.0.4/tests/test_grading_diagrams.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1148 2023-04-14 08:01:51.000000 dbis-er-diagram-1.0.4/tests/test_merging.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1035 2023-04-14 08:01:51.000000 dbis-er-diagram-1.0.4/tests/test_other_methods.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-03 14:36:43.581057 dbis-er-diagram-1.0.5/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11357 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/LICENSE
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15713 2023-05-03 14:36:43.581057 dbis-er-diagram-1.0.5/PKG-INFO
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15133 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/README.md
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-03 14:36:43.580057 dbis-er-diagram-1.0.5/dbis_er_diagram.egg-info/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15713 2023-05-03 14:36:43.000000 dbis-er-diagram-1.0.5/dbis_er_diagram.egg-info/PKG-INFO
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      565 2023-05-03 14:36:43.000000 dbis-er-diagram-1.0.5/dbis_er_diagram.egg-info/SOURCES.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        1 2023-05-03 14:36:43.000000 dbis-er-diagram-1.0.5/dbis_er_diagram.egg-info/dependency_links.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       48 2023-05-03 14:36:43.000000 dbis-er-diagram-1.0.5/dbis_er_diagram.egg-info/requires.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       10 2023-05-03 14:36:43.000000 dbis-er-diagram-1.0.5/dbis_er_diagram.egg-info/top_level.txt
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-03 14:36:43.580057 dbis-er-diagram-1.0.5/erdiagram/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      246 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/erdiagram/__init__.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     7697 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/erdiagram/drawing.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    38914 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/erdiagram/er.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    31969 2023-05-03 14:36:33.000000 dbis-er-diagram-1.0.5/erdiagram/grading.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6591 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/erdiagram/merging.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      306 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/erdiagram/node_type.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      881 2023-05-03 14:36:33.000000 dbis-er-diagram-1.0.5/pyproject.toml
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       38 2023-05-03 14:36:43.581057 dbis-er-diagram-1.0.5/setup.cfg
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-03 14:36:43.580057 dbis-er-diagram-1.0.5/tests/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     5117 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/tests/test_adders.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1728 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/tests/test_drawing.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11855 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/tests/test_getters.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1916 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/tests/test_grading_components.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     7118 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/tests/test_grading_diagrams.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3617 2023-05-03 14:36:33.000000 dbis-er-diagram-1.0.5/tests/test_grading_special_cases.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1148 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/tests/test_merging.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1035 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/tests/test_other_methods.py
```

### Comparing `dbis-er-diagram-1.0.4/LICENSE` & `dbis-er-diagram-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.4/PKG-INFO` & `dbis-er-diagram-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-er-diagram
-Version: 1.0.4
+Version: 1.0.5
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: Michal Slupczynski <slupczynski@dbis.rwth-aachen.de>, Beyza Akyüz <beyza.akyuez@rwth-aachen.de>, Til Mohr <til.mohr@rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis/dbis-er-diagram
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-er-diagram-1.0.4/README.md` & `dbis-er-diagram-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.4/dbis_er_diagram.egg-info/PKG-INFO` & `dbis-er-diagram-1.0.5/dbis_er_diagram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-er-diagram
-Version: 1.0.4
+Version: 1.0.5
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: Michal Slupczynski <slupczynski@dbis.rwth-aachen.de>, Beyza Akyüz <beyza.akyuez@rwth-aachen.de>, Til Mohr <til.mohr@rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis/dbis-er-diagram
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-er-diagram-1.0.4/dbis_er_diagram.egg-info/SOURCES.txt` & `dbis-er-diagram-1.0.5/dbis_er_diagram.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,9 +13,10 @@
 erdiagram/merging.py
 erdiagram/node_type.py
 tests/test_adders.py
 tests/test_drawing.py
 tests/test_getters.py
 tests/test_grading_components.py
 tests/test_grading_diagrams.py
+tests/test_grading_special_cases.py
 tests/test_merging.py
 tests/test_other_methods.py
```

### Comparing `dbis-er-diagram-1.0.4/erdiagram/drawing.py` & `dbis-er-diagram-1.0.5/erdiagram/drawing.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.4/erdiagram/er.py` & `dbis-er-diagram-1.0.5/erdiagram/er.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.4/erdiagram/grading.py` & `dbis-er-diagram-1.0.5/erdiagram/grading.py`

 * *Files 21% similar despite different names*

```diff
@@ -206,14 +206,40 @@
         log += f"\t✗ Entity '{solution_label}' not found in submission. ({scores['missing_entity']})\n"
         score += scores["missing_entity"]
 
     return score, log
 
 
 @typechecked
+def __parse_cardinality(s: str) -> int | str | tuple[int | str, int | str]:
+    """
+    Parses a string and returns the corresponding value.
+    """
+    # Remove any whitespace from the string
+    s = s.strip()
+
+    if s.isdigit():
+        # The string represents an integer
+        return int(s)
+    elif s.isalpha():
+        # The string represents a single character string
+        return s
+    elif s.startswith("(") and s.endswith(")"):
+        # The string represents a tuple of two values
+        parts = s[1:-1].split(",")
+        if len(parts) != 2:
+            raise ValueError("String does not represent a tuple of two values.")
+        val1 = parts[0].strip()
+        val2 = parts[1].strip()
+        return (val1, val2)
+    else:
+        raise ValueError("String could not be parsed.")
+
+
+@typechecked
 def _grade_relation_pair(
     relation_pair: tuple[dict[str, Any], dict[str, Any]],
     solution: erdiagram.ER,
     submission: erdiagram.ER,
 ) -> Optional[tuple[float, str]]:
     """
     Grades a pair of relations.
@@ -281,33 +307,76 @@
                         sanitize(solution_to_entity["label"]),
                         sanitize(submission_to_entity["label"]),
                     ),
                 ),
             )
         )
 
+    cardinality_letter_map = dict()
+
     for solution_from_entity, submission_from_entity in from_entity_pairs:
         original_solution_from_entity_label = solution_from_entity["label"]
         original_submission_from_entity_label = submission_from_entity["label"]
         solution_from_entity_label = sanitize(original_solution_from_entity_label)
         submission_from_entity_label = sanitize(original_submission_from_entity_label)
         label_ratio = ratio(solution_from_entity_label, submission_from_entity_label)
         if label_ratio < ratio_threshold:
             score += scores["missing_relation_property"] * 3
             log += f"\t✗ Relation '{original_solution_label}' should have a from entity '{original_solution_from_entity_label}'. ({scores['missing_relation_property'] * 3})\n"
             continue
 
         log += f"\t✓ Relation '{original_solution_label}' has a from entity '{original_solution_from_entity_label}' comparable to '{original_submission_from_entity_label}' with a label ratio of {label_ratio:.2f}.\n"
 
         # check for the same cardinality
-        solution_from_entity_cardinality = solution_from_entity["cardinality"]
-        submission_from_entity_cardinality = submission_from_entity["cardinality"]
-        if str(solution_from_entity_cardinality).replace(" ", "") != str(
-            submission_from_entity_cardinality
-        ).replace(" ", ""):
+        solution_from_entity_cardinality = __parse_cardinality(
+            str(solution_from_entity["cardinality"]).replace(" ", "")
+        )
+        submission_from_entity_cardinality = __parse_cardinality(
+            str(submission_from_entity["cardinality"]).replace(" ", "")
+        )
+
+        # if both are strings
+        if isinstance(solution_from_entity_cardinality, str) and isinstance(
+            submission_from_entity_cardinality, str
+        ):
+            # check if there exists a cardinality letter mapping for the solution cardinality
+            if submission_from_entity_cardinality not in cardinality_letter_map:
+                cardinality_letter_map[
+                    submission_from_entity_cardinality
+                ] = solution_from_entity_cardinality
+
+            submission_from_entity_cardinality = cardinality_letter_map[
+                submission_from_entity_cardinality
+            ]
+
+        # if both a tuples
+        if isinstance(solution_from_entity_cardinality, tuple) and isinstance(
+            submission_from_entity_cardinality, tuple
+        ):
+            # do the above, but for each index
+            assert (
+                len(solution_from_entity_cardinality)
+                == len(submission_from_entity_cardinality)
+                == 2
+            )
+            new_submission_cardinality_tuple = []
+            for index in range(2):
+                if (
+                    submission_from_entity_cardinality[index]
+                    not in cardinality_letter_map
+                ):
+                    cardinality_letter_map[
+                        submission_from_entity_cardinality[index]
+                    ] = solution_from_entity_cardinality[index]
+                new_submission_cardinality_tuple.append(
+                    cardinality_letter_map[submission_from_entity_cardinality[index]]
+                )
+            submission_from_entity_cardinality = tuple(new_submission_cardinality_tuple)
+
+        if solution_from_entity_cardinality != submission_from_entity_cardinality:
             score += scores["missing_relation_property"]
             log += f"\t✗ Relation '{original_solution_label}' should have a from entity '{original_solution_from_entity_label}' with cardinality '{solution_from_entity_cardinality}', but has '{submission_from_entity_cardinality}'. ({scores['missing_relation_property']})\n"
 
         # check for the same is_weak
         solution_from_entity_is_weak = solution_from_entity["is_weak"]
         submission_from_entity_is_weak = submission_from_entity["is_weak"]
         if solution_from_entity_is_weak != submission_from_entity_is_weak:
@@ -324,19 +393,60 @@
             score += scores["missing_relation_property"] * 3
             log += f"\t✗ Relation '{original_solution_label}' should have a to entity '{original_solution_to_entity_label}'. ({scores['missing_relation_property'] * 3})\n"
             continue
 
         log += f"\t✓ Relation '{original_solution_label}' has a to entity '{original_solution_to_entity_label}' comparable to '{original_submission_to_entity_label}' with a label ratio of {label_ratio:.2f}.\n"
 
         # check for the same cardinality
-        solution_to_entity_cardinality = solution_to_entity["cardinality"]
-        submission_to_entity_cardinality = submission_to_entity["cardinality"]
-        if str(solution_to_entity_cardinality).replace(" ", "") != str(
-            submission_to_entity_cardinality
-        ).replace(" ", ""):
+        solution_to_entity_cardinality = __parse_cardinality(
+            str(solution_to_entity["cardinality"]).replace(" ", "")
+        )
+        submission_to_entity_cardinality = __parse_cardinality(
+            str(submission_to_entity["cardinality"]).replace(" ", "")
+        )
+
+        # if both are strings
+        if isinstance(solution_to_entity_cardinality, str) and isinstance(
+            submission_to_entity_cardinality, str
+        ):
+            # check if there exists a cardinality letter mapping for the solution cardinality
+            if submission_to_entity_cardinality not in cardinality_letter_map:
+                cardinality_letter_map[
+                    submission_to_entity_cardinality
+                ] = solution_to_entity_cardinality
+
+            submission_to_entity_cardinality = cardinality_letter_map[
+                submission_to_entity_cardinality
+            ]
+
+        # if both a tuples
+        if isinstance(solution_to_entity_cardinality, tuple) and isinstance(
+            submission_to_entity_cardinality, tuple
+        ):
+            # do the above, but for each index
+            assert (
+                len(solution_to_entity_cardinality)
+                == len(submission_to_entity_cardinality)
+                == 2
+            )
+            new_submission_cardinality_tuple = []
+            for index in range(2):
+                if (
+                    submission_to_entity_cardinality[index]
+                    not in cardinality_letter_map
+                ):
+                    cardinality_letter_map[
+                        submission_to_entity_cardinality[index]
+                    ] = solution_to_entity_cardinality[index]
+                new_submission_cardinality_tuple.append(
+                    cardinality_letter_map[submission_to_entity_cardinality[index]]
+                )
+            submission_to_entity_cardinality = tuple(new_submission_cardinality_tuple)
+
+        if solution_to_entity_cardinality != submission_to_entity_cardinality:
             score += scores["missing_relation_property"]
             log += f"\t✗ Relation '{original_solution_label}' should have a to entity '{original_solution_to_entity_label}' with cardinality '{solution_to_entity_cardinality}', but has '{submission_to_entity_cardinality}'. ({scores['missing_relation_property']})\n"
 
         # check for the same is_weak
         solution_to_entity_is_weak = solution_to_entity["is_weak"]
         submission_to_entity_is_weak = submission_to_entity["is_weak"]
         if solution_to_entity_is_weak != submission_to_entity_is_weak:
@@ -492,18 +602,18 @@
             if label_ratio < ratio_threshold:
                 s = scores["missing_is_a_property"] * label_ratio
                 score += s
                 log += f"\t✗ The is-a relation {solution_super_label} -> {solution_sub_labels} has a custom text with a ratio of {label_ratio:.2f}. ({s})\n"
 
         # check if `is_total` and `is_disjunct` are the same
         if solution_is_a["is_total"] != submission_is_a[0]["is_total"]:
-            log += f"\t✗ The is-a relation {solution_super_label} -> {solution_sub_labels} should{' not' if solution_is_a['is_total'] else ''} be total. ({scores['missing_is_a_property']})\n"
+            log += f"\t✗ The is-a relation {solution_super_label} -> {solution_sub_labels} should{'' if solution_is_a['is_total'] else ' not'} be total. ({scores['missing_is_a_property']})\n"
             score += scores["missing_is_a_property"]
         if solution_is_a["is_disjunct"] != submission_is_a[0]["is_disjunct"]:
-            log += f"\t✗ The is-a relation {solution_super_label} -> {solution_sub_labels} should{' not' if solution_is_a['is_disjunct'] else ''} be disjunct. ({scores['missing_is_a_property']})\n"
+            log += f"\t✗ The is-a relation {solution_super_label} -> {solution_sub_labels} should{'' if solution_is_a['is_disjunct'] else ' not'} be disjunct. ({scores['missing_is_a_property']})\n"
             score += scores["missing_is_a_property"]
 
     return score, log
 
 
 @typechecked
 def _grade_attributes(
@@ -593,21 +703,21 @@
             log += f"\t✗ Attribute {solution_attribute_label} of {str(solution_parent_type).lower()} {solution_parent_label} not found in submission.({s})\n"
             continue
 
         log += f"\t✓ Attribute {solution_attribute_label} of {str(solution_parent_type).lower()} {solution_parent_label} found in submission. (Matched against submission attribute {submission_attribute[0]['label']} of {str(submission_attribute[0]['parent_type']).lower()} {submission.get_label_by_id(submission_attribute[0]['parent_id'])} with ratio {submission_attribute[1]:.2f})\n"
 
         # check if `is_pk`, `is_multiple`, and `is_weak` are the same
         if solution_attribute["is_pk"] != submission_attribute[0]["is_pk"]:
-            log += f"\t✗ The attribute {solution_attribute_label} of {str(solution_parent_type).lower()} {solution_parent_label} should{' not' if solution_attribute['is_pk'] else ''} be a primary key. ({scores['missing_attribute_property']})\n"
+            log += f"\t✗ The attribute {solution_attribute_label} of {str(solution_parent_type).lower()} {solution_parent_label} should{'' if solution_attribute['is_pk'] else ' not'} be a primary key. ({scores['missing_attribute_property']})\n"
             score += scores["missing_attribute_property"]
         if solution_attribute["is_multiple"] != submission_attribute[0]["is_multiple"]:
-            log += f"\t✗ The attribute {solution_attribute_label} of {str(solution_parent_type).lower()} {solution_parent_label} should{' not' if solution_attribute['is_multiple'] else ''} be multiple. ({scores['missing_attribute_property']})\n"
+            log += f"\t✗ The attribute {solution_attribute_label} of {str(solution_parent_type).lower()} {solution_parent_label} should{'' if solution_attribute['is_multiple'] else ' not'} be multiple. ({scores['missing_attribute_property']})\n"
             score += scores["missing_attribute_property"]
         if solution_attribute["is_weak"] != submission_attribute[0]["is_weak"]:
-            log += f"\t✗ The attribute {solution_attribute_label} of {str(solution_parent_type).lower()} {solution_parent_label} should{' not' if solution_attribute['is_weak'] else ''} be weak. ({scores['missing_attribute_property']})\n"
+            log += f"\t✗ The attribute {solution_attribute_label} of {str(solution_parent_type).lower()} {solution_parent_label} should{'' if solution_attribute['is_weak'] else ' not'} be weak. ({scores['missing_attribute_property']})\n"
             score += scores["missing_attribute_property"]
 
         solution_composed_attribute_labels = [
             sanitize(solution.get_label_by_id(composed_attribute_id))
             for composed_attribute_id in solution_attribute["composed_of_attribute_ids"]
         ]
         submission_composed_attribute_labels = [
```

### Comparing `dbis-er-diagram-1.0.4/erdiagram/merging.py` & `dbis-er-diagram-1.0.5/erdiagram/merging.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.4/pyproject.toml` & `dbis-er-diagram-1.0.5/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbis-er-diagram"
-version = "1.0.4"
+version = "1.0.5"
 description = "RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme"
 authors = [
 	{ name = "Michal Slupczynski", email = "slupczynski@dbis.rwth-aachen.de" },
 	{ name = "Beyza Akyüz", email = "beyza.akyuez@rwth-aachen.de" },
 	{ name = "Til Mohr", email = "til.mohr@rwth-aachen.de" },
 ]
 readme = "README.md"
```

### Comparing `dbis-er-diagram-1.0.4/tests/test_adders.py` & `dbis-er-diagram-1.0.5/tests/test_adders.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.4/tests/test_drawing.py` & `dbis-er-diagram-1.0.5/tests/test_drawing.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.4/tests/test_getters.py` & `dbis-er-diagram-1.0.5/tests/test_getters.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.4/tests/test_grading_components.py` & `dbis-er-diagram-1.0.5/tests/test_grading_components.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.4/tests/test_grading_diagrams.py` & `dbis-er-diagram-1.0.5/tests/test_grading_diagrams.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.4/tests/test_merging.py` & `dbis-er-diagram-1.0.5/tests/test_merging.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.4/tests/test_other_methods.py` & `dbis-er-diagram-1.0.5/tests/test_other_methods.py`

 * *Files identical despite different names*

