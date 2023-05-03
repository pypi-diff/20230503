# Comparing `tmp/arraymap-0.1.5.tar.gz` & `tmp/arraymap-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraymap-0.1.5.tar", last modified: Sat Apr 22 21:47:43 2023, max compression
+gzip compressed data, was "arraymap-0.1.6.tar", last modified: Wed May  3 02:59:41 2023, max compression
```

## Comparing `arraymap-0.1.5.tar` & `arraymap-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:47:43.251312 arraymap-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-22 21:47:42.000000 arraymap-0.1.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-22 21:47:42.000000 arraymap-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-22 21:47:43.251312 arraymap-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-22 21:47:42.000000 arraymap-0.1.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    61022 2023-04-22 21:47:42.000000 arraymap-0.1.5/arraymap.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:47:43.251312 arraymap-0.1.5/arraymap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-22 21:47:43.000000 arraymap-0.1.5/arraymap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-22 21:47:43.000000 arraymap-0.1.5/arraymap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 21:47:43.000000 arraymap-0.1.5/arraymap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-22 21:47:43.000000 arraymap-0.1.5/arraymap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-22 21:47:43.000000 arraymap-0.1.5/arraymap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-22 21:47:43.251312 arraymap-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-22 21:47:42.000000 arraymap-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:47:43.251312 arraymap-0.1.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-04-22 21:47:42.000000 arraymap-0.1.5/test/test_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    15954 2023-04-22 21:47:42.000000 arraymap-0.1.5/test/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:59:41.724670 arraymap-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-03 02:59:37.000000 arraymap-0.1.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-03 02:59:37.000000 arraymap-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-03 02:59:41.724670 arraymap-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-03 02:59:37.000000 arraymap-0.1.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    90207 2023-05-03 02:59:37.000000 arraymap-0.1.6/arraymap.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:59:41.724670 arraymap-0.1.6/arraymap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-03 02:59:41.000000 arraymap-0.1.6/arraymap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-03 02:59:41.000000 arraymap-0.1.6/arraymap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 02:59:41.000000 arraymap-0.1.6/arraymap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 02:59:41.000000 arraymap-0.1.6/arraymap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 02:59:41.000000 arraymap-0.1.6/arraymap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-03 02:59:41.728670 arraymap-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-03 02:59:37.000000 arraymap-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:59:41.724670 arraymap-0.1.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-05-03 02:59:37.000000 arraymap-0.1.6/test/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24341 2023-05-03 02:59:37.000000 arraymap-0.1.6/test/test_unit.py
```

### Comparing `arraymap-0.1.5/LICENSE.md` & `arraymap-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arraymap-0.1.5/PKG-INFO` & `arraymap-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arraymap
-Version: 0.1.5
+Version: 0.1.6
 Summary: Dictionary-like lookup from NumPy array values to their integer positions
 Home-page: https://github.com/static-frame/arraymap
 Author: Christopher Ariza, Brandt Bucher
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
@@ -54,14 +54,22 @@
 - NumPy >= 1.18.5
 
 
 
 What is New in ArrayMap
 -------------------------
 
+0.1.6
+........
+
+Implemented ``get_all()`` and ``get_any()`` for optimized lookup of multiple keys from arrays or lists.
+
+Implemented full support for ``np.datetime64`` arrays.
+
+
 0.1.5
 ........
 
 Improved handling for Unicode elements that contain non-terminal NULL strings.
 
 
 0.1.4
```

### Comparing `arraymap-0.1.5/README.rst` & `arraymap-0.1.6/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -32,14 +32,22 @@
 - NumPy >= 1.18.5
 
 
 
 What is New in ArrayMap
 -------------------------
 
+0.1.6
+........
+
+Implemented ``get_all()`` and ``get_any()`` for optimized lookup of multiple keys from arrays or lists.
+
+Implemented full support for ``np.datetime64`` arrays.
+
+
 0.1.5
 ........
 
 Improved handling for Unicode elements that contain non-terminal NULL strings.
 
 
 0.1.4
```

### Comparing `arraymap-0.1.5/arraymap.egg-info/PKG-INFO` & `arraymap-0.1.6/arraymap.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arraymap
-Version: 0.1.5
+Version: 0.1.6
 Summary: Dictionary-like lookup from NumPy array values to their integer positions
 Home-page: https://github.com/static-frame/arraymap
 Author: Christopher Ariza, Brandt Bucher
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
@@ -54,14 +54,22 @@
 - NumPy >= 1.18.5
 
 
 
 What is New in ArrayMap
 -------------------------
 
