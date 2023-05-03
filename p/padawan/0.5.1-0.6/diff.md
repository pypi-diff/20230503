# Comparing `tmp/padawan-0.5.1.tar.gz` & `tmp/padawan-0.6.tar.gz`

## Comparing `padawan-0.5.1.tar` & `padawan-0.6.tar`

### file list

```diff
@@ -1,41 +1,43 @@
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 padawan-0.5.1/.readthedocs.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 padawan-0.5.1/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 padawan-0.5.1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 padawan-0.5.1/.pytest_cache/README.md
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 padawan-0.5.1/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 padawan-0.5.1/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 padawan-0.5.1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 padawan-0.5.1/docs/Makefile
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 padawan-0.5.1/docs/api.rst
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 padawan-0.5.1/docs/conf.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 padawan-0.5.1/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 padawan-0.5.1/docs/make.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 padawan-0.5.1/docs/requirements.txt
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/__init__.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/collated_dataset.py
--rw-r--r--   0        0        0    16594 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/dataset.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/joined_dataset.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/json_io.py
--rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/mapped_dataset.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/metadata.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/ordering.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/parallelize.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/persisted_dataset.py
--rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/reindexed_dataset.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/renamed_dataset.py
--rw-r--r--   0        0        0     8309 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/repartitioned_dataset.py
--rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 padawan-0.5.1/src/padawan/sliced_dataset.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 padawan-0.5.1/tests/fixtures.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 padawan-0.5.1/tests/test_collate.py
--rw-r--r--   0        0        0     7636 2020-02-02 00:00:00.000000 padawan-0.5.1/tests/test_io.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 padawan-0.5.1/tests/test_join.py
--rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 padawan-0.5.1/tests/test_map.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 padawan-0.5.1/tests/test_rename.py
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 padawan-0.5.1/tests/test_repartition.py
--rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 padawan-0.5.1/tests/test_slice.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 padawan-0.5.1/tests/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 padawan-0.5.1/.gitignore
--rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 padawan-0.5.1/LICENSE
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 padawan-0.5.1/README.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 padawan-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 padawan-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 padawan-0.6/.readthedocs.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 padawan-0.6/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 padawan-0.6/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 padawan-0.6/.pytest_cache/README.md
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 padawan-0.6/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 padawan-0.6/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 padawan-0.6/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 padawan-0.6/docs/Makefile
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 padawan-0.6/docs/api.rst
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 padawan-0.6/docs/conf.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 padawan-0.6/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 padawan-0.6/docs/make.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 padawan-0.6/docs/requirements.txt
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/__init__.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/collated_dataset.py
+-rw-r--r--   0        0        0    16594 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/dataset.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/in_memory_dataset.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/joined_dataset.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/json_io.py
+-rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/mapped_dataset.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/metadata.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/ordering.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/parallelize.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/persisted_dataset.py
+-rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/reindexed_dataset.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/renamed_dataset.py
+-rw-r--r--   0        0        0     8309 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/repartitioned_dataset.py
+-rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/sliced_dataset.py
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 padawan-0.6/tests/fixtures.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 padawan-0.6/tests/test_collate.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 padawan-0.6/tests/test_from_polars.py
+-rw-r--r--   0        0        0     7636 2020-02-02 00:00:00.000000 padawan-0.6/tests/test_io.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 padawan-0.6/tests/test_join.py
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 padawan-0.6/tests/test_map.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 padawan-0.6/tests/test_rename.py
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 padawan-0.6/tests/test_repartition.py
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 padawan-0.6/tests/test_slice.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 padawan-0.6/tests/utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 padawan-0.6/.gitignore
+-rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 padawan-0.6/LICENSE
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 padawan-0.6/README.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 padawan-0.6/pyproject.toml
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 padawan-0.6/PKG-INFO
```

### Comparing `padawan-0.5.1/.pytest_cache/v/cache/nodeids` & `padawan-0.6/.pytest_cache/v/cache/nodeids`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9682539682539683%*

 * *Differences: {'insert': "[(2, 'tests/test_from_polars.py::test__from_polars__with_index_columns'), (3, "*

 * *           "'tests/test_from_polars.py::test__from_polars__without_index_columns')]"}*

```diff
@@ -1,10 +1,12 @@
 [
     "tests/test_collate.py::test__collate__parallel",
     "tests/test_collate.py::test__collate__sequential",
+    "tests/test_from_polars.py::test__from_polars__with_index_columns",
+    "tests/test_from_polars.py::test__from_polars__without_index_columns",
     "tests/test_io.py::test__collect__parallel",
     "tests/test_io.py::test__collect__sequential",
     "tests/test_io.py::test__collect_stats__no_index_cols",
     "tests/test_io.py::test__collect_stats__parallel",
     "tests/test_io.py::test__collect_stats__sequential",
     "tests/test_io.py::test__iter",
     "tests/test_io.py::test__reindex__no_index_cols",
```

