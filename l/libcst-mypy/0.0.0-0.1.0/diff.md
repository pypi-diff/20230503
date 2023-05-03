# Comparing `tmp/libcst_mypy-0.0.0.tar.gz` & `tmp/libcst_mypy-0.1.0.tar.gz`

## Comparing `libcst_mypy-0.0.0.tar` & `libcst_mypy-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 libcst_mypy-0.0.0/.cruft.json
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 libcst_mypy-0.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 libcst_mypy-0.0.0/requirements.txt
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 libcst_mypy-0.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 libcst_mypy-0.0.0/.github/workflows/main.yml
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 libcst_mypy-0.0.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 libcst_mypy-0.0.0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 libcst_mypy-0.0.0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 libcst_mypy-0.0.0/libcst_mypy/__init__.py
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 libcst_mypy-0.0.0/libcst_mypy/provider.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libcst_mypy-0.0.0/libcst_mypy/py.typed
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 libcst_mypy-0.0.0/libcst_mypy/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libcst_mypy-0.0.0/tests/__init__.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 libcst_mypy-0.0.0/tests/test_inferencer.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 libcst_mypy-0.0.0/tests/data/simple_class.py
--rw-r--r--   0        0        0    13530 2020-02-02 00:00:00.000000 libcst_mypy-0.0.0/tests/data/simples_class.json
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 libcst_mypy-0.0.0/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 libcst_mypy-0.0.0/LICENSE
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 libcst_mypy-0.0.0/README.md
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 libcst_mypy-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 libcst_mypy-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 libcst_mypy-0.1.0/.cruft.json
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 libcst_mypy-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 libcst_mypy-0.1.0/requirements.txt
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 libcst_mypy-0.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 libcst_mypy-0.1.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 libcst_mypy-0.1.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 libcst_mypy-0.1.0/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 libcst_mypy-0.1.0/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 libcst_mypy-0.1.0/libcst_mypy/__init__.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 libcst_mypy-0.1.0/libcst_mypy/provider.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libcst_mypy-0.1.0/libcst_mypy/py.typed
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 libcst_mypy-0.1.0/libcst_mypy/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libcst_mypy-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 libcst_mypy-0.1.0/tests/test_inferencer.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 libcst_mypy-0.1.0/tests/data/simple_class.py
+-rw-r--r--   0        0        0    13530 2020-02-02 00:00:00.000000 libcst_mypy-0.1.0/tests/data/simples_class.json
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 libcst_mypy-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 libcst_mypy-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 libcst_mypy-0.1.0/README.md
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 libcst_mypy-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 libcst_mypy-0.1.0/PKG-INFO
```

### Comparing `libcst_mypy-0.0.0/.cruft.json` & `libcst_mypy-0.1.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `libcst_mypy-0.0.0/.pre-commit-config.yaml` & `libcst_mypy-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `libcst_mypy-0.0.0/.github/workflows/main.yml` & `libcst_mypy-0.1.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `libcst_mypy-0.0.0/.github/workflows/publish.yml` & `libcst_mypy-0.1.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `libcst_mypy-0.0.0/libcst_mypy/provider.py` & `libcst_mypy-0.1.0/libcst_mypy/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,18 +42,18 @@
         options.preserve_asts = True
         options.fine_grained_incremental = True
         options.use_fine_grained_cache = True
         mypy_result = mypy.build.build(targets, options=options)
         cache = {}
         for path in paths:
             module = calculate_module_and_package(str(root_path), path).name
-            mypy_file = mypy_result.graph[module].tree
-            if mypy_file is not None:
+            mypy_file = mypy_result.graph.get(module)
+            if mypy_file is not None and mypy_file.tree is not None:
                 cache[path] = MypyTypeInferenceProviderCache(
-                    module_name=module, mypy_file=mypy_file
+                    module_name=module, mypy_file=mypy_file.tree
                 )
         return cache
 
     def __init__(self, cache: Optional[MypyTypeInferenceProviderCache]) -> None:
         super().__init__(cache)
         self._mypy_node_locations: Dict[CodeRange, "mypy.nodes.Node"] = {}
         if cache is None:
```

### Comparing `libcst_mypy-0.0.0/libcst_mypy/utils.py` & `libcst_mypy-0.1.0/libcst_mypy/utils.py`

 * *Files identical despite different names*

### Comparing `libcst_mypy-0.0.0/tests/test_inferencer.py` & `libcst_mypy-0.1.0/tests/test_inferencer.py`

 * *Files identical despite different names*

### Comparing `libcst_mypy-0.0.0/tests/data/simple_class.py` & `libcst_mypy-0.1.0/tests/data/simple_class.py`

 * *Files identical despite different names*

### Comparing `libcst_mypy-0.0.0/tests/data/simples_class.json` & `libcst_mypy-0.1.0/tests/data/simples_class.json`

 * *Files identical despite different names*

### Comparing `libcst_mypy-0.0.0/.gitignore` & `libcst_mypy-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `libcst_mypy-0.0.0/LICENSE` & `libcst_mypy-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libcst_mypy-0.0.0/README.md` & `libcst_mypy-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `libcst_mypy-0.0.0/pyproject.toml` & `libcst_mypy-0.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = 'hatchling.build'
 
 [project]
 name = "libcst-mypy"
-version = "0.0.0"
+version = "0.1.0"
 description = "Infer types to be used for codemods using mypy! :sparkles:"
 readme = "README.md"
 authors = [{ name = "Marcelo Trylesinski", email = "marcelotryle@email.com" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
```

### Comparing `libcst_mypy-0.0.0/PKG-INFO` & `libcst_mypy-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libcst-mypy
-Version: 0.0.0
+Version: 0.1.0
 Summary: Infer types to be used for codemods using mypy! :sparkles:
 Project-URL: Homepage, https://github.com/Kludex/libcst-mypy
 Project-URL: Source, https://github.com/Kludex/libcst-mypy
 Project-URL: Twitter, https://twitter.com/marcelotryle
 Project-URL: Funding, https://github.com/sponsors/Kludex
 Author-email: Marcelo Trylesinski <marcelotryle@email.com>
 License-Expression: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: libcst-mypy Version: 0.0.0 Summary: Infer types to
+Metadata-Version: 2.1 Name: libcst-mypy Version: 0.1.0 Summary: Infer types to
 be used for codemods using mypy! :sparkles: Project-URL: Homepage, https://
 github.com/Kludex/libcst-mypy Project-URL: Source, https://github.com/Kludex/
 libcst-mypy Project-URL: Twitter, https://twitter.com/marcelotryle Project-URL:
 Funding, https://github.com/sponsors/Kludex Author-email: Marcelo Trylesinski
 email.com> License-Expression: MIT License-File: LICENSE Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
```

