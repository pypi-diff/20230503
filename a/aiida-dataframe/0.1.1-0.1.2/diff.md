# Comparing `tmp/aiida-dataframe-0.1.1.tar.gz` & `tmp/aiida-dataframe-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-dataframe-0.1.1.tar", last modified: Tue Sep 13 08:51:52 2022, max compression
+gzip compressed data, was "aiida-dataframe-0.1.2.tar", last modified: Wed May  3 19:25:06 2023, max compression
```

## Comparing `aiida-dataframe-0.1.1.tar` & `aiida-dataframe-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rwxr-xr-x   0        0        0      195 2022-09-13 08:51:48.827614 aiida-dataframe-0.1.1/.github/install_aiida_github.sh
--rw-r--r--   0        0        0     2232 2022-09-13 08:51:48.827614 aiida-dataframe-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      762 2022-09-13 08:51:48.827614 aiida-dataframe-0.1.1/.github/workflows/publish-on-pypi.yml
--rw-r--r--   0        0        0      121 2022-09-13 08:51:48.827614 aiida-dataframe-0.1.1/.gitignore
--rw-r--r--   0        0        0      774 2022-09-13 08:51:48.827614 aiida-dataframe-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      159 2022-09-13 08:51:48.827614 aiida-dataframe-0.1.1/.readthedocs.yml
--rw-r--r--   0        0        0     1073 2022-09-13 08:51:48.827614 aiida-dataframe-0.1.1/LICENSE
--rw-r--r--   0        0        0     2424 2022-09-13 08:51:48.827614 aiida-dataframe-0.1.1/README.md
--rw-r--r--   0        0        0       95 2022-09-13 08:51:48.831614 aiida-dataframe-0.1.1/aiida_dataframe/__init__.py
--rw-r--r--   0        0        0     2171 2022-09-13 08:51:48.831614 aiida-dataframe-0.1.1/aiida_dataframe/cli.py
--rw-r--r--   0        0        0      182 2022-09-13 08:51:48.831614 aiida-dataframe-0.1.1/aiida_dataframe/data/__init__.py
--rw-r--r--   0        0        0     4562 2022-09-13 08:51:48.831614 aiida-dataframe-0.1.1/aiida_dataframe/data/dataframe.py
--rw-r--r--   0        0        0      322 2022-09-13 08:51:48.831614 aiida-dataframe-0.1.1/conftest.py
--rw-r--r--   0        0        0        7 2022-09-13 08:51:48.831614 aiida-dataframe-0.1.1/docs/.gitignore
--rwxr-xr-x   0        0        0     1554 2022-09-13 08:51:48.831614 aiida-dataframe-0.1.1/docs/Makefile
--rwxr-xr-x   0        0        0     7656 2022-09-13 08:51:48.831614 aiida-dataframe-0.1.1/docs/source/conf.py
--rw-r--r--   0        0        0     3008 2022-09-13 08:51:48.831614 aiida-dataframe-0.1.1/docs/source/developer_guide/index.rst
--rw-r--r--   0        0        0    76300 2022-09-13 08:51:48.831614 aiida-dataframe-0.1.1/docs/source/images/AiiDA_transparent_logo.png
--rwxr-xr-x   0        0        0     1269 2022-09-13 08:51:48.831614 aiida-dataframe-0.1.1/docs/source/index.rst
--rw-r--r--   0        0        0     2176 2022-09-13 08:51:48.831614 aiida-dataframe-0.1.1/docs/source/user_guide/get_started.rst
--rw-r--r--   0        0        0       94 2022-09-13 08:51:48.831614 aiida-dataframe-0.1.1/docs/source/user_guide/index.rst
--rw-r--r--   0        0        0      243 2022-09-13 08:51:48.831614 aiida-dataframe-0.1.1/docs/source/user_guide/tutorial.rst
--rw-r--r--   0        0        0     3325 2022-09-13 08:51:48.831614 aiida-dataframe-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      215 2022-09-13 08:51:48.831614 aiida-dataframe-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     2016 2022-09-13 08:51:48.831614 aiida-dataframe-0.1.1/tests/test_cli.py
--rw-r--r--   0        0        0      143 2022-09-13 08:51:48.831614 aiida-dataframe-0.1.1/tests/test_cli/test_dataframe_export.csv
--rw-r--r--   0        0        0      488 2022-09-13 08:51:48.831614 aiida-dataframe-0.1.1/tests/test_cli/test_dataframe_show.txt
--rw-r--r--   0        0        0    11036 2022-09-13 08:51:48.831614 aiida-dataframe-0.1.1/tests/test_data.py
--rw-r--r--   0        0        0     4220 1970-01-01 00:00:00.000000 aiida-dataframe-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0      195 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/.github/install_aiida_github.sh
+-rw-r--r--   0        0        0     2240 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      762 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/.github/workflows/publish-on-pypi.yml
+-rw-r--r--   0        0        0      121 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/.gitignore
+-rw-r--r--   0        0        0      852 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      159 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/.readthedocs.yml
+-rw-r--r--   0        0        0     1073 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2424 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/README.md
+-rw-r--r--   0        0        0       95 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/aiida_dataframe/__init__.py
+-rw-r--r--   0        0        0     2171 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/aiida_dataframe/cli.py
+-rw-r--r--   0        0        0      182 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/aiida_dataframe/data/__init__.py
+-rw-r--r--   0        0        0     4711 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/aiida_dataframe/data/dataframe.py
+-rw-r--r--   0        0        0      322 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/conftest.py
+-rw-r--r--   0        0        0        7 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/docs/.gitignore
+-rwxr-xr-x   0        0        0     1554 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/docs/Makefile
+-rwxr-xr-x   0        0        0     7656 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/docs/source/conf.py
+-rw-r--r--   0        0        0     3008 2023-05-03 19:24:59.441109 aiida-dataframe-0.1.2/docs/source/developer_guide/index.rst
+-rw-r--r--   0        0        0    76300 2023-05-03 19:24:59.445109 aiida-dataframe-0.1.2/docs/source/images/AiiDA_transparent_logo.png
+-rwxr-xr-x   0        0        0     1269 2023-05-03 19:24:59.445109 aiida-dataframe-0.1.2/docs/source/index.rst
+-rw-r--r--   0        0        0     2326 2023-05-03 19:24:59.445109 aiida-dataframe-0.1.2/docs/source/user_guide/get_started.rst
+-rw-r--r--   0        0        0       94 2023-05-03 19:24:59.445109 aiida-dataframe-0.1.2/docs/source/user_guide/index.rst
+-rw-r--r--   0        0        0      243 2023-05-03 19:24:59.445109 aiida-dataframe-0.1.2/docs/source/user_guide/tutorial.rst
+-rw-r--r--   0        0        0     3371 2023-05-03 19:24:59.445109 aiida-dataframe-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      215 2023-05-03 19:24:59.445109 aiida-dataframe-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     2016 2023-05-03 19:24:59.445109 aiida-dataframe-0.1.2/tests/test_cli.py
+-rw-r--r--   0        0        0      143 2023-05-03 19:24:59.445109 aiida-dataframe-0.1.2/tests/test_cli/test_dataframe_export.csv
+-rw-r--r--   0        0        0      488 2023-05-03 19:24:59.445109 aiida-dataframe-0.1.2/tests/test_cli/test_dataframe_show.txt
+-rw-r--r--   0        0        0    12759 2023-05-03 19:24:59.445109 aiida-dataframe-0.1.2/tests/test_data.py
+-rw-r--r--   0        0        0     4271 1970-01-01 00:00:00.000000 aiida-dataframe-0.1.2/PKG-INFO
```

### Comparing `aiida-dataframe-0.1.1/.github/workflows/ci.yml` & `aiida-dataframe-0.1.2/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 jobs:
 
   tests:
     runs-on: ubuntu-latest
     timeout-minutes: 30
     strategy:
       matrix:
