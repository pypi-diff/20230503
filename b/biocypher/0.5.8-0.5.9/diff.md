# Comparing `tmp/biocypher-0.5.8.tar.gz` & `tmp/biocypher-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biocypher-0.5.8.tar", max compression
+gzip compressed data, was "biocypher-0.5.9.tar", max compression
```

## Comparing `biocypher-0.5.8.tar` & `biocypher-0.5.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1065 2023-03-30 20:37:41.854561 biocypher-0.5.8/LICENSE
--rw-r--r--   0        0        0     6253 2023-03-30 20:37:41.854642 biocypher-0.5.8/README.md
--rw-r--r--   0        0        0      900 2023-03-30 20:37:41.854735 biocypher-0.5.8/biocypher/__init__.py
--rw-r--r--   0        0        0     3646 2023-03-30 20:37:41.854838 biocypher-0.5.8/biocypher/_config/__init__.py
--rw-r--r--   0        0        0     2338 2023-03-30 20:37:41.854903 biocypher-0.5.8/biocypher/_config/biocypher_config.yaml
--rw-r--r--   0        0        0      119 2023-03-30 20:37:41.854954 biocypher-0.5.8/biocypher/_config/test_config.yaml
--rw-r--r--   0        0        0     3120 2023-03-31 16:34:16.016334 biocypher-0.5.8/biocypher/_config/test_schema_config.yaml
--rw-r--r--   0        0        0       68 2023-03-31 16:03:12.333903 biocypher-0.5.8/biocypher/_config/test_schema_config_disconnected.yaml
--rw-r--r--   0        0        0     3347 2023-03-31 16:33:52.833258 biocypher-0.5.8/biocypher/_config/test_schema_config_extended.yaml
--rw-r--r--   0        0        0    12699 2023-03-30 20:37:41.855118 biocypher-0.5.8/biocypher/_connect.py
--rw-r--r--   0        0        0    15036 2023-03-31 15:43:16.055100 biocypher-0.5.8/biocypher/_core.py
--rw-r--r--   0        0        0     9077 2023-03-30 20:37:41.855319 biocypher-0.5.8/biocypher/_create.py
--rw-r--r--   0        0        0     2926 2023-03-30 20:37:41.855380 biocypher-0.5.8/biocypher/_logger.py
--rw-r--r--   0        0        0     9352 2023-03-30 20:37:41.855460 biocypher-0.5.8/biocypher/_mapping.py
--rw-r--r--   0        0        0     1662 2023-03-31 17:21:43.809219 biocypher-0.5.8/biocypher/_metadata.py
--rw-r--r--   0        0        0     4586 2023-03-30 20:37:41.855607 biocypher-0.5.8/biocypher/_misc.py
--rw-r--r--   0        0        0    20371 2023-03-31 16:26:51.044725 biocypher-0.5.8/biocypher/_ontology.py
--rw-r--r--   0        0        0    16497 2023-03-30 20:37:41.855962 biocypher-0.5.8/biocypher/_translate.py
--rw-r--r--   0        0        0    63308 2023-03-31 16:52:54.443472 biocypher-0.5.8/biocypher/_write.py
--rw-r--r--   0        0        0     2896 2023-03-31 17:21:43.809179 biocypher-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     7182 1970-01-01 00:00:00.000000 biocypher-0.5.8/setup.py
--rw-r--r--   0        0        0     7583 1970-01-01 00:00:00.000000 biocypher-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-03-30 20:37:41.854561 biocypher-0.5.9/LICENSE
+-rw-r--r--   0        0        0     6253 2023-03-30 20:37:41.854642 biocypher-0.5.9/README.md
+-rw-r--r--   0        0        0      900 2023-03-30 20:37:41.854735 biocypher-0.5.9/biocypher/__init__.py
+-rw-r--r--   0        0        0     3646 2023-03-30 20:37:41.854838 biocypher-0.5.9/biocypher/_config/__init__.py
+-rw-r--r--   0        0        0     2338 2023-03-30 20:37:41.854903 biocypher-0.5.9/biocypher/_config/biocypher_config.yaml
+-rw-r--r--   0        0        0      119 2023-03-30 20:37:41.854954 biocypher-0.5.9/biocypher/_config/test_config.yaml
+-rw-r--r--   0        0        0     3120 2023-03-31 16:34:16.016334 biocypher-0.5.9/biocypher/_config/test_schema_config.yaml
+-rw-r--r--   0        0        0       68 2023-03-31 16:03:12.333903 biocypher-0.5.9/biocypher/_config/test_schema_config_disconnected.yaml
+-rw-r--r--   0        0        0     3347 2023-03-31 16:33:52.833258 biocypher-0.5.9/biocypher/_config/test_schema_config_extended.yaml
+-rw-r--r--   0        0        0    12699 2023-03-30 20:37:41.855118 biocypher-0.5.9/biocypher/_connect.py
+-rw-r--r--   0        0        0    15036 2023-03-31 15:43:16.055100 biocypher-0.5.9/biocypher/_core.py
+-rw-r--r--   0        0        0     9077 2023-03-30 20:37:41.855319 biocypher-0.5.9/biocypher/_create.py
+-rw-r--r--   0        0        0     2926 2023-03-30 20:37:41.855380 biocypher-0.5.9/biocypher/_logger.py
+-rw-r--r--   0        0        0     9352 2023-03-30 20:37:41.855460 biocypher-0.5.9/biocypher/_mapping.py
+-rw-r--r--   0        0        0     1662 2023-03-31 19:07:28.578101 biocypher-0.5.9/biocypher/_metadata.py
+-rw-r--r--   0        0        0     4586 2023-03-30 20:37:41.855607 biocypher-0.5.9/biocypher/_misc.py
+-rw-r--r--   0        0        0    20371 2023-03-31 16:26:51.044725 biocypher-0.5.9/biocypher/_ontology.py
+-rw-r--r--   0        0        0    16497 2023-03-30 20:37:41.855962 biocypher-0.5.9/biocypher/_translate.py
+-rw-r--r--   0        0        0    66219 2023-03-31 19:05:35.690593 biocypher-0.5.9/biocypher/_write.py
+-rw-r--r--   0        0        0     2896 2023-03-31 19:07:28.578040 biocypher-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     7182 1970-01-01 00:00:00.000000 biocypher-0.5.9/setup.py
+-rw-r--r--   0        0        0     7583 1970-01-01 00:00:00.000000 biocypher-0.5.9/PKG-INFO
```

### Comparing `biocypher-0.5.8/LICENSE` & `biocypher-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `biocypher-0.5.8/README.md` & `biocypher-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `biocypher-0.5.8/biocypher/__init__.py` & `biocypher-0.5.9/biocypher/__init__.py`

 * *Files identical despite different names*

### Comparing `biocypher-0.5.8/biocypher/_config/__init__.py` & `biocypher-0.5.9/biocypher/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `biocypher-0.5.8/biocypher/_config/biocypher_config.yaml` & `biocypher-0.5.9/biocypher/_config/biocypher_config.yaml`

 * *Files identical despite different names*

