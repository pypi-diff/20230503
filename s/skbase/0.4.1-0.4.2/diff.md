# Comparing `tmp/skbase-0.4.1.tar.gz` & `tmp/skbase-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skbase-0.4.1.tar", last modified: Wed Apr 26 19:06:04 2023, max compression
+gzip compressed data, was "skbase-0.4.2.tar", last modified: Tue May  2 20:55:49 2023, max compression
```

## Comparing `skbase-0.4.1.tar` & `skbase-0.4.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.796428 skbase-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-04-26 19:05:53.000000 skbase-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     6452 2023-04-26 19:06:04.796428 skbase-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3231 2023-04-26 19:05:53.000000 skbase-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.788428 skbase-0.4.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.792428 skbase-0.4.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     9845 2023-04-26 19:05:53.000000 skbase-0.4.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3294 2023-04-26 19:05:53.000000 skbase-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      347 2023-04-26 19:06:04.796428 skbase-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.792428 skbase-0.4.1/skbase/
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.792428 skbase-0.4.1/skbase/base/
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    42244 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/base/_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    35626 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/base/_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.792428 skbase-0.4.1/skbase/base/_pretty_printing/
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/base/_pretty_printing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11539 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/base/_pretty_printing/_object_html_repr.py
--rw-r--r--   0 runner    (1001) docker     (122)    15634 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/base/_pretty_printing/_pprint.py
--rw-r--r--   0 runner    (1001) docker     (122)     7290 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/base/_tagmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.792428 skbase-0.4.1/skbase/lookup/
--rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/lookup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    38915 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/lookup/_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.792428 skbase-0.4.1/skbase/lookup/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/lookup/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    36924 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/lookup/tests/test_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.792428 skbase-0.4.1/skbase/testing/
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    36016 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/testing/test_all_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.792428 skbase-0.4.1/skbase/testing/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/testing/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9890 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/testing/utils/_conditional_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)    10359 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/testing/utils/_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    11063 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/testing/utils/deep_equals.py
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/testing/utils/inspect.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.792428 skbase-0.4.1/skbase/testing/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/testing/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/testing/utils/tests/test_check_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/testing/utils/tests/test_deep_equals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.796428 skbase-0.4.1/skbase/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7803 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.796428 skbase-0.4.1/skbase/tests/mock_package/
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/tests/mock_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/tests/mock_package/test_mock_package.py
--rw-r--r--   0 runner    (1001) docker     (122)    40245 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4730 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/tests/test_baseestimator.py
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/tests/test_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.796428 skbase-0.4.1/skbase/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/utils/_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     8037 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/utils/_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4566 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/utils/_nested_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3134 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/utils/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.796428 skbase-0.4.1/skbase/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/utils/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     4918 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/utils/tests/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/utils/tests/test_nested_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/utils/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.796428 skbase-0.4.1/skbase/validate/
--rw-r--r--   0 runner    (1001) docker     (122)      676 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14918 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/validate/_named_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)    12123 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/validate/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.796428 skbase-0.4.1/skbase/validate/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       70 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/validate/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7438 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/validate/tests/test_iterable_named_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)    14131 2023-04-26 19:05:53.000000 skbase-0.4.1/skbase/validate/tests/test_type_validations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 19:06:04.792428 skbase-0.4.1/skbase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6452 2023-04-26 19:06:04.000000 skbase-0.4.1/skbase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1772 2023-04-26 19:06:04.000000 skbase-0.4.1/skbase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 19:06:04.000000 skbase-0.4.1/skbase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-26 19:06:04.000000 skbase-0.4.1/skbase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-26 19:06:04.000000 skbase-0.4.1/skbase.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 19:06:04.000000 skbase-0.4.1/skbase.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.979898 skbase-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-05-02 20:55:32.000000 skbase-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     6492 2023-05-02 20:55:49.979898 skbase-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-05-02 20:55:32.000000 skbase-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.971898 skbase-0.4.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.975898 skbase-0.4.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     9845 2023-05-02 20:55:32.000000 skbase-0.4.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-05-02 20:55:32.000000 skbase-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-05-02 20:55:49.979898 skbase-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.975898 skbase-0.4.2/skbase/
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.975898 skbase-0.4.2/skbase/base/
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43633 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/base/_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35626 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/base/_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.975898 skbase-0.4.2/skbase/base/_pretty_printing/
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/base/_pretty_printing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11539 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/base/_pretty_printing/_object_html_repr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15634 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/base/_pretty_printing/_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7290 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/base/_tagmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.975898 skbase-0.4.2/skbase/lookup/
+-rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/lookup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38936 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/lookup/_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.975898 skbase-0.4.2/skbase/lookup/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/lookup/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36924 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/lookup/tests/test_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.975898 skbase-0.4.2/skbase/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36450 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/testing/test_all_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.975898 skbase-0.4.2/skbase/testing/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/testing/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9890 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/testing/utils/_conditional_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10359 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/testing/utils/_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11063 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/testing/utils/deep_equals.py
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/testing/utils/inspect.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.975898 skbase-0.4.2/skbase/testing/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/testing/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/testing/utils/tests/test_check_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/testing/utils/tests/test_deep_equals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.979898 skbase-0.4.2/skbase/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7762 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.979898 skbase-0.4.2/skbase/tests/mock_package/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/tests/mock_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/tests/mock_package/test_mock_package.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41672 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4730 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/tests/test_baseestimator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/tests/test_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.979898 skbase-0.4.2/skbase/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/utils/_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8037 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/utils/_iter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4566 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/utils/_nested_iter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3134 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/utils/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.979898 skbase-0.4.2/skbase/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/utils/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4918 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/utils/tests/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/utils/tests/test_nested_iter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/utils/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.979898 skbase-0.4.2/skbase/validate/
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14777 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/validate/_named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12123 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/validate/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.979898 skbase-0.4.2/skbase/validate/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/validate/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7438 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/validate/tests/test_iterable_named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14131 2023-05-02 20:55:32.000000 skbase-0.4.2/skbase/validate/tests/test_type_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:55:49.975898 skbase-0.4.2/skbase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6492 2023-05-02 20:55:49.000000 skbase-0.4.2/skbase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1772 2023-05-02 20:55:49.000000 skbase-0.4.2/skbase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 20:55:49.000000 skbase-0.4.2/skbase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2023-05-02 20:55:49.000000 skbase-0.4.2/skbase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-02 20:55:49.000000 skbase-0.4.2/skbase.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 20:55:49.000000 skbase-0.4.2/skbase.egg-info/zip-safe
```

### Comparing `skbase-0.4.1/LICENSE` & `skbase-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/PKG-INFO` & `skbase-0.4.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skbase
-Version: 0.4.1
+Version: 0.4.2
 Summary: Base classes for sklearn-like parametric objects
 Author: Franz Király, Markus Löning, Ryan Kuhns
 Maintainer-email: Franz Kiraly <f.kiraly@ucl.ac.uk>, Ryan Kuhns <rk.skbase@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, skbase Developers
         All rights reserved.