-        python-version: ["3.7","3.8", "3.9", "3.10"] #3.7 will install AiiDA 1.X
+        python-version: ["3.7","3.8", "3.9", "3.10", "3.11"] #3.7 will install AiiDA 1.X
         aiida-version: ["stable"]
       fail-fast: False
 
     services:
       postgres:
         image: postgres:10
         env:
```

### Comparing `aiida-dataframe-0.1.1/.github/workflows/publish-on-pypi.yml` & `aiida-dataframe-0.1.2/.github/workflows/publish-on-pypi.yml`

 * *Files identical despite different names*

### Comparing `aiida-dataframe-0.1.1/.pre-commit-config.yaml` & `aiida-dataframe-0.1.2/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,36 @@
+ci:
+    autoupdate_schedule: monthly
+    autofix_prs: true
+    skip: [pylint]
+
 # Install pre-commit hooks via:
 # pre-commit install
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.1.0
+  rev: v4.4.0
   hooks:
     - id: end-of-file-fixer
     - id: mixed-line-ending
     - id: trailing-whitespace
     - id: check-json
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: v2.31.0
+  rev: v3.3.2
   hooks:
   - id: pyupgrade
     args: ["--py37-plus"]
 
 - repo: https://github.com/PyCQA/isort
-  rev: 5.10.1
+  rev: 5.12.0
   hooks:
     - id: isort
 
 - repo: https://github.com/psf/black
