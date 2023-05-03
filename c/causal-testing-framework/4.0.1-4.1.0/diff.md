# Comparing `tmp/causal_testing_framework-4.0.1.tar.gz` & `tmp/causal_testing_framework-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causal_testing_framework-4.0.1.tar", last modified: Wed Apr 26 15:31:36 2023, max compression
+gzip compressed data, was "causal_testing_framework-4.1.0.tar", last modified: Wed May  3 14:59:03 2023, max compression
```

## Comparing `causal_testing_framework-4.0.1.tar` & `causal_testing_framework-4.1.0.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.782781 causal_testing_framework-4.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.762781 causal_testing_framework-4.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.762781 causal_testing_framework-4.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.762781 causal_testing_framework-4.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/.github/workflows/ci-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/.github/workflows/lint-format.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/.mega-linter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-26 15:31:36.782781 causal_testing_framework-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.762781 causal_testing_framework-4.0.1/causal_testing/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.762781 causal_testing_framework-4.0.1/causal_testing/data_collection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/data_collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/data_collection/data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.762781 causal_testing_framework-4.0.1/causal_testing/generation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/generation/abstract_causal_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/generation/enum_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.766781 causal_testing_framework-4.0.1/causal_testing/json_front/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/json_front/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18684 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/json_front/json_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.766781 causal_testing_framework-4.0.1/causal_testing/specification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/specification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26803 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/specification/causal_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/specification/causal_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/specification/metamorphic_relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/specification/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/specification/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.766781 causal_testing_framework-4.0.1/causal_testing/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/testing/base_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/testing/causal_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    13663 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/testing/causal_test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/testing/causal_test_outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/testing/causal_test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/testing/causal_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/testing/effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    30782 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/testing/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/testing/intervention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/causal_testing/testing/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.766781 causal_testing_framework-4.0.1/causal_testing_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-26 15:31:36.000000 causal_testing_framework-4.0.1/causal_testing_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-26 15:31:36.000000 causal_testing_framework-4.0.1/causal_testing_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:31:36.000000 causal_testing_framework-4.0.1/causal_testing_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-26 15:31:36.000000 causal_testing_framework-4.0.1/causal_testing_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-26 15:31:36.000000 causal_testing_framework-4.0.1/causal_testing_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.766781 causal_testing_framework-4.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.770781 causal_testing_framework-4.0.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/docs/source/description.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.770781 causal_testing_framework-4.0.1/docs/source/frontends/
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/docs/source/frontends/json_front_end.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/docs/source/frontends/test_suite.rst
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/docs/source/glossary.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.770781 causal_testing_framework-4.0.1/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/docs/source/images/workflow.png
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/docs/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.770781 causal_testing_framework-4.0.1/docs/source/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/docs/source/modules/causal_specification.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/docs/source/modules/causal_tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/docs/source/modules/data_collector.rst
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/docs/source/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.770781 causal_testing_framework-4.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.758781 causal_testing_framework-4.0.1/examples/covasim_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.770781 causal_testing_framework-4.0.1/examples/covasim_/doubling_beta/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/covasim_/doubling_beta/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/covasim_/doubling_beta/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    24596 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/covasim_/doubling_beta/dag.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.770781 causal_testing_framework-4.0.1/examples/covasim_/doubling_beta/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1355776 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/covasim_/doubling_beta/data/10k_observational_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15718 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/covasim_/doubling_beta/example_beta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.774781 causal_testing_framework-4.0.1/examples/covasim_/vaccinating_elderly/
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/covasim_/vaccinating_elderly/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/covasim_/vaccinating_elderly/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    23290 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/covasim_/vaccinating_elderly/dag.png
--rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/covasim_/vaccinating_elderly/example_vaccine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.774781 causal_testing_framework-4.0.1/examples/lr91/
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/lr91/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/lr91/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    73886 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/lr91/dag.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.774781 causal_testing_framework-4.0.1/examples/lr91/data/
--rw-r--r--   0 runner    (1001) docker     (123)    40715 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/lr91/data/normalised_results.csv
--rw-r--r--   0 runner    (1001) docker     (123)    40686 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/lr91/data/results.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/lr91/example_max_conductances.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/lr91/example_max_conductances_test_suite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.774781 causal_testing_framework-4.0.1/examples/poisson/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/poisson/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/poisson/causal_tests.json
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/poisson/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    61017 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/poisson/data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/poisson/example_run_causal_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.778781 causal_testing_framework-4.0.1/examples/poisson-line-process/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/poisson-line-process/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/poisson-line-process/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/poisson-line-process/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    53765 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/poisson-line-process/dag.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.762781 causal_testing_framework-4.0.1/examples/poisson-line-process/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.778781 causal_testing_framework-4.0.1/examples/poisson-line-process/data/random/
--rw-r--r--   0 runner    (1001) docker     (123)   102007 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/poisson-line-process/data/random/data_random_1000.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.778781 causal_testing_framework-4.0.1/examples/poisson-line-process/data/smt_100/
--rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14925 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    17103 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    26889 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/examples/poisson-line-process/example_poisson_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.778781 causal_testing_framework-4.0.1/images/
--rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/images/workflow.png
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 15:31:36.782781 causal_testing_framework-4.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.778781 causal_testing_framework-4.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.778781 causal_testing_framework-4.0.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   374288 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/tests/data/nhefs.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.778781 causal_testing_framework-4.0.1/tests/data_collection_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/tests/data_collection_tests/test_observational_data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.778781 causal_testing_framework-4.0.1/tests/generation_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/tests/generation_tests/test_abstract_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.778781 causal_testing_framework-4.0.1/tests/json_front_tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10798 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/tests/json_front_tests/test_json_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.762781 causal_testing_framework-4.0.1/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.782781 causal_testing_framework-4.0.1/tests/resources/data/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/tests/resources/data/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/tests/resources/data/data.csv
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/tests/resources/data/data_with_meta.csv
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/tests/resources/data/tests.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.782781 causal_testing_framework-4.0.1/tests/specification_tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17967 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/tests/specification_tests/test_causal_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)    13719 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/tests/specification_tests/test_metamorphic_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/tests/specification_tests/test_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/tests/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:31:36.782781 causal_testing_framework-4.0.1/tests/testing_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/tests/testing_tests/test_causal_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    13873 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/tests/testing_tests/test_causal_test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/tests/testing_tests/test_causal_test_outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/tests/testing_tests/test_causal_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    18696 2023-04-26 15:30:39.000000 causal_testing_framework-4.0.1/tests/testing_tests/test_estimators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.705007 causal_testing_framework-4.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.677007 causal_testing_framework-4.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.677007 causal_testing_framework-4.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.677007 causal_testing_framework-4.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/.github/workflows/ci-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/.github/workflows/lint-format.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/.mega-linter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-03 14:59:03.705007 causal_testing_framework-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.677007 causal_testing_framework-4.1.0/causal_testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.677007 causal_testing_framework-4.1.0/causal_testing/data_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/data_collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/data_collection/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.677007 causal_testing_framework-4.1.0/causal_testing/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/generation/abstract_causal_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/generation/enum_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.677007 causal_testing_framework-4.1.0/causal_testing/json_front/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/json_front/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18897 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/json_front/json_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.681007 causal_testing_framework-4.1.0/causal_testing/specification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/specification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26803 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/specification/causal_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/specification/causal_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/specification/metamorphic_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/specification/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/specification/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.681007 causal_testing_framework-4.1.0/causal_testing/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/testing/base_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/testing/causal_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13663 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/testing/causal_test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/testing/causal_test_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/testing/causal_test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/testing/causal_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/testing/effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30782 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/testing/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/testing/intervention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/testing/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.681007 causal_testing_framework-4.1.0/causal_testing_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-03 14:59:03.000000 causal_testing_framework-4.1.0/causal_testing_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-05-03 14:59:03.000000 causal_testing_framework-4.1.0/causal_testing_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 14:59:03.000000 causal_testing_framework-4.1.0/causal_testing_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-03 14:59:03.000000 causal_testing_framework-4.1.0/causal_testing_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-03 14:59:03.000000 causal_testing_framework-4.1.0/causal_testing_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.681007 causal_testing_framework-4.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.681007 causal_testing_framework-4.1.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/description.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.681007 causal_testing_framework-4.1.0/docs/source/frontends/
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/frontends/json_front_end.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/frontends/test_suite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/glossary.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.681007 causal_testing_framework-4.1.0/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/images/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.681007 causal_testing_framework-4.1.0/docs/source/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/modules/causal_specification.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/modules/causal_tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/modules/data_collector.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.685007 causal_testing_framework-4.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.673007 causal_testing_framework-4.1.0/examples/covasim_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.685007 causal_testing_framework-4.1.0/examples/covasim_/doubling_beta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/covasim_/doubling_beta/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/covasim_/doubling_beta/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    24596 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/covasim_/doubling_beta/dag.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.685007 causal_testing_framework-4.1.0/examples/covasim_/doubling_beta/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1355776 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15718 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/covasim_/doubling_beta/example_beta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.685007 causal_testing_framework-4.1.0/examples/covasim_/vaccinating_elderly/
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/covasim_/vaccinating_elderly/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/covasim_/vaccinating_elderly/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    23290 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/covasim_/vaccinating_elderly/dag.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/covasim_/vaccinating_elderly/example_vaccine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.685007 causal_testing_framework-4.1.0/examples/lr91/
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/lr91/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/lr91/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    73886 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/lr91/dag.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.685007 causal_testing_framework-4.1.0/examples/lr91/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    40715 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/lr91/data/normalised_results.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    40686 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/lr91/data/results.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/lr91/example_max_conductances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/lr91/example_max_conductances_test_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.693007 causal_testing_framework-4.1.0/examples/poisson/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson/causal_tests.json
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    61017 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson/data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson/example_run_causal_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.693007 causal_testing_framework-4.1.0/examples/poisson-line-process/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    53765 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/dag.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.673007 causal_testing_framework-4.1.0/examples/poisson-line-process/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.693007 causal_testing_framework-4.1.0/examples/poisson-line-process/data/random/
+-rw-r--r--   0 runner    (1001) docker     (123)   102007 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/data/random/data_random_1000.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.697007 causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/
+-rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14925 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    17103 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    26889 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/example_poisson_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.697007 causal_testing_framework-4.1.0/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/images/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 14:59:03.705007 causal_testing_framework-4.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.697007 causal_testing_framework-4.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.697007 causal_testing_framework-4.1.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   374288 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/data/nhefs.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.697007 causal_testing_framework-4.1.0/tests/data_collection_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/data_collection_tests/test_observational_data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.697007 causal_testing_framework-4.1.0/tests/generation_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/generation_tests/test_abstract_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.701007 causal_testing_framework-4.1.0/tests/json_front_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10798 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/json_front_tests/test_json_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.677007 causal_testing_framework-4.1.0/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.701007 causal_testing_framework-4.1.0/tests/resources/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/resources/data/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/resources/data/data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/resources/data/data_with_meta.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/resources/data/tests.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.701007 causal_testing_framework-4.1.0/tests/specification_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17967 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/specification_tests/test_causal_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13719 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/specification_tests/test_metamorphic_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/specification_tests/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.705007 causal_testing_framework-4.1.0/tests/testing_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/testing_tests/test_causal_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13873 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/testing_tests/test_causal_test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/testing_tests/test_causal_test_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/testing_tests/test_causal_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18696 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/testing_tests/test_estimators.py
```

### Comparing `causal_testing_framework-4.0.1/.github/CONTRIBUTING.md` & `causal_testing_framework-4.1.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/.github/ISSUE_TEMPLATE/bug_report.md` & `causal_testing_framework-4.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/.github/ISSUE_TEMPLATE/feature_request.md` & `causal_testing_framework-4.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/.github/workflows/ci-tests.yaml` & `causal_testing_framework-4.1.0/.github/workflows/ci-tests.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/.github/workflows/lint-format.yaml` & `causal_testing_framework-4.1.0/.github/workflows/lint-format.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/.github/workflows/publish-to-pypi.yaml` & `causal_testing_framework-4.1.0/.github/workflows/publish-to-pypi.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/.gitignore` & `causal_testing_framework-4.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/.pylintrc` & `causal_testing_framework-4.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/.readthedocs.yaml` & `causal_testing_framework-4.1.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/LICENSE` & `causal_testing_framework-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/PKG-INFO` & `causal_testing_framework-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causal_testing_framework
-Version: 4.0.1
+Version: 4.1.0
 Summary: A framework for causal testing using causal directed acyclic graphs.
 Author: The CITCOM team
 License: MIT
 Project-URL: Bug_Tracker, https://github.com/CITCOM-project/CausalTestingFramework/issues
 Project-URL: Documentation, https://causal-testing-framework.readthedocs.io/
 Project-URL: Source, https://github.com/CITCOM-project/CausalTestingFramework
 Keywords: causal inference,verification