### Comparing `biocypher-0.5.8/biocypher/_config/test_schema_config.yaml` & `biocypher-0.5.9/biocypher/_config/test_schema_config.yaml`

 * *Files identical despite different names*

### Comparing `biocypher-0.5.8/biocypher/_config/test_schema_config_extended.yaml` & `biocypher-0.5.9/biocypher/_config/test_schema_config_extended.yaml`

 * *Files identical despite different names*

### Comparing `biocypher-0.5.8/biocypher/_connect.py` & `biocypher-0.5.9/biocypher/_connect.py`

 * *Files identical despite different names*

### Comparing `biocypher-0.5.8/biocypher/_core.py` & `biocypher-0.5.9/biocypher/_core.py`

 * *Files identical despite different names*

### Comparing `biocypher-0.5.8/biocypher/_create.py` & `biocypher-0.5.9/biocypher/_create.py`

 * *Files identical despite different names*

### Comparing `biocypher-0.5.8/biocypher/_logger.py` & `biocypher-0.5.9/biocypher/_logger.py`

 * *Files identical despite different names*

### Comparing `biocypher-0.5.8/biocypher/_mapping.py` & `biocypher-0.5.9/biocypher/_mapping.py`

 * *Files identical despite different names*

### Comparing `biocypher-0.5.8/biocypher/_metadata.py` & `biocypher-0.5.9/biocypher/_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import os
 import pathlib
 import importlib.metadata
 
 import toml
 