@@ -69,22 +69,22 @@
 
 > A base class for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these
 design patterns.
 
-:rocket: Version 0.4.1 is now available. Checkout our
+:rocket: Version 0.4.2 is now available. Checkout our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
-| **Code** |  [![!pypi](https://img.shields.io/pypi/v/skbase?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/skbase)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
-| **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/skbase) [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/skbase) [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skbase) |
+| **Code** |  [![!pypi](https://img.shields.io/pypi/v/scikit-base?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
+| **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-13-orange.svg?style=flat-square)](#contributors)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 ## Documentation
```

### Comparing `skbase-0.4.1/README.md` & `skbase-0.4.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 > A base class for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these
 design patterns.
 
-:rocket: Version 0.4.1 is now available. Checkout our
+:rocket: Version 0.4.2 is now available. Checkout our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
-| **Code** |  [![!pypi](https://img.shields.io/pypi/v/skbase?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/skbase)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
-| **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/skbase) [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/skbase) [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skbase) |
+| **Code** |  [![!pypi](https://img.shields.io/pypi/v/scikit-base?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
+| **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-13-orange.svg?style=flat-square)](#contributors)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 ## Documentation
```

### Comparing `skbase-0.4.1/docs/source/conf.py` & `skbase-0.4.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/pyproject.toml` & `skbase-0.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "skbase"
-version = "0.4.1"
+version = "0.4.2"
 description = "Base classes for sklearn-like parametric objects"
 authors = [
     {name = "Franz Király"},
     {name = "Markus Löning"},
     {name = "Ryan Kuhns"},
 ]
 maintainers = [
@@ -31,22 +31,21 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 requires-python = ">=3.7,<3.12"
-dependencies = [
-    "scikit-learn>=0.24.0,<1.3.0", "typing-extensions", "pytest"
-]
+dependencies = []
 
 [project.optional-dependencies]
 all_extras = ["numpy", "pandas"]
 
 dev = [
+    "scikit-learn>=0.24.0",
     "pre-commit",
     "pytest",
     "pytest-cov"
 ]
 
 linters = [
     "mypy",
@@ -69,30 +68,31 @@
 
 docs = [
     "jupyter",
     "myst-parser",
     "nbsphinx>=0.8.6",
     "numpydoc",
     "pydata-sphinx-theme",
-    "sphinx-copybutton",
-    "sphinx-issues",
-    "sphinx-gallery",
+    "sphinx_issues==1.2.0",
+    "sphinx-gallery==0.6.0",
     "sphinx-panels",
-    "sphinx-design",
-    "sphinx",
+    "sphinx-design==0.3.0",
+    "sphinx==4.1.1",
+    "tabulate",
 ]
 
 test = [
     "pytest",
     "coverage",
     "pytest-cov",
     "safety",
     "numpy",
     "scipy",
     "pandas",
+    "scikit-learn>=0.24.0",
 ]
 
 [project.urls]
 homepage = "https://github.com/sktime/skbase"
 repository = "https://github.com/sktime/skbase"
 documentation = "https://github.com/sktime/skbase"
 download = "https://pypi.org/project/skbase/#files"
```

### Comparing `skbase-0.4.1/skbase/_exceptions.py` & `skbase-0.4.2/skbase/_exceptions.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/base/__init__.py` & `skbase-0.4.2/skbase/base/__init__.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/base/_base.py` & `skbase-0.4.2/skbase/base/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,34 +55,32 @@
 import inspect
 import re
 import warnings
 from collections import defaultdict
 from copy import deepcopy
 from typing import List
 
-from sklearn import clone
-from sklearn.base import BaseEstimator as _BaseEstimator
-
 from skbase._exceptions import NotFittedError
 from skbase.base._pretty_printing._object_html_repr import _object_html_repr
 from skbase.base._tagmanager import _FlagManager
 
 __author__: List[str] = ["mloning", "RNKuhns", "fkiraly"]
 __all__: List[str] = ["BaseEstimator", "BaseObject"]
 
 
-class BaseObject(_FlagManager, _BaseEstimator):
+class BaseObject(_FlagManager):
     """Base class for parametric objects with sktime style tag interface.
 
     Extends scikit-learn's BaseEstimator to include sktime style interface for tags.
     """
 
     _config = {
         "display": "diagram",
         "print_changed_only": True,
+        "check_clone": True,  # whether to execute validity checks in clone
     }
 
     def __init__(self):
         """Construct BaseObject."""
         self._init_flags(flag_attr_name="_tags")
         self._init_flags(flag_attr_name="_config")
         super(BaseObject, self).__init__()
@@ -144,19 +142,52 @@
 
     def clone(self):
         """Obtain a clone of the object with same hyper-parameters.
 
         A clone is a different object without shared references, in post-init state.
         This function is equivalent to returning sklearn.clone of self.
 
+        Raises
+        ------
+        RuntimeError if the clone is non-conforming, due to faulty ``__init__``.
+
         Notes
         -----
-        Also equal in value to `type(self)(**self.get_params(deep=False))`.
+        If successful, equal in value to ``type(self)(**self.get_params(deep=False))``.
         """
-        return clone(self)
+        self_params = self.get_params(deep=False)
+        self_clone = type(self)(**self_params)
+
+        # if checking the clone is turned off, return now
+        if not self.get_config()["check_clone"]:
+            return self_clone
+
+        from skbase.testing.utils.deep_equals import deep_equals
+
+        # check that all attributes are written to the clone
+        for attrname in self_params.keys():
+            if not hasattr(self_clone, attrname):
+                raise RuntimeError(
+                    f"error in {self}.clone, __init__ must write all arguments "
+                    f"to self and not mutate them, but {attrname} was not found. "
+                    f"Please check __init__ of {self}."
+                )
+
+        clone_attrs = {attr: getattr(self_clone, attr) for attr in self_params.keys()}
+
+        # check equality of parameters post-clone and pre-clone
+        clone_attrs_valid, msg = deep_equals(self_params, clone_attrs, return_msg=True)
+        if not clone_attrs_valid:
+            raise RuntimeError(
+                f"error in {self}.clone, __init__ must write all arguments "
+                f"to self and not mutate them, but this is not the case. "
+                f"Error on equality check of arguments (x) vs parameters (y): {msg}"
+            )
+
+        return self_clone
 
     @classmethod
     def _get_init_signature(cls):
         """Get class init sigature.
 
         Useful in parameter inspection.
```

### Comparing `skbase-0.4.1/skbase/base/_meta.py` & `skbase-0.4.2/skbase/base/_meta.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/base/_pretty_printing/_object_html_repr.py` & `skbase-0.4.2/skbase/base/_pretty_printing/_object_html_repr.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/base/_pretty_printing/_pprint.py` & `skbase-0.4.2/skbase/base/_pretty_printing/_pprint.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/base/_tagmanager.py` & `skbase-0.4.2/skbase/base/_tagmanager.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/lookup/__init__.py` & `skbase-0.4.2/skbase/lookup/__init__.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/lookup/_lookup.py` & `skbase-0.4.2/skbase/lookup/_lookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,83 +21,69 @@
 import pathlib
 import pkgutil
 import sys
 import warnings
 from collections.abc import Iterable
 from copy import deepcopy
 from operator import itemgetter
-from types import FunctionType, ModuleType
-from typing import (
-    Any,
-    List,
-    Mapping,
-    MutableMapping,
-    Optional,
-    Sequence,
-    Tuple,
-    Type,
-    Union,
-)
+from types import ModuleType
+from typing import Any, List, Mapping, MutableMapping, Optional, Sequence, Tuple, Union
 
 from skbase.base import BaseObject
 from skbase.validate import check_sequence
 
-# Conditionally import TypedDict based on Python version
-if sys.version_info >= (3, 8):
-    from typing import TypedDict
-else:
-    from typing_extensions import TypedDict
-
 __all__: List[str] = ["all_objects", "get_package_metadata"]
 __author__: List[str] = [
     "fkiraly",
     "mloning",
     "katiebuc",
     "miraep8",
     "xloem",
     "rnkuhns",
 ]
 
+# the below is commented out to avoid a dependency on typing_extensions
+# but still left in place as it is informative regarding expected return type
 
-class ClassInfo(TypedDict):
-    """Type definitions for information on a module's classes."""
+# class ClassInfo(TypedDict):
+#     """Type definitions for information on a module's classes."""
 
-    klass: Type
-    name: str
-    description: str
-    tags: MutableMapping[str, Any]
-    is_concrete_implementation: bool
-    is_base_class: bool
-    is_base_object: bool
-    authors: Optional[Union[List[str], str]]
-    module_name: str
-
-
-class FunctionInfo(TypedDict):
-    """Information on a module's functions."""
-
-    func: FunctionType
-    name: str
-    description: str
-    module_name: str
-
-
-class ModuleInfo(TypedDict):
-    """Module information type definitions."""
-
-    path: str
-    name: str
-    classes: MutableMapping[str, ClassInfo]
-    functions: MutableMapping[str, FunctionInfo]
-    __all__: List[str]
-    authors: str
-    is_package: bool
-    contains_concrete_class_implementations: bool
-    contains_base_classes: bool
-    contains_base_objects: bool
+#     klass: Type
+#     name: str
+#     description: str
+#     tags: MutableMapping[str, Any]
+#     is_concrete_implementation: bool
+#     is_base_class: bool
+#     is_base_object: bool
+#     authors: Optional[Union[List[str], str]]
+#     module_name: str
+
+
+# class FunctionInfo(TypedDict):
+#     """Information on a module's functions."""
+
+#     func: FunctionType
+#     name: str
+#     description: str
+#     module_name: str
+
+
+# class ModuleInfo(TypedDict):
+#     """Module information type definitions."""
+
+#     path: str
+#     name: str
+#     classes: MutableMapping[str, ClassInfo]
+#     functions: MutableMapping[str, FunctionInfo]
+#     __all__: List[str]
+#     authors: str
+#     is_package: bool
+#     contains_concrete_class_implementations: bool
+#     contains_base_classes: bool
+#     contains_base_objects: bool
 
 
 def _is_non_public_module(module_name: str) -> bool:
     """Determine if a module is non-public or not.
 
     Parameters
     ----------
@@ -402,15 +388,15 @@
     is_pkg: bool,
     path: str,
     package_base_classes: Union[type, Tuple[type, ...]],
     exclude_non_public_items: bool = True,
     class_filter: Optional[Union[type, Sequence[type]]] = None,
     tag_filter: Optional[Union[str, Sequence[str], Mapping[str, Any]]] = None,
     classes_to_exclude: Optional[Union[type, Sequence[type]]] = None,
-) -> ModuleInfo:
+) -> dict:  # of ModuleInfo type
     # Make package_base_classes a tuple if it was supplied as a class
     base_classes_none = False
     if isinstance(package_base_classes, Iterable):
         package_base_classes = tuple(package_base_classes)
     elif not isinstance(package_base_classes, tuple):
         if package_base_classes is None:
             base_classes_none = True
@@ -425,15 +411,15 @@
         exclude_classes = (classes_to_exclude,)
 
     designed_imports: List[str] = getattr(module, "__all__", [])
     authors: Union[str, List[str]] = getattr(module, "__author__", [])
     if isinstance(authors, (list, tuple)):
         authors = ", ".join(authors)
     # Compile information on classes in the module
-    module_classes: MutableMapping[str, ClassInfo] = {}
+    module_classes: MutableMapping = {}  # of ClassInfo type
     for name, klass in inspect.getmembers(module, inspect.isclass):
         # Skip a class if non-public items should be excluded and it starts with "_"
         if (
             (exclude_non_public_items and klass.__name__.startswith("_"))
             or (exclude_classes is not None and klass in exclude_classes)
             or not _filter_by_tags(klass, tag_filter=tag_filter)
             or not _filter_by_class(klass, class_filter=class_filter)
@@ -463,15 +449,15 @@
                 "is_concrete_implementation": concrete_implementation,
                 "is_base_class": klass in package_base_classes,
                 "is_base_object": issubclass(klass, BaseObject),
                 "authors": klass_authors,
                 "module_name": module.__name__,
             }
 
-    module_functions: MutableMapping[str, FunctionInfo] = {}
+    module_functions: MutableMapping = {}  # of FunctionInfo type
     for name, func in inspect.getmembers(module, inspect.isfunction):
         if func.__module__ == module.__name__ or name in designed_imports:
             # Skip a class if non-public items should be excluded and it starts with "_"
             if exclude_non_public_items and func.__name__.startswith("_"):
                 continue
             # Otherwise, store info about the class
             module_functions[name] = {
@@ -480,15 +466,15 @@
                 "description": (
                     "" if func.__doc__ is None else func.__doc__.split("\n")[0]
                 ),
                 "module_name": module.__name__,
             }
 
     # Combine all the information on the module together
-    module_info: ModuleInfo = {
+    module_info = {  # of ModuleInfo type
         "path": path,
         "name": module.__name__,
         "classes": module_classes,
         "functions": module_functions,
         "__all__": designed_imports,
         "authors": authors,
         "is_package": is_pkg,
@@ -513,15 +499,15 @@
     exclude_non_public_modules: bool = True,
     modules_to_ignore: Union[str, List[str], Tuple[str]] = ("tests",),
     package_base_classes: Union[type, Tuple[type, ...]] = (BaseObject,),
     class_filter: Optional[Union[type, Sequence[type]]] = None,
     tag_filter: Optional[Union[str, Sequence[str], Mapping[str, Any]]] = None,
     classes_to_exclude: Optional[Union[type, Sequence[type]]] = None,
     suppress_import_stdout: bool = True,
-) -> Mapping[str, ModuleInfo]:
+) -> Mapping:  # of ModuleInfo type
     """Return a dictionary mapping all package modules to their metadata.
 
     Parameters
     ----------
     package_name : str
         The name of the package/module to return metadata for.
 
@@ -602,15 +588,15 @@
           inherit from ``BaseObject`` and are not `package_base_classes`.
         - "contains_base_classes": whether any module classes that are
           `package_base_classes`.
         - "contains_base_objects": whether any module classes that
           inherit from ``BaseObject``.
     """
     module, path, loader = _determine_module_path(package_name, path)
-    module_info: MutableMapping[str, ModuleInfo] = {}
+    module_info: MutableMapping = {}  # of ModuleInfo type
     # Get any metadata at the top-level of the provided package
     # This is because the pkgutil.walk_packages doesn't include __init__
     # file when walking a package
     if not _is_ignored_module(package_name, modules_to_ignore=modules_to_ignore):
         module_info[package_name] = _get_module_info(
             module,
             loader.is_package(package_name),
```

### Comparing `skbase-0.4.1/skbase/lookup/tests/test_lookup.py` & `skbase-0.4.2/skbase/lookup/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/testing/test_all_objects.py` & `skbase-0.4.2/skbase/testing/test_all_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,26 +6,23 @@
 """
 import numbers
 import types
 from copy import deepcopy
 from inspect import getfullargspec, isclass, signature
 from typing import List
 
-import joblib
 import numpy as np
 import pytest
-from sklearn.utils.estimator_checks import (
-    check_get_params_invariance as _check_get_params_invariance,
-)
 
 from skbase.base import BaseObject
 from skbase.lookup import all_objects
 from skbase.testing.utils._conditional_fixtures import (
     create_conditional_fixtures_and_names,
 )
+from skbase.testing.utils._dependencies import _check_soft_dependencies
 from skbase.testing.utils.deep_equals import deep_equals
 from skbase.testing.utils.inspect import _get_args
 
 __author__: List[str] = ["fkiraly"]
 
 
 class BaseFixtureGenerator:
@@ -658,16 +655,24 @@
 
     @pytest.mark.parametrize("a", [True, 42])
     def test_no_between_test_case_side_effects(self, object_instance, a):
         """Test that there are no side effects across instances of the same test."""
         assert not hasattr(object_instance, "test__attr")
         object_instance.test__attr = 42
 
+    @pytest.mark.skipif(
+        not _check_soft_dependencies("sklearn", severity="none"),
+        reason="skip test if sklearn is not available",
+    )  # sklearn is part of the dev dependency set, test should be executed with that
     def test_get_params(self, object_instance):
-        """Check that get_params works correctly."""
+        """Check that get_params works correctly, against sklearn interface."""
+        from sklearn.utils.estimator_checks import (
+            check_get_params_invariance as _check_get_params_invariance,
+        )
+
         params = object_instance.get_params()
         assert isinstance(params, dict)
         _check_get_params_invariance(
             object_instance.__class__.__name__, object_instance
         )
 
     def test_set_params(self, object_instance):
@@ -794,34 +799,39 @@
 
         init_params = [
             param
             for param in init_params
             if param.name not in required_params and param.name not in test_params
         ]
 
+        allowed_param_types = [
+            str,
+            int,
+            float,
+            bool,
+            tuple,
+            type(None),
+            np.float64,
+            types.FunctionType,
+        ]
+        if _check_soft_dependencies("joblib", severity="none"):
+            from joblib import Memory
+
+            allowed_param_types += [Memory]
+
         for param in init_params:
             assert param.default != param.empty, (
                 "parameter `%s` for %s has no default value and is not "
                 "included in `_required_parameters`"
                 % (param.name, obj.__class__.__name__)
             )
             if type(param.default) is type:
                 assert param.default in [np.float64, np.int64]
             else:
-                assert type(param.default) in [
-                    str,
-                    int,
-                    float,
-                    bool,
-                    tuple,
-                    type(None),
-                    np.float64,
-                    types.FunctionType,
-                    joblib.Memory,
-                ]
+                assert type(param.default) in allowed_param_types
 
             param_value = params[param.name]
             if isinstance(param_value, np.ndarray):
                 np.testing.assert_array_equal(param_value, param.default)
             else:
                 if bool(
                     isinstance(param_value, numbers.Real) and np.isnan(param_value)
```

### Comparing `skbase-0.4.1/skbase/testing/utils/_conditional_fixtures.py` & `skbase-0.4.2/skbase/testing/utils/_conditional_fixtures.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/testing/utils/_dependencies.py` & `skbase-0.4.2/skbase/testing/utils/_dependencies.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/testing/utils/deep_equals.py` & `skbase-0.4.2/skbase/testing/utils/deep_equals.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/testing/utils/inspect.py` & `skbase-0.4.2/skbase/testing/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/testing/utils/tests/test_check_dependencies.py` & `skbase-0.4.2/skbase/testing/utils/tests/test_check_dependencies.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/testing/utils/tests/test_deep_equals.py` & `skbase-0.4.2/skbase/testing/utils/tests/test_deep_equals.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/tests/conftest.py` & `skbase-0.4.2/skbase/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         "BaseMetaEstimator",
         "BaseMetaObject",
         "BaseObject",
     ),
     "skbase.base._base": ("BaseEstimator", "BaseObject"),
     "skbase.base._meta": ("BaseMetaObject", "BaseMetaEstimator"),
     "skbase.base._pretty_printing._pprint": ("KeyValTuple", "KeyValTupleParam"),
-    "skbase.lookup._lookup": ("ClassInfo", "FunctionInfo", "ModuleInfo"),
+    "skbase.lookup._lookup": (),
     "skbase.testing": ("BaseFixtureGenerator", "QuickTester", "TestAllObjects"),
     "skbase.testing.test_all_objects": (
         "BaseFixtureGenerator",
         "QuickTester",
         "TestAllObjects",
     ),
 }
```

### Comparing `skbase-0.4.1/skbase/tests/mock_package/test_mock_package.py` & `skbase-0.4.2/skbase/tests/mock_package/test_mock_package.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/tests/test_base.py` & `skbase-0.4.2/skbase/tests/test_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,18 +71,16 @@
 from copy import deepcopy
 from typing import Any, Dict, Type
 
 import numpy as np
 import pytest
 import scipy.sparse as sp
 
-# TODO: Update with import of skbase clone function once implemented
-from sklearn.base import clone
-
 from skbase.base import BaseEstimator, BaseObject
+from skbase.testing.utils._dependencies import _check_soft_dependencies
 from skbase.tests.conftest import Child, Parent
 from skbase.tests.mock_package.test_mock_package import CompositionDummy
 
 
 # TODO: Determine if we need to add sklearn style test of
 # test_set_params_passes_all_parameters
 class ResetTester(BaseObject):
@@ -137,15 +135,15 @@
     def __init__(self, a=None):
         self.a = 1
         self._a = a
         super().__init__()
 
 
 class ModifyParam(BaseObject):
-    """A non-conforming BaseObject that modifyies parameters in init."""
+    """A non-conforming BaseObject that modifies parameters in init."""
 
     def __init__(self, a=7):
         self.a = deepcopy(a)
         super().__init__()
 
 
 @pytest.fixture
@@ -819,61 +817,89 @@
     with pytest.raises(RuntimeError):
         buggy.clone()
 
     varg_obj = fixture_invalid_init(a=7)
     with pytest.raises(RuntimeError):
         varg_obj.clone()
 
-    obj_that_modifies = fixture_modify_param(a=[0])
-    with pytest.raises(RuntimeError):
-        obj_that_modifies.clone()
+    # fkiraly note: I don't think this class violates the contract,
+    # as equality is defined as via deepcopy
+    # leaving the code here for reference and potential discussion
+    #
+    # obj_that_modifies = fixture_modify_param(a=[0])
+    # with pytest.raises(RuntimeError):
+    #     obj_that_modifies.clone()
 
 
+@pytest.mark.skipif(
+    not _check_soft_dependencies("sklearn", severity="none"),
+    reason="skip test if sklearn is not available",
+)  # sklearn is part of the dev dependency set, test should be executed with that
 def test_clone_param_is_none(fixture_class_parent: Type[Parent]):
     """Test clone with keyword parameter set to None."""
+    from sklearn.base import clone
+
     base_obj = fixture_class_parent(c=None)
     new_base_obj = clone(base_obj)
     new_base_obj2 = base_obj.clone()
     assert base_obj.c is new_base_obj.c
     assert base_obj.c is new_base_obj2.c
 
 
+@pytest.mark.skipif(
+    not _check_soft_dependencies("sklearn", severity="none"),
+    reason="skip test if sklearn is not available",
+)  # sklearn is part of the dev dependency set, test should be executed with that
 def test_clone_empty_array(fixture_class_parent: Type[Parent]):
     """Test clone with keyword parameter is scipy sparse matrix.
 
     This test is based on scikit-learn regression test to make sure clone
     works with default parameter set to scipy sparse matrix.
     """
+    from sklearn.base import clone
+
     # Regression test for cloning estimators with empty arrays
     base_obj = fixture_class_parent(c=np.array([]))
     new_base_obj = clone(base_obj)
     new_base_obj2 = base_obj.clone()
     np.testing.assert_array_equal(base_obj.c, new_base_obj.c)
     np.testing.assert_array_equal(base_obj.c, new_base_obj2.c)
 
 
+@pytest.mark.skipif(
+    not _check_soft_dependencies("sklearn", severity="none"),
+    reason="skip test if sklearn is not available",
+)  # sklearn is part of the dev dependency set, test should be executed with that
 def test_clone_sparse_matrix(fixture_class_parent: Type[Parent]):
     """Test clone with keyword parameter is scipy sparse matrix.
 
     This test is based on scikit-learn regression test to make sure clone
     works with default parameter set to scipy sparse matrix.
     """
+    from sklearn.base import clone
+
     base_obj = fixture_class_parent(c=sp.csr_matrix(np.array([[0]])))
     new_base_obj = clone(base_obj)
     new_base_obj2 = base_obj.clone()
     np.testing.assert_array_equal(base_obj.c, new_base_obj.c)
     np.testing.assert_array_equal(base_obj.c, new_base_obj2.c)
 
 
+@pytest.mark.skipif(
+    not _check_soft_dependencies("sklearn", severity="none"),
+    reason="skip test if sklearn is not available",
+)  # sklearn is part of the dev dependency set, test should be executed with that
 def test_clone_nan(fixture_class_parent: Type[Parent]):
     """Test clone with keyword parameter is np.nan.
 
     This test is based on scikit-learn regression test to make sure clone
     works with default parameter set to np.nan.
     """
+    from sklearn.base import clone
+
     # Regression test for cloning estimators with default parameter as np.nan
     base_obj = fixture_class_parent(c=np.nan)
     new_base_obj = clone(base_obj)
     new_base_obj2 = base_obj.clone()
 
     assert base_obj.c is new_base_obj.c
     assert base_obj.c is new_base_obj2.c
@@ -883,18 +909,24 @@
     """Test clone works for parameters that are types rather than instances."""
     base_obj = fixture_class_parent(c=fixture_class_parent)
     new_base_obj = base_obj.clone()
 
     assert base_obj.c == new_base_obj.c
 
 
+@pytest.mark.skipif(
+    not _check_soft_dependencies("sklearn", severity="none"),
+    reason="skip test if sklearn is not available",
+)  # sklearn is part of the dev dependency set, test should be executed with that
 def test_clone_class_rather_than_instance_raises_error(
     fixture_class_parent: Type[Parent],
 ):
     """Test clone raises expected error when cloning a class instead of an instance."""
+    from sklearn.base import clone
+
     msg = "You should provide an instance of scikit-learn estimator"
     with pytest.raises(TypeError, match=msg):
         clone(fixture_class_parent)
 
 
 # Tests of BaseObject pretty printing representation inspired by sklearn
 def test_baseobject_repr(
```

### Comparing `skbase-0.4.1/skbase/tests/test_baseestimator.py` & `skbase-0.4.2/skbase/tests/test_baseestimator.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/tests/test_exceptions.py` & `skbase-0.4.2/skbase/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/tests/test_meta.py` & `skbase-0.4.2/skbase/tests/test_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     # Verify that BaseMetaEstimator is an estimator
     assert (
         estimator_is_subclass_of_baseobejct
         and estimator_instance_is_baseobject_instance
     ), "`BaseMetaEstimator` not correctly subclassing `BaseEstimator` and `BaseObject`."
 
     # Verify expected MRO inherittence order
-    assert BaseMetaEstimator.__mro__[:-3] == (
+    assert BaseMetaEstimator.__mro__[:-2] == (
         BaseMetaEstimator,
         _MetaObjectMixin,
         _MetaTagLogicMixin,
         BaseEstimator,
         BaseObject,
     ), "`BaseMetaEstimator` has incorrect mro."
```

### Comparing `skbase-0.4.1/skbase/utils/__init__.py` & `skbase-0.4.2/skbase/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/utils/_check.py` & `skbase-0.4.2/skbase/utils/_check.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/utils/_iter.py` & `skbase-0.4.2/skbase/utils/_iter.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/utils/_nested_iter.py` & `skbase-0.4.2/skbase/utils/_nested_iter.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/utils/_utils.py` & `skbase-0.4.2/skbase/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/utils/tests/test_check.py` & `skbase-0.4.2/skbase/utils/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/utils/tests/test_iter.py` & `skbase-0.4.2/skbase/utils/tests/test_iter.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/utils/tests/test_nested_iter.py` & `skbase-0.4.2/skbase/utils/tests/test_nested_iter.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/utils/tests/test_utils.py` & `skbase-0.4.2/skbase/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/validate/__init__.py` & `skbase-0.4.2/skbase/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/validate/_named_objects.py` & `skbase-0.4.2/skbase/validate/_named_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # -*- coding: utf-8 -*-
 # copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
 """Validate if an input is one of the allowed named object formats."""
 import collections.abc
-import sys
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     List,
     Optional,
     Sequence,
     Tuple,
     Union,
     overload,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
-
 from skbase.base import BaseObject
 
 __all__: List[str] = [
     "check_sequence_named_objects",
     "is_named_object_tuple",
     "is_sequence_named_objects",
 ]
@@ -252,26 +246,26 @@
 
     return is_expected_format
 
 
 @overload
 def check_sequence_named_objects(
     seq_to_check: Union[Sequence[Tuple[str, BaseObject]], Dict[str, BaseObject]],
-    allow_dict: Literal[True] = True,
+    allow_dict: bool = True,
     require_unique_names=False,
     object_type: Optional[Union[type, Tuple[type]]] = None,
     sequence_name: Optional[str] = None,
 ) -> Union[Sequence[Tuple[str, BaseObject]], Dict[str, BaseObject]]:
     ...  # pragma: no cover
 
 
 @overload
 def check_sequence_named_objects(
     seq_to_check: Sequence[Tuple[str, BaseObject]],
-    allow_dict: Literal[False],
+    allow_dict: bool,
     require_unique_names=False,
     object_type: Optional[Union[type, Tuple[type]]] = None,
     sequence_name: Optional[str] = None,
 ) -> Sequence[Tuple[str, BaseObject]]:
     ...  # pragma: no cover
```

### Comparing `skbase-0.4.1/skbase/validate/_types.py` & `skbase-0.4.2/skbase/validate/_types.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/validate/tests/test_iterable_named_objects.py` & `skbase-0.4.2/skbase/validate/tests/test_iterable_named_objects.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase/validate/tests/test_type_validations.py` & `skbase-0.4.2/skbase/validate/tests/test_type_validations.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.1/skbase.egg-info/PKG-INFO` & `skbase-0.4.2/skbase.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skbase
-Version: 0.4.1
+Version: 0.4.2
 Summary: Base classes for sklearn-like parametric objects
 Author: Franz Király, Markus Löning, Ryan Kuhns
 Maintainer-email: Franz Kiraly <f.kiraly@ucl.ac.uk>, Ryan Kuhns <rk.skbase@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, skbase Developers
         All rights reserved.
@@ -69,22 +69,22 @@
 
 > A base class for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these
 design patterns.
 
-:rocket: Version 0.4.1 is now available. Checkout our
+:rocket: Version 0.4.2 is now available. Checkout our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
-| **Code** |  [![!pypi](https://img.shields.io/pypi/v/skbase?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/skbase)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
-| **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/skbase) [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/skbase) [![Downloads](https://static.pepy.tech/personalized-badge/skbase?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skbase) |
+| **Code** |  [![!pypi](https://img.shields.io/pypi/v/scikit-base?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
+| **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-13-orange.svg?style=flat-square)](#contributors)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 ## Documentation
```

### Comparing `skbase-0.4.1/skbase.egg-info/SOURCES.txt` & `skbase-0.4.2/skbase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