```

### Comparing `causal_testing_framework-4.0.1/README.md` & `causal_testing_framework-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/causal_testing/data_collection/data_collector.py` & `causal_testing_framework-4.1.0/causal_testing/data_collection/data_collector.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/causal_testing/generation/abstract_causal_test_case.py` & `causal_testing_framework-4.1.0/causal_testing/generation/abstract_causal_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/causal_testing/generation/enum_gen.py` & `causal_testing_framework-4.1.0/causal_testing/generation/enum_gen.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/causal_testing/json_front/json_class.py` & `causal_testing_framework-4.1.0/causal_testing/json_front/json_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from causal_testing.data_collection.data_collector import ObservationalDataCollector
 from causal_testing.generation.abstract_causal_test_case import AbstractCausalTestCase
 from causal_testing.specification.causal_dag import CausalDAG
 from causal_testing.specification.causal_specification import CausalSpecification
 from causal_testing.specification.scenario import Scenario
 from causal_testing.specification.variable import Input, Meta, Output
 from causal_testing.testing.causal_test_case import CausalTestCase
+from causal_testing.testing.causal_test_result import CausalTestResult
 from causal_testing.testing.causal_test_engine import CausalTestEngine
 from causal_testing.testing.estimators import Estimator
 from causal_testing.testing.base_test_case import BaseTestCase
 
 logger = logging.getLogger(__name__)
 
 
