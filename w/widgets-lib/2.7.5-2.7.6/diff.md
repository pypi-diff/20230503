# Comparing `tmp/widgets-lib-2.7.5.tar.gz` & `tmp/widgets-lib-2.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widgets-lib-2.7.5.tar", last modified: Wed May  3 17:55:52 2023, max compression
+gzip compressed data, was "widgets-lib-2.7.6.tar", last modified: Wed May  3 19:09:16 2023, max compression
```

## Comparing `widgets-lib-2.7.5.tar` & `widgets-lib-2.7.6.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:55:52.735257 widgets-lib-2.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-03 17:55:52.735257 widgets-lib-2.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 17:55:52.735257 widgets-lib-2.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:55:52.719256 widgets-lib-2.7.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:55:52.719256 widgets-lib-2.7.5/src/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:55:52.723256 widgets-lib-2.7.5/src/widgets/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/base/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/base/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    21852 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/base/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/base/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:55:52.723256 widgets-lib-2.7.5/src/widgets/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:55:52.723256 widgets-lib-2.7.5/src/widgets/st_base/
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/st_base/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/st_base/value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:55:52.723256 widgets-lib-2.7.5/src/widgets/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/streamlit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:55:52.723256 widgets-lib-2.7.5/src/widgets/streamlit/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/streamlit/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/streamlit/resource/columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/streamlit/resource/duplicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/streamlit/resource/expander.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:55:52.727256 widgets-lib-2.7.5/src/widgets/streamlit/resource/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/streamlit/resource/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/streamlit/resource/files/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/streamlit/resource/files/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/streamlit/resource/files/download_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/streamlit/resource/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/streamlit/resource/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:55:52.727256 widgets-lib-2.7.5/src/widgets/streamlit/resource/values/
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/streamlit/resource/values/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/streamlit/resource/values/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/streamlit/resource/values/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/streamlit/resource/values/multiselect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/streamlit/resource/values/selectstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/streamlit/resource/values/slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/streamlit/resource/values/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/streamlit/resource/values/textarea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:55:52.727256 widgets-lib-2.7.5/src/widgets/streamlit/widget/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/streamlit/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/streamlit/widget/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:55:52.731256 widgets-lib-2.7.5/src/widgets/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/templates/source.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/templates/streamlit_single.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/templates/streamlit_single.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/src/widgets/templates/streamlit_single_ga.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:55:52.731256 widgets-lib-2.7.5/src/widgets_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-03 17:55:52.000000 widgets-lib-2.7.5/src/widgets_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-03 17:55:52.000000 widgets-lib-2.7.5/src/widgets_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 17:55:52.000000 widgets-lib-2.7.5/src/widgets_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-03 17:55:52.000000 widgets-lib-2.7.5/src/widgets_lib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 17:55:52.000000 widgets-lib-2.7.5/src/widgets_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 17:55:52.000000 widgets-lib-2.7.5/src/widgets_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:55:52.735257 widgets-lib-2.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/tests/test_duplicator.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/tests/test_source_parents.py
--rw-r--r--   0 runner    (1001) docker     (123)    10120 2023-05-03 17:55:06.000000 widgets-lib-2.7.5/tests/test_streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:09:16.809231 widgets-lib-2.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-03 19:09:16.809231 widgets-lib-2.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 19:09:16.809231 widgets-lib-2.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:09:16.801231 widgets-lib-2.7.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:09:16.805231 widgets-lib-2.7.6/src/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:09:16.805231 widgets-lib-2.7.6/src/widgets/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/base/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/base/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21852 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/base/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/base/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:09:16.805231 widgets-lib-2.7.6/src/widgets/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:09:16.805231 widgets-lib-2.7.6/src/widgets/st_base/
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/st_base/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/st_base/value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:09:16.805231 widgets-lib-2.7.6/src/widgets/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/streamlit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:09:16.805231 widgets-lib-2.7.6/src/widgets/streamlit/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/streamlit/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/streamlit/resource/columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/streamlit/resource/duplicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/streamlit/resource/expander.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:09:16.805231 widgets-lib-2.7.6/src/widgets/streamlit/resource/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/streamlit/resource/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/streamlit/resource/files/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/streamlit/resource/files/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/streamlit/resource/files/download_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/streamlit/resource/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/streamlit/resource/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:09:16.805231 widgets-lib-2.7.6/src/widgets/streamlit/resource/values/
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/streamlit/resource/values/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/streamlit/resource/values/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/streamlit/resource/values/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/streamlit/resource/values/multiselect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/streamlit/resource/values/selectstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/streamlit/resource/values/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/streamlit/resource/values/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/streamlit/resource/values/textarea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:09:16.805231 widgets-lib-2.7.6/src/widgets/streamlit/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/streamlit/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/streamlit/widget/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:09:16.809231 widgets-lib-2.7.6/src/widgets/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/templates/source.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/templates/streamlit_single.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/templates/streamlit_single.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/src/widgets/templates/streamlit_single_ga.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:09:16.809231 widgets-lib-2.7.6/src/widgets_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-03 19:09:16.000000 widgets-lib-2.7.6/src/widgets_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-03 19:09:16.000000 widgets-lib-2.7.6/src/widgets_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:09:16.000000 widgets-lib-2.7.6/src/widgets_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-03 19:09:16.000000 widgets-lib-2.7.6/src/widgets_lib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 19:09:16.000000 widgets-lib-2.7.6/src/widgets_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 19:09:16.000000 widgets-lib-2.7.6/src/widgets_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:09:16.809231 widgets-lib-2.7.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/tests/test_duplicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/tests/test_source_parents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10120 2023-05-03 19:08:39.000000 widgets-lib-2.7.6/tests/test_streamlit.py
```

### Comparing `widgets-lib-2.7.5/LICENSE` & `widgets-lib-2.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/PKG-INFO` & `widgets-lib-2.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widgets-lib
-Version: 2.7.5
+Version: 2.7.6
 Summary: Merging code and data in webpages
 Author-email: Samuel Minot <sminot@fredhutch.org>
 Project-URL: Homepage, https://github.com/FredHutch/widgets
 Project-URL: Bug Tracker, https://github.com/FredHutch/widgets/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `widgets-lib-2.7.5/README.md` & `widgets-lib-2.7.6/README.md`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/pyproject.toml` & `widgets-lib-2.7.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/base/exceptions.py` & `widgets-lib-2.7.6/src/widgets/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/base/helpers.py` & `widgets-lib-2.7.6/src/widgets/base/helpers.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/base/io.py` & `widgets-lib-2.7.6/src/widgets/base/io.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/base/resource.py` & `widgets-lib-2.7.6/src/widgets/base/resource.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/base/widget.py` & `widgets-lib-2.7.6/src/widgets/base/widget.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/cli/main.py` & `widgets-lib-2.7.6/src/widgets/cli/main.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/st_base/resource.py` & `widgets-lib-2.7.6/src/widgets/st_base/resource.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/st_base/value.py` & `widgets-lib-2.7.6/src/widgets/st_base/value.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/streamlit/__init__.py` & `widgets-lib-2.7.6/src/widgets/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/streamlit/resource/columns.py` & `widgets-lib-2.7.6/src/widgets/streamlit/resource/columns.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     def __init__(
         self,
         id="columns",
         children: List[Resource] = [],
         spec=None,
         sidebar=True,
         gap="small",