+0.1.6
+........
+
+Implemented ``get_all()`` and ``get_any()`` for optimized lookup of multiple keys from arrays or lists.
+
+Implemented full support for ``np.datetime64`` arrays.
+
+
 0.1.5
 ........
 
 Improved handling for Unicode elements that contain non-terminal NULL strings.
 
 
 0.1.4
```

### Comparing `arraymap-0.1.5/setup.py` & `arraymap-0.1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 import typing as tp
 import site
 import os
 
 
-AM_VERSION = "0.1.5"
+AM_VERSION = "0.1.6"
 
 
 with open("README.rst") as file:
     LONG_DESCRIPTION = file.read()
 
 
 def get_ext_dir(*components: tp.Iterable[str]) -> tp.Sequence[str]:
```

### Comparing `arraymap-0.1.5/test/test_unit.py` & `arraymap-0.1.6/test/test_unit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-import typing
 import pickle
 import pytest
-import sys
 import numpy as np
 
 from arraymap import AutoMap
 from arraymap import FrozenAutoMap
 from arraymap import NonUniqueError
 
 
@@ -88,33 +86,75 @@
     a1 = np.array((-2, -1, 1, 2), dtype=np.int8)
     a1.flags.writeable = False
     fam = FrozenAutoMap(a1)
     for k in a1:
         assert k in fam
 
 
+def test_fam_constructor_array_int_e():
+    # https://github.com/static-frame/arraymap/issues/12
+    a1 = np.array((0, 0, 1, 1, 2, 2), dtype=int)
+    a2 = a1[[0, 2, 4]]
+    a2.flags.writeable = False
+    fam1 = FrozenAutoMap(a2)
+    assert list(fam1) == [0, 1, 2]
+
+    d1 = {i: int(i) for i in a2}
+    fam2 = FrozenAutoMap(d1)
+    assert list(fam2) == [0, 1, 2]
+
+    d2 = {0: 0, 3: 1}
+    fam3 = FrozenAutoMap(d2)
+    assert list(fam3) == [0, 3]
+
+
 # ------------------------------------------------------------------------------
 
 
 def test_fam_constructor_array_float_a():
     a1 = np.array((1.2, 8.8, 1.2))
     a1.flags.writeable = False
     with pytest.raises(NonUniqueError):
         fam = FrozenAutoMap(a1)
 
 
 # ------------------------------------------------------------------------------
 
 
 def test_fam_constructor_array_dt64_a():
-    a1 = np.array(("2022-01", "2023-05"), dtype=np.datetime64)
+    a1 = np.array(("1970-01", "2023-05"), dtype=np.datetime64)
     a1.flags.writeable = False
     fam = FrozenAutoMap(a1)
+
     assert fam[np.datetime64("2023-05")] == 1
-    # assert np.datetime64('2022-05') in a1
+    assert fam[np.datetime64("1970-01")] == 0
+
+    with pytest.raises(KeyError):
+        fam[np.datetime64("nat")]
+
+    with pytest.raises(KeyError):
+        fam[np.datetime64("1970")]
+
+
+def test_fam_constructor_array_dt64_b():
+    a1 = np.array(("1542", "nat"), dtype=np.datetime64)
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+    assert fam[np.datetime64("nat")] == 1
+    assert fam[np.datetime64("nat", "D")] == 1
+    assert fam[np.datetime64("nat", "ns")] == 1
+    assert fam[np.datetime64("1542")] == 0
+
+
+def test_fam_constructor_array_dt64_c():
+    a1 = np.array(("nat", "nat"), dtype=np.datetime64)
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+    # when we get "generic" dt64 units, we load scalars in a list, and can thus support multiple NaNs
+    assert len(fam) == 2
 
 
 # ------------------------------------------------------------------------------
 
 
 def test_fam_constructor_array_unicode_a():
     a1 = np.array(("a", "b", "a"))
@@ -213,14 +253,28 @@
     assert fam2[b"ccc"] == 1
     assert fam2[b"bb"] == 2
 
 
 # ------------------------------------------------------------------------------
 
 
+def test_fam_array_bytes_get_a():
+    a1 = np.array((b"", b"  ", b"   ", b"    "))
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+
+    assert fam.get(b"") == 0
+    assert fam.get(b" ") == None
+    assert fam.get(b"   ") == 2
+    assert fam.get(b"    ") == 3
+
+
+# ------------------------------------------------------------------------------
+
+
 def test_fam_array_len_a():
     a1 = np.array((10, 20, 30, 40), dtype=np.int64)
     a1.flags.writeable = False
     fam = FrozenAutoMap(a1)
     assert len(fam) == 4
 
 