@@ -120,36 +121,37 @@
                 if test["estimate_type"] == "coefficient":
                     base_test_case = BaseTestCase(
                         treatment_variable=next(self.scenario.variables[v] for v in test["mutations"]),
                         outcome_variable=next(self.scenario.variables[v] for v in test["expected_effect"]),
                         effect=test.get("effect", "direct"),
                     )
                     assert len(test["expected_effect"]) == 1, "Can only have one expected effect."
-                    concrete_tests = [
-                        CausalTestCase(
-                            base_test_case=base_test_case,
-                            expected_causal_effect=next(
-                                effects[effect] for variable, effect in test["expected_effect"].items()
-                            ),
-                            estimate_type="coefficient",
-                            effect_modifier_configuration={
-                                self.scenario.variables[v] for v in test.get("effect_modifiers", [])
-                            },
-                        )
-                    ]
-                    failures = self._execute_tests(concrete_tests, test, f_flag)
+                    causal_test_case = CausalTestCase(
+                        base_test_case=base_test_case,
+                        expected_causal_effect=next(
+                            effects[effect] for variable, effect in test["expected_effect"].items()
+                        ),
+                        estimate_type="coefficient",
+                        effect_modifier_configuration={
+                            self.scenario.variables[v] for v in test.get("effect_modifiers", [])
+                        },
+                    )
+                    result = self._execute_test_case(causal_test_case=causal_test_case, test=test, f_flag=f_flag)
                     msg = (
                         f"Executing test: {test['name']} \n"
-                        + f"  {concrete_tests[0]} \n"
-                        + f"  {failures}/{len(concrete_tests)} failed for {test['name']}"
+                        + f"  {causal_test_case} \n"
+                        + "  "
+                        + ("\n  ").join(str(result[1]).split("\n"))
+                        + "==============\n"
+                        + f"  Result: {'FAILED' if result[0] else 'Passed'}"
                     )
                 else:
                     abstract_test = self._create_abstract_test_case(test, mutates, effects)