-_VERSION = '0.5.8'
+_VERSION = '0.5.9'
 
 
 def get_metadata():
     """
     Basic package metadata.
 
     Retrieves package metadata from the current project directory or from
```

### Comparing `biocypher-0.5.8/biocypher/_misc.py` & `biocypher-0.5.9/biocypher/_misc.py`

 * *Files identical despite different names*

### Comparing `biocypher-0.5.8/biocypher/_ontology.py` & `biocypher-0.5.9/biocypher/_ontology.py`

 * *Files identical despite different names*

### Comparing `biocypher-0.5.8/biocypher/_translate.py` & `biocypher-0.5.9/biocypher/_translate.py`

 * *Files identical despite different names*

### Comparing `biocypher-0.5.8/biocypher/_write.py` & `biocypher-0.5.9/biocypher/_write.py`

 * *Files 4% similar despite different names*

```diff
@@ -272,14 +272,23 @@
 
     @property
     def outdir(self):
         """
         Property for output directory path.
         """
 
+        return self._outdir
+
+
+    @property
+    def import_call_file_prefix(self):
+        """
+        Property for output directory path.
+        """
+
         if self._import_call_file_prefix is None:
             return self._outdir
         else:
             return self._import_call_file_prefix
 
     def _process_delimiter(self, delimiter: str) -> str:
         """
@@ -956,27 +965,30 @@
             )
 
         # write to file
         padded_part = str(next_part).zfill(3)
         logger.info(
             f'Writing {len(lines)} entries to {label_pascal}-part{padded_part}.csv',
         )
+
+        # store name only in case import_call_file_prefix is set
+        part = f'{label_pascal}-part{padded_part}.csv'
         file_path = os.path.join(
-            self.outdir, f'{label_pascal}-part{padded_part}.csv'
+            self.outdir, part
         )
 
         with open(file_path, 'w', encoding='utf-8') as f:
 
             # concatenate with delimiter
             f.writelines(lines)
 
         if not self.parts.get(label):
-            self.parts[label] = [file_path]
+            self.parts[label] = [part]
         else:
-            self.parts[label].append(file_path)
+            self.parts[label].append(part)
 
     def get_import_call(self) -> str:
         """
         Function to return the import call detailing folder and
         individual node and edge headers and data files, as well as
         delimiters and database name.
 
@@ -1090,19 +1102,20 @@
         for label, props in self.node_property_dict.items():
 
             _id = ':ID'
 
             # translate label to PascalCase
             pascal_label = self.translator.name_sentence_to_pascal(label)
 
+            header = f'{pascal_label}-header.csv'
             header_path = os.path.join(
                 self.outdir,
-                f'{pascal_label}-header.csv',
+                header,
             )
-            parts_path = os.path.join(self.outdir, f'{pascal_label}-part.*')
+            parts = f'{pascal_label}-part.*'
 
             # check if file already exists
             if os.path.exists(header_path):
                 logger.warning(
                     f'Header file `{header_path}` already exists. Overwriting.',
                 )
 
@@ -1126,16 +1139,25 @@
             out_list = [val for sublist in out_list for val in sublist]
 
             with open(header_path, 'w', encoding='utf-8') as f:
                 # concatenate with delimiter
                 row = self.delim.join(out_list)
                 f.write(row)
 
-            # add file path to neo4 admin import statement
-            self.import_call_nodes.add((header_path, parts_path))
+            # add file path to neo4 admin import statement (import call file
+            # path may be different from actual file path)
+            import_call_header_path = os.path.join(
+                self.import_call_file_prefix,
+                header,
+            )
+            import_call_parts_path = os.path.join(
+                self.import_call_file_prefix,
+                parts,
+            )
+            self.import_call_nodes.add((import_call_header_path, import_call_parts_path))
 
         return True
 
     def _write_edge_headers(self):
         """
         Writes single CSV file for a graph entity that is represented
         as an edge as per the definition in the `schema_config.yaml`,
