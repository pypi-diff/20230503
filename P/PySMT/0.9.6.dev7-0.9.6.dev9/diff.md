# Comparing `tmp/PySMT-0.9.6.dev7.tar.gz` & `tmp/PySMT-0.9.6.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySMT-0.9.6.dev7.tar", last modified: Sat May 28 20:26:54 2022, max compression
+gzip compressed data, was "PySMT-0.9.6.dev9.tar", last modified: Mon May 30 07:33:15 2022, max compression
```

## Comparing `PySMT-0.9.6.dev7.tar` & `PySMT-0.9.6.dev9.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 20:26:54.949428 PySMT-0.9.6.dev7/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/NOTICE
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-05-28 20:26:54.949428 PySMT-0.9.6.dev7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 20:26:54.937428 PySMT-0.9.6.dev7/PySMT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-05-28 20:26:54.000000 PySMT-0.9.6.dev7/PySMT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3808 2022-05-28 20:26:54.000000 PySMT-0.9.6.dev7/PySMT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-28 20:26:54.000000 PySMT-0.9.6.dev7/PySMT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-05-28 20:26:54.000000 PySMT-0.9.6.dev7/PySMT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-05-28 20:26:54.000000 PySMT-0.9.6.dev7/PySMT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10360 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 20:26:54.937428 PySMT-0.9.6.dev7/docs/
--rw-r--r--   0 runner    (1001) docker     (121)    39504 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/docs/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1710 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/docs/api_ref.rst
--rw-r--r--   0 runner    (1001) docker     (121)    16966 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8691 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1651 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 20:26:54.937428 PySMT-0.9.6.dev7/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (121)     4786 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/docs/tutorials/boolean_logic.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2368 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/docs/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 20:26:54.937428 PySMT-0.9.6.dev7/pysmt/
--rw-r--r--   0 runner    (1001) docker     (121)     1596 2022-05-28 20:26:54.000000 PySMT-0.9.6.dev7/pysmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 20:26:54.941428 PySMT-0.9.6.dev7/pysmt/cmd/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2366 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/cmd/check_version.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10203 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/cmd/install.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 20:26:54.941428 PySMT-0.9.6.dev7/pysmt/cmd/installers/
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/cmd/installers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12781 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/cmd/installers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2559 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/cmd/installers/bdd.py
--rw-r--r--   0 runner    (1001) docker     (121)     4086 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/cmd/installers/btor.py
--rw-r--r--   0 runner    (1001) docker     (121)     3936 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/cmd/installers/cvc4.py
--rw-r--r--   0 runner    (1001) docker     (121)     5144 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/cmd/installers/msat.py
--rw-r--r--   0 runner    (1001) docker     (121)     3141 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/cmd/installers/pico.py
--rw-r--r--   0 runner    (1001) docker     (121)     3312 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/cmd/installers/yices.py
--rw-r--r--   0 runner    (1001) docker     (121)     3336 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/cmd/installers/z3.py
--rw-r--r--   0 runner    (1001) docker     (121)     4334 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/cmd/shell.py
--rw-r--r--   0 runner    (1001) docker     (121)     4539 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     4844 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     3965 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     6522 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/environment.py
--rw-r--r--   0 runner    (1001) docker     (121)     4419 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    23923 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)    33628 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/fnode.py
--rw-r--r--   0 runner    (1001) docker     (121)    43460 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/formula.py
--rw-r--r--   0 runner    (1001) docker     (121)    27818 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/logics.py
--rw-r--r--   0 runner    (1001) docker     (121)     8132 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/operators.py
--rw-r--r--   0 runner    (1001) docker     (121)    19461 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/oracles.py
--rw-r--r--   0 runner    (1001) docker     (121)    20786 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/parsing.py
--rw-r--r--   0 runner    (1001) docker     (121)    13387 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/printers.py
--rw-r--r--   0 runner    (1001) docker     (121)    33289 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/rewritings.py
--rw-r--r--   0 runner    (1001) docker     (121)    38485 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (121)    41464 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/simplifier.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 20:26:54.941428 PySMT-0.9.6.dev7/pysmt/smtlib/
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/smtlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4167 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/smtlib/annotations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/smtlib/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 20:26:54.941428 PySMT-0.9.6.dev7/pysmt/smtlib/parser/
--rw-r--r--   0 runner    (1001) docker     (121)     4025 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/smtlib/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    58385 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/smtlib/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    24551 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/smtlib/printers.py
--rw-r--r--   0 runner    (1001) docker     (121)    13387 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/smtlib/script.py
--rw-r--r--   0 runner    (1001) docker     (121)     7987 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/smtlib/solver.py
--rw-r--r--   0 runner    (1001) docker     (121)     2043 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/smtlib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 20:26:54.941428 PySMT-0.9.6.dev7/pysmt/solvers/
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15936 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/solvers/bdd.py
--rw-r--r--   0 runner    (1001) docker     (121)    23813 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/solvers/btor.py
--rw-r--r--   0 runner    (1001) docker     (121)    24538 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/solvers/cvc4.py
--rw-r--r--   0 runner    (1001) docker     (121)     3297 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/solvers/eager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/solvers/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (121)    54967 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/solvers/msat.py
--rw-r--r--   0 runner    (1001) docker     (121)     3837 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/solvers/options.py
--rw-r--r--   0 runner    (1001) docker     (121)    10630 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/solvers/pico.py
--rw-r--r--   0 runner    (1001) docker     (121)     9059 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/solvers/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (121)     4823 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/solvers/qelim.py
--rw-r--r--   0 runner    (1001) docker     (121)     8997 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/solvers/smtlib.py
--rw-r--r--   0 runner    (1001) docker     (121)    17663 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/solvers/solver.py
--rw-r--r--   0 runner    (1001) docker     (121)    23347 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/solvers/yices.py
--rw-r--r--   0 runner    (1001) docker     (121)    40768 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/solvers/z3.py
--rw-r--r--   0 runner    (1001) docker     (121)    13812 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/substituter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 20:26:54.945428 PySMT-0.9.6.dev7/pysmt/test/
--rw-r--r--   0 runner    (1001) docker     (121)     4985 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 20:26:54.945428 PySMT-0.9.6.dev7/pysmt/test/configs/
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/configs/config1.ini
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/configs/config_bad.ini
--rw-r--r--   0 runner    (1001) docker     (121)    39096 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/examples.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 20:26:54.949428 PySMT-0.9.6.dev7/pysmt/test/smtlib/
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/smtlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8434 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/smtlib/parser_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6209 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/smtlib/test_annotations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/smtlib/test_fuzzed.py
--rw-r--r--   0 runner    (1001) docker     (121)     7869 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/smtlib/test_generic_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2893 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/smtlib/test_griggio.py
--rw-r--r--   0 runner    (1001) docker     (121)     3076 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/smtlib/test_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (121)     9930 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/smtlib/test_parser_examples.py
--rw-r--r--   0 runner    (1001) docker     (121)     3659 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/smtlib/test_parser_extensibility.py
--rw-r--r--   0 runner    (1001) docker     (121)      972 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/smtlib/test_parser_lra.py
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/smtlib/test_parser_qf_arrays.py
--rw-r--r--   0 runner    (1001) docker     (121)      981 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/smtlib/test_parser_qf_lia.py
--rw-r--r--   0 runner    (1001) docker     (121)      988 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/smtlib/test_parser_qf_lira.py
--rw-r--r--   0 runner    (1001) docker     (121)      982 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/smtlib/test_parser_qf_lra.py
--rw-r--r--   0 runner    (1001) docker     (121)      981 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/smtlib/test_parser_qf_nia.py
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/smtlib/test_parser_qf_nra.py
--rw-r--r--   0 runner    (1001) docker     (121)      978 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/smtlib/test_parser_qf_uf.py
--rw-r--r--   0 runner    (1001) docker     (121)      984 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/smtlib/test_parser_qf_ufbv.py
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/smtlib/test_parser_type_error.py
--rw-r--r--   0 runner    (1001) docker     (121)    11013 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/smtlib/test_smtlibscript.py
--rw-r--r--   0 runner    (1001) docker     (121)     5788 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_array.py
--rw-r--r--   0 runner    (1001) docker     (121)     3402 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_back.py
--rw-r--r--   0 runner    (1001) docker     (121)     6195 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_bdd.py
--rw-r--r--   0 runner    (1001) docker     (121)    12284 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_bv.py
--rw-r--r--   0 runner    (1001) docker     (121)    14511 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_bv_simplification.py
--rw-r--r--   0 runner    (1001) docker     (121)     3369 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_cnf.py
--rw-r--r--   0 runner    (1001) docker     (121)     3757 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     4618 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     1851 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_cvc4_quantifiers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2850 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_dwf.py
--rw-r--r--   0 runner    (1001) docker     (121)     3662 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_eager_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     4118 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_env.py
--rw-r--r--   0 runner    (1001) docker     (121)     3455 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_euf.py
--rw-r--r--   0 runner    (1001) docker     (121)    38595 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_formula.py
--rw-r--r--   0 runner    (1001) docker     (121)     2754 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_hr_parsing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)     1980 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_int.py
--rw-r--r--   0 runner    (1001) docker     (121)     3941 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2175 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_lira.py
--rw-r--r--   0 runner    (1001) docker     (121)     6734 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_logics.py
--rw-r--r--   0 runner    (1001) docker     (121)     2748 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3439 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_native_qe.py
--rw-r--r--   0 runner    (1001) docker     (121)     6500 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_nia.py
--rw-r--r--   0 runner    (1001) docker     (121)     4417 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_nlira.py
--rw-r--r--   0 runner    (1001) docker     (121)     5615 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_oracles.py
--rw-r--r--   0 runner    (1001) docker     (121)     7133 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (121)     8749 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_printing.py
--rw-r--r--   0 runner    (1001) docker     (121)     7136 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_qe.py
--rw-r--r--   0 runner    (1001) docker     (121)    20119 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_regressions.py
--rw-r--r--   0 runner    (1001) docker     (121)    15625 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_rewritings.py
--rw-r--r--   0 runner    (1001) docker     (121)     3082 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_shannon_expansion.py
--rw-r--r--   0 runner    (1001) docker     (121)     7620 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (121)     3261 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_size.py
--rw-r--r--   0 runner    (1001) docker     (121)    24829 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_solving.py
--rw-r--r--   0 runner    (1001) docker     (121)     6033 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_sorts.py
--rw-r--r--   0 runner    (1001) docker     (121)     8096 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_string.py
--rw-r--r--   0 runner    (1001) docker     (121)     6977 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_typechecker.py
--rw-r--r--   0 runner    (1001) docker     (121)     6563 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_unsat_cores.py
--rw-r--r--   0 runner    (1001) docker     (121)     3522 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_walker_ext.py
--rw-r--r--   0 runner    (1001) docker     (121)     9481 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/test/test_walkers.py
--rw-r--r--   0 runner    (1001) docker     (121)    13271 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/type_checker.py
--rw-r--r--   0 runner    (1001) docker     (121)    17714 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2302 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 20:26:54.949428 PySMT-0.9.6.dev7/pysmt/walkers/
--rw-r--r--   0 runner    (1001) docker     (121)     1585 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/walkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5352 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/walkers/dag.py
--rw-r--r--   0 runner    (1001) docker     (121)     4534 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/walkers/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)     8737 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/walkers/identitydag.py
--rw-r--r--   0 runner    (1001) docker     (121)     2846 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/pysmt/walkers/tree.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-28 20:26:54.949428 PySMT-0.9.6.dev7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1941 2022-05-28 20:26:50.000000 PySMT-0.9.6.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 07:33:15.354791 PySMT-0.9.6.dev9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      601 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-05-30 07:33:15.354791 PySMT-0.9.6.dev9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 07:33:15.322791 PySMT-0.9.6.dev9/PySMT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-05-30 07:33:15.000000 PySMT-0.9.6.dev9/PySMT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3808 2022-05-30 07:33:15.000000 PySMT-0.9.6.dev9/PySMT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-30 07:33:15.000000 PySMT-0.9.6.dev9/PySMT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-05-30 07:33:15.000000 PySMT-0.9.6.dev9/PySMT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-05-30 07:33:15.000000 PySMT-0.9.6.dev9/PySMT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10360 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 07:33:15.322791 PySMT-0.9.6.dev9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)    39504 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/docs/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1710 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/docs/api_ref.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    16966 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     8691 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1651 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 07:33:15.322791 PySMT-0.9.6.dev9/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (121)     4786 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/docs/tutorials/boolean_logic.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2368 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/docs/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 07:33:15.330791 PySMT-0.9.6.dev9/pysmt/
+-rw-r--r--   0 runner    (1001) docker     (121)     1596 2022-05-30 07:33:14.000000 PySMT-0.9.6.dev9/pysmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 07:33:15.330791 PySMT-0.9.6.dev9/pysmt/cmd/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2366 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/cmd/check_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    10203 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/cmd/install.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 07:33:15.330791 PySMT-0.9.6.dev9/pysmt/cmd/installers/
+-rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/cmd/installers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12781 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/cmd/installers/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2559 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/cmd/installers/bdd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4086 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/cmd/installers/btor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3936 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/cmd/installers/cvc4.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5144 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/cmd/installers/msat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3141 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/cmd/installers/pico.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3312 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/cmd/installers/yices.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3336 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/cmd/installers/z3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4334 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/cmd/shell.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4539 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4844 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3965 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6522 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/environment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4419 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23923 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33628 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/fnode.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43460 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/formula.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27818 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/logics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8132 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19461 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/oracles.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20786 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13387 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/printers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33289 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/rewritings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38485 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41464 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/simplifier.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 07:33:15.334791 PySMT-0.9.6.dev9/pysmt/smtlib/
+-rw-r--r--   0 runner    (1001) docker     (121)      650 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/smtlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4167 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/smtlib/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/smtlib/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 07:33:15.334791 PySMT-0.9.6.dev9/pysmt/smtlib/parser/
+-rw-r--r--   0 runner    (1001) docker     (121)     4025 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/smtlib/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    58385 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/smtlib/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24551 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/smtlib/printers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13387 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/smtlib/script.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7987 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/smtlib/solver.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2043 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/smtlib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 07:33:15.338791 PySMT-0.9.6.dev9/pysmt/solvers/
+-rw-r--r--   0 runner    (1001) docker     (121)      650 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15936 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/solvers/bdd.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23813 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/solvers/btor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24538 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/solvers/cvc4.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3297 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/solvers/eager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/solvers/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    54967 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/solvers/msat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3837 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/solvers/options.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10630 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/solvers/pico.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9059 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/solvers/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4823 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/solvers/qelim.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8997 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/solvers/smtlib.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17663 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/solvers/solver.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23347 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/solvers/yices.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40768 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/solvers/z3.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13812 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/substituter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 07:33:15.346791 PySMT-0.9.6.dev9/pysmt/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     4985 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 07:33:15.346791 PySMT-0.9.6.dev9/pysmt/test/configs/
+-rw-r--r--   0 runner    (1001) docker     (121)      224 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/configs/config1.ini
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/configs/config_bad.ini
+-rw-r--r--   0 runner    (1001) docker     (121)    39096 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/examples.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 07:33:15.354791 PySMT-0.9.6.dev9/pysmt/test/smtlib/
+-rw-r--r--   0 runner    (1001) docker     (121)      650 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/smtlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8434 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/smtlib/parser_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6209 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/smtlib/test_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/smtlib/test_fuzzed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7869 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/smtlib/test_generic_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2893 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/smtlib/test_griggio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3076 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/smtlib/test_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9930 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/smtlib/test_parser_examples.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3659 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/smtlib/test_parser_extensibility.py
+-rw-r--r--   0 runner    (1001) docker     (121)      972 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/smtlib/test_parser_lra.py
+-rw-r--r--   0 runner    (1001) docker     (121)      987 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/smtlib/test_parser_qf_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (121)      981 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/smtlib/test_parser_qf_lia.py
+-rw-r--r--   0 runner    (1001) docker     (121)      988 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/smtlib/test_parser_qf_lira.py
+-rw-r--r--   0 runner    (1001) docker     (121)      982 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/smtlib/test_parser_qf_lra.py
+-rw-r--r--   0 runner    (1001) docker     (121)      981 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/smtlib/test_parser_qf_nia.py
+-rw-r--r--   0 runner    (1001) docker     (121)      979 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/smtlib/test_parser_qf_nra.py
+-rw-r--r--   0 runner    (1001) docker     (121)      978 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/smtlib/test_parser_qf_uf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      984 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/smtlib/test_parser_qf_ufbv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/smtlib/test_parser_type_error.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11013 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/smtlib/test_smtlibscript.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5788 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3402 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_back.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6195 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12284 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_bv.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14511 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_bv_simplification.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3369 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_cnf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3757 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4618 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1851 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_cvc4_quantifiers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2850 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_dwf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3662 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_eager_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4118 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3455 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_euf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38595 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_formula.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2754 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_hr_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1980 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_int.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3941 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2175 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_lira.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6734 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_logics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2748 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3439 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_native_qe.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6500 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_nia.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4417 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_nlira.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5615 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_oracles.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7133 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8749 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_printing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7136 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_qe.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20119 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15625 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_rewritings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3082 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_shannon_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7620 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3261 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_size.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24829 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_solving.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6033 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_sorts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8096 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6977 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_typechecker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6563 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_unsat_cores.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3522 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_walker_ext.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9481 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/test/test_walkers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13271 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17714 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/typing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2302 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 07:33:15.354791 PySMT-0.9.6.dev9/pysmt/walkers/
+-rw-r--r--   0 runner    (1001) docker     (121)     1585 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/walkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5352 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/walkers/dag.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4534 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/walkers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8737 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/walkers/identitydag.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2846 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/pysmt/walkers/tree.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-30 07:33:15.354791 PySMT-0.9.6.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1941 2022-05-30 07:33:10.000000 PySMT-0.9.6.dev9/setup.py
```

### Comparing `PySMT-0.9.6.dev7/LICENSE` & `PySMT-0.9.6.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/NOTICE` & `PySMT-0.9.6.dev9/NOTICE`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/PKG-INFO` & `PySMT-0.9.6.dev9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: PySMT
-Version: 0.9.6.dev7
+Version: 0.9.6.dev9
 Summary: A solver-agnostic library for SMT Formulae manipulation and solving
 Home-page: http://www.pysmt.org
 Author: PySMT Team
 Author-email: info@pysmt.org
 License: APACHE
 Description: ============================================================
          pySMT: A library for SMT formulae manipulation and solving
```

