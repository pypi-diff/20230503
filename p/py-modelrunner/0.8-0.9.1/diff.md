# Comparing `tmp/py-modelrunner-0.8.tar.gz` & `tmp/py-modelrunner-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-modelrunner-0.8.tar", last modified: Sun Nov 20 10:09:33 2022, max compression
+gzip compressed data, was "py-modelrunner-0.9.1.tar", last modified: Wed Nov 30 09:30:44 2022, max compression
```

## Comparing `py-modelrunner-0.8.tar` & `py-modelrunner-0.9.1.tar`

### file list

```diff
@@ -1,41 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 10:09:33.219696 py-modelrunner-0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-20 10:09:22.000000 py-modelrunner-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-11-20 10:09:22.000000 py-modelrunner-0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    12461 2022-11-20 10:09:33.219696 py-modelrunner-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9393 2022-11-20 10:09:22.000000 py-modelrunner-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 10:09:33.219696 py-modelrunner-0.8/modelrunner/
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-11-20 10:09:22.000000 py-modelrunner-0.8/modelrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-11-20 10:09:22.000000 py-modelrunner-0.8/modelrunner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12820 2022-11-20 10:09:22.000000 py-modelrunner-0.8/modelrunner/model.py
--rw-r--r--   0 runner    (1001) docker     (121)    24914 2022-11-20 10:09:22.000000 py-modelrunner-0.8/modelrunner/parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-11-20 10:09:22.000000 py-modelrunner-0.8/modelrunner/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    18371 2022-11-20 10:09:22.000000 py-modelrunner-0.8/modelrunner/results.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 10:09:33.219696 py-modelrunner-0.8/modelrunner/run/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-11-20 10:09:22.000000 py-modelrunner-0.8/modelrunner/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1577 2022-11-20 10:09:22.000000 py-modelrunner-0.8/modelrunner/run/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9037 2022-11-20 10:09:22.000000 py-modelrunner-0.8/modelrunner/run/job.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 10:09:33.219696 py-modelrunner-0.8/modelrunner/run/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-11-20 10:09:22.000000 py-modelrunner-0.8/modelrunner/run/templates/background.template
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-11-20 10:09:22.000000 py-modelrunner-0.8/modelrunner/run/templates/foreground.template
--rw-r--r--   0 runner    (1001) docker     (121)      714 2022-11-20 10:09:22.000000 py-modelrunner-0.8/modelrunner/run/templates/qsub.template
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 10:09:33.219696 py-modelrunner-0.8/modelrunner/run/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-20 10:09:22.000000 py-modelrunner-0.8/modelrunner/run/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2805 2022-11-20 10:09:22.000000 py-modelrunner-0.8/modelrunner/run/tests/test_job.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 10:09:33.219696 py-modelrunner-0.8/modelrunner/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-20 10:09:22.000000 py-modelrunner-0.8/modelrunner/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-11-20 10:09:22.000000 py-modelrunner-0.8/modelrunner/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (121)      707 2022-11-20 10:09:22.000000 py-modelrunner-0.8/modelrunner/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (121)     7090 2022-11-20 10:09:22.000000 py-modelrunner-0.8/modelrunner/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     6982 2022-11-20 10:09:22.000000 py-modelrunner-0.8/modelrunner/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     3434 2022-11-20 10:09:22.000000 py-modelrunner-0.8/modelrunner/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-11-20 10:09:22.000000 py-modelrunner-0.8/modelrunner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 10:09:33.219696 py-modelrunner-0.8/py_modelrunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12461 2022-11-20 10:09:33.000000 py-modelrunner-0.8/py_modelrunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      931 2022-11-20 10:09:33.000000 py-modelrunner-0.8/py_modelrunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-20 10:09:33.000000 py-modelrunner-0.8/py_modelrunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-20 10:09:33.000000 py-modelrunner-0.8/py_modelrunner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-20 10:09:33.000000 py-modelrunner-0.8/py_modelrunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-20 10:09:33.000000 py-modelrunner-0.8/py_modelrunner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-20 10:09:22.000000 py-modelrunner-0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-11-20 10:09:33.219696 py-modelrunner-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2198 2022-11-20 10:09:22.000000 py-modelrunner-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 09:30:44.115020 py-modelrunner-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 09:30:44.103020 py-modelrunner-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 09:30:44.107020 py-modelrunner-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/.github/workflows/coverage_report.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/.github/workflows/release_pip.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2022-11-30 09:30:44.115020 py-modelrunner-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 09:30:44.107020 py-modelrunner-0.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)       49 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/docs/build_all.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 09:30:44.107020 py-modelrunner-0.9.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/docs/source/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7847 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/docs/source/installation.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1964 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/docs/source/run_autodoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/docs/source/sphinx_simplify_typehints.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/docs/source/structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 09:30:44.107020 py-modelrunner-0.9.1/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      656 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/examples/io_hdf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      519 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/examples/io_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      519 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/examples/io_yaml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      439 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/examples/model_class.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      330 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/examples/model_decorator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      365 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/examples/model_function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      672 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/examples/read_many.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      437 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/examples/script_custom_func.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      405 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/examples/script_function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      593 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/examples/script_many_classes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      255 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/examples/script_minimal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      359 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/examples/script_model_class.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      629 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/examples/submit_function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      775 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/examples/submit_many_func.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      928 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/examples/submit_many_iter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      654 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/examples/submit_shebang.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 09:30:44.111020 py-modelrunner-0.9.1/modelrunner/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2022-11-30 09:30:43.000000 py-modelrunner-0.9.1/modelrunner/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14805 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24914 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18515 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 09:30:44.111020 py-modelrunner-0.9.1/modelrunner/run/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/run/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/run/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 09:30:44.111020 py-modelrunner-0.9.1/modelrunner/run/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/run/templates/background.template
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/run/templates/foreground.template
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/run/templates/qsub.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 09:30:44.111020 py-modelrunner-0.9.1/modelrunner/run/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/run/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 09:30:44.111020 py-modelrunner-0.9.1/modelrunner/run/tests/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      114 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/run/tests/scripts/function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      125 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/run/tests/scripts/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/run/tests/test_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 09:30:44.111020 py-modelrunner-0.9.1/modelrunner/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 09:30:44.111020 py-modelrunner-0.9.1/modelrunner/tests/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/tests/scripts/empty.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/tests/scripts/function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      180 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/tests/scripts/function_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      223 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/tests/scripts/function_marked.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/tests/scripts/make_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/tests/scripts/make_model_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/tests/scripts/make_model_marked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/modelrunner/tests/test_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 09:30:44.111020 py-modelrunner-0.9.1/py_modelrunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2022-11-30 09:30:44.000000 py-modelrunner-0.9.1/py_modelrunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2022-11-30 09:30:44.000000 py-modelrunner-0.9.1/py_modelrunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-30 09:30:44.000000 py-modelrunner-0.9.1/py_modelrunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-30 09:30:43.000000 py-modelrunner-0.9.1/py_modelrunner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2022-11-30 09:30:44.000000 py-modelrunner-0.9.1/py_modelrunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2022-11-30 09:30:44.000000 py-modelrunner-0.9.1/py_modelrunner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-11-30 09:30:44.115020 py-modelrunner-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 09:30:44.115020 py-modelrunner-0.9.1/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/tests/format_code.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/tests/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5942 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/tests/run_tests.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      197 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/tests/tests_all.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      123 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/tests/tests_codestyle.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      114 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/tests/tests_coverage.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      277 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/tests/tests_parallel.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      255 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/tests/tests_run.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       43 2022-11-30 09:30:01.000000 py-modelrunner-0.9.1/tests/tests_types.sh
```

### Comparing `py-modelrunner-0.8/LICENSE` & `py-modelrunner-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-modelrunner-0.8/PKG-INFO` & `py-modelrunner-0.9.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,296 +1,296 @@
 Metadata-Version: 2.1
 Name: py-modelrunner