-  rev: 22.3.0
+  rev: 23.3.0
   hooks:
     - id: black
 
 - repo: local
   hooks:
   - id: pylint
     language: system
```

### Comparing `aiida-dataframe-0.1.1/LICENSE` & `aiida-dataframe-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida-dataframe-0.1.1/README.md` & `aiida-dataframe-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `aiida-dataframe-0.1.1/aiida_dataframe/cli.py` & `aiida-dataframe-0.1.2/aiida_dataframe/cli.py`

 * *Files identical despite different names*

### Comparing `aiida-dataframe-0.1.1/aiida_dataframe/data/dataframe.py` & `aiida-dataframe-0.1.2/aiida_dataframe/data/dataframe.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,43 +31,48 @@
     """
 
     DEFAULT_FILENAME = "dataframe.h5"
 
     def __init__(
         self, df: pd.DataFrame, filename: str | None = None, **kwargs: Any
     ) -> None:
-
         if df is None:
             raise TypeError("the `df` argument cannot be `None`.")
 
         if not isinstance(df, pd.DataFrame):
             raise TypeError("the `df` argument is not a pandas DataFrame.")
 
-        super().__init__(None, filename=filename, **kwargs)
+        super().__init__(None, **kwargs)
         self._update_dataframe(df, filename=filename)
         self._df = df
 
     def _update_dataframe(self, df: pd.DataFrame, filename: str | None = None) -> None:
         """
         Update the stored HDF5 file. Raises if the node is already stored
         """
         if self.is_stored:
             raise exceptions.ModificationNotAllowed(
                 "cannot update the DataFrame on a stored node"
             )
+        if filename is None:
+            try:
+                filename = self.filename
+            except AttributeError:
+                filename = self.DEFAULT_FILENAME
 
         with tempfile.TemporaryDirectory() as td:
             df.to_hdf(Path(td) / self.DEFAULT_FILENAME, "w", format="table")
 
             with open(Path(td) / self.DEFAULT_FILENAME, "rb") as file:
                 self.set_file(file, filename=filename)
 
         self.set_attribute("_pandas_data_hash", self._hash_dataframe(df))
         self.set_attribute("index", list(df.index))
         self.set_attribute("columns", list(df.columns.to_flat_index()))
+        self._df = df
 
     @staticmethod
     def _hash_dataframe(df):
         """
         Return a hash corresponding to the Data inside the dataframe (not column names)
         """
         return hashlib.sha256(hash_pandas_object(df, index=True).values).hexdigest()
@@ -123,10 +128,10 @@
         sync the HDF5 storage with the _df attribute on the node
         This catches changes to the node made by using setitem
         on the dataframe e.g. `df["A"] = new_value`
         This is only done if the hashes of the DATA does not match up
         """
         current_hash = self._hash_dataframe(self._df)
         if current_hash != self.get_attribute("_pandas_data_hash"):
-            self._update_dataframe(self._df, filename=self.filename)
+            self._update_dataframe(self._df)
 
         return super().store(*args, **kwargs)
```

### Comparing `aiida-dataframe-0.1.1/docs/Makefile` & `aiida-dataframe-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiida-dataframe-0.1.1/docs/source/conf.py` & `aiida-dataframe-0.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `aiida-dataframe-0.1.1/docs/source/developer_guide/index.rst` & `aiida-dataframe-0.1.2/docs/source/developer_guide/index.rst`

 * *Files identical despite different names*

### Comparing `aiida-dataframe-0.1.1/docs/source/images/AiiDA_transparent_logo.png` & `aiida-dataframe-0.1.2/docs/source/images/AiiDA_transparent_logo.png`

 * *Files identical despite different names*

### Comparing `aiida-dataframe-0.1.1/docs/source/index.rst` & `aiida-dataframe-0.1.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `aiida-dataframe-0.1.1/docs/source/user_guide/get_started.rst` & `aiida-dataframe-0.1.2/docs/source/user_guide/get_started.rst`

 * *Files 8% similar despite different names*

