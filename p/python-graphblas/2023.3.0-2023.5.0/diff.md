# Comparing `tmp/python-graphblas-2023.3.0.tar.gz` & `tmp/python-graphblas-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-graphblas-2023.3.0.tar", last modified: Fri Mar 31 19:57:22 2023, max compression
+gzip compressed data, was "python-graphblas-2023.5.0.tar", last modified: Wed May  3 15:17:55 2023, max compression
```

## Comparing `python-graphblas-2023.3.0.tar` & `python-graphblas-2023.5.0.tar`

### file list

```diff
@@ -1,114 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:57:22.287931 python-graphblas-2023.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25253 2023-03-31 19:57:22.287931 python-graphblas-2023.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10313 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:57:22.255931 python-graphblas-2023.3.0/graphblas/
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:57:22.255931 python-graphblas-2023.3.0/graphblas/agg/
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/agg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/agg/ss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:57:22.255931 python-graphblas-2023.3.0/graphblas/binary/
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/binary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/binary/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/binary/ss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:57:22.263931 python-graphblas-2023.3.0/graphblas/core/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/agg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12689 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/automethods.py
--rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)    21115 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/expr.py
--rw-r--r--   0 runner    (1001) docker     (123)    30123 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    20225 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/infix.py
--rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/infixmethods.py
--rw-r--r--   0 runner    (1001) docker     (123)    15867 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)   140629 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:57:22.267931 python-graphblas-2023.3.0/graphblas/core/operator/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23889 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/operator/agg.py
--rw-r--r--   0 runner    (1001) docker     (123)    18078 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/operator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    30558 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/operator/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/operator/indexunary.py
--rw-r--r--   0 runner    (1001) docker     (123)    15293 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/operator/monoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/operator/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    20466 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/operator/semiring.py
--rw-r--r--   0 runner    (1001) docker     (123)    14742 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/operator/unary.py
--rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/operator/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    39234 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/slice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:57:22.271931 python-graphblas-2023.3.0/graphblas/core/ss/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/ss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/ss/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/ss/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)   158516 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/ss/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/ss/prefix_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)    59209 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/ss/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12906 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    81671 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/core/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12489 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/graphblas.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:57:22.271931 python-graphblas-2023.3.0/graphblas/indexunary/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/indexunary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22976 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:57:22.271931 python-graphblas-2023.3.0/graphblas/monoid/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/monoid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/monoid/numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:57:22.271931 python-graphblas-2023.3.0/graphblas/op/
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/op/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/op/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/op/ss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:57:22.271931 python-graphblas-2023.3.0/graphblas/select/
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/select/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:57:22.271931 python-graphblas-2023.3.0/graphblas/semiring/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/semiring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/semiring/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/semiring/ss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:57:22.275931 python-graphblas-2023.3.0/graphblas/ss/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/ss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/ss/_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:57:22.283931 python-graphblas-2023.3.0/graphblas/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/pickle1-vanilla.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/pickle1.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/pickle2-vanilla.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/pickle2.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/pickle3-vanilla.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/pickle3.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/test_auto_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/test_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/test_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/test_external_init.py
--rw-r--r--   0 runner    (1001) docker     (123)   185979 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/test_infix.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/test_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)   148559 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    12335 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/test_numpyops.py
--rw-r--r--   0 runner    (1001) docker     (123)    50785 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/test_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/test_operator_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/test_prefix_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     9199 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/test_recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/test_resolving.py
--rw-r--r--   0 runner    (1001) docker     (123)    19052 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/test_scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/test_ss_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    86887 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/tests/test_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:57:22.287931 python-graphblas-2023.3.0/graphblas/unary/
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/unary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/unary/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/unary/ss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/graphblas/viz.py
--rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 19:57:22.287931 python-graphblas-2023.3.0/python_graphblas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25253 2023-03-31 19:57:22.000000 python-graphblas-2023.3.0/python_graphblas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-03-31 19:57:22.000000 python-graphblas-2023.3.0/python_graphblas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 19:57:22.000000 python-graphblas-2023.3.0/python_graphblas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-31 19:57:22.000000 python-graphblas-2023.3.0/python_graphblas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-31 19:57:22.000000 python-graphblas-2023.3.0/python_graphblas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 19:57:22.287931 python-graphblas-2023.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 19:57:02.000000 python-graphblas-2023.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.581513 python-graphblas-2023.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    26264 2023-05-03 15:17:55.581513 python-graphblas-2023.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.565513 python-graphblas-2023.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.565513 python-graphblas-2023.5.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.569513 python-graphblas-2023.5.0/docs/_static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/docs/_static/img/draw-example.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/docs/_static/img/logo-name-medium.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/docs/_static/img/repr-matrix.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.569513 python-graphblas-2023.5.0/graphblas/
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.569513 python-graphblas-2023.5.0/graphblas/agg/
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/agg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/agg/ss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.569513 python-graphblas-2023.5.0/graphblas/binary/
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/binary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/binary/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/binary/ss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.569513 python-graphblas-2023.5.0/graphblas/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/agg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12689 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/automethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21115 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30152 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20225 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/infix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/infixmethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15867 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)   140889 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.573513 python-graphblas-2023.5.0/graphblas/core/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24808 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/operator/agg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17765 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/operator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36090 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/operator/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19095 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/operator/indexunary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16879 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/operator/monoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11902 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/operator/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21700 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/operator/semiring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18209 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/operator/unary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/operator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39703 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/slice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.573513 python-graphblas-2023.5.0/graphblas/core/ss/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/ss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/ss/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/ss/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   158708 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/ss/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/ss/prefix_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59191 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/ss/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83507 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/core/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/graphblas.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.573513 python-graphblas-2023.5.0/graphblas/indexunary/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/indexunary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.573513 python-graphblas-2023.5.0/graphblas/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/io/_awkward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/io/_matrixmarket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/io/_networkx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/io/_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/io/_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/io/_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/io/_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.577513 python-graphblas-2023.5.0/graphblas/monoid/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/monoid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/monoid/numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.577513 python-graphblas-2023.5.0/graphblas/op/
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/op/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/op/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/op/ss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.577513 python-graphblas-2023.5.0/graphblas/select/
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/select/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.577513 python-graphblas-2023.5.0/graphblas/semiring/
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/semiring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/semiring/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/semiring/ss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.577513 python-graphblas-2023.5.0/graphblas/ss/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/ss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/ss/_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.581513 python-graphblas-2023.5.0/graphblas/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/pickle1-vanilla.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/pickle1.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/pickle2-vanilla.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/pickle2.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/pickle3-vanilla.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/pickle3.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_auto_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_external_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187980 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_infix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16612 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151341 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_numpyops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54654 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_operator_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_prefix_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9199 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_resolving.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19247 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_ss_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88452 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/tests/test_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.581513 python-graphblas-2023.5.0/graphblas/unary/
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/unary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/unary/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/unary/ss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/graphblas/viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16813 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:17:55.581513 python-graphblas-2023.5.0/python_graphblas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26264 2023-05-03 15:17:55.000000 python-graphblas-2023.5.0/python_graphblas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-03 15:17:55.000000 python-graphblas-2023.5.0/python_graphblas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:17:55.000000 python-graphblas-2023.5.0/python_graphblas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-03 15:17:55.000000 python-graphblas-2023.5.0/python_graphblas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 15:17:55.000000 python-graphblas-2023.5.0/python_graphblas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:17:55.581513 python-graphblas-2023.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:17:35.000000 python-graphblas-2023.5.0/setup.py
```

### Comparing `python-graphblas-2023.3.0/LICENSE` & `python-graphblas-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/PKG-INFO` & `python-graphblas-2023.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-graphblas
-Version: 2023.3.0
+Version: 2023.5.0
 Summary: Python library for GraphBLAS: high-performance sparse linear algebra for scalable graph analytics
 Author: Jim Kitchen, Python-graphblas contributors
 Author-email: Erik Welch <erik.n.welch@gmail.com>
 Maintainer-email: Erik Welch <erik.n.welch@gmail.com>, Jim Kitchen <jim22k@gmail.com>, Sultan Orazbayev <contact@econpoint.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -218,80 +218,100 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: suitesparse
+Provides-Extra: networkx
+Provides-Extra: numba
+Provides-Extra: pandas
+Provides-Extra: scipy
+Provides-Extra: suitesparse-udf
 Provides-Extra: repr
 Provides-Extra: io
 Provides-Extra: viz
+Provides-Extra: datashade
 Provides-Extra: test
-Provides-Extra: complete
+Provides-Extra: default
+Provides-Extra: all
 License-File: LICENSE
 