@@ -1153,19 +1175,20 @@
 
         for label, props in self.edge_property_dict.items():
 
             # translate label to PascalCase
             pascal_label = self.translator.name_sentence_to_pascal(label)
 
             # paths
+            header = f'{pascal_label}-header.csv'
             header_path = os.path.join(
                 self.outdir,
-                f'{pascal_label}-header.csv',
+                header,
             )
-            parts_path = os.path.join(self.outdir, f'{pascal_label}-part.*')
+            parts = f'{pascal_label}-part.*'
 
             # check for file exists
             if os.path.exists(header_path):
                 logger.warning(
                     f'File {header_path} already exists. Overwriting.'
                 )
 
@@ -1187,16 +1210,25 @@
             out_list = [':START_ID', *props_list, ':END_ID', ':TYPE']
 
             with open(header_path, 'w', encoding='utf-8') as f:
                 # concatenate with delimiter
                 row = self.delim.join(out_list)
                 f.write(row)
 
-            # add file path to neo4 admin import statement
-            self.import_call_edges.add((header_path, parts_path))
+            # add file path to neo4 admin import statement (import call file
+            # path may be different from actual file path)
+            import_call_header_path = os.path.join(
+                self.import_call_file_prefix,
+                header,
+            )
+            import_call_parts_path = os.path.join(
+                self.import_call_file_prefix,
+                parts,
+            )
+            self.import_call_edges.add((import_call_header_path, import_call_parts_path))
 
         return True
 
     def _get_import_script_name(self) -> str:
         """
         Returns the name of the neo4j admin import script
 
@@ -1289,17 +1321,18 @@
             # create header CSV with ID, properties, labels
 
             _id = '_key'
 
             # translate label to PascalCase
             pascal_label = self.translator.name_sentence_to_pascal(label)
 
+            header = f'{pascal_label}-header.csv'
             header_path = os.path.join(
                 self.outdir,
-                f'{pascal_label}-header.csv',
+                header,
             )
 
             # check if file already exists
             if os.path.exists(header_path):
                 logger.warning(
                     f'File {header_path} already exists. Overwriting.'
                 )
@@ -1333,16 +1366,25 @@
 
                 raise ValueError(
                     f'No parts found for node label {label}. '
                     f'Check that the data was parsed first.',
                 )
 
             for part in parts:
+                
+                import_call_header_path = os.path.join(
+                    self.import_call_file_prefix,
+                    header,
+                )
+                import_call_parts_path = os.path.join(
+                    self.import_call_file_prefix,
+                    part,
+                )
 
-                self.import_call_nodes.add((header_path, part, collection))
+                self.import_call_nodes.add((import_call_header_path, import_call_parts_path, collection))
 
         return True
 
     def _write_edge_headers(self):
         """
         Writes single CSV file for a graph entity that is represented
         as an edge as per the definition in the `schema_config.yaml`,
@@ -1360,19 +1402,20 @@
 
         for label, props in self.edge_property_dict.items():
 
             # translate label to PascalCase
             pascal_label = self.translator.name_sentence_to_pascal(label)
 
             # paths
+            header = f'{pascal_label}-header.csv'
             header_path = os.path.join(
                 self.outdir,
-                f'{pascal_label}-header.csv',
+                header,
             )
-            parts_path = os.path.join(self.outdir, f'{pascal_label}-part.*')
+            parts = f'{pascal_label}-part.*'
 
             # check for file exists
             if os.path.exists(header_path):
                 logger.warning(
                     f'Header file {header_path} already exists. Overwriting.'
                 )
 