### Comparing `PySMT-0.9.6.dev7/PySMT.egg-info/PKG-INFO` & `PySMT-0.9.6.dev9/PySMT.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: PySMT
-Version: 0.9.6.dev7
+Version: 0.9.6.dev9
 Summary: A solver-agnostic library for SMT Formulae manipulation and solving
 Home-page: http://www.pysmt.org
 Author: PySMT Team
 Author-email: info@pysmt.org
 License: APACHE
 Description: ============================================================
          pySMT: A library for SMT formulae manipulation and solving
```

### Comparing `PySMT-0.9.6.dev7/PySMT.egg-info/SOURCES.txt` & `PySMT-0.9.6.dev9/PySMT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/README.rst` & `PySMT-0.9.6.dev9/README.rst`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/docs/CHANGES.rst` & `PySMT-0.9.6.dev9/docs/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/docs/api_ref.rst` & `PySMT-0.9.6.dev9/docs/api_ref.rst`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/docs/development.rst` & `PySMT-0.9.6.dev9/docs/development.rst`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/docs/getting_started.rst` & `PySMT-0.9.6.dev9/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/docs/index.rst` & `PySMT-0.9.6.dev9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/docs/tutorials/boolean_logic.rst` & `PySMT-0.9.6.dev9/docs/tutorials/boolean_logic.rst`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/docs/tutorials.rst` & `PySMT-0.9.6.dev9/docs/tutorials.rst`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/__init__.py` & `PySMT-0.9.6.dev9/pysmt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-VERSION = (0, 9, 6, "dev", 7)
+VERSION = (0, 9, 6, "dev", 9)
 
 # Try to provide human-readable version of latest commit for dev versions
 # E.g. v0.5.1-4-g49a49f2-wip
 #      * 4 commits after tag v0.5.1
 #      * Latest commit "49a49f2"
 #      * -wip: Working tree is dirty (non committed stuff)
 # See: https://git-scm.com/docs/git-describe
```