-# Python-graphblas
+![Python-graphblas](docs/_static/img/logo-name-medium.svg)
 
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/python-graphblas.svg)](https://anaconda.org/conda-forge/python-graphblas)
 [![pypi](https://img.shields.io/pypi/v/python-graphblas.svg)](https://pypi.python.org/pypi/python-graphblas/)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/python-graphblas)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/python-graphblas)](https://pypi.python.org/pypi/python-graphblas/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/python-graphblas/python-graphblas/blob/main/LICENSE)
+<br>
 [![Tests](https://github.com/python-graphblas/python-graphblas/workflows/Tests/badge.svg?branch=main)](https://github.com/python-graphblas/python-graphblas/actions)
 [![Docs](https://readthedocs.org/projects/python-graphblas/badge/?version=latest)](https://python-graphblas.readthedocs.io/en/latest/)
 [![Coverage](https://coveralls.io/repos/python-graphblas/python-graphblas/badge.svg?branch=main)](https://coveralls.io/r/python-graphblas/python-graphblas)
+<br>
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7328791.svg)](https://doi.org/10.5281/zenodo.7328791)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/python-graphblas/python-graphblas/HEAD?filepath=notebooks%2FIntro%20to%20GraphBLAS%20%2B%20SSSP%20example.ipynb)
 [![Discord](https://img.shields.io/badge/Chat-Discord-blue)](https://discord.com/invite/vur45CbwMz)
 
 Python library for GraphBLAS: high-performance sparse linear algebra for scalable graph analytics.
+For algorithms, see
+[`graphblas-algorithms`](https://github.com/python-graphblas/graphblas-algorithms).
 
 - **Documentation:** [https://python-graphblas.readthedocs.io/](https://python-graphblas.readthedocs.io/)
+  - **FAQ:** [https://python-graphblas.readthedocs.io/en/stable/getting_started/faq.html](https://python-graphblas.readthedocs.io/en/stable/getting_started/faq.html)
   - **GraphBLAS C API:** [https://graphblas.org/docs/GraphBLAS_API_C_v2.0.0.pdf](https://graphblas.org/docs/GraphBLAS_API_C_v2.0.0.pdf)
   - **SuiteSparse:GraphBLAS User Guide:** [https://github.com/DrTimothyAldenDavis/GraphBLAS/raw/stable/Doc/GraphBLAS_UserGuide.pdf](https://github.com/DrTimothyAldenDavis/GraphBLAS/raw/stable/Doc/GraphBLAS_UserGuide.pdf)
 - **Source:** [https://github.com/python-graphblas/python-graphblas](https://github.com/python-graphblas/python-graphblas)
 - **Bug reports:** [https://github.com/python-graphblas/python-graphblas/issues](https://github.com/python-graphblas/python-graphblas/issues)
 - **Github discussions:** [https://github.com/python-graphblas/python-graphblas/discussions](https://github.com/python-graphblas/python-graphblas/discussions)
 - **Weekly community call:** [https://github.com/python-graphblas/python-graphblas/issues/247](https://github.com/python-graphblas/python-graphblas/issues/247)
 - **Chat via Discord:** [https://discord.com/invite/vur45CbwMz](https://discord.com/invite/vur45CbwMz) in the [#graphblas channel](https://discord.com/channels/786703927705862175/1024732940233605190)
 
+<p float="left">
+  <img src="docs/_static/img/draw-example.png" width="231" align="top" alt="Directed graph", title="Directed graph"/>
+  <img src="docs/_static/img/repr-matrix.png" width="231" align="top" alt="Adjacency matrix" title="Adjacency matrix"/>
+</p>
+
 ## Install
 Install the latest version of Python-graphblas via conda:
 ```
 $ conda install -c conda-forge python-graphblas
 ```
 or pip:
 ```
-$ pip install python-graphblas
+$ pip install python-graphblas[default]
 ```
 This will also install the [SuiteSparse:GraphBLAS](https://github.com/DrTimothyAldenDavis/GraphBLAS) compiled C library.
+We currently support the [GraphBLAS C API 2.0 specification](https://graphblas.org/docs/GraphBLAS_API_C_v2.0.0.pdf).
 
 ### Optional Dependencies
 
 The following are not required by python-graphblas, but may be needed for certain functionality to work.
 
 - `pandas` – required for nicer `__repr__`;
 - `matplotlib` – required for basic plotting of graphs;
-- `scipy` – used in io module to read/write `scipy.sparse` format;
+- `scipy` – used in `io` module to read/write `scipy.sparse` format;
 - `networkx` – used in `io` module to interface with `networkx` graphs;
 - `fast-matrix-market` - for faster read/write of Matrix Market files with `gb.io.mmread` and `gb.io.mmwrite`.
 
 ## Description
 Currently works with [SuiteSparse:GraphBLAS](https://github.com/DrTimothyAldenDavis/GraphBLAS), but the goal is to make it work with all implementations of the GraphBLAS spec.
 
-The approach taken with this library is to follow the C-API specification as closely as possible while making improvements
+The approach taken with this library is to follow the C-API 2.0 specification as closely as possible while making improvements
 allowed with the Python syntax. Because the spec always passes in the output object to be written to, we follow the same,
 which is very different from the way Python normally operates. In fact, many who are familiar with other Python data
 libraries (numpy, pandas, etc) will find it strange to not create new objects for every call.
 
 At the highest level, the goal is to separate output, mask, and accumulator on the left side of the assignment
 operator `=` and put the computation on the right side. Unfortunately, that approach doesn't always work very well
 with how Python handles assignment, so instead we (ab)use the left-shift `<<` notation to give the same flavor of
```

### Comparing `python-graphblas-2023.3.0/README.md` & `python-graphblas-2023.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,67 @@
-# Python-graphblas
+![Python-graphblas](docs/_static/img/logo-name-medium.svg)
 
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/python-graphblas.svg)](https://anaconda.org/conda-forge/python-graphblas)
 [![pypi](https://img.shields.io/pypi/v/python-graphblas.svg)](https://pypi.python.org/pypi/python-graphblas/)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/python-graphblas)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/python-graphblas)](https://pypi.python.org/pypi/python-graphblas/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/python-graphblas/python-graphblas/blob/main/LICENSE)
+<br>
 [![Tests](https://github.com/python-graphblas/python-graphblas/workflows/Tests/badge.svg?branch=main)](https://github.com/python-graphblas/python-graphblas/actions)
 [![Docs](https://readthedocs.org/projects/python-graphblas/badge/?version=latest)](https://python-graphblas.readthedocs.io/en/latest/)
 [![Coverage](https://coveralls.io/repos/python-graphblas/python-graphblas/badge.svg?branch=main)](https://coveralls.io/r/python-graphblas/python-graphblas)
+<br>
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7328791.svg)](https://doi.org/10.5281/zenodo.7328791)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/python-graphblas/python-graphblas/HEAD?filepath=notebooks%2FIntro%20to%20GraphBLAS%20%2B%20SSSP%20example.ipynb)
 [![Discord](https://img.shields.io/badge/Chat-Discord-blue)](https://discord.com/invite/vur45CbwMz)
 
 Python library for GraphBLAS: high-performance sparse linear algebra for scalable graph analytics.
+For algorithms, see
+[`graphblas-algorithms`](https://github.com/python-graphblas/graphblas-algorithms).
 
 - **Documentation:** [https://python-graphblas.readthedocs.io/](https://python-graphblas.readthedocs.io/)
+  - **FAQ:** [https://python-graphblas.readthedocs.io/en/stable/getting_started/faq.html](https://python-graphblas.readthedocs.io/en/stable/getting_started/faq.html)
   - **GraphBLAS C API:** [https://graphblas.org/docs/GraphBLAS_API_C_v2.0.0.pdf](https://graphblas.org/docs/GraphBLAS_API_C_v2.0.0.pdf)
   - **SuiteSparse:GraphBLAS User Guide:** [https://github.com/DrTimothyAldenDavis/GraphBLAS/raw/stable/Doc/GraphBLAS_UserGuide.pdf](https://github.com/DrTimothyAldenDavis/GraphBLAS/raw/stable/Doc/GraphBLAS_UserGuide.pdf)
 - **Source:** [https://github.com/python-graphblas/python-graphblas](https://github.com/python-graphblas/python-graphblas)
 - **Bug reports:** [https://github.com/python-graphblas/python-graphblas/issues](https://github.com/python-graphblas/python-graphblas/issues)
 - **Github discussions:** [https://github.com/python-graphblas/python-graphblas/discussions](https://github.com/python-graphblas/python-graphblas/discussions)
 - **Weekly community call:** [https://github.com/python-graphblas/python-graphblas/issues/247](https://github.com/python-graphblas/python-graphblas/issues/247)
 - **Chat via Discord:** [https://discord.com/invite/vur45CbwMz](https://discord.com/invite/vur45CbwMz) in the [#graphblas channel](https://discord.com/channels/786703927705862175/1024732940233605190)
 
+<p float="left">
+  <img src="docs/_static/img/draw-example.png" width="231" align="top" alt="Directed graph", title="Directed graph"/>
+  <img src="docs/_static/img/repr-matrix.png" width="231" align="top" alt="Adjacency matrix" title="Adjacency matrix"/>
+</p>
+
 ## Install
 Install the latest version of Python-graphblas via conda:
 ```
 $ conda install -c conda-forge python-graphblas
 ```
 or pip:
 ```
-$ pip install python-graphblas
+$ pip install python-graphblas[default]
 ```
 This will also install the [SuiteSparse:GraphBLAS](https://github.com/DrTimothyAldenDavis/GraphBLAS) compiled C library.
+We currently support the [GraphBLAS C API 2.0 specification](https://graphblas.org/docs/GraphBLAS_API_C_v2.0.0.pdf).
 
 ### Optional Dependencies
 
 The following are not required by python-graphblas, but may be needed for certain functionality to work.
 
 - `pandas` – required for nicer `__repr__`;
 - `matplotlib` – required for basic plotting of graphs;
-- `scipy` – used in io module to read/write `scipy.sparse` format;
+- `scipy` – used in `io` module to read/write `scipy.sparse` format;
 - `networkx` – used in `io` module to interface with `networkx` graphs;
 - `fast-matrix-market` - for faster read/write of Matrix Market files with `gb.io.mmread` and `gb.io.mmwrite`.
 
 ## Description
 Currently works with [SuiteSparse:GraphBLAS](https://github.com/DrTimothyAldenDavis/GraphBLAS), but the goal is to make it work with all implementations of the GraphBLAS spec.
 
-The approach taken with this library is to follow the C-API specification as closely as possible while making improvements
+The approach taken with this library is to follow the C-API 2.0 specification as closely as possible while making improvements
 allowed with the Python syntax. Because the spec always passes in the output object to be written to, we follow the same,
 which is very different from the way Python normally operates. In fact, many who are familiar with other Python data
 libraries (numpy, pandas, etc) will find it strange to not create new objects for every call.
 
 At the highest level, the goal is to separate output, mask, and accumulator on the left side of the assignment
 operator `=` and put the computation on the right side. Unfortunately, that approach doesn't always work very well
 with how Python handles assignment, so instead we (ab)use the left-shift `<<` notation to give the same flavor of
```

### Comparing `python-graphblas-2023.3.0/graphblas/__init__.py` & `python-graphblas-2023.5.0/graphblas/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -133,15 +133,29 @@
                 "graphblas initialized multiple times with different init parameters"
             )
         # Already initialized with these parameters; nothing more to do
         return
 
     backend = backend_arg
     if backend in {"suitesparse", "suitesparse-vanilla"}:
-        from suitesparse_graphblas import ffi, initialize, is_initialized, lib
+        try:
+            from suitesparse_graphblas import ffi, initialize, is_initialized, lib
+        except ImportError:  # pragma: no cover (import)
+            raise ImportError(
+                f"suitesparse_graphblas is required for {backend!r} backend. "
+                "It may be installed with pip or conda:\n\n"
+                "    $ pip install suitesparse-graphblas\n"
+                "    $ conda install -c conda-forge python-suitesparse-graphblas\n\n"
+                "SuiteSparse:GraphBLAS is the primary C implementation and backend of "
+                "python-graphblas and is what we recommend to most users. If you are "
+                "installing python-graphblas with pip, we recommend installing with one "
+                "of the following to automatically include suitespare-graphblas:\n\n"
+                "    $ pip install python-graphblas[suitesparse]\n"
+                "    $ pip install python-graphblas[default]"
+            ) from None
 
         if is_initialized():
             mode = ffi.new("int32_t*")
             if lib.GxB_Global_Option_get_INT32(lib.GxB_MODE, mode) != 0:
                 raise RuntimeError("Could not get GraphBLAS mode")  # pragma: no cover (safety)
             is_blocking = mode[0] == lib.GrB_BLOCKING
             if blocking is None:
```

### Comparing `python-graphblas-2023.3.0/graphblas/agg/__init__.py` & `python-graphblas-2023.5.0/graphblas/agg/__init__.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/binary/__init__.py` & `python-graphblas-2023.5.0/graphblas/binary/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 # All items are dynamically added by classes in operator.py
 # This module acts as a container of BinaryOp instances
+from ..core import _supports_udfs
+
 _delayed = {}
 _delayed_commutes_to = {
     "absfirst": "abssecond",
     "abssecond": "absfirst",
     "floordiv": "rfloordiv",
     "rfloordiv": "floordiv",
     "rpow": "pow",
 }
 _deprecated = {}
+_udfs = {
+    "absfirst",
+    "abssecond",
+    "binom",
+    "floordiv",
+    "isclose",
+    "rfloordiv",
+    "rpow",
+}
 
 
 def __dir__():
     return globals().keys() | _delayed.keys() | _deprecated.keys() | {"ss"}
 
 
 def __getattr__(key):
@@ -46,14 +57,19 @@
                 f'module {__name__!r} only has attribute "ss" when backend is "suitesparse"'
             )
         from importlib import import_module
 
         ss = import_module(".ss", __name__)
         globals()["ss"] = ss
         return ss
+    if not _supports_udfs and key in _udfs:
+        raise AttributeError(
+            f"module {__name__!r} unable to compile UDF for {key!r}; "
+            "install numba for UDF support"
+        )
     raise AttributeError(f"module {__name__!r} has no attribute {key!r}")
 
 
 from ..core import operator  # noqa: E402 isort:skip
 from . import numpy  # noqa: E402 isort:skip
 
 del operator
```

### Comparing `python-graphblas-2023.3.0/graphblas/binary/numpy.py` & `python-graphblas-2023.5.0/graphblas/binary/numpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 """
 import numpy as _np
 
 from .. import _STANDARD_OPERATOR_NAMES
 from .. import binary as _binary
 from .. import config as _config
+from ..core import _supports_udfs
 
 _delayed = {}
 _binary_names = {
     # Math operations
     "add",
     "subtract",
     "multiply",
@@ -126,26 +127,32 @@
 }
 # Don't commute: arctan2, around, copysign, divide, floor_divide, fmod, ldexp,
 # left_shift, mod, nextafter, power, remainder, right_shift, subtract, true_divide.
 # If desired, we could create r-versions of these so they can commute to something.
 
 
 def __dir__():
-    return globals().keys() | _delayed.keys() | _binary_names
+    if not _supports_udfs and not _config["mapnumpy"]:
+        # float_power is special: it's constructed from builtin operators
+        return globals().keys() | {"float_power"}  # FLAKY COVERAGE
+    attrs = _delayed.keys() | _binary_names
+    if not _supports_udfs:
+        attrs &= _numpy_to_graphblas.keys()
+    return attrs | globals().keys()
 
 
 def __getattr__(name):
     if name in _delayed:
         delayed_func, kwargs = _delayed.pop(name)
         rv = delayed_func(**kwargs)
         globals()[name] = rv
         return rv
     if name not in _binary_names:
         raise AttributeError(f"module {__name__!r} has no attribute {name!r}")
-    if _config.get("mapnumpy") and name in _numpy_to_graphblas:
+    if _config.get("mapnumpy") and name in _numpy_to_graphblas or name == "float_power":
         if name == "float_power":
             from ..core.operator import binary
             from ..dtypes import FP64
 
             new_op = binary.BinaryOp(f"numpy.{name}")
             builtin_op = _binary.pow
             for dtype in builtin_op.types:
@@ -162,14 +169,19 @@
                     orig_op.gb_obj,
                     orig_op.gb_name,
                 )
                 new_op._add(cur_op)
             globals()[name] = new_op
         else:
             globals()[name] = getattr(_binary, _numpy_to_graphblas[name])
+    elif not _supports_udfs:
+        raise AttributeError(
+            f"module {__name__!r} unable to compile UDF for {name!r}; "
+            "install numba for UDF support"
+        )
     else:
         numpy_func = getattr(_np, name)
 
         def func(x, y):  # pragma: no cover (numba)
             return numpy_func(x, y)
 
         _binary.register_new(f"numpy.{name}", func)
```

### Comparing `python-graphblas-2023.3.0/graphblas/core/automethods.py` & `python-graphblas-2023.5.0/graphblas/core/automethods.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/core/base.py` & `python-graphblas-2023.5.0/graphblas/core/base.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/core/descriptor.py` & `python-graphblas-2023.5.0/graphblas/core/descriptor.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/core/expr.py` & `python-graphblas-2023.5.0/graphblas/core/expr.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/core/formatting.py` & `python-graphblas-2023.5.0/graphblas/core/formatting.py`

 * *Files 0% similar despite different names*

```diff
@@ -876,14 +876,15 @@
     )
 
     computed = ""
     if config.get("autocompute"):
         computed = get_expr_result(expr, html=True)
         if "__EXPR__" in computed:
             return computed.replace("<tt>__EXPR__</tt>", topline)
+        # BRANCH NOT COVERED
 
     keys = []
     values = []
     if expr.output_type is Vector:
         keys.append("size")
         values.append(expr._size)
     elif expr.output_type is Matrix:
```

### Comparing `python-graphblas-2023.3.0/graphblas/core/infix.py` & `python-graphblas-2023.5.0/graphblas/core/infix.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/core/infixmethods.py` & `python-graphblas-2023.5.0/graphblas/core/infixmethods.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/core/mask.py` & `python-graphblas-2023.5.0/graphblas/core/mask.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/core/matrix.py` & `python-graphblas-2023.5.0/graphblas/core/matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from collections.abc import Sequence
 
 import numpy as np
 
 from .. import backend, binary, monoid, select, semiring
 from ..dtypes import _INDEX, FP64, INT64, lookup_dtype, unify
 from ..exceptions import DimensionMismatch, InvalidValue, NoValue, check_status
-from . import automethods, ffi, lib, utils
+from . import _supports_udfs, automethods, ffi, lib, utils
 from .base import BaseExpression, BaseType, _check_mask, call
 from .descriptor import lookup as descriptor_lookup
 from .expr import _ALL_INDICES, AmbiguousAssignOrExtract, IndexerResolver, Updater
 from .mask import Mask, StructuralMask, ValueMask
 from .operator import UNKNOWN_OPCLASS, find_opclass, get_semiring, get_typed_op, op_from_string
 from .scalar import (
     _COMPLETE,
@@ -29,15 +29,15 @@
     get_order,
     ints_to_numpy_buffer,
     normalize_values,
     output_type,
     values_to_numpy_buffer,
     wrapdoc,
 )
-from .vector import Vector, VectorExpression, VectorIndexExpr, _select_mask
+from .vector import Vector, VectorExpression, VectorIndexExpr, _isclose_recipe, _select_mask
 
 if backend == "suitesparse":
     from .ss.matrix import ss
 
 ffi_new = ffi.new
 
 _CSR_FORMAT = Scalar.from_value(
@@ -364,14 +364,16 @@
             return False
         if self._nrows != other._nrows:
             return False
         if self._ncols != other._ncols:
             return False
         if self._nvals != other._nvals:
             return False
+        if not _supports_udfs:
+            return _isclose_recipe(self, other, rel_tol, abs_tol, **opts)
 
         matches = self.ewise_mult(other, binary.isclose(rel_tol, abs_tol)).new(
             bool, name="M_isclose", **opts
         )
         # ewise_mult performs intersection, so nvals will indicate mismatched empty values
         if matches._nvals != self._nvals:
             return False
@@ -607,22 +609,23 @@
         if n == 0:
             return
 
         dup_op_given = dup_op is not None
         if not dup_op_given:
             if not self.dtype._is_udt:
                 dup_op = binary.plus
-            else:
+            elif backend != "suitesparse":
                 dup_op = binary.any
-        # SS:SuiteSparse-specific: we could use NULL for dup_op
-        dup_op = get_typed_op(dup_op, self.dtype, kind="binary")
-        if dup_op.opclass == "Monoid":
-            dup_op = dup_op.binaryop
-        else:
-            self._expect_op(dup_op, "BinaryOp", within="build", argname="dup_op")
+            # SS:SuiteSparse-specific: we use NULL for dup_op
+        if dup_op is not None:
+            dup_op = get_typed_op(dup_op, self.dtype, kind="binary")
+            if dup_op.opclass == "Monoid":
+                dup_op = dup_op.binaryop
+            else:
+                self._expect_op(dup_op, "BinaryOp", within="build", argname="dup_op")
 
         rows = _CArray(rows)
         columns = _CArray(columns)
         values = _CArray(values, self.dtype)
         dtype_name = "UDT" if self.dtype._is_udt else self.dtype.name
         call(
             f"GrB_Matrix_build_{dtype_name}",
@@ -1580,15 +1583,15 @@
         iter_values = itertools.chain.from_iterable(v.values() for v in dicts)
         if dtype is None:
             values, dtype = values_to_numpy_buffer(list(iter_values), subarray_after=1)
         else:
             # If we know the dtype, then using `np.fromiter` is much faster
             dtype = lookup_dtype(dtype)
             if dtype.np_type.subdtype is not None and np.__version__[:5] in {"1.21.", "1.22."}:
-                values, dtype = values_to_numpy_buffer(list(iter_values), dtype)
+                values, dtype = values_to_numpy_buffer(list(iter_values), dtype)  # FLAKY COVERAGE
             else:
                 values = np.fromiter(iter_values, dtype.np_type)
         return getattr(cls, methodname)(
             *args, indptr, col_indices, values, dtype, nrows=nrows, ncols=ncols, name=name
         )
 
     def _to_csx(self, fmt, dtype, sort):
@@ -2462,14 +2465,15 @@
                     extra_message="Literal scalars also accepted.",
                     op=op,
                 )
         op = get_typed_op(op, self.dtype, thunk.dtype, is_right_scalar=True, kind="select")
         self._expect_op(op, ("SelectOp", "IndexUnaryOp"), within=method_name, argname="op")
         if thunk._is_cscalar:
             if thunk.dtype._is_udt:
+                # NOT COVERED
                 dtype_name = "UDT"
                 thunk = _Pointer(thunk)
             else:
                 dtype_name = thunk.dtype.name
             cfunc_name = f"GrB_Matrix_select_{dtype_name}"
         else:
             cfunc_name = "GrB_Matrix_select_Scalar"
```

### Comparing `python-graphblas-2023.3.0/graphblas/core/operator/__init__.py` & `python-graphblas-2023.5.0/graphblas/core/operator/__init__.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/core/operator/agg.py` & `python-graphblas-2023.5.0/graphblas/core/operator/agg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from functools import partial
 from operator import getitem
 
 import numpy as np
 
 from ... import agg, backend, binary, monoid, semiring, unary
 from ...dtypes import INT64, lookup_dtype
+from .. import _supports_udfs
 from ..utils import output_type
 
 
 def _get_types(ops, initdtype):
     """Determine the input and output types of an aggregator based on a list of ops."""
     if initdtype is None:
         prev = dict(ops[0].types)
@@ -34,28 +35,30 @@
         name,
         *,
         initval=None,
         monoid=None,
         semiring=None,
         switch=False,
         semiring2=None,
+        applybegin=None,
         finalize=None,
         composite=None,
         custom=None,
         types=None,
         any_dtype=None,
     ):
         self.name = name
         self._initval_orig = initval
         self._initval = False if initval is None else initval
         self._initdtype = lookup_dtype(type(self._initval), self._initval)
         self._monoid = monoid
         self._semiring = semiring
         self._semiring2 = semiring2
         self._switch = switch
+        self._applybegin = applybegin
         self._finalize = finalize
         self._composite = composite
         self._custom = custom
         if types is None:
             if monoid is not None:
                 types = [monoid]
             elif semiring is not None:
@@ -148,30 +151,32 @@
             self.return_type = agg._any_dtype
 
     def __repr__(self):
         return f"agg.{self.name}[{self.type}]"
 
     def _new(self, updater, expr, *, in_composite=False):
         agg = self.parent
+        opts = updater.opts
         if agg._monoid is not None:
             x = expr.args[0]
+            if agg._applybegin is not None:  # pragma: no cover (unused)
+                x = agg._applybegin(x).new(**opts)
             method = getattr(x, expr.method_name)
             if expr.output_type.__name__ == "Scalar":
                 expr = method(agg._monoid[self.type], allow_empty=not expr._is_cscalar)
             else:
                 expr = method(agg._monoid[self.type])
             updater << expr
             if in_composite:
                 parent = updater.parent
                 if not parent._is_scalar:
                     return parent
                 return parent._as_vector()
             return
 
-        opts = updater.opts
         if agg._composite is not None:
             # Masks are applied throughout the aggregation, including composite aggregations.
             # Aggregations done while `in_composite is True` should return the updater parent
             # if the result is not a Scalar.  If the result is a Scalar, then there can be no
             # output mask, and a Vector of size 1 should be returned instead.
             results = []
             mask = updater.kwargs.get("mask")
@@ -199,14 +204,16 @@
         if agg._custom is not None:
             return agg._custom(self, updater, expr, opts, in_composite=in_composite)
 
         semiring = get_typed_op(agg._semiring, self.type, agg._initdtype)
         if expr.cfunc_name == "GrB_Matrix_reduce_Aggregator":
             # Matrix -> Vector
             A = expr.args[0]
+            if agg._applybegin is not None:
+                A = agg._applybegin(A).new(**opts)
             orig_updater = updater
             if agg._finalize is not None:
                 step1 = expr.construct_output(semiring.return_type)
                 updater = step1(mask=updater.kwargs.get("mask"), **opts)
             if expr.method_name == "reduce_columnwise":
                 A = A.T
             size = A._ncols
@@ -219,14 +226,16 @@
             if agg._finalize is not None:
                 orig_updater << agg._finalize[semiring.return_type](step1)
             if in_composite:
                 return orig_updater.parent
         elif expr.cfunc_name.startswith("GrB_Vector_reduce"):
             # Vector -> Scalar
             v = expr.args[0]
+            if agg._applybegin is not None:
+                v = agg._applybegin(v).new(**opts)
             step1 = expr._new_vector(semiring.return_type, size=1)
             init = expr._new_matrix(agg._initdtype, nrows=v._size, ncols=1)
             init(**opts)[...] = agg._initval  # O(1) dense column vector in SuiteSparse 5
             if agg._switch:
                 step1(**opts) << semiring(init.T @ v)
             else:
                 step1(**opts) << semiring(v @ init)
@@ -238,14 +247,16 @@
                     step1 = finalize(step1).new(finalize.return_type, **opts)
             if in_composite:
                 return step1
             updater << step1[0]
         elif expr.cfunc_name.startswith("GrB_Matrix_reduce"):
             # Matrix -> Scalar
             A = expr.args[0]
+            if agg._applybegin is not None:
+                A = agg._applybegin(A).new(**opts)
             # We need to compute in two steps: Matrix -> Vector -> Scalar.
             # This has not been benchmarked or optimized.
             # We may be able to intelligently choose the faster path.
             init1 = expr._new_vector(agg._initdtype, size=A._ncols)
             init1(**opts)[...] = agg._initval  # O(1) dense vector in SuiteSparse 5
             step1 = expr._new_vector(semiring.return_type, size=A._nrows)
             if agg._switch:
@@ -335,19 +346,29 @@
     finalize=unary.log2,
 )
 # Alternatives
 # logaddexp = Aggregator('logaddexp', monoid=semiring.numpy.logaddexp)
 # logaddexp2 = Aggregator('logaddexp2', monoid=semiring.numpy.logaddexp2)
 # hypot as monoid doesn't work if single negative element!
 # hypot = Aggregator('hypot', monoid=semiring.numpy.hypot)
+# hypot = Aggregator('hypot', applybegin=unary.abs, monoid=semiring.numpy.hypot)
 
 agg.L0norm = agg.count_nonzero
-agg.L1norm = Aggregator("L1norm", semiring="plus_absfirst", semiring2=semiring.plus_first)
 agg.L2norm = agg.hypot
-agg.Linfnorm = Aggregator("Linfnorm", semiring="max_absfirst", semiring2=semiring.max_first)
+if _supports_udfs:
+    agg.L1norm = Aggregator("L1norm", semiring="plus_absfirst", semiring2=semiring.plus_first)
+    agg.Linfnorm = Aggregator("Linfnorm", semiring="max_absfirst", semiring2=semiring.max_first)
+else:
+    # Are these always better?
+    agg.L1norm = Aggregator(
+        "L1norm", applybegin=unary.abs, semiring=semiring.plus_first, semiring2=semiring.plus_first
+    )
+    agg.Linfnorm = Aggregator(
+        "Linfnorm", applybegin=unary.abs, semiring=semiring.max_first, semiring2=semiring.max_first
+    )
 
 
 # Composite
 def _mean_finalize(c, x, opts):
     return binary.truediv(x & c)
```

### Comparing `python-graphblas-2023.3.0/graphblas/core/operator/base.py` & `python-graphblas-2023.5.0/graphblas/core/operator/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-from functools import lru_cache, reduce
-from operator import getitem, mul
+from functools import lru_cache
+from operator import getitem
 from types import BuiltinFunctionType, ModuleType
 
-import numba
-import numpy as np
-
 from ... import _STANDARD_OPERATOR_NAMES, backend, op
 from ...dtypes import BOOL, INT8, UINT64, _supports_complex, lookup_dtype
-from .. import lib
+from .. import _has_numba, _supports_udfs, lib
 from ..expr import InfixExprBase
 from ..utils import output_type
 
+if _has_numba:
+    import numba
+    from numba import NumbaError
+else:
+    NumbaError = TypeError
+
 UNKNOWN_OPCLASS = "UnknownOpClass"
 
 # These now live as e.g. `gb.unary.ss.positioni`
 # Deprecations such as `gb.unary.positioni` will be removed in 2023.9.0 or later.
 _SS_OPERATORS = {
     # unary
     "erf",  # scipy.special.erf
@@ -154,104 +157,77 @@
         "Expected an infix expression or an apply with a Vector or Matrix and a scalar:\n"
         f"    - {op!r}(A & B)\n"
         f"    - {op!r}(A, 1)\n"
         f"    - {op!r}(1, A)"
     )
 
 
-_udt_mask_cache = {}
+if _has_numba:
 
-
-def _udt_mask(dtype):
-    """Create mask to determine which bytes of UDTs to use for equality check."""
-    if dtype in _udt_mask_cache:
-        return _udt_mask_cache[dtype]
-    if dtype.subdtype is not None:
-        mask = _udt_mask(dtype.subdtype[0])
-        N = reduce(mul, dtype.subdtype[1])
-        rv = np.concatenate([mask] * N)
-    elif dtype.names is not None:
-        prev_offset = mask = None
-        masks = []
-        for name in dtype.names:
-            dtype2, offset = dtype.fields[name]
-            if mask is not None:
-                masks.append(np.pad(mask, (0, offset - prev_offset - mask.size)))
-            mask = _udt_mask(dtype2)
-            prev_offset = offset
-        masks.append(np.pad(mask, (0, dtype.itemsize - prev_offset - mask.size)))
-        rv = np.concatenate(masks)
-    else:
-        rv = np.ones(dtype.itemsize, dtype=bool)
-    # assert rv.size == dtype.itemsize
-    _udt_mask_cache[dtype] = rv
-    return rv
-
-
-def _get_udt_wrapper(numba_func, return_type, dtype, dtype2=None, *, include_indexes=False):
-    ztype = INT8 if return_type == BOOL else return_type
-    xtype = INT8 if dtype == BOOL else dtype
-    nt = numba.types
-    wrapper_args = [nt.CPointer(ztype.numba_type), nt.CPointer(xtype.numba_type)]
-    if include_indexes:
-        wrapper_args.extend([UINT64.numba_type, UINT64.numba_type])
-    if dtype2 is not None:
-        ytype = INT8 if dtype2 == BOOL else dtype2
-        wrapper_args.append(nt.CPointer(ytype.numba_type))
-    wrapper_sig = nt.void(*wrapper_args)
-
-    zarray = xarray = yarray = BL = BR = yarg = yname = rcidx = ""
-    if return_type._is_udt:
-        if return_type.np_type.subdtype is None:
-            zarray = "    z = numba.carray(z_ptr, 1)\n"
-            zname = "z[0]"
+    def _get_udt_wrapper(numba_func, return_type, dtype, dtype2=None, *, include_indexes=False):
+        ztype = INT8 if return_type == BOOL else return_type
+        xtype = INT8 if dtype == BOOL else dtype
+        nt = numba.types
+        wrapper_args = [nt.CPointer(ztype.numba_type), nt.CPointer(xtype.numba_type)]
+        if include_indexes:
+            wrapper_args.extend([UINT64.numba_type, UINT64.numba_type])
+        if dtype2 is not None:
+            ytype = INT8 if dtype2 == BOOL else dtype2
+            wrapper_args.append(nt.CPointer(ytype.numba_type))
+        wrapper_sig = nt.void(*wrapper_args)
+
+        zarray = xarray = yarray = BL = BR = yarg = yname = rcidx = ""
+        if return_type._is_udt:
+            if return_type.np_type.subdtype is None:
+                zarray = "    z = numba.carray(z_ptr, 1)\n"
+                zname = "z[0]"
+            else:
+                zname = "z_ptr[0]"
+                BR = "[0]"
         else:
             zname = "z_ptr[0]"
-            BR = "[0]"
-    else:
-        zname = "z_ptr[0]"
-        if return_type == BOOL:
-            BL = "bool("
-            BR = ")"
-
-    if dtype._is_udt:
-        if dtype.np_type.subdtype is None:
-            xarray = "    x = numba.carray(x_ptr, 1)\n"
-            xname = "x[0]"
+            if return_type == BOOL:
+                BL = "bool("
+                BR = ")"
+
+        if dtype._is_udt:
+            if dtype.np_type.subdtype is None:
+                xarray = "    x = numba.carray(x_ptr, 1)\n"
+                xname = "x[0]"
+            else:
+                xname = "x_ptr"
+        elif dtype == BOOL:
+            xname = "bool(x_ptr[0])"
         else:
-            xname = "x_ptr"
-    elif dtype == BOOL:
-        xname = "bool(x_ptr[0])"
-    else:
-        xname = "x_ptr[0]"
+            xname = "x_ptr[0]"
 
-    if dtype2 is not None:
-        yarg = ", y_ptr"
-        if dtype2._is_udt:
-            if dtype2.np_type.subdtype is None:
-                yarray = "    y = numba.carray(y_ptr, 1)\n"
-                yname = ", y[0]"
+        if dtype2 is not None:
+            yarg = ", y_ptr"
+            if dtype2._is_udt:
+                if dtype2.np_type.subdtype is None:
+                    yarray = "    y = numba.carray(y_ptr, 1)\n"
+                    yname = ", y[0]"
+                else:
+                    yname = ", y_ptr"
+            elif dtype2 == BOOL:
+                yname = ", bool(y_ptr[0])"
             else:
-                yname = ", y_ptr"
-        elif dtype2 == BOOL:
-            yname = ", bool(y_ptr[0])"
-        else:
-            yname = ", y_ptr[0]"
+                yname = ", y_ptr[0]"
 
-    if include_indexes:
-        rcidx = ", row, col"
+        if include_indexes:
+            rcidx = ", row, col"
 
-    d = {"numba": numba, "numba_func": numba_func}
-    text = (
-        f"def wrapper(z_ptr, x_ptr{rcidx}{yarg}):\n"
-        f"{zarray}{xarray}{yarray}"
-        f"    {zname} = {BL}numba_func({xname}{rcidx}{yname}){BR}\n"
-    )
-    exec(text, d)  # pylint: disable=exec-used
-    return d["wrapper"], wrapper_sig
+        d = {"numba": numba, "numba_func": numba_func}
+        text = (
+            f"def wrapper(z_ptr, x_ptr{rcidx}{yarg}):\n"
+            f"{zarray}{xarray}{yarray}"
+            f"    {zname} = {BL}numba_func({xname}{rcidx}{yname}){BR}\n"
+        )
+        exec(text, d)  # pylint: disable=exec-used
+        return d["wrapper"], wrapper_sig
 
 
 class TypedOpBase:
     __slots__ = (
         "parent",
         "name",
         "type",
@@ -356,14 +332,16 @@
             if type_ not in self._typed_ops:
                 if self._udt_types is None:
                     if self.is_positional:
                         return self._typed_ops[UINT64]
                     raise KeyError(f"{self.name} does not work with {type_}")
             else:
                 return self._typed_ops[type_]
+        if not _supports_udfs:
+            raise KeyError(f"{self.name} does not work with {type_}")
         # This is a UDT or is able to operate on UDTs such as `first` any `any`
         dtype = lookup_dtype(type_)
         return self._compile_udt(dtype, dtype)
 
     def _add(self, op):
         self._typed_ops[op.type] = op
         self.types[op.type] = op.return_type
@@ -372,15 +350,15 @@
         type_ = lookup_dtype(type_)
         del self._typed_ops[type_]
         del self.types[type_]
 
     def __contains__(self, type_):
         try:
             self[type_]
-        except (TypeError, KeyError, numba.NumbaError):
+        except (TypeError, KeyError, NumbaError):
             return False
         return True
 
     @classmethod
     def _remove_nesting(cls, funcname, *, module=None, modname=None, strict=True):
         if module is None:
             module = cls._module
@@ -483,15 +461,15 @@
                         gb_obj = getattr(lib, varname)
                         # Determine return type
                         if return_prefix == "BOOL":
                             return_type = BOOL
                             if type_ is None:
                                 type_ = BOOL
                         else:
-                            if type_ is None:  # pragma: no cover
+                            if type_ is None:  # pragma: no cover (safety)
                                 raise TypeError(f"Unable to determine return type for {varname}")
                             if return_prefix is None:
                                 return_type = type_
                             else:
                                 # Grab the number of bits from type_
                                 num_bits = type_[-2:]
                                 if num_bits not in {"32", "64"}:  # pragma: no cover (safety)
@@ -509,14 +487,21 @@
 
     @classmethod
     def _deserialize(cls, name, *args):
         if (rv := cls._find(name)) is not None:
             return rv  # Should we verify this is what the user expects?
         return cls.register_new(name, *args)
 
+    @classmethod
+    def _check_supports_udf(cls, method_name):
+        if not _supports_udfs:
+            raise RuntimeError(
+                f"{cls.__name__}.{method_name}(...) unavailable; install numba for UDF support"
+            )
+
 
 _builtin_to_op = {}  # Populated in .utils
 
 
 def find_opclass(gb_op):
     if isinstance(gb_op, OpBase):
         opclass = type(gb_op).__name__
```

### Comparing `python-graphblas-2023.3.0/graphblas/core/operator/binary.py` & `python-graphblas-2023.5.0/graphblas/core/operator/binary.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import inspect
 import re
-from functools import lru_cache
+from functools import lru_cache, reduce
+from operator import mul
 from types import FunctionType
 
-import numba
 import numpy as np
 
 from ... import _STANDARD_OPERATOR_NAMES, backend, binary, monoid, op
 from ...dtypes import (
     BOOL,
     FP32,
     FP64,
@@ -20,33 +20,63 @@
     UINT32,
     UINT64,
     _sample_values,
     _supports_complex,
     lookup_dtype,
 )
 from ...exceptions import UdfParseError, check_status_carg
-from .. import ffi, lib
+from .. import _has_numba, _supports_udfs, ffi, lib
 from ..expr import InfixExprBase
 from .base import (
     _SS_OPERATORS,
     OpBase,
     ParameterizedUdf,
     TypedOpBase,
     _call_op,
     _deserialize_parameterized,
-    _get_udt_wrapper,
     _hasop,
-    _udt_mask,
 )
 
+if _has_numba:
+    import numba
+
+    from .base import _get_udt_wrapper
 if _supports_complex:
     from ...dtypes import FC32, FC64
 
 ffi_new = ffi.new
 
+if _has_numba:
+    _udt_mask_cache = {}
+
+    def _udt_mask(dtype):
+        """Create mask to determine which bytes of UDTs to use for equality check."""
+        if dtype in _udt_mask_cache:
+            return _udt_mask_cache[dtype]
+        if dtype.subdtype is not None:
+            mask = _udt_mask(dtype.subdtype[0])
+            N = reduce(mul, dtype.subdtype[1])
+            rv = np.concatenate([mask] * N)
+        elif dtype.names is not None:
+            prev_offset = mask = None
+            masks = []
+            for name in dtype.names:
+                dtype2, offset = dtype.fields[name]
+                if mask is not None:
+                    masks.append(np.pad(mask, (0, offset - prev_offset - mask.size)))
+                mask = _udt_mask(dtype2)
+                prev_offset = offset
+            masks.append(np.pad(mask, (0, dtype.itemsize - prev_offset - mask.size)))
+            rv = np.concatenate(masks)
+        else:
+            rv = np.ones(dtype.itemsize, dtype=bool)
+        # assert rv.size == dtype.itemsize
+        _udt_mask_cache[dtype] = rv
+        return rv
+
 
 class TypedBuiltinBinaryOp(TypedOpBase):
     __slots__ = ()
     opclass = "BinaryOp"
 
     def __call__(self, left, right=None, *, left_default=None, right_default=None):
         if left_default is not None or right_default is not None:
@@ -596,35 +626,106 @@
         return op
 
     @classmethod
     def register_anonymous(cls, func, name=None, *, parameterized=False, is_udt=False):
         """Register a BinaryOp without registering it in the ``graphblas.binary`` namespace.
 
         Because it is not registered in the namespace, the name is optional.
+
+        Parameters
+        ----------
+        func : FunctionType
+            The function to compile. For all current backends, this must be able
+            to be compiled with ``numba.njit``.
+            ``func`` takes two input parameters of any dtype and returns any dtype.
+        name : str, optional
+            The name of the operator. This *does not* show up as ``gb.binary.{name}``.
+        parameterized : bool, default False
+            When True, create a parameterized user-defined operator, which means
+            additional parameters can be "baked into" the operator when used.
+            For example, ``gb.binary.isclose`` is a parameterized function that
+            optionally accepts ``rel_tol`` and ``abs_tol`` parameters, and it
+            can be used as: ``A.ewise_mult(B, gb.binary.isclose(rel_tol=1e-5))``.
+            When creating a parameterized user-defined operator, the ``func``
+            parameter must be a callable that *returns* a function that will
+            then get compiled.
+        is_udt : bool, default False
+            Whether the operator is intended to operate on user-defined types.
+            If True, then the function will not be automatically compiled for
+            builtin types, and it will be compiled "just in time" when used.
+            Setting ``is_udt=True`` is also helpful when the left and right
+            dtypes need to be different.
+
+        Returns
+        -------
+        BinaryOp or ParameterizedBinaryOp
         """
+        cls._check_supports_udf("register_anonymous")
         if parameterized:
             return ParameterizedBinaryOp(name, func, anonymous=True, is_udt=is_udt)
         return cls._build(name, func, anonymous=True, is_udt=is_udt)
 
     @classmethod
     def register_new(cls, name, func, *, parameterized=False, is_udt=False, lazy=False):
-        """Register a BinaryOp. The name will be used to identify the BinaryOp in the
-        ``graphblas.binary`` namespace.
+        """Register a new BinaryOp and save it to ``graphblas.binary`` namespace.
 
-            >>> def max_zero(x, y):
-                    r = 0
-                    if x > r:
-                        r = x
-                    if y > r:
-                        r = y
-                    return r
-            >>> gb.core.operator.BinaryOp.register_new("max_zero", max_zero)
-            >>> dir(gb.binary)
-            [..., 'max_zero', ...]
+        Parameters
+        ----------
+        name : str
+            The name of the operator. This will show up as ``gb.binary.{name}``.
+            The name may contain periods, ".", which will result in nested objects
+            such as ``gb.binary.x.y.z`` for name ``"x.y.z"``.
+        func : FunctionType
+            The function to compile. For all current backends, this must be able
+            to be compiled with ``numba.njit``.
+            ``func`` takes two input parameters of any dtype and returns any dtype.
+        parameterized : bool, default False
+            When True, create a parameterized user-defined operator, which means
+            additional parameters can be "baked into" the operator when used.
+            For example, ``gb.binary.isclose`` is a parameterized function that
+            optionally accepts ``rel_tol`` and ``abs_tol`` parameters, and it
+            can be used as: ``A.ewise_mult(B, gb.binary.isclose(rel_tol=1e-5))``.
+            When creating a parameterized user-defined operator, the ``func``
+            parameter must be a callable that *returns* a function that will
+            then get compiled. See the ``user_isclose`` example below.
+        is_udt : bool, default False
+            Whether the operator is intended to operate on user-defined types.
+            If True, then the function will not be automatically compiled for
+            builtin types, and it will be compiled "just in time" when used.
+            Setting ``is_udt=True`` is also helpful when the left and right
+            dtypes need to be different.
+        lazy : bool, default False
+            If False (the default), then the function will be automatically
+            compiled for builtin types (unless ``is_udt`` is True).
+            Compiling functions can be slow, however, so you may want to
+            delay compilation and only compile when the operator is used,
+            which is done by setting ``lazy=True``.
+
+        Examples
+        --------
+        >>> def max_zero(x, y):
+                r = 0
+                if x > r:
+                    r = x
+                if y > r:
+                    r = y
+                return r
+        >>> gb.core.operator.BinaryOp.register_new("max_zero", max_zero)
+        >>> dir(gb.binary)
+        [..., 'max_zero', ...]
+
+        This is how ``gb.binary.isclose`` is defined:
+
+        >>> def user_isclose(rel_tol=1e-7, abs_tol=0.0):
+        >>>     def inner(x, y):
+        >>>         return x == y or abs(x - y) <= max(rel_tol * max(abs(x), abs(y)), abs_tol)
+        >>>     return inner
+        >>> gb.binary.register_new("user_isclose", user_isclose, parameterized=True)
         """
+        cls._check_supports_udf("register_new")
         module, funcname = cls._remove_nesting(name)
         if lazy:
             module._delayed[funcname] = (
                 cls.register_new,
                 {"name": name, "func": func, "parameterized": parameterized},
             )
         elif parameterized:
@@ -677,29 +778,30 @@
                     new_op.name,
                     dtype,
                     builtin_op.types[orig_dtype],
                     orig_op.gb_obj,
                     orig_op.gb_name,
                 )
                 new_op._add(cur_op)
-        # Add floordiv
-        # cdiv truncates towards 0, while floordiv truncates towards -inf
-        BinaryOp.register_new("floordiv", _floordiv, lazy=True)  # cast to integer
-        BinaryOp.register_new("rfloordiv", _rfloordiv, lazy=True)  # cast to integer
-
-        # For aggregators
-        BinaryOp.register_new("absfirst", _absfirst, lazy=True)
-        BinaryOp.register_new("abssecond", _abssecond, lazy=True)
-        BinaryOp.register_new("rpow", _rpow, lazy=True)
-
-        # For algorithms
-        binary._delayed["binom"] = (_register_binom, {})  # Lazy with custom creation
-        op._delayed["binom"] = binary
+        if _supports_udfs:
+            # Add floordiv
+            # cdiv truncates towards 0, while floordiv truncates towards -inf
+            BinaryOp.register_new("floordiv", _floordiv, lazy=True)  # cast to integer
+            BinaryOp.register_new("rfloordiv", _rfloordiv, lazy=True)  # cast to integer
+
+            # For aggregators
+            BinaryOp.register_new("absfirst", _absfirst, lazy=True)
+            BinaryOp.register_new("abssecond", _abssecond, lazy=True)
+            BinaryOp.register_new("rpow", _rpow, lazy=True)
+
+            # For algorithms
+            binary._delayed["binom"] = (_register_binom, {})  # Lazy with custom creation
+            op._delayed["binom"] = binary
 
-        BinaryOp.register_new("isclose", _isclose, parameterized=True)
+            BinaryOp.register_new("isclose", _isclose, parameterized=True)
 
         # Update type information with sane coercion
         position_dtypes = [
             BOOL,
             FP32,
             FP64,
             INT8,
@@ -773,22 +875,31 @@
             if backend == "suitesparse" and right_name in _SS_OPERATORS:
                 left._commutes_to = f"ss.{right_name}"
             else:
                 left._commutes_to = right_name
             if right_name not in binary._delayed:
                 if right_name in _SS_OPERATORS:
                     right = binary._deprecated[right_name]
-                else:
+                elif _supports_udfs:
                     right = getattr(binary, right_name)
+                else:
+                    right = getattr(binary, right_name, None)
+                    if right is None:
+                        continue
                 if backend == "suitesparse" and left_name in _SS_OPERATORS:
                     right._commutes_to = f"ss.{left_name}"
                 else:
                     right._commutes_to = left_name
         for name in cls._commutative:
-            cur_op = getattr(binary, name)
+            if _supports_udfs:
+                cur_op = getattr(binary, name)
+            else:
+                cur_op = getattr(binary, name, None)
+                if cur_op is None:
+                    continue
             cur_op._commutes_to = name
         for left_name, right_name in cls._commutes_to_in_semiring.items():
             if left_name in _SS_OPERATORS:
                 left = binary._deprecated[left_name]
             else:  # pragma: no cover (safety)
                 left = getattr(binary, left_name)
             if right_name in _SS_OPERATORS:
@@ -801,15 +912,18 @@
         for binop, func in [
             (binary.first, _first),
             (binary.second, _second),
             (binary.pair, _pair),
             (binary.any, _first),
         ]:
             binop.orig_func = func
-            binop._numba_func = numba.njit(func)
+            if _has_numba:
+                binop._numba_func = numba.njit(func)
+            else:
+                binop._numba_func = None
             binop._udt_types = {}
             binop._udt_ops = {}
         binary.any._numba_func = binary.first._numba_func
         binary.eq._udt_types = {}
         binary.eq._udt_ops = {}
         binary.ne._udt_types = {}
         binary.ne._udt_ops = {}
```

### Comparing `python-graphblas-2023.3.0/graphblas/core/operator/indexunary.py` & `python-graphblas-2023.5.0/graphblas/core/operator/indexunary.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 import inspect
 import re
 from types import FunctionType
 
-import numba
-
 from ... import _STANDARD_OPERATOR_NAMES, indexunary, select
 from ...dtypes import BOOL, FP64, INT8, INT64, UINT64, _sample_values, lookup_dtype
 from ...exceptions import UdfParseError, check_status_carg
-from .. import ffi, lib
-from .base import (
-    OpBase,
-    ParameterizedUdf,
-    TypedOpBase,
-    _call_op,
-    _deserialize_parameterized,
-    _get_udt_wrapper,
-)
+from .. import _has_numba, ffi, lib
+from .base import OpBase, ParameterizedUdf, TypedOpBase, _call_op, _deserialize_parameterized
+
+if _has_numba:
+    import numba
 
+    from .base import _get_udt_wrapper
 ffi_new = ffi.new
 
 
 class TypedBuiltinIndexUnaryOp(TypedOpBase):
     __slots__ = ()
     opclass = "IndexUnaryOp"
 
@@ -61,21 +56,23 @@
 
     def _call(self, *args, **kwargs):
         indexunary = self.func(*args, **kwargs)
         indexunary._parameterized_info = (self, args, kwargs)
         return IndexUnaryOp.register_anonymous(indexunary, self.name, is_udt=self._is_udt)
 
     def __reduce__(self):
+        # NOT COVERED
         name = f"indexunary.{self.name}"
         if not self._anonymous and name in _STANDARD_OPERATOR_NAMES:
             return name
         return (self._deserialize, (self.name, self.func, self._anonymous))
 
     @staticmethod
     def _deserialize(name, func, anonymous):
+        # NOT COVERED
         if anonymous:
             return IndexUnaryOp.register_anonymous(func, name, parameterized=True)
         if (rv := IndexUnaryOp._find(name)) is not None:
             return rv
         return IndexUnaryOp.register_new(name, func, parameterized=True)
 
 
@@ -240,35 +237,107 @@
         )
         self._udt_types[dtypes] = ret_type
         self._udt_ops[dtypes] = op
         return op
 
     @classmethod
     def register_anonymous(cls, func, name=None, *, parameterized=False, is_udt=False):
-        """Register an IndexUnaryOp without registering it in the
-        ``graphblas.indexunary`` namespace.
+        """Register a IndexUnary without registering it in the ``graphblas.indexunary`` namespace.
 
         Because it is not registered in the namespace, the name is optional.
+
+        Parameters
+        ----------
+        func : FunctionType
+            The function to compile. For all current backends, this must be able
+            to be compiled with ``numba.njit``.
+            ``func`` takes four input parameters--any dtype, int64, int64,
+            any dtype and returns any dtype. The first argument (any dtype) is
+            the value of the input Matrix or Vector, the second argument (int64)
+            is the row index of the Matrix or the index of the Vector, the third
+            argument (int64) is the column index of the Matrix or 0 for a Vector,
+            and the fourth argument (any dtype) is the value of the input Scalar.
+        name : str, optional
+            The name of the operator. This *does not* show up as ``gb.indexunary.{name}``.
+        parameterized : bool, default False
+            When True, create a parameterized user-defined operator, which means
+            additional parameters can be "baked into" the operator when used.
+            For example, ``gb.binary.isclose`` is a parameterized BinaryOp that
+            optionally accepts ``rel_tol`` and ``abs_tol`` parameters, and it
+            can be used as: ``A.ewise_mult(B, gb.binary.isclose(rel_tol=1e-5))``.
+            When creating a parameterized user-defined operator, the ``func``
+            parameter must be a callable that *returns* a function that will
+            then get compiled.
+        is_udt : bool, default False
+            Whether the operator is intended to operate on user-defined types.
+            If True, then the function will not be automatically compiled for
+            builtin types, and it will be compiled "just in time" when used.
+            Setting ``is_udt=True`` is also helpful when the left and right
+            dtypes need to be different.
+
+        Returns
+        -------
+        return IndexUnaryOp or ParameterizedIndexUnaryOp
         """
+        cls._check_supports_udf("register_anonymous")
         if parameterized:
             return ParameterizedIndexUnaryOp(name, func, anonymous=True, is_udt=is_udt)
         return cls._build(name, func, anonymous=True, is_udt=is_udt)
 
     @classmethod
     def register_new(cls, name, func, *, parameterized=False, is_udt=False, lazy=False):
-        """Register an IndexUnaryOp. The name will be used to identify the IndexUnaryOp in the
-        ``graphblas.indexunary`` namespace.
+        """Register a new IndexUnaryOp and save it to ``graphblas.indexunary`` namespace.
 
         If the return type is Boolean, the function will also be registered as a SelectOp
-        with the same name.
+        (and saved to ``grablas.select`` namespace) with the same name.
 
-            >>> gb.indexunary.register_new("row_mod", lambda x, i, j, thunk: i % max(thunk, 2))
-            >>> dir(gb.indexunary)
-            [..., 'row_mod', ...]
+        Parameters
+        ----------
+        name : str
+            The name of the operator. This will show up as ``gb.indexunary.{name}``.
+            The name may contain periods, ".", which will result in nested objects
+            such as ``gb.indexunary.x.y.z`` for name ``"x.y.z"``.
+        func : FunctionType
+            The function to compile. For all current backends, this must be able
+            to be compiled with ``numba.njit``.
+            ``func`` takes four input parameters--any dtype, int64, int64,
+            any dtype and returns any dtype. The first argument (any dtype) is
+            the value of the input Matrix or Vector, the second argument (int64)
+            is the row index of the Matrix or the index of the Vector, the third
+            argument (int64) is the column index of the Matrix or 0 for a Vector,
+            and the fourth argument (any dtype) is the value of the input Scalar.
+        parameterized : bool, default False
+            When True, create a parameterized user-defined operator, which means
+            additional parameters can be "baked into" the operator when used.
+            For example, ``gb.binary.isclose`` is a parameterized BinaryOp that
+            optionally accepts ``rel_tol`` and ``abs_tol`` parameters, and it
+            can be used as: ``A.ewise_mult(B, gb.binary.isclose(rel_tol=1e-5))``.
+            When creating a parameterized user-defined operator, the ``func``
+            parameter must be a callable that *returns* a function that will
+            then get compiled.
+        is_udt : bool, default False
+            Whether the operator is intended to operate on user-defined types.
+            If True, then the function will not be automatically compiled for
+            builtin types, and it will be compiled "just in time" when used.
+            Setting ``is_udt=True`` is also helpful when the left and right
+            dtypes need to be different.
+        lazy : bool, default False
+            If False (the default), then the function will be automatically
+            compiled for builtin types (unless ``is_udt`` is True).
+            Compiling functions can be slow, however, so you may want to
+            delay compilation and only compile when the operator is used,
+            which is done by setting ``lazy=True``.
+
+        Examples
+        --------
+        >>> gb.indexunary.register_new("row_mod", lambda x, i, j, thunk: i % max(thunk, 2))
+        >>> dir(gb.indexunary)
+        [..., 'row_mod', ...]
         """
+        cls._check_supports_udf("register_new")
         module, funcname = cls._remove_nesting(name)
         if lazy:
             module._delayed[funcname] = (
                 cls.register_new,
                 {"name": name, "func": func, "parameterized": parameterized},
             )
         elif parameterized:
@@ -277,17 +346,20 @@
         else:
             indexunary_op = cls._build(name, func, is_udt=is_udt)
             setattr(module, funcname, indexunary_op)
             # If return type is BOOL, register additionally as a SelectOp
             if all(x == BOOL for x in indexunary_op.types.values()):
                 from .select import SelectOp
 
-                setattr(select, funcname, SelectOp._from_indexunary(indexunary_op))
+                select_module, funcname = SelectOp._remove_nesting(name, strict=False)
+                setattr(select_module, funcname, SelectOp._from_indexunary(indexunary_op))
+                if not cls._initialized:  # pragma: no cover (safety)
+                    _STANDARD_OPERATOR_NAMES.add(f"{SelectOp._modname}.{name}")
 
-        if not cls._initialized:
+        if not cls._initialized:  # pragma: no cover (safety)
             _STANDARD_OPERATOR_NAMES.add(f"{cls._modname}.{name}")
         if not lazy:
             return indexunary_op
 
     @classmethod
     def _initialize(cls):
         if cls._initialized:
@@ -319,14 +391,15 @@
         # fmt: off
         # Add SelectOp when it makes sense
         for name in ["tril", "triu", "diag", "offdiag",
                      "colle", "colgt", "rowle", "rowgt", "indexle", "indexgt",
                      "valueeq", "valuene", "valuegt", "valuege", "valuelt", "valuele"]:
             iop = getattr(indexunary, name)
             setattr(select, name, SelectOp._from_indexunary(iop))
+            _STANDARD_OPERATOR_NAMES.add(f"{SelectOp._modname}.{name}")
         # fmt: on
         cls._initialized = True
 
     def __init__(
         self,
         name,
         func=None,
@@ -344,14 +417,16 @@
         if is_udt:
             self._udt_types = {}  # {dtype: DataType}
             self._udt_ops = {}  # {dtype: TypedUserIndexUnaryOp}
 
     def __reduce__(self):
         if self._anonymous:
             if hasattr(self.orig_func, "_parameterized_info"):
+                # NOT COVERED
                 return (_deserialize_parameterized, self.orig_func._parameterized_info)
             return (self.register_anonymous, (self.orig_func, self.name))
         if (name := f"indexunary.{self.name}") in _STANDARD_OPERATOR_NAMES:
             return name
+        # NOT COVERED
         return (self._deserialize, (self.name, self.orig_func))
 
     __call__ = TypedBuiltinIndexUnaryOp.__call__
```

### Comparing `python-graphblas-2023.3.0/graphblas/core/operator/monoid.py` & `python-graphblas-2023.5.0/graphblas/core/operator/monoid.py`

 * *Files 11% similar despite different names*

```diff
@@ -265,45 +265,72 @@
         self._udt_ops[dtype] = op
         return op
 
     @classmethod
     def register_anonymous(cls, binaryop, identity, name=None, *, is_idempotent=False):
         """Register a Monoid without registering it in the ``graphblas.monoid`` namespace.
 
+        A monoid is a binary operator whose inputs and output are the same dtype.
         Because it is not registered in the namespace, the name is optional.
 
         Parameters
         ----------
-        binaryop : BinaryOp
-            Builtin or registered binary operator
-        identity :
-            Identity value of the monoid
+        binaryop: BinaryOp or ParameterizedBinaryOp
+            The binary operator of the monoid, which should be able to use the same
+            dtype for both inputs and the output.
+        identity: scalar or Mapping
+            The identity of the monoid such that ``op(x, identity) == x`` for any x.
+            ``identity`` may also be a mapping from dtype to scalar.
         name : str, optional
-            Name associated with the monoid
+            The name of the operator. This *does not* show up as ``gb.monoid.{name}``.
         is_idempotent : bool, default False
             Does ``op(x, x) == x`` for any x?
 
         Returns
         -------
-        Function handle
+        Monoid or ParameterizedMonoid
         """
         if type(binaryop) is ParameterizedBinaryOp:
             return ParameterizedMonoid(
                 name, binaryop, identity, is_idempotent=is_idempotent, anonymous=True
             )
         return cls._build(name, binaryop, identity, is_idempotent=is_idempotent, anonymous=True)
 
     @classmethod
     def register_new(cls, name, binaryop, identity, *, is_idempotent=False, lazy=False):
-        """Register a Monoid. The name will be used to identify the Monoid in the
-        ``graphblas.monoid`` namespace.
+        """Register a new Monoid and save it to ``graphblas.monoid`` namespace.
 
-            >>> gb.core.operator.Monoid.register_new("max_zero", gb.binary.max_zero, 0)
-            >>> dir(gb.monoid)
-            [..., 'max_zero', ...]
+        A monoid is a binary operator whose inputs and output are the same dtype.
+
+        Parameters
+        ----------
+        name : str
+            The name of the operator. This will show up as ``gb.monoid.{name}``.
+            The name may contain periods, ".", which will result in nested objects
+            such as ``gb.monoid.x.y.z`` for name ``"x.y.z"``.
+        binaryop: BinaryOp or ParameterizedBinaryOp
+            The binary operator of the monoid, which should be able to use the same
+            dtype for both inputs and the output.
+        identity: scalar or Mapping
+            The identity of the monoid such that ``op(x, identity) == x`` for any x.
+            ``identity`` may also be a mapping from dtype to scalar.
+        is_idempotent : bool, default False
+            Does ``op(x, x) == x`` for any x?
+        lazy : bool, default False
+            If False (the default), then the function will be automatically
+            compiled for builtin types (unless ``is_udt`` was True for the binaryop).
+            Compiling functions can be slow, however, so you may want to
+            delay compilation and only compile when the operator is used,
+            which is done by setting ``lazy=True``.
+
+        Examples
+        --------
+        >>> gb.core.operator.Monoid.register_new("max_zero", gb.binary.max_zero, 0)
+        >>> dir(gb.monoid)
+        [..., 'max_zero', ...]
         """
         module, funcname = cls._remove_nesting(name)
         if lazy:
             module._delayed[funcname] = (
                 cls.register_new,
                 {"name": name, "binaryop": binaryop, "identity": identity},
             )
```

### Comparing `python-graphblas-2023.3.0/graphblas/core/operator/semiring.py` & `python-graphblas-2023.5.0/graphblas/core/operator/semiring.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     UINT8,
     UINT16,
     UINT32,
     UINT64,
     _supports_complex,
 )
 from ...exceptions import check_status_carg
-from .. import ffi, lib
+from .. import _supports_udfs, ffi, lib
 from .base import _SS_OPERATORS, OpBase, ParameterizedUdf, TypedOpBase, _call_op, _hasop
 from .binary import BinaryOp, ParameterizedBinaryOp
 from .monoid import Monoid, ParameterizedMonoid
 
 if _supports_complex:
     from ...dtypes import FC32, FC64
 
@@ -273,37 +273,55 @@
     def register_anonymous(cls, monoid, binaryop, name=None):
         """Register a Semiring without registering it in the ``graphblas.semiring`` namespace.
 
         Because it is not registered in the namespace, the name is optional.
 
         Parameters
         ----------
-        monoid : Monoid
-            Builtin or registered monoid
-        binaryop : BinaryOp
-            Builtin or registered binary operator
+        monoid : Monoid or ParameterizedMonoid
+            The monoid of the semiring (like "plus" in the default "plus_times" semiring).
+        binaryop : BinaryOp or ParameterizedBinaryOp
+            The binaryop of the semiring (like "times" in the default "plus_times" semiring).
         name : str, optional
-            Name associated with the semiring
+            The name of the operator. This *does not* show up as ``gb.semiring.{name}``.
 
         Returns
         -------
-        Function handle
+        Semiring or ParameterizedSemiring
         """
         if type(monoid) is ParameterizedMonoid or type(binaryop) is ParameterizedBinaryOp:
             return ParameterizedSemiring(name, monoid, binaryop, anonymous=True)
         return cls._build(name, monoid, binaryop, anonymous=True)
 
     @classmethod
     def register_new(cls, name, monoid, binaryop, *, lazy=False):
-        """Register a Semiring. The name will be used to identify the Semiring in the
-        ``graphblas.semiring`` namespace.
+        """Register a new Semiring and save it to ``graphblas.semiring`` namespace.
 
-            >>> gb.core.operator.Semiring.register_new("max_max", gb.monoid.max, gb.binary.max)
-            >>> dir(gb.semiring)
-            [..., 'max_max', ...]
+        Parameters
+        ----------
+        name : str
+            The name of the operator. This will show up as ``gb.semiring.{name}``.
+            The name may contain periods, ".", which will result in nested objects
+            such as ``gb.semiring.x.y.z`` for name ``"x.y.z"``.
+        monoid : Monoid or ParameterizedMonoid
+            The monoid of the semiring (like "plus" in the default "plus_times" semiring).
+        binaryop : BinaryOp or ParameterizedBinaryOp
+            The binaryop of the semiring (like "times" in the default "plus_times" semiring).
+        lazy : bool, default False
+            If False (the default), then the function will be automatically
+            compiled for builtin types (unless ``is_udt`` is True).
+            Compiling functions can be slow, however, so you may want to
+            delay compilation and only compile when the operator is used,
+            which is done by setting ``lazy=True``.
+
+        Examples
+        --------
+        >>> gb.core.operator.Semiring.register_new("max_max", gb.monoid.max, gb.binary.max)
+        >>> dir(gb.semiring)
+        [..., 'max_max', ...]
         """
         module, funcname = cls._remove_nesting(name)
         if lazy:
             module._delayed[funcname] = (
                 cls.register_new,
                 {"name": name, "monoid": monoid, "binaryop": binaryop},
             )
@@ -354,23 +372,25 @@
                     orig_semiring.gb_name,
                 )
                 cdiv_semiring._add(new_semiring)
         # Also add truediv (always floating point) and floordiv (truncate towards -inf)
         for orig_name, orig in div_semirings.items():
             cls.register_new(f"{orig_name[:-3]}truediv", orig.monoid, binary.truediv, lazy=True)
             cls.register_new(f"{orig_name[:-3]}rtruediv", orig.monoid, "rtruediv", lazy=True)
-            cls.register_new(f"{orig_name[:-3]}floordiv", orig.monoid, "floordiv", lazy=True)
-            cls.register_new(f"{orig_name[:-3]}rfloordiv", orig.monoid, "rfloordiv", lazy=True)
+            if _supports_udfs:
+                cls.register_new(f"{orig_name[:-3]}floordiv", orig.monoid, "floordiv", lazy=True)
+                cls.register_new(f"{orig_name[:-3]}rfloordiv", orig.monoid, "rfloordiv", lazy=True)
         # For aggregators
         cls.register_new("plus_pow", monoid.plus, binary.pow)
-        cls.register_new("plus_rpow", monoid.plus, "rpow", lazy=True)
-        cls.register_new("plus_absfirst", monoid.plus, "absfirst", lazy=True)
-        cls.register_new("max_absfirst", monoid.max, "absfirst", lazy=True)
-        cls.register_new("plus_abssecond", monoid.plus, "abssecond", lazy=True)
-        cls.register_new("max_abssecond", monoid.max, "abssecond", lazy=True)
+        if _supports_udfs:
+            cls.register_new("plus_rpow", monoid.plus, "rpow", lazy=True)
+            cls.register_new("plus_absfirst", monoid.plus, "absfirst", lazy=True)
+            cls.register_new("max_absfirst", monoid.max, "absfirst", lazy=True)
+            cls.register_new("plus_abssecond", monoid.plus, "abssecond", lazy=True)
+            cls.register_new("max_abssecond", monoid.max, "abssecond", lazy=True)
 
         # Update type information with sane coercion
         for lname in ["any", "eq", "land", "lor", "lxnor", "lxor"]:
             target_name = f"{lname}_ne"
             source_name = f"{lname}_lxor"
             if not _hasop(semiring, target_name):
                 continue
```

### Comparing `python-graphblas-2023.3.0/graphblas/core/operator/unary.py` & `python-graphblas-2023.5.0/graphblas/core/operator/unary.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import inspect
 import re
 from types import FunctionType
 
-import numba
-
 from ... import _STANDARD_OPERATOR_NAMES, op, unary
 from ...dtypes import (
     BOOL,
     FP32,
     FP64,
     INT8,
     INT16,
@@ -18,28 +16,31 @@
     UINT32,
     UINT64,
     _sample_values,
     _supports_complex,
     lookup_dtype,
 )
 from ...exceptions import UdfParseError, check_status_carg
-from .. import ffi, lib
+from .. import _has_numba, ffi, lib
 from ..utils import output_type
 from .base import (
     _SS_OPERATORS,
     OpBase,
     ParameterizedUdf,
     TypedOpBase,
     _deserialize_parameterized,
-    _get_udt_wrapper,
     _hasop,
 )
 
 if _supports_complex:
     from ...dtypes import FC32, FC64
+if _has_numba:
+    import numba
+
+    from .base import _get_udt_wrapper
 
 ffi_new = ffi.new
 
 
 class TypedBuiltinUnaryOp(TypedOpBase):
     __slots__ = ()
     opclass = "UnaryOp"
@@ -271,28 +272,87 @@
         return op
 
     @classmethod
     def register_anonymous(cls, func, name=None, *, parameterized=False, is_udt=False):
         """Register a UnaryOp without registering it in the ``graphblas.unary`` namespace.
 
         Because it is not registered in the namespace, the name is optional.
+
+        Parameters
+        ----------
+        func : FunctionType
+            The function to compile. For all current backends, this must be able
+            to be compiled with ``numba.njit``.
+            ``func`` takes one input parameters of any dtype and returns any dtype.
+        name : str, optional
+            The name of the operator. This *does not* show up as ``gb.unary.{name}``.
+        parameterized : bool, default False
+            When True, create a parameterized user-defined operator, which means
+            additional parameters can be "baked into" the operator when used.
+            For example, ``gb.binary.isclose`` is a parameterized function that
+            optionally accepts ``rel_tol`` and ``abs_tol`` parameters, and it
+            can be used as: ``A.ewise_mult(B, gb.binary.isclose(rel_tol=1e-5))``.
+            When creating a parameterized user-defined operator, the ``func``
+            parameter must be a callable that *returns* a function that will
+            then get compiled. See the ``user_isclose`` example below.
+        is_udt : bool, default False
+            Whether the operator is intended to operate on user-defined types.
+            If True, then the function will not be automatically compiled for
+            builtin types, and it will be compiled "just in time" when used.
+
+        Returns
+        -------
+        UnaryOp or ParameterizedUnaryOp
         """
+        cls._check_supports_udf("register_anonymous")
         if parameterized:
             return ParameterizedUnaryOp(name, func, anonymous=True, is_udt=is_udt)
         return cls._build(name, func, anonymous=True, is_udt=is_udt)
 
     @classmethod
     def register_new(cls, name, func, *, parameterized=False, is_udt=False, lazy=False):
-        """Register a UnaryOp. The name will be used to identify the UnaryOp in the
-        ``graphblas.unary`` namespace.
+        """Register a new UnaryOp and save it to ``graphblas.unary`` namespace.
 
-            >>> gb.core.operator.UnaryOp.register_new("plus_one", lambda x: x + 1)
-            >>> dir(gb.unary)
-            [..., 'plus_one', ...]
+        Parameters
+        ----------
+        name : str
+            The name of the operator. This will show up as ``gb.unary.{name}``.
+            The name may contain periods, ".", which will result in nested objects
+            such as ``gb.unary.x.y.z`` for name ``"x.y.z"``.
+        func : FunctionType
+            The function to compile. For all current backends, this must be able
+            to be compiled with ``numba.njit``.
+            ``func`` takes one input parameters of any dtype and returns any dtype.
+        parameterized : bool, default False
+            When True, create a parameterized user-defined operator, which means
+            additional parameters can be "baked into" the operator when used.
+            For example, ``gb.binary.isclose`` is a parameterized function that
+            optionally accepts ``rel_tol`` and ``abs_tol`` parameters, and it
+            can be used as: ``A.ewise_mult(B, gb.binary.isclose(rel_tol=1e-5))``.
+            When creating a parameterized user-defined operator, the ``func``
+            parameter must be a callable that *returns* a function that will
+            then get compiled. See the ``user_isclose`` example below.
+        is_udt : bool, default False
+            Whether the operator is intended to operate on user-defined types.
+            If True, then the function will not be automatically compiled for
+            builtin types, and it will be compiled "just in time" when used.
+        lazy : bool, default False
+            If False (the default), then the function will be automatically
+            compiled for builtin types (unless ``is_udt`` is True).
+            Compiling functions can be slow, however, so you may want to
+            delay compilation and only compile when the operator is used,
+            which is done by setting ``lazy=True``.
+
+        Examples
+        --------
+        >>> gb.core.operator.UnaryOp.register_new("plus_one", lambda x: x + 1)
+        >>> dir(gb.unary)
+        [..., 'plus_one', ...]
         """
+        cls._check_supports_udf("register_new")
         module, funcname = cls._remove_nesting(name)
         if lazy:
             module._delayed[funcname] = (
                 cls.register_new,
                 {"name": name, "func": func, "parameterized": parameterized},
             )
         elif parameterized:
@@ -368,15 +428,18 @@
                             op.coercions[dtype] = target_type
         # Allow some functions to work on UDTs
         for unop, func in [
             (unary.identity, _identity),
             (unary.one, _one),
         ]:
             unop.orig_func = func
-            unop._numba_func = numba.njit(func)
+            if _has_numba:
+                unop._numba_func = numba.njit(func)
+            else:
+                unop._numba_func = None
             unop._udt_types = {}
             unop._udt_ops = {}
         cls._initialized = True
 
     def __init__(
         self,
         name,
```

### Comparing `python-graphblas-2023.3.0/graphblas/core/operator/utils.py` & `python-graphblas-2023.5.0/graphblas/core/operator/utils.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/core/recorder.py` & `python-graphblas-2023.5.0/graphblas/core/recorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,18 +133,18 @@
             "</table>",
             "</summary>",
             '<blockquote class="gb-expr-blockquote" style="margin-left: -8px;">',
         ]
         tail = "\n</blockquote>\n</details>\n</div>"
         return "\n".join(head), tail
 
-    def _repr_html_(self):  # pragma: no cover
+    def _repr_html_(self):
         try:
             from IPython.display import Code
-        except ImportError as exc:
+        except ImportError as exc:  # pragma: no cover (import)
             raise NotImplementedError from exc
         lines = self._get_repr_lines()
         code = Code("\n".join(lines), language="C")
         head, tail = self._repr_base_()
         return head + code._repr_html_() + tail
 
     def _repr_markdown_(self):
```

### Comparing `python-graphblas-2023.3.0/graphblas/core/scalar.py` & `python-graphblas-2023.5.0/graphblas/core/scalar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import itertools
 
 import numpy as np
 
 from .. import backend, binary, config, monoid
-from ..binary import isclose
 from ..dtypes import _INDEX, FP64, lookup_dtype, unify
 from ..exceptions import EmptyObject, check_status
-from . import automethods, ffi, lib, utils
+from . import _has_numba, _supports_udfs, automethods, ffi, lib, utils
 from .base import BaseExpression, BaseType, call
 from .expr import AmbiguousAssignOrExtract
 from .operator import get_typed_op
 from .utils import _Pointer, output_type, wrapdoc
 
+if _supports_udfs:
+    from ..binary import isclose
+else:
+    from .operator.binary import _isclose as isclose
+
 ffi_new = ffi.new
 
 
 def _scalar_index(name):
     """Fast way to create scalars with GrB_Index type; used internally."""
     self = object.__new__(Scalar)
     self.name = name
@@ -257,14 +261,25 @@
             return False
         if self._is_empty:
             return other._is_empty
         if other._is_empty:
             return False
         # We can't yet call a UDF on a scalar as part of the spec, so let's do it ourselves
         isclose_func = isclose(rel_tol, abs_tol)
+        if not _has_numba:
+            # Check if types are compatible
+            get_typed_op(
+                binary.eq,
+                self.dtype,
+                other.dtype,
+                is_left_scalar=True,
+                is_right_scalar=True,
+                kind="binary",
+            )
+            return isclose_func(self.value, other.value)
         isclose_func = get_typed_op(
             isclose_func,
             self.dtype,
             other.dtype,
             is_left_scalar=True,
             is_right_scalar=True,
             kind="binary",
```

### Comparing `python-graphblas-2023.3.0/graphblas/core/slice.py` & `python-graphblas-2023.5.0/graphblas/core/slice.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/core/ss/config.py` & `python-graphblas-2023.5.0/graphblas/core/ss/config.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/core/ss/descriptor.py` & `python-graphblas-2023.5.0/graphblas/core/ss/descriptor.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/core/ss/matrix.py` & `python-graphblas-2023.5.0/graphblas/core/ss/matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import itertools
 import warnings
 
-import numba
 import numpy as np
-from numba import njit
 from suitesparse_graphblas.utils import claim_buffer, claim_buffer_2d, unclaim_buffer
 
 import graphblas as gb
 
 from ... import binary, monoid
 from ...dtypes import _INDEX, BOOL, INT64, UINT64, _string_to_dtype, lookup_dtype
 from ...exceptions import _error_code_lookup, check_status, check_status_carg
-from .. import NULL, ffi, lib
+from .. import NULL, _has_numba, ffi, lib
 from ..base import call
 from ..operator import get_typed_op
 from ..scalar import Scalar, _as_scalar, _scalar_index
 from ..utils import (
     _CArray,
     _MatrixArray,
     _Pointer,
@@ -26,14 +24,24 @@
     output_type,
     values_to_numpy_buffer,
     wrapdoc,
 )
 from .config import BaseConfig
 from .descriptor import get_descriptor
 
+if _has_numba:
+    from numba import njit, prange
+else:
+
+    def njit(func=None, **kwargs):
+        if func is not None:
+            return func
+        return njit
+
+    prange = range
 ffi_new = ffi.new
 
 
 def head(matrix, n=10, dtype=None, *, sort=False):
     """Like ``matrix.to_coo()``, but only returns the first n elements.
 
     If sort is True, then the results will be sorted as appropriate for the internal format,
@@ -884,15 +892,15 @@
                 parent,
             )
             is_iso = is_iso[0]
             indptr = claim_buffer(ffi, Ap[0], Ap_size[0] // index_dtype.itemsize, index_dtype)
             col_indices = claim_buffer(ffi, Aj[0], Aj_size[0] // index_dtype.itemsize, index_dtype)
             values = claim_buffer(ffi, Ax[0], Ax_size[0] // dtype.itemsize, dtype)
             if not raw:
-                if indptr.size > nrows + 1:
+                if indptr.size > nrows + 1:  # pragma: no cover (suitesparse)
                     indptr = indptr[: nrows + 1]
                 if col_indices.size > nvals:
                     col_indices = col_indices[:nvals]
                 if is_iso:
                     if values.size > 1:  # pragma: no branch (suitesparse)
                         values = values[:1]
                 elif values.size > nvals:  # pragma: no branch (suitesparse)
@@ -925,15 +933,15 @@
                 parent,
             )
             is_iso = is_iso[0]
             indptr = claim_buffer(ffi, Ap[0], Ap_size[0] // index_dtype.itemsize, index_dtype)
             row_indices = claim_buffer(ffi, Ai[0], Ai_size[0] // index_dtype.itemsize, index_dtype)
             values = claim_buffer(ffi, Ax[0], Ax_size[0] // dtype.itemsize, dtype)
             if not raw:
-                if indptr.size > ncols + 1:
+                if indptr.size > ncols + 1:  # pragma: no cover (suitesparse)
                     indptr = indptr[: ncols + 1]
                 if row_indices.size > nvals:
                     row_indices = row_indices[:nvals]
                 if is_iso:
                     if values.size > 1:  # pragma: no cover (suitesparse)
                         values = values[:1]
                 elif values.size > nvals:
@@ -1782,14 +1790,15 @@
 
         Create a new Matrix from standard HyperCSC format.
 
         Parameters
         ----------
         nrows : int
         ncols : int
+        cols : array-like
         indptr : array-like
         values : array-like
         row_indices : array-like
         nvec : int, optional
             The number of elements in "cols" to use.
             If not specified, will be set to ``len(cols)``.
         is_iso : bool, default False
@@ -4367,77 +4376,77 @@
         )
         rv = gb.Matrix._from_obj(gb_obj, dtype, -1, -1, name=name)
         rv._nrows = rv.nrows
         rv._ncols = rv.ncols
         return rv
 
 
-@numba.njit(parallel=True)
+@njit(parallel=True)
 def argsort_values(indptr, indices, values):  # pragma: no cover (numba)
     rv = np.empty(indptr[-1], dtype=np.uint64)
-    for i in numba.prange(indptr.size - 1):
+    for i in prange(indptr.size - 1):
         rv[indptr[i] : indptr[i + 1]] = indices[
             np.int64(indptr[i]) + np.argsort(values[indptr[i] : indptr[i + 1]])
         ]
     return rv
 
 
-@numba.njit(parallel=True)
+@njit(parallel=True)
 def sort_values(indptr, values):  # pragma: no cover (numba)
     rv = np.empty(indptr[-1], dtype=values.dtype)
-    for i in numba.prange(indptr.size - 1):
+    for i in prange(indptr.size - 1):
         rv[indptr[i] : indptr[i + 1]] = np.sort(values[indptr[i] : indptr[i + 1]])
     return rv
 
 
-@numba.njit(parallel=True)
+@njit(parallel=True)
 def compact_values(old_indptr, new_indptr, values):  # pragma: no cover (numba)
     rv = np.empty(new_indptr[-1], dtype=values.dtype)
-    for i in numba.prange(new_indptr.size - 1):
+    for i in prange(new_indptr.size - 1):
         start = np.int64(new_indptr[i])
         offset = np.int64(old_indptr[i]) - start
         for j in range(start, new_indptr[i + 1]):
             rv[j] = values[j + offset]
     return rv
 
 
-@numba.njit(parallel=True)
+@njit(parallel=True)
 def reverse_values(indptr, values):  # pragma: no cover (numba)
     rv = np.empty(indptr[-1], dtype=values.dtype)
-    for i in numba.prange(indptr.size - 1):
+    for i in prange(indptr.size - 1):
         offset = np.int64(indptr[i]) + np.int64(indptr[i + 1]) - 1
         for j in range(indptr[i], indptr[i + 1]):
             rv[j] = values[offset - j]
     return rv
 
 
-@numba.njit(parallel=True)
+@njit(parallel=True)
 def compact_indices(indptr, k):  # pragma: no cover (numba)
     """Given indptr from hypercsr, create a new col_indices array that is compact.
 
     That is, for each row with degree N, the column indices will be 0..N-1.
     """
     if k is not None:
         indptr = create_indptr(indptr, k)
     col_indices = np.empty(indptr[-1], dtype=np.uint64)
     N = np.int64(0)
-    for i in numba.prange(indptr.size - 1):
+    for i in prange(indptr.size - 1):
         start = np.int64(indptr[i])
         deg = np.int64(indptr[i + 1]) - start
         N = max(N, deg)
         for j in range(deg):
             col_indices[start + j] = j
     return indptr, col_indices, N
 
 
 @njit(parallel=True)
 def choose_random1(indptr):  # pragma: no cover (numba)
     choices = np.empty(indptr.size - 1, dtype=indptr.dtype)
     new_indptr = np.arange(indptr.size, dtype=indptr.dtype)
-    for i in numba.prange(indptr.size - 1):
+    for i in prange(indptr.size - 1):
         idx = np.int64(indptr[i])
         deg = np.int64(indptr[i + 1]) - idx
         if deg == 1:
             choices[i] = idx
         else:
             choices[i] = np.random.randint(idx, idx + deg)
     return choices, new_indptr
@@ -4466,15 +4475,15 @@
     if k == 1:
         return choose_random1(indptr)
 
     # The results in choices don't need to be random.  In fact, it may
     # be nice to have them sorted if convenient to do so.
     new_indptr = create_indptr(indptr, k)
     choices = np.empty(new_indptr[-1], dtype=indptr.dtype)
-    for i in numba.prange(indptr.size - 1):
+    for i in prange(indptr.size - 1):
         idx = np.int64(indptr[i])
         deg = np.int64(indptr[i + 1]) - idx
         if k < deg:
             curk = k
         else:
             curk = deg
         index = np.int64(new_indptr[i])
@@ -4547,15 +4556,15 @@
     if k == 1:
         choices = indptr[:-1]
         new_indptr = np.arange(indptr.size, dtype=indptr.dtype)
         return choices, new_indptr
 
     new_indptr = create_indptr(indptr, k)
     choices = np.empty(new_indptr[-1], dtype=indptr.dtype)
-    for i in numba.prange(indptr.size - 1):
+    for i in prange(indptr.size - 1):
         idx = np.int64(indptr[i])
         deg = np.int64(indptr[i + 1]) - idx
         if k < deg:
             curk = k
         else:
             curk = deg
         j = np.int64(new_indptr[i])
@@ -4571,15 +4580,15 @@
     if k == 1:
         choices = (indptr[1:].astype(np.int64) - 1).astype(indptr.dtype)
         new_indptr = np.arange(indptr.size, dtype=indptr.dtype)
         return choices, new_indptr
 
     new_indptr = create_indptr(indptr, k)
     choices = np.empty(new_indptr[-1], dtype=indptr.dtype)
-    for i in numba.prange(indptr.size - 1):
+    for i in prange(indptr.size - 1):
         idx = np.int64(indptr[i])
         deg = np.int64(indptr[i + 1]) - idx
         if k < deg:
             curk = k
         else:
             curk = deg
         j = np.int64(new_indptr[i])
@@ -4604,26 +4613,27 @@
 
 
 @njit
 def indices_to_indptr(indices, size):  # pragma: no cover (numba)
     """Calculate the indptr for e.g. CSR from sorted COO rows."""
     indptr = np.zeros(size, dtype=indices.dtype)
     index = np.uint64(0)
+    one = np.uint64(1)
     for i in range(indices.size):
         row = indices[i]
         if row != index:
-            indptr[index + 1] = i
+            indptr[index + one] = i
             index = row
-    indptr[index + 1] = indices.size
+    indptr[index + one] = indices.size
     return indptr
 
 
 @njit(parallel=True)
 def indptr_to_indices(indptr):  # pragma: no cover (numba)
     indices = np.empty(indptr[-1], dtype=indptr.dtype)
-    for i in numba.prange(indptr.size - 1):
+    for i in prange(indptr.size - 1):
         for j in range(indptr[i], indptr[i + 1]):
             indices[j] = i
     return indices
 
 
 from .prefix_scan import prefix_scan  # noqa: E402 isort:skip
```

### Comparing `python-graphblas-2023.3.0/graphblas/core/ss/prefix_scan.py` & `python-graphblas-2023.5.0/graphblas/core/ss/prefix_scan.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/core/ss/vector.py` & `python-graphblas-2023.5.0/graphblas/core/ss/vector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import itertools
 
 import numpy as np
-from numba import njit
 from suitesparse_graphblas.utils import claim_buffer, unclaim_buffer
 
 import graphblas as gb
 
 from ... import binary, monoid
 from ...dtypes import _INDEX, INT64, UINT64, _string_to_dtype, lookup_dtype
 from ...exceptions import _error_code_lookup, check_status, check_status_carg
@@ -19,15 +18,15 @@
     ints_to_numpy_buffer,
     normalize_chunks,
     values_to_numpy_buffer,
     wrapdoc,
 )
 from .config import BaseConfig
 from .descriptor import get_descriptor
-from .matrix import _concat_mn
+from .matrix import _concat_mn, njit
 from .prefix_scan import prefix_scan
 
 ffi_new = ffi.new
 
 
 def head(vector, n=10, dtype=None, *, sort=False):
     """Like ``vector.to_coo()``, but only returns the first n elements.
@@ -584,15 +583,15 @@
             values = claim_buffer(ffi, vx[0], vx_size[0] // dtype.itemsize, dtype)
             if not raw:
                 if bitmap.size > size:  # pragma: no branch (suitesparse)
                     bitmap = bitmap[:size]
                 if is_iso:
                     if values.size > 1:  # pragma: no cover (suitesparse)
                         values = values[:1]
-                elif values.size > size:  # pragma: no branch (suitesparse)
+                elif values.size > size:  # pragma: no cover (suitesparse)
                     values = values[:size]
             rv = {
                 "bitmap": bitmap,
                 "nvals": nvals[0],
             }
             if raw:
                 rv["size"] = size
```

### Comparing `python-graphblas-2023.3.0/graphblas/core/utils.py` & `python-graphblas-2023.5.0/graphblas/core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,15 @@
         # Get nrows and ncols from the first 2d array
         is_subarray = dtype.np_type.subdtype is not None
         for name, arr in arrays.items():
             if name == "values" and is_subarray:
                 # We could be smarter and determine the shape of the dtype sub-arrays
                 if arr.ndim >= 3:
                     break
+                # BRANCH NOT COVERED
             elif arr.ndim == 2:
                 break
         else:
             raise ValueError(
                 "Either nrows and ncols must be provided, or one of the following arrays"
                 f'must be 2d (from which to get nrows and ncols): {", ".join(arrays)}'
             )
```

### Comparing `python-graphblas-2023.3.0/graphblas/core/vector.py` & `python-graphblas-2023.5.0/graphblas/core/vector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import itertools
 import warnings
 
 import numpy as np
 
-from .. import backend, binary, monoid, select, semiring
+from .. import backend, binary, monoid, select, semiring, unary
 from ..dtypes import _INDEX, FP64, INT64, lookup_dtype, unify
 from ..exceptions import DimensionMismatch, NoValue, check_status
-from . import automethods, ffi, lib, utils
+from . import _supports_udfs, automethods, ffi, lib, utils
 from .base import BaseExpression, BaseType, _check_mask, call
 from .descriptor import lookup as descriptor_lookup
 from .expr import _ALL_INDICES, AmbiguousAssignOrExtract, IndexerResolver, Updater
 from .mask import Mask, StructuralMask, ValueMask
 from .operator import UNKNOWN_OPCLASS, find_opclass, get_semiring, get_typed_op, op_from_string
 from .scalar import (
     _COMPLETE,
@@ -89,14 +89,53 @@
         finally:
             updater.kwargs = orig_kwargs
     else:
         # Can we do any better depending on accum, replace, and type of masks?
         updater << obj.dup(mask=mask)
 
 
+def _isclose_recipe(self, other, rel_tol, abs_tol, **opts):
+    #  x == y or abs(x - y) <= max(rel_tol * max(abs(x), abs(y)), abs_tol)
+    isequal = self.ewise_mult(other, binary.eq).new(bool, name="isclose", **opts)
+    if isequal._nvals != self._nvals:
+        return False
+    if type(isequal) is Vector:
+        val = isequal.reduce(monoid.land, allow_empty=False).new(**opts).value
+    else:
+        val = isequal.reduce_scalar(monoid.land, allow_empty=False).new(**opts).value
+    if val:
+        return True
+    # So we can use structural mask below
+    isequal(**opts) << select.value(isequal == True)  # noqa: E712
+
+    # abs(x)
+    x = self.apply(unary.abs).new(FP64, mask=~isequal.S, **opts)
+    # abs(y)
+    y = other.apply(unary.abs).new(FP64, mask=~isequal.S, **opts)
+    # max(abs(x), abs(y))
+    x(**opts) << x.ewise_mult(y, binary.max)
+    max_x_y = x
+    # rel_tol * max(abs(x), abs(y))
+    max_x_y(**opts) << max_x_y.apply(binary.times, rel_tol)
+    # max(rel_tol * max(abs(x), abs(y)), abs_tol)
+    max_x_y(**opts) << max_x_y.apply(binary.max, abs_tol)
+
+    # x - y
+    y(~isequal.S, replace=True, **opts) << self.ewise_mult(other, binary.minus)
+    abs_x_y = y
+    # abs(x - y)
+    abs_x_y(**opts) << abs_x_y.apply(unary.abs)
+
+    # abs(x - y) <= max(rel_tol * max(abs(x), abs(y)), abs_tol)
+    isequal(**opts) << abs_x_y.ewise_mult(max_x_y, binary.le)
+    if isequal.ndim == 1:
+        return isequal.reduce(monoid.land, allow_empty=False).new(**opts).value
+    return isequal.reduce_scalar(monoid.land, allow_empty=False).new(**opts).value
+
+
 class Vector(BaseType):
     """Create a new GraphBLAS Sparse Vector.
 
     Parameters
     ----------
     dtype :
         Data type for elements in the Vector.
@@ -350,14 +389,16 @@
         other = self._expect_type(other, Vector, within="isclose", argname="other")
         if check_dtype and self.dtype != other.dtype:
             return False
         if self._size != other._size:
             return False
         if self._nvals != other._nvals:
             return False
+        if not _supports_udfs:
+            return _isclose_recipe(self, other, rel_tol, abs_tol, **opts)
 
         matches = self.ewise_mult(other, binary.isclose(rel_tol, abs_tol)).new(
             bool, name="M_isclose", **opts
         )
         # ewise_mult performs intersection, so nvals will indicate mismatched empty values
         if matches._nvals != self._nvals:
             return False
@@ -516,22 +557,23 @@
         if n == 0:
             return
 
         dup_op_given = dup_op is not None
         if not dup_op_given:
             if not self.dtype._is_udt:
                 dup_op = binary.plus
-            else:
+            elif backend != "suitesparse":
                 dup_op = binary.any
-        # SS:SuiteSparse-specific: we could use NULL for dup_op
-        dup_op = get_typed_op(dup_op, self.dtype, kind="binary")
-        if dup_op.opclass == "Monoid":
-            dup_op = dup_op.binaryop
-        else:
-            self._expect_op(dup_op, "BinaryOp", within="build", argname="dup_op")
+            # SS:SuiteSparse-specific: we use NULL for dup_op
+        if dup_op is not None:
+            dup_op = get_typed_op(dup_op, self.dtype, kind="binary")
+            if dup_op.opclass == "Monoid":
+                dup_op = dup_op.binaryop
+            else:
+                self._expect_op(dup_op, "BinaryOp", within="build", argname="dup_op")
 
         indices = _CArray(indices)
         values = _CArray(values, self.dtype)
         dtype_name = "UDT" if self.dtype._is_udt else self.dtype.name
         call(
             f"GrB_Vector_build_{dtype_name}",
             [self, indices, values, _as_scalar(n, _INDEX, is_cscalar=True), dup_op],
@@ -1496,14 +1538,15 @@
                 )
         op = get_typed_op(op, self.dtype, thunk.dtype, is_right_scalar=True, kind="select")
         self._expect_op(op, ("SelectOp", "IndexUnaryOp"), within=method_name, argname="op")
         if thunk._is_cscalar:
             if thunk.dtype._is_udt:
                 dtype_name = "UDT"
                 thunk = _Pointer(thunk)
+                # NOT COVERED
             else:
                 dtype_name = thunk.dtype.name
             cfunc_name = f"GrB_Vector_select_{dtype_name}"
         else:
             cfunc_name = "GrB_Vector_select_Scalar"
         return VectorExpression(
             method_name,
@@ -1813,21 +1856,22 @@
                             values, dtype = values_to_numpy_buffer(value, dtype)
                         except Exception:
                             extra_message = "Literal scalars and lists also accepted."
                         else:
                             shape = values.shape
                             try:
                                 vals = Vector.from_dense(values, dtype=dtype)
-                            except Exception:  # pragma: no cover (safety)
+                            except Exception:
                                 vals = None
                             else:
                                 if dtype.np_type.subdtype is not None:
                                     shape = vals.shape
                             if vals is None or shape != (size,):
                                 if dtype.np_type.subdtype is not None:
+                                    # NOT COVERED
                                     extra = (
                                         " (this is assigning to a vector with sub-array dtype "
                                         f"({dtype}), so array shape should include dtype shape)"
                                     )
                                 else:
                                     extra = ""
                                 raise ValueError(
@@ -1939,15 +1983,15 @@
         indices = np.fromiter(d.keys(), np.uint64)
         if dtype is None:
             values, dtype = values_to_numpy_buffer(list(d.values()), subarray_after=1)
         else:
             # If we know the dtype, then using `np.fromiter` is much faster
             dtype = lookup_dtype(dtype)
             if dtype.np_type.subdtype is not None and np.__version__[:5] in {"1.21.", "1.22."}:
-                values, dtype = values_to_numpy_buffer(list(d.values()), dtype)
+                values, dtype = values_to_numpy_buffer(list(d.values()), dtype)  # FLAKY COVERAGE
             else:
                 values = np.fromiter(d.values(), dtype.np_type)
         if size is None and indices.size == 0:
             size = 0
         return cls.from_coo(indices, values, dtype, size=size, name=name)
 
     def to_dict(self):
```

### Comparing `python-graphblas-2023.3.0/graphblas/dtypes.py` & `python-graphblas-2023.5.0/graphblas/dtypes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import warnings as _warnings
 
-import numba as _numba
 import numpy as _np
 from numpy import find_common_type as _find_common_type
 from numpy import promote_types as _promote_types
 
 from . import backend
 from .core import NULL as _NULL
+from .core import _has_numba
 from .core import ffi as _ffi
 from .core import lib as _lib
 
+if _has_numba:
+    import numba as _numba
+
 # Default assumption unless FC32/FC64 are found in lib
 _supports_complex = hasattr(_lib, "GrB_FC64") or hasattr(_lib, "GxB_FC64")
 
 
 class DataType:
     __slots__ = "name", "gb_obj", "gb_name", "c_type", "numba_type", "np_type", "__weakref__"
 
@@ -136,69 +139,151 @@
     else:
         status = _lib.GrB_Type_new(gb_obj, dtype.itemsize)
     check_status_carg(status, "Type", gb_obj[0])
 
     # For now, let's use "opaque" unsigned bytes for the c type.
     if name is None:
         name = _default_name(dtype)
-    numba_type = _numba.typeof(dtype).dtype
+    numba_type = _numba.typeof(dtype).dtype if _has_numba else None
     rv = DataType(name, gb_obj, None, f"uint8_t[{dtype.itemsize}]", numba_type, dtype)
     _registry[gb_obj] = rv
     _registry[dtype] = rv
-    _registry[numba_type] = rv
-    _registry[numba_type.name] = rv
+    if _has_numba:
+        _registry[numba_type] = rv
+        _registry[numba_type.name] = rv
     return rv
 
 
-BOOL = DataType("BOOL", _lib.GrB_BOOL, "GrB_BOOL", "_Bool", _numba.types.bool_, _np.bool_)
-INT8 = DataType("INT8", _lib.GrB_INT8, "GrB_INT8", "int8_t", _numba.types.int8, _np.int8)
-UINT8 = DataType("UINT8", _lib.GrB_UINT8, "GrB_UINT8", "uint8_t", _numba.types.uint8, _np.uint8)
-INT16 = DataType("INT16", _lib.GrB_INT16, "GrB_INT16", "int16_t", _numba.types.int16, _np.int16)
+BOOL = DataType(
+    "BOOL",
+    _lib.GrB_BOOL,
+    "GrB_BOOL",
+    "_Bool",
+    _numba.types.bool_ if _has_numba else None,
+    _np.bool_,
+)
+INT8 = DataType(
+    "INT8", _lib.GrB_INT8, "GrB_INT8", "int8_t", _numba.types.int8 if _has_numba else None, _np.int8
+)
+UINT8 = DataType(
+    "UINT8",
+    _lib.GrB_UINT8,
+    "GrB_UINT8",
+    "uint8_t",
+    _numba.types.uint8 if _has_numba else None,
+    _np.uint8,
+)
+INT16 = DataType(
+    "INT16",
+    _lib.GrB_INT16,
+    "GrB_INT16",
+    "int16_t",
+    _numba.types.int16 if _has_numba else None,
+    _np.int16,
+)
 UINT16 = DataType(
-    "UINT16", _lib.GrB_UINT16, "GrB_UINT16", "uint16_t", _numba.types.uint16, _np.uint16
+    "UINT16",
+    _lib.GrB_UINT16,
+    "GrB_UINT16",
+    "uint16_t",
+    _numba.types.uint16 if _has_numba else None,
+    _np.uint16,
+)
+INT32 = DataType(
+    "INT32",
+    _lib.GrB_INT32,
+    "GrB_INT32",
+    "int32_t",
+    _numba.types.int32 if _has_numba else None,
+    _np.int32,
 )
-INT32 = DataType("INT32", _lib.GrB_INT32, "GrB_INT32", "int32_t", _numba.types.int32, _np.int32)
 UINT32 = DataType(
-    "UINT32", _lib.GrB_UINT32, "GrB_UINT32", "uint32_t", _numba.types.uint32, _np.uint32
+    "UINT32",
+    _lib.GrB_UINT32,
+    "GrB_UINT32",
+    "uint32_t",
+    _numba.types.uint32 if _has_numba else None,
+    _np.uint32,
+)
+INT64 = DataType(
+    "INT64",
+    _lib.GrB_INT64,
+    "GrB_INT64",
+    "int64_t",
+    _numba.types.int64 if _has_numba else None,
+    _np.int64,
 )
-INT64 = DataType("INT64", _lib.GrB_INT64, "GrB_INT64", "int64_t", _numba.types.int64, _np.int64)
 # _Index (like UINT64) is for internal use only and shouldn't be exposed to the user
 _INDEX = DataType(
-    "UINT64", _lib.GrB_UINT64, "GrB_Index", "GrB_Index", _numba.types.uint64, _np.uint64
+    "UINT64",
+    _lib.GrB_UINT64,
+    "GrB_Index",
+    "GrB_Index",
+    _numba.types.uint64 if _has_numba else None,
+    _np.uint64,
 )
 UINT64 = DataType(
-    "UINT64", _lib.GrB_UINT64, "GrB_UINT64", "uint64_t", _numba.types.uint64, _np.uint64
+    "UINT64",
+    _lib.GrB_UINT64,
+    "GrB_UINT64",
+    "uint64_t",
+    _numba.types.uint64 if _has_numba else None,
+    _np.uint64,
+)
+FP32 = DataType(
+    "FP32",
+    _lib.GrB_FP32,
+    "GrB_FP32",
+    "float",
+    _numba.types.float32 if _has_numba else None,
+    _np.float32,
+)
+FP64 = DataType(
+    "FP64",
+    _lib.GrB_FP64,
+    "GrB_FP64",
+    "double",
+    _numba.types.float64 if _has_numba else None,
+    _np.float64,
 )
-FP32 = DataType("FP32", _lib.GrB_FP32, "GrB_FP32", "float", _numba.types.float32, _np.float32)
-FP64 = DataType("FP64", _lib.GrB_FP64, "GrB_FP64", "double", _numba.types.float64, _np.float64)
 
 if _supports_complex and hasattr(_lib, "GxB_FC32"):
     FC32 = DataType(
-        "FC32", _lib.GxB_FC32, "GxB_FC32", "float _Complex", _numba.types.complex64, _np.complex64
+        "FC32",
+        _lib.GxB_FC32,
+        "GxB_FC32",
+        "float _Complex",
+        _numba.types.complex64 if _has_numba else None,
+        _np.complex64,
     )
 if _supports_complex and hasattr(_lib, "GrB_FC32"):  # pragma: no cover (unused)
     FC32 = DataType(
-        "FC32", _lib.GrB_FC32, "GrB_FC32", "float _Complex", _numba.types.complex64, _np.complex64
+        "FC32",
+        _lib.GrB_FC32,
+        "GrB_FC32",
+        "float _Complex",
+        _numba.types.complex64 if _has_numba else None,
+        _np.complex64,
     )
 if _supports_complex and hasattr(_lib, "GxB_FC64"):
     FC64 = DataType(
         "FC64",
         _lib.GxB_FC64,
         "GxB_FC64",
         "double _Complex",
-        _numba.types.complex128,
+        _numba.types.complex128 if _has_numba else None,
         _np.complex128,
     )
 if _supports_complex and hasattr(_lib, "GrB_FC64"):  # pragma: no cover (unused)
     FC64 = DataType(
         "FC64",
         _lib.GrB_FC64,
         "GrB_FC64",
         "double _Complex",
-        _numba.types.complex128,
+        _numba.types.complex128 if _has_numba else None,
         _np.complex128,
     )
 
 # Used for testing user-defined functions
 _sample_values = {
     INT8: _np.int8(1),
     UINT8: _np.uint8(1),
@@ -242,16 +327,17 @@
     _registry[dtype.name] = dtype
     _registry[dtype.name.lower()] = dtype
     _registry[dtype.gb_obj] = dtype
     _registry[dtype.gb_name] = dtype
     _registry[dtype.gb_name.lower()] = dtype
     _registry[dtype.c_type] = dtype
     _registry[dtype.c_type.upper()] = dtype
-    _registry[dtype.numba_type] = dtype
-    _registry[dtype.numba_type.name] = dtype
+    if _has_numba:
+        _registry[dtype.numba_type] = dtype
+        _registry[dtype.numba_type.name] = dtype
     val = _sample_values[dtype]
     _registry[val.dtype] = dtype
     _registry[val.dtype.name] = dtype
 del dtype, val
 
 # Add some common Python types as lookup keys
 _registry[bool] = BOOL
```

### Comparing `python-graphblas-2023.3.0/graphblas/exceptions.py` & `python-graphblas-2023.5.0/graphblas/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/monoid/__init__.py` & `python-graphblas-2023.5.0/graphblas/monoid/__init__.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/monoid/numpy.py` & `python-graphblas-2023.5.0/graphblas/monoid/numpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """Create UDFs of numpy functions supported by numba.
 
 See list of numpy ufuncs supported by numpy here:
 
 https://numba.readthedocs.io/en/stable/reference/numpysupported.html#math-operations
 
 """
-import numba as _numba
 import numpy as _np
 
 from .. import _STANDARD_OPERATOR_NAMES
 from .. import binary as _binary
 from .. import config as _config
 from .. import monoid as _monoid
+from ..core import _has_numba, _supports_udfs
 from ..dtypes import _supports_complex
 
+if _has_numba:
+    import numba as _numba
+
 _delayed = {}
 _complex_dtypes = {"FC32", "FC64"}
 _float_dtypes = {"FP32", "FP64"}
 _int_dtypes = {"INT8", "UINT8", "INT16", "UINT16", "INT32", "UINT32", "INT64", "UINT64"}
 _bool_int_dtypes = _int_dtypes | {"BOOL"}
 
 _monoid_identities = {
@@ -82,15 +85,16 @@
         dict.fromkeys(_complex_dtypes, complex(-_np.inf, -_np.inf))
     )
     _monoid_identities["minimum"].update(dict.fromkeys(_complex_dtypes, complex(_np.inf, _np.inf)))
 
 # To increase import speed, only call njit when `_config.get("mapnumpy")` is False
 if (
     _config.get("mapnumpy")
-    or type(_numba.njit(lambda x, y: _np.fmax(x, y))(1, 2))  # pragma: no branch (numba)
+    or _has_numba
+    and type(_numba.njit(lambda x, y: _np.fmax(x, y))(1, 2))  # pragma: no branch (numba)
     is not float
 ):
     # Incorrect behavior was introduced in numba 0.56.2 and numpy 1.23
     # See: https://github.com/numba/numba/issues/8478
     # MAINT: we may be able to remove the behavior-based check above in 2025
     _monoid_identities["fmax"].update(
         {
@@ -151,15 +155,20 @@
     "logical_or",
     "maximum",
     "minimum",
 }
 
 
 def __dir__():
-    return globals().keys() | _delayed.keys() | _monoid_identities.keys()
+    if not _supports_udfs and not _config.get("mapnumpy"):
+        return globals().keys()  # FLAKY COVERAGE
+    attrs = _delayed.keys() | _monoid_identities.keys()
+    if not _supports_udfs:
+        attrs &= _numpy_to_graphblas.keys()
+    return attrs | globals().keys()
 
 
 def __getattr__(name):
     if name in _delayed:
         func, kwargs = _delayed.pop(name)
         if type(kwargs["binaryop"]) is str:
             from ..binary import from_string
```

### Comparing `python-graphblas-2023.3.0/graphblas/op/__init__.py` & `python-graphblas-2023.5.0/graphblas/op/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,22 @@
                 f'module {__name__!r} only has attribute "ss" when backend is "suitesparse"'
             )
         from importlib import import_module
 
         ss = import_module(".ss", __name__)
         globals()["ss"] = ss
         return ss
+    if not _supports_udfs:
+        from .. import binary, semiring
+
+        if key in binary._udfs or key in semiring._udfs:
+            raise AttributeError(
+                f"module {__name__!r} unable to compile UDF for {key!r}; "
+                "install numba for UDF support"
+            )
     raise AttributeError(f"module {__name__!r} has no attribute {key!r}")
 
 
-from ..core import operator  # noqa: E402 isort:skip
+from ..core import operator, _supports_udfs  # noqa: E402 isort:skip
 from . import numpy  # noqa: E402 isort:skip
 
 del operator
```

### Comparing `python-graphblas-2023.3.0/graphblas/op/numpy.py` & `python-graphblas-2023.5.0/graphblas/op/numpy.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from ..binary import numpy as _np_binary
+from ..core import _supports_udfs
 from ..semiring import numpy as _np_semiring
 from ..unary import numpy as _np_unary
 
 _delayed = {}
 _op_to_mod = dict.fromkeys(_np_unary.__all__, _np_unary)
 _op_to_mod.update(dict.fromkeys(_np_binary.__all__, _np_binary))
 _op_to_mod.update(dict.fromkeys(_np_semiring.__all__, _np_semiring))
 __all__ = list(_op_to_mod)
 
 
 def __dir__():
-    return globals().keys() | _delayed.keys() | _op_to_mod.keys()
+    attrs = _delayed.keys() | _op_to_mod.keys()
+    if not _supports_udfs:
+        attrs &= _np_unary.__dir__() | _np_binary.__dir__() | _np_semiring.__dir__()
+    return attrs | globals().keys()
 
 
 def __getattr__(name):
     if name in _delayed:
         module = _delayed.pop(name)
         rv = getattr(module, name)
         globals()[name] = rv
```

### Comparing `python-graphblas-2023.3.0/graphblas/select/__init__.py` & `python-graphblas-2023.5.0/graphblas/select/__init__.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/semiring/numpy.py` & `python-graphblas-2023.5.0/graphblas/semiring/numpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import itertools as _itertools
 
 from .. import _STANDARD_OPERATOR_NAMES
 from .. import binary as _binary
 from .. import config as _config
 from .. import monoid as _monoid
 from ..binary.numpy import _binary_names
+from ..core import _supports_udfs
 from ..monoid.numpy import _fmin_is_float, _monoid_identities
 
 _delayed = {}
 _semiring_names = {
     f"{monoid_name}_{binary_name}"
     for monoid_name, binary_name in _itertools.product(_monoid_identities, _binary_names)
 }
@@ -128,15 +129,25 @@
 
 
 _STANDARD_OPERATOR_NAMES.update(f"semiring.numpy.{name}" for name in _semiring_names)
 __all__ = list(_semiring_names)
 
 
 def __dir__():
-    return globals().keys() | _delayed.keys() | _semiring_names
+    if not _supports_udfs and not _config.get("mapnumpy"):
+        return globals().keys()  # FLAKY COVERAGE
+    attrs = _delayed.keys() | _semiring_names
+    if not _supports_udfs:
+        attrs &= {
+            f"{monoid_name}_{binary_name}"
+            for monoid_name, binary_name in _itertools.product(
+                dir(_monoid.numpy), dir(_binary.numpy)
+            )
+        }
+    return attrs | globals().keys()
 
 
 def __getattr__(name):
     from ..core.operator import get_semiring
 
     if name in _delayed:
         func, kwargs = _delayed.pop(name)
```

### Comparing `python-graphblas-2023.3.0/graphblas/ss/_core.py` & `python-graphblas-2023.5.0/graphblas/ss/_core.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/tests/conftest.py` & `python-graphblas-2023.5.0/graphblas/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import atexit
 import functools
 import itertools
+import platform
 from pathlib import Path
 
 import numpy as np
 import pytest
 
 import graphblas as gb
+from graphblas.core import _supports_udfs as supports_udfs
 
 orig_binaryops = set()
 orig_semirings = set()
 
+pypy = platform.python_implementation() == "PyPy"
+
 
 def pytest_configure(config):
     rng = np.random.default_rng()
     randomly = config.getoption("--randomly", False)
     backend = config.getoption("--backend", None)
     if backend is None:
         if randomly:
@@ -44,15 +48,15 @@
         f"record={record}, mapnumpy={mapnumpy}, runslow={runslow}"
     )
     if record:
         rec = gb.Recorder()
         rec.start()
 
         def save_records():
-            with Path("record.txt").open("w") as f:  # pragma: no cover
+            with Path("record.txt").open("w") as f:  # pragma: no cover (???)
                 f.write("\n".join(rec.data))
 
         # I'm sure there's a `pytest` way to do this...
         atexit.register(save_records)
     orig_semirings.update(
         key
         for key in dir(gb.semiring)
@@ -112,7 +116,12 @@
             return func(*args, **kwargs)
 
     return inner
 
 
 def compute(x):
     return x
+
+
+def shouldhave(module, opname):
+    """Whether an "operator" module should have the given operator."""
+    return supports_udfs or hasattr(module, opname)
```

### Comparing `python-graphblas-2023.3.0/graphblas/tests/pickle1-vanilla.pkl` & `python-graphblas-2023.5.0/graphblas/tests/pickle1-vanilla.pkl`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/tests/pickle1.pkl` & `python-graphblas-2023.5.0/graphblas/tests/pickle1.pkl`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/tests/pickle2-vanilla.pkl` & `python-graphblas-2023.5.0/graphblas/tests/pickle2-vanilla.pkl`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/tests/pickle2.pkl` & `python-graphblas-2023.5.0/graphblas/tests/pickle2.pkl`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/tests/pickle3-vanilla.pkl` & `python-graphblas-2023.5.0/graphblas/tests/pickle3-vanilla.pkl`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/tests/pickle3.pkl` & `python-graphblas-2023.5.0/graphblas/tests/pickle3.pkl`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/tests/test_core.py` & `python-graphblas-2023.5.0/graphblas/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,14 @@
     # Currently assume s`pyproject.toml` is at the same level as `graphblas` folder.
     # This probably isn't always True, and we can probably do a better job of finding it.
     path = pathlib.Path(gb.__file__).parent
     pkgs = [f"graphblas.{x}" for x in setuptools.find_packages(str(path))]
     pkgs.append("graphblas")
     pkgs.sort()
     pyproject = path.parent / "pyproject.toml"
-    if not pyproject.exists():
+    if not pyproject.exists():  # pragma: no cover (safety)
         pytest.skip("Did not find pyproject.toml")
     with pyproject.open("rb") as f:
         pkgs2 = sorted(tomli.load(f)["tool"]["setuptools"]["packages"])
     assert (
         pkgs == pkgs2
     ), "If there are extra items on the left, add them to pyproject.toml:tool.setuptools.packages"
```

### Comparing `python-graphblas-2023.3.0/graphblas/tests/test_descriptor.py` & `python-graphblas-2023.5.0/graphblas/tests/test_descriptor.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/tests/test_dtype.py` & `python-graphblas-2023.5.0/graphblas/tests/test_dtype.py`

 * *Files 4% similar despite different names*

```diff
@@ -248,11 +248,8 @@
     if not is_win:
         assert dtypes._supports_complex
         return
 
     import suitesparse_graphblas as ssgb
     from packaging.version import parse
 
-    if parse(ssgb.__version__) < parse("7.4.3.1"):
-        assert not dtypes._supports_complex
-    else:
-        assert dtypes._supports_complex
+    assert dtypes._supports_complex == (parse(ssgb.__version__) >= parse("7.4.3.1"))
```

### Comparing `python-graphblas-2023.3.0/graphblas/tests/test_formatting.py` & `python-graphblas-2023.5.0/graphblas/tests/test_formatting.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,17 +36,16 @@
     is_style = False
     for line in lines[:-1]:
         if in_style:
             if line.startswith("</style>"):
                 # line = f"f'{{CSS_STYLE}}'"
                 in_style = False
                 is_style = True
-            else:  # pragma: no cover (???)
-                # This definitely gets covered, but why is it not picked up?
-                continue
+            else:
+                continue  # FLAKY COVERAGE
         if repr_name == "repr_html" and line.startswith("<style>"):
             prev_line = prev_line[:-1]  # remove "\n"
             in_style = True
             continue
 
         line = line + "\n"
         if line == prev_line:
@@ -5015,7 +5014,75 @@
     A = Matrix(int, 0, 5)
     repr_printer(A, "A")
     assert repr(A) == (
         '"M_1"      nvals  nrows  ncols  dtype  format\n'
         "gb.Matrix      0      0      5  INT64     csr\n"
         "---------------------------------------------"
     )
+
+
+@pytest.mark.skipif("not pd")
+def test_vector_as_matrix():
+    v = Vector.from_coo([1], [2], name="v_A")
+    A = v._as_matrix()
+    repr_printer(A, "A")
+    assert repr(A) == (
+        '"(GrB_Matrix)v_A"  nvals  nrows  ncols  dtype         format\n'
+        "gb.Matrix              1      2      1  INT64  bitmapc (iso)\n"
+        "------------------------------------------------------------\n"
+        "   0\n"
+        "0   \n"
+        "1  2"
+    )
+    html_printer(A, "A")
+    assert repr_html(A) == (
+        "<div>"
+        f"{CSS_STYLE}"
+        '<details open class="gb-arg-details"><summary class="gb-arg-summary"><tt>v<sub>A</sub></tt><div>\n'
+        '<table class="gb-info-table">\n'
+        "  <tr>\n"
+        '    <td rowspan="2" class="gb-info-name-cell"><pre>gb.Vector</pre></td>\n'
+        "    <td><pre>nvals</pre></td>\n"
+        "    <td><pre>size</pre></td>\n"
+        "    <td><pre>dtype</pre></td>\n"
+        "    <td><pre>format</pre></td>\n"
+        "  </tr>\n"
+        "  <tr>\n"
+        "    <td>1</td>\n"
+        "    <td>2</td>\n"
+        "    <td>INT64</td>\n"
+        "    <td>bitmap (iso)</td>\n"
+        "  </tr>\n"
+        "</table>\n"
+        "</div>\n"
+        "</summary><div>\n"
+        "<style scoped>\n"
+        "    .dataframe tbody tr th:only-of-type {\n"
+        "        vertical-align: middle;\n"
+        "    }\n"
+        "\n"
+        "    .dataframe tbody tr th {\n"
+        "        vertical-align: top;\n"
+        "    }\n"
+        "\n"
+        "    .dataframe thead th {\n"
+        "        text-align: right;\n"
+        "    }\n"
+        "</style>\n"
+        '<table border="1" class="dataframe">\n'
+        "  <thead>\n"
+        '    <tr style="text-align: right;">\n'
+        "      <th></th>\n"
+        "      <th>0</th>\n"
+        "      <th>1</th>\n"
+        "    </tr>\n"
+        "  </thead>\n"
+        "  <tbody>\n"
+        "    <tr>\n"
+        "      <th></th>\n"
+        "      <td></td>\n"
+        "      <td>2</td>\n"
+        "    </tr>\n"
+        "  </tbody>\n"
+        "</table>\n"
+        "</div></details></div>"
+    )
```

### Comparing `python-graphblas-2023.3.0/graphblas/tests/test_infix.py` & `python-graphblas-2023.5.0/graphblas/tests/test_infix.py`

 * *Files 2% similar despite different names*

```diff
@@ -356,7 +356,14 @@
     assert expr._value is None
     assert type(expr._get_value()) is Matrix
     assert type(expr._expr) is MatrixExpression
     assert type(expr.new()) is Matrix
     assert expr._expr is not None
     assert expr._value is None
     assert type(expr.new()) is Matrix
+    assert type(expr._get_value()) is Matrix
+    assert expr._expr is not None
+    assert expr._value is not None
+    assert expr._expr._value is not None
+    expr._value = None
+    assert expr._value is None
+    assert expr._expr._value is None
```

### Comparing `python-graphblas-2023.3.0/graphblas/tests/test_io.py` & `python-graphblas-2023.5.0/graphblas/tests/test_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,17 +263,21 @@
             continue
         mm_in = StringIO(getattr(test_mmio, example))
         if over64:
             with pytest.raises((OverflowError, ValueError)):
                 # fast_matrix_market v1.4.5 raises ValueError instead of OverflowError
                 M = gb.io.mmread(mm_in, engine)
         else:
-            if example == "_empty_lines_example" and engine in {"fmm", "auto"} and fmm is not None:
-                # TODO MAINT: is this a bug in fast_matrix_market, or does scipy.io.mmread
-                # read an invalid file? `fast_matrix_market` v1.4.5 does not handle this.
+            if (
+                example == "_empty_lines_example"
+                and engine in {"fmm", "auto"}
+                and fmm is not None
+                and fmm.__version__ in {"1.4.5"}
+            ):
+                # `fast_matrix_market` __version__ v1.4.5 does not handle this, but v1.5.0 does
                 continue
             M = gb.io.mmread(mm_in, engine)
             if not M.isequal(expected):  # pragma: no cover (debug)
                 print(example)
                 print("Expected:")
                 print(expected)
                 print("Got:")
```

### Comparing `python-graphblas-2023.3.0/graphblas/tests/test_mask.py` & `python-graphblas-2023.5.0/graphblas/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/tests/test_matrix.py` & `python-graphblas-2023.5.0/graphblas/tests/test_matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,27 +7,28 @@
 
 import numpy as np
 import pytest
 from numpy.testing import assert_array_equal
 
 import graphblas as gb
 from graphblas import agg, backend, binary, dtypes, indexunary, monoid, select, semiring, unary
+from graphblas.core import _supports_udfs as supports_udfs
 from graphblas.core import lib
 from graphblas.exceptions import (
     DimensionMismatch,
     DomainMismatch,
     EmptyObject,
     IndexOutOfBound,
     InvalidObject,
     InvalidValue,
     NotImplementedException,
     OutputNotEmpty,
 )
 
-from .conftest import autocompute, compute
+from .conftest import autocompute, compute, pypy, shouldhave
 
 from graphblas import Matrix, Scalar, Vector  # isort:skip (for dask-graphblas)
 
 suitesparse = backend == "suitesparse"
 
 
 @pytest.fixture
@@ -1226,14 +1227,16 @@
     w4 = indexunary.valueeq(A, s3).new()
     assert w1.isequal(A3)
     assert w2.isequal(A3)
     assert w3.isequal(A3)
     assert w4.isequal(A3)
     with pytest.raises(TypeError, match="left"):
         A.apply(select.valueeq, left=s3)
+    assert pickle.loads(pickle.dumps(indexunary.tril)) is indexunary.tril
+    assert pickle.loads(pickle.dumps(indexunary.tril[int])) is indexunary.tril[int]
 
 
 def test_select(A):
     A3 = Matrix.from_coo([0, 3, 3, 6], [3, 0, 2, 4], [3, 3, 3, 3], nrows=7, ncols=7)
     w1 = A.select(select.valueeq, 3).new()
     w1b = A.select(indexunary.valueeq, 3).new()
     w2 = A.select("==", 3).new()
@@ -1255,14 +1258,24 @@
         [0, 0, 1, 2, 4, 1], [1, 3, 4, 5, 5, 6], [2, 3, 8, 1, 7, 4], nrows=7, ncols=7
     )
     w7 = A.select("TRIU").new()
     assert w7.isequal(Aupper)
     with pytest.raises(TypeError, match="thunk"):
         A.select(select.valueeq, object())
 
+    A3rows = Matrix.from_coo([0, 0, 1, 1, 2], [1, 3, 4, 6, 5], [2, 3, 8, 4, 1], nrows=7, ncols=7)
+    w8 = select.rowle(A, 2).new()
+    w9 = A.select("row<=", 2).new()
+    w10 = select.row(A < 3).new()
+    assert w8.isequal(A3rows)
+    assert w9.isequal(A3rows)
+    assert w10.isequal(A3rows)
+    assert pickle.loads(pickle.dumps(select.tril)) is select.tril
+    assert pickle.loads(pickle.dumps(select.tril[bool])) is select.tril[bool]
+
 
 @autocompute
 def test_select_bools_and_masks(A):
     A3 = Matrix.from_coo([0, 3, 3, 6], [3, 0, 2, 4], [3, 3, 3, 3], nrows=7, ncols=7)
     # Select with boolean and masks
     w8 = A.select((A == 3).new()).new()
     assert w8.isequal(A3)
@@ -1279,24 +1292,35 @@
         A.select(w8.V, 777)
     with pytest.raises(TypeError, match="thunk"):
         A.select(A == 3, 777)
     with pytest.raises(TypeError):
         A.select(A[0, :].new().S)
 
 
+@pytest.mark.skipif("not supports_udfs")
 @pytest.mark.slow
 def test_indexunary_udf(A):
     def threex_minusthunk(x, row, col, thunk):  # pragma: no cover (numba)
         return 3 * x - thunk
 
-    indexunary.register_new("threex_minusthunk", threex_minusthunk)
+    assert indexunary.register_new("threex_minusthunk", threex_minusthunk) is not None
     assert hasattr(indexunary, "threex_minusthunk")
     assert not hasattr(select, "threex_minusthunk")
     with pytest.raises(ValueError, match="SelectOp must have BOOL return type"):
         select.register_anonymous(threex_minusthunk)
+    with pytest.raises(ValueError, match="SelectOp must have BOOL return type"):
+        select.register_new("bad_select", threex_minusthunk)
+    assert not hasattr(indexunary, "bad_select")
+    assert not hasattr(select, "bad_select")
+    assert select.register_new("bad_select", threex_minusthunk, lazy=True) is None
+    with pytest.raises(ValueError, match="SelectOp must have BOOL return type"):
+        select.bad_select
+    assert not hasattr(select, "bad_select")
+    assert hasattr(indexunary, "bad_select")  # Keep it
+
     expected = Matrix.from_coo(
         [3, 0, 3, 5, 6, 0, 6, 1, 6, 2, 4, 1],
         [0, 1, 2, 2, 2, 3, 3, 4, 4, 5, 5, 6],
         [5, 2, 5, -1, 11, 5, 17, 20, 5, -1, 17, 8],
     )
     result = indexunary.threex_minusthunk(A, 4).new()
     assert result.isequal(expected)
@@ -1304,14 +1328,16 @@
 
     def iii(x, row, col, thunk):  # pragma: no cover (numba)
         return (row + col) // 2 >= thunk
 
     select.register_new("iii", iii)
     assert hasattr(indexunary, "iii")
     assert hasattr(select, "iii")
+    assert indexunary.iii[int].orig_func is select.iii[int].orig_func is select.iii.orig_func
+    assert indexunary.iii[int]._numba_func is select.iii[int]._numba_func is select.iii._numba_func
     iii_apply = indexunary.register_anonymous(iii)
     expected = Matrix.from_coo(
         [3, 0, 3, 5, 6, 0, 6, 1, 6, 2, 4, 1],
         [0, 1, 2, 2, 2, 3, 3, 4, 4, 5, 5, 6],
         [False, False, True, True, True, False, True, True, True, True, True, True],
     )
     result = iii_apply(A, 2).new()
@@ -1349,23 +1375,25 @@
     assert w4.isequal(counts)
 
     Asquared = monoid.times(A & A).new()
     squared = Asquared.reduce_rowwise(monoid.plus).new()
     expected = unary.sqrt[float](squared).new()
     w5 = A.reduce_rowwise(agg.hypot).new()
     assert w5.isclose(expected)
-    w6 = A.reduce_rowwise(monoid.numpy.hypot[float]).new()
-    assert w6.isclose(expected)
+    if shouldhave(monoid.numpy, "hypot"):
+        w6 = A.reduce_rowwise(monoid.numpy.hypot[float]).new()
+        assert w6.isclose(expected)
     w7 = Vector(w5.dtype, size=w5.size)
     w7 << A.reduce_rowwise(agg.hypot)
     assert w7.isclose(expected)
 
     w8 = A.reduce_rowwise(agg.logaddexp).new()
-    expected = A.reduce_rowwise(monoid.numpy.logaddexp[float]).new()
-    assert w8.isclose(w8)
+    if shouldhave(monoid.numpy, "logaddexp"):
+        expected = A.reduce_rowwise(monoid.numpy.logaddexp[float]).new()
+        assert w8.isclose(w8)
 
     result = Vector.from_coo([0, 1, 2, 3, 4, 5, 6], [3, 2, 9, 10, 11, 8, 4])
     w9 = A.reduce_columnwise(agg.sum).new()
     assert w9.isequal(result)
     w10 = A.T.reduce_rowwise(agg.sum).new()
     assert w10.isequal(result)
 
@@ -1594,14 +1622,15 @@
             w = B.reduce_columnwise(aggr).new()
             assert we.isequal(w)
             if attr not in {"argmin", "argmax", "first_index", "last_index"}:
                 s = B.reduce_scalar(aggr).new()
                 assert compute(s.value) is None
 
 
+@pytest.mark.skipif("not supports_udfs")
 def test_reduce_row_udf(A):
     result = Vector.from_coo([0, 1, 2, 3, 4, 5, 6], [5, 12, 1, 6, 7, 1, 15])
 
     def plus(x, y):  # pragma: no cover (numba)
         return x + y
 
     binop = gb.core.operator.BinaryOp.register_anonymous(plus)
@@ -2003,14 +2032,20 @@
     assert_array_equal(d["row_indices"], [3, 0, 3, 5, 6, 0, 6, 1, 6, 2, 4, 1])
     if not do_iso:
         assert_array_equal(d["values"], [3, 2, 3, 1, 5, 3, 7, 8, 3, 1, 7, 4])
     if in_method == "import":
         B4 = Matrix.ss.import_any(**d)
         assert B4.isequal(A)
         assert B4.ss.is_iso is do_iso
+        if do_iso:
+            d["values"] = 1
+            d["is_iso"] = False
+            B4b = Matrix.ss.import_any(**d)
+            assert B4b.isequal(A)
+            assert B4b.ss.is_iso is True
     else:
         A4.ss.pack_any(**d)
         assert A4.isequal(A)
         assert A4.ss.is_iso is do_iso
 
     A5 = A.dup()
     d = getattr(A5.ss, out_method)("bitmapr")
@@ -2258,14 +2293,19 @@
 
 
 @pytest.mark.skipif("not suitesparse")
 def test_ss_import_on_view():
     A = Matrix.from_coo([0, 0, 1, 1], [0, 1, 0, 1], [1, 2, 3, 4])
     B = Matrix.ss.import_any(nrows=2, ncols=2, values=np.array([1, 2, 3, 4, 99, 99, 99])[:4])
     assert A.isequal(B)
+    values = np.arange(16).reshape(4, 4)[::2, ::2]
+    bitmap = np.ones((4, 4), dtype=bool)[::2, ::2]
+    C = Matrix.ss.import_any(values=values, bitmap=bitmap)
+    D = Matrix.ss.import_any(values=values.copy(), bitmap=bitmap.copy())
+    assert C.isequal(D)
 
 
 @pytest.mark.skipif("not suitesparse")
 def test_ss_import_export_empty():
     A = Matrix(int, 2, 3)
     A1 = A.dup()
     d = A1.ss.export("csr")
@@ -2898,26 +2938,27 @@
         "from_dicts",
         "from_edgelist",
         "from_scalar",
         "from_values",
         "resize",
         "update",
     }
-    assert attrs - expr_attrs == expected, (
+    ignore = {"__sizeof__"}
+    assert attrs - expr_attrs - ignore == expected, (
         "If you see this message, you probably added a method to Matrix.  You may need to "
         "add an entry to `matrix` or `matrix_vector` set in `graphblas.core.automethods` "
         "and then run `python -m graphblas.core.automethods`.  If you're messing with infix "
         "methods, then you may need to run `python -m graphblas.core.infixmethods`."
     )
-    assert attrs - infix_attrs == expected
+    assert attrs - infix_attrs - ignore == expected
     # TransposedMatrix is used differently than other expressions,
     # so maybe it shouldn't support everything.
     if suitesparse:
         expected.add("ss")
-    assert attrs - transposed_attrs == (expected | {"_as_vector", "S", "V"}) - {
+    assert attrs - transposed_attrs - ignore == (expected | {"_as_vector", "S", "V"}) - {
         "_prep_for_extract",
         "_extract_element",
     }
     # Make sure signatures actually match
     skip = {"__init__", "__repr__", "_repr_html_"}
     for expr in [binary.times(B & B), B & B, B.T]:
         print(type(expr).__name__)
@@ -2961,15 +3002,16 @@
         "from_dense",
         "from_dicts",
         "from_edgelist",
         "from_values",
         "from_scalar",
         "resize",
     }
-    assert attrs - expr_attrs == expected, (
+    ignore = {"__sizeof__"}
+    assert attrs - expr_attrs - ignore == expected, (
         "If you see this message, you probably added a method to Matrix.  You may need to "
         "add an entry to `matrix` or `matrix_vector` set in `graphblas.core.automethods` "
         "and then run `python -m graphblas.core.automethods`.  If you're messing with infix "
         "methods, then you may need to run `python -m graphblas.core.infixmethods`."
     )
     # Make sure signatures actually match. `update` has different docstring.
     skip = {"__call__", "__init__", "__repr__", "_repr_html_", "update"}
@@ -3106,18 +3148,20 @@
     assert binary.plus(1, A).isequal(1 + A)
     assert binary.minus(A, 1).isequal(A - 1)
     assert binary.minus(1, A).isequal(1 - A)
     assert binary.times(A, 2).isequal(A * 2)
     assert binary.times(2, A).isequal(2 * A)
     assert binary.truediv(A, 2).isequal(A / 2)
     assert binary.truediv(5, A).isequal(5 / A)
-    assert binary.floordiv(A, 2).isequal(A // 2)
-    assert binary.floordiv(5, A).isequal(5 // A)
-    assert binary.numpy.mod(A, 2).isequal(A % 2)
-    assert binary.numpy.mod(5, A).isequal(5 % A)
+    if shouldhave(binary, "floordiv"):
+        assert binary.floordiv(A, 2).isequal(A // 2)
+        assert binary.floordiv(5, A).isequal(5 // A)
+    if shouldhave(binary.numpy, "mod"):
+        assert binary.numpy.mod(A, 2).isequal(A % 2)
+        assert binary.numpy.mod(5, A).isequal(5 % A)
     assert binary.pow(A, 2).isequal(A**2)
     assert binary.pow(2, A).isequal(2**A)
     assert binary.pow(A, 2).isequal(pow(A, 2))
     assert unary.ainv(A).isequal(-A)
     assert unary.ainv(A.T).isequal(-A.T)
     B = A.dup(dtype=bool)
     assert unary.lnot(B).isequal(~B)
@@ -3136,34 +3180,35 @@
         6 ^ B
     assert binary.lt(A, 4).isequal(A < 4)
     assert binary.le(A, 4).isequal(A <= 4)
     assert binary.gt(A, 4).isequal(A > 4)
     assert binary.ge(A, 4).isequal(A >= 4)
     assert binary.eq(A, 4).isequal(A == 4)
     assert binary.ne(A, 4).isequal(A != 4)
-    x, y = divmod(A, 3)
-    assert binary.floordiv(A, 3).isequal(x)
-    assert binary.numpy.mod(A, 3).isequal(y)
-    assert binary.fmod(A, 3).isequal(y)
-    assert A.isequal(binary.plus((3 * x) & y))
-    x, y = divmod(-A, 3)
-    assert binary.floordiv(-A, 3).isequal(x)
-    assert binary.numpy.mod(-A, 3).isequal(y)
-    # assert binary.fmod(-A, 3).isequal(y)  # The reason we use numpy.mod
-    assert (-A).isequal(binary.plus((3 * x) & y))
-    x, y = divmod(3, A)
-    assert binary.floordiv(3, A).isequal(x)
-    assert binary.numpy.mod(3, A).isequal(y)
-    assert binary.fmod(3, A).isequal(y)
-    assert binary.plus(binary.times(A & x) & y).isequal(3 * unary.one(A))
-    x, y = divmod(-3, A)
-    assert binary.floordiv(-3, A).isequal(x)
-    assert binary.numpy.mod(-3, A).isequal(y)
-    # assert binary.fmod(-3, A).isequal(y)  # The reason we use numpy.mod
-    assert binary.plus(binary.times(A & x) & y).isequal(-3 * unary.one(A))
+    if shouldhave(binary, "floordiv") and shouldhave(binary.numpy, "mod"):
+        x, y = divmod(A, 3)
+        assert binary.floordiv(A, 3).isequal(x)
+        assert binary.numpy.mod(A, 3).isequal(y)
+        assert binary.fmod(A, 3).isequal(y)
+        assert A.isequal(binary.plus((3 * x) & y))
+        x, y = divmod(-A, 3)
+        assert binary.floordiv(-A, 3).isequal(x)
+        assert binary.numpy.mod(-A, 3).isequal(y)
+        # assert binary.fmod(-A, 3).isequal(y)  # The reason we use numpy.mod
+        assert (-A).isequal(binary.plus((3 * x) & y))
+        x, y = divmod(3, A)
+        assert binary.floordiv(3, A).isequal(x)
+        assert binary.numpy.mod(3, A).isequal(y)
+        assert binary.fmod(3, A).isequal(y)
+        assert binary.plus(binary.times(A & x) & y).isequal(3 * unary.one(A))
+        x, y = divmod(-3, A)
+        assert binary.floordiv(-3, A).isequal(x)
+        assert binary.numpy.mod(-3, A).isequal(y)
+        # assert binary.fmod(-3, A).isequal(y)  # The reason we use numpy.mod
+        assert binary.plus(binary.times(A & x) & y).isequal(-3 * unary.one(A))
 
     assert binary.eq(A & A).isequal(A == A)
     assert binary.ne(A.T & A.T).isequal(A.T != A.T)
     assert binary.lt(A & A.T).isequal(A < A.T)
     assert binary.ge(A.T & A).isequal(A.T >= A)
 
     B = A.dup()
@@ -3178,22 +3223,24 @@
     B *= 2
     assert type(B) is Matrix
     assert binary.times(A, 2).isequal(B)
     B = A.dup(dtype=float)
     B /= 2
     assert type(B) is Matrix
     assert binary.truediv(A, 2).isequal(B)
-    B = A.dup()
-    B //= 2
-    assert type(B) is Matrix
-    assert binary.floordiv(A, 2).isequal(B)
-    B = A.dup()
-    B %= 2
-    assert type(B) is Matrix
-    assert binary.numpy.mod(A, 2).isequal(B)
+    if shouldhave(binary, "floordiv"):
+        B = A.dup()
+        B //= 2
+        assert type(B) is Matrix
+        assert binary.floordiv(A, 2).isequal(B)
+    if shouldhave(binary.numpy, "mod"):
+        B = A.dup()
+        B %= 2
+        assert type(B) is Matrix
+        assert binary.numpy.mod(A, 2).isequal(B)
     B = A.dup()
     B **= 2
     assert type(B) is Matrix
     assert binary.pow(A, 2).isequal(B)
     B = A.dup(dtype=bool)
     B ^= True
     assert type(B) is Matrix
@@ -3516,15 +3563,15 @@
     assert A.ndim == 2
     assert A.ewise_mult(A).ndim == 2
     assert (A & A).ndim == 2
     assert (A @ A).ndim == 2
 
 
 def test_sizeof(A):
-    if suitesparse:
+    if suitesparse and not pypy:
         assert sys.getsizeof(A) > A.nvals * 16
     else:
         with pytest.raises(TypeError):
             sys.getsizeof(A)
 
 
 def test_ewise_union():
@@ -3603,14 +3650,15 @@
     assert len(list(A.ss.iterkeys(-N))) == N
     assert len(list(A.ss.itervalues(-N - 1))) == N
     assert next(A.ss.iterkeys()) in A
     assert next(A.ss.itervalues()) is not None
     assert next(A.ss.iteritems()) is not None
 
 
+@pytest.mark.skipif("not supports_udfs")
 @pytest.mark.slow
 def test_udt():
     record_dtype = np.dtype([("x", np.bool_), ("y", np.float64)], align=True)
     udt = dtypes.register_anonymous(record_dtype, "MatrixUDT")
     A = Matrix(udt, nrows=2, ncols=2)
     a = np.zeros(1, dtype=record_dtype)
     A[0, 0] = a[0]
@@ -3913,15 +3961,15 @@
     A.ss.config["format"] = lib.GxB_BY_ROW
     assert A.ss.config["format"] == "by_row"
     with pytest.raises(InvalidValue):
         A.ss.config["format"] = lib.GxB_NO_FORMAT
 
 
 def test_to_csr_from_csc(A):
-    assert Matrix.from_csr(*A.to_csr(dtype=int)).isequal(A, check_dtype=True)
+    assert Matrix.from_csr(*A.to_csr(sort=False, dtype=int)).isequal(A, check_dtype=True)
     assert Matrix.from_csr(*A.T.to_csc()).isequal(A, check_dtype=True)
     assert Matrix.from_csc(*A.to_csc()).isequal(A)
     assert Matrix.from_csc(*A.T.to_csr()).isequal(A)
     assert Matrix.from_csr(*A.to_csr(dtype=float)).isequal(A.dup(float), check_dtype=True)
 
     #    0 1 2
     # 0 [- 1 -]
@@ -4122,15 +4170,19 @@
     with pytest.raises(TypeError, match="missing"):
         Matrix.from_scalar(1, nrows=2)
     with pytest.raises(TypeError, match="Literal scalars also accepted"):
         Matrix.from_scalar(A, nrows=2, ncols=3)
     A = Matrix.from_scalar(1, dtype="INT64[2]", nrows=3, ncols=4)
     B = Matrix("INT64[2]", nrows=3, ncols=4)
     B << [1, 1]
-    assert A.isequal(B, check_dtype=True)
+    if supports_udfs:
+        assert A.isequal(B, check_dtype=True)
+    else:
+        with pytest.raises(KeyError, match="eq does not work with"):
+            assert A.isequal(B, check_dtype=True)
 
 
 def test_to_dense_from_dense():
     A = Matrix.from_dense(np.arange(6).reshape(2, 3))
     B = Matrix.from_coo([0, 0, 0, 1, 1, 1], [0, 1, 2, 0, 1, 2], np.arange(6))
     assert A.isequal(B, check_dtype=True)
     assert_array_equal(A.to_dense(dtype=int), [[0, 1, 2], [3, 4, 5]])
@@ -4248,15 +4300,15 @@
         # Bad option should show list of valid options
         with pytest.raises(ValueError, match="nthreads"):
             C1(bad_opt=True) << A
         with pytest.raises(ValueError, match="Duplicate descriptor"):
             (A @ A).new(nthreads=4, Nthreads=5)
         with pytest.raises(ValueError, match="escriptor"):
             A[0, 0].new(bad_opt=True)
-        A[0, 0].new(nthreads=4)  # ignored, but okay
+        A[0, 0].new(nthreads=4, sort=None)  # ignored, but okay
         with pytest.raises(ValueError, match="escriptor"):
             A.__setitem__((0, 0), 1, bad_opt=True)
         A.__setitem__((0, 0), 1, nthreads=4)  # ignored, but okay
         with pytest.raises(ValueError, match="escriptor"):
             A.dup(bad_opt=True)
         A.dup(nthreads=4)
         # These are interesting cases: we auto-compute a value, then provide custom descriptor
@@ -4282,14 +4334,15 @@
 
 @autocompute
 def test_wait_chains(A):
     result = A.wait().T.wait().reduce_rowwise().wait().reduce().wait()
     assert result == 47
 
 
+@pytest.mark.skipif("not supports_udfs")
 def test_subarray_dtypes():
     a = np.arange(3 * 4, dtype=np.int64).reshape(3, 4)
     A = Matrix.from_coo([1, 3, 5], [0, 1, 3], a)
     B = Matrix("INT64[4]", nrows=6, ncols=4)
     B[1, 0] = [0, 1, 2, 3]
     B[3, 1] = [4, 5, 6, 7]
     B[5, 3] = [8, 9, 10, 11]
```

### Comparing `python-graphblas-2023.3.0/graphblas/tests/test_numpyops.py` & `python-graphblas-2023.5.0/graphblas/tests/test_numpyops.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,30 +7,33 @@
 import pytest
 
 import graphblas as gb
 import graphblas.binary.numpy as npbinary
 import graphblas.monoid.numpy as npmonoid
 import graphblas.semiring.numpy as npsemiring
 import graphblas.unary.numpy as npunary
-from graphblas import Vector, backend
+from graphblas import Vector, backend, config
+from graphblas.core import _supports_udfs as supports_udfs
 from graphblas.dtypes import _supports_complex
 
-from .conftest import compute
+from .conftest import compute, shouldhave
 
 is_win = sys.platform.startswith("win")
 suitesparse = backend == "suitesparse"
 
 
 def test_numpyops_dir():
-    assert "exp2" in dir(npunary)
-    assert "logical_and" in dir(npbinary)
-    assert "logaddexp" in dir(npmonoid)
-    assert "add_add" in dir(npsemiring)
+    udf_or_mapped = supports_udfs or config["mapnumpy"]
+    assert ("exp2" in dir(npunary)) == udf_or_mapped
+    assert ("logical_and" in dir(npbinary)) == udf_or_mapped
+    assert ("logaddexp" in dir(npmonoid)) == supports_udfs
+    assert ("add_add" in dir(npsemiring)) == udf_or_mapped
 
 
+@pytest.mark.skipif("not supports_udfs")
 @pytest.mark.slow
 def test_bool_doesnt_get_too_large():
     a = Vector.from_coo([0, 1, 2, 3], [True, False, True, False])
     b = Vector.from_coo([0, 1, 2, 3], [True, True, False, False])
     if gb.config["mapnumpy"]:
         with pytest.raises(KeyError, match="plus does not work with BOOL"):
             z = a.ewise_mult(b, gb.monoid.numpy.add).new()
@@ -66,17 +69,20 @@
         "FC64": {"ceil", "floor", "trunc"},
     }
     if suitesparse and is_win and gb.config["mapnumpy"]:
         # asin and asinh are known to be wrong in SuiteSparse:GraphBLAS
         # due to limitation of MSVC with complex
         blocklist["FC64"].update({"arcsin", "arcsinh"})
         blocklist["FC32"] = {"arcsin", "arcsinh"}
-    isclose = gb.binary.isclose(1e-6, 0)
+    if shouldhave(gb.binary, "isclose"):
+        isclose = gb.binary.isclose(1e-6, 0)
+    else:
+        isclose = None
     for gb_input, np_input in data:
-        for unary_name in sorted(npunary._unary_names):
+        for unary_name in sorted(npunary._unary_names & npunary.__dir__()):
             op = getattr(npunary, unary_name)
             if gb_input.dtype not in op.types or unary_name in blocklist.get(
                 gb_input.dtype.name, ()
             ):
                 continue
             if gb_input.dtype.name.startswith("FC"):
                 # There are some nasty branch cuts as 1
@@ -95,14 +101,16 @@
                         compare_op = isclose
                     else:
                         compare_op = npbinary.equal
             np_result = Vector.from_coo(
                 list(range(np_input.size)), list(np_result), dtype=gb_result.dtype
             )
             assert gb_result.nvals == np_result.size
+            if compare_op is None:
+                continue  # FLAKY COVERAGE
             match = gb_result.ewise_mult(np_result, compare_op).new()
             if gb_result.dtype.name.startswith("F"):
                 match(accum=gb.binary.lor) << gb_result.apply(npunary.isnan)
             compare = match.reduce(gb.monoid.land).new()
             if not compare:  # pragma: no cover (debug)
                 print(unary_name, gb_input.dtype)
                 print(compute(gb_result))
@@ -145,17 +153,32 @@
                 [np.array(values1, dtype=np.complex128), np.array(values2, dtype=np.complex128)],
             ],
         )
     blocklist = {
         "FP64": {"floor_divide"},  # numba/numpy difference for 1.0 / 0.0
         "BOOL": {"gcd", "lcm", "subtract"},  # not supported by numpy
     }
-    isclose = gb.binary.isclose(1e-7, 0)
+    if shouldhave(gb.binary, "isclose"):
+        isclose = gb.binary.isclose(1e-7, 0)
+    else:
+        isclose = None
+    if shouldhave(npbinary, "equal"):
+        equal = npbinary.equal
+    else:
+        equal = gb.binary.eq
+    if shouldhave(npbinary, "isnan"):
+        isnan = npunary.isnan
+    else:
+        isnan = gb.unary.isnan
+    if shouldhave(npbinary, "isinf"):
+        isinf = npunary.isinf
+    else:
+        isinf = gb.unary.isinf
     for (gb_left, gb_right), (np_left, np_right) in data:
-        for binary_name in sorted(npbinary._binary_names):
+        for binary_name in sorted(npbinary._binary_names & npbinary.__dir__()):
             op = getattr(npbinary, binary_name)
             if gb_left.dtype not in op.types or binary_name in blocklist.get(
                 gb_left.dtype.name, ()
             ):
                 continue
             if is_win and binary_name == "ldexp":
                 # On Windows, the second argument must be int32 or less (I'm not sure why)
@@ -167,28 +190,30 @@
                         np_result = getattr(np, binary_name)(np_left, np_right, dtype="float32")
                         compare_op = isclose
                     else:
                         np_result = getattr(np, binary_name)(np_left, np_right)
                         if binary_name in {"arctan2"}:
                             compare_op = isclose
                         else:
-                            compare_op = npbinary.equal
+                            compare_op = equal
                 except Exception:  # pragma: no cover (debug)
                     print(f"Error computing numpy result for {binary_name}")
                     print(f"dtypes: ({gb_left.dtype}, {gb_right.dtype}) -> {gb_result.dtype}")
                     raise
             np_result = Vector.from_coo(np.arange(np_left.size), np_result, dtype=gb_result.dtype)
 
             assert gb_result.nvals == np_result.size
+            if compare_op is None:
+                continue  # FLAKY COVERAGE
             match = gb_result.ewise_mult(np_result, compare_op).new()
             if gb_result.dtype.name.startswith("F"):
-                match(accum=gb.binary.lor) << gb_result.apply(npunary.isnan)
+                match(accum=gb.binary.lor) << gb_result.apply(isnan)
             if gb_result.dtype.name.startswith("FC"):
                 # Divide by 0j sometimes result in different behavior, such as `nan` or `(inf+0j)`
-                match(accum=gb.binary.lor) << gb_result.apply(npunary.isinf)
+                match(accum=gb.binary.lor) << gb_result.apply(isinf)
             compare = match.reduce(gb.monoid.land).new()
             if not compare:  # pragma: no cover (debug)
                 print(compare_op)
                 print(binary_name)
                 print(compute(gb_left))
                 print(compute(gb_right))
                 print(compute(gb_result))
@@ -219,15 +244,15 @@
                 Vector.from_coo([0, 1, 2, 3], [True, False, True, False]),
                 Vector.from_coo([0, 1, 2, 3], [True, True, False, False]),
             ],
             [np.array([True, False, True, False]), np.array([True, True, False, False])],
         ],
     ]
     # Complex monoids not working yet (they segfault upon creation in gb.core.operators)
-    if _supports_complex:  # pragma: no branch
+    if _supports_complex:
         data.append(
             [
                 [
                     Vector.from_coo(index, values1, dtype="FC64"),
                     Vector.from_coo(index, values2, dtype="FC64"),
                 ],
                 [
@@ -237,21 +262,21 @@
             ]
         )
     blocklist = {}
     reduction_blocklist = {
         "BOOL": {"add"},
     }
     for (gb_left, gb_right), (np_left, np_right) in data:
-        for binary_name in sorted(npmonoid._monoid_identities):
+        for binary_name in sorted(npmonoid._monoid_identities.keys() & npmonoid.__dir__()):
             op = getattr(npmonoid, binary_name)
             assert len(op.types) > 0, op.name
             if gb_left.dtype not in op.types or binary_name in blocklist.get(
                 gb_left.dtype.name, ()
-            ):  # pragma: no cover (flaky)
-                continue
+            ):
+                continue  # FLAKY COVERAGE
             with np.errstate(divide="ignore", over="ignore", under="ignore", invalid="ignore"):
                 gb_result = gb_left.ewise_mult(gb_right, op).new()
                 np_result = getattr(np, binary_name)(np_left, np_right)
             np_result = Vector.from_coo(np.arange(np_left.size), np_result, dtype=gb_result.dtype)
             assert gb_result.nvals == np_result.size
             match = gb_result.ewise_mult(np_result, npbinary.equal).new()
             if gb_result.dtype.name.startswith("F"):
@@ -275,15 +300,16 @@
             np_result = getattr(np, binary_name).reduce(np_right)
             assert gb_result.value == np_result
 
 
 @pytest.mark.slow
 def test_npsemiring():
     for monoid_name, binary_name in itertools.product(
-        sorted(npmonoid._monoid_identities), sorted(npbinary._binary_names)
+        sorted(npmonoid._monoid_identities.keys() & npmonoid.__dir__()),
+        sorted(npbinary._binary_names & npbinary.__dir__()),
     ):
         monoid = getattr(npmonoid, monoid_name)
         binary = getattr(npbinary, binary_name)
         name = monoid.name.split(".")[-1] + "_" + binary.name.split(".")[-1]
         if name in {"eq_pow", "eq_minus"}:
             continue
         semiring = gb.core.operator.Semiring.register_anonymous(monoid, binary, name)
```

### Comparing `python-graphblas-2023.3.0/graphblas/tests/test_op.py` & `python-graphblas-2023.5.0/graphblas/tests/test_op.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 import itertools
 
 import numpy as np
 import pytest
 
 import graphblas as gb
-from graphblas import agg, backend, binary, dtypes, indexunary, monoid, op, select, semiring, unary
+from graphblas import (
+    agg,
+    backend,
+    binary,
+    config,
+    dtypes,
+    indexunary,
+    monoid,
+    op,
+    select,
+    semiring,
+    unary,
+)
+from graphblas.core import _supports_udfs as supports_udfs
 from graphblas.core import lib, operator
 from graphblas.core.operator import BinaryOp, IndexUnaryOp, Monoid, Semiring, UnaryOp, get_semiring
 from graphblas.dtypes import (
     BOOL,
     FP32,
     FP64,
     INT8,
@@ -18,14 +31,16 @@
     UINT8,
     UINT16,
     UINT32,
     UINT64,
 )
 from graphblas.exceptions import DomainMismatch, UdfParseError
 
+from .conftest import shouldhave
+
 if dtypes._supports_complex:
     from graphblas.dtypes import FC32, FC64
 
 from graphblas import Matrix, Vector  # isort:skip (for dask-graphblas)
 
 suitesparse = backend == "suitesparse"
 
@@ -138,22 +153,53 @@
     with pytest.raises(ValueError, match="Unknown binary or aggregator"):
         operator.get_typed_op("bad_op_name", dtypes.INT64, kind="binary|aggregator")
     with pytest.raises(AttributeError):
         # get_typed_op expects dtypes to already be dtypes
         operator.get_typed_op(binary.plus, dtypes.INT64, "bad dtype")
 
 
+@pytest.mark.skipif("supports_udfs")
+def test_udf_mentions_numba():
+    with pytest.raises(AttributeError, match="install numba"):
+        binary.rfloordiv
+    assert "rfloordiv" not in dir(binary)
+    with pytest.raises(AttributeError, match="install numba"):
+        semiring.any_rfloordiv
+    assert "any_rfloordiv" not in dir(semiring)
+    with pytest.raises(AttributeError, match="install numba"):
+        op.absfirst
+    assert "absfirst" not in dir(op)
+    with pytest.raises(AttributeError, match="install numba"):
+        op.plus_rpow
+    assert "plus_rpow" not in dir(op)
+    with pytest.raises(AttributeError, match="install numba"):
+        binary.numpy.gcd
+    assert "gcd" not in dir(binary.numpy)
+    assert "gcd" not in dir(op.numpy)
+
+
+@pytest.mark.skipif("supports_udfs")
+def test_unaryop_udf_no_support():
+    def plus_one(x):  # pragma: no cover (numba)
+        return x + 1
+
+    with pytest.raises(RuntimeError, match="UnaryOp.register_new.* unavailable"):
+        unary.register_new("plus_one", plus_one)
+
+
+@pytest.mark.skipif("not supports_udfs")
 def test_unaryop_udf():
     def plus_one(x):
         return x + 1  # pragma: no cover (numba)
 
     unary.register_new("plus_one", plus_one)
     assert hasattr(unary, "plus_one")
     assert unary.plus_one.orig_func is plus_one
     assert unary.plus_one[int].orig_func is plus_one
+    assert unary.plus_one[int]._numba_func(1) == 2
     comp_set = {
         INT8,
         INT16,
         INT32,
         INT64,
         UINT8,
         UINT16,
@@ -178,14 +224,15 @@
     with pytest.raises(TypeError, match="UDF argument must be a function"):
         UnaryOp.register_new("bad", object())
     assert not hasattr(unary, "bad")
     with pytest.raises(UdfParseError, match="Unable to parse function using Numba"):
         UnaryOp.register_new("bad", lambda x: v)
 
 
+@pytest.mark.skipif("not supports_udfs")
 @pytest.mark.slow
 def test_unaryop_parameterized():
     def plus_x(x=0):
         def inner(val):
             return val + x  # pragma: no cover (numba)
 
         return inner
@@ -203,14 +250,15 @@
     UnaryOp._initialize()  # no-op
     UnaryOp.register_new("plus_x_parameterized", plus_x, parameterized=True)
     op = unary.plus_x_parameterized
     v11 = v.apply(op(x=10)["INT32"]).new()
     assert r10.isequal(v11, check_dtype=True)
 
 
+@pytest.mark.skipif("not supports_udfs")
 @pytest.mark.slow
 def test_binaryop_parameterized():
     def plus_plus_x(x=0):
         def inner(left, right):
             return left + right + x  # pragma: no cover (numba)
 
         return inner
@@ -264,14 +312,15 @@
     def my_add(x, y):
         return x + y  # pragma: no cover (numba)
 
     op = BinaryOp.register_anonymous(my_add)
     assert op.name == "my_add"
 
 
+@pytest.mark.skipif("not supports_udfs")
 @pytest.mark.slow
 def test_monoid_parameterized():
     def plus_plus_x(x=0):
         def inner(left, right):
             return left + right + x  # pragma: no cover (numba)
 
         return inner
@@ -359,14 +408,15 @@
         bin_op, bad_identity, is_idempotent=True, name="broken_monoid"
     )
     assert bin_op.monoid is monoid
     assert bin_op(1).monoid is None
     assert monoid.is_idempotent
 
 
+@pytest.mark.skipif("not supports_udfs")
 @pytest.mark.slow
 def test_semiring_parameterized():
     def plus_plus_x(x=0):
         def inner(left, right):
             return left + right + x  # pragma: no cover (numba)
 
         return inner
@@ -486,14 +536,15 @@
 
     assert A.reduce_scalar(bin_op).new() == A.reduce_scalar(binary.plus).new()
 
     B = A.kronecker(A, bin_op).new()
     assert B.isequal(A.kronecker(A, binary.plus).new())
 
 
+@pytest.mark.skipif("not supports_udfs")
 def test_unaryop_udf_bool_result():
     # numba has trouble compiling this, but we have a work-around
     def is_positive(x):
         return x > 0  # pragma: no cover (numba)
 
     UnaryOp.register_new("is_positive", is_positive)
     assert hasattr(unary, "is_positive")
@@ -512,20 +563,22 @@
     }
     v = Vector.from_coo([0, 1, 3], [1, 2, -4], dtype=dtypes.INT32)
     w = v.apply(unary.is_positive).new()
     result = Vector.from_coo([0, 1, 3], [True, True, False], dtype=dtypes.BOOL)
     assert w.isequal(result)
 
 
+@pytest.mark.skipif("not supports_udfs")
 def test_binaryop_udf():
     def times_minus_sum(x, y):
         return x * y - (x + y)  # pragma: no cover (numba)
 
     BinaryOp.register_new("bin_test_func", times_minus_sum)
     assert hasattr(binary, "bin_test_func")
+    assert binary.bin_test_func[int].orig_func is times_minus_sum
     comp_set = {
         BOOL,  # goes to INT64
         INT8,
         INT16,
         INT32,
         INT64,
         UINT8,
@@ -541,14 +594,15 @@
     v1 = Vector.from_coo([0, 1, 3], [1, 2, -4], dtype=dtypes.INT32)
     v2 = Vector.from_coo([0, 2, 3], [2, 3, 7], dtype=dtypes.INT32)
     w = v1.ewise_add(v2, binary.bin_test_func).new()
     result = Vector.from_coo([0, 1, 2, 3], [-1, 2, 3, -31], dtype=dtypes.INT32)
     assert w.isequal(result)
 
 
+@pytest.mark.skipif("not supports_udfs")
 def test_monoid_udf():
     def plus_plus_one(x, y):
         return x + y + 1  # pragma: no cover (numba)
 
     BinaryOp.register_new("plus_plus_one", plus_plus_one)
     Monoid.register_new("plus_plus_one", binary.plus_plus_one, -1)
     assert hasattr(monoid, "plus_plus_one")
@@ -575,14 +629,15 @@
 
     with pytest.raises(DomainMismatch):
         Monoid.register_anonymous(binary.plus_plus_one, {"BOOL": True})
     with pytest.raises(DomainMismatch):
         Monoid.register_anonymous(binary.plus_plus_one, {"BOOL": -1})
 
 
+@pytest.mark.skipif("not supports_udfs")
 @pytest.mark.slow
 def test_semiring_udf():
     def plus_plus_two(x, y):
         return x + y + 2  # pragma: no cover (numba)
 
     BinaryOp.register_new("plus_plus_two", plus_plus_two)
     Semiring.register_new("extra_twos", monoid.plus, binary.plus_plus_two)
@@ -604,18 +659,20 @@
     vec1 = Vector.from_coo([0], [1], dtype=dtypes.INT64)
     vec2 = Vector.from_coo([0], [2], dtype=dtypes.INT64)
     result = vec1.ewise_mult(vec2, binary.truediv).new()
     assert result.isclose(Vector.from_coo([0], [0.5], dtype=dtypes.FP64), check_dtype=True)
     vec4 = Vector.from_coo([0], [-3], dtype=dtypes.INT64)
     result2 = vec4.ewise_mult(vec2, binary.cdiv).new()
     assert result2.isequal(Vector.from_coo([0], [-1], dtype=dtypes.INT64), check_dtype=True)
-    result3 = vec4.ewise_mult(vec2, binary.floordiv).new()
-    assert result3.isequal(Vector.from_coo([0], [-2], dtype=dtypes.INT64), check_dtype=True)
+    if shouldhave(binary, "floordiv"):
+        result3 = vec4.ewise_mult(vec2, binary.floordiv).new()
+        assert result3.isequal(Vector.from_coo([0], [-2], dtype=dtypes.INT64), check_dtype=True)
 
 
+@pytest.mark.skipif("not supports_udfs")
 @pytest.mark.slow
 def test_nested_names():
     def plus_three(x):
         return x + 3  # pragma: no cover (numba)
 
     UnaryOp.register_new("incrementers.plus_three", plus_three)
     assert hasattr(unary, "incrementers")
@@ -667,20 +724,25 @@
 @pytest.mark.slow
 def test_op_namespace():
     assert op.abs is unary.abs
     assert op.minus is binary.minus
     assert op.plus is binary.plus
     assert op.plus_times is semiring.plus_times
 
-    assert op.numpy.fabs is unary.numpy.fabs
-    assert op.numpy.subtract is binary.numpy.subtract
-    assert op.numpy.add is binary.numpy.add
-    assert op.numpy.add_add is semiring.numpy.add_add
+    if shouldhave(unary.numpy, "fabs"):
+        assert op.numpy.fabs is unary.numpy.fabs
+    if shouldhave(binary.numpy, "subtract"):
+        assert op.numpy.subtract is binary.numpy.subtract
+    if shouldhave(binary.numpy, "add"):
+        assert op.numpy.add is binary.numpy.add
+    if shouldhave(semiring.numpy, "add_add"):
+        assert op.numpy.add_add is semiring.numpy.add_add
     assert len(dir(op)) > 300
-    assert len(dir(op.numpy)) > 500
+    if supports_udfs:
+        assert len(dir(op.numpy)) > 500
 
     with pytest.raises(
         AttributeError, match="module 'graphblas.op.numpy' has no attribute 'bad_attr'"
     ):
         op.numpy.bad_attr
 
     # Make sure all have been initialized so `vars` below works
@@ -736,42 +798,53 @@
     assert indexunarynames - opnames == indexunarynames, indexunarynames - opnames
     assert selectnames - opnames == selectnames, selectnames - opnames
 
 
 @pytest.mark.slow
 def test_binaryop_attributes_numpy():
     # Some coverage from this test depends on order of tests
-    assert binary.numpy.add[int].monoid is monoid.numpy.add[int]
-    assert binary.numpy.subtract[int].monoid is None
-    assert binary.numpy.add.monoid is monoid.numpy.add
-    assert binary.numpy.subtract.monoid is None
+    if shouldhave(monoid.numpy, "add"):
+        assert binary.numpy.add[int].monoid is monoid.numpy.add[int]
+        assert binary.numpy.add.monoid is monoid.numpy.add
+    if shouldhave(binary.numpy, "subtract"):
+        assert binary.numpy.subtract[int].monoid is None
+        assert binary.numpy.subtract.monoid is None
+
+
+@pytest.mark.skipif("not supports_udfs")
+@pytest.mark.slow
+def test_binaryop_monoid_numpy():
+    assert gb.binary.numpy.minimum[int].monoid is gb.monoid.numpy.minimum[int]
 
 
 @pytest.mark.slow
 def test_binaryop_attributes():
     assert binary.plus[int].monoid is monoid.plus[int]
     assert binary.minus[int].monoid is None
     assert binary.plus.monoid is monoid.plus
     assert binary.minus.monoid is None
 
     def plus(x, y):
         return x + y  # pragma: no cover (numba)
 
-    op = BinaryOp.register_anonymous(plus, name="plus")
-    assert op.monoid is None
-    assert op[int].monoid is None
+    if supports_udfs:
+        op = BinaryOp.register_anonymous(plus, name="plus")
+        assert op.monoid is None
+        assert op[int].monoid is None
+        assert op[int].parent is op
 
     assert binary.plus[int].parent is binary.plus
-    assert binary.numpy.add[int].parent is binary.numpy.add
-    assert op[int].parent is op
+    if shouldhave(binary.numpy, "add"):
+        assert binary.numpy.add[int].parent is binary.numpy.add
 
     # bad type
     assert binary.plus[bool].monoid is None
-    assert binary.numpy.equal[int].monoid is None
-    assert binary.numpy.equal[bool].monoid is monoid.numpy.equal[bool]  # sanity
+    if shouldhave(binary.numpy, "equal"):
+        assert binary.numpy.equal[int].monoid is None
+        assert binary.numpy.equal[bool].monoid is monoid.numpy.equal[bool]  # sanity
 
     for attr, val in vars(binary).items():
         if not isinstance(val, BinaryOp):
             continue
         print(attr)
         if hasattr(monoid, attr):
             assert val.monoid is not None
@@ -786,30 +859,33 @@
 @pytest.mark.slow
 def test_monoid_attributes():
     assert monoid.plus[int].binaryop is binary.plus[int]
     assert monoid.plus[int].identity == 0
     assert monoid.plus.binaryop is binary.plus
     assert monoid.plus.identities == {typ: 0 for typ in monoid.plus.types}
 
-    assert monoid.numpy.add[int].binaryop is binary.numpy.add[int]
-    assert monoid.numpy.add[int].identity == 0
-    assert monoid.numpy.add.binaryop is binary.numpy.add
-    assert monoid.numpy.add.identities == {typ: 0 for typ in monoid.numpy.add.types}
+    if shouldhave(monoid.numpy, "add"):
+        assert monoid.numpy.add[int].binaryop is binary.numpy.add[int]
+        assert monoid.numpy.add[int].identity == 0
+        assert monoid.numpy.add.binaryop is binary.numpy.add
+        assert monoid.numpy.add.identities == {typ: 0 for typ in monoid.numpy.add.types}
 
     def plus(x, y):  # pragma: no cover (numba)
         return x + y
 
-    binop = BinaryOp.register_anonymous(plus, name="plus")
-    op = Monoid.register_anonymous(binop, 0, name="plus")
-    assert op.binaryop is binop
-    assert op[int].binaryop is binop[int]
+    if supports_udfs:
+        binop = BinaryOp.register_anonymous(plus, name="plus")
+        op = Monoid.register_anonymous(binop, 0, name="plus")
+        assert op.binaryop is binop
+        assert op[int].binaryop is binop[int]
+        assert op[int].parent is op
 
     assert monoid.plus[int].parent is monoid.plus
-    assert monoid.numpy.add[int].parent is monoid.numpy.add
-    assert op[int].parent is op
+    if shouldhave(monoid.numpy, "add"):
+        assert monoid.numpy.add[int].parent is monoid.numpy.add
 
     for attr, val in vars(monoid).items():
         if not isinstance(val, Monoid):
             continue
         print(attr)
         assert val.binaryop is not None
         assert val.identities is not None
@@ -822,33 +898,35 @@
 @pytest.mark.slow
 def test_semiring_attributes():
     assert semiring.min_plus[int].monoid is monoid.min[int]
     assert semiring.min_plus[int].binaryop is binary.plus[int]
     assert semiring.min_plus.monoid is monoid.min
     assert semiring.min_plus.binaryop is binary.plus
 
-    assert semiring.numpy.add_subtract[int].monoid is monoid.numpy.add[int]
-    assert semiring.numpy.add_subtract[int].binaryop is binary.numpy.subtract[int]
-    assert semiring.numpy.add_subtract.monoid is monoid.numpy.add
-    assert semiring.numpy.add_subtract.binaryop is binary.numpy.subtract
+    if shouldhave(semiring.numpy, "add_subtract"):
+        assert semiring.numpy.add_subtract[int].monoid is monoid.numpy.add[int]
+        assert semiring.numpy.add_subtract[int].binaryop is binary.numpy.subtract[int]
+        assert semiring.numpy.add_subtract.monoid is monoid.numpy.add
+        assert semiring.numpy.add_subtract.binaryop is binary.numpy.subtract
+        assert semiring.numpy.add_subtract[int].parent is semiring.numpy.add_subtract
 
     def plus(x, y):
         return x + y  # pragma: no cover (numba)
 
-    binop = BinaryOp.register_anonymous(plus, name="plus")
-    mymonoid = Monoid.register_anonymous(binop, 0, name="plus")
-    op = Semiring.register_anonymous(mymonoid, binop, name="plus_plus")
-    assert op.binaryop is binop
-    assert op.binaryop[int] is binop[int]
-    assert op.monoid is mymonoid
-    assert op.monoid[int] is mymonoid[int]
+    if supports_udfs:
+        binop = BinaryOp.register_anonymous(plus, name="plus")
+        mymonoid = Monoid.register_anonymous(binop, 0, name="plus")
+        op = Semiring.register_anonymous(mymonoid, binop, name="plus_plus")
+        assert op.binaryop is binop
+        assert op.binaryop[int] is binop[int]
+        assert op.monoid is mymonoid
+        assert op.monoid[int] is mymonoid[int]
+        assert op[int].parent is op
 
     assert semiring.min_plus[int].parent is semiring.min_plus
-    assert semiring.numpy.add_subtract[int].parent is semiring.numpy.add_subtract
-    assert op[int].parent is op
 
     for attr, val in vars(semiring).items():
         if not isinstance(val, Semiring):
             continue
         print(attr)
         assert val.binaryop is not None
         assert val.monoid is not None
@@ -877,17 +955,18 @@
     assert result[0, 0].new() == -1
     assert result.dtype == dtypes.INT64
 
     result = A1.T.mxm(A2, semiring.plus_truediv).new()
     assert result[0, 0].new() == -2
     assert result.dtype == dtypes.FP64
 
-    result = A1.T.mxm(A2, semiring.plus_floordiv).new()
-    assert result[0, 0].new() == -3
-    assert result.dtype == dtypes.INT64
+    if shouldhave(semiring, "plus_floordiv"):
+        result = A1.T.mxm(A2, semiring.plus_floordiv).new()
+        assert result[0, 0].new() == -3
+        assert result.dtype == dtypes.INT64
 
 
 @pytest.mark.slow
 def test_get_semiring():
     sr = get_semiring(monoid.plus, binary.times)
     assert sr is semiring.plus_times
     # Be somewhat forgiving
@@ -898,33 +977,35 @@
     # But not if switched
     with pytest.raises(TypeError, match="switch"):
         get_semiring(binary.plus, monoid.times)
 
     def myplus(x, y):
         return x + y  # pragma: no cover (numba)
 
-    binop = BinaryOp.register_anonymous(myplus, name="myplus")
-    st = get_semiring(monoid.plus, binop)
-    assert st.monoid is monoid.plus
-    assert st.binaryop is binop
-
-    binop = BinaryOp.register_new("myplus", myplus)
-    assert binop is binary.myplus
-    st = get_semiring(monoid.plus, binop)
-    assert st.monoid is monoid.plus
-    assert st.binaryop is binop
+    if supports_udfs:
+        binop = BinaryOp.register_anonymous(myplus, name="myplus")
+        st = get_semiring(monoid.plus, binop)
+        assert st.monoid is monoid.plus
+        assert st.binaryop is binop
+
+        binop = BinaryOp.register_new("myplus", myplus)
+        assert binop is binary.myplus
+        st = get_semiring(monoid.plus, binop)
+        assert st.monoid is monoid.plus
+        assert st.binaryop is binop
 
     with pytest.raises(TypeError, match="Monoid"):
         get_semiring(None, binary.times)
     with pytest.raises(TypeError, match="Binary"):
         get_semiring(monoid.plus, None)
 
-    sr = get_semiring(monoid.plus, binary.numpy.copysign)
-    assert sr.monoid is monoid.plus
-    assert sr.binaryop is binary.numpy.copysign
+    if shouldhave(binary.numpy, "copysign"):
+        sr = get_semiring(monoid.plus, binary.numpy.copysign)
+        assert sr.monoid is monoid.plus
+        assert sr.binaryop is binary.numpy.copysign
 
 
 def test_create_semiring():
     # stress test / sanity check
     monoid_names = {x for x in dir(monoid) if not x.startswith("_")}
     binary_names = {x for x in dir(binary) if not x.startswith("_") and x != "ss"}
     for monoid_name, binary_name in itertools.product(monoid_names, binary_names):
@@ -954,25 +1035,30 @@
     assert not binary.atan2.is_commutative
     assert semiring.plus_times.commutes_to is semiring.plus_times
     assert semiring.plus_times.is_commutative
     assert semiring.any_first.commutes_to is semiring.any_second
     assert semiring.plus_times.is_commutative
     if suitesparse:
         assert semiring.ss.min_secondi.commutes_to is semiring.ss.min_firstj
-    assert semiring.plus_pow.commutes_to is semiring.plus_rpow
+    if shouldhave(semiring, "plus_pow") and shouldhave(semiring, "plus_rpow"):
+        assert semiring.plus_pow.commutes_to is semiring.plus_rpow
     assert not semiring.plus_pow.is_commutative
-    assert binary.isclose.commutes_to is binary.isclose
-    assert binary.isclose.is_commutative
-    assert binary.isclose(0.1).commutes_to is binary.isclose(0.1)
-    assert binary.floordiv.commutes_to is binary.rfloordiv
-    assert not binary.floordiv.is_commutative
-    assert binary.numpy.add.commutes_to is binary.numpy.add
-    assert binary.numpy.add.is_commutative
-    assert binary.numpy.less.commutes_to is binary.numpy.greater
-    assert not binary.numpy.less.is_commutative
+    if shouldhave(binary, "isclose"):
+        assert binary.isclose.commutes_to is binary.isclose
+        assert binary.isclose.is_commutative
+        assert binary.isclose(0.1).commutes_to is binary.isclose(0.1)
+    if shouldhave(binary, "floordiv") and shouldhave(binary, "rfloordiv"):
+        assert binary.floordiv.commutes_to is binary.rfloordiv
+        assert not binary.floordiv.is_commutative
+    if shouldhave(binary.numpy, "add"):
+        assert binary.numpy.add.commutes_to is binary.numpy.add
+        assert binary.numpy.add.is_commutative
+    if shouldhave(binary.numpy, "less") and shouldhave(binary.numpy, "greater"):
+        assert binary.numpy.less.commutes_to is binary.numpy.greater
+        assert not binary.numpy.less.is_commutative
 
     # Typed
     assert binary.plus[int].commutes_to is binary.plus[int]
     assert binary.plus[int].is_commutative
     assert binary.first[int].commutes_to is binary.second[int]
     assert not binary.first[int].is_commutative
     assert monoid.plus[int].commutes_to is monoid.plus[int]
@@ -981,23 +1067,28 @@
     assert not binary.atan2[int].is_commutative
     assert semiring.plus_times[int].commutes_to is semiring.plus_times[int]
     assert semiring.plus_times[int].is_commutative
     assert semiring.any_first[int].commutes_to is semiring.any_second[int]
     assert semiring.plus_times[int].is_commutative
     if suitesparse:
         assert semiring.ss.min_secondi[int].commutes_to is semiring.ss.min_firstj[int]
-    assert semiring.plus_pow[int].commutes_to is semiring.plus_rpow[int]
+    if shouldhave(semiring, "plus_rpow"):
+        assert semiring.plus_pow[int].commutes_to is semiring.plus_rpow[int]
     assert not semiring.plus_pow[int].is_commutative
-    assert binary.isclose(0.1)[int].commutes_to is binary.isclose(0.1)[int]
-    assert binary.floordiv[int].commutes_to is binary.rfloordiv[int]
-    assert not binary.floordiv[int].is_commutative
-    assert binary.numpy.add[int].commutes_to is binary.numpy.add[int]
-    assert binary.numpy.add[int].is_commutative
-    assert binary.numpy.less[int].commutes_to is binary.numpy.greater[int]
-    assert not binary.numpy.less[int].is_commutative
+    if shouldhave(binary, "isclose"):
+        assert binary.isclose(0.1)[int].commutes_to is binary.isclose(0.1)[int]
+    if shouldhave(binary, "floordiv") and shouldhave(binary, "rfloordiv"):
+        assert binary.floordiv[int].commutes_to is binary.rfloordiv[int]
+        assert not binary.floordiv[int].is_commutative
+    if shouldhave(binary.numpy, "add"):
+        assert binary.numpy.add[int].commutes_to is binary.numpy.add[int]
+        assert binary.numpy.add[int].is_commutative
+    if shouldhave(binary.numpy, "less") and shouldhave(binary.numpy, "greater"):
+        assert binary.numpy.less[int].commutes_to is binary.numpy.greater[int]
+        assert not binary.numpy.less[int].is_commutative
 
     # Stress test (this can create extra semirings)
     names = dir(semiring)
     for name in names:
         if name in semiring._deprecated:
             val = semiring._deprecated[name]
         elif name == "ss":
@@ -1010,17 +1101,20 @@
 
 
 def test_from_string():
     assert unary.from_string("-") is unary.ainv
     assert unary.from_string("abs[float]") is unary.abs[float]
     assert binary.from_string("+") is binary.plus
     assert binary.from_string("-[int]") is binary.minus[int]
-    assert binary.from_string("true_divide") is binary.numpy.true_divide
-    assert binary.from_string("//") is binary.floordiv
-    assert binary.from_string("%") is binary.numpy.mod
+    if config["mapnumpy"] or shouldhave(binary.numpy, "true_divide"):
+        assert binary.from_string("true_divide") is binary.numpy.true_divide
+    if shouldhave(binary, "floordiv"):
+        assert binary.from_string("//") is binary.floordiv
+    if shouldhave(binary.numpy, "mod"):
+        assert binary.from_string("%") is binary.numpy.mod
     assert monoid.from_string("*[FP64]") is monoid.times["FP64"]
     assert semiring.from_string("min.plus") is semiring.min_plus
     assert semiring.from_string("min.+") is semiring.min_plus
     assert semiring.from_string("min_plus") is semiring.min_plus
 
     with pytest.raises(ValueError, match="does not end with"):
         assert binary.from_string("plus[int")
@@ -1049,14 +1143,15 @@
     assert agg.from_string("count") is agg.count
     assert agg.from_string("|") is agg.any
     assert agg.from_string("+[int]") is agg.sum[int]
     with pytest.raises(ValueError, match="Unknown agg string"):
         agg.from_string("bad_agg")
 
 
+@pytest.mark.skipif("not supports_udfs")
 @pytest.mark.slow
 def test_lazy_op():
     UnaryOp.register_new("lazy", lambda x: x, lazy=True)  # pragma: no branch (numba)
     assert isinstance(op.lazy, UnaryOp)
     assert isinstance(unary.lazy, UnaryOp)
     BinaryOp.register_new("lazy", lambda x, y: x + y, lazy=True)  # pragma: no branch (numba)
     Monoid.register_new("lazy", "lazy", 0, lazy=True)
@@ -1111,14 +1206,15 @@
         assert unary.ss.positionj[float].is_positional
         assert binary.ss.firsti.is_positional
         assert binary.ss.secondj1[int].is_positional
         assert semiring.ss.any_firsti.is_positional
         assert semiring.ss.any_secondj[int].is_positional
 
 
+@pytest.mark.skipif("not supports_udfs")
 @pytest.mark.slow
 def test_udt():
     record_dtype = np.dtype([("x", np.bool_), ("y", np.float64)], align=True)
     udt = dtypes.register_new("TestUDT", record_dtype)
     assert not udt._is_anonymous
     v = Vector(udt, size=3)
     w = Vector(udt, size=3)
@@ -1276,14 +1372,15 @@
         commutes_to = val.commutes_to
         if commutes_to is not None and commutes_to not in vals:  # pragma: no cover (debug)
             missing.add(commutes_to.name)
     if missing:
         raise AssertionError("Missing binaryops: " + ", ".join(sorted(missing)))
 
 
+@pytest.mark.skipif("not supports_udfs")
 def test_binom():
     v = Vector.from_coo([0, 1, 2], [3, 4, 5])
     result = v.apply(binary.binom, 2).new()
     expected = Vector.from_coo([0, 1, 2], [3, 6, 10])
     assert result.isequal(expected)
     assert op.binom is binary.binom
 
@@ -1337,13 +1434,15 @@
 
 
 def test_is_idempotent():
     assert monoid.min.is_idempotent
     assert monoid.max[int].is_idempotent
     assert monoid.lor.is_idempotent
     assert monoid.band.is_idempotent
-    assert monoid.numpy.gcd.is_idempotent
+    if shouldhave(monoid.numpy, "gcd"):
+        assert monoid.numpy.gcd.is_idempotent
     assert not monoid.plus.is_idempotent
     assert not monoid.times[float].is_idempotent
-    assert not monoid.numpy.equal.is_idempotent
+    if config["mapnumpy"] or shouldhave(monoid.numpy, "equal"):
+        assert not monoid.numpy.equal.is_idempotent
     with pytest.raises(AttributeError):
         binary.min.is_idempotent
```

### Comparing `python-graphblas-2023.3.0/graphblas/tests/test_operator_types.py` & `python-graphblas-2023.5.0/graphblas/tests/test_operator_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import itertools
 from collections import defaultdict
 
 from graphblas import backend, binary, dtypes, monoid, semiring, unary
+from graphblas.core import _supports_udfs as supports_udfs
 from graphblas.core import operator
 from graphblas.dtypes import (
     BOOL,
     FP32,
     FP64,
     INT8,
     INT16,
@@ -79,14 +80,19 @@
     (NOFC, NOFC): {"isge", "isgt", "isle", "islt", "land", "lor", "lxor", "max", "min"},
 }
 # Remove "suitesparse-vailla" once these deprecations are removed
 if backend in {"suitesparse", "suitesparse-vanilla"}:  # pragma: no branch (future)
     BINARY[(ALL, POS)] = {
         "firsti", "firsti1", "firstj", "firstj1", "secondi", "secondi1", "secondj", "secondj1",
     }
+if not supports_udfs:
+    udfs = {"absfirst", "abssecond", "binom", "floordiv", "rfloordiv", "rpow"}
+    for funcnames in BINARY.values():
+        funcnames -= udfs
+    BINARY = {key: val for key, val in BINARY.items() if val}
 
 MONOID = {
     (UINT, UINT): {"band", "bor", "bxnor", "bxor"},
     (BOOL, BOOL): {"eq"},
     (NOFC, BOOL): {"land", "lor", "lxnor", "lxor"},  # others coerced to bool
     (NOFC, NOFC): {"max", "min"},  # max[bool] -> lor, min[bool] -> land
     (NOBOOL, NOBOOL): {"plus"},
```

### Comparing `python-graphblas-2023.3.0/graphblas/tests/test_pickle.py` & `python-graphblas-2023.5.0/graphblas/tests/test_pickle.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pickle
 from pathlib import Path
 
 import numpy as np
 import pytest
 
 import graphblas as gb
+from graphblas.core import _supports_udfs as supports_udfs  # noqa: F401
 
 suitesparse = gb.backend == "suitesparse"
 
 
 def unarypickle(x):
     return x + 1  # pragma: no cover (numba)
 
@@ -32,14 +33,15 @@
 @pytest.fixture
 def extra():
     if gb.backend == "suitesparse-vanilla":
         return "-vanilla"
     return ""
 
 
+@pytest.mark.skipif("not supports_udfs")
 @pytest.mark.slow
 def test_deserialize(extra):
     path = Path(__file__).parent / f"pickle1{extra}.pkl"
     with path.open("rb") as f:
         d = pickle.load(f)
     check_values(d)
     # Again!
@@ -58,14 +60,15 @@
     d3 = pickle.loads(pkl)
     assert d3["unary_pickle"] is gb.unary.unary_pickle
     assert d3["binary_pickle"] is gb.binary.binary_pickle
     assert d3["monoid_pickle"] is gb.monoid.monoid_pickle
     assert d3["semiring_pickle"] is gb.semiring.semiring_pickle
 
 
+@pytest.mark.skipif("not supports_udfs")
 @pytest.mark.slow
 def test_serialize():
     v = gb.Vector.from_coo([1], 2)
 
     # unary_pickle = gb.core.operator.UnaryOp.register_new("unary_pickle", unarypickle)
     # binary_pickle = gb.core.operator.BinaryOp.register_new("binary_pickle", binarypickle)
     # monoid_pickle = gb.core.operator.Monoid.register_new("monoid_pickle", binary_pickle, 0)
@@ -228,14 +231,15 @@
     return inner
 
 
 def identity_par(z):
     return -z
 
 
+@pytest.mark.skipif("not supports_udfs")
 @pytest.mark.slow
 def test_serialize_parameterized():
     # unary_pickle = gb.core.operator.UnaryOp.register_new(
     #     "unary_pickle_par", unarypickle_par, parameterized=True
     # )
     # binary_pickle = gb.core.operator.BinaryOp.register_new(
     #     "binary_pickle_par", binarypickle_par, parameterized=True
@@ -281,24 +285,26 @@
                 pickle.dumps(val)
             except Exception as exc:
                 print(f"Pickle error: {key} {exc!r}")
         raise
     pickle.loads(pkl)  # TODO: check results
 
 
+@pytest.mark.skipif("not supports_udfs")
 @pytest.mark.slow
 def test_deserialize_parameterized(extra):
     path = Path(__file__).parent / f"pickle2{extra}.pkl"
     with path.open("rb") as f:
         pickle.load(f)  # TODO: check results
     # Again!
     with path.open("rb") as f:
         pickle.load(f)  # TODO: check results
 
 
+@pytest.mark.skipif("not supports_udfs")
 def test_udt(extra):
     record_dtype = np.dtype([("x", np.bool_), ("y", np.int64)], align=True)
     udt = gb.dtypes.register_new("PickleUDT", record_dtype)
     assert not udt._is_anonymous
     assert pickle.loads(pickle.dumps(udt)) is udt
 
     np_dtype = np.dtype("(3,)uint16")
```

### Comparing `python-graphblas-2023.3.0/graphblas/tests/test_prefix_scan.py` & `python-graphblas-2023.5.0/graphblas/tests/test_prefix_scan.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/tests/test_recorder.py` & `python-graphblas-2023.5.0/graphblas/tests/test_recorder.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/tests/test_resolving.py` & `python-graphblas-2023.5.0/graphblas/tests/test_resolving.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/tests/test_scalar.py` & `python-graphblas-2023.5.0/graphblas/tests/test_scalar.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import numpy as np
 import pytest
 
 import graphblas as gb
 from graphblas import backend, binary, dtypes, monoid, replace, select, unary
 from graphblas.exceptions import EmptyObject
 
-from .conftest import autocompute, compute
+from .conftest import autocompute, compute, pypy
 
 from graphblas import Matrix, Scalar, Vector  # isort:skip (for dask-graphblas)
 
 suitesparse = backend == "suitesparse"
 
 
 @pytest.fixture
@@ -205,32 +205,32 @@
         s.V
     with pytest.raises(AttributeError):
         s.T
     with pytest.raises(TypeError, match="is not subscriptable"):
         s[0]
     with pytest.raises(TypeError, match="does not support"):
         s[0] = 0
-    with pytest.raises(TypeError, match="doesn't support"):
+    with pytest.raises(TypeError, match="doesn't support|does not support"):
         del s[0]
 
 
 def test_is_empty(s):
-    with pytest.raises(AttributeError, match="can't set attribute"):
+    with pytest.raises(AttributeError, match="can't set attribute|object has no setter"):
         s.is_empty = True
 
 
 def test_update(s):
     s << 1
     assert s == 1
     s << Scalar.from_value(2)
     assert s == 2
     s << Scalar.from_value(3)
     assert s == 3
     if s._is_cscalar:
-        with pytest.raises(TypeError, match="an integer is required"):
+        with pytest.raises(TypeError, match="an integer is required|expected integer"):
             s << Scalar.from_value(4.4)
     else:
         s << Scalar.from_value(4.4)
         assert s == 4
     s() << 5
     assert s == 5
     # with pytest.raises(TypeError, match="is not supported"):
@@ -354,22 +354,23 @@
         "_update",
         "clear",
         "from_value",
         "update",
     }
     if s.is_cscalar:
         expected.add("_empty")
-    assert attrs - expr_attrs == expected, (
+    ignore = {"__sizeof__"}
+    assert attrs - expr_attrs - ignore == expected, (
         "If you see this message, you probably added a method to Scalar.  You may need to "
         "add an entry to `scalar` set in `graphblas.core.automethods` "
         "and then run `python -m graphblas.core.automethods`.  If you're messing with infix "
         "methods, then you may need to run `python -m graphblas.core.infixmethods`."
     )
-    assert attrs - infix_attrs == expected
-    assert attrs - scalar_infix_attrs == expected
+    assert attrs - infix_attrs - ignore == expected
+    assert attrs - scalar_infix_attrs - ignore == expected
     # Make sure signatures actually match. `expr.dup` has `**opts`
     skip = {"__init__", "__repr__", "_repr_html_", "dup"}
     for expr in [v.inner(v), v @ v, t & t]:
         print(type(expr).__name__)
         for attr, val in inspect.getmembers(expr):
             if attr in skip or not isinstance(val, types.MethodType) or not hasattr(s, attr):
                 continue
@@ -395,15 +396,16 @@
         "_name_counter",
         "_update",
         "clear",
         "from_value",
     }
     if s.is_cscalar:
         expected.add("_empty")
-    assert attrs - expr_attrs == expected, (
+    ignore = {"__sizeof__"}
+    assert attrs - expr_attrs - ignore == expected, (
         "If you see this message, you probably added a method to Scalar.  You may need to "
         "add an entry to `scalar` set in `graphblas.core.automethods` "
         "and then run `python -m graphblas.core.automethods`.  If you're messing with infix "
         "methods, then you may need to run `python -m graphblas.core.infixmethods`."
     )
     # Make sure signatures actually match. `update` has different docstring.
     skip = {"__call__", "__init__", "__repr__", "_repr_html_", "update", "dup"}
@@ -501,18 +503,18 @@
     assert expr == 2  # Autocompute and cache value
     assert expr.new().is_cscalar is False  # b/c default reduce is to allow empty
     assert expr == 2  # Autocompute and cache value
     assert expr.new(is_cscalar=True).is_cscalar is True  # We should respect keyword
 
 
 def test_sizeof(s):
-    if suitesparse or s._is_cscalar:
+    if (suitesparse or s._is_cscalar) and not pypy:
         assert 1 < sys.getsizeof(s) < 1000
     else:
-        with pytest.raises(TypeError):
+        with pytest.raises(TypeError):  # flakey coverage (why?!)
             sys.getsizeof(s)
 
 
 def test_ewise_union(s):
     t = Scalar(int)
     result = s.ewise_union(t, binary.plus, 10, 20).new()
     assert result == 25
```

### Comparing `python-graphblas-2023.3.0/graphblas/tests/test_ss_utils.py` & `python-graphblas-2023.5.0/graphblas/tests/test_ss_utils.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/tests/test_vector.py` & `python-graphblas-2023.5.0/graphblas/tests/test_vector.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,25 +7,27 @@
 
 import numpy as np
 import pytest
 from numpy.testing import assert_array_equal
 
 import graphblas as gb
 from graphblas import agg, backend, binary, dtypes, indexunary, monoid, select, semiring, unary
+from graphblas.core import _supports_udfs as supports_udfs
 from graphblas.exceptions import (
     DimensionMismatch,
     DomainMismatch,
     EmptyObject,
     IndexOutOfBound,
     InvalidObject,
     InvalidValue,
     OutputNotEmpty,
+    UdfParseError,
 )
 
-from .conftest import autocompute, compute
+from .conftest import autocompute, compute, pypy
 
 from graphblas import Matrix, Scalar, Vector  # isort:skip (for dask-graphblas)
 
 
 suitesparse = backend == "suitesparse"
 
 
@@ -794,47 +796,73 @@
     w9 << 1
     w9(binary.plus) << v.select(w7.V)
     w8 << 1
     w8(binary.plus) << v.dup(mask=w7.V)
     assert w8.isequal(w9)
 
 
+@pytest.mark.skipif("not supports_udfs")
 @pytest.mark.slow
 def test_indexunary_udf(v):
     def twox_minusthunk(x, row, col, thunk):  # pragma: no cover (numba)
         return 2 * x - thunk
 
-    indexunary.register_new("twox_minusthunk", twox_minusthunk)
+    indexunary.register_new("twox_minusthunk", twox_minusthunk, lazy=True)
     assert hasattr(indexunary, "twox_minusthunk")
     assert not hasattr(select, "twox_minusthunk")
     with pytest.raises(ValueError, match="SelectOp must have BOOL return type"):
         select.register_anonymous(twox_minusthunk)
     with pytest.raises(TypeError, match="must be a function"):
         select.register_anonymous(object())
     expected = Vector.from_coo([1, 3, 4, 6], [-2, -2, 0, -4], size=7)
     result = indexunary.twox_minusthunk(v, 4).new()
     assert result.isequal(expected)
+    assert pickle.loads(pickle.dumps(indexunary.triu)) is indexunary.triu
+    assert indexunary.twox_minusthunk[int]._numba_func(1, 2, 3, 4) == twox_minusthunk(1, 2, 3, 4)
+    assert indexunary.twox_minusthunk[int].orig_func is twox_minusthunk
     delattr(indexunary, "twox_minusthunk")
 
     def ii(x, idx, _, thunk):  # pragma: no cover (numba)
         return idx // 2 >= thunk
 
-    select.register_new("ii", ii)
-    assert hasattr(indexunary, "ii")
+    def iin(n):
+        def inner(x, idx, _, thunk):  # pragma: no cover (numba)
+            return idx // n >= thunk
+
+        return inner
+
+    select.register_new("ii", ii, lazy=True)
+    select.register_new("iin", iin, parameterized=True)
+    assert "ii" in dir(select)
+    assert "ii" in dir(indexunary)
     assert hasattr(select, "ii")
+    assert hasattr(indexunary, "ii")
     ii_apply = indexunary.register_anonymous(ii)
     expected = Vector.from_coo([1, 3, 4, 6], [False, False, True, True], size=7)
     result = ii_apply(v, 2).new()
     assert result.isequal(expected)
+    result = v.apply(indexunary.iin(2), 2).new()
+    assert result.isequal(expected)
+    result = v.apply(indexunary.register_anonymous(iin, parameterized=True)(2), 2).new()
+    assert result.isequal(expected)
+
     ii_select = select.register_anonymous(ii)
     expected = Vector.from_coo([4, 6], [2, 0], size=7)
     result = ii_select(v, 2).new()
     assert result.isequal(expected)
+    result = v.select(select.iin(2), 2).new()
+    assert result.isequal(expected)
+    result = v.select(select.register_anonymous(iin, parameterized=True)(2), 2).new()
+    assert result.isequal(expected)
     delattr(indexunary, "ii")
     delattr(select, "ii")
+    delattr(indexunary, "iin")
+    delattr(select, "iin")
+    with pytest.raises(UdfParseError, match="Unable to parse function using Numba"):
+        indexunary.register_new("bad", lambda x, row, col, thunk: result)
 
 
 def test_reduce(v):
     s = v.reduce(monoid.plus).new()
     assert s == 4
     assert s.dtype == dtypes.INT64
     assert v.reduce(binary.plus).new() == 4
@@ -1620,21 +1648,22 @@
         "from_dict",
         "from_pairs",
         "from_scalar",
         "from_values",
         "resize",
         "update",
     }
-    assert attrs - expr_attrs == expected, (
+    ignore = {"__sizeof__"}
+    assert attrs - expr_attrs - ignore == expected, (
         "If you see this message, you probably added a method to Vector.  You may need to "
         "add an entry to `vector` or `matrix_vector` set in `graphblas.core.automethods` "
         "and then run `python -m graphblas.core.automethods`.  If you're messing with infix "
         "methods, then you may need to run `python -m graphblas.core.infixmethods`."
     )
-    assert attrs - infix_attrs == expected
+    assert attrs - infix_attrs - ignore == expected
     # Make sure signatures actually match
     skip = {"__init__", "__repr__", "_repr_html_"}
     for expr in [binary.times(w & w), w & w]:
         print(type(expr).__name__)
         for attr, val in inspect.getmembers(expr):
             if attr in skip or not isinstance(val, types.MethodType) or not hasattr(w, attr):
                 continue
@@ -1668,15 +1697,16 @@
         "from_dense",
         "from_dict",
         "from_pairs",
         "from_scalar",
         "from_values",
         "resize",
     }
-    assert attrs - expr_attrs == expected, (
+    ignore = {"__sizeof__"}
+    assert attrs - expr_attrs - ignore == expected, (
         "If you see this message, you probably added a method to Vector.  You may need to "
         "add an entry to `vector` or `matrix_vector` set in `graphblas.core.automethods` "
         "and then run `python -m graphblas.core.automethods`.  If you're messing with infix "
         "methods, then you may need to run `python -m graphblas.core.infixmethods`."
     )
     # Make sure signatures actually match. `update` has different docstring.
     skip = {"__call__", "__init__", "__repr__", "_repr_html_", "update"}
@@ -1959,15 +1989,15 @@
     assert v.ndim == 1
     assert v.ewise_mult(v).ndim == 1
     assert (v & v).ndim == 1
     assert (A @ v).ndim == 1
 
 
 def test_sizeof(v):
-    if suitesparse:
+    if suitesparse and not pypy:
         assert sys.getsizeof(v) > v.nvals * 16
     else:
         with pytest.raises(TypeError):
             sys.getsizeof(v)
 
 
 def test_ewise_union():
@@ -2002,14 +2032,15 @@
 def test_delete_via_scalar(v):
     del v[[1, 3]]
     assert v.isequal(Vector.from_coo([4, 6], [2, 0]))
     del v[:]
     assert v.nvals == 0
 
 
+@pytest.mark.skipif("not supports_udfs")
 def test_udt():
     record_dtype = np.dtype([("x", np.bool_), ("y", np.float64)], align=True)
     udt = dtypes.register_anonymous(record_dtype, "VectorUDT")
     assert udt._is_anonymous
     v = Vector(udt, size=3)
     a = np.zeros(1, dtype=record_dtype)
     v[0] = a[0]
@@ -2376,14 +2407,15 @@
     assert idx is None
     assert_array_equal(vals, values)
     assert vals.dtype == float
     idx, vals = v.to_coo(values=True, dtype=v.dtype, sort=False)
     assert vals.dtype == np.int64
 
 
+@pytest.mark.skipif("not supports_udfs")
 def test_lambda_udfs(v):
     result = v.apply(lambda x: x + 1).new()  # pragma: no branch (numba)
     expected = binary.plus(v, 1).new()
     assert result.isequal(expected)
     result = v.ewise_mult(v, lambda x, y: x + y).new()  # pragma: no branch (numba)
     expected = binary.plus(v & v).new()
     assert result.isequal(expected)
@@ -2502,15 +2534,16 @@
     with pytest.raises(TypeError, match="missing"):
         Vector.from_scalar(1)
     with pytest.raises(TypeError, match="Literal scalars also accepted"):
         Vector.from_scalar(v, size=2)
     v = Vector.from_scalar(1, dtype="INT64[2]", size=3)
     w = Vector("INT64[2]", size=3)
     w << [1, 1]
-    assert v.isequal(w, check_dtype=True)
+    if supports_udfs:
+        assert v.isequal(w, check_dtype=True)
 
 
 def test_to_dense_from_dense():
     v = Vector.from_dense([1, 2, 3])
     w = Vector.from_coo([0, 1, 2], [1, 2, 3])
     assert v.isequal(w, check_dtype=True)
     assert_array_equal(v.to_dense(dtype=int), [1, 2, 3])
@@ -2555,24 +2588,26 @@
     w, _ = v.ss.sort(">", permutation=False)
     expected = Vector.from_coo([0, 1, 2, 3], [2, 1, 1, 0], size=7)
     assert w.isequal(expected)
     with pytest.raises(DomainMismatch):
         v.ss.sort(binary.plus)
 
     # Like compactify
-    _, p = v.ss.sort(lambda x, y: False, values=False)  # pragma: no branch (numba)
-    expected_p = Vector.from_coo([0, 1, 2, 3], [1, 3, 4, 6], size=7)
-    assert p.isequal(expected_p)
+    if supports_udfs:
+        _, p = v.ss.sort(lambda x, y: False, values=False)  # pragma: no branch (numba)
+        expected_p = Vector.from_coo([0, 1, 2, 3], [1, 3, 4, 6], size=7)
+        assert p.isequal(expected_p)
     # reversed
     _, p = v.ss.sort(binary.pair[bool], values=False)
     expected_p = Vector.from_coo([0, 1, 2, 3], [6, 4, 3, 1], size=7)
     assert p.isequal(expected_p)
     w, p = v.ss.sort(monoid.lxor)  # Weird, but user-defined monoids may not commute, so okay
 
 
+@pytest.mark.skipif("not supports_udfs")
 def test_subarray_dtypes():
     a = np.arange(3 * 4, dtype=np.int64).reshape(3, 4)
     v = Vector.from_coo([1, 3, 5], a)
     w = Vector("INT64[4]", size=6)
     w[1] = [0, 1, 2, 3]
     w[3] = [4, 5, 6, 7]
     w[5] = [8, 9, 10, 11]
```

### Comparing `python-graphblas-2023.3.0/graphblas/unary/__init__.py` & `python-graphblas-2023.5.0/graphblas/unary/__init__.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/graphblas/unary/numpy.py` & `python-graphblas-2023.5.0/graphblas/unary/numpy.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 """
 import numpy as _np
 
 from .. import _STANDARD_OPERATOR_NAMES
 from .. import config as _config
 from .. import unary as _unary
+from ..core import _supports_udfs
 from ..dtypes import _supports_complex
 
 _delayed = {}
 _unary_names = {
     # Math operations
     "negative",
     "abs",
@@ -115,27 +116,37 @@
 # _graphblas_to_numpy = {val: key for key, val in _numpy_to_graphblas.items()}  # Soon...
 
 _STANDARD_OPERATOR_NAMES.update(f"unary.numpy.{name}" for name in _unary_names)
 __all__ = list(_unary_names)
 
 
 def __dir__():
-    return globals().keys() | _delayed.keys() | _unary_names
+    if not _supports_udfs and not _config.get("mapnumpy"):
+        return globals().keys()  # FLAKY COVERAGE
+    attrs = _delayed.keys() | _unary_names
+    if not _supports_udfs:
+        attrs &= _numpy_to_graphblas.keys()
+    return attrs | globals().keys()
 
 
 def __getattr__(name):
     if name in _delayed:
         delayed_func, kwargs = _delayed.pop(name)
         rv = delayed_func(**kwargs)
         globals()[name] = rv
         return rv
     if name not in _unary_names:
         raise AttributeError(f"module {__name__!r} has no attribute {name!r}")
     if _config.get("mapnumpy") and name in _numpy_to_graphblas:
         globals()[name] = getattr(_unary, _numpy_to_graphblas[name])
+    elif not _supports_udfs:
+        raise AttributeError(
+            f"module {__name__!r} unable to compile UDF for {name!r}; "
+            "install numba for UDF support"
+        )
     else:
         numpy_func = getattr(_np, name)
 
         def func(x):  # pragma: no cover (numba)
             return numpy_func(x)
 
         _unary.register_new(f"numpy.{name}", func)
```

### Comparing `python-graphblas-2023.3.0/graphblas/viz.py` & `python-graphblas-2023.5.0/graphblas/viz.py`

 * *Files identical despite different names*

### Comparing `python-graphblas-2023.3.0/pyproject.toml` & `python-graphblas-2023.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -43,69 +43,91 @@
     "Operating System :: POSIX :: Linux",
     "Operating System :: Microsoft :: Windows",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Intended Audience :: Developers",
     "Intended Audience :: Other Audience",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
-    "suitesparse-graphblas >=7.4.0.0, <7.5",
     "numpy >=1.21",
-    "numba >=0.55",
     "donfig >=0.6",
     "pyyaml >=5.4",
+    # These won't be installed by default after 2024.3.0
+    # Use e.g. "python-graphblas[suitesparse]" or "python-graphblas[default]" instead
+    "suitesparse-graphblas >=7.4.0.0, <7.5",
+    "numba >=0.55; python_version<'3.12'",  # make optional where numba is not supported
 ]
 
 [project.urls]
 homepage = "https://github.com/python-graphblas/python-graphblas"
 documentation = "https://python-graphblas.readthedocs.io"
 repository = "https://github.com/python-graphblas/python-graphblas"
 changelog = "https://github.com/python-graphblas/python-graphblas/releases"
 
 [project.optional-dependencies]
-repr = [
-    "pandas >=1.2",
+suitesparse = [
+    "suitesparse-graphblas >=7.4.0.0, <7.5",
 ]
-io = [
+networkx = [
     "networkx >=2.8",
-    "scipy >=1.8",
-    "awkward >=1.9",
-    "sparse >=0.12",
-    "fast-matrix-market >=1.4.5",
 ]
-viz = [
-    "matplotlib >=3.5",
+numba = [
+    "numba >=0.55",
 ]
-test = [
-    "pytest",
-    "packaging",
+pandas = [
     "pandas >=1.2",
-    "scipy >=1.8",
-    "tomli",
 ]
-complete = [
-    "pandas >=1.2",
-    "networkx >=2.8",
+scipy = [
     "scipy >=1.8",
+]
+suitesparse-udf = [  # udf requires numba
+    "python-graphblas[suitesparse,numba]",
+]
+repr = [
+    "python-graphblas[pandas]",
+]
+io = [
+    "python-graphblas[networkx,scipy]",
+    "python-graphblas[numba]; python_version<'3.12'",
     "awkward >=1.9",
-    "sparse >=0.12",
+    "sparse >=0.13; python_version<'3.12'",  # make optional, b/c sparse needs numba
     "fast-matrix-market >=1.4.5",
+]
+viz = [
+    "python-graphblas[networkx,scipy]",
     "matplotlib >=3.5",
-    "pytest",
-    "packaging",
-    "tomli",
+]
+datashade = [  # datashade requires numba
+    "python-graphblas[numba,pandas,scipy]",
+    "datashader >=0.12",
+    "hvplot >=0.7",
+]
+test = [
+    "python-graphblas[suitesparse,pandas,scipy]",
+    "packaging >=21",
+    "pytest >=6.2",
+    "tomli >=1",
+]
+default = [
+    "python-graphblas[suitesparse,pandas,scipy]",
+    "python-graphblas[numba]; python_version<'3.12'",  # make optional where numba is not supported
+]
+all = [
+    "python-graphblas[default,io,viz,test]",
+    "python-graphblas[datashade]; python_version<'3.12'",  # make optional, b/c datashade needs numba
 ]
 
 [tool.setuptools]
 # Let's be explicit
 # $ python -c 'from setuptools import find_packages ; [print(x) for x in sorted(find_packages())]'
 # $ find graphblas/ -name __init__.py -print | sort | sed -e 's/\/__init__.py//g' -e 's/\//./g'
 # $ python -c 'import tomli ; [print(x) for x in sorted(tomli.load(open("pyproject.toml", "rb"))["tool"]["setuptools"]["packages"])]'
@@ -113,14 +135,15 @@
     "graphblas",
     "graphblas.agg",
     "graphblas.binary",
     "graphblas.core",
     "graphblas.core.operator",
     "graphblas.core.ss",
     "graphblas.indexunary",
+    "graphblas.io",
     "graphblas.monoid",
     "graphblas.op",
     "graphblas.semiring",
     "graphblas.select",
     "graphblas.ss",
     "graphblas.tests",
     "graphblas.unary",
@@ -150,26 +173,31 @@
 markers = [
     "slow: Skipped unless --runslow passed",
 ]
 filterwarnings = [
     # See: https://docs.python.org/3/library/warnings.html#describing-warning-filters
     # and: https://docs.pytest.org/en/7.2.x/how-to/capture-warnings.html#controlling-warnings
     "error",
-    # MAINT: we can drop support for sparse <0.13 at any time
-    "ignore:`np.bool` is a deprecated alias:DeprecationWarning:sparse._umath",  # sparse <0.13
     # sparse 0.14.0 (2022-02-24) began raising this warning; it has been reported and fixed upstream.
     "ignore:coords should be an ndarray. This will raise a ValueError:DeprecationWarning:sparse._coo.core",
 
     # setuptools v67.3.0 deprecated `pkg_resources.declare_namespace` on 13 Feb 2023. See:
     # https://setuptools.pypa.io/en/latest/history.html#v67-3-0
     # MAINT: check if this is still necessary in 2025
     "ignore:Deprecated call to `pkg_resources.declare_namespace:DeprecationWarning:pkg_resources",
     # And this deprecation warning was added in setuptools v67.5.0 (8 Mar 2023). See:
     # https://setuptools.pypa.io/en/latest/history.html#v67-5-0
     "ignore:pkg_resources is deprecated as an API:DeprecationWarning:pkg_resources",
+
+    # sre_parse deprecated in 3.11; this is triggered by awkward 0.10
+    "ignore:module 'sre_parse' is deprecated:DeprecationWarning:",
+    "ignore:module 'sre_constants' is deprecated:DeprecationWarning:",
+
+    # pypy gives this warning
+    "ignore:can't resolve package from __spec__ or __package__:ImportWarning:",
 ]
 
 [tool.coverage.run]
 branch = true
 source = ["graphblas"]
 omit = [
     "graphblas/viz.py",  # TODO: test and get coverage for viz.py
@@ -289,14 +317,16 @@
     "PLW0603",  # Using the global statement to update ... is discouraged (Note: yeah, discouraged, but too strict)
     "PLW2901",  # Outer for loop variable ... overwritten by inner assignment target (Note: good advice, but too strict)
     "RET502",  # Do not implicitly `return None` in function able to return non-`None` value
     "RET503",  # Missing explicit `return` at the end of function able to return non-`None` value
     "RET504",  # Unnecessary variable assignment before `return` statement
     "S110",  # `try`-`except`-`pass` detected, consider logging the exception (Note: good advice, but we don't log)
     "S112",  # `try`-`except`-`continue` detected, consider logging the exception (Note: good advice, but we don't log)
+    "S603",  # `subprocess` call: check for execution of untrusted input (Note: not important for us)
+    "S607",  # Starting a process with a partial executable path (Note: not important for us)
     "SIM102",  # Use a single `if` statement instead of nested `if` statements (Note: often necessary)
     "SIM105",  # Use contextlib.suppress(...) instead of try-except-pass (Note: try-except-pass is much faster)
     "SIM108",  # Use ternary operator ... instead of if-else-block (Note: if-else better for coverage and sometimes clearer)
     "TRY003",  # Avoid specifying long messages outside the exception class (Note: why?)
 
     # Ignored categories
     "C90",  # mccabe (Too strict, but maybe we should make things less complex)
@@ -317,23 +347,25 @@
 ]
 
 [tool.ruff.per-file-ignores]
 "graphblas/core/agg.py" = ["F401", "F403"]  # Deprecated
 "graphblas/core/operator/base.py" = ["S102"]  # exec is used for UDF
 "graphblas/core/ss/matrix.py" = ["NPY002"]  # numba doesn't support rng generator yet
 "graphblas/core/ss/vector.py" = ["NPY002"]  # numba doesn't support rng generator yet
+"graphblas/core/utils.py" = ["PLE0302"]  # `__set__` is used as a property
 "graphblas/ss/_core.py" = ["N999"]  # We want _core.py to be underscopre
 # Allow useless expressions, assert, pickle, RNG, print, no docstring, and yoda in tests
 "graphblas/tests/*py" = ["B018", "S101", "S301", "S311", "T201", "D103", "D100", "SIM300"]
 "graphblas/tests/test_formatting.py" = ["E501"]  # Allow long lines
 "graphblas/**/__init__.py" = ["F401"]  # Allow unused imports (w/o defining `__all__`)
 "scripts/*.py" = ["INP001"]  # Not a package
 "scripts/create_pickle.py" = ["F403", "F405"]  # Allow `from foo import *`
 "docs/*.py" = ["INP001"]  # Not a package
 
+
 [tool.ruff.flake8-builtins]
 builtins-ignorelist = ["copyright", "format", "min", "max"]
 
 [tool.ruff.flake8-pytest-style]
 fixture-parentheses = false
 mark-parentheses = false
```

### Comparing `python-graphblas-2023.3.0/python_graphblas.egg-info/PKG-INFO` & `python-graphblas-2023.5.0/python_graphblas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-graphblas
-Version: 2023.3.0
+Version: 2023.5.0
 Summary: Python library for GraphBLAS: high-performance sparse linear algebra for scalable graph analytics
 Author: Jim Kitchen, Python-graphblas contributors
 Author-email: Erik Welch <erik.n.welch@gmail.com>
 Maintainer-email: Erik Welch <erik.n.welch@gmail.com>, Jim Kitchen <jim22k@gmail.com>, Sultan Orazbayev <contact@econpoint.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -218,80 +218,100 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: suitesparse
+Provides-Extra: networkx
+Provides-Extra: numba
+Provides-Extra: pandas
+Provides-Extra: scipy
+Provides-Extra: suitesparse-udf
 Provides-Extra: repr
 Provides-Extra: io
 Provides-Extra: viz
+Provides-Extra: datashade
 Provides-Extra: test
-Provides-Extra: complete
+Provides-Extra: default
+Provides-Extra: all
 License-File: LICENSE
 
-# Python-graphblas
+![Python-graphblas](docs/_static/img/logo-name-medium.svg)
 
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/python-graphblas.svg)](https://anaconda.org/conda-forge/python-graphblas)
 [![pypi](https://img.shields.io/pypi/v/python-graphblas.svg)](https://pypi.python.org/pypi/python-graphblas/)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/python-graphblas)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/python-graphblas)](https://pypi.python.org/pypi/python-graphblas/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/python-graphblas/python-graphblas/blob/main/LICENSE)
+<br>
 [![Tests](https://github.com/python-graphblas/python-graphblas/workflows/Tests/badge.svg?branch=main)](https://github.com/python-graphblas/python-graphblas/actions)
 [![Docs](https://readthedocs.org/projects/python-graphblas/badge/?version=latest)](https://python-graphblas.readthedocs.io/en/latest/)
 [![Coverage](https://coveralls.io/repos/python-graphblas/python-graphblas/badge.svg?branch=main)](https://coveralls.io/r/python-graphblas/python-graphblas)
+<br>
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7328791.svg)](https://doi.org/10.5281/zenodo.7328791)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/python-graphblas/python-graphblas/HEAD?filepath=notebooks%2FIntro%20to%20GraphBLAS%20%2B%20SSSP%20example.ipynb)
 [![Discord](https://img.shields.io/badge/Chat-Discord-blue)](https://discord.com/invite/vur45CbwMz)
 
 Python library for GraphBLAS: high-performance sparse linear algebra for scalable graph analytics.
+For algorithms, see
+[`graphblas-algorithms`](https://github.com/python-graphblas/graphblas-algorithms).
 
 - **Documentation:** [https://python-graphblas.readthedocs.io/](https://python-graphblas.readthedocs.io/)
+  - **FAQ:** [https://python-graphblas.readthedocs.io/en/stable/getting_started/faq.html](https://python-graphblas.readthedocs.io/en/stable/getting_started/faq.html)
   - **GraphBLAS C API:** [https://graphblas.org/docs/GraphBLAS_API_C_v2.0.0.pdf](https://graphblas.org/docs/GraphBLAS_API_C_v2.0.0.pdf)
   - **SuiteSparse:GraphBLAS User Guide:** [https://github.com/DrTimothyAldenDavis/GraphBLAS/raw/stable/Doc/GraphBLAS_UserGuide.pdf](https://github.com/DrTimothyAldenDavis/GraphBLAS/raw/stable/Doc/GraphBLAS_UserGuide.pdf)
 - **Source:** [https://github.com/python-graphblas/python-graphblas](https://github.com/python-graphblas/python-graphblas)
 - **Bug reports:** [https://github.com/python-graphblas/python-graphblas/issues](https://github.com/python-graphblas/python-graphblas/issues)
 - **Github discussions:** [https://github.com/python-graphblas/python-graphblas/discussions](https://github.com/python-graphblas/python-graphblas/discussions)
 - **Weekly community call:** [https://github.com/python-graphblas/python-graphblas/issues/247](https://github.com/python-graphblas/python-graphblas/issues/247)
 - **Chat via Discord:** [https://discord.com/invite/vur45CbwMz](https://discord.com/invite/vur45CbwMz) in the [#graphblas channel](https://discord.com/channels/786703927705862175/1024732940233605190)
 
+<p float="left">
+  <img src="docs/_static/img/draw-example.png" width="231" align="top" alt="Directed graph", title="Directed graph"/>
+  <img src="docs/_static/img/repr-matrix.png" width="231" align="top" alt="Adjacency matrix" title="Adjacency matrix"/>
+</p>
+
 ## Install
 Install the latest version of Python-graphblas via conda:
 ```
 $ conda install -c conda-forge python-graphblas
 ```
 or pip:
 ```
-$ pip install python-graphblas
+$ pip install python-graphblas[default]
 ```
 This will also install the [SuiteSparse:GraphBLAS](https://github.com/DrTimothyAldenDavis/GraphBLAS) compiled C library.
+We currently support the [GraphBLAS C API 2.0 specification](https://graphblas.org/docs/GraphBLAS_API_C_v2.0.0.pdf).
 
 ### Optional Dependencies
 
 The following are not required by python-graphblas, but may be needed for certain functionality to work.
 
 - `pandas` – required for nicer `__repr__`;
 - `matplotlib` – required for basic plotting of graphs;
-- `scipy` – used in io module to read/write `scipy.sparse` format;
+- `scipy` – used in `io` module to read/write `scipy.sparse` format;
 - `networkx` – used in `io` module to interface with `networkx` graphs;
 - `fast-matrix-market` - for faster read/write of Matrix Market files with `gb.io.mmread` and `gb.io.mmwrite`.
 
 ## Description
 Currently works with [SuiteSparse:GraphBLAS](https://github.com/DrTimothyAldenDavis/GraphBLAS), but the goal is to make it work with all implementations of the GraphBLAS spec.
 
-The approach taken with this library is to follow the C-API specification as closely as possible while making improvements
+The approach taken with this library is to follow the C-API 2.0 specification as closely as possible while making improvements
 allowed with the Python syntax. Because the spec always passes in the output object to be written to, we follow the same,
 which is very different from the way Python normally operates. In fact, many who are familiar with other Python data
 libraries (numpy, pandas, etc) will find it strange to not create new objects for every call.
 
 At the highest level, the goal is to separate output, mask, and accumulator on the left side of the assignment
 operator `=` and put the computation on the right side. Unfortunately, that approach doesn't always work very well
 with how Python handles assignment, so instead we (ab)use the left-shift `<<` notation to give the same flavor of
```

### Comparing `python-graphblas-2023.3.0/python_graphblas.egg-info/SOURCES.txt` & `python-graphblas-2023.5.0/python_graphblas.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
+docs/_static/img/draw-example.png
+docs/_static/img/logo-name-medium.svg
+docs/_static/img/repr-matrix.png
 graphblas/__init__.py
 graphblas/dtypes.py
 graphblas/exceptions.py
 graphblas/graphblas.yaml
-graphblas/io.py
 graphblas/viz.py
 graphblas/agg/__init__.py
 graphblas/agg/ss.py
 graphblas/binary/__init__.py
 graphblas/binary/numpy.py
 graphblas/binary/ss.py
 graphblas/core/__init__.py
@@ -43,14 +45,22 @@
 graphblas/core/ss/__init__.py
 graphblas/core/ss/config.py
 graphblas/core/ss/descriptor.py
 graphblas/core/ss/matrix.py
 graphblas/core/ss/prefix_scan.py
 graphblas/core/ss/vector.py
 graphblas/indexunary/__init__.py
+graphblas/io/__init__.py
+graphblas/io/_awkward.py
+graphblas/io/_matrixmarket.py
+graphblas/io/_networkx.py
+graphblas/io/_numpy.py
+graphblas/io/_scipy.py
+graphblas/io/_sparse.py
+graphblas/io/_viz.py
 graphblas/monoid/__init__.py
 graphblas/monoid/numpy.py
 graphblas/op/__init__.py
 graphblas/op/numpy.py
 graphblas/op/ss.py
 graphblas/select/__init__.py
 graphblas/semiring/__init__.py
```