-                    concrete_tests, dummy = abstract_test.generate_concrete_tests(5, 0.05)
-                    failures = self._execute_tests(concrete_tests, test, f_flag)
+                    concrete_tests, _ = abstract_test.generate_concrete_tests(5, 0.05)
+                    failures, _ = self._execute_tests(concrete_tests, test, f_flag)
 
                     msg = (
                         f"Executing test: {test['name']} \n"
                         + "  abstract_test \n"
                         + f"  {abstract_test} \n"
                         + f"  {abstract_test.treatment_variable.name},"
                         + f"  {abstract_test.treatment_variable.distribution} \n"
@@ -169,37 +171,36 @@
                 causal_test_case = CausalTestCase(
                     base_test_case=base_test_case,
                     expected_causal_effect=effects[test["expected_effect"][outcome_variable]],
                     control_value=test["control_value"],
                     treatment_value=test["treatment_value"],
                     estimate_type=test["estimate_type"],
                 )
-                if self._execute_test_case(causal_test_case=causal_test_case, test=test, f_flag=f_flag):
-                    result = "failed"
-                else:
-                    result = "passed"
+                failed, _ = self._execute_test_case(causal_test_case=causal_test_case, test=test, f_flag=f_flag)
 
                 msg = (
                     f"Executing concrete test: {test['name']} \n"
                     + f"treatment variable: {test['treatment_variable']} \n"
                     + f"outcome_variable = {outcome_variable} \n"
                     + f"control value = {test['control_value']}, treatment value = {test['treatment_value']} \n"
-                    + f"result - {result}"
+                    + f"Result: {'FAILED' if failed else 'Passed'}"
                 )
                 self._append_to_file(msg, logging.INFO)
 
     def _execute_tests(self, concrete_tests, test, f_flag):
         failures = 0
+        details = []
         if "formula" in test:
             self._append_to_file(f"Estimator formula used for test: {test['formula']}")
         for concrete_test in concrete_tests:
-            failed = self._execute_test_case(concrete_test, test, f_flag)
+            failed, result = self._execute_test_case(concrete_test, test, f_flag)
+            details.append(result)
             if failed:
                 failures += 1
-        return failures
+        return failures, details
 
     def _json_parse(self):
         """Parse a JSON input file into inputs, outputs, metas and a test plan"""
         with open(self.input_paths.json_path, encoding="utf-8") as f:
             self.test_plan = json.load(f)
         for data_file in self.input_paths.data_paths:
             df = pd.read_csv(data_file, header=0)
@@ -209,15 +210,17 @@
     def _populate_metas(self):
         """
         Populate data with meta-variable values and add distributions to Causal Testing Framework Variables
         """
         for meta in self.scenario.variables_of_type(Meta):
             meta.populate(self.data)
 
-    def _execute_test_case(self, causal_test_case: CausalTestCase, test: Iterable[Mapping], f_flag: bool) -> bool:
+    def _execute_test_case(
+        self, causal_test_case: CausalTestCase, test: Iterable[Mapping], f_flag: bool
+    ) -> (bool, CausalTestResult):
         """Executes a singular test case, prints the results and returns the test case result
         :param causal_test_case: The concrete test case to be executed
         :param test: Single JSON test definition stored in a mapping (dict)
         :param f_flag: Failure flag that if True the script will stop executing when a test fails.
         :return: A boolean that if True indicates the causal test case passed and if false indicates the test case
          failed.
         :rtype: bool
@@ -245,15 +248,15 @@
             if f_flag:
                 raise StatisticsError(
                     f"{causal_test_case}\n    FAILED - expected {causal_test_case.expected_causal_effect}, "
                     f"got {result_string}"
                 )
             failed = True
             logger.warning("   FAILED- expected %s, got %s", causal_test_case.expected_causal_effect, result_string)
-        return failed
+        return failed, causal_test_result
 
     def _setup_test(
         self, causal_test_case: CausalTestCase, test: Mapping, conditions: list[str] = None
     ) -> tuple[CausalTestEngine, Estimator]:
         """Create the necessary inputs for a single test case
         :param causal_test_case: The concrete test case to be executed
         :param test: Single JSON test definition stored in a mapping (dict)
```

### Comparing `causal_testing_framework-4.0.1/causal_testing/specification/causal_dag.py` & `causal_testing_framework-4.1.0/causal_testing/specification/causal_dag.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/causal_testing/specification/causal_specification.py` & `causal_testing_framework-4.1.0/causal_testing/specification/causal_specification.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/causal_testing/specification/metamorphic_relation.py` & `causal_testing_framework-4.1.0/causal_testing/specification/metamorphic_relation.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/causal_testing/specification/scenario.py` & `causal_testing_framework-4.1.0/causal_testing/specification/scenario.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/causal_testing/specification/variable.py` & `causal_testing_framework-4.1.0/causal_testing/specification/variable.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/causal_testing/testing/base_test_case.py` & `causal_testing_framework-4.1.0/causal_testing/testing/base_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/causal_testing/testing/causal_test_case.py` & `causal_testing_framework-4.1.0/causal_testing/testing/causal_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/causal_testing/testing/causal_test_engine.py` & `causal_testing_framework-4.1.0/causal_testing/testing/causal_test_engine.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/causal_testing/testing/causal_test_outcome.py` & `causal_testing_framework-4.1.0/causal_testing/testing/causal_test_outcome.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/causal_testing/testing/causal_test_result.py` & `causal_testing_framework-4.1.0/causal_testing/testing/causal_test_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """This module contains the CausalTestResult class, which is a container for the results of a causal test, and the
 TestValue dataclass.
 """
 from typing import Any
 from dataclasses import dataclass
+import pandas as pd
 
 from causal_testing.testing.estimators import Estimator
 from causal_testing.specification.variable import Variable
 
 
 @dataclass
 class TestValue:
@@ -83,16 +84,16 @@
         """Return the higher bracket of the confidence intervals."""
         if self.confidence_intervals and all(self.confidence_intervals):
             return max(self.confidence_intervals)
         return None
 
     def ci_valid(self) -> bool:
         """Return whether or not the result has valid confidence invervals"""
-        return self.ci_low() and self.ci_high()
+        return self.ci_low() and (not pd.isnull(self.ci_low())) and self.ci_high() and (not pd.isnull(self.ci_high()))
 
     def summary(self):
         """Summarise the causal test result as an intuitive sentence."""
         print(
-            f"The causal effect of changing {self.estimator.treatment[0]} = {self.estimator.control_value} to "
-            f"{self.estimator.treatment[0]}' = {self.estimator.treatment_value} is {self.test_value.value}"
+            f"The causal effect of changing {self.estimator.treatment} = {self.estimator.control_value} to "
+            f"{self.estimator.treatment}' = {self.estimator.treatment_value} is {self.test_value.value}"
             f"(95% confidence intervals: {self.confidence_intervals})."
         )
```

### Comparing `causal_testing_framework-4.0.1/causal_testing/testing/causal_test_suite.py` & `causal_testing_framework-4.1.0/causal_testing/testing/causal_test_suite.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/causal_testing/testing/estimators.py` & `causal_testing_framework-4.1.0/causal_testing/testing/estimators.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/causal_testing/testing/intervention.py` & `causal_testing_framework-4.1.0/causal_testing/testing/intervention.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/causal_testing/testing/validation.py` & `causal_testing_framework-4.1.0/causal_testing/testing/validation.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/causal_testing_framework.egg-info/PKG-INFO` & `causal_testing_framework-4.1.0/causal_testing_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causal-testing-framework
-Version: 4.0.1
+Version: 4.1.0
 Summary: A framework for causal testing using causal directed acyclic graphs.
 Author: The CITCOM team
 License: MIT
 Project-URL: Bug_Tracker, https://github.com/CITCOM-project/CausalTestingFramework/issues
 Project-URL: Documentation, https://causal-testing-framework.readthedocs.io/
 Project-URL: Source, https://github.com/CITCOM-project/CausalTestingFramework
 Keywords: causal inference,verification
```

### Comparing `causal_testing_framework-4.0.1/causal_testing_framework.egg-info/SOURCES.txt` & `causal_testing_framework-4.1.0/causal_testing_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/docs/Makefile` & `causal_testing_framework-4.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/docs/README.md` & `causal_testing_framework-4.1.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/docs/make.bat` & `causal_testing_framework-4.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/docs/source/conf.py` & `causal_testing_framework-4.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/docs/source/description.rst` & `causal_testing_framework-4.1.0/docs/source/description.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/docs/source/frontends/json_front_end.rst` & `causal_testing_framework-4.1.0/docs/source/frontends/json_front_end.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/docs/source/frontends/test_suite.rst` & `causal_testing_framework-4.1.0/docs/source/frontends/test_suite.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/docs/source/images/workflow.png` & `causal_testing_framework-4.1.0/docs/source/images/workflow.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/docs/source/index.rst` & `causal_testing_framework-4.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/docs/source/installation.rst` & `causal_testing_framework-4.1.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/docs/source/modules/causal_specification.rst` & `causal_testing_framework-4.1.0/docs/source/modules/causal_specification.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/docs/source/modules/causal_tests.rst` & `causal_testing_framework-4.1.0/docs/source/modules/causal_tests.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/docs/source/modules/data_collector.rst` & `causal_testing_framework-4.1.0/docs/source/modules/data_collector.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/docs/source/usage.rst` & `causal_testing_framework-4.1.0/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/covasim_/doubling_beta/README.md` & `causal_testing_framework-4.1.0/examples/covasim_/doubling_beta/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/covasim_/doubling_beta/dag.png` & `causal_testing_framework-4.1.0/examples/covasim_/doubling_beta/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/covasim_/doubling_beta/data/10k_observational_data.csv` & `causal_testing_framework-4.1.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/covasim_/doubling_beta/example_beta.py` & `causal_testing_framework-4.1.0/examples/covasim_/doubling_beta/example_beta.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/covasim_/vaccinating_elderly/README.md` & `causal_testing_framework-4.1.0/examples/covasim_/vaccinating_elderly/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/covasim_/vaccinating_elderly/dag.png` & `causal_testing_framework-4.1.0/examples/covasim_/vaccinating_elderly/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/covasim_/vaccinating_elderly/example_vaccine.py` & `causal_testing_framework-4.1.0/examples/covasim_/vaccinating_elderly/example_vaccine.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/lr91/README.md` & `causal_testing_framework-4.1.0/examples/lr91/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/lr91/dag.dot` & `causal_testing_framework-4.1.0/examples/lr91/dag.dot`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/lr91/dag.png` & `causal_testing_framework-4.1.0/examples/lr91/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/lr91/data/normalised_results.csv` & `causal_testing_framework-4.1.0/examples/lr91/data/normalised_results.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/lr91/data/results.csv` & `causal_testing_framework-4.1.0/examples/lr91/data/results.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/lr91/example_max_conductances.py` & `causal_testing_framework-4.1.0/examples/lr91/example_max_conductances.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/lr91/example_max_conductances_test_suite.py` & `causal_testing_framework-4.1.0/examples/lr91/example_max_conductances_test_suite.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/poisson/README.md` & `causal_testing_framework-4.1.0/examples/poisson/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/poisson/causal_tests.json` & `causal_testing_framework-4.1.0/examples/poisson/causal_tests.json`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/poisson/dag.dot` & `causal_testing_framework-4.1.0/examples/poisson/dag.dot`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/poisson/data.csv` & `causal_testing_framework-4.1.0/examples/poisson/data.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/poisson/example_run_causal_tests.py` & `causal_testing_framework-4.1.0/examples/poisson/example_run_causal_tests.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/poisson-line-process/README.md` & `causal_testing_framework-4.1.0/examples/poisson-line-process/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/poisson-line-process/dag.png` & `causal_testing_framework-4.1.0/examples/poisson-line-process/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/poisson-line-process/data/random/data_random_1000.csv` & `causal_testing_framework-4.1.0/examples/poisson-line-process/data/random/data_random_1000.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv` & `causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv` & `causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv` & `causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv` & `causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv` & `causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv` & `causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv` & `causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv` & `causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv` & `causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv` & `causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/examples/poisson-line-process/example_poisson_process.py` & `causal_testing_framework-4.1.0/examples/poisson-line-process/example_poisson_process.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/images/workflow.png` & `causal_testing_framework-4.1.0/images/workflow.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/pyproject.toml` & `causal_testing_framework-4.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/tests/data/nhefs.csv` & `causal_testing_framework-4.1.0/tests/data/nhefs.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/tests/data_collection_tests/test_observational_data_collector.py` & `causal_testing_framework-4.1.0/tests/data_collection_tests/test_observational_data_collector.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/tests/generation_tests/test_abstract_test_case.py` & `causal_testing_framework-4.1.0/tests/generation_tests/test_abstract_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/tests/json_front_tests/test_json_class.py` & `causal_testing_framework-4.1.0/tests/json_front_tests/test_json_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         estimators = {"LinearRegressionEstimator": LinearRegressionEstimator}
 
         self.json_class.run_json_tests(effects=effects, mutates={}, estimators=estimators, f_flag=False)
 
         # Test that the final log message prints that failed tests are printed, which is expected behaviour for this scenario
         with open("temp_out.txt", "r") as reader:
             temp_out = reader.readlines()
-        self.assertIn("failed", temp_out[-1])
+        self.assertIn("FAILED", temp_out[-1])
 
     def test_run_json_tests_from_json(self):
         example_test = {
             "tests": [
                 {
                     "name": "test1",
                     "mutations": {"test_input": "Increase"},
@@ -230,15 +230,15 @@
         self.json_class.test_plan = example_test
         effects = {"NoEffect": NoEffect()}
         estimators = {"LinearRegressionEstimator": LinearRegressionEstimator}
 
         self.json_class.run_json_tests(effects=effects, estimators=estimators, f_flag=False)
         with open("temp_out.txt", "r") as reader:
             temp_out = reader.readlines()
-        self.assertIn("failed", temp_out[-1])
+        self.assertIn("FAILED", temp_out[-1])
 
     def tearDown(self) -> None:
         remove_temp_dir_if_existent()
 
 
 def populate_example(*args, **kwargs):
     pass
```

### Comparing `causal_testing_framework-4.0.1/tests/specification_tests/test_causal_dag.py` & `causal_testing_framework-4.1.0/tests/specification_tests/test_causal_dag.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/tests/specification_tests/test_metamorphic_relations.py` & `causal_testing_framework-4.1.0/tests/specification_tests/test_metamorphic_relations.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/tests/specification_tests/test_variable.py` & `causal_testing_framework-4.1.0/tests/specification_tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/tests/test_helpers.py` & `causal_testing_framework-4.1.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/tests/testing_tests/test_causal_test_case.py` & `causal_testing_framework-4.1.0/tests/testing_tests/test_causal_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/tests/testing_tests/test_causal_test_engine.py` & `causal_testing_framework-4.1.0/tests/testing_tests/test_causal_test_engine.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/tests/testing_tests/test_causal_test_outcome.py` & `causal_testing_framework-4.1.0/tests/testing_tests/test_causal_test_outcome.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/tests/testing_tests/test_causal_test_suite.py` & `causal_testing_framework-4.1.0/tests/testing_tests/test_causal_test_suite.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.0.1/tests/testing_tests/test_estimators.py` & `causal_testing_framework-4.1.0/tests/testing_tests/test_estimators.py`

 * *Files identical despite different names*