@@ -354,14 +408,22 @@
     assert 2.0 in fam
     assert 2.1 not in fam
     assert True in fam
     assert False in fam
     assert 4 in fam
 
 
+def test_fam_array_int_get_e():
+    a1 = np.array((1,), dtype=np.int16)
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+    assert a1[0] in fam
+    assert 1 in fam
+
+
 # ------------------------------------------------------------------------------
 
 
 def test_fam_array_uint_get_a():
     a1 = np.array((1, 100, 300, 4000), dtype=np.uint64)
     a1.flags.writeable = False
     fam = FrozenAutoMap(a1)
@@ -548,14 +610,25 @@
     assert fam.get("ccc") == 2
     assert fam.get(None) is None
     assert fam.get(3.2) is None
     assert fam.get("cc") is None
     assert fam.get("cccc") is None
 
 
+def test_fam_array_unicode_get_b():
+    a1 = np.array(("", "  ", "   ", "    "))
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+
+    assert fam.get("") == 0
+    assert fam.get(" ") == None
+    assert fam.get("   ") == 2
+    assert fam.get("    ") == 3
+
+
 # ------------------------------------------------------------------------------
 
 
 def test_fam_array_values_a():
     a1 = np.array((10, 20, 30, 40), dtype=np.int64)
     a1.flags.writeable = False
     fam = FrozenAutoMap(a1)
@@ -643,13 +716,250 @@
 # ------------------------------------------------------------------------------
 
 
 def test_fam_array_pickle_a():
     a1 = np.array(("a", "b", "c", "d"))
     a1.flags.writeable = False
     fam1 = FrozenAutoMap(a1)
-
     fam2 = pickle.loads(pickle.dumps(fam1))
+    assert list(fam1.values()) == list(fam2.values())
+
+
+# ------------------------------------------------------------------------------
+
+
+def test_fam_array_get_all_a():
+    a1 = np.array((1, 100, 300, 4000))
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+
+    with pytest.raises(TypeError):
+        fam.get_all((3, 3))
+
+    with pytest.raises(TypeError):
+        fam.get_all("a")
+
+    with pytest.raises(TypeError):
+        fam.get_all(None)
+
+
+def test_fam_array_get_all_b():
+    a1 = np.array((1, 100, 300, 4000))
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+    post1 = fam.get_all([300, 100])
+    assert post1.tolist() == [2, 1]
+    x = [y for y in post1]
+    del x
+    del post1
+    post2 = fam.get_all([4000, 4000, 4000])
+    assert post2.tolist() == [3, 3, 3]
+    x = [y for y in post2]
+    del x
+
+
+def test_fam_array_get_all_c():
+    a1 = np.array(("a", "bb", "ccc"))
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+    with pytest.raises(KeyError):
+        fam.get_all(["bb", "c"])
+
+
+def test_fam_array_get_all_d1():
+    a1 = np.array(("a", "bb", "ccc"))
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+    post1 = fam.get_all(np.array(("bb", "a", "ccc", "a", "bb")))
+    assert post1.tolist() == [1, 0, 2, 0, 1]
+    assert post1.flags.writeable == False
+
+
+def test_fam_array_get_all_d2():
+    a1 = np.array(("a", "bb", "ccc"))
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+    with pytest.raises(KeyError):
+        fam.get_all(np.array(("bb", "a", "ccc", "aa")))
+
+
+def test_fam_array_get_all_e():
+    a1 = np.array((2,), dtype=np.uint64)
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+    assert fam.get_all([2]) == [0]
+    assert fam.get_all(a1) == [0]
+
+
+def test_fam_array_get_all_f1():
+    a1 = np.array(("a", "bb", "ccc", "dd"))
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+
+    post = fam.get_all(np.array(["ccc", "dd", "bb", "bb"]))
+    assert post.tolist() == [2, 3, 1, 1]
+
+
+def test_fam_array_get_all_f2():
+    a1 = np.array(("a", "bb", "ccc", "dd"))
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+
+    with pytest.raises(KeyError):
+        fam.get_all(np.array(["bb", "c"]))
+
+
+def test_fam_array_get_all_g1():
+    a1 = np.array((b"a", b"bb", b"ccc", b"dd"))
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+
+    post = fam.get_all(np.array([b"ccc", b"dd", b"bb", b"bb"]))
+    assert post.tolist() == [2, 3, 1, 1]
+
+
+def test_fam_array_get_all_g2():
+    a1 = np.array((b"a", b"bb", b"ccc", b"dd"))
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+
+    with pytest.raises(KeyError):
+        fam.get_all(np.array([b"dd", b"x"]))
+
+
+def test_fam_array_get_all_h():
+    a1 = np.array((b"a", b""))
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+
+    post = fam.get_all(np.array([b"", b"", b"a"]))
+    assert post.tolist() == [1, 1, 0]
+
+
+def test_fam_array_get_all_i():
+    a1 = np.array((b"foo", b"bar"))
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+    with pytest.raises(KeyError):
+        _ = fam.get_all(np.array([b"fo", b"ba"]))
+
+    with pytest.raises(KeyError):
+        _ = fam.get_all(np.array([b"", b""]))
+
+
+def test_fam_array_get_all_j():
+    a1 = np.array(("aaaaa", "bb", "ccc", "dd"))
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+
+    with pytest.raises(KeyError):
+        _ = fam.get_all(np.array(["a", "b"]))
+
+    assert fam.get_all(np.array(("bb", "dd", "bb", "dd"))).tolist() == [1, 3, 1, 3]
+
+
+def test_fam_array_get_all_k1():
+    a1 = np.array(("2023-01-05", "1854-05-02"), np.datetime64)
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+
+    post = fam.get_all(
+        np.array(["1854-05-02", "2023-01-05", "2023-01-05"], np.datetime64)
+    )
+    assert post.tolist() == [1, 0, 0]
+
+
+def test_fam_array_get_all_k2():
+    a1 = np.array(("2023-01-05", "1854-05-02"), np.datetime64)
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+
+    with pytest.raises(KeyError):
+        post = fam.get_all(
+            np.array(["1854-05-02", "2023-01-05", "2020-01-05"], np.datetime64)
+        )
 