### Comparing `padawan-0.5.1/docs/Makefile` & `padawan-0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `padawan-0.5.1/docs/conf.py` & `padawan-0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5.1/docs/index.rst` & `padawan-0.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `padawan-0.5.1/docs/make.bat` & `padawan-0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `padawan-0.5.1/src/padawan/collated_dataset.py` & `padawan-0.6/src/padawan/collated_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5.1/src/padawan/dataset.py` & `padawan-0.6/src/padawan/dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5.1/src/padawan/joined_dataset.py` & `padawan-0.6/src/padawan/joined_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5.1/src/padawan/json_io.py` & `padawan-0.6/src/padawan/json_io.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5.1/src/padawan/mapped_dataset.py` & `padawan-0.6/src/padawan/mapped_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5.1/src/padawan/metadata.py` & `padawan-0.6/src/padawan/metadata.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5.1/src/padawan/ordering.py` & `padawan-0.6/src/padawan/ordering.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5.1/src/padawan/parallelize.py` & `padawan-0.6/src/padawan/parallelize.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5.1/src/padawan/persisted_dataset.py` & `padawan-0.6/src/padawan/persisted_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5.1/src/padawan/reindexed_dataset.py` & `padawan-0.6/src/padawan/reindexed_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         collect_stats=True,
         parallel=False,
         progress=False,
 ):
     """Set index columns and compute partition sizes and bounds.
 
     Args:
-      index_columns (tuple of str, optional): The columns to used as index.
+      index_columns (tuple of str, optional): The columns to use as index.
         Defaults to ``None``, in which case partition sizes and bounds are
         computed for the current index columns.
 
         If `index_columns` is a truncation of the current index
         columns (e.g. ``self.index_columns`` is ``('a', 'b', 'c')`` and
         `index_columns` is ``('a', 'b')``) the new partition bounds can and
         will be computed purely from the metadata and without loading any
```

### Comparing `padawan-0.5.1/src/padawan/renamed_dataset.py` & `padawan-0.6/src/padawan/renamed_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5.1/src/padawan/repartitioned_dataset.py` & `padawan-0.6/src/padawan/repartitioned_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5.1/src/padawan/sliced_dataset.py` & `padawan-0.6/src/padawan/sliced_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5.1/tests/fixtures.py` & `padawan-0.6/tests/fixtures.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 @pytest.fixture
 def datetime_sample():
     t0 = datetime(2022, 1, 1)
     t1 = datetime(2022, 1, 5)
     dt = timedelta(hours=1)
-    t = pl.date_range(t0, t1, dt, name='t', closed='left')
+    t = pl.date_range(t0, t1, dt, name='t', closed='left', eager=True)
     day = t.dt.truncate('1d').cast(pl.Date).alias('date')
     hour = (t - day).alias('hour')
     a = pl.Series('a', np.arange(len(t)))
     df = pl.DataFrame([t, day, hour, a])
 
     null_df = pl.DataFrame([
         pl.Series('t', [None, None], pl.Datetime),
@@ -77,15 +77,15 @@
 
 
 @pytest.fixture
 def date_sample():
     t0 = datetime(2022, 1, 2)
     t1 = datetime(2022, 1, 6)
     dt = timedelta(days=1)
-    t = pl.date_range(t0, t1, dt, name='t', closed='left')
+    t = pl.date_range(t0, t1, dt, name='t', closed='left', eager=True)
     day = t.dt.truncate('1d').cast(pl.Date).alias('date')
     x = pl.Series('x', np.arange(len(day)))
     df = pl.DataFrame([day, x])
 
 
     divisions = [0, 2, 4]
```

### Comparing `padawan-0.5.1/tests/test_collate.py` & `padawan-0.6/tests/test_collate.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5.1/tests/test_io.py` & `padawan-0.6/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5.1/tests/test_join.py` & `padawan-0.6/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5.1/tests/test_map.py` & `padawan-0.6/tests/test_map.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 )
 
 
 def test__map__preserves_none(datetime_sample):
     ds = (
         padawan.scan_parquet(datetime_sample['path'])
         .reindex(['date', 'hour', 't'])
-        .map(lambda df: df.with_column((2*pl.col('a')).alias('b')))
+        .map(lambda df: df.with_columns((2*pl.col('a')).alias('b')))
     )
     assert ds.known_sizes is False
     assert ds.known_bounds is False
 
     df = ds.collect()
     b = df.get_column('b').to_numpy()
     a = datetime_sample['data'].get_column('a').to_numpy()
@@ -25,15 +25,15 @@
 
 
 def test__map__preserves_bounds(datetime_sample):
     ds = (
         padawan.scan_parquet(datetime_sample['path'])
         .reindex(['date', 'hour', 't'])
         .map(
-            lambda df: df.with_column((2*pl.col('a')).alias('b')),
+            lambda df: df.with_columns((2*pl.col('a')).alias('b')),
             preserves='bounds',
         )
     )
     assert ds.known_sizes is False
     assert ds.known_bounds is True
     assert ds.lower_bounds == datetime_sample['lower_bounds']
     assert ds.upper_bounds == datetime_sample['upper_bounds']
@@ -45,15 +45,15 @@
 
 
 def test__map__preserves_sizes(datetime_sample):
     ds = (
         padawan.scan_parquet(datetime_sample['path'])
         .reindex(['date', 'hour', 't'])
         .map(
-            lambda df: df.with_column((2*pl.col('a')).alias('b')),
+            lambda df: df.with_columns((2*pl.col('a')).alias('b')),
             preserves='sizes',
         )
     )
     assert ds.known_sizes is True
     assert ds.sizes == datetime_sample['sizes']
     assert ds.known_bounds is False
 
@@ -64,15 +64,15 @@
 
 
 def test__map__preserves_all(datetime_sample):
     ds = (
         padawan.scan_parquet(datetime_sample['path'])
         .reindex(['date', 'hour', 't'])
         .map(
-            lambda df: df.with_column((2*pl.col('a')).alias('b')),
+            lambda df: df.with_columns((2*pl.col('a')).alias('b')),
             preserves='all',
         )
     )
     assert ds.known_sizes is True
     assert ds.sizes == datetime_sample['sizes']
     assert ds.known_bounds is True
     assert ds.lower_bounds == datetime_sample['lower_bounds']
@@ -82,15 +82,15 @@
     b = df.get_column('b').to_numpy()
     a = datetime_sample['data'].get_column('a').to_numpy()
     assert np.all(b == 2*a)
 
 
 def test__map__sequential_with_args(datetime_sample):
     def f(df, alpha, beta):
-        return df.with_column((alpha*pl.col('a') + beta).alias('b'))
+        return df.with_columns((alpha*pl.col('a') + beta).alias('b'))
 
     ds = (
         padawan.scan_parquet(datetime_sample['path'])
         .reindex(['date', 'hour', 't'])
         .map(
             f,
             shared_args=[2, 3],
@@ -107,15 +107,15 @@
     b = df.get_column('b').to_numpy()
     a = datetime_sample['data'].get_column('a').to_numpy()
     assert np.all(b == 2*a + 3)
 
 
 def test__map__parallel_with_args(datetime_sample):
     def f(df, alpha, beta):
-        return df.with_column((alpha*pl.col('a') + beta).alias('b'))
+        return df.with_columns((alpha*pl.col('a') + beta).alias('b'))
 
     ds = (
         padawan.scan_parquet(datetime_sample['path'])
         .reindex(['date', 'hour', 't'])
         .map(
             f,
             shared_args=[2, 3],
```

### Comparing `padawan-0.5.1/tests/test_rename.py` & `padawan-0.6/tests/test_rename.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5.1/tests/test_repartition.py` & `padawan-0.6/tests/test_repartition.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5.1/tests/test_slice.py` & `padawan-0.6/tests/test_slice.py`

 * *Files identical despite different names*

### Comparing `padawan-0.5.1/LICENSE` & `padawan-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `padawan-0.5.1/README.md` & `padawan-0.6/README.md`

 * *Files identical despite different names*

### Comparing `padawan-0.5.1/pyproject.toml` & `padawan-0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "padawan"
-version = "0.5.1"
+version = "0.6"
 authors = [
   { name="Martin Wiebusch" },
 ]
 description = "Wrangle partitioned data with polars."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `padawan-0.5.1/PKG-INFO` & `padawan-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: padawan
-Version: 0.5.1
+Version: 0.6
 Summary: Wrangle partitioned data with polars.
 Project-URL: Homepage, https://github.com/mwiebusch78/padawan
 Project-URL: Bug Tracker, https://github.com/mwiebusch78/padawan/issues
 Project-URL: Documentation, https://padawan.readthedocs.io/en/latest/
 Author: Martin Wiebusch
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