### Comparing `PySMT-0.9.6.dev7/pysmt/__main__.py` & `PySMT-0.9.6.dev9/pysmt/__main__.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/cmd/check_version.py` & `PySMT-0.9.6.dev9/pysmt/cmd/check_version.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/cmd/install.py` & `PySMT-0.9.6.dev9/pysmt/cmd/install.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/cmd/installers/__init__.py` & `PySMT-0.9.6.dev9/pysmt/cmd/installers/__init__.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/cmd/installers/base.py` & `PySMT-0.9.6.dev9/pysmt/cmd/installers/base.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/cmd/installers/bdd.py` & `PySMT-0.9.6.dev9/pysmt/cmd/installers/bdd.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/cmd/installers/btor.py` & `PySMT-0.9.6.dev9/pysmt/cmd/installers/btor.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/cmd/installers/cvc4.py` & `PySMT-0.9.6.dev9/pysmt/cmd/installers/cvc4.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/cmd/installers/msat.py` & `PySMT-0.9.6.dev9/pysmt/cmd/installers/msat.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/cmd/installers/pico.py` & `PySMT-0.9.6.dev9/pysmt/cmd/installers/pico.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/cmd/installers/yices.py` & `PySMT-0.9.6.dev9/pysmt/cmd/installers/yices.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/cmd/installers/z3.py` & `PySMT-0.9.6.dev9/pysmt/cmd/installers/z3.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/cmd/shell.py` & `PySMT-0.9.6.dev9/pysmt/cmd/shell.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/configuration.py` & `PySMT-0.9.6.dev9/pysmt/configuration.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/constants.py` & `PySMT-0.9.6.dev9/pysmt/constants.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/decorators.py` & `PySMT-0.9.6.dev9/pysmt/decorators.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/environment.py` & `PySMT-0.9.6.dev9/pysmt/environment.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/exceptions.py` & `PySMT-0.9.6.dev9/pysmt/exceptions.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/factory.py` & `PySMT-0.9.6.dev9/pysmt/factory.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/fnode.py` & `PySMT-0.9.6.dev9/pysmt/fnode.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/formula.py` & `PySMT-0.9.6.dev9/pysmt/formula.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/logics.py` & `PySMT-0.9.6.dev9/pysmt/logics.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/operators.py` & `PySMT-0.9.6.dev9/pysmt/operators.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/oracles.py` & `PySMT-0.9.6.dev9/pysmt/oracles.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/parsing.py` & `PySMT-0.9.6.dev9/pysmt/parsing.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/printers.py` & `PySMT-0.9.6.dev9/pysmt/printers.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/rewritings.py` & `PySMT-0.9.6.dev9/pysmt/rewritings.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/shortcuts.py` & `PySMT-0.9.6.dev9/pysmt/shortcuts.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/simplifier.py` & `PySMT-0.9.6.dev9/pysmt/simplifier.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/smtlib/__init__.py` & `PySMT-0.9.6.dev9/pysmt/smtlib/__init__.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/smtlib/annotations.py` & `PySMT-0.9.6.dev9/pysmt/smtlib/annotations.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/smtlib/commands.py` & `PySMT-0.9.6.dev9/pysmt/smtlib/commands.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/smtlib/parser/__init__.py` & `PySMT-0.9.6.dev9/pysmt/smtlib/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/smtlib/parser/parser.py` & `PySMT-0.9.6.dev9/pysmt/smtlib/parser/parser.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/smtlib/printers.py` & `PySMT-0.9.6.dev9/pysmt/smtlib/printers.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/smtlib/script.py` & `PySMT-0.9.6.dev9/pysmt/smtlib/script.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/smtlib/solver.py` & `PySMT-0.9.6.dev9/pysmt/smtlib/solver.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/smtlib/utils.py` & `PySMT-0.9.6.dev9/pysmt/smtlib/utils.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/solvers/__init__.py` & `PySMT-0.9.6.dev9/pysmt/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/solvers/bdd.py` & `PySMT-0.9.6.dev9/pysmt/solvers/bdd.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/solvers/btor.py` & `PySMT-0.9.6.dev9/pysmt/solvers/btor.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/solvers/cvc4.py` & `PySMT-0.9.6.dev9/pysmt/solvers/cvc4.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/solvers/eager.py` & `PySMT-0.9.6.dev9/pysmt/solvers/eager.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/solvers/interpolation.py` & `PySMT-0.9.6.dev9/pysmt/solvers/interpolation.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/solvers/msat.py` & `PySMT-0.9.6.dev9/pysmt/solvers/msat.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/solvers/options.py` & `PySMT-0.9.6.dev9/pysmt/solvers/options.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/solvers/pico.py` & `PySMT-0.9.6.dev9/pysmt/solvers/pico.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/solvers/portfolio.py` & `PySMT-0.9.6.dev9/pysmt/solvers/portfolio.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/solvers/qelim.py` & `PySMT-0.9.6.dev9/pysmt/solvers/qelim.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/solvers/smtlib.py` & `PySMT-0.9.6.dev9/pysmt/solvers/smtlib.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/solvers/solver.py` & `PySMT-0.9.6.dev9/pysmt/solvers/solver.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/solvers/yices.py` & `PySMT-0.9.6.dev9/pysmt/solvers/yices.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/solvers/z3.py` & `PySMT-0.9.6.dev9/pysmt/solvers/z3.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/substituter.py` & `PySMT-0.9.6.dev9/pysmt/substituter.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/__init__.py` & `PySMT-0.9.6.dev9/pysmt/test/__init__.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/examples.py` & `PySMT-0.9.6.dev9/pysmt/test/examples.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/smtlib/__init__.py` & `PySMT-0.9.6.dev9/pysmt/test/smtlib/__init__.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/smtlib/parser_utils.py` & `PySMT-0.9.6.dev9/pysmt/test/smtlib/parser_utils.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/smtlib/test_annotations.py` & `PySMT-0.9.6.dev9/pysmt/test/smtlib/test_annotations.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/smtlib/test_fuzzed.py` & `PySMT-0.9.6.dev9/pysmt/test/smtlib/test_fuzzed.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/smtlib/test_generic_wrapper.py` & `PySMT-0.9.6.dev9/pysmt/test/smtlib/test_generic_wrapper.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/smtlib/test_griggio.py` & `PySMT-0.9.6.dev9/pysmt/test/smtlib/test_griggio.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/smtlib/test_model_validation.py` & `PySMT-0.9.6.dev9/pysmt/test/smtlib/test_model_validation.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/smtlib/test_parser_examples.py` & `PySMT-0.9.6.dev9/pysmt/test/smtlib/test_parser_examples.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/smtlib/test_parser_extensibility.py` & `PySMT-0.9.6.dev9/pysmt/test/smtlib/test_parser_extensibility.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/smtlib/test_parser_lra.py` & `PySMT-0.9.6.dev9/pysmt/test/smtlib/test_parser_lra.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/smtlib/test_parser_qf_arrays.py` & `PySMT-0.9.6.dev9/pysmt/test/smtlib/test_parser_qf_arrays.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/smtlib/test_parser_qf_lia.py` & `PySMT-0.9.6.dev9/pysmt/test/smtlib/test_parser_qf_lia.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/smtlib/test_parser_qf_lira.py` & `PySMT-0.9.6.dev9/pysmt/test/smtlib/test_parser_qf_lira.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/smtlib/test_parser_qf_lra.py` & `PySMT-0.9.6.dev9/pysmt/test/smtlib/test_parser_qf_lra.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/smtlib/test_parser_qf_nia.py` & `PySMT-0.9.6.dev9/pysmt/test/smtlib/test_parser_qf_nia.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/smtlib/test_parser_qf_nra.py` & `PySMT-0.9.6.dev9/pysmt/test/smtlib/test_parser_qf_nra.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/smtlib/test_parser_qf_uf.py` & `PySMT-0.9.6.dev9/pysmt/test/smtlib/test_parser_qf_uf.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/smtlib/test_parser_qf_ufbv.py` & `PySMT-0.9.6.dev9/pysmt/test/smtlib/test_parser_qf_ufbv.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/smtlib/test_parser_type_error.py` & `PySMT-0.9.6.dev9/pysmt/test/smtlib/test_parser_type_error.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/smtlib/test_smtlibscript.py` & `PySMT-0.9.6.dev9/pysmt/test/smtlib/test_smtlibscript.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_array.py` & `PySMT-0.9.6.dev9/pysmt/test/test_array.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_back.py` & `PySMT-0.9.6.dev9/pysmt/test/test_back.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_bdd.py` & `PySMT-0.9.6.dev9/pysmt/test/test_bdd.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_bv.py` & `PySMT-0.9.6.dev9/pysmt/test/test_bv.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_bv_simplification.py` & `PySMT-0.9.6.dev9/pysmt/test/test_bv_simplification.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_cnf.py` & `PySMT-0.9.6.dev9/pysmt/test/test_cnf.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_configuration.py` & `PySMT-0.9.6.dev9/pysmt/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_constants.py` & `PySMT-0.9.6.dev9/pysmt/test/test_constants.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_cvc4_quantifiers.py` & `PySMT-0.9.6.dev9/pysmt/test/test_cvc4_quantifiers.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_dwf.py` & `PySMT-0.9.6.dev9/pysmt/test/test_dwf.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_eager_model.py` & `PySMT-0.9.6.dev9/pysmt/test/test_eager_model.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_env.py` & `PySMT-0.9.6.dev9/pysmt/test/test_env.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_euf.py` & `PySMT-0.9.6.dev9/pysmt/test/test_euf.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_formula.py` & `PySMT-0.9.6.dev9/pysmt/test/test_formula.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_hr_parsing.py` & `PySMT-0.9.6.dev9/pysmt/test/test_hr_parsing.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_imports.py` & `PySMT-0.9.6.dev9/pysmt/test/test_imports.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_int.py` & `PySMT-0.9.6.dev9/pysmt/test/test_int.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_interpolation.py` & `PySMT-0.9.6.dev9/pysmt/test/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_lira.py` & `PySMT-0.9.6.dev9/pysmt/test/test_lira.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_logics.py` & `PySMT-0.9.6.dev9/pysmt/test/test_logics.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_models.py` & `PySMT-0.9.6.dev9/pysmt/test/test_models.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_native_qe.py` & `PySMT-0.9.6.dev9/pysmt/test/test_native_qe.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_nia.py` & `PySMT-0.9.6.dev9/pysmt/test/test_nia.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_nlira.py` & `PySMT-0.9.6.dev9/pysmt/test/test_nlira.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_oracles.py` & `PySMT-0.9.6.dev9/pysmt/test/test_oracles.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_portfolio.py` & `PySMT-0.9.6.dev9/pysmt/test/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_printing.py` & `PySMT-0.9.6.dev9/pysmt/test/test_printing.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_qe.py` & `PySMT-0.9.6.dev9/pysmt/test/test_qe.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_regressions.py` & `PySMT-0.9.6.dev9/pysmt/test/test_regressions.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_rewritings.py` & `PySMT-0.9.6.dev9/pysmt/test/test_rewritings.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_shannon_expansion.py` & `PySMT-0.9.6.dev9/pysmt/test/test_shannon_expansion.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_simplify.py` & `PySMT-0.9.6.dev9/pysmt/test/test_simplify.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_size.py` & `PySMT-0.9.6.dev9/pysmt/test/test_size.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_solving.py` & `PySMT-0.9.6.dev9/pysmt/test/test_solving.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_sorts.py` & `PySMT-0.9.6.dev9/pysmt/test/test_sorts.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_string.py` & `PySMT-0.9.6.dev9/pysmt/test/test_string.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_typechecker.py` & `PySMT-0.9.6.dev9/pysmt/test/test_typechecker.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_unsat_cores.py` & `PySMT-0.9.6.dev9/pysmt/test/test_unsat_cores.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_walker_ext.py` & `PySMT-0.9.6.dev9/pysmt/test/test_walker_ext.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/test/test_walkers.py` & `PySMT-0.9.6.dev9/pysmt/test/test_walkers.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/type_checker.py` & `PySMT-0.9.6.dev9/pysmt/type_checker.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/typing.py` & `PySMT-0.9.6.dev9/pysmt/typing.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/utils.py` & `PySMT-0.9.6.dev9/pysmt/utils.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/walkers/__init__.py` & `PySMT-0.9.6.dev9/pysmt/walkers/__init__.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/walkers/dag.py` & `PySMT-0.9.6.dev9/pysmt/walkers/dag.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/walkers/generic.py` & `PySMT-0.9.6.dev9/pysmt/walkers/generic.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/walkers/identitydag.py` & `PySMT-0.9.6.dev9/pysmt/walkers/identitydag.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/pysmt/walkers/tree.py` & `PySMT-0.9.6.dev9/pysmt/walkers/tree.py`

 * *Files identical despite different names*

### Comparing `PySMT-0.9.6.dev7/setup.py` & `PySMT-0.9.6.dev9/setup.py`

 * *Files identical despite different names*

