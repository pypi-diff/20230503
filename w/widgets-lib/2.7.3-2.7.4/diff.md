# Comparing `tmp/widgets-lib-2.7.3.tar.gz` & `tmp/widgets-lib-2.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widgets-lib-2.7.3.tar", last modified: Mon May  1 20:55:01 2023, max compression
+gzip compressed data, was "widgets-lib-2.7.4.tar", last modified: Wed May  3 17:29:09 2023, max compression
```

## Comparing `widgets-lib-2.7.3.tar` & `widgets-lib-2.7.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.880685 widgets-lib-2.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-01 20:55:01.880685 widgets-lib-2.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 20:55:01.880685 widgets-lib-2.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.864685 widgets-lib-2.7.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.868686 widgets-lib-2.7.3/src/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.868686 widgets-lib-2.7.3/src/widgets/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/base/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/base/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    21852 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/base/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/base/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.868686 widgets-lib-2.7.3/src/widgets/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.868686 widgets-lib-2.7.3/src/widgets/st_base/
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/st_base/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/st_base/value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.868686 widgets-lib-2.7.3/src/widgets/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.872686 widgets-lib-2.7.3/src/widgets/streamlit/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/duplicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/expander.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.872686 widgets-lib-2.7.3/src/widgets/streamlit/resource/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/files/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/files/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/files/download_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.876685 widgets-lib-2.7.3/src/widgets/streamlit/resource/values/
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/values/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/values/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/values/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/values/multiselect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/values/selectstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/values/slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/values/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/resource/values/textarea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.876685 widgets-lib-2.7.3/src/widgets/streamlit/widget/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/streamlit/widget/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.876685 widgets-lib-2.7.3/src/widgets/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/templates/source.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/templates/streamlit_single.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/templates/streamlit_single.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/src/widgets/templates/streamlit_single_ga.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.876685 widgets-lib-2.7.3/src/widgets_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-01 20:55:01.000000 widgets-lib-2.7.3/src/widgets_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-01 20:55:01.000000 widgets-lib-2.7.3/src/widgets_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:55:01.000000 widgets-lib-2.7.3/src/widgets_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-01 20:55:01.000000 widgets-lib-2.7.3/src/widgets_lib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-01 20:55:01.000000 widgets-lib-2.7.3/src/widgets_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 20:55:01.000000 widgets-lib-2.7.3/src/widgets_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:55:01.880685 widgets-lib-2.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/tests/test_duplicator.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/tests/test_source_parents.py
--rw-r--r--   0 runner    (1001) docker     (123)    10120 2023-05-01 20:54:16.000000 widgets-lib-2.7.3/tests/test_streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:29:09.892491 widgets-lib-2.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-03 17:29:09.892491 widgets-lib-2.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 17:29:09.892491 widgets-lib-2.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:29:09.888491 widgets-lib-2.7.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:29:09.888491 widgets-lib-2.7.4/src/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:29:09.888491 widgets-lib-2.7.4/src/widgets/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/base/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/base/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21852 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/base/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/base/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:29:09.888491 widgets-lib-2.7.4/src/widgets/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:29:09.888491 widgets-lib-2.7.4/src/widgets/st_base/
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/st_base/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/st_base/value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:29:09.888491 widgets-lib-2.7.4/src/widgets/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/streamlit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:29:09.888491 widgets-lib-2.7.4/src/widgets/streamlit/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/streamlit/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/streamlit/resource/columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/streamlit/resource/duplicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/streamlit/resource/expander.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:29:09.892491 widgets-lib-2.7.4/src/widgets/streamlit/resource/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/streamlit/resource/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/streamlit/resource/files/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/streamlit/resource/files/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/streamlit/resource/files/download_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/streamlit/resource/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/streamlit/resource/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:29:09.892491 widgets-lib-2.7.4/src/widgets/streamlit/resource/values/
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/streamlit/resource/values/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/streamlit/resource/values/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/streamlit/resource/values/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/streamlit/resource/values/multiselect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/streamlit/resource/values/selectstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/streamlit/resource/values/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/streamlit/resource/values/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/streamlit/resource/values/textarea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:29:09.892491 widgets-lib-2.7.4/src/widgets/streamlit/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/streamlit/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/streamlit/widget/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:29:09.892491 widgets-lib-2.7.4/src/widgets/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/templates/source.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/templates/streamlit_single.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/templates/streamlit_single.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/src/widgets/templates/streamlit_single_ga.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:29:09.892491 widgets-lib-2.7.4/src/widgets_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-03 17:29:09.000000 widgets-lib-2.7.4/src/widgets_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-03 17:29:09.000000 widgets-lib-2.7.4/src/widgets_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 17:29:09.000000 widgets-lib-2.7.4/src/widgets_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-03 17:29:09.000000 widgets-lib-2.7.4/src/widgets_lib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 17:29:09.000000 widgets-lib-2.7.4/src/widgets_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 17:29:09.000000 widgets-lib-2.7.4/src/widgets_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:29:09.892491 widgets-lib-2.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/tests/test_duplicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/tests/test_source_parents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10120 2023-05-03 17:28:33.000000 widgets-lib-2.7.4/tests/test_streamlit.py
```

### Comparing `widgets-lib-2.7.3/LICENSE` & `widgets-lib-2.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/PKG-INFO` & `widgets-lib-2.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widgets-lib
-Version: 2.7.3
+Version: 2.7.4
 Summary: Merging code and data in webpages
 Author-email: Samuel Minot <sminot@fredhutch.org>
 Project-URL: Homepage, https://github.com/FredHutch/widgets
 Project-URL: Bug Tracker, https://github.com/FredHutch/widgets/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `widgets-lib-2.7.3/README.md` & `widgets-lib-2.7.4/README.md`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/pyproject.toml` & `widgets-lib-2.7.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets/base/exceptions.py` & `widgets-lib-2.7.4/src/widgets/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets/base/helpers.py` & `widgets-lib-2.7.4/src/widgets/base/helpers.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets/base/io.py` & `widgets-lib-2.7.4/src/widgets/base/io.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets/base/resource.py` & `widgets-lib-2.7.4/src/widgets/base/resource.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets/base/widget.py` & `widgets-lib-2.7.4/src/widgets/base/widget.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets/cli/main.py` & `widgets-lib-2.7.4/src/widgets/cli/main.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets/st_base/resource.py` & `widgets-lib-2.7.4/src/widgets/st_base/resource.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets/st_base/value.py` & `widgets-lib-2.7.4/src/widgets/st_base/value.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets/streamlit/__init__.py` & `widgets-lib-2.7.4/src/widgets/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets/streamlit/resource/columns.py` & `widgets-lib-2.7.4/src/widgets/streamlit/resource/columns.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     def __init__(
         self,
         id="columns",
         children: List[Resource] = [],
         spec=None,
         sidebar=True,
         gap="small",