-Version: 0.8
+Version: 0.9.1
 Summary: Python classes for organizing (HPC) simulations
-Home-page: https://github.com/zwicker-group/py-modelrunner
-Author: David Zwicker
-Author-email: david.zwicker@ds.mpg.de
+Author-email: David Zwicker <david.zwicker@ds.mpg.de>
 License: MIT
-Download-URL: https://github.com/zwicker-group/py-modelrunner/archive/v0.8.tar.gz
-Description: # py-modelrunner
-        
-        
-        [![Build status](https://github.com/zwicker-group/py-modelrunner/workflows/build/badge.svg)](https://github.com/zwicker-group/py-modelrunner/actions?query=workflow%3Abuild)
-        [![Documentation Status](https://readthedocs.org/projects/py-modelrunner/badge/?version=latest)](https://py-modelrunner.readthedocs.io/en/latest/?badge=latest)
-        [![PyPI version](https://badge.fury.io/py/py-modelrunner.svg)](https://badge.fury.io/py/py-modelrunner)
-        [![Conda Version](https://img.shields.io/conda/vn/conda-forge/py-modelrunner.svg)](https://anaconda.org/conda-forge/py-modelrunner)
-        
-        [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
-        [![codecov](https://codecov.io/gh/zwicker-group/py-modelrunner/branch/main/graph/badge.svg)](https://codecov.io/gh/zwicker-group/py-modelrunner)
-        [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/zwicker-group/py-modelrunner.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/zwicker-group/py-modelrunner/context:python)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        
-        
-        
-        This package provides python classes for handling and running physical simulations.
-        The main aim is to easily wrap simulation code and deal with input and output automatically.
-        The package also facilitates submitting simulations to high performance computing
-        environments and it provides functions for running parameter scans.
-        
-        
-        Installation
-        ============
-        The package can simply be cloned from github, but it is also available on `pip` and `conda`:
-        
-        ```bash
-        pip install py-modelrunner
-        ```
-        
-        Usage
-        =====
-        
-        This package has multiple purposes that are described in more detail below. Additional
-        examples can be found in the `examples` folder.
-        
-        Minimal example
-        ---------------
-        Assume you have written a python simulation in form of a simple script that defines a
-        function with several arguments, like so
-        
-        ```python
-        def main(a: float = 1, b: int = 2, negate: bool = False):
-            res = a ** b
-            if negate:
-            	res *= -1
-            return res
-        ```
-        
-        The `modelrunner` package now allows you to wrap a convenient command line interface
-        around this simple function. Assuming the script is saved in a file called `script.py`,
-        calling `python -m modelrunner script.py -h` shows the follwing help
-        
-        ```
-        usage: test.py [-h] [--a VALUE] [--b VALUE] [--negate] [--json JSON] [-o PATH]
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --json JSON           JSON-encoded parameter values. Overwrites other parameters. (default: None)
-          -o PATH, --output PATH
-                                Path to output file. If omitted, no output file is created. (default: None)
-        
-          --a VALUE             Parameter `a` (default: 1)
-          --b VALUE             Parameter `b` (default: 2)
-          --negate              Parameter `negate` (default: False)
-        ```
-        
-        Consequently, the function can be called using `python -m modelrunner script.py --a 2 --b 3 --negate -o result.yaml`,
-        which produces a file `result.yaml` with the following content:
-        
-        ```yaml
-        info:
-          time: # TIMESTAMP
-        model:
-          class: main
-          description: null
-          name: main
-          parameters:
-            a: 2.0
-            b: 3
-            negate: true
-        result: -8.0
-        ```
-        
-        This file not only contains the result, but also metainformation including the
-        parameters to run the simulation and the time when it was started.
-        
-        
-        Creating models
-        ---------------
-        The package introduces a base class `ModelBase` that describes the bare structure all
-        models are supposed to have.
-        Custom models can be created by inheriting from `ModelBase` and defining suitable
-        parameters:
-        
-        ```python
-        from modelrunner import ModelBase
-        
-        class MyModel(ModelBase):  # define custom model
-        
-            # defines supported parameters with default values
-            parameters_default = {"a": 1, "b": 2}
-        
-            def __call__(self):
-                """calculate the actual model"""
-                return self.parameters["a"] * self.parameters["b"]
-        
-        
-        model = MyModel({"a" : 3})
-        ```
-        
-        The last line actually creates an instance of the model with custom parameters.
-        
-        Alternatively, a model can also be defined from a simple function:
-        
-        ```python
-        from modelrunner import make_model
-        
-        @make_model
-        def multiply(a=1, b=2):
-            return a * b
-        
-        model = multiply(a=3)
-        ```
-        
-        The main aim of defining models like this is to provide a unified interface for
-        running models for the subsequent sections.
-        
-        
-        Run models from command line
-        ----------------------------
-        
-        Models can be run with different parameters. In both examples shown above, the model
-        can be run from within the python code by simply calling the model instance: `model()`.
-        In the cases shown above, these calls will simply return `6`.
-        
-        In typical numerical simulations, models need to be evaluated for many different
-        parameters. The packages facilitates this by providing a special interface to set
-        arguments from the command line. To show this, either one of the model definitions
-        given above can be saved as a python file `model.py`. Using the special call
-        `python -m modelrunner model.py` provides a command line interface for adjusting model parameters.
-        The supported parameters can be obtained with the following command
-        
-        ```console
-        $ python -m modelrunner model.py --help
-        
-        usage: model.py [-h] [--a VALUE] [--b VALUE] [-o PATH] [--json JSON]
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -o PATH, --output PATH
-                                Path to output file. If omitted, no output file is created. (default: None)
-          --json JSON           JSON-encoded parameter values. Overwrites other parameters. (default: None)
-        
-          --a VALUE             Parameter `a` (default: 1)
-          --b VALUE             Parameter `b` (default: 2)
-        ```
-        
-        This can be helpful to call a model automatically and save the result. For instance, by
-        calling `python -m modelrunner model.py -h --a 3 -o result.yaml`, we obtain a file `result.yaml` that
-        looks something like this:
-        
-        ```yaml
-        model:
-          class: multiply
-          name: multiply
-          parameters:
-            a: 3
-            b: 2
-        result: 6
-        ```
-        
-        Other supported output formats include JSON (extension `.json`) and HDF (extension `.hdf`).
-        
-        
-        Submit models to an HPC queue
-        -----------------------------
-        The package also provides methods to submit scripts to an high performance compute (HPC)
-        system. 
-        A simple full script displaying this reads
-        
-        ```python
-        from modelrunner import make_model, submit_job
-        
-        @make_model
-        def multiply(a=1, b=2):
-            return a * b
-        
-        if __name__ == "__main__":
-            submit_job(__file__, parameters={'a': 2}, output="data.hdf5", method="local")
-        ```
-        Here, the `output` argument specifies a file to which the results are written, while
-        `method` chooses how the script is submitted.
-        
-        In particular, this method allows submitting the same script with multiple different
-        parameters to conduct a parameter study:
-        
-        ```python
-        from modelrunner import make_model, submit_job
-        
-        @make_model
-        def multiply(a=1, b=2):
-            return a * b
-        
-        if __name__ == "__main__":
-            for a in range(5):
-                submit_job(__file__, parameters={'a': a}, output=f"data_{a}.hdf5", method="local")
-        ```
-        
-        Note that the safe-guard `if __name__ == "__main__"` is absolutely crucial to ensure that
-        jobs are only submitted during the initial run and not when the file is imported again
-        when the actual jobs start. It is also important to choose unique file names for the
-        `output` flag since otherwise different jobs overwrite each others data.
-        
-        We also support submitting multiple jobs of a parameter study:
-        
-        ```python
-        from modelrunner import make_model, submit_jobs
-        
-        @make_model
-        def multiply(a=1, b=2):
-            return a * b
-        
-        if __name__ == "__main__":
-            submit_jobs(__file__, parameters={'a': range(5)}, output_folder="data", method="local")
-        ```
-        
-        Finally, the packages also offers a method to submit a model script to the cluster using
-        a simple command: `python3 -m modelrunner.run script.py`. This command also offers multiple options
-        that can be adjusted using command line arguments:
-        
-        ```
-        usage: python -m modelrunner.run [-h] [-n NAME] [-p JSON] [-o PATH] [-f] [-m METHOD] [-t PATH] script
-        
-        Run a script as a job
-        
-        positional arguments:
-          script                The script that should be run
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -n NAME, --name NAME  Name of job
-          -p JSON, --parameters JSON
-                                JSON-encoded dictionary of parameters for the model
-          -o PATH, --output PATH
-                                Path to output file
-          -f, --force           Overwrite data if it already exists
-          -m METHOD, --method METHOD
-                                Method for job submission
-          -t PATH, --template PATH
-                                Path to template file for submission script
-        ```
-        
-        Collating results
-        -----------------
-        Finally, the package also provides some rudimentary support for collection results from
-        many different simulations that have been run in parallel. In particular, the class
-        `ResultCollection` provides a class method `from_folder` to scan a folder for result files.
-        For instance, the data from the multiple jobs ran above can be collected using
-        
-        ```python
-        from modelrunner import ResultCollection
-        
-        results = ResultCollection.from_folder(".", pattern="data_*.hdf5")
-        print(results.dataframe)
-        ```
-        
-        This example should print all results using a pandas Dataframe, where each row
-        corresponds to a separate simulation.
-        
-        
-        Development
-        ===========
-        The package is in an early phase and breaking changes are thus likely.
-        
-Platform: UNKNOWN
+Project-URL: homepage, https://github.com/zwicker-group/py-modelrunner
+Project-URL: documentation, http://py-modelrunner.readthedocs.io
+Project-URL: repository, https://github.com/zwicker-group/py-modelrunner
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# py-modelrunner
+
+
+[![Build status](https://github.com/zwicker-group/py-modelrunner/workflows/build/badge.svg)](https://github.com/zwicker-group/py-modelrunner/actions?query=workflow%3Abuild)
+[![Documentation Status](https://readthedocs.org/projects/py-modelrunner/badge/?version=latest)](https://py-modelrunner.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/py-modelrunner.svg)](https://badge.fury.io/py/py-modelrunner)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/py-modelrunner.svg)](https://anaconda.org/conda-forge/py-modelrunner)
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
+[![codecov](https://codecov.io/gh/zwicker-group/py-modelrunner/branch/main/graph/badge.svg)](https://codecov.io/gh/zwicker-group/py-modelrunner)
+[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/zwicker-group/py-modelrunner.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/zwicker-group/py-modelrunner/context:python)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+
+
+This package provides python classes for handling and running physical simulations.
+The main aim is to easily wrap simulation code and deal with input and output automatically.
+The package also facilitates submitting simulations to high performance computing
+environments and it provides functions for running parameter scans.
+
+
+Installation
+============
+The package can simply be cloned from github, but it is also available on `pip` and `conda`:
+
+```bash
+pip install py-modelrunner
+```
+
+Usage
+=====
+
+This package has multiple purposes that are described in more detail below. Additional
+examples can be found in the `examples` folder.
+
+Minimal example
+---------------
+Assume you have written a python simulation in form of a simple script that defines a
+function with several arguments, like so
+
+```python
+def main(a: float = 1, b: int = 2, negate: bool = False):
+    res = a ** b
+    if negate:
+    	res *= -1
+    return res
+```
+
+The `modelrunner` package now allows you to wrap a convenient command line interface
+around this simple function. Assuming the script is saved in a file called `script.py`,
+calling `python -m modelrunner script.py -h` shows the follwing help
+
+```
+usage: test.py [-h] [--a VALUE] [--b VALUE] [--negate] [--json JSON] [-o PATH]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --json JSON           JSON-encoded parameter values. Overwrites other parameters. (default: None)
+  -o PATH, --output PATH
+                        Path to output file. If omitted, no output file is created. (default: None)
+
+  --a VALUE             Parameter `a` (default: 1)
+  --b VALUE             Parameter `b` (default: 2)
+  --negate              Parameter `negate` (default: False)
+```
+
+Consequently, the function can be called using `python -m modelrunner script.py --a 2 --b 3 --negate -o result.yaml`,
+which produces a file `result.yaml` with the following content:
+
+```yaml
+info:
+  time: # TIMESTAMP
+model:
+  class: main
+  description: null
+  name: main
+  parameters:
+    a: 2.0
+    b: 3
+    negate: true
+result: -8.0
+```
+
+This file not only contains the result, but also metainformation including the
+parameters to run the simulation and the time when it was started.
+
+
+Creating models
+---------------
+The package introduces a base class `ModelBase` that describes the bare structure all
+models are supposed to have.
+Custom models can be created by inheriting from `ModelBase` and defining suitable
+parameters:
+
+```python
+from modelrunner import ModelBase
+
+class MyModel(ModelBase):  # define custom model
+
+    # defines supported parameters with default values
+    parameters_default = {"a": 1, "b": 2}
+
+    def __call__(self):
+        """calculate the actual model"""
+        return self.parameters["a"] * self.parameters["b"]
+
+
+model = MyModel({"a" : 3})
+```
+
+The last line actually creates an instance of the model with custom parameters.
+
+Alternatively, a model can also be defined from a simple function:
+
+```python
+from modelrunner import make_model
+
+@make_model
+def multiply(a=1, b=2):
+    return a * b
+
+model = multiply(a=3)
+```
+
+The main aim of defining models like this is to provide a unified interface for
+running models for the subsequent sections.
+
+
+Run models from command line
+----------------------------
+
+Models can be run with different parameters. In both examples shown above, the model
+can be run from within the python code by simply calling the model instance: `model()`.
+In the cases shown above, these calls will simply return `6`.
+
+In typical numerical simulations, models need to be evaluated for many different
+parameters. The packages facilitates this by providing a special interface to set
+arguments from the command line. To show this, either one of the model definitions
+given above can be saved as a python file `model.py`. Using the special call
+`python -m modelrunner model.py` provides a command line interface for adjusting model parameters.
+The supported parameters can be obtained with the following command
+
+```console
+$ python -m modelrunner model.py --help
+
+usage: model.py [-h] [--a VALUE] [--b VALUE] [-o PATH] [--json JSON]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -o PATH, --output PATH
+                        Path to output file. If omitted, no output file is created. (default: None)
+  --json JSON           JSON-encoded parameter values. Overwrites other parameters. (default: None)
+
+  --a VALUE             Parameter `a` (default: 1)
+  --b VALUE             Parameter `b` (default: 2)
+```
+
+This can be helpful to call a model automatically and save the result. For instance, by
+calling `python -m modelrunner model.py -h --a 3 -o result.yaml`, we obtain a file `result.yaml` that
+looks something like this:
+
+```yaml
+model:
+  class: multiply
+  name: multiply
+  parameters:
+    a: 3
+    b: 2
+result: 6
+```
+
+Other supported output formats include JSON (extension `.json`) and HDF (extension `.hdf`).
+
+
+Submit models to an HPC queue
+-----------------------------
+The package also provides methods to submit scripts to an high performance compute (HPC)
+system. 
+A simple full script displaying this reads
+
+```python
+from modelrunner import make_model, submit_job
+
+@make_model
+def multiply(a=1, b=2):
+    return a * b
+
+if __name__ == "__main__":
+    submit_job(__file__, parameters={'a': 2}, output="data.hdf5", method="local")
+```
+Here, the `output` argument specifies a file to which the results are written, while
+`method` chooses how the script is submitted.
+
+In particular, this method allows submitting the same script with multiple different
+parameters to conduct a parameter study:
+
+```python
+from modelrunner import make_model, submit_job
+
+@make_model
+def multiply(a=1, b=2):
+    return a * b
+
+if __name__ == "__main__":
+    for a in range(5):
+        submit_job(__file__, parameters={'a': a}, output=f"data_{a}.hdf5", method="local")
+```
+
+Note that the safe-guard `if __name__ == "__main__"` is absolutely crucial to ensure that
+jobs are only submitted during the initial run and not when the file is imported again
+when the actual jobs start. It is also important to choose unique file names for the
+`output` flag since otherwise different jobs overwrite each others data.
+
+We also support submitting multiple jobs of a parameter study:
+
+```python
+from modelrunner import make_model, submit_jobs
+
+@make_model
+def multiply(a=1, b=2):
+    return a * b
+
+if __name__ == "__main__":
+    submit_jobs(__file__, parameters={'a': range(5)}, output_folder="data", method="local")
+```
+
+Finally, the packages also offers a method to submit a model script to the cluster using
+a simple command: `python3 -m modelrunner.run script.py`. This command also offers multiple options
+that can be adjusted using command line arguments:
+
+```
+usage: python -m modelrunner.run [-h] [-n NAME] [-p JSON] [-o PATH] [-f] [-m METHOD] [-t PATH] script
+
+Run a script as a job
+
+positional arguments:
+  script                The script that should be run
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -n NAME, --name NAME  Name of job
+  -p JSON, --parameters JSON
+                        JSON-encoded dictionary of parameters for the model
+  -o PATH, --output PATH
+                        Path to output file
+  -f, --force           Overwrite data if it already exists
+  -m METHOD, --method METHOD
+                        Method for job submission
+  -t PATH, --template PATH
+                        Path to template file for submission script
+```
+
+Collating results
+-----------------
+Finally, the package also provides some rudimentary support for collection results from
+many different simulations that have been run in parallel. In particular, the class
+`ResultCollection` provides a class method `from_folder` to scan a folder for result files.
+For instance, the data from the multiple jobs ran above can be collected using
+
+```python
+from modelrunner import ResultCollection
+
+results = ResultCollection.from_folder(".", pattern="data_*.hdf5")
+print(results.dataframe)
+```
+
+This example should print all results using a pandas Dataframe, where each row
+corresponds to a separate simulation.
+
+
+Development
+===========
+The package is in an early phase and breaking changes are thus likely.
```

### Comparing `py-modelrunner-0.8/README.md` & `py-modelrunner-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `py-modelrunner-0.8/modelrunner/model.py` & `py-modelrunner-0.9.1/modelrunner/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,44 +51,50 @@
         self._logger = logging.getLogger(self.__class__.__name__)
 
     @abstractmethod
     def __call__(self):
         """main method calculating the result"""
         pass
 
-    def get_result(self, result=None) -> "Result":
+    def get_result(self, result_data=None) -> "Result":
         """get the result as a :class:`~model.Result` object
 
         Args:
-            result: The result data. If omitted, the model is ran to obtain results
+            result_data:
+                The result data. If omitted, the model is run to obtain results
+
+        Returns:
+            :class:`Result`: The result after the model is run
         """
         from .results import Result  # @Reimport
 
-        if result is None:
-            result = self()
+        if result_data is None:
+            result_data = self()
+        elif isinstance(result_data, Result):
+            return result_data
 
         info = {"time": datetime.now().strftime("%Y-%m-%d %H:%M:%S")}
-        return Result(self, result, info=info)
+        return Result(self, result_data, info=info)
 
-    def write_result(self, output: Optional[str] = None, result=None) -> None:
+    def write_result(self, output: Optional[str] = None, result_data=None) -> None:
         """write the result to the output file
 
         Args:
             output (str):
                 File where the output will be written to. If omitted self.output will be
                 used. If self.output is also None, an error will be thrown.
-            result:
-                The result data. If omitted, the model is ran to obtain results
+            result_data:
+                The result data. If omitted, the model is run to obtain results
         """
         if output is None:
             output = self.output
         if output is None:
             raise RuntimeError("output file needs to be specified")
 
-        result = self.get_result(result)
+        result = self.get_result(result_data)
         result.write_to_file(output)
 
     @classmethod
     def _prepare_argparser(cls, name: Optional[str] = None) -> argparse.ArgumentParser:
         """create argument parser for setting parameters of this model
 
         Args:
@@ -132,14 +138,17 @@
         """create model from command line parameters
 
         Args:
             args (list):
                 Sequence of strings corresponding to the command line arguments
             name (str):
                 Name of the program, which will be shown in the command line help
+
+        Returns:
+            :class:`ModelBase`: An instance of this model with appropriate parameters
         """
         if args is None:
             args = []
 
         # read the command line arguments
         parser = cls._prepare_argparser(name)
 
@@ -169,39 +178,75 @@
         """run model using command line parameters
 
         Args:
             args (list):
                 Sequence of strings corresponding to the command line arguments
             name (str):
                 Name of the program, which will be shown in the command line help
+
+        Returns:
+            :class:`Result`: The result of running the model
         """
         # create model from command line parameters
         mdl = cls.from_command_line(args, name)
         # run the model
         result = mdl.get_result()
 
         # write the results (if output file was specified)
         if mdl.output:
-            mdl.write_result(output=None, result=result)
+            mdl.write_result(output=None, result_data=result)
 
         return result
 
     @property
     def attributes(self) -> Dict[str, Any]:
         """dict: information about the element state, which does not change in time"""
         return {
             "class": self.__class__.__name__,
             "name": self.name,
             "description": self.description,
             "parameters": self.parameters,
         }
 
 
-def make_model_class(func: Callable) -> Type[ModelBase]:
-    """create a model from a function by interpreting its signature"""
+_DEFAULT_MODEL: Union[Callable, ModelBase, None] = None
+"""stores the default model that will be used automatically"""
+
+
+def set_default(func_or_model: Union[Callable, ModelBase, None]) -> None:
+    """sets the function or model as the default model
+
+    The last model that received this flag will be run automatically. This only affects
+    the behavior when the script is run using `modelrunner` from the command line, e.g.,
+    using :code:`python -m modelrunner script.py`.
+
+    Args:
+        func_or_model (callabel or :class:`ModelBase`, optional):
+            The function or model that should be called when the script is run.
+
+    Returns:
+        `func_or_model`, so the function can be used as a decorator
+    """
+    global _DEFAULT_MODEL
+    _DEFAULT_MODEL = func_or_model
+    return func_or_model
+
+
+def make_model_class(func: Callable, *, default: bool = False) -> Type[ModelBase]:
+    """create a model from a function by interpreting its signature
+
+    Args:
+        func (callable):
+            The function that will be turned into a Model
+        default (bool):
+            If True, set this model as the default one for the current script
+
+    Returns:
+        :class:`ModelBase`: A subclass of ModelBase, which encompasses `func`
+    """
     # determine the parameters of the function
     parameters_default = []
     for name, param in inspect.signature(func).parameters.items():
         if param.annotation is param.empty:
             cls = object
         else:
             cls = param.annotation
@@ -228,58 +273,80 @@
     args = {
         "name": func.__name__,
         "description": func.__doc__,
         "parameters_default": parameters_default,
         "__call__": __call__,
     }
     newclass = type(func.__name__, (ModelBase,), args)
+    if default:
+        set_default(newclass)
     return newclass
 
 
 def make_model(
-    func: Callable, parameters: Optional[Dict[str, Any]] = None
+    func: Callable,
+    parameters: Optional[Dict[str, Any]] = None,
+    *,
+    default: bool = False,
 ) -> ModelBase:
-    """create model from a function and a dictionary of parameters"""
-    model_class = make_model_class(func)
-    return model_class(parameters)
+    """create model from a function and a dictionary of parameters
 
+    Args:
+        func (callable):
+            The function that will be turned into a Model
+        parameters (dict):
+            Paramter values with which the model is initialized
+        default (bool):
+            If True, set this model as the default one for the current script
 
-_DEFAULT_MODEL: Union[Callable, ModelBase, None] = None
-"""stores the default model that will be used automatically"""
-
+    Returns:
+        :class:`ModelBase`: An instance of a subclass of ModelBase encompassing `func`
+    """
+    model_class = make_model_class(func, default=default)
+    return model_class(parameters)
 
-def set_default(func_or_model: Union[Callable, ModelBase, None]):
-    """sets the function or model as the default model
 
-    The last model that received this flag will be run automatically. This only affects
-    the behavior when the script is run using `modelrunner` from the command line, e.g.,
-    using :code:`python -m modelrunner script.py`.
+def run_function_with_cmd_args(
+    func: Callable, args: Optional[Sequence[str]] = None, *, name: Optional[str] = None
+) -> "Result":
+    """create model from a function and obtain parameters from command line
 
     Args:
-        func_or_model (callabel or :class:`ModelBase`, optional):
-            The function or model that should be called when the script is run.
-    """
-    global _DEFAULT_MODEL
-    _DEFAULT_MODEL = func_or_model
+        func (callable):
+            The function that will be turned into a Model
+        args (list of str):
+            Command line arguments, typically :code:`sys.argv[1:]`
+        name (str):
+            Name of the program, which will be shown in the command line help
 
+    Returns:
+        :class:`ModelBase`: An instance of a subclass of ModelBase encompassing `func`
 
-def run_function_with_cmd_args(
-    func: Callable, args: Optional[Sequence[str]] = None, name: Optional[str] = None
-) -> "Result":
-    """create model from a function and obtain parameters from command line"""
+    """
     return make_model_class(func).run_from_command_line(args, name=name)
 
 
 def run_script(script_path: str, model_args: Sequence[str]) -> "Result":
     """helper function that runs a model script
+
+    The function detects models automatically by trying several methods until one yields
+    a unique model to run:
+
+    * A model that have been marked as default by :func:`set_default`
+    * A function named `main`
+    * A model instance if there is exactly one (throw error if there are many)
+    * A model class if there is exactly one (throw error if there are many)
+    * A function if there is exactly one (throw error if there are many)
+
     Args:
         script_path (str):
             Path to the script that contains the model definition
         model_args (sequence):
             Additional arugments that define how the model is run
+
     Returns:
         :class:`~modelrunner.result.Result`: The result of the run
     """
     global _DEFAULT_MODEL
     logger = logging.getLogger("modelrunner")
 
     # load the script as a module
@@ -338,22 +405,18 @@
         return cls.run_from_command_line(model_args, name=filename)
 
     elif len(candidate_classes) > 1:
         # there are multiple instance => we do not know which one do use
         names = ", ".join(sorted(candidate_classes.keys()))
         raise RuntimeError(f"Found multiple model classes: {names}")
 
-    elif len(candidate_funcs) == 1 or "main" in candidate_funcs:
+    elif len(candidate_funcs) == 1:
         # there is a single function of a model => use this
-        if "main" in candidate_funcs:
-            func = candidate_funcs["main"]
-            logger.info("Run model function named `main`")
-        else:
-            _, func = candidate_funcs.popitem()
-            logger.info("Run model function named `%s`", func.__name__)
+        _, func = candidate_funcs.popitem()
+        logger.info("Run model function named `%s`", func.__name__)
         return run_function_with_cmd_args(func, args=model_args, name=filename)
 
     elif len(candidate_funcs) > 1:
         # there are multiple functions and we do not know which one to run
         names = ", ".join(sorted(candidate_funcs.keys()))
         raise RuntimeError(f"Found many function, but no 'main' function: {names}")
```

### Comparing `py-modelrunner-0.8/modelrunner/parameters.py` & `py-modelrunner-0.9.1/modelrunner/parameters.py`

 * *Files identical despite different names*

### Comparing `py-modelrunner-0.8/modelrunner/results.py` & `py-modelrunner-0.9.1/modelrunner/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,56 +136,61 @@
     def __repr__(self):
         return f"{self.__class__.__name__}({self.parameters})"
 
 
 class Result:
     """describes a model (with parameters) together with its result"""
 
-    def __init__(self, model: ModelBase, result, info: Optional[Dict[str, Any]] = None):
+    def __init__(
+        self, model: ModelBase, result_data, info: Optional[Dict[str, Any]] = None
+    ):
         """
         Args:
             model (:class:`ModelBase`): The model from which the result was obtained
-            result: The actual result
+            result_data: The actual result data
             info (dict): Additional information for this result
         """
         self.model = model
         self.info = info
-        if isinstance(result, Result):
-            self.result: Any = result.result
+        if isinstance(result_data, Result):
+            self.result: Any = result_data.result
         else:
-            self.result = result
+            self.result = result_data
 
     @classmethod
     def from_data(
         cls,
         model_data: Dict[str, Any],
-        result,
+        result_data,
         model: Optional[ModelBase] = None,
         info: Optional[Dict[str, Any]] = None,
     ) -> Result:
         """create result from data
 
         Args:
             model_data (dict): The data identifying the model
-            result: The actual result
+            result_data: The actual result data
             model (:class:`ModelBase`): The model from which the result was obtained
             info (dict): Additional information for this result
+
+        Returns:
+            :class:`Result`: The result object
         """
         if model is None:
             model_cls: Type[ModelBase] = MockModel
         else:
             model_cls = model if inspect.isclass(model) else model.__class__
 
         if not model_data:
             warnings.warn("Model data not found")
         obj = model_cls(model_data.get("parameters", {}))
         obj.name = model_data.get("name")
         obj.description = model_data.get("description")
 
-        return cls(obj, result, info)
+        return cls(obj, result_data, info)
 
     @property
     def parameters(self) -> Dict[str, Any]:
         return self.model.parameters
 
     @classmethod
     def from_file(cls, path, model: Optional[ModelBase] = None):
@@ -233,15 +238,15 @@
             data = json.load(fp)
 
         info = data.get("info", {})
         info.setdefault("name", Path(path).with_suffix("").stem)
 
         return cls.from_data(
             model_data=data.get("model", {}),
-            result=data.get("result"),
+            result_data=data.get("result"),
             model=model,
             info=info,
         )
 
     def write_to_json(self, path) -> None:
         """write result to JSON file
 
@@ -272,15 +277,15 @@
             data = yaml.safe_load(fp)
 
         info = data.get("info", {})
         info.setdefault("name", Path(path).with_suffix("").stem)
 
         return cls.from_data(
             model_data=data.get("model", {}),
-            result=data.get("result"),
+            result_data=data.get("result"),
             model=model,
             info=info,
         )
 
     def write_to_yaml(self, path) -> None:
         """write result to YAML file
 
@@ -318,15 +323,15 @@
                 result = model_data.pop("result")
             # check for other nodes, which might not be read
 
         info = model_data.pop("__info__") if "__info__" in model_data else {}
         info.setdefault("name", Path(path).with_suffix("").stem)
 
         return cls.from_data(
-            model_data=model_data, result=result, model=model, info=info
+            model_data=model_data, result_data=result, model=model, info=info
         )
 
     def write_to_hdf(self, path) -> None:
         """write result to HDF file
 
         Args:
             path (str or :class:`~pathlib.Path`): The path to the file
```

### Comparing `py-modelrunner-0.8/modelrunner/run/__main__.py` & `py-modelrunner-0.9.1/modelrunner/run/__main__.py`

 * *Files identical despite different names*

### Comparing `py-modelrunner-0.8/modelrunner/run/job.py` & `py-modelrunner-0.9.1/modelrunner/run/job.py`

 * *Files identical despite different names*

### Comparing `py-modelrunner-0.8/modelrunner/run/templates/background.template` & `py-modelrunner-0.9.1/modelrunner/run/templates/background.template`

 * *Files identical despite different names*

### Comparing `py-modelrunner-0.8/modelrunner/run/templates/qsub.template` & `py-modelrunner-0.9.1/modelrunner/run/templates/qsub.template`

 * *Files identical despite different names*

### Comparing `py-modelrunner-0.8/modelrunner/run/tests/test_job.py` & `py-modelrunner-0.9.1/modelrunner/run/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `py-modelrunner-0.8/modelrunner/tests/test_examples.py` & `py-modelrunner-0.9.1/modelrunner/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `py-modelrunner-0.8/modelrunner/tests/test_main.py` & `py-modelrunner-0.9.1/modelrunner/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `py-modelrunner-0.8/modelrunner/tests/test_model.py` & `py-modelrunner-0.9.1/modelrunner/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `py-modelrunner-0.8/modelrunner/tests/test_parameters.py` & `py-modelrunner-0.9.1/modelrunner/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `py-modelrunner-0.8/modelrunner/tests/test_results.py` & `py-modelrunner-0.9.1/modelrunner/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `py-modelrunner-0.8/py_modelrunner.egg-info/PKG-INFO` & `py-modelrunner-0.9.1/py_modelrunner.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,296 +1,296 @@
 Metadata-Version: 2.1
 Name: py-modelrunner
-Version: 0.8
+Version: 0.9.1
 Summary: Python classes for organizing (HPC) simulations
-Home-page: https://github.com/zwicker-group/py-modelrunner
-Author: David Zwicker
-Author-email: david.zwicker@ds.mpg.de
+Author-email: David Zwicker <david.zwicker@ds.mpg.de>
 License: MIT
-Download-URL: https://github.com/zwicker-group/py-modelrunner/archive/v0.8.tar.gz
-Description: # py-modelrunner
-        
-        
-        [![Build status](https://github.com/zwicker-group/py-modelrunner/workflows/build/badge.svg)](https://github.com/zwicker-group/py-modelrunner/actions?query=workflow%3Abuild)
-        [![Documentation Status](https://readthedocs.org/projects/py-modelrunner/badge/?version=latest)](https://py-modelrunner.readthedocs.io/en/latest/?badge=latest)
-        [![PyPI version](https://badge.fury.io/py/py-modelrunner.svg)](https://badge.fury.io/py/py-modelrunner)
-        [![Conda Version](https://img.shields.io/conda/vn/conda-forge/py-modelrunner.svg)](https://anaconda.org/conda-forge/py-modelrunner)
-        
-        [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
-        [![codecov](https://codecov.io/gh/zwicker-group/py-modelrunner/branch/main/graph/badge.svg)](https://codecov.io/gh/zwicker-group/py-modelrunner)
-        [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/zwicker-group/py-modelrunner.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/zwicker-group/py-modelrunner/context:python)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        
-        
-        
-        This package provides python classes for handling and running physical simulations.
-        The main aim is to easily wrap simulation code and deal with input and output automatically.
-        The package also facilitates submitting simulations to high performance computing
-        environments and it provides functions for running parameter scans.
-        
-        
-        Installation
-        ============
-        The package can simply be cloned from github, but it is also available on `pip` and `conda`:
-        
-        ```bash
-        pip install py-modelrunner
-        ```
-        
-        Usage
-        =====
-        
-        This package has multiple purposes that are described in more detail below. Additional
-        examples can be found in the `examples` folder.
-        
-        Minimal example
-        ---------------
-        Assume you have written a python simulation in form of a simple script that defines a
-        function with several arguments, like so
-        
-        ```python
-        def main(a: float = 1, b: int = 2, negate: bool = False):
-            res = a ** b
-            if negate:
-            	res *= -1
-            return res
-        ```
-        
-        The `modelrunner` package now allows you to wrap a convenient command line interface
-        around this simple function. Assuming the script is saved in a file called `script.py`,
-        calling `python -m modelrunner script.py -h` shows the follwing help
-        
-        ```
-        usage: test.py [-h] [--a VALUE] [--b VALUE] [--negate] [--json JSON] [-o PATH]
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --json JSON           JSON-encoded parameter values. Overwrites other parameters. (default: None)
-          -o PATH, --output PATH
-                                Path to output file. If omitted, no output file is created. (default: None)
-        
-          --a VALUE             Parameter `a` (default: 1)
-          --b VALUE             Parameter `b` (default: 2)
-          --negate              Parameter `negate` (default: False)
-        ```
-        
-        Consequently, the function can be called using `python -m modelrunner script.py --a 2 --b 3 --negate -o result.yaml`,
-        which produces a file `result.yaml` with the following content:
-        
-        ```yaml
-        info:
-          time: # TIMESTAMP
-        model:
-          class: main
-          description: null
-          name: main
-          parameters:
-            a: 2.0
-            b: 3
-            negate: true
-        result: -8.0
-        ```
-        
-        This file not only contains the result, but also metainformation including the
-        parameters to run the simulation and the time when it was started.
-        
-        
-        Creating models
-        ---------------
-        The package introduces a base class `ModelBase` that describes the bare structure all
-        models are supposed to have.
-        Custom models can be created by inheriting from `ModelBase` and defining suitable
-        parameters:
-        
-        ```python
-        from modelrunner import ModelBase
-        
-        class MyModel(ModelBase):  # define custom model
-        
-            # defines supported parameters with default values
-            parameters_default = {"a": 1, "b": 2}
-        
-            def __call__(self):
-                """calculate the actual model"""
-                return self.parameters["a"] * self.parameters["b"]
-        
-        
-        model = MyModel({"a" : 3})
-        ```
-        
-        The last line actually creates an instance of the model with custom parameters.
-        
-        Alternatively, a model can also be defined from a simple function:
-        
-        ```python
-        from modelrunner import make_model
-        
-        @make_model
-        def multiply(a=1, b=2):
-            return a * b
-        
-        model = multiply(a=3)
-        ```
-        
-        The main aim of defining models like this is to provide a unified interface for
-        running models for the subsequent sections.
-        
-        
-        Run models from command line
-        ----------------------------
-        
-        Models can be run with different parameters. In both examples shown above, the model
-        can be run from within the python code by simply calling the model instance: `model()`.
-        In the cases shown above, these calls will simply return `6`.
-        
-        In typical numerical simulations, models need to be evaluated for many different
-        parameters. The packages facilitates this by providing a special interface to set
-        arguments from the command line. To show this, either one of the model definitions
-        given above can be saved as a python file `model.py`. Using the special call
-        `python -m modelrunner model.py` provides a command line interface for adjusting model parameters.
-        The supported parameters can be obtained with the following command
-        
-        ```console
-        $ python -m modelrunner model.py --help
-        
-        usage: model.py [-h] [--a VALUE] [--b VALUE] [-o PATH] [--json JSON]
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -o PATH, --output PATH
-                                Path to output file. If omitted, no output file is created. (default: None)
-          --json JSON           JSON-encoded parameter values. Overwrites other parameters. (default: None)
-        
-          --a VALUE             Parameter `a` (default: 1)
-          --b VALUE             Parameter `b` (default: 2)
-        ```
-        
-        This can be helpful to call a model automatically and save the result. For instance, by
-        calling `python -m modelrunner model.py -h --a 3 -o result.yaml`, we obtain a file `result.yaml` that
-        looks something like this:
-        
-        ```yaml
-        model:
-          class: multiply
-          name: multiply
-          parameters:
-            a: 3
-            b: 2
-        result: 6
-        ```
-        
-        Other supported output formats include JSON (extension `.json`) and HDF (extension `.hdf`).
-        
-        
-        Submit models to an HPC queue
-        -----------------------------
-        The package also provides methods to submit scripts to an high performance compute (HPC)
-        system. 
-        A simple full script displaying this reads
-        
-        ```python
-        from modelrunner import make_model, submit_job
-        
-        @make_model
-        def multiply(a=1, b=2):
-            return a * b
-        
-        if __name__ == "__main__":
-            submit_job(__file__, parameters={'a': 2}, output="data.hdf5", method="local")
-        ```
-        Here, the `output` argument specifies a file to which the results are written, while
-        `method` chooses how the script is submitted.
-        
-        In particular, this method allows submitting the same script with multiple different
-        parameters to conduct a parameter study:
-        
-        ```python
-        from modelrunner import make_model, submit_job
-        
-        @make_model
-        def multiply(a=1, b=2):
-            return a * b
-        
-        if __name__ == "__main__":
-            for a in range(5):
-                submit_job(__file__, parameters={'a': a}, output=f"data_{a}.hdf5", method="local")
-        ```
-        
-        Note that the safe-guard `if __name__ == "__main__"` is absolutely crucial to ensure that
-        jobs are only submitted during the initial run and not when the file is imported again
-        when the actual jobs start. It is also important to choose unique file names for the
-        `output` flag since otherwise different jobs overwrite each others data.
-        
-        We also support submitting multiple jobs of a parameter study:
-        
-        ```python
-        from modelrunner import make_model, submit_jobs
-        
-        @make_model
-        def multiply(a=1, b=2):
-            return a * b
-        
-        if __name__ == "__main__":
-            submit_jobs(__file__, parameters={'a': range(5)}, output_folder="data", method="local")
-        ```
-        
-        Finally, the packages also offers a method to submit a model script to the cluster using
-        a simple command: `python3 -m modelrunner.run script.py`. This command also offers multiple options
-        that can be adjusted using command line arguments:
-        
-        ```
-        usage: python -m modelrunner.run [-h] [-n NAME] [-p JSON] [-o PATH] [-f] [-m METHOD] [-t PATH] script
-        
-        Run a script as a job
-        
-        positional arguments:
-          script                The script that should be run
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -n NAME, --name NAME  Name of job
-          -p JSON, --parameters JSON
-                                JSON-encoded dictionary of parameters for the model
-          -o PATH, --output PATH
-                                Path to output file
-          -f, --force           Overwrite data if it already exists
-          -m METHOD, --method METHOD
-                                Method for job submission
-          -t PATH, --template PATH
-                                Path to template file for submission script
-        ```
-        
-        Collating results
-        -----------------
-        Finally, the package also provides some rudimentary support for collection results from
-        many different simulations that have been run in parallel. In particular, the class
-        `ResultCollection` provides a class method `from_folder` to scan a folder for result files.
-        For instance, the data from the multiple jobs ran above can be collected using
-        
-        ```python
-        from modelrunner import ResultCollection
-        
-        results = ResultCollection.from_folder(".", pattern="data_*.hdf5")
-        print(results.dataframe)
-        ```
-        
-        This example should print all results using a pandas Dataframe, where each row
-        corresponds to a separate simulation.
-        
-        
-        Development
-        ===========
-        The package is in an early phase and breaking changes are thus likely.
-        
-Platform: UNKNOWN
+Project-URL: homepage, https://github.com/zwicker-group/py-modelrunner
+Project-URL: documentation, http://py-modelrunner.readthedocs.io
+Project-URL: repository, https://github.com/zwicker-group/py-modelrunner
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# py-modelrunner
+
+
+[![Build status](https://github.com/zwicker-group/py-modelrunner/workflows/build/badge.svg)](https://github.com/zwicker-group/py-modelrunner/actions?query=workflow%3Abuild)
+[![Documentation Status](https://readthedocs.org/projects/py-modelrunner/badge/?version=latest)](https://py-modelrunner.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/py-modelrunner.svg)](https://badge.fury.io/py/py-modelrunner)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/py-modelrunner.svg)](https://anaconda.org/conda-forge/py-modelrunner)
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
+[![codecov](https://codecov.io/gh/zwicker-group/py-modelrunner/branch/main/graph/badge.svg)](https://codecov.io/gh/zwicker-group/py-modelrunner)
+[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/zwicker-group/py-modelrunner.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/zwicker-group/py-modelrunner/context:python)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+
+
+This package provides python classes for handling and running physical simulations.
+The main aim is to easily wrap simulation code and deal with input and output automatically.
+The package also facilitates submitting simulations to high performance computing
+environments and it provides functions for running parameter scans.
+
+
+Installation
+============
+The package can simply be cloned from github, but it is also available on `pip` and `conda`:
+
+```bash
+pip install py-modelrunner
+```
+
+Usage
+=====
+
+This package has multiple purposes that are described in more detail below. Additional
+examples can be found in the `examples` folder.
+
+Minimal example
+---------------
+Assume you have written a python simulation in form of a simple script that defines a
+function with several arguments, like so
+
+```python
+def main(a: float = 1, b: int = 2, negate: bool = False):
+    res = a ** b
+    if negate:
+    	res *= -1
+    return res
+```
+
+The `modelrunner` package now allows you to wrap a convenient command line interface
+around this simple function. Assuming the script is saved in a file called `script.py`,
+calling `python -m modelrunner script.py -h` shows the follwing help
+
+```
+usage: test.py [-h] [--a VALUE] [--b VALUE] [--negate] [--json JSON] [-o PATH]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --json JSON           JSON-encoded parameter values. Overwrites other parameters. (default: None)
+  -o PATH, --output PATH
+                        Path to output file. If omitted, no output file is created. (default: None)
+
+  --a VALUE             Parameter `a` (default: 1)
+  --b VALUE             Parameter `b` (default: 2)
+  --negate              Parameter `negate` (default: False)
+```
+
+Consequently, the function can be called using `python -m modelrunner script.py --a 2 --b 3 --negate -o result.yaml`,
+which produces a file `result.yaml` with the following content:
+
+```yaml
+info:
+  time: # TIMESTAMP
+model:
+  class: main
+  description: null
+  name: main
+  parameters:
+    a: 2.0
+    b: 3
+    negate: true
+result: -8.0
+```
+
+This file not only contains the result, but also metainformation including the
+parameters to run the simulation and the time when it was started.
+
+
+Creating models
+---------------
+The package introduces a base class `ModelBase` that describes the bare structure all
+models are supposed to have.
+Custom models can be created by inheriting from `ModelBase` and defining suitable
+parameters:
+
+```python
+from modelrunner import ModelBase
+
+class MyModel(ModelBase):  # define custom model
+
+    # defines supported parameters with default values
+    parameters_default = {"a": 1, "b": 2}
+
+    def __call__(self):
+        """calculate the actual model"""
+        return self.parameters["a"] * self.parameters["b"]
+
+
+model = MyModel({"a" : 3})
+```
+
+The last line actually creates an instance of the model with custom parameters.
+
+Alternatively, a model can also be defined from a simple function:
+
+```python
+from modelrunner import make_model
+
+@make_model
+def multiply(a=1, b=2):
+    return a * b
+
+model = multiply(a=3)
+```
+
+The main aim of defining models like this is to provide a unified interface for
+running models for the subsequent sections.
+
+
+Run models from command line
+----------------------------
+
+Models can be run with different parameters. In both examples shown above, the model
+can be run from within the python code by simply calling the model instance: `model()`.
+In the cases shown above, these calls will simply return `6`.
+
+In typical numerical simulations, models need to be evaluated for many different
+parameters. The packages facilitates this by providing a special interface to set
+arguments from the command line. To show this, either one of the model definitions
+given above can be saved as a python file `model.py`. Using the special call
+`python -m modelrunner model.py` provides a command line interface for adjusting model parameters.
+The supported parameters can be obtained with the following command
+
+```console
+$ python -m modelrunner model.py --help
+
+usage: model.py [-h] [--a VALUE] [--b VALUE] [-o PATH] [--json JSON]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -o PATH, --output PATH
+                        Path to output file. If omitted, no output file is created. (default: None)
+  --json JSON           JSON-encoded parameter values. Overwrites other parameters. (default: None)
+
+  --a VALUE             Parameter `a` (default: 1)
+  --b VALUE             Parameter `b` (default: 2)
+```
+
+This can be helpful to call a model automatically and save the result. For instance, by
+calling `python -m modelrunner model.py -h --a 3 -o result.yaml`, we obtain a file `result.yaml` that
+looks something like this:
+
+```yaml
+model:
+  class: multiply
+  name: multiply
+  parameters:
+    a: 3
+    b: 2
+result: 6
+```
+
+Other supported output formats include JSON (extension `.json`) and HDF (extension `.hdf`).
+
+
+Submit models to an HPC queue
+-----------------------------
+The package also provides methods to submit scripts to an high performance compute (HPC)
+system. 
+A simple full script displaying this reads
+
+```python
+from modelrunner import make_model, submit_job
+
+@make_model
+def multiply(a=1, b=2):
+    return a * b
+
+if __name__ == "__main__":
+    submit_job(__file__, parameters={'a': 2}, output="data.hdf5", method="local")
+```
+Here, the `output` argument specifies a file to which the results are written, while
+`method` chooses how the script is submitted.
+
+In particular, this method allows submitting the same script with multiple different
+parameters to conduct a parameter study:
+
+```python
+from modelrunner import make_model, submit_job
+
+@make_model
+def multiply(a=1, b=2):
+    return a * b
+
+if __name__ == "__main__":
+    for a in range(5):
+        submit_job(__file__, parameters={'a': a}, output=f"data_{a}.hdf5", method="local")
+```
+
+Note that the safe-guard `if __name__ == "__main__"` is absolutely crucial to ensure that
+jobs are only submitted during the initial run and not when the file is imported again
+when the actual jobs start. It is also important to choose unique file names for the
+`output` flag since otherwise different jobs overwrite each others data.
+
+We also support submitting multiple jobs of a parameter study:
+
+```python
+from modelrunner import make_model, submit_jobs
+
+@make_model
+def multiply(a=1, b=2):
+    return a * b
+
+if __name__ == "__main__":
+    submit_jobs(__file__, parameters={'a': range(5)}, output_folder="data", method="local")
+```
+
+Finally, the packages also offers a method to submit a model script to the cluster using
+a simple command: `python3 -m modelrunner.run script.py`. This command also offers multiple options
+that can be adjusted using command line arguments:
+
+```
+usage: python -m modelrunner.run [-h] [-n NAME] [-p JSON] [-o PATH] [-f] [-m METHOD] [-t PATH] script
+
+Run a script as a job
+
+positional arguments:
+  script                The script that should be run
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -n NAME, --name NAME  Name of job
+  -p JSON, --parameters JSON
+                        JSON-encoded dictionary of parameters for the model
+  -o PATH, --output PATH
+                        Path to output file
+  -f, --force           Overwrite data if it already exists
+  -m METHOD, --method METHOD
+                        Method for job submission
+  -t PATH, --template PATH
+                        Path to template file for submission script
+```
+
+Collating results
+-----------------
+Finally, the package also provides some rudimentary support for collection results from
+many different simulations that have been run in parallel. In particular, the class
+`ResultCollection` provides a class method `from_folder` to scan a folder for result files.
+For instance, the data from the multiple jobs ran above can be collected using
+
+```python
+from modelrunner import ResultCollection
+
+results = ResultCollection.from_folder(".", pattern="data_*.hdf5")
+print(results.dataframe)
+```
+
+This example should print all results using a pandas Dataframe, where each row
+corresponds to a separate simulation.
+
+
+Development
+===========
+The package is in an early phase and breaking changes are thus likely.
```

