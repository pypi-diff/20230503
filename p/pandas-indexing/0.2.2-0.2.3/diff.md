# Comparing `tmp/pandas-indexing-0.2.2.tar.gz` & `tmp/pandas-indexing-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-indexing-0.2.2.tar", last modified: Tue May  2 11:17:54 2023, max compression
+gzip compressed data, was "pandas-indexing-0.2.3.tar", last modified: Wed May  3 21:24:02 2023, max compression
```

## Comparing `pandas-indexing-0.2.2.tar` & `pandas-indexing-0.2.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:17:54.904339 pandas-indexing-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-02 11:17:54.904339 pandas-indexing-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:17:54.904339 pandas-indexing-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/docs/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:17:54.904339 pandas-indexing-0.2.2/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)   221702 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/docs/notebooks/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 11:17:54.904339 pandas-indexing-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:17:54.900339 pandas-indexing-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:17:54.904339 pandas-indexing-0.2.2/src/pandas_indexing/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/src/pandas_indexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/src/pandas_indexing/accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/src/pandas_indexing/arithmetics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/src/pandas_indexing/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:17:54.904339 pandas-indexing-0.2.2/src/pandas_indexing/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/src/pandas_indexing/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/src/pandas_indexing/datasets/remindhighre_power.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/src/pandas_indexing/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-02 11:17:31.000000 pandas-indexing-0.2.2/src/pandas_indexing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:17:54.904339 pandas-indexing-0.2.2/src/pandas_indexing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-02 11:17:54.000000 pandas-indexing-0.2.2/src/pandas_indexing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-02 11:17:54.000000 pandas-indexing-0.2.2/src/pandas_indexing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:17:54.000000 pandas-indexing-0.2.2/src/pandas_indexing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-02 11:17:54.000000 pandas-indexing-0.2.2/src/pandas_indexing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 11:17:54.000000 pandas-indexing-0.2.2/src/pandas_indexing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:24:02.164447 pandas-indexing-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-03 21:24:02.164447 pandas-indexing-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:24:02.156448 pandas-indexing-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/docs/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:24:02.156448 pandas-indexing-0.2.3/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)   221702 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/docs/notebooks/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 21:24:02.164447 pandas-indexing-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:24:02.152447 pandas-indexing-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:24:02.160447 pandas-indexing-0.2.3/src/pandas_indexing/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/src/pandas_indexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/src/pandas_indexing/accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/src/pandas_indexing/arithmetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11725 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/src/pandas_indexing/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:24:02.164447 pandas-indexing-0.2.3/src/pandas_indexing/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/src/pandas_indexing/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/src/pandas_indexing/datasets/remindhighre_power.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/src/pandas_indexing/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-03 21:23:37.000000 pandas-indexing-0.2.3/src/pandas_indexing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:24:02.160447 pandas-indexing-0.2.3/src/pandas_indexing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-03 21:24:02.000000 pandas-indexing-0.2.3/src/pandas_indexing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-03 21:24:02.000000 pandas-indexing-0.2.3/src/pandas_indexing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 21:24:02.000000 pandas-indexing-0.2.3/src/pandas_indexing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-03 21:24:02.000000 pandas-indexing-0.2.3/src/pandas_indexing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 21:24:02.000000 pandas-indexing-0.2.3/src/pandas_indexing.egg-info/top_level.txt
```

### Comparing `pandas-indexing-0.2.2/CHANGELOG.rst` & `pandas-indexing-0.2.3/CHANGELOG.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 .. currentmodule:: pandas_indexing
 
 Changelog
 =========
 
+v0.2.3 (2023-05-03)
+------------------------------------------------------------
+* :py:func:`~core.uniquelevel` or ``.idx.unique`` returns the unique values of one
+  or multiple levels. :pull:`8`
+* :py:func:`~core.summarylevel` creates a string summarizing the index levels and their
+  values. Can also be accessed as ``df.idx`` or ``index.idx`` :pull:`9`
+
+v0.2.2 (2023-05-02)
+------------------------------------------------------------
 * :py:func:`~core.assignlevel` takes labels from an optional positional dataframe :pull:`5`
 * Add :py:func:`~core.dropnalevel` to remove missing index entries :pull:`4`, :pull:`6`
 
 v0.2.1 (2023-04-08)
 ------------------------------------------------------------
 
 * Restore compatibility with python 3.8