```diff
@@ -49,12 +49,14 @@
    print(df_node.df.head())
 
 .. warning:: Note on Mutability of DataFrame objects
 
     Methods on :py:class:`pandas.DataFrame` objects return a new instance of the
     object and do not mutate the original instance. This means that as soon as the
     :py:class:`~aiida_dataframe.data.dataframe.PandasFrameData` is initialized the associated
-    DataFrame can essentially not be changed, even if the node is not yet stored.
+    DataFrame essentially is fixed. Any operation on the dataframe on the
+    :py:class:`~aiida_dataframe.data.dataframe.PandasFrameData` class will completely overwrite
+    and recreate the associated HDF5 file in it's repository.
 
     Some methods of `pandas` have an `in_place` option to mutate the original. This is
     explicitly not supported if the :py:class:`pandas.DataFrame` is already associated
     with a node the changes will be ignored if you load it from the database
```

### Comparing `aiida-dataframe-0.1.1/pyproject.toml` & `aiida-dataframe-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     "Natural Language :: English",
     'Development Status :: 4 - Beta',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     "Framework :: AiiDA"
 ]
 keywords = ["aiida", "plugin"]
 requires-python = ">=3.7"
 dependencies = [
     "aiida-core>=1.0,<3",
     "pandas",
```

### Comparing `aiida-dataframe-0.1.1/tests/test_cli.py` & `aiida-dataframe-0.1.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `aiida-dataframe-0.1.1/tests/test_data.py` & `aiida-dataframe-0.1.2/tests/test_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -426,7 +426,71 @@
 
     node = PandasFrameData(df)
     node.store()
 
     loaded = load_node(node.pk)
     assert loaded is not node
     assert_frame_equal(loaded.df, df)
+
+
+@pytest.mark.parametrize(
+    "entry_point",
+    ("dataframe.frame",),
+)
+def test_modification_before_instance_update(entry_point):
+    """
+    Test that modifying the dataframe before storing is propagated
+    """
+
+    PandasFrameData = DataFactory(entry_point)
+
+    # Example from pandas Docs
+    df = pd.DataFrame(
+        {
+            "A": 1.0,
+            "B": pd.Timestamp("20130102"),
+            "C": pd.Series(1, index=list(range(4)), dtype="float32"),
+            "D": np.array([3] * 4, dtype="int32"),
+            "E": pd.Categorical(["test", "train", "test", "train"]),
+            "F": "foo",
+        }
+    )
+    df_changed = df.copy(deep=True)
+    df_changed = df_changed.set_index("C")
+
+    node = PandasFrameData(df)
+    node.df = node.df.set_index("C")
+    assert_frame_equal(node.df, df_changed)
+
+
+@pytest.mark.parametrize(
+    "entry_point",
+    ("dataframe.frame",),
+)
+def test_non_default_filename(entry_point):
+    """
+    Test that modifying the dataframe before storing is propagated
+    """
+
+    PandasFrameData = DataFactory(entry_point)
+
+    # Example from pandas Docs
+    df = pd.DataFrame(
+        {
+            "A": 1.0,
+            "B": pd.Timestamp("20130102"),
+            "C": pd.Series(1, index=list(range(4)), dtype="float32"),
+            "D": np.array([3] * 4, dtype="int32"),
+            "E": pd.Categorical(["test", "train", "test", "train"]),
+            "F": "foo",
+        }
+    )
+
+    node = PandasFrameData(df, filename="non_default.h5")
+    node.store()
+
+    assert node.list_object_names() == ["non_default.h5"]
+
+    loaded = load_node(node.pk)
+    assert loaded is not node
+    assert loaded.list_object_names() == ["non_default.h5"]
+    assert_frame_equal(loaded.df, df)
```

### Comparing `aiida-dataframe-0.1.1/PKG-INFO` & `aiida-dataframe-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-dataframe
-Version: 0.1.1
+Version: 0.1.2
 Summary: AiiDA data plugin for pandas DataFrame objects
 Keywords: aiida,plugin
 Author-email: Henning Janßen <henning.janssen@gmx.net>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Science/Research
@@ -12,14 +12,15 @@
 Classifier: Natural Language :: English
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: AiiDA
 Requires-Dist: aiida-core>=1.0,<3
 Requires-Dist: pandas
 Requires-Dist: tables
 Requires-Dist: tabulate
 Requires-Dist: sphinx ; extra == "docs"
 Requires-Dist: sphinxcontrib-contentui ; extra == "docs"
```

