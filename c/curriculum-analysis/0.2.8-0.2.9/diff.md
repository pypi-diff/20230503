# Comparing `tmp/curriculum_analysis-0.2.8.tar.gz` & `tmp/curriculum_analysis-0.2.9.tar.gz`

## Comparing `curriculum_analysis-0.2.8.tar` & `curriculum_analysis-0.2.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/curriculum_analysis/__init__.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/curriculum_analysis/analysis.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/curriculum_analysis/config.cfg.default
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/curriculum_analysis/corpus.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/curriculum_analysis/csv_exporter.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/curriculum_analysis/js_exporter.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/curriculum_analysis/json_exporter.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/curriculum_analysis/keywords.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/curriculum_analysis/keywords.txt
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/curriculum_analysis/main.py
--rw-r--r--   0        0        0     8806 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/curriculum_analysis/txt_parser.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/curriculum_analysis/html/data.js
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/curriculum_analysis/html/index.html
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/curriculum_analysis/html/index.js
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/curriculum_analysis/html/module.html
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/curriculum_analysis/html/module.js
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/curriculum_analysis/top-level/index.html
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/curriculum_analysis/top-level/index.js
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/curriculum_analysis/top-level/pages.js
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/curriculum_analysis/top-level/style.css
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/LICENCE
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/README.md
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/curriculum_analysis/__init__.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/curriculum_analysis/analysis.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/curriculum_analysis/config.cfg.default
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/curriculum_analysis/corpus.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/curriculum_analysis/csv_exporter.py
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/curriculum_analysis/js_exporter.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/curriculum_analysis/json_exporter.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/curriculum_analysis/keywords.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/curriculum_analysis/keywords.txt
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/curriculum_analysis/main.py
+-rw-r--r--   0        0        0     8806 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/curriculum_analysis/txt_parser.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/curriculum_analysis/html/data.js
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/curriculum_analysis/html/index.html
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/curriculum_analysis/html/index.js
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/curriculum_analysis/html/module.html
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/curriculum_analysis/html/module.js
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/curriculum_analysis/top-level/index.html
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/curriculum_analysis/top-level/index.js
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/curriculum_analysis/top-level/pages.js
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/curriculum_analysis/top-level/style.css
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/LICENCE
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/README.md
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.9/PKG-INFO
```

### Comparing `curriculum_analysis-0.2.8/curriculum_analysis/analysis.py` & `curriculum_analysis-0.2.9/curriculum_analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.8/curriculum_analysis/corpus.py` & `curriculum_analysis-0.2.9/curriculum_analysis/corpus.py`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.8/curriculum_analysis/csv_exporter.py` & `curriculum_analysis-0.2.9/curriculum_analysis/csv_exporter.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,29 +8,29 @@
         self.output_path = output_path / f"{self.file.type}s"
         self.output_path.mkdir(exist_ok=True)
         self.code_header = f"{self.file.type} code"
         self.name_header = f"{self.file.type} full title"
         self.summary_path = self.output_path / 'summary.csv'
 
     def export(self, keywords):
-        with self.summary_path.open('w') as summary_file:
+        with self.summary_path.open('w', encoding='utf8', errors='surrogateescape') as summary_file:
             summary_csv = DictWriter(summary_file, fieldnames=[self.code_header, self.name_header, *keywords])
             summary_csv.writeheader()
             for obj in self.file:
                 analysis = Analysis(obj)
                 analysis.analyse(keywords)
                 summary_record = analysis.summary
                 total_matches = sum(summary_record.values())
                 summary_record[self.code_header] = obj.code
                 summary_record[self.name_header] = obj.full_title
                 summary_csv.writerow(summary_record)
                 if not total_matches:
                     continue
                 detail_path = self.output_path / f"{obj.code}.txt"
-                with detail_path.open('w') as detail_file:
+                with detail_path.open('w', encoding='utf8', errors='surrogateescape') as detail_file:
                     for kw, results in analysis.results.items():
                         if not summary_record[kw]:
                             continue
                         for section, examples in results.items():
                             if not examples:
                                 continue
                             msg = f'found keyword "{kw}" {len(examples)} times in "{section}"'
```