+        disable_sidebar=False,
         **kwargs
     ) -> None:
         """
         Set up the StColumns object
         """
 
         # If no spec has been provided, or if an integer was provided
@@ -67,14 +68,15 @@
             id=id,
             children=children,
             label="",
             help="",
             spec=spec,
             gap=gap,
             sidebar=sidebar,
+            disable_sidebar=disable_sidebar,
             **kwargs
         )
 
     def prep(self) -> None:
         """
         Instantiate a column container and place the children
         in those containers.
```

### Comparing `widgets-lib-2.7.3/src/widgets/streamlit/resource/duplicator.py` & `widgets-lib-2.7.4/src/widgets/streamlit/resource/duplicator.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets/streamlit/resource/expander.py` & `widgets-lib-2.7.4/src/widgets/streamlit/resource/expander.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         self,
         id="expander",
         children: List[Resource] = [],
         label=None,
         help=None,
         expanded=False,
         sidebar=True,
+        disable_sidebar=False,
         **kwargs
     ) -> None:
         """
         Set up the StExpander object
         """
 
         # If the sidebar flag is set to False
@@ -33,14 +34,15 @@
         super().__init__(
             id=id,
             children=children,
             label=label,
             help=help,
             expanded=expanded,
             sidebar=sidebar,
+            disable_sidebar=disable_sidebar,
             **kwargs
         )
 
     def prep(self) -> None:
         """
         Instantiate a expand/collapse container
         """
```

### Comparing `widgets-lib-2.7.3/src/widgets/streamlit/resource/files/base.py` & `widgets-lib-2.7.4/src/widgets/streamlit/resource/files/base.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets/streamlit/resource/files/dataframe.py` & `widgets-lib-2.7.4/src/widgets/streamlit/resource/files/dataframe.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets/streamlit/resource/files/download_dataframe.py` & `widgets-lib-2.7.4/src/widgets/streamlit/resource/files/download_dataframe.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets/streamlit/resource/markdown.py` & `widgets-lib-2.7.4/src/widgets/streamlit/resource/markdown.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,25 +7,27 @@
     value = ""
     sidebar = False
 
     def __init__(
         self,
         id="markdown",
         value="",
-        sidebar=False
+        sidebar=False,
+        disable_sidebar=False,
     ) -> None:
         """
         Set up the attributes which are used by all Resource objects.
         """
 
         super().__init__(
             id=id,
             value=value,
             children=[],
-            sidebar=sidebar
+            sidebar=sidebar,
+            disable_sidebar=disable_sidebar
         )
 
     def run_self(self):
 
         self._get_ui_element(
             sidebar=self.sidebar,
             empty=True
```

### Comparing `widgets-lib-2.7.3/src/widgets/streamlit/resource/selector.py` & `widgets-lib-2.7.4/src/widgets/streamlit/resource/selector.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
     def __init__(
         self,
         id="selector",
         label="Select Resource",
         options: List[StResource] = None,
         value: Union[str, None] = None,
+        disable_sidebar=False,
         **kwargs
     ):
 
         # The user must have provided a list of Resources to select from
         if options is None:
             if self.__class__.options is None:
                 msg = f"Selector must have options provided ({id})"
@@ -74,14 +75,15 @@
                 StSelectString(
                     id='_selector_menu',
                     label=label,
                     options=label_list,
                     value=value
                 )
             ] + options,
+            disable_sidebar=disable_sidebar,
             **kwargs
         )
 
     def all_values(self, path=[], flatten=False, **kwargs) -> dict:
         """
         Return the .all_values() call of the child resource
         which is currently selected.
