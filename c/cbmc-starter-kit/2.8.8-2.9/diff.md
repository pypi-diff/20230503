# Comparing `tmp/cbmc-starter-kit-2.8.8.tar.gz` & `tmp/cbmc-starter-kit-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbmc-starter-kit-2.8.8.tar", last modified: Wed Dec 21 23:08:51 2022, max compression
+gzip compressed data, was "cbmc-starter-kit-2.9.tar", last modified: Tue Feb 14 18:56:23 2023, max compression
```

## Comparing `cbmc-starter-kit-2.8.8.tar` & `cbmc-starter-kit-2.9.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.389377 cbmc-starter-kit-2.8.8/
--rw-r--r--   0 runner    (1001) docker     (122)      926 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       67 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/NOTICE
--rw-r--r--   0 runner    (1001) docker     (122)     2683 2022-12-21 23:08:51.389377 cbmc-starter-kit-2.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2124 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      192 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1465 2022-12-21 23:08:51.389377 cbmc-starter-kit-2.8.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.377377 cbmc-starter-kit-2.8.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.381377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1696 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/arguments.py
--rw-r--r--   0 runner    (1001) docker     (122)     6392 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/ctagst.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.377377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/etc/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.381377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/etc/bash_completion.d/
--rw-r--r--   0 runner    (1001) docker     (122)     1413 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/etc/bash_completion.d/cbmc-starter-kit.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)     5149 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/migrate_license.py
--rw-r--r--   0 runner    (1001) docker     (122)     6091 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/repository.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3567 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6035 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/setup_ci.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2929 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/setup_proof.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.381377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-ci-workflow/
--rw-r--r--   0 runner    (1001) docker     (122)     7802 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-ci-workflow/proof_ci.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.381377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-ci-workflow/proof_ci_resources/
--rw-r--r--   0 runner    (1001) docker     (122)      252 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-ci-workflow/proof_ci_resources/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.385377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-proof/
--rw-r--r--   0 runner    (1001) docker     (122)      582 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-proof/FUNCTION_harness.c
--rw-r--r--   0 runner    (1001) docker     (122)     1607 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-proof/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      462 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-proof/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-proof/cbmc-proof.txt
--rw-r--r--   0 runner    (1001) docker     (122)      126 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-proof/cbmc-viewer.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.385377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/
--rw-r--r--   0 runner    (1001) docker     (122)      299 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.385377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/include/
--rw-r--r--   0 runner    (1001) docker     (122)      233 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/include/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.385377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/
--rw-r--r--   0 runner    (1001) docker     (122)      563 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.385377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/assert/
--rw-r--r--   0 runner    (1001) docker     (122)      286 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/assert/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      259 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/assert/assert_harness.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.385377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/bounds_check/
--rw-r--r--   0 runner    (1001) docker     (122)      292 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/bounds_check/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      290 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/bounds_check/bounds_check_harness.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.385377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/conversion_check/
--rw-r--r--   0 runner    (1001) docker     (122)      296 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/conversion_check/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      268 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/conversion_check/conversion_check_harness.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.385377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/div_by_zero_check/
--rw-r--r--   0 runner    (1001) docker     (122)      297 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/div_by_zero_check/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      250 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/div_by_zero_check/div_by_zero_check_harness.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.385377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/float_overflow_check/
--rw-r--r--   0 runner    (1001) docker     (122)      300 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/float_overflow_check/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      271 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/float_overflow_check/float_overflow_check_harness.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.385377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/float_underflow_check/
--rw-r--r--   0 runner    (1001) docker     (122)      301 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/float_underflow_check/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      274 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/float_underflow_check/float_underflow_check_harness.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.385377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/nan_check/
--rw-r--r--   0 runner    (1001) docker     (122)      289 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/nan_check/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      227 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/nan_check/nan_check_harness.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.385377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/pointer_check/
--rw-r--r--   0 runner    (1001) docker     (122)      293 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/pointer_check/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      234 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/pointer_check/pointer_check_harness.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.385377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/pointer_overflow_check/
--rw-r--r--   0 runner    (1001) docker     (122)      302 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/pointer_overflow_check/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      299 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/pointer_overflow_check/pointer_overflow_check_harness.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.385377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/pointer_primitive_check/
--rw-r--r--   0 runner    (1001) docker     (122)      344 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/pointer_primitive_check/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      279 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/pointer_primitive_check/pointer_primitive_check_harness.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.385377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/pointer_underflow_check/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/pointer_underflow_check/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      300 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/pointer_underflow_check/pointer_underflow_check_harness.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.385377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/signed_overflow_check/
--rw-r--r--   0 runner    (1001) docker     (122)      301 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/signed_overflow_check/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      265 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/signed_overflow_check/signed_overflow_check_harness.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.385377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/signed_underflow_check/
--rw-r--r--   0 runner    (1001) docker     (122)      302 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/signed_underflow_check/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      268 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/signed_underflow_check/signed_underflow_check_harness.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.385377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/undefined_shift_check/
--rw-r--r--   0 runner    (1001) docker     (122)      301 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/undefined_shift_check/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      289 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/undefined_shift_check/undefined_shift_check_harness.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.385377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/unsigned_overflow_check/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/unsigned_overflow_check/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      274 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/unsigned_overflow_check/unsigned_overflow_check_harness.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.385377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/unsigned_underflow_check/
--rw-r--r--   0 runner    (1001) docker     (122)      304 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/unsigned_underflow_check/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      277 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/unsigned_underflow_check/unsigned_underflow_check_harness.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.389377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/proofs/
--rw-r--r--   0 runner    (1001) docker     (122)     1213 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/proofs/Makefile-project-defines
--rw-r--r--   0 runner    (1001) docker     (122)      336 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/proofs/Makefile-project-targets
--rw-r--r--   0 runner    (1001) docker     (122)      379 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/proofs/Makefile-project-testing
--rw-r--r--   0 runner    (1001) docker     (122)    35667 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/proofs/Makefile.common
--rw-r--r--   0 runner    (1001) docker     (122)     1149 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/proofs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.389377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/proofs/lib/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/proofs/lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1898 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/proofs/lib/print_tool_versions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3743 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/proofs/lib/summarize.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    14301 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/proofs/run-cbmc-proofs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.389377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/sources/
--rw-r--r--   0 runner    (1001) docker     (122)      209 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/sources/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.389377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/stubs/
--rw-r--r--   0 runner    (1001) docker     (122)      245 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/stubs/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     5156 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/update.py
--rw-r--r--   0 runner    (1001) docker     (122)     3982 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/util.py
--rw-r--r--   0 runner    (1001) docker     (122)      601 2022-12-21 23:08:37.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 23:08:51.381377 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2683 2022-12-21 23:08:51.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5261 2022-12-21 23:08:51.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-21 23:08:51.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      250 2022-12-21 23:08:51.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2022-12-21 23:08:51.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2022-12-21 23:08:51.000000 cbmc-starter-kit-2.8.8/src/cbmc_starter_kit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.223044 cbmc-starter-kit-2.9/
+-rw-r--r--   0 runner    (1001) docker     (122)      926 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)     2681 2023-02-14 18:56:23.223044 cbmc-starter-kit-2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2124 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1463 2023-02-14 18:56:23.223044 cbmc-starter-kit-2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.207042 cbmc-starter-kit-2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.215043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1696 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/ctagst.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.211043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/etc/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.215043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/etc/bash_completion.d/
+-rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/etc/bash_completion.d/cbmc-starter-kit.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5149 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/migrate_license.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6091 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/repository.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3567 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6094 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/setup_ci.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2929 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/setup_proof.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.215043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-ci-workflow/
+-rw-r--r--   0 runner    (1001) docker     (122)     7949 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-ci-workflow/proof_ci.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.215043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-ci-workflow/proof_ci_resources/
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-ci-workflow/proof_ci_resources/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.215043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-proof/
+-rw-r--r--   0 runner    (1001) docker     (122)      582 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-proof/FUNCTION_harness.c
+-rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-proof/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-proof/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-proof/cbmc-proof.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-proof/cbmc-viewer.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.215043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.215043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/include/
+-rw-r--r--   0 runner    (1001) docker     (122)      233 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/include/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.215043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      563 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.215043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/assert/
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/assert/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/assert/assert_harness.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.215043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/bounds_check/
+-rw-r--r--   0 runner    (1001) docker     (122)      292 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/bounds_check/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      290 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/bounds_check/bounds_check_harness.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.219043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/conversion_check/
+-rw-r--r--   0 runner    (1001) docker     (122)      296 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/conversion_check/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/conversion_check/conversion_check_harness.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.219043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/div_by_zero_check/
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/div_by_zero_check/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      250 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/div_by_zero_check/div_by_zero_check_harness.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.219043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/float_overflow_check/
+-rw-r--r--   0 runner    (1001) docker     (122)      300 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/float_overflow_check/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      271 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/float_overflow_check/float_overflow_check_harness.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.219043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/float_underflow_check/
+-rw-r--r--   0 runner    (1001) docker     (122)      301 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/float_underflow_check/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/float_underflow_check/float_underflow_check_harness.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.219043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/nan_check/
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/nan_check/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/nan_check/nan_check_harness.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.219043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/pointer_check/
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/pointer_check/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/pointer_check/pointer_check_harness.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.219043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/pointer_overflow_check/
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/pointer_overflow_check/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/pointer_overflow_check/pointer_overflow_check_harness.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.219043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/pointer_primitive_check/
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/pointer_primitive_check/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      279 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/pointer_primitive_check/pointer_primitive_check_harness.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.219043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/pointer_underflow_check/
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/pointer_underflow_check/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      300 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/pointer_underflow_check/pointer_underflow_check_harness.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.219043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/signed_overflow_check/
+-rw-r--r--   0 runner    (1001) docker     (122)      301 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/signed_overflow_check/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/signed_overflow_check/signed_overflow_check_harness.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.219043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/signed_underflow_check/
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/signed_underflow_check/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/signed_underflow_check/signed_underflow_check_harness.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.219043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/undefined_shift_check/
+-rw-r--r--   0 runner    (1001) docker     (122)      301 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/undefined_shift_check/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/undefined_shift_check/undefined_shift_check_harness.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.219043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/unsigned_overflow_check/
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/unsigned_overflow_check/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/unsigned_overflow_check/unsigned_overflow_check_harness.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.219043 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/unsigned_underflow_check/
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/unsigned_underflow_check/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/unsigned_underflow_check/unsigned_underflow_check_harness.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.223044 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/proofs/
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/proofs/Makefile-project-defines
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/proofs/Makefile-project-targets
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/proofs/Makefile-project-testing
+-rw-r--r--   0 runner    (1001) docker     (122)    35733 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/proofs/Makefile.common
+-rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/proofs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.223044 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/proofs/lib/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/proofs/lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1898 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/proofs/lib/print_tool_versions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4512 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/proofs/lib/summarize.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    14301 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/proofs/run-cbmc-proofs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.223044 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/sources/
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/sources/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.223044 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/stubs/
+-rw-r--r--   0 runner    (1001) docker     (122)      245 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/stubs/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     5474 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)      960 2023-02-14 18:56:07.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 18:56:23.215043 cbmc-starter-kit-2.9/src/cbmc_starter_kit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2681 2023-02-14 18:56:23.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5261 2023-02-14 18:56:23.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-14 18:56:23.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      250 2023-02-14 18:56:23.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-02-14 18:56:23.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-02-14 18:56:23.000000 cbmc-starter-kit-2.9/src/cbmc_starter_kit.egg-info/top_level.txt
```

### Comparing `cbmc-starter-kit-2.8.8/LICENSE` & `cbmc-starter-kit-2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cbmc-starter-kit-2.8.8/PKG-INFO` & `cbmc-starter-kit-2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbmc-starter-kit
-Version: 2.8.8
+Version: 2.9
 Summary: CBMC starter kit makes it easy to add CBMC verification to a software project
 Home-page: https://github.com/model-checking/cbmc-starter-kit
 Author: Mark R. Tuttle
 Author-email: mrtuttle@amazon.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `cbmc-starter-kit-2.8.8/README.md` & `cbmc-starter-kit-2.9/README.md`

 * *Files identical despite different names*