```

### Comparing `pandas-indexing-0.2.2/CODE_OF_CONDUCT.md` & `pandas-indexing-0.2.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.2/CONTRIBUTING.rst` & `pandas-indexing-0.2.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.2/LICENSE` & `pandas-indexing-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.2/PKG-INFO` & `pandas-indexing-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-indexing
-Version: 0.2.2
+Version: 0.2.3
 Summary: Helpers to facilitate working with pandas indices in particular multiindices
 Author-email: Jonas Hörsch <coroa@posteo.de>
 License: MIT
 Project-URL: homepage, https://github.com/coroa/pandas-indexing
 Project-URL: documentation, https://pandas-indexing.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/coroa/pandas-indexing.git
 Project-URL: changelog, https://github.com/coroa/pandas-indexing/blob/main/CHANGELOG.rst
```

### Comparing `pandas-indexing-0.2.2/README.rst` & `pandas-indexing-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.2/docs/api.rst` & `pandas-indexing-0.2.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.2/docs/conf.py` & `pandas-indexing-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.2/docs/notebooks/introduction.ipynb` & `pandas-indexing-0.2.3/docs/notebooks/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.2/pyproject.toml` & `pandas-indexing-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.2/src/pandas_indexing/__init__.py` & `pandas-indexing-0.2.3/src/pandas_indexing/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     alignlevel,
     alignlevels,
     assignlevel,
     dropnalevel,
     index_names,
     projectlevel,
     semijoin,
+    uniquelevel,
 )
 from .selectors import isin, ismatch
 
 
 try:
     __version__ = _version("pandas-indexing")
 except Exception:
```

### Comparing `pandas-indexing-0.2.2/src/pandas_indexing/accessors.py` & `pandas-indexing-0.2.3/src/pandas_indexing/accessors.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,36 @@
 
 from typing import Any, Literal, Optional, Sequence, Union
 
 import pandas as pd
 from pandas import DataFrame, Index, MultiIndex, Series
 
 from . import arithmetics
-from .core import Data, assignlevel, dropnalevel, projectlevel, semijoin
+from .core import (
+    Data,
+    assignlevel,
+    dropnalevel,
+    projectlevel,
+    semijoin,
+    summarylevel,
+    uniquelevel,
+)
 
 
 class _IdxAccessor:
     """
     Convenience accessor for accessing `pandas-indexing` functions.
     """
 
     def __init__(self, pandas_obj):
         self._obj = pandas_obj
 
+    def __repr__(self):
+        return summarylevel(self.obj)
+
     def assign(
         self,
         frame: Optional[Data] = None,
         order: bool = False,
         axis: int = 0,
         **labels: Any,
     ) -> Union[DataFrame, Series, MultiIndex]:
@@ -52,14 +63,39 @@
         Returns
         -------
         df
             Series or DataFrame with changed index or new MultiIndex
         """
         return assignlevel(self._obj, frame=frame, order=order, axis=axis, **labels)
 
+    def unique(
+        self,
+        levels: Union[str, Sequence[str], None],
+        axis: Union[int, Literal["index", "columns"]] = 0,
+    ) -> Index:
+        """
+        Return unique index levels.
+
+        Parameters
+        ----------
+        levels : str or Sequence[str], optional
+            Names of levels to get unique values of
+        axis : int, optional
+            Axis of DataFrame to check on, by default 0
+
+        Returns
+        -------
+        unique_index : Index
+
+        See also
+        --------
+        pandas.Index.unique
+        """
+        return uniquelevel(self.obj, levels=levels, axis=axis)
+
     def project(
         self,
         levels: Sequence[str],
         axis: Union[int, str] = 0,
     ) -> Union[DataFrame, Series, Index]:
         """
         Project multiindex to given `levels`
```

### Comparing `pandas-indexing-0.2.2/src/pandas_indexing/arithmetics.py` & `pandas-indexing-0.2.3/src/pandas_indexing/arithmetics.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.2/src/pandas_indexing/core.py` & `pandas-indexing-0.2.3/src/pandas_indexing/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from operator import and_, or_
 from typing import Any, Literal, Optional, Sequence, TypeVar, Union
 
 import numpy as np
 from pandas import DataFrame, Index, MultiIndex, Series
 from pandas.core.indexes.frozen import FrozenList
 