@@ -1399,16 +1442,25 @@
 
             else:
 
                 collection = self.extended_schema[label].get(
                     'db_collection_name', None
                 )
 
-            # add file path to neo4 admin import statement
-            self.import_call_edges.add((header_path, parts_path, collection))
+            # add file path to neo4 admin import statement (import call path
+            # may be different from actual output path)
+            header_import_call_path = os.path.join(
+                self.import_call_file_prefix,
+                header,
+            )
+            parts_import_call_path = os.path.join(
+                self.import_call_file_prefix,
+                parts,
+            )
+            self.import_call_edges.add((header_import_call_path, parts_import_call_path, collection,))
 
         return True
 
     def _construct_import_call(self) -> str:
         """
         Function to construct the import call detailing folder and
         individual node and edge headers and data files, as well as
@@ -1549,23 +1601,19 @@
                 'Header information not found. Was the data parsed first?',
             )
             return False
 
         for label, props in self.node_property_dict.items():
             # create header CSV with ID, properties, labels
 
-            # to programmatically define properties to be written, the
-            # data would have to be parsed before writing the header.
-            # alternatively, desired properties can also be provided
-            # via the schema_config.yaml.
-
             # translate label to PascalCase
             pascal_label = self.translator.name_sentence_to_pascal(label)
 
-            parts_paths = os.path.join(self.outdir, f'{pascal_label}-part*.csv')
+            parts = f'{pascal_label}-part*.csv'
+            parts_paths = os.path.join(self.outdir, parts)
             parts_paths = glob.glob(parts_paths)
             parts_paths.sort()
 
             # adjust label for import to psql
             pascal_label = self._adjust_pascal_to_psql(pascal_label)
             table_create_command_path = os.path.join(
                 self.outdir,
@@ -1593,19 +1641,36 @@
                     command += f'DROP TABLE IF EXISTS {pascal_label};\n'
 
                 # table creation requires comma separation
                 command += f'CREATE TABLE {pascal_label}({",".join(columns)});\n'
                 f.write(command)
 
                 for parts_path in parts_paths:
+                    
+                    # if import_call_file_prefix is set, replace actual path 
+                    # with prefix
+                    if self.import_call_file_prefix != self.outdir:
+                        parts_path = parts_path.replace(
+                            self.outdir,
+                            self.import_call_file_prefix,
+                        )
+
                     self._copy_from_csv_commands.add(
                         f'\\copy {pascal_label} FROM \'{parts_path}\' DELIMITER E\'{self.delim}\' CSV;'
                     )
 
             # add file path to import statement
+            # if import_call_file_prefix is set, replace actual path
+            # with prefix
+            if self.import_call_file_prefix != self.outdir:
+                table_create_command_path = table_create_command_path.replace(
+                    self.outdir,
+                    self.import_call_file_prefix,
+                )
+
             self.import_call_nodes.add(table_create_command_path)
 
         return True
 
     def _write_edge_headers(self):
         """
         Writes single CSV file for a graph entity that is represented
@@ -1664,19 +1729,36 @@
                     command += f'DROP TABLE IF EXISTS {pascal_label};\n'
 
                 # table creation requires comma separation
                 command += f'CREATE TABLE {pascal_label}({",".join(out_list)});\n'
                 f.write(command)
 
                 for parts_path in parts_paths:
+
+                    # if import_call_file_prefix is set, replace actual path
+                    # with prefix
+                    if self.import_call_file_prefix != self.outdir:
+                        parts_path = parts_path.replace(
+                            self.outdir,
+                            self.import_call_file_prefix,
+                        )
+
                     self._copy_from_csv_commands.add(
                         f'\\copy {pascal_label} FROM \'{parts_path}\' DELIMITER E\'{self.delim}\' CSV;'
                     )
 
             # add file path to import statement