-    # import ipdb
 
-    # ipdb.set_trace()
+def test_fam_array_get_all_l():
+    a1 = np.array(("2023-01-05", "1854-05-02", "1988-01-01"), np.datetime64)
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+    with pytest.raises(KeyError):
+        _ = fam.get_all(np.array(["2022-01", "2023-01", "1988-01"], np.datetime64))
+
+
+# -------------------------------------------------------------------------------
+
+
+def test_fam_array_get_any_a1():
+    a1 = np.array(("a", "bb", "ccc"))
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+    post1 = fam.get_any(["bbb", "ccc", "a", "bbb"])
+    assert post1 == [2, 0]
+
+    post2 = fam.get_any(["bbb", "bbb"])
+    assert post2 == []
+
+
+def test_fam_array_get_any_a2():
+    a1 = np.array(("a", "bb", "ccc"))
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+    post1 = fam.get_any(np.array(("bbb", "a", "ccc", "aa", "bbb")))
+    assert post1 == [0, 2]
+
+
+def test_fam_array_get_any_a3():
+    a1 = np.array(("a", "bb", "ccc"))
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+    post1 = fam.get_any(np.array(["bbb", "ccc", "a", "bbb"]))
+    assert post1 == [2, 0]
+
+    post2 = fam.get_any(np.array(["bbb", "bbb"]))
+    assert post2 == []
+
+
+def test_fam_array_get_any_b():
+    a1 = np.array([4294967295], dtype=np.uint32)
+    a1.flags.writeable = False
+    a1_list = list(a1)
+    fam = FrozenAutoMap(a1)
+    assert a1[0] in fam
+    assert 4294967295 in fam
+
+    post1 = fam.get_any(a1_list)
+    assert post1 == list(fam.values())
+
+
+def test_fam_array_get_any_c1():
+    a1 = np.array(("2023-01-05", "1854-05-02"), np.datetime64)
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+
+    post = fam.get_any(
+        np.array(
+            ["1854-05-02", "nat", "1854-05-02", "2023-01-05", "nat"], np.datetime64
+        )
+    )
+    assert post == [1, 1, 0]
+
+
+def test_fam_array_get_any_c2():
+    a1 = np.array(("2023-01-05", "1854-05-02"), np.datetime64)
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+
+    post = fam.get_any(
+        np.array(["1854-05-02", "2023-01-05", "2020-01-05"], np.datetime64)
+    )
+    assert post == [1, 0]
+
+
+def test_fam_array_get_any_d():
+    a1 = np.array(("2023-01-05", "1854-05-02", "1988-01-01"), np.datetime64)
+    a1.flags.writeable = False
+    fam = FrozenAutoMap(a1)
+
+    post = fam.get_any(np.array(["2022-01", "2023-01", "1988-01"], np.datetime64))
+    assert post == []
```