+from .utils import print_list
+
 
 Data = Union[Series, DataFrame]
 T = TypeVar("T", bound=Union[Index, DataFrame, Series])
 S = TypeVar("S", bound=Union[DataFrame, Series])
 
 
 def _assignlevel(
@@ -198,14 +200,95 @@
 
     if axis in (0, "index"):
         return index_or_series.loc[_notna(index_or_series.index, subset, how)]
 
     return index_or_series.loc[:, _notna(index_or_series.columns, subset, how)]
 
 
+def uniquelevel(
+    index_or_data: Union[DataFrame, Series, Index],
+    levels: Union[str, Sequence[str], None],
+    axis: Union[int, Literal["index", "columns"]] = 0,
+) -> Index:
+    """
+    Return unique index levels.
+
+    Parameters
+    ----------
+    index_or_data : Index|Series|DataFrame
+        Index, Series or DataFrame from which to get unique values
+    levels : str or Sequence[str], optional
+        Names of levels to get unique values of
+    axis : int, optional
+        Axis of DataFrame to check on, by default 0
+
+    Returns
+    -------
+    unique_index : Index
+
+    See also
+    --------
+    pandas.Index.unique
+    """
+    if isinstance(index_or_data, (DataFrame, Series)):
+        index_or_data = (
+            index_or_data.index if axis in (0, "index") else index_or_data.columns
+        )
+
+    if levels is None or isinstance(levels, str):
+        return index_or_data.unique(level=levels)
+
+    levels = list(levels)
+    if len(levels) == 1:
+        return index_or_data.unique(level=levels[0])
+
+    return projectlevel(index_or_data, levels).unique()
+
+
+def _summarylevel(index: Index, n: int = 80) -> str:
+    def name(l):
+        return "<unnamed>" if l is None else l
+
+    c1 = max(len(name(l)) for l in index.names) + 1
+    c2 = n - c1 - 5
+    return "\n".join(
+        f" * {name(l):{c1}}: {print_list(index.unique(l), c2)}" for l in index.names
+    )
+
+
+def summarylevel(index_or_data: Union[DataFrame, Series, Index], n: int = 80):
+    """
+    Summarize index levels.
+
+    Parameters
+    ----------
+    index_or_data : Index|Series|DataFrame
+        Index, Series or DataFrame of which to summarize index levels
+    n : int, default 80
+        The maximum line length
+
+    Returns
+    -------
+    summary : str
+
+    See also
+    --------
+    pandas.DataFrame.describe
+    """
+    if isinstance(index_or_data, DataFrame):
+        index_desc = _summarylevel(index_or_data.index, n=n)
+        columns_desc = _summarylevel(index_or_data.columns, n=n)
+        return f"Index:\n{index_desc}\n\nColumns:\n{columns_desc}"
+
+    if isinstance(index_or_data, Series):
+        index_or_data = index_or_data.index
+
+    return f"Index:\n{_summarylevel(index_or_data, n=n)}"
+
+
 def index_names(s, raise_on_index=False):
     if isinstance(s, (Series, DataFrame)):
         s = s.index
 
     if isinstance(s, MultiIndex):
         names = s.names
     elif isinstance(s, Index):
```

### Comparing `pandas-indexing-0.2.2/src/pandas_indexing/datasets/__init__.py` & `pandas-indexing-0.2.3/src/pandas_indexing/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.2/src/pandas_indexing/datasets/remindhighre_power.csv` & `pandas-indexing-0.2.3/src/pandas_indexing/datasets/remindhighre_power.csv`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.2/src/pandas_indexing/selectors.py` & `pandas-indexing-0.2.3/src/pandas_indexing/selectors.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.2/src/pandas_indexing.egg-info/PKG-INFO` & `pandas-indexing-0.2.3/src/pandas_indexing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-indexing
-Version: 0.2.2
+Version: 0.2.3
 Summary: Helpers to facilitate working with pandas indices in particular multiindices
 Author-email: Jonas Hörsch <coroa@posteo.de>
 License: MIT
 Project-URL: homepage, https://github.com/coroa/pandas-indexing
 Project-URL: documentation, https://pandas-indexing.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/coroa/pandas-indexing.git
 Project-URL: changelog, https://github.com/coroa/pandas-indexing/blob/main/CHANGELOG.rst
```

### Comparing `pandas-indexing-0.2.2/src/pandas_indexing.egg-info/SOURCES.txt` & `pandas-indexing-0.2.3/src/pandas_indexing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