+            # if import_call_file_prefix is set, replace actual path
+            # with prefix
+            if self.import_call_file_prefix != self.outdir:
+                table_create_command_path = table_create_command_path.replace(
+                    self.outdir,
+                    self.import_call_file_prefix,
+                )
+                
             self.import_call_edges.add(table_create_command_path)
 
         return True
 
     def _construct_import_call(self) -> str:
         """
         Function to construct the import call detailing folder and
```

### Comparing `biocypher-0.5.8/pyproject.toml` & `biocypher-0.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "biocypher"
-version = "0.5.8"
+version = "0.5.9"
 description = "A unifying framework for biomedical research knowledge graphs"
 authors = [
     "Sebastian Lobentanzer <sebastian.lobentanzer@gmail.com>",
     "Denes Turei <turei.denes@gmail.com>"
 ]
 license = "MIT"
 packages = [
```

### Comparing `biocypher-0.5.8/setup.py` & `biocypher-0.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'networkx>=3.0,<4.0',
  'rdflib>=6.2.0,<7.0.0',
  'stringcase>=1.2.0,<2.0.0',
  'treelib>=1.6.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'biocypher',
-    'version': '0.5.8',
+    'version': '0.5.9',
     'description': 'A unifying framework for biomedical research knowledge graphs',
     'long_description': '# BioCypher\n\n## 📖 Documentation\nTutorial and developer docs at https://biocypher.org. For a quickstart into your\nown pipeline, you can refer to our [project\ntemplate](https://github.com/biocypher/project-template), and for an\noverview of existing and planned adapters for resources and outputs, as well\nas other features, visit our [GitHub Project\nBoard](https://github.com/orgs/biocypher/projects/3/views/2).\n\n## ❓ Description\nThis is the development repository for BioCypher, our proposal for a unifying\nframework to create knowledge graph databases for systems biomedicine. For an\noverview, usage notes, and a tutorial, read the docs\n[here](https://biocypher.org).\n\n<img\n    style="display: block;\n           margin-left: auto;\n           margin-right: auto;\n           width: 70%;"\n    src="graphical_abstract.png"\n    alt="Graphical Abstract">\n</img>\n\n## ⚙️ Usage\nBioCypher is currently in prototype stage. Installation instructions can be\nfound [here](https://biocypher.org/installation.html).\n\nExemplary usage of BioCypher to build a graph database is shown in various\npipelines we have created. You can find these on the [Components Project\nBoard](https://github.com/orgs/biocypher/projects/3/views/2).\n\n## 🤝 Getting involved\nWe are very happy about contributions from the community, large and small!\nIf you would like to contribute to BioCypher development, please refer to\nour [contribution guidelines](CONTRIBUTING.md). :)\n\nIf you want to ask informal questions, talk about dev things, or just chat, please join our community at https://biocypher.zulipchat.com!\n\n> **Imposter syndrome disclaimer:** We want your help. No, really. There may be a little voice inside your head that is telling you that you\'re not ready, that you aren\'t skilled enough to contribute. We assure you that the little voice in your head is wrong. Most importantly, there are many valuable ways to contribute besides writing code.\n>\n> This disclaimer was adapted from the [Pooch](https://github.com/fatiando/pooch) project.\n\n## ✍️ Citation\nThe BioCypher paper is available as a preprint at https://arxiv.org/abs/2212.13543.\n\n## Acknowledgements\nThis project has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement No 965193 for DECIDER and No 116030 for TransQST.\n\n[![Powered by the Bioregistry](https://img.shields.io/static/v1?label=Powered%20by&message=Bioregistry&color=BA274A&style=flat&logo=image/png;base64,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)](https://github.com/biopragmatics/bioregistry) [![Downloads](https://static.pepy.tech/badge/biocypher)](https://pepy.tech/project/biocypher)\n',
     'author': 'Sebastian Lobentanzer',
     'author_email': 'sebastian.lobentanzer@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/biocypher/biocypher',
```

### Comparing `biocypher-0.5.8/PKG-INFO` & `biocypher-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biocypher
-Version: 0.5.8
+Version: 0.5.9
 Summary: A unifying framework for biomedical research knowledge graphs
 Home-page: https://github.com/biocypher/biocypher
 License: MIT
 Author: Sebastian Lobentanzer
 Author-email: sebastian.lobentanzer@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