### Comparing `cbmc-starter-kit-2.8.8/setup.cfg` & `cbmc-starter-kit-2.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cbmc-starter-kit
-version = 2.8.8
+version = 2.9
 author = Mark R. Tuttle
 author_email = mrtuttle@amazon.com
 description = CBMC starter kit makes it easy to add CBMC verification to a software project
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/model-checking/cbmc-starter-kit
 license = Apache License 2.0
```

### Comparing `cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/arguments.py` & `cbmc-starter-kit-2.9/src/cbmc_starter_kit/arguments.py`

 * *Files identical despite different names*

### Comparing `cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/ctagst.py` & `cbmc-starter-kit-2.9/src/cbmc_starter_kit/ctagst.py`

 * *Files identical despite different names*

### Comparing `cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/etc/bash_completion.d/cbmc-starter-kit.sh` & `cbmc-starter-kit-2.9/src/cbmc_starter_kit/etc/bash_completion.d/cbmc-starter-kit.sh`

 * *Files identical despite different names*

### Comparing `cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/migrate_license.py` & `cbmc-starter-kit-2.9/src/cbmc_starter_kit/migrate_license.py`

 * *Files identical despite different names*

### Comparing `cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/repository.py` & `cbmc-starter-kit-2.9/src/cbmc_starter_kit/repository.py`

 * *Files identical despite different names*

### Comparing `cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/setup.py` & `cbmc-starter-kit-2.9/src/cbmc_starter_kit/setup.py`

 * *Files identical despite different names*

### Comparing `cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/setup_ci.py` & `cbmc-starter-kit-2.9/src/cbmc_starter_kit/setup_ci.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """Set up the AWS infrastructure to run proofs in CI."""
 
 import logging
 import shutil
 from argparse import RawDescriptionHelpFormatter
 
 