-        disable_sidebar=False,
         **kwargs
     ) -> None:
         """
         Set up the StColumns object
         """
 
         # If no spec has been provided, or if an integer was provided
@@ -53,15 +52,16 @@
                 msg = "StColumns: spec length must match children"
                 raise ResourceConfigurationException(msg)
 
         if gap not in ["small", "medium", "large"]:
             msg = "StColumns: gap must be one of small, medium, large"
             raise ResourceConfigurationException(msg)
 
-        # Disable the sidebar for all child elements IF the sidebar flag is set to False
+        # Disable the sidebar for all child elements
+        # IF the sidebar flag is set to False
         kwargs["disable_sidebar"] = not sidebar
 
         # Set up the core attributes of the StResource
         super().__init__(
             id=id,
             children=children,
             label="",
```

### Comparing `widgets-lib-2.7.5/src/widgets/streamlit/resource/duplicator.py` & `widgets-lib-2.7.6/src/widgets/streamlit/resource/duplicator.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/streamlit/resource/expander.py` & `widgets-lib-2.7.6/src/widgets/streamlit/resource/expander.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,36 +13,32 @@
         self,
         id="expander",
         children: List[Resource] = [],
         label=None,
         help=None,
         expanded=False,
         sidebar=True,
-        disable_sidebar=False,
         **kwargs
     ) -> None:
         """
         Set up the StExpander object
         """
 