### Comparing `curriculum_analysis-0.2.8/curriculum_analysis/js_exporter.py` & `curriculum_analysis-0.2.9/curriculum_analysis/js_exporter.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         js_string = f"""
         async function loadJSON() {{ 
             return {json_string}; 
         }}
         """
         log.info(f"exporting results as HTML to {self.output_path.absolute()}")
         copy_tree(str(Path(__file__).parent / 'html'), str(self.output_path), update=True)
-        with self.data_path.open('w') as data_script:
+        with self.data_path.open('w', encoding='utf8', errors='surrogateescape') as data_script:
             data_script.write(js_string)
         self.recreate_index()
         log.info(f"See {self.output_path.absolute() / 'index.html'}")
         webbrowser.open(str(self.output_path.absolute() / 'index.html'))    
 
     def recreate_index(self):
         result = []
@@ -55,9 +55,9 @@
         json_string = json.dumps(result)
         js_string = f"""
         async function loadJSON() {{
             return {json_string}
         }}
         """
         copy_tree(str(Path(__file__).parent / 'top-level'), str(self.output_path.parent), update=True)
-        with self.pages_path.open('w') as pages_script:
+        with self.pages_path.open('w', encoding='utf8', errors='surrogateescape') as pages_script:
             pages_script.write(js_string)
```

### Comparing `curriculum_analysis-0.2.8/curriculum_analysis/json_exporter.py` & `curriculum_analysis-0.2.9/curriculum_analysis/json_exporter.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,10 +20,10 @@
             analysis.analyse(keywords)
             record = {
                 "code": obj.code,
                 "title": obj.full_title,
                 "data": analysis.results
             }
             result.append(record)
-        with self.summary_path.open('w') as summary_file:
+        with self.summary_path.open('w', encoding='utf8', errors='surrogateescape') as summary_file:
             json.dump(result, summary_file)
         copy_tree(str(Path(__file__).parent / 'html'), str(self.output_path), update=True)
```

### Comparing `curriculum_analysis-0.2.8/curriculum_analysis/main.py` & `curriculum_analysis-0.2.9/curriculum_analysis/main.py`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.8/curriculum_analysis/txt_parser.py` & `curriculum_analysis-0.2.9/curriculum_analysis/txt_parser.py`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.8/curriculum_analysis/html/index.html` & `curriculum_analysis-0.2.9/curriculum_analysis/html/index.html`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.8/curriculum_analysis/html/index.js` & `curriculum_analysis-0.2.9/curriculum_analysis/html/index.js`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.8/curriculum_analysis/html/module.html` & `curriculum_analysis-0.2.9/curriculum_analysis/html/module.html`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.8/curriculum_analysis/html/module.js` & `curriculum_analysis-0.2.9/curriculum_analysis/html/module.js`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.8/curriculum_analysis/top-level/index.html` & `curriculum_analysis-0.2.9/curriculum_analysis/top-level/index.html`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.8/curriculum_analysis/top-level/style.css` & `curriculum_analysis-0.2.9/curriculum_analysis/top-level/style.css`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.8/LICENCE` & `curriculum_analysis-0.2.9/LICENCE`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.8/README.md` & `curriculum_analysis-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.8/pyproject.toml` & `curriculum_analysis-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   "curriculum_analysis/html/*",
   "curriculum_analysis/top-level/*",
   "**/*.py",
 ]
 
 [project]
 name = "curriculum_analysis"
-version = "0.2.8"
+version = "0.2.9"
 authors = [
   { name="Tom Harrison" },
   { name="Graeme Stuart", email="gstuart@dmu.ac.uk" },
 ]
 description = "A simple tool for analysing DMU module and programme specifications with respect to provided keywords."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `curriculum_analysis-0.2.8/PKG-INFO` & `curriculum_analysis-0.2.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curriculum_analysis
-Version: 0.2.8
+Version: 0.2.9
 Summary: A simple tool for analysing DMU module and programme specifications with respect to provided keywords.
 Project-URL: Homepage, https://github.com/IESD/curriculumAnalysis
 Project-URL: Bug Tracker, https://github.com/IESD/curriculumAnalysis/issues
 Author: Tom Harrison
 Author-email: Graeme Stuart <gstuart@dmu.ac.uk>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
```