-from cbmc_starter_kit import arguments, repository, util
+from cbmc_starter_kit import arguments, repository, util, version
 
 ################################################################
 
 def parse_arguments():
     """Parse arguments for cbmc-starter-kit-setup-ci command"""
     desc = """
     Copy a GitHub Action workflow to `.github/workflows` in this repository,
@@ -149,13 +149,14 @@
     shutil.copytree(
         util.package_ci_workflow_template_root(),
         workflows_root,
         dirs_exist_ok=True)
 
     patch_proof_ci_config(config, args)
     patch_proof_ci_workflow(workflow, args.github_actions_runner)
+    version.copy_with_version(workflow, workflow)
 
     repo_root = repository.repository_root()
     copy_lib_directory(repo_root)
 
 if __name__ == "__main__":
     main()
```

### Comparing `cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/setup_proof.py` & `cbmc-starter-kit-2.9/src/cbmc_starter_kit/setup_proof.py`

 * *Files identical despite different names*

### Comparing `cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-ci-workflow/proof_ci.yaml` & `cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-ci-workflow/proof_ci.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: MIT-0
+# _CBMC_STARTER_KIT_VERSION_
 name: Run CBMC proofs
 on:
   push:
     branches-ignore:
       - gh-pages
+  pull_request:
+    branches-ignore:
+      - gh-pages
+  workflow_dispatch:
 
 # USAGE
 #
 # If you need to use different versions for tools like CBMC, modify this file:
 # .github/workflows/proof_ci_resources/config.yaml
 #
 # If you want the CI to use a different GitHub-hosted runner (which must still
@@ -147,35 +152,37 @@
           echo "$(pwd)" >> $GITHUB_PATH
       - name: Run CBMC proofs
         shell: bash
         env:
           EXTERNAL_SAT_SOLVER: kissat
         working-directory: ${{ env.PROOFS_DIR }}
         run: ${{ env.RUN_CBMC_PROOFS_COMMAND }}
+      - name: Check repository visibility
+        shell: bash
+        run: |
+          VIZ="${{ fromJson(toJson(github.event.repository)).visibility }}";
+          echo "REPO_VISIBILITY=${VIZ}" | tee -a "${GITHUB_ENV}";
       - name: Set name for zip artifact with CBMC proof results
         id: artifact
-        if: ${{ env.AWS_CLOUDFRONT_DOMAIN == '' }}
+        if: ${{ env.REPO_VISIBILITY == 'public' }}
         run: |
           echo "name=cbmc_proof_results_${{ fromJson(toJson(github.event.repository)).name }}_$(date +%Y_%m_%d_%H_%M_%S)" >> $GITHUB_OUTPUT
       - name: Create zip artifact with CBMC proof results
-        if: ${{ env.AWS_CLOUDFRONT_DOMAIN == '' }}
+        if: ${{ env.REPO_VISIBILITY == 'public' }}
         shell: bash
         run: |
           FINAL_REPORT_DIR=$PROOFS_DIR/output/latest/html
           pushd $FINAL_REPORT_DIR \
             && zip -r ${{ steps.artifact.outputs.name }}.zip . \
             && popd \
             && mv $FINAL_REPORT_DIR/${{ steps.artifact.outputs.name }}.zip .
       - name: Upload zip artifact of CBMC proof results to GitHub Actions
-        if: ${{ env.AWS_CLOUDFRONT_DOMAIN == '' }}
+        if: ${{ env.REPO_VISIBILITY == 'public' }}
         uses: actions/upload-artifact@v3
         with:
           name: ${{ steps.artifact.outputs.name }}
           path: ${{ steps.artifact.outputs.name }}.zip
       - name: CBMC proof results
         shell: bash
         run: |
           python3 ${{ env.PROOFS_DIR }}/lib/summarize.py \
-            --run-file ${{ env.PROOFS_DIR }}/output/latest/html/run.json > summary.md
-          cat summary.md >> $GITHUB_STEP_SUMMARY
-          cat summary.md
-          cat summary.md | [[ $(grep -cim1 -e "fail" -e "in progress") -eq 0 ]] ; echo $?
+            --run-file ${{ env.PROOFS_DIR }}/output/latest/html/run.json
```

### Comparing `cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-proof/FUNCTION_harness.c` & `cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-proof/FUNCTION_harness.c`

 * *Files identical despite different names*

### Comparing `cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-proof/Makefile` & `cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-proof/Makefile`

 * *Files identical despite different names*

### Comparing `cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/negative_tests/README.md` & `cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/negative_tests/README.md`

 * *Files identical despite different names*

### Comparing `cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/proofs/Makefile-project-defines` & `cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/proofs/Makefile-project-defines`

 * *Files identical despite different names*

### Comparing `cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/proofs/Makefile.common` & `cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/proofs/Makefile.common`

 * *Files 2% similar despite different names*

```diff
@@ -600,74 +600,74 @@
 	  --ci-stage build \
 	  --description "$(PROOF_UID): removing static"
 
 ################################################################
 # Build targets that make the relevant .goto files
 
 # Compile project sources
-$(PROJECT_GOTO)1.goto: $(PROJECT_SOURCES) $(REWRITTEN_SOURCES)
+$(PROJECT_GOTO)0100.goto: $(PROJECT_SOURCES) $(REWRITTEN_SOURCES)
 	$(LITANI) add-job \
 	  --command \
 	    '$(GOTO_CC) $(CBMC_VERBOSITY) $(COMPILE_FLAGS) $(EXPORT_FILE_LOCAL_SYMBOLS) $(INCLUDES) $(DEFINES) $^ -o $@' \
 	  --inputs $^ \
 	  --outputs $@ \
 	  --stdout-file $(LOGDIR)/project_sources-log.txt \
 	  --pipeline-name "$(PROOF_UID)" \
 	  --ci-stage build \
 	  --description "$(PROOF_UID): building project binary"
 
 # Compile proof sources
-$(PROOF_GOTO)1.goto: $(PROOF_SOURCES)
+$(PROOF_GOTO)0100.goto: $(PROOF_SOURCES)
 	$(LITANI) add-job \
 	  --command \
 	    '$(GOTO_CC) $(CBMC_VERBOSITY) $(COMPILE_FLAGS) $(EXPORT_FILE_LOCAL_SYMBOLS) $(INCLUDES) $(DEFINES) $^ -o $@' \
 	  --inputs $^ \
 	  --outputs $@ \
 	  --stdout-file $(LOGDIR)/proof_sources-log.txt \
 	  --pipeline-name "$(PROOF_UID)" \
 	  --ci-stage build \
 	  --description "$(PROOF_UID): building proof binary"
 
 # Remove function bodies from project sources
-$(PROJECT_GOTO)2.goto: $(PROJECT_GOTO)1.goto
+$(PROJECT_GOTO)0200.goto: $(PROJECT_GOTO)0100.goto
 	$(LITANI) add-job \
 	  --command \
 	    '$(GOTO_INSTRUMENT) $(CBMC_VERBOSITY) $(CBMC_REMOVE_FUNCTION_BODY) $^ $@' \
 	  --inputs $^ \
 	  --outputs $@ \
 	  --stdout-file $(LOGDIR)/remove_function_body-log.txt \
 	  --pipeline-name "$(PROOF_UID)" \
 	  --ci-stage build \
 	  --description "$(PROOF_UID): removing function bodies from project sources"
 
 # Link project and proof sources into the proof harness
-$(HARNESS_GOTO)1.goto: $(PROOF_GOTO)1.goto $(PROJECT_GOTO)2.goto
+$(HARNESS_GOTO)0100.goto: $(PROOF_GOTO)0100.goto $(PROJECT_GOTO)0200.goto
 	$(LITANI) add-job \
 	  --command '$(GOTO_CC) $(CBMC_VERBOSITY) --function $(HARNESS_ENTRY) $^ $(LINK_FLAGS) -o $@' \
 	  --inputs $^ \
 	  --outputs $@ \
 	  --stdout-file $(LOGDIR)/link_proof_project-log.txt \
 	  --pipeline-name "$(PROOF_UID)" \
 	  --ci-stage build \
 	  --description "$(PROOF_UID): linking project to proof"
 
 # Restrict function pointers
-$(HARNESS_GOTO)2.goto: $(HARNESS_GOTO)1.goto
+$(HARNESS_GOTO)0200.goto: $(HARNESS_GOTO)0100.goto
 	$(LITANI) add-job \
 	  --command \
 	    '$(GOTO_INSTRUMENT) $(CBMC_VERBOSITY) $(CBMC_RESTRICT_FUNCTION_POINTER) --remove-function-pointers $^ $@' \
 	  --inputs $^ \
 	  --outputs $@ \
 	  --stdout-file $(LOGDIR)/restrict_function_pointer-log.txt \
 	  --pipeline-name "$(PROOF_UID)" \
 	  --ci-stage build \
 	  --description "$(PROOF_UID): restricting function pointers in project sources"
 
 # Fill static variable with unconstrained values
-$(HARNESS_GOTO)3.goto: $(HARNESS_GOTO)2.goto
+$(HARNESS_GOTO)0300.goto: $(HARNESS_GOTO)0200.goto
 ifneq ($(strip $(CODE_CONTRACTS)),)
 	$(LITANI) add-job \
 	  --command 'cp $^ $@' \
 	  --inputs $^ \
 	  --outputs $@ \
 	  --stdout-file $(LOGDIR)/nondet_static-log.txt \
 	  --pipeline-name "$(PROOF_UID)" \
@@ -682,15 +682,15 @@
 	  --stdout-file $(LOGDIR)/nondet_static-log.txt \
 	  --pipeline-name "$(PROOF_UID)" \
 	  --ci-stage build \
 	  --description "$(PROOF_UID): setting static variables to nondet"
 endif
 
 # Link CPROVER library if DFCC mode is on
-$(HARNESS_GOTO)4.goto: $(HARNESS_GOTO)3.goto
+$(HARNESS_GOTO)0400.goto: $(HARNESS_GOTO)0300.goto
 ifneq ($(strip $(USE_DYNAMIC_FRAMES)),)
 	$(LITANI) add-job \
 	  --command \
 	    '$(GOTO_INSTRUMENT) $(CBMC_VERBOSITY) $(ADD_LIBRARY_FLAG) $(CBMC_OPT_CONFIG_LIBRARY) $^ $@' \
 	  --inputs $^ \
 	  --outputs $@ \
 	  --stdout-file $(LOGDIR)/linking-library-models-log.txt \
@@ -705,15 +705,15 @@
 	  --stdout-file $(LOGDIR)/linking-library-models-log.txt \
 	  --pipeline-name "$(PROOF_UID)" \
 	  --ci-stage build \
 	  --description "$(PROOF_UID): not linking CPROVER library"
 endif
 
 # Early unwind all loops on DFCC mode; otherwise, only unwind loops in proof and project code
-$(HARNESS_GOTO)5.goto: $(HARNESS_GOTO)4.goto
+$(HARNESS_GOTO)0500.goto: $(HARNESS_GOTO)0400.goto
 ifneq ($(strip $(USE_DYNAMIC_FRAMES)),)
 	$(LITANI) add-job \
 	  --command \
 	    '$(GOTO_INSTRUMENT) $(CBMC_VERBOSITY) $(CBMC_UNWINDSET) $(CBMC_CPROVER_LIBRARY_UNWINDSET) $(CBMC_DEFAULT_UNWIND) $(CBMC_FLAG_UNWINDING_ASSERTIONS) $^ $@' \
 	  --inputs $^ \
 	  --outputs $@ \
 	  --stdout-file $(LOGDIR)/unwind_loops-log.txt \
@@ -738,51 +738,51 @@
 	  --stdout-file $(LOGDIR)/linking-library-models-log.txt \
 	  --pipeline-name "$(PROOF_UID)" \
 	  --ci-stage build \
 	  --description "$(PROOF_UID): not unwinding loops"
 endif
 
 # Replace function contracts, check function contracts, instrument for loop contracts
-$(HARNESS_GOTO)6.goto: $(HARNESS_GOTO)5.goto
+$(HARNESS_GOTO)0600.goto: $(HARNESS_GOTO)0500.goto
 	$(LITANI) add-job \
 	  --command \
 	    '$(GOTO_INSTRUMENT) $(CBMC_USE_DYNAMIC_FRAMES) $(NONDET_STATIC) $(CBMC_VERBOSITY) $(CBMC_CHECK_FUNCTION_CONTRACTS) $(CBMC_USE_FUNCTION_CONTRACTS) $(CBMC_APPLY_LOOP_CONTRACTS) $^ $@' \
 	  --inputs $^ \
 	  --outputs $@ \
 	  --stdout-file $(LOGDIR)/check_function_contracts-log.txt \
 	  --pipeline-name "$(PROOF_UID)" \
 	  --ci-stage build \
 	  --description "$(PROOF_UID): checking function contracts"
 
 # Omit initialization of unused global variables (reduces problem size)
-$(HARNESS_GOTO)7.goto: $(HARNESS_GOTO)6.goto
+$(HARNESS_GOTO)0700.goto: $(HARNESS_GOTO)0600.goto
 	$(LITANI) add-job \
 	  --command \
 	    '$(GOTO_INSTRUMENT) $(CBMC_VERBOSITY) --slice-global-inits $^ $@' \
 	  --inputs $^ \
 	  --outputs $@ \
 	  --stdout-file $(LOGDIR)/slice_global_inits-log.txt \
 	  --pipeline-name "$(PROOF_UID)" \
 	  --ci-stage build \
 	  --description "$(PROOF_UID): slicing global initializations"
 
 # Omit unused functions (sharpens coverage calculations)
-$(HARNESS_GOTO)8.goto: $(HARNESS_GOTO)7.goto
+$(HARNESS_GOTO)0800.goto: $(HARNESS_GOTO)0700.goto
 	$(LITANI) add-job \
 	  --command \
 	    '$(GOTO_INSTRUMENT) $(CBMC_VERBOSITY) --drop-unused-functions $^ $@' \
 	  --inputs $^ \
 	  --outputs $@ \
 	  --stdout-file $(LOGDIR)/drop_unused_functions-log.txt \
 	  --pipeline-name "$(PROOF_UID)" \
 	  --ci-stage build \
 	  --description "$(PROOF_UID): dropping unused functions"
 
 # Final name for proof harness
-$(HARNESS_GOTO).goto: $(HARNESS_GOTO)8.goto
+$(HARNESS_GOTO).goto: $(HARNESS_GOTO)0800.goto
 	$(LITANI) add-job \
 	  --command 'cp $< $@' \
 	  --inputs $^ \
 	  --outputs $@ \
 	  --pipeline-name "$(PROOF_UID)" \
 	  --ci-stage build \
 	  --description "$(PROOF_UID): copying final goto-binary"
```

### Comparing `cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/proofs/README.md` & `cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/proofs/README.md`

 * *Files identical despite different names*

### Comparing `cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/proofs/lib/print_tool_versions.py` & `cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/proofs/lib/print_tool_versions.py`

 * *Files identical despite different names*

### Comparing `cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/template-for-repository/proofs/run-cbmc-proofs.py` & `cbmc-starter-kit-2.9/src/cbmc_starter_kit/template-for-repository/proofs/run-cbmc-proofs.py`

 * *Files identical despite different names*

### Comparing `cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/update.py` & `cbmc-starter-kit-2.9/src/cbmc_starter_kit/update.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 
 from pathlib import Path
 import logging
 import platform
 import re
 import shutil
 
-from cbmc_starter_kit import arguments
-from cbmc_starter_kit import util
-from cbmc_starter_kit import version
+from cbmc_starter_kit import arguments, repository, util, version
 
 ################################################################
 
 def parse_arguments():
     desc = 'Update CBMC starter kit in a CBMC proof repository.'
     options = [
         {'flag': '--cbmc-root',
@@ -114,14 +112,21 @@
     if system == "Linux":
         logging.warning("Consider installing the litani command available via "
                         "'apt install litani*.deb'")
         logging.warning("Download the litani Debian package from "
                         "https://github.com/awslabs/aws-build-accumulator/releases/latest")
     return
 
+def check_for_proof_ci_workflow():
+    workflow_root = repository.github_actions_workflows_root()
+    path_to_workflow_in_customer_repo = workflow_root / "proof_ci.yaml"
+    if path_to_workflow_in_customer_repo.exists():
+        version.update_existing_version_in_workflow_file(
+            path_to_workflow_in_customer_repo)
+
 ################################################################
 
 def main():
     """Update files, that were previously added, during installation of the
     CBMC starter kit package."""
 
     args = parse_arguments()
@@ -130,12 +135,14 @@
     args = validate_cbmc_root(args)
 
     if not args.no_test_removal:
         remove_negative_tests(args.cbmc_root)
     if not args.no_update:
         update(args.cbmc_root)
     check_for_litani(args.cbmc_root)
+    check_for_proof_ci_workflow()
+
 
 ################################################################
 
 if __name__ == '__main__':
     main()
```

### Comparing `cbmc-starter-kit-2.8.8/src/cbmc_starter_kit/util.py` & `cbmc-starter-kit-2.9/src/cbmc_starter_kit/util.py`

 * *Files identical despite different names*

### Comparing `cbmc-starter-kit-2.8.8/src/cbmc_starter_kit.egg-info/PKG-INFO` & `cbmc-starter-kit-2.9/src/cbmc_starter_kit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbmc-starter-kit
-Version: 2.8.8
+Version: 2.9
 Summary: CBMC starter kit makes it easy to add CBMC verification to a software project
 Home-page: https://github.com/model-checking/cbmc-starter-kit
 Author: Mark R. Tuttle
 Author-email: mrtuttle@amazon.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `cbmc-starter-kit-2.8.8/src/cbmc_starter_kit.egg-info/SOURCES.txt` & `cbmc-starter-kit-2.9/src/cbmc_starter_kit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