-        # If the sidebar flag is set to False
-        if not sidebar:
-
-            # Disable the sidebar for all child elements
-            kwargs["disable_sidebar"] = True
+        # Disable the sidebar for all child elements
+        # IF the sidebar flag is set to False
+        kwargs["disable_sidebar"] = not sidebar
 
         # Set up the core attributes of the StResource
         super().__init__(
             id=id,
             children=children,
             label=label,
             help=help,
             expanded=expanded,
             sidebar=sidebar,
-            disable_sidebar=disable_sidebar,
             **kwargs
         )
 
     def prep(self) -> None:
         """
         Instantiate a expand/collapse container
         """
```

### Comparing `widgets-lib-2.7.5/src/widgets/streamlit/resource/files/base.py` & `widgets-lib-2.7.6/src/widgets/streamlit/resource/files/base.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/streamlit/resource/files/dataframe.py` & `widgets-lib-2.7.6/src/widgets/streamlit/resource/files/dataframe.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/streamlit/resource/files/download_dataframe.py` & `widgets-lib-2.7.6/src/widgets/streamlit/resource/files/download_dataframe.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/streamlit/resource/markdown.py` & `widgets-lib-2.7.6/src/widgets/streamlit/resource/markdown.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/streamlit/resource/selector.py` & `widgets-lib-2.7.6/src/widgets/streamlit/resource/selector.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/streamlit/resource/values/checkbox.py` & `widgets-lib-2.7.6/src/widgets/streamlit/resource/values/checkbox.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/streamlit/resource/values/float.py` & `widgets-lib-2.7.6/src/widgets/streamlit/resource/values/float.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/streamlit/resource/values/integer.py` & `widgets-lib-2.7.6/src/widgets/streamlit/resource/values/integer.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/streamlit/resource/values/multiselect.py` & `widgets-lib-2.7.6/src/widgets/streamlit/resource/values/multiselect.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/streamlit/resource/values/selectstring.py` & `widgets-lib-2.7.6/src/widgets/streamlit/resource/values/selectstring.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/streamlit/resource/values/slider.py` & `widgets-lib-2.7.6/src/widgets/streamlit/resource/values/slider.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/streamlit/resource/values/string.py` & `widgets-lib-2.7.6/src/widgets/streamlit/resource/values/string.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/streamlit/resource/values/textarea.py` & `widgets-lib-2.7.6/src/widgets/streamlit/resource/values/textarea.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/streamlit/widget/base.py` & `widgets-lib-2.7.6/src/widgets/streamlit/widget/base.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/templates/streamlit_single.html.j2` & `widgets-lib-2.7.6/src/widgets/templates/streamlit_single.html.j2`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets/templates/streamlit_single_ga.html.j2` & `widgets-lib-2.7.6/src/widgets/templates/streamlit_single_ga.html.j2`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/src/widgets_lib.egg-info/PKG-INFO` & `widgets-lib-2.7.6/src/widgets_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widgets-lib
-Version: 2.7.5
+Version: 2.7.6
 Summary: Merging code and data in webpages
 Author-email: Samuel Minot <sminot@fredhutch.org>
 Project-URL: Homepage, https://github.com/FredHutch/widgets
 Project-URL: Bug Tracker, https://github.com/FredHutch/widgets/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `widgets-lib-2.7.5/src/widgets_lib.egg-info/SOURCES.txt` & `widgets-lib-2.7.6/src/widgets_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/tests/test_base.py` & `widgets-lib-2.7.6/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/tests/test_cli.py` & `widgets-lib-2.7.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/tests/test_duplicator.py` & `widgets-lib-2.7.6/tests/test_duplicator.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/tests/test_helpers.py` & `widgets-lib-2.7.6/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/tests/test_io.py` & `widgets-lib-2.7.6/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/tests/test_source_parents.py` & `widgets-lib-2.7.6/tests/test_source_parents.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.5/tests/test_streamlit.py` & `widgets-lib-2.7.6/tests/test_streamlit.py`

 * *Files identical despite different names*