```

### Comparing `widgets-lib-2.7.3/src/widgets/streamlit/resource/values/checkbox.py` & `widgets-lib-2.7.4/src/widgets/streamlit/resource/values/checkbox.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets/streamlit/resource/values/float.py` & `widgets-lib-2.7.4/src/widgets/streamlit/resource/values/float.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets/streamlit/resource/values/integer.py` & `widgets-lib-2.7.4/src/widgets/streamlit/resource/values/integer.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets/streamlit/resource/values/multiselect.py` & `widgets-lib-2.7.4/src/widgets/streamlit/resource/values/multiselect.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets/streamlit/resource/values/selectstring.py` & `widgets-lib-2.7.4/src/widgets/streamlit/resource/values/selectstring.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets/streamlit/resource/values/slider.py` & `widgets-lib-2.7.4/src/widgets/streamlit/resource/values/slider.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets/streamlit/resource/values/string.py` & `widgets-lib-2.7.4/src/widgets/streamlit/resource/values/string.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets/streamlit/resource/values/textarea.py` & `widgets-lib-2.7.4/src/widgets/streamlit/resource/values/textarea.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets/streamlit/widget/base.py` & `widgets-lib-2.7.4/src/widgets/streamlit/widget/base.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets/templates/streamlit_single.html.j2` & `widgets-lib-2.7.4/src/widgets/templates/streamlit_single.html.j2`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets/templates/streamlit_single_ga.html.j2` & `widgets-lib-2.7.4/src/widgets/templates/streamlit_single_ga.html.j2`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/src/widgets_lib.egg-info/PKG-INFO` & `widgets-lib-2.7.4/src/widgets_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widgets-lib
-Version: 2.7.3
+Version: 2.7.4
 Summary: Merging code and data in webpages
 Author-email: Samuel Minot <sminot@fredhutch.org>
 Project-URL: Homepage, https://github.com/FredHutch/widgets
 Project-URL: Bug Tracker, https://github.com/FredHutch/widgets/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `widgets-lib-2.7.3/src/widgets_lib.egg-info/SOURCES.txt` & `widgets-lib-2.7.4/src/widgets_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/tests/test_base.py` & `widgets-lib-2.7.4/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/tests/test_cli.py` & `widgets-lib-2.7.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/tests/test_duplicator.py` & `widgets-lib-2.7.4/tests/test_duplicator.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/tests/test_helpers.py` & `widgets-lib-2.7.4/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/tests/test_io.py` & `widgets-lib-2.7.4/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/tests/test_source_parents.py` & `widgets-lib-2.7.4/tests/test_source_parents.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.7.3/tests/test_streamlit.py` & `widgets-lib-2.7.4/tests/test_streamlit.py`

 * *Files identical despite different names*

