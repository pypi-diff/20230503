# Comparing `tmp/thermoextrap-0.2.3.tar.gz` & `tmp/thermoextrap-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thermoextrap-0.2.3.tar", last modified: Tue Apr 11 03:03:46 2023, max compression
+gzip compressed data, was "thermoextrap-0.3.0.tar", last modified: Wed May  3 20:15:44 2023, max compression
```

## Comparing `thermoextrap-0.2.3.tar` & `thermoextrap-0.3.0.tar`

### file list

```diff
@@ -1,86 +1,106 @@
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-11 03:03:46.944791 thermoextrap-0.2.3/
--rw-r--r--   0 wpk      (42033)    36681     1869 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/.cruft.json
--rw-r--r--   0 wpk      (42033)    36681     1373 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/.gitignore
--rw-r--r--   0 wpk      (42033)    36681      104 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/.gitmodules
--rw-r--r--   0 wpk      (42033)    36681     2901 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033)    36681      163 2023-04-10 21:01:10.000000 thermoextrap-0.2.3/AUTHORS.md
--rw-r--r--   0 wpk      (42033)    36681     6909 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033)    36681       59 2023-04-10 21:01:10.000000 thermoextrap-0.2.3/HISTORY.md
--rw-r--r--   0 wpk      (42033)    36681     1645 2023-04-10 21:01:10.000000 thermoextrap-0.2.3/LICENSE
--rw-r--r--   0 wpk      (42033)    36681      266 2023-04-11 03:00:42.000000 thermoextrap-0.2.3/MANIFEST.in
--rw-r--r--   0 wpk      (42033)    36681     8464 2023-04-10 21:01:10.000000 thermoextrap-0.2.3/Makefile
--rw-r--r--   0 wpk      (42033)    36681     8307 2023-04-11 03:03:46.945126 thermoextrap-0.2.3/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681     5401 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/README.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-11 03:03:46.912608 thermoextrap-0.2.3/environment/
--rw-r--r--   0 wpk      (42033)    36681       11 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/environment/conda-spec.txt
--rw-r--r--   0 wpk      (42033)    36681     1095 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/environment/dev-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      345 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/environment/dev.yaml
--rw-r--r--   0 wpk      (42033)    36681      120 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033)    36681       87 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033)    36681      692 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      476 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/environment/docs.yaml
--rw-r--r--   0 wpk      (42033)    36681       40 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      262 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/environment/test.yaml
--rw-r--r--   0 wpk      (42033)    36681      343 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/environment.yaml
--rw-r--r--   0 wpk      (42033)    36681     4872 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/pyproject.toml
--rw-r--r--   0 wpk      (42033)    36681      397 2023-04-11 03:03:46.946361 thermoextrap-0.2.3/setup.cfg
--rw-r--r--   0 wpk      (42033)    36681      323 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/setup.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-11 03:03:46.901302 thermoextrap-0.2.3/src/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-11 03:03:46.915495 thermoextrap-0.2.3/src/thermoextrap/
--rw-r--r--   0 wpk      (42033)    36681     1560 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/__init__.py
--rw-r--r--   0 wpk      (42033)    36681    18804 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/src/thermoextrap/adaptive_interp.py
--rw-r--r--   0 wpk      (42033)    36681    17305 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/beta.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-11 03:03:46.921839 thermoextrap-0.2.3/src/thermoextrap/core/
--rw-r--r--   0 wpk      (42033)    36681      134 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/core/__init__.py
--rw-r--r--   0 wpk      (42033)    36681     4998 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/core/_attrs_utils.py
--rw-r--r--   0 wpk      (42033)    36681    12082 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/src/thermoextrap/core/_deprecate.py
--rw-r--r--   0 wpk      (42033)    36681     8229 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/core/_docstrings.py
--rw-r--r--   0 wpk      (42033)    36681     5672 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/core/cached_decorators.py
--rw-r--r--   0 wpk      (42033)    36681    52840 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/src/thermoextrap/core/data.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-11 03:03:46.923918 thermoextrap-0.2.3/src/thermoextrap/core/external/
--rw-r--r--   0 wpk      (42033)    36681       23 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/core/external/__init__.py
--rw-r--r--   0 wpk      (42033)    36681    19656 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/core/external/docfiller.py
--rw-r--r--   0 wpk      (42033)    36681    23537 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/core/external/docscrape.py
--rw-r--r--   0 wpk      (42033)    36681    10298 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/core/idealgas.py
--rw-r--r--   0 wpk      (42033)    36681    32148 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/core/models.py
--rw-r--r--   0 wpk      (42033)    36681      322 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/core/sputils.py
--rw-r--r--   0 wpk      (42033)    36681    18816 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/core/stack.py
--rw-r--r--   0 wpk      (42033)    36681     3159 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/core/xrutils.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-11 03:03:46.927418 thermoextrap-0.2.3/src/thermoextrap/gpr_active/
--rw-r--r--   0 wpk      (42033)    36681      717 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/gpr_active/__init__.py
--rw-r--r--   0 wpk      (42033)    36681    88989 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/gpr_active/active_utils.py
--rw-r--r--   0 wpk      (42033)    36681    56361 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/gpr_active/gp_models.py
--rw-r--r--   0 wpk      (42033)    36681     3386 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/gpr_active/ig_active.py
--rw-r--r--   0 wpk      (42033)    36681     3003 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/gpr_active/sine_active.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-11 03:03:46.934091 thermoextrap-0.2.3/src/thermoextrap/legacy/
--rw-r--r--   0 wpk      (42033)    36681      629 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/legacy/__init__.py
--rw-r--r--   0 wpk      (42033)    36681     9563 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/legacy/extrap.py
--rw-r--r--   0 wpk      (42033)    36681    18316 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/legacy/gpr.py
--rw-r--r--   0 wpk      (42033)    36681    16856 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/legacy/gpr_stack.py
--rw-r--r--   0 wpk      (42033)    36681     5547 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/legacy/ig.py
--rw-r--r--   0 wpk      (42033)    36681    16626 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/legacy/interp.py
--rw-r--r--   0 wpk      (42033)    36681     9580 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/legacy/old_scripts.py
--rw-r--r--   0 wpk      (42033)    36681    21063 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/legacy/recursive_interp.py
--rw-r--r--   0 wpk      (42033)    36681     8609 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/legacy/reweight.py
--rw-r--r--   0 wpk      (42033)    36681    10983 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/legacy/utilities.py
--rw-r--r--   0 wpk      (42033)    36681    13032 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/src/thermoextrap/lnpi.py
--rw-r--r--   0 wpk      (42033)    36681    21947 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/src/thermoextrap/recursive_interp.py
--rw-r--r--   0 wpk      (42033)    36681     5855 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/volume.py
--rw-r--r--   0 wpk      (42033)    36681     4391 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/src/thermoextrap/volume_idealgas.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-11 03:03:46.944403 thermoextrap-0.2.3/src/thermoextrap.egg-info/
--rw-r--r--   0 wpk      (42033)    36681     1979 2023-04-11 03:03:46.000000 thermoextrap-0.2.3/src/thermoextrap.egg-info/SOURCES.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-11 03:03:46.941969 thermoextrap-0.2.3/tests/
--rw-r--r--   0 wpk      (42033)    36681     9121 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/tests/conftest.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-11 03:03:46.942599 thermoextrap-0.2.3/tests/lnpi_data/
--rw-r--r--   0 wpk      (42033)    36681   667972 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/tests/lnpi_data/sample_data.json
--rw-r--r--   0 wpk      (42033)    36681    23103 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/tests/test_GPs.py
--rw-r--r--   0 wpk      (42033)    36681    25332 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/tests/test_active.py
--rw-r--r--   0 wpk      (42033)    36681    32495 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/tests/test_beta.py
--rw-r--r--   0 wpk      (42033)    36681     2259 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/tests/test_data.py
--rw-r--r--   0 wpk      (42033)    36681     1421 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/tests/test_idealgas.py
--rw-r--r--   0 wpk      (42033)    36681     3437 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/tests/test_lnPi.py
--rw-r--r--   0 wpk      (42033)    36681     2099 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/tests/test_stack.py
--rw-r--r--   0 wpk      (42033)    36681     7641 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/tests/test_u_data.py
--rw-r--r--   0 wpk      (42033)    36681     2051 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/tests/test_u_equations.py
--rw-r--r--   0 wpk      (42033)    36681     2703 2023-04-10 21:01:11.000000 thermoextrap-0.2.3/tests/test_volume.py
--rw-r--r--   0 wpk      (42033)    36681     4245 2023-04-11 02:16:02.000000 thermoextrap-0.2.3/tox.ini
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.728277 thermoextrap-0.3.0/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1480 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/.cruft.json
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      540 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/.editorconfig
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1324 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/.gitignore
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      104 2023-04-11 02:16:02.000000 thermoextrap-0.3.0/.gitmodules
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3681 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      163 2023-04-24 16:24:54.000000 thermoextrap-0.3.0/AUTHORS.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1386 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9227 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1645 2023-04-10 21:01:10.000000 thermoextrap-0.3.0/LICENSE
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      285 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/MANIFEST.in
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    11351 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/Makefile
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9570 2023-05-03 20:15:44.728674 thermoextrap-0.3.0/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5362 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/README.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.692236 thermoextrap-0.3.0/changelog.d/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.692571 thermoextrap-0.3.0/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.693235 thermoextrap-0.3.0/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      213 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      774 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      269 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/changelog.d/templates/new_fragment.md.j2
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.697698 thermoextrap-0.3.0/environment/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       11 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/environment/conda-spec.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      985 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/environment/dev-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      423 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      108 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       79 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      638 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/environment/docs-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      584 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       53 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/environment/lint-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      337 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/environment/lint.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       36 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      328 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/environment/test.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      299 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/environment/tools.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      369 2023-05-03 20:14:50.000000 thermoextrap-0.3.0/environment.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6719 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/pyproject.toml
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.700635 thermoextrap-0.3.0/scripts/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      399 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/scripts/dist-conda.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      312 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/scripts/dist-pypi.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1099 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/scripts/docs-examples-symlinks.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      266 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/scripts/lint.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       91 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/scripts/run-prettier.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      489 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/scripts/tox-ipykernel-display-name.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      293 2023-05-03 20:15:44.730206 thermoextrap-0.3.0/setup.cfg
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      323 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/setup.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.684145 thermoextrap-0.3.0/src/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.706335 thermoextrap-0.3.0/src/thermoextrap/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1583 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18791 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/adaptive_interp.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    17295 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/beta.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.709989 thermoextrap-0.3.0/src/thermoextrap/core/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/core/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4998 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/core/_attrs_utils.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    12082 2023-04-11 02:16:02.000000 thermoextrap-0.3.0/src/thermoextrap/core/_deprecate.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      322 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/core/sputils.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3159 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/core/xrutils.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    52780 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/data.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3513 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/docstrings.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.711784 thermoextrap-0.3.0/src/thermoextrap/gpr_active/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      717 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/gpr_active/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    89013 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/gpr_active/active_utils.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    56361 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/gpr_active/gp_models.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3377 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/gpr_active/ig_active.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3003 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/gpr_active/sine_active.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10310 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/idealgas.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.718196 thermoextrap-0.3.0/src/thermoextrap/legacy/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      629 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/legacy/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9563 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/legacy/extrap.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18311 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/legacy/gpr.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    16775 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/legacy/gpr_stack.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5547 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/legacy/ig.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    16626 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/legacy/interp.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9580 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/legacy/old_scripts.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    21063 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/legacy/recursive_interp.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     8609 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/legacy/reweight.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10983 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/src/thermoextrap/legacy/utilities.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    12877 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/lnpi.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    32051 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/models.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    21933 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/recursive_interp.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18752 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/stack.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5827 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/volume.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4387 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/src/thermoextrap/volume_idealgas.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.708269 thermoextrap-0.3.0/src/thermoextrap.egg-info/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9570 2023-05-03 20:15:44.000000 thermoextrap-0.3.0/src/thermoextrap.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2466 2023-05-03 20:15:44.000000 thermoextrap-0.3.0/src/thermoextrap.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-05-03 20:15:44.000000 thermoextrap-0.3.0/src/thermoextrap.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-04-10 21:05:09.000000 thermoextrap-0.3.0/src/thermoextrap.egg-info/not-zip-safe
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      360 2023-05-03 20:15:44.000000 thermoextrap-0.3.0/src/thermoextrap.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       13 2023-05-03 20:15:44.000000 thermoextrap-0.3.0/src/thermoextrap.egg-info/top_level.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.726147 thermoextrap-0.3.0/tests/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9072 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/tests/conftest.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-03 20:15:44.726702 thermoextrap-0.3.0/tests/lnpi_data/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   794879 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/tests/lnpi_data/sample_data.json
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    23103 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/tests/test_GPs.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    25332 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/tests/test_active.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    32495 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/tests/test_beta.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2259 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/tests/test_data.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1421 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/tests/test_idealgas.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3437 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/tests/test_lnPi.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2094 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/tests/test_stack.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     7641 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/tests/test_u_data.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2046 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/tests/test_u_equations.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2703 2023-04-10 21:01:11.000000 thermoextrap-0.3.0/tests/test_volume.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3981 2023-05-03 20:14:51.000000 thermoextrap-0.3.0/tox.ini
```

### Comparing `thermoextrap-0.2.3/.cruft.json` & `thermoextrap-0.3.0/.cruft.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8381761695906432%*

 * *Differences: {"'commit'": "'cb20a32f67dadb4142be54898a87de1efdce6bd6'",*

 * * "'context'": "{'cookiecutter': {'_copy_without_render': {insert: [(6, 'changelog.d/templates/*'), "*

 * *              "(7, 'changelog.d/templates/auto-changlog/*')], delete: [4]}}}",*

 * * "'skip'": "{insert: [(1, 'docs/examples/usage/demo.ipynb'), (2, 'examples/usage/demo.ipynb'), (3, "*

 * *           "'docs/examples/example-usage.md')], delete: [12, 11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1]}"}*

```diff
@@ -1,20 +1,21 @@
 {
     "checkout": "feature/markdown",
-    "commit": "be1b9cec709f862f8de5132e517a42db90758f04",
+    "commit": "cb20a32f67dadb4142be54898a87de1efdce6bd6",
     "context": {
         "cookiecutter": {
             "_copy_without_render": [
                 "*.html",
                 "docs/_templates/*.rst",
                 "docs/_templates/autosummary/*.rst",
                 "docs/_templates/autodocsumm/*.rst",
-                "docs/_static/*",
                 "docs/_static/css/*",
-                "docs/_static/js/*"
+                "docs/_static/js/*",
+                "changelog.d/templates/*",
+                "changelog.d/templates/auto-changlog/*"
             ],
             "_template": "https://github.com/wpk-nist-gov/cookiecutter-pypackage.git",
             "command_line_interface": "No command-line interface",
             "conda_channel": "wpk-nist",
             "create_author_file": "y",
             "email": "wpk@nist.gov",
             "full_name": "William P. Krekelberg",
@@ -31,22 +32,13 @@
             "use_pytest": "y",
             "version": "0.0.1"
         }
     },
     "directory": null,
     "skip": [
         "src/thermoextrap/__init__.py",
-        "environment.yaml",
-        "HISTORY.md",
-        "AUTHORS.md",
-        "MANIFEST.in",
-        "README.md",
-        "docs/spelling_wordlist.txt",
-        "environment/dev-extras.yaml",
-        "environment/docs-extras.yaml",
-        "environment/test-extras.yaml",
-        "docs/index.md",
-        "docs/installation.md",
-        ".gitignore"
+        "docs/examples/usage/demo.ipynb",
+        "examples/usage/demo.ipynb",
+        "docs/examples/example-usage.md"
     ],
     "template": "https://github.com/wpk-nist-gov/cookiecutter-pypackage.git"
 }
```

### Comparing `thermoextrap-0.2.3/.gitignore` & `thermoextrap-0.3.0/.gitignore`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 # Distribution / packaging
 .Python
 env/
 build/
 develop-eggs/
 dist/
-dist-conda/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
@@ -103,13 +102,11 @@
 .mypy_cache/
 
 # IDE settings
 .vscode/
 pyrightconfig.json
 .autoenv.zsh
 .autoenv_leave.zsh
-/docs/generated/
+/docs/**/generated/
 /monkeytype.sqlite3
-/dist-conda/
-/cruft.patch
-/docs/jupyter_execute/
-/docs/reference/generated/
+/dist-conda/*
+!/dist-conda/Makefile
```

### Comparing `thermoextrap-0.2.3/.pre-commit-config.yaml` & `thermoextrap-0.3.0/.pre-commit-config.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,88 +1,135 @@
 ---
 # pre-commit install
 # pre-commit run --all-files
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
+default_install_hook_types:
+  - pre-commit
+  - commit-msg
 repos:
+  #* Top level
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-added-large-files
       - id: check-yaml
-        #     args: [--unsafe]
-  # Ruff
+      - id: check-json
+      - id: check-merge-conflict
+      - id: check-symlinks
+      - id: check-toml
+  #* Formatting
+  - repo: https://github.com/pre-commit/mirrors-prettier
+    rev: "v3.0.0-alpha.6"
+    hooks:
+      - id: prettier
+        stages: [commit]
+        additional_dependencies:
+          - prettier-plugin-toml
+        exclude: ^tests/lnpy_data/sample_data.json
+  #** markdown
+  - repo: https://github.com/DavidAnson/markdownlint-cli2
+    rev: v0.6.0
+    hooks:
+      - id: markdownlint-cli2
+        args: ["--style prettier"]
+  #* Linting
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     # Ruff version.
-    rev: 'v0.0.254'
+    rev: "v0.0.261"
     hooks:
       - id: ruff
-        args: ["--fix"]
-  # isort should run before black as black sometimes tweaks the isort output
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
-    hooks:
-      - id: isort
-        stages: [manual]
-  # https://github.com/python/black#version-control-integration
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
-      - id: black-jupyter
+      # - id: black-jupyter
+      # Move to just black.  use nbqa for notebook formatting
+      - id: black
   - repo: https://github.com/adamchainz/blacken-docs
-    rev: "1.13.0"  # replace with latest tag on GitHub
+    rev: "1.13.0"
     hooks:
       - id: blacken-docs
         additional_dependencies:
-          - black==23.1.0
+          - black==23.3.0
         exclude: ^README.md
-  - repo: https://github.com/keewis/blackdoc
-    rev: v0.3.8
+  - repo: https://github.com/nbQA-dev/nbQA
+    rev: 1.7.0
     hooks:
-      - id: blackdoc
-        additional_dependencies: ["black==23.1.0"]
-      - id: blackdoc-autoupdate-black
-  - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+      - id: nbqa-ruff
+        additional_dependencies: [ruff]
+      - id: nbqa-black
+        additional_dependencies: [black]
+
+  #* Commit message
+  - repo: https://github.com/commitizen-tools/commitizen
+    rev: v3.0.1
+    hooks:
+      - id: commitizen
+        stages: [commit-msg]
+
+  #* Manual Linting
+  - repo: local
     hooks:
-      - id: codespell
-        types_or: [python, rst, markdown, cython, c]
-        additional_dependencies: [tomli]
-        args: [-I, docs/spelling_wordlist.txt]
+      - id: mypy
+        name: mypy
+        entry: tox
+        args: ["-e", "lint-mypy"]
+        language: system
+        pass_filenames: false
+        # additional_dependencies: [tox]
+        types: [python]
+        require_serial: true
+        stages: [manual]
+      - id: pyright
+        name: pyright
+        entry: pyright
+        args: []
+        language: system
+        pass_filenames: true
+        # additional_dependencies: [tox]
+        types: [python]
+        require_serial: true
         stages: [manual]
-  # this should be run before flake8 to
-  # this should be run externally
-  # messes up too many things
-  # - repo: https://github.com/PyCQA/docformatter
-  #   rev: v1.5.0
-  #   hooks:
-  #     - id: docformatter
-  #       args: [--in-place]
+  # isort, pyupgrade, flake8 defer to ruff
+  - repo: https://github.com/PyCQA/isort
+    rev: 5.12.0
+    hooks:
+      - id: isort
+        stages: [manual]
+  - repo: https://github.com/asottile/pyupgrade
+    rev: v3.3.1
+    hooks:
+      - id: pyupgrade
+        stages: [manual]
+        args: [--py38-plus]
   - repo: https://github.com/pycqa/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
         stages: [manual]
-        additional_dependencies: [flake8-docstrings]
-        exclude: ^tests/|examples/gpr_active_learning/|src/thermoextrap/legacy/|^docs/conf.py|^setup.py
-  - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.1.1
+        additional_dependencies:
+          - flake8-docstrings
+          - Flake8-pyproject
+          # - pep8-naming
+          # - flake8-rst-docstrings
+        exclude: ^tests/|^src/thermoextrap/tests/|^docs/conf.py|^setup.py|example/gpr_active_learning/|src/thermoextrap/legacy
+  - repo: https://github.com/nbQA-dev/nbQA
+    rev: 1.7.0
     hooks:
-      - id: mypy
-        # `properies` & `asv_bench` are copied from setup.cfg.
-        # `_typed_ops.py` is added since otherwise mypy will complain (but notably only in pre-commit)
-        exclude: properties|asv_bench|_typed_ops.py|conf.py
-        # This is slow and so we take it out of the fast-path; requires passing
-        # `--hook-stage manual` to pre-commit
+      - id: nbqa-pyupgrade
+        additional_dependencies: [pyupgrade]
         stages: [manual]
-        additional_dependencies: [types-pkg_resources, typing-extensions==3.10.0.0, numpy]
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+        args: [--py38-plus]
+      - id: nbqa-isort
+        additional_dependencies: [isort]
+        stages: [manual]
+  #** spelling
+  - repo: https://github.com/codespell-project/codespell
+    rev: v2.2.4
     hooks:
-      - id: pyupgrade
+      - id: codespell
+        types_or: [python, rst, markdown, cython, c]
+        additional_dependencies: [tomli]
+        args: [-I, docs/spelling_wordlist.txt]
         stages: [manual]
-        args:
-          - --py38-plus
-          # remove on f-strings in Py3.7
-          - --keep-percent-format
```

### Comparing `thermoextrap-0.2.3/CONTRIBUTING.md` & `thermoextrap-0.3.0/CONTRIBUTING.md`

 * *Files 23% similar despite different names*

```diff
@@ -31,243 +31,361 @@
 
 `thermoextrap` could always use more documentation, whether as part of the
 official `thermoextrap` docs, in docstrings, or even on the web in blog posts,
 articles, and such.
 
 ### Submit Feedback
 
-The best way to send feedback is to file an issue at <https://github.com/usnistgov/thermoextrap/issues>.
+The best way to send feedback is to file an issue at
+<https://github.com/usnistgov/thermoextrap/issues>.
 
 If you are proposing a feature:
 
 - Explain in detail how it would work.
 - Keep the scope as narrow as possible, to make it easier to implement.
-- Remember that this is a volunteer-driven project, and that contributions
-  are welcome :)
-
-## Get Started!
+- Remember that this is a volunteer-driven project, and that contributions are
+  welcome :)
 
+## Get Started
 
 ### Environment setup
 
 [pipx]: https://github.com/pypa/pipx
 [condax]: https://github.com/mariusvniekerk/condax
 [mamba]: https://github.com/mamba-org/mamba
-[conda-fast-setup]: https://www.anaconda.com/blog/a-faster-conda-for-a-growing-community
+[conda-fast-setup]:
+  https://www.anaconda.com/blog/a-faster-conda-for-a-growing-community
 [pre-commit]: https://pre-commit.com/
 [tox]: https://tox.wiki/en/latest/
 [tox-conda]: https://github.com/tox-dev/tox-conda
 [cruft]: https://github.com/cruft/cruft
 [conda-merge]: https://github.com/amitbeka/conda-merge
 [git-flow]: https://github.com/nvie/gitflow
-
-This project uses a host of tools to (hopefully) make development easier.  We recommend installing some of these tools system wide.  For this, we recommend using
-either [pipx] or [condax].  We mostly use conda/condax, but the choice is yours.  For conda, we recommend actually using [mamba]. Alternatively, you can setup `conda` to use the faster `mamba` solver.
-See [here][conda-fast-setup] for details.
-
-Additional dependencies are:
-
-* [pre-commit]
-* [tox] and [tox-conda]
-* [cruft]
-* [conda-merge]
+[scriv]: https://github.com/nedbat/scriv
+[conventional-style]: https://www.conventionalcommits.org/en/v1.0.0/
+[commitizen]: https://github.com/commitizen-tools/commitizen
+[nb_conda_kernels]: https://github.com/Anaconda-Platform/nb_conda_kernels
+
+This project uses a host of tools to (hopefully) make development easier. We
+recommend installing some of these tools system wide. For this, we recommend
+using either [pipx] or [condax]. We mostly use conda/condax, but the choice is
+yours. For conda, we recommend actually using [mamba]. Alternatively, you can
+setup `conda` to use the faster `mamba` solver. See [here][conda-fast-setup] for
+details.
+
+Additional tools are:
+
+- [pre-commit]
+- [tox] and [tox-conda]
+- [cruft]
+- [conda-merge]
+- [scriv]
 
 These are setup using the following:
 
-```bash
+```console
 condax install pre-commit
 condax install tox
 condax inject tox tox-conda
 condax install cruft
 condax install conda-merge
+condax install commitizen
+pipx install scriv
 ```
 
+Alternatively, you can install these dependencies using:
+
+```console
+conda env update -n {env-name} environment/tools.yaml
+```
 
 ### Getting the repo
 
 Ready to contribute? Here's how to set up `thermoextrap` for local development.
 
-1. Fork the `thermoextrap` repo on GitHub.
+- Fork the `thermoextrap` repo on GitHub.
 
-2. Clone your fork locally:
+- Clone your fork locally:
 
-    ```bash
-    git clone git@github.com:your_name_here/thermoextrap.git
-    ```
+  ```bash
+  git clone git@github.com:your_name_here/thermoextrap.git
+  ```
+
+  If the repo includes submodules, you can add them either with the initial
+  close using:
+
+  ```bash
+  git clone --recursive-submodules git@github.com:your_name_here/thermoextrap.git
+  ```
 
-    The example notebooks require the `examples/data` submodule to be loaded.
+  or after the clone using
+
+  ```bash
+  cd thermoextrap
+  git submodule update --init --recursive
+  ```
+
+- Create development environment. There are two options to create the
+  development environment.
+
+  - The recommended method is to use tox by using either:
 
     ```bash
-    git submodule update --init --recursive
+    tox -e dev
     ```
 
-3. Create development environment.  Using the `make` will install a development version using mamba.
+    or
 
     ```bash
-    make mamba-dev
+    make dev-env
     ```
 
-4. Initiate pre-commit with:
+    These create a development environment located at `.tox/dev`.
 
     ```bash
-    pre-commit init
+    make tox-ipykernel-display-name
     ```
 
-    To update the recipe, periodically run:
+    This will add a meaningful display name for the kernel (assuming you're
+    using [nb_conda_kernels])
+
+  - Alternativley, you can create centrally located conda environmentment using
+    the command:
 
     ```bash
-    pre-commit autoupdate
+    make mamba-dev
     ```
 
-5. Install editable package:
+    This will create a conda environment 'thermoextrap-env' in the default
+    location.
+
+    To install (an editable version) of the current package:
 
     ```bash
     pip install -e . --no-deps
     ```
 
     or
 
     ```bash
     make install-dev
     ```
 
-07. Create a branch for local development:
+- Initiate [pre-commit] with:
 
-    ```bash
-    git checkout -b name-of-your-bugfix-or-feature
-    ```
+  ```bash
+  pre-commit install
+  ```
 
-    Now you can make your changes locally.  Alternatively, we recommend using [git-flow].
+  To update the recipe, periodically run:
 
-08. When you're done making changes, check that your changes pass the pre-commit checks:
-    tests.
+  ```bash
+  pre-commit autoupdate
+  ```
 
-    ```bash
-    pre-commit run [--all-files]
-    ```
+  If recipes change over time, you can clean up old installs with:
 
-    To run tests, use:
+  ```bash
+  pre-commit gc
+  ```
 
-    ```bash
-    pytest
-    ```
+- Create a branch for local development:
 
-    To test against multiple python versions, use tox:
+  ```bash
+  git checkout -b name-of-your-bugfix-or-feature
+  ```
 
-    ```bash
-    tox
-    ```
+  Now you can make your changes locally. Alternatively, we recommend using
+  [git-flow].
 
-    or using the `make`:
+- When you're done making changes, check that your changes pass the pre-commit
+  checks: tests.
 
-    ```bash
-    make test-all
-    ```
+  ```bash
+  pre-commit run [--all-files]
+  ```
 
+  To run tests, use:
 
-09. Commit your changes and push your branch to GitHub:
+  ```bash
+  pytest
+  ```
 
-    ```
-    $ git add .
-    $ git commit -m "Your detailed description of your changes."
-    $ git push origin name-of-your-bugfix-or-feature
-    ```
+  To test against multiple python versions, use tox:
 
-10. Submit a pull request through the GitHub website.
+  ```bash
+  tox
+  ```
 
+  or using the `make`:
 
-### Dependency management
+  ```bash
+  make test-all
+  ```
+
+  Additionally, you should run the following:
+
+  ```bash
+  make pre-commit-lint-markdown
+  make pre-commit-codespell
+  ```
+
+- Create changelog fragment. See [scriv] for more info.
+
+  ```bash
+  scriv create --edit
+  ```
+
+- Commit your changes and push your branch to GitHub:
 
-Dependencies need to be placed in a few locations, which depend on the nature of the dependency.
+  ```bash
+  git add .
+  git commit -m "Your detailed description of your changes."
+  git push origin name-of-your-bugfix-or-feature
+  ```
 
-* Package dependency: `environment.yaml` and `dependencies` section of `pyproject.toml`
-* Documentation dependency: `environment/docs-extras.yaml` and `test` section of `pyproject.toml`
-* Development dependency: `environment/dev-extras.yaml` and `dev` section of `pyproject.toml`
+  Note that the pre-commit hooks will force the commit message to be in the
+  [conventional sytle][conventional-style]. To assist this, you may want to
+  commit using [commitizen].
 
-Note that total yaml files are build using [conda-merge].  For example, `environment.yaml` is combined with `environment/docs-extras.yaml` to produce `environment/docs.yaml`.  This is automated in the `Makefile`.  You can also run, after doing any updates,
+  ```bash
+  cz commit
+  ```
+
+- Submit a pull request through the GitHub website.
+
+### Dependency management
+
+Dependencies need to be placed in a few locations, which depend on the nature of
+the dependency.
+
+- Package dependency: `environment.yaml` and `dependencies` section of
+  `pyproject.toml`
+- Documentation dependency: `environment/docs-extras.yaml` and `test` section of
+  `pyproject.toml`
+- Development dependency: `environment/dev-extras.yaml` and `dev` section of
+  `pyproject.toml`
+
+Note that total yaml files are build using [conda-merge]. For example,
+`environment.yaml` is combined with `environment/docs-extras.yaml` to produce
+`environment/docs.yaml`. This is automated in the `Makefile`. You can also run,
+after doing any updates,
 
 ```bash
-make environment-files
+make environment-files-build
 ```
 
 which will rebuild all the needed yaml files.
 
-
 ## Pull Request Guidelines
 
 Before you submit a pull request, check that it meets these guidelines:
 
-1. The pull request should include tests.
-2. If the pull request adds functionality, the docs should be updated. Put
-   your new functionality into a function with a docstring, and add the
-   feature to the list in README.rst.
-3. The pull request should work for Python 3.8, 3.9, 3.10.
+- The pull request should include tests.
+- If the pull request adds functionality, the docs should be updated. Put your
+  new functionality into a function with a docstring, and add the feature to the
+  list in CHANGELOG.md. You should use [scriv] for this.
+- The pull request should work for Python 3.8, 3.9, 3.10.
 
 ## Building the docs
 
-We use [tox] to isolate the documentation build.  Useful commands are as follows.
+We use [tox] to isolate the documentation build. Useful commands are as follows.
 
-* Build the docs:
+- Build the docs:
 
-    ```bash
-    tox -e docs-build
-    ```
+  ```bash
+  tox -e docs -- build
+  ```
 
-* Spellcheck the docs:
+- Spellcheck the docs:
 
-    ```bash
-    tox -e docs-spelling
-    ```
+  ```bash
+  tox -e docs -- spelling
+  ```
 
-* Create a release of the docs:
+- Create a release of the docs:
 
-    ```bash
-    tox -e docs-release
-    ```
+  ```bash
+  tox -e docs -- release
+  ```
+
+  If you make any changes to `docs/examples`, you should run:
 
-    After this, the docs can be pushed to the correct branch for distribution.
+  ```bash
+  make docs-examples-symlink
+  ```
 
-* Live documentation updates using
+  to update symlinks from `docs/examples` to `examples`.
+
+  After this, the docs can be pushed to the correct branch for distribution.
+
+- Live documentation updates using
+
+  ```bash
+  make docs-livehtml
+  ```
 
 ## Using tox
 
-The package is setup to use tox to test, build and release pip and conda distributions, and release the docs.  Most of these tasks have a command in the `Makefile`.  To test against multiple versions, use:
+The package is setup to use tox to test, build and release pip and conda
+distributions, and release the docs. Most of these tasks have a command in the
+`Makefile`. To test against multiple versions, use:
 
-```
-$ make test-all
+```bash
+make test-all
 ```
 
 To build the documentation in an isolated environment, use:
 
-```
-$ make docs-build
+```bash
+make docs-build
 ```
 
 To release the documentation use:
 
-```
-$ make docs-release posargs='-m "commit message" -r origin -p'
+```bash
+make docs-release release_args='-m "commit message" -r origin -p'
 ```
 
-Where posargs is are passed to ghp-import.  Note that the branch created is called `nist-pages`.  This can be changed in `tox.ini`.
+Where posargs is are passed to ghp-import. Note that the branch created is
+called `nist-pages`. This can be changed in `tox.ini`.
 
 To build the distribution, use:
 
-```
-$ make dist-pypi-[build-testrelease-release]
+```bash
+make dist-pypi-[build-testrelease-release]
 ```
 
-where `build` build to distro, `testrelease` tests putting on `testpypi` and release puts the distro on pypi.
+where `build` build to distro, `testrelease` tests putting on `testpypi` and
+release puts the distro on pypi.
 
 To build the conda distribution, use:
 
-```
-$ make dist-conda-[recipe, build]
+```bash
+make dist-conda-[recipe, build]
 ```
 
-where `recipe` makes the conda recipe (using grayskull), and `build` makes the distro.  This can be manually added to a channel.
+where `recipe` makes the conda recipe (using grayskull), and `build` makes the
+distro. This can be manually added to a channel.
 
 To test the created distributions, you can use one of:
 
+```bash
+tox -e test-dist-[pypi, conda]-[local,remote]-py[38,39,...]
 ```
-$ make test-dist-[pypi, conda]-[local,remote] py=[38, 39, 310]
+
+or
+
+```bash
+make test-dist-[pypi, conda]-[local,remote] py=[38, 39, 310]
 ```
+
+where one options in the brackets should be choosen.
+
+## Package version
+
+[setuptools_scm]: https://github.com/pypa/setuptools_scm
+
+Versioning is handled with [setuptools_scm].The pacakge version is set by the
+git tag. For convenience, you can override the version in the makefile (calling
+tox) by setting `version=v{major}.{minor}.{micro}`. This is useful for updating
+the docs, etc.
```

### Comparing `thermoextrap-0.2.3/LICENSE` & `thermoextrap-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.3/Makefile` & `thermoextrap-0.3.0/Makefile`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 endef
 export BROWSER_PYSCRIPT
 
 define PRINT_HELP_PYSCRIPT
 import re, sys
 
 for line in sys.stdin:
-	match = re.match(r'^([a-zA-Z_-]+):.*?## (.*)$$', line)
+	match = re.match(r'^([a-zA-Z_/.-]+):.*?## (.*)$$', line)
 	if match:
 		target, help = match.groups()
 		print("%-20s %s" % (target, help))
 endef
 export PRINT_HELP_PYSCRIPT
 
 BROWSER := python -c "$$BROWSER_PYSCRIPT"
@@ -50,57 +50,64 @@
 
 
 
 
 ################################################################################
 # utilities
 ################################################################################
-.PHONY: lint pre-commit-init pre-commit-run pre-commit-run-all pre-commit-lint-extra pre-commit-codespell init
-
-lint: ## check style with flake8
-	flake8 cmomy tests
-
+.PHONY: pre-commit-init pre-commit pre-commit-all
 pre-commit-init: ## install pre-commit
 	pre-commit install
 
-pre-commit-run: ## run pre-commit
+pre-commit: ## run pre-commit
 	pre-commit run
 
-pre-commit-run-all: ## run pre-commit on all files
+pre-commit-all: ## run pre-commit on all files
 	pre-commit run --all-files
 
-pre-commit-run-all-ruff: ## run ruff on on all files
+.PHONY: pre-commit-lint pre-commit-lint-notebooks pre-commit-prettier pre-commit-lint-markdown
+pre-commit-lint: ## run ruff and black on on all files
 	pre-commit run --all-files ruff
+	pre-commit run --all-files black
+	pre-commit run --all-files blacken-docs
+
+pre-commit-lint-notebooks: ## Run nbqa linting
+	pre-commit run --all-files nbqa-ruff
+	pre-commit run --all-files nbqa-black
+
+pre-commit-prettier: ## run prettier on all files.
+	pre-commit run --all-files prettier
 
-pre-commit-manual: ## run pre-commit manual flags
-	pre-commit run --hook-stage manual
+pre-commit-lint-markdown: ## run markdown linter.
+	pre-commit run --all-files --hook-stage manual markdownlint-cli2
 
-pre-commit-lint-extra: ## run all linting
+.PHONY: pre-commit-lint-extra pre-commit-mypy pre-commit-codespell
+pre-commit-lint-extra: ## run all extra linting (isort, flake8, pyupgrade, nbqa isort and pyupgrade)
 	pre-commit run --all-files --hook-stage manual isort
 	pre-commit run --all-files --hook-stage manual flake8
 	pre-commit run --all-files --hook-stage manual pyupgrade
+	pre-commit run --all-files --hook-stage manual nbqa-pyupgrade
+	pre-commit run --all-files --hook-stage manual nbqa-isort
 
 pre-commit-mypy: ## run mypy
 	pre-commit run --all-files --hook-stage manual mypy
 
+pre-commit-pyright: ## run pyright
+	pre-commit run --all-files --hook-stage manual pyright
+
 pre-commit-codespell: ## run codespell. Note that this imports allowed words from docs/spelling_wordlist.txt
 	pre-commit run --all-files --hook-stage manual codespell
 
-.git: ## init git
-	git init
-
-init: .git pre-commit-init ## run git-init pre-commit
-
 
 ################################################################################
 # my convenience functions
 ################################################################################
 .PHONY: user-venv user-autoenv-zsh user-all
 user-venv: ## create .venv file with name of conda env
-	echo thermoextrap-env > .venv
+	echo $${PWD}/.tox/dev > .venv
 
 user-autoenv-zsh: ## create .autoenv.zsh files
 	echo conda activate $$(cat .venv) > .autoenv.zsh
 	echo conda deactivate > .autoenv_leave.zsh
 
 user-all: user-venv user-autoenv-zsh ## runs user scripts
 
@@ -130,28 +137,40 @@
 	python -c 'import thermoextrap; print(thermoextrap.__version__)'
 
 version: version-scm version-import
 
 ################################################################################
 # Environment files
 ################################################################################
+ENVIRONMENTS = $(addsuffix .yaml,$(addprefix environment/, dev docs test))
+PRETTIER = bash scripts/run-prettier.sh
 
-environment/dev.yaml: environment.yaml environment/dev-extras.yaml ## build development yaml file
+environment/%.yaml: environment.yaml environment/%-extras.yaml ## create combined environment/{dev,docs,test}.yaml
 	conda-merge $^ > $@
+	$(PRETTIER) $@
+
+environment/dev.yaml: ## development environment yaml file
+environment/test.yaml: ## testing environment yaml file
+enviornment/docs.yaml: ## docs environment yaml file
 
-environment/docs.yaml: environment.yaml environment/docs-extras.yaml ## build docs yaml file
-	conda-merge $^ > $@
 
-environment/test.yaml: environment.yaml environment/test-extras.yaml ## build test yaml file
+# special for linters
+environment/lint.yaml: environment.yaml $(addsuffix .yaml, $(addprefix environment/, test-extras lint-extras)) ## mypy environment
+	echo $^
 	conda-merge $^ > $@
+	$(PRETTIER) $@
 
-.PHONY: environment-files
+ENVIRONMENTS += environment/lint.yaml
 
-environment-files: environment/dev.yaml environment/docs.yaml environment/test.yaml ## rebuild all environment files
+.PHONY: environment-files-clean
+environment-files-clean: ## clean all created environment/{dev,docs,test}.yaml
+	-rm $(ENVIRONMENTS) 2> /dev/null || true
 
+.PHONY: environment-files-build
+environment-files-build: $(ENVIRONMENTS) ## rebuild all environment files
 
 ################################################################################
 # virtual env
 ################################################################################
 .PHONY: mamba-env mamba-dev mamba-env-update mamba-dev-update
 
 mamba-env: environment.yaml ## create base environment
@@ -165,98 +184,136 @@
 
 mamba-dev-update: environment/dev.yaml ## update development environment
 	mamba env update -f $<
 
 ################################################################################
 # TOX
 ###############################################################################
-tox_posargs?=-v
-TOX=CONDA_EXE=mamba tox $(tox_posargs)
+tox_args?=-v
+version?=
+TOX=CONDA_EXE=mamba SETUPTOOLS_SCM_PRETEND_VERSION=$(version) tox $(tox_args)
+
+.PHONY: tox-ipykernel-display-name
+tox-ipykernel-display-name: ## Update display-name for any tox env with ipykernel
+	bash ./scripts/tox-ipykernel-display-name.sh thermoextrap
+
+## dev env
+.PHONY: dev-env
+dev-env: environment/dev.yaml ## create development environment using tox
+	tox -e dev
 
 ## testing
-
 .PHONY: test-all
-test-all: environment/test.yaml ## run tests on every Python version with tox
+test-all: environment/test.yaml ## run tests on every Python version with tox.  can pass posargs=...
 	$(TOX) -- $(posargs)
 
-
 ## docs
-.PHONY: docs-build docs-release docs-clean docs-spelling docs-nist-pages docs-open docs-live docs-clean-build docs-linkcheck
-posargs=
+.PHONY: docs-examples-symlink
+docs-examples-symlink: ## create symlinks to notebooks from /examples/ to /docs/examples.
+	bash ./scripts/docs-examples-symlinks.sh
+
+
+.PHONY: docs-build docs-release docs-clean docs-command
 docs-build: ## build docs in isolation
-	$(TOX) -e $@ -- $(posargs)
+	$(TOX) -e docs -- build
 docs-clean: ## clean docs
 	rm -rf docs/_build/*
 	rm -rf docs/generated/*
 	rm -rf docs/reference/generated/*
 docs-clean-build: docs-clean docs-build ## clean and build
-docs-release: ## release docs.  use posargs=... to override stuff
-	$(TOX) -e $@ -- $(posargs)
+docs-release: ## release docs.  use release_args=... to override stuff
+	$(TOX) -e docs -- release
+docs-command: ## run command with command=...
+	$(TOX) -e docs -- command
+
+.PHONY: .docs-spelling docs-nist-pages docs-open docs-livehtml docs-clean-build docs-linkcheck
 docs-spelling: ## run spell check with sphinx
-	$(TOX) -e $@ -- $(posargs)
-docs-nist-pages: ## do both build and releas
-	$(TOX) -e $@ -- $(posargs)
-docs-live: ## use autobuild for docs
-	$(TOX) -e $@ -- $(posargs)
+	$(TOX) -e docs -- spelling
+docs-livehtml: ## use autobuild for docs
+	$(TOX) -e docs -- livehtml
 docs-open: ## open the build
 	$(BROWSER) docs/_build/html/index.html
 docs-linkcheck: ## check links
-	$(TOX) -e docs-build -- linkcheck
+	$(TOX) -e docs -- linkcheck
 
-docs-build docs-release docs-clean docs-spelling docs-nist-pages docs-live: environment/docs.yaml
+docs-build docs-release docs-command docs-clean docs-livehtml docs-linkcheck: environment/docs.yaml
 
+## linting
+.PHONY: lint-mypy lint-pyright lint-pytype lint-all lint-command
+lint-mypy: ## run mypy mypy_args=...
+	$(TOX) -e lint -- mypy
+lint-pyright: ## run pyright pyright_args=...
+	$(TOX) -e lint -- pyright
+lint-pytype: ## run pytype pytype_args=...
+	$(TOX) -e lint -- pytype
+lint-all:
+	$(TOX) -e lint -- all
+lint-command:
+	$(TOX) -e lint -- command
+
+lint-mypy lint-pyright lint-pytype lint-all lint-command: environment/lint.yaml
 
 ## distribution
-.PHONY: dist-pypi-build dist-pypi-testrelease dist-pypi-release dist-conda-recipe dist-conda-build
+.PHONY: dist-pypi-build dist-pypi-testrelease dist-pypi-release dist-pypi-command
 
-posargs=
-dist-pypi-build: ## build dist, can pass posargs=... and tox_posargs=...
-	$(TOX) -e $@ -- $(posargs)
-dist-pypi-testrelease: ## test release on testpypi. can pass posargs=... and tox_posargs=...
-	$(TOX) -e $@ -- $(posargs)
+dist-pypi-build: ## build dist
+	$(TOX) -e dist-pypi -- build
+dist-pypi-testrelease: ## test release on testpypi
+	$(TOX) -e dist-pypi -- testrelease
 dist-pypi-release: ## release to pypi, can pass posargs=...
-	$(TOX) -e $@ -- $(posargs)
-dist-pypi-build dist-pypi-testrelease dist-pypi-release: environment/dist-pypi.yaml
+	$(TOX) -e dist-pypi -- release
+dist-pypi-command: ## run command with command=...
+	$(TOX) -e dist-pypi -- command
+dist-pypi-build dist-pypi-testrelease dist-pypi-release dist-pypi-command: environment/dist-pypi.yaml
 
+.PHONY: dist-conda-recipe dist-conda-build dist-conda-command
 dist-conda-recipe: ## build conda recipe can pass posargs=...
-	$(TOX) -e $@ -- $(posargs)
+	$(TOX) -e dist-conda -- recipe
 dist-conda-build: ## build conda recipe can pass posargs=...
-	$(TOX) -e $@ -- $(pasargs)
-dist-conda-build dist-conda-recipe: environment/dist-conda.yaml
+	$(TOX) -e dist-conda -- build
+dist-conda-command: ## run command with command=...
+	$(TOX) -e dist-conda -- command
+dist-conda-build dist-conda-recipe dist-conda-command: environment/dist-conda.yaml
 
 
 ## test distribution
-.PHONY: test-dist-pypi-remote test-dist-conda-remote test-dist-pypi-local test-dist-conda-local
+.PHONY: testdist-pypi-remote testdist-conda-remote testdist-pypi-local testdist-conda-local
 
 py?=310
-test-dist-pypi-remote: ## test pypi install, can run as `make test-dist-pypi-remote py=39` to run test-dist-pypi-local-py39
+testdist-pypi-remote: ## testdist-pypi-remote: ## test pypi install, can run as `make test-dist-pypi-remote py=39` to run test-dist-pypi-local-py39.  Can specify version setting, eg,  TEST_VERSION='==0.1.0'.  Note that the the format should be '=={version}'.
 	$(TOX) -e $@-py$(py) -- $(posargs)
-
-test-dist-conda-remote: ## test conda install, can run as `make test-dist-conda-remote py=39` to run test-dist-conda-local-py39
+testdist-conda-remote: ## test conda install, can run as `make test-dist-conda-remote py=39` to run test-dist-conda-local-py39
 	$(TOX) -e $@-py$(py) -- $(poasargs)
-
-test-dist-pypi-local: ## test pypi install, can run as `make test-dist-pypi-local py=39` to run test-dist-pypi-local-py39
+testdist-pypi-local: ## test pypi install, can run as `make test-dist-pypi-local py=39` to run test-dist-pypi-local-py39
 	$(TOX) -e $@-py$(py) -- $(posargs)
-
-test-dist-conda-local: ## test conda install, can run as `make test-dist-conda-local py=39` to run test-dist-conda-local-py39
+testdist-conda-local: ## test conda install, can run as `make test-dist-conda-local py=39` to run test-dist-conda-local-py39
 	$(TOX) -e $@-py$(py) -- $(poasargs)
 
-
-test-dist-pypi: environment/test.
-
+testdist-pypi-remote testdist-conda-remote testdist-pypi-local testdist-conda-local: environment/test.yaml
 
 ## list all options
 .PHONY: tox-list
-
 tox-list:
 	$(TOX) -a
 
 
 ################################################################################
 # installation
 ################################################################################
 .PHONY: install install-dev
 install: ## install the package to the active Python's site-packages (run clean?)
 	pip install . --no-deps
 
 install-dev: ## install development version (run clean?)
 	pip install -e . --no-deps
+
+
+################################################################################
+# other tools
+################################################################################
+
+# Note that this requires `auto-changelog`, which can be installed with pip(x)
+auto-changelog: ## autogenerate changelog and print to stdout
+	auto-changelog -u -r usnistgov -v unreleased --tag-prefix v --stdout --template changelog.d/templates/auto-changelog/template.jinja2
+
+commitizen-changelog:
+	cz changelog --unreleased-version unreleased --dry-run --incremental
```

### Comparing `thermoextrap-0.2.3/PKG-INFO` & `thermoextrap-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thermoextrap
-Version: 0.2.3
+Version: 0.3.0
 Summary: Thermodynamic extrapolation
 Home-page: https://github.com/usnistgov/thermoextrap
 Author-email: Jacob Monroe <jacob.monroe@nist.gov>, William Krekelberg <wpk@nist.gov>
 License: "NIST license https://www.nist.gov/director/licensing"
 Project-URL: homepage, https://github.com/usnistgov/thermoextrap
 Project-URL: documentation, https://pages.nist.gov/thermoextrap/
 Keywords: thermoextrap
@@ -25,164 +25,228 @@
 Provides-Extra: viz
 Provides-Extra: mbar
 Provides-Extra: gpr
 Provides-Extra: openmm
 Provides-Extra: all
 Provides-Extra: test
 License-File: LICENSE
-License-File: AUTHORS.md
 
-[![Repo][repo-badge]][repo-link]
-[![Docs][docs-badge]][docs-link]
+<!-- markdownlint-disable MD041 -->
+
+[![Repo][repo-badge]][repo-link] [![Docs][docs-badge]][docs-link]
 [![PyPI license][license-badge]][license-link]
 [![PyPI version][pypi-badge]][pypi-link]
 [![Conda (channel only)][conda-badge]][conda-link]
 [![Code style: black][black-badge]][black-link]
 
+<!-- For more badges, see
+https://shields.io/category/other
+https://naereen.github.io/badges/
+[pypi-badge]: https://badge.fury.io/py/thermoextrap
+-->
 
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
-[black-link]: https://github.com/ambv/black
+[black-link]: https://github.com/psf/black
 [pypi-badge]: https://img.shields.io/pypi/v/thermoextrap
-<!-- [pypi-badge]: https://badge.fury.io/py/thermoextrap -->
 [pypi-link]: https://pypi.org/project/thermoextrap
 [docs-badge]: https://img.shields.io/badge/docs-sphinx-informational
 [docs-link]: https://pages.nist.gov/thermoextrap/
 [repo-badge]: https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff
 [repo-link]: https://github.com/usnistgov/thermoextrap
 [conda-badge]: https://img.shields.io/conda/v/wpk-nist/thermoextrap
 [conda-link]: https://anaconda.org/wpk-nist/thermoextrap
-<!-- Use total link so works from anywhere -->
 [license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
-[license-link]: https://github.com/usnistgov/thermoextrap/blob/master/LICENSE
-<!-- For more badges, see https://shields.io/category/other and https://naereen.github.io/badges/ -->
-
-[numpy]: https://numpy.org
-[Numba]: https://numba.pydata.org/
-[xarray]: https://docs.xarray.dev/en/stable/
-[cmomy]: https://github.com/usnistgov/cmomy
-[gpr-link]: https://github.com/usnistgov/thermoextrap/tree/master/examples/gpr_active_learning
-[notebook-link]: https://github.com/usnistgov/thermoextrap/tree/master/examples/usage
+[license-link]: https://github.com/usnistgov/thermoextrap/blob/main/LICENSE
 
+<!-- other links -->
 
+[cmomy]: https://github.com/usnistgov/cmomy
+[gpr-link]:
+  https://github.com/usnistgov/thermoextrap/tree/main/examples/gpr_active_learning
+[notebook-link]:
+  https://github.com/usnistgov/thermoextrap/tree/main/examples/usage
 
 # `thermoextrap`: Thermodynamic Extrapolation/Interpolation Library
 
 This repository contains code used and described in references [^fn1] [^fn2].
 
-[^fn1]: [Extrapolation and Interpolation Strategies for Efficiently Estimating Structural Observables as a Function of Temperature and Density](https://doi.org/10.1063/5.0014282)
-
-[^fn2]: Leveraging Uncertainty Estimates and Derivative Information in Gaussian Process Regression for Expedited Data Collection in Molecular Simulations. In preparation.
+[^fn1]:
+    [Extrapolation and Interpolation Strategies for Efficiently Estimating Structural Observables as a Function of Temperature and Density](https://doi.org/10.1063/5.0014282)
 
+[^fn2]:
+    Leveraging Uncertainty Estimates and Derivative Information in Gaussian
+    Process Regression for Expedited Data Collection in Molecular Simulations.
+    In preparation.
 
 ## Overview
 
-If you find this code useful in producing published works, please provide an appropriate citation.
-Note that the second citation is focused on adding features that make use of GPR models based on derivative information produced by the core code base.
-For now, the GPR code, along with more information, may be found under [here][gpr-link].
-In a future release, we expect this to be fully integrated into the code base rather than a standalone module.
+If you find this code useful in producing published works, please provide an
+appropriate citation. Note that the second citation is focused on adding
+features that make use of GPR models based on derivative information produced by
+the core code base. For now, the GPR code, along with more information, may be
+found under [here][gpr-link]. In a future release, we expect this to be fully
+integrated into the code base rather than a standalone module.
 
 Code included here can be used to perform thermodynamic extrapolation and
 interpolation of observables calculated from molecular simulations. This allows
 for more efficient use of simulation data for calculating how observables change
 with simulation conditions, including temperature, density, pressure, chemical
 potential, or force field parameters. Users are highly encourage to work through
-the [Jupyter Notebooks][notebook-link] presenting examples for
-a variety of different observable functional forms. We only guarantee that this
-code is functional for the test cases we present here or for which it has
-previously been applied Additionally, the code may be in continuous development
-at any time. Use at your own risk and always check to make sure the produced
-results make sense. If bugs are found, please report them. If specific features
-would be helpful just let us know and we will be happy to work with you to come
-up with a solution.
-
+the [Jupyter Notebooks][notebook-link] presenting examples for a variety of
+different observable functional forms. We only guarantee that this code is
+functional for the test cases we present here or for which it has previously
+been applied Additionally, the code may be in continuous development at any
+time. Use at your own risk and always check to make sure the produced results
+make sense. If bugs are found, please report them. If specific features would be
+helpful just let us know and we will be happy to work with you to come up with a
+solution.
 
 ## Features
 
-* Fast calculation of derivatives
+- Fast calculation of derivatives
 
 ## Status
 
-This package is actively used by the author.  Please feel free to create a pull request for wanted features and suggestions!
-
+This package is actively used by the author. Please feel free to create a pull
+request for wanted features and suggestions!
 
 ## Quick start
 
 `thermoextrap` may be installed with either (recommended)
+
 ```bash
 conda install -c wpk-nist thermoextrap
 ```
+
 or
+
 ```bash
 pip install thermoextrap
 ```
 
 If you use pip, then you can include additional dependencies using
+
 ```bash
 pip install thermoextrap[all]
 ```
 
-If you install `thermoextrap` with conda, there are additional optional dependencies that take some care for installation.  We recommend installing the following via `pip`, as the versions on the conda/conda-forge channels are often a bit old.
+If you install `thermoextrap` with conda, there are additional optional
+dependencies that take some care for installation. We recommend installing the
+following via `pip`, as the versions on the conda/conda-forge channels are often
+a bit old.
+
 ```bash
 pip install tensorflow tensorflow-probability gpflow
 ```
 
 To install from source do the following:
+
 ```bash
 git clone git@github.com:usnistgov/thermoextrap.git
 cd thermoextrap
 pip install . [-e]
 ```
 
 To (optionally) include the example data do the following:
+
 ```bash
 git submodule update --init  --recursive
 ```
 
-
 ## Example usage
 
 ```python
 import thermoextrap
 
 ```
 
 <!-- end-docs -->
 
 ## Documentation
 
 See the [documentation][docs-link] for a look at `thermoextrap` in action.
 
-To have a look at using `thermoextrap` with Gaussian process regression, look in the [gpr][docs/notebooks/gpr] directory.
+To have a look at using `thermoextrap` with Gaussian process regression, look in
+the [gpr](examples/usage/gpr) and
+[gpr_active_learning](examples/gpr_active_learning) directories.
 
 ## License
 
-This is free software.  See [LICENSE][license-link].
+This is free software. See [LICENSE][license-link].
 
 ## Related work
 
 This package extensively uses the [cmomy] package to handle central comoments.
 
+## Contact
 
-# Contact
-Questions may be addressed to Bill Krekelberg at william.krekelberg@nist.gov or Jacob Monroe at jacob.monroe@uark.edu.
-
+Questions may be addressed to Bill Krekelberg at william.krekelberg@nist.gov or
+Jacob Monroe at jacob.monroe@uark.edu.
 
 ## Credits
 
 This package was created with
 [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
 [wpk-nist-gov/cookiecutter-pypackage](https://github.com/wpk-nist-gov/cookiecutter-pypackage)
 Project template forked from
 [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).
 
-# History
+# Changelog
+
+Changelog for `thermoextrap`
+
+## Unreleased
+
+See the fragment files in
+[changelog.d](https://github.com/usnistgov/thermoextrap)
+
+<!-- scriv-insert-here -->
+
+## v0.3.0 — 2023-05-03
+
+### Changed
+
+- New linters via pre-commit
+- Development env now handled by tox
+
+- Moved `modesl, data, idealgas` from `thermoextrap.core` to `thermoextrap`.
+  These were imported at top level anyway. This fixes issues with doing things
+  like `from thermoextrap.data import ...`, etc.
+- Moved `core._docstrings_` to `docstrings`.
+- Now using `cmomy.docstrings` instead of repeating them here.
+
+Full set of changes:
+[`v0.2.2...v0.3.0`](https://github.com/usnistgov/thermoextrap/compare/v0.2.2...0.3.0)
+
+## v0.2.2 - 2023-04-05
+
+Full set of changes:
+[`v0.2.1...v0.2.2`](https://github.com/usnistgov/thermoextrap/compare/v0.2.1...v0.2.2)
+
+## v0.2.1 - 2023-03-30
+
+Full set of changes:
+[`v0.2.0...v0.2.1`](https://github.com/usnistgov/thermoextrap/compare/v0.2.0...v0.2.1)
+
+## v0.2.0 - 2023-03-28
+
+Full set of changes:
+[`v0.1.9...v0.2.0`](https://github.com/usnistgov/thermoextrap/compare/v0.1.9...v0.2.0)
+
+## v0.1.9 - 2023-02-15
+
+Full set of changes:
+[`v0.1.8...v0.1.9`](https://github.com/usnistgov/thermoextrap/compare/v0.1.8...v0.1.9)
+
+## v0.1.8 - 2023-02-15
 
-## 0.0.1 (2021-01-04)
+Full set of changes:
+[`v0.1.7...v0.1.8`](https://github.com/usnistgov/thermoextrap/compare/v0.1.7...v0.1.8)
 
-- First release on PyPI.
+## v0.1.7 - 2023-02-14
 
 This software was developed by employees of the National Institute of Standards
 and Technology (NIST), an agency of the Federal Government. Pursuant to title 17
 United States Code Section 105, works of NIST employees are not subject to
 copyright protection in the United States and are considered to be in the public
 domain. Permission to freely use, copy, modify, and distribute this software and
 its documentation without fee is hereby granted, provided that this notice and
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `thermoextrap-0.2.3/README.md` & `thermoextrap-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,141 +1,158 @@
-[![Repo][repo-badge]][repo-link]
-[![Docs][docs-badge]][docs-link]
+<!-- markdownlint-disable MD041 -->
+
+[![Repo][repo-badge]][repo-link] [![Docs][docs-badge]][docs-link]
 [![PyPI license][license-badge]][license-link]
 [![PyPI version][pypi-badge]][pypi-link]
 [![Conda (channel only)][conda-badge]][conda-link]
 [![Code style: black][black-badge]][black-link]
 
+<!-- For more badges, see
+https://shields.io/category/other
+https://naereen.github.io/badges/
+[pypi-badge]: https://badge.fury.io/py/thermoextrap
+-->
 
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
-[black-link]: https://github.com/ambv/black
+[black-link]: https://github.com/psf/black
 [pypi-badge]: https://img.shields.io/pypi/v/thermoextrap
-<!-- [pypi-badge]: https://badge.fury.io/py/thermoextrap -->
 [pypi-link]: https://pypi.org/project/thermoextrap
 [docs-badge]: https://img.shields.io/badge/docs-sphinx-informational
 [docs-link]: https://pages.nist.gov/thermoextrap/
 [repo-badge]: https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff
 [repo-link]: https://github.com/usnistgov/thermoextrap
 [conda-badge]: https://img.shields.io/conda/v/wpk-nist/thermoextrap
 [conda-link]: https://anaconda.org/wpk-nist/thermoextrap
-<!-- Use total link so works from anywhere -->
 [license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
-[license-link]: https://github.com/usnistgov/thermoextrap/blob/master/LICENSE
-<!-- For more badges, see https://shields.io/category/other and https://naereen.github.io/badges/ -->
-
-[numpy]: https://numpy.org
-[Numba]: https://numba.pydata.org/
-[xarray]: https://docs.xarray.dev/en/stable/
-[cmomy]: https://github.com/usnistgov/cmomy
-[gpr-link]: https://github.com/usnistgov/thermoextrap/tree/master/examples/gpr_active_learning
-[notebook-link]: https://github.com/usnistgov/thermoextrap/tree/master/examples/usage
+[license-link]: https://github.com/usnistgov/thermoextrap/blob/main/LICENSE
 
+<!-- other links -->
 
+[cmomy]: https://github.com/usnistgov/cmomy
+[gpr-link]:
+  https://github.com/usnistgov/thermoextrap/tree/main/examples/gpr_active_learning
+[notebook-link]:
+  https://github.com/usnistgov/thermoextrap/tree/main/examples/usage
 
 # `thermoextrap`: Thermodynamic Extrapolation/Interpolation Library
 
 This repository contains code used and described in references [^fn1] [^fn2].
 
-[^fn1]: [Extrapolation and Interpolation Strategies for Efficiently Estimating Structural Observables as a Function of Temperature and Density](https://doi.org/10.1063/5.0014282)
-
-[^fn2]: Leveraging Uncertainty Estimates and Derivative Information in Gaussian Process Regression for Expedited Data Collection in Molecular Simulations. In preparation.
+[^fn1]:
+    [Extrapolation and Interpolation Strategies for Efficiently Estimating Structural Observables as a Function of Temperature and Density](https://doi.org/10.1063/5.0014282)
 
+[^fn2]:
+    Leveraging Uncertainty Estimates and Derivative Information in Gaussian
+    Process Regression for Expedited Data Collection in Molecular Simulations.
+    In preparation.
 
 ## Overview
 
-If you find this code useful in producing published works, please provide an appropriate citation.
-Note that the second citation is focused on adding features that make use of GPR models based on derivative information produced by the core code base.
-For now, the GPR code, along with more information, may be found under [here][gpr-link].
-In a future release, we expect this to be fully integrated into the code base rather than a standalone module.
+If you find this code useful in producing published works, please provide an
+appropriate citation. Note that the second citation is focused on adding
+features that make use of GPR models based on derivative information produced by
+the core code base. For now, the GPR code, along with more information, may be
+found under [here][gpr-link]. In a future release, we expect this to be fully
+integrated into the code base rather than a standalone module.
 
 Code included here can be used to perform thermodynamic extrapolation and
 interpolation of observables calculated from molecular simulations. This allows
 for more efficient use of simulation data for calculating how observables change
 with simulation conditions, including temperature, density, pressure, chemical
 potential, or force field parameters. Users are highly encourage to work through
-the [Jupyter Notebooks][notebook-link] presenting examples for
-a variety of different observable functional forms. We only guarantee that this
-code is functional for the test cases we present here or for which it has
-previously been applied Additionally, the code may be in continuous development
-at any time. Use at your own risk and always check to make sure the produced
-results make sense. If bugs are found, please report them. If specific features
-would be helpful just let us know and we will be happy to work with you to come
-up with a solution.
-
+the [Jupyter Notebooks][notebook-link] presenting examples for a variety of
+different observable functional forms. We only guarantee that this code is
+functional for the test cases we present here or for which it has previously
+been applied Additionally, the code may be in continuous development at any
+time. Use at your own risk and always check to make sure the produced results
+make sense. If bugs are found, please report them. If specific features would be
+helpful just let us know and we will be happy to work with you to come up with a
+solution.
 
 ## Features
 
-* Fast calculation of derivatives
+- Fast calculation of derivatives
 
 ## Status
 
-This package is actively used by the author.  Please feel free to create a pull request for wanted features and suggestions!
-
+This package is actively used by the author. Please feel free to create a pull
+request for wanted features and suggestions!
 
 ## Quick start
 
 `thermoextrap` may be installed with either (recommended)
+
 ```bash
 conda install -c wpk-nist thermoextrap
 ```
+
 or
+
 ```bash
 pip install thermoextrap
 ```
 
 If you use pip, then you can include additional dependencies using
+
 ```bash
 pip install thermoextrap[all]
 ```
 
-If you install `thermoextrap` with conda, there are additional optional dependencies that take some care for installation.  We recommend installing the following via `pip`, as the versions on the conda/conda-forge channels are often a bit old.
+If you install `thermoextrap` with conda, there are additional optional
+dependencies that take some care for installation. We recommend installing the
+following via `pip`, as the versions on the conda/conda-forge channels are often
+a bit old.
+
 ```bash
 pip install tensorflow tensorflow-probability gpflow
 ```
 
 To install from source do the following:
+
 ```bash
 git clone git@github.com:usnistgov/thermoextrap.git
 cd thermoextrap
 pip install . [-e]
 ```
 
 To (optionally) include the example data do the following:
+
 ```bash
 git submodule update --init  --recursive
 ```
 
-
 ## Example usage
 
 ```python
 import thermoextrap
 
 ```
 
 <!-- end-docs -->
 
 ## Documentation
 
 See the [documentation][docs-link] for a look at `thermoextrap` in action.
 
-To have a look at using `thermoextrap` with Gaussian process regression, look in the [gpr][docs/notebooks/gpr] directory.
+To have a look at using `thermoextrap` with Gaussian process regression, look in
+the [gpr](examples/usage/gpr) and
+[gpr_active_learning](examples/gpr_active_learning) directories.
 
 ## License
 
-This is free software.  See [LICENSE][license-link].
+This is free software. See [LICENSE][license-link].
 
 ## Related work
 
 This package extensively uses the [cmomy] package to handle central comoments.
 
+## Contact
 
-# Contact
-Questions may be addressed to Bill Krekelberg at william.krekelberg@nist.gov or Jacob Monroe at jacob.monroe@uark.edu.
-
+Questions may be addressed to Bill Krekelberg at william.krekelberg@nist.gov or
+Jacob Monroe at jacob.monroe@uark.edu.
 
 ## Credits
 
 This package was created with
 [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
 [wpk-nist-gov/cookiecutter-pypackage](https://github.com/wpk-nist-gov/cookiecutter-pypackage)
 Project template forked from
```

### Comparing `thermoextrap-0.2.3/environment/dev-extras.yaml` & `thermoextrap-0.3.0/environment/dev-extras.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 dependencies:
-    # numerics/tests
-    - matplotlib
-    # - pandas
-    # development
-    # - isort
-    # - black
-    # - blackdoc
-    # - flake8
-    # testing
-    - pytest
-    - pytest-cov
-    - pytest-xdist
-    # - tox-conda
-    # specials
-    # - pre-commit
-    # repl
-    - ipython
-    - ipykernel
-    - nbconvert
-    # build
-    - setuptools-scm
-    # - setuptools
-    # - twine
-    # - setuptools_scm_git_archive
-    # - build
-    # conda specific
-    # - conda-build
-    # - anaconda-client
-    # - greyskull
-    # doc stuff
-    # - sphinx
-    # - sphinx_rtd_theme
-    # - recommonmark # if want markdown
-    # - nbsphinx # if want notebooks
-    # - sphinxcontrib-spelling
-    # - sphinx-toolbox
-    # lsp stuff
-    # - autoflake
-    # - pyls-mypy
-    # - pyls-black
-    # - pyls-isort
-    # mypy
-    # - mypy
-    # - pytest-mypy
-    # # Monkeytype: autocreate type hints
-    # - MonkeyType
-    # - pip
-    # - pip:
-    #     - pytest-accept
-    #     - mypy-extensions
-    #     - pytest-monkeytype
-    #     - flake8-mypy
-    #     - attr-utils
-    #     spelling?
-    #     - pyenchant
+  # numerics/tests
+  - matplotlib
+  # - pandas
+  # development
+  # - isort
+  # - black
+  # - blackdoc
+  # - flake8
+  # testing
+  - pytest
+  - pytest-cov
+  - pytest-xdist
+  # - tox-conda
+  # specials
+  # - pre-commit
+  # repl
+  - ipython
+  - ipykernel
+  - nbconvert
+  # build
+  - setuptools-scm
+  # - setuptools
+  # - twine
+  # - setuptools_scm_git_archive
+  # - build
+  # conda specific
+  # - conda-build
+  # - anaconda-client
+  # - greyskull
+  # doc stuff
+  # - sphinx
+  # - sphinx_rtd_theme
+  # - recommonmark # if want markdown
+  # - nbsphinx # if want notebooks
+  # - sphinxcontrib-spelling
+  # - sphinx-toolbox
+  # lsp stuff
+  # - autoflake
+  # - pyls-mypy
+  # - pyls-black
+  # - pyls-isort
+  # mypy
+  # - mypy
+  # - pytest-mypy
+  # # Monkeytype: autocreate type hints
+  # - MonkeyType
+  # - pip
+  # - pip:
+  #     - pytest-accept
+  #     - mypy-extensions
+  #     - pytest-monkeytype
+  #     - flake8-mypy
+  #     - attr-utils
+  #     spelling?
+  #     - pyenchant
```

### Comparing `thermoextrap-0.2.3/environment/docs-extras.yaml` & `thermoextrap-0.3.0/environment/docs-extras.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 channels:
   - conda-forge
 dependencies:
-    - setuptools-scm
-    - ipython
-    ## package deps
-    - matplotlib
-    # - pandas
-    - pip
-    - pip:
-        - pyenchant
-        # TODO: something goes wonky with sphinx-book-theme and higher versions of sphinx
-        - ghp-import
-        - sphinx
-        ## themes
-        - sphinx-book-theme
-        ## error with == 0.13.3
-        - pydata-sphinx-theme==0.13.1
-        ## optionals
-        # sphinx-design
-        - sphinx-copybutton
-        - sphinxcontrib-spelling
-        # sphinxext-rediraffe
-        ## autobuild
-        - sphinx-autobuild
-        ## myst
-        # myst-parser
-        - myst-nb
-        ## others
-        - autodocsumm
+  - setuptools-scm
+  - ipython
+  ## package deps
+  - matplotlib
+  # - pandas
+  - pip
+  - pip:
+      - pyenchant
+      # TODO: something goes wonky with sphinx-book-theme and higher versions of sphinx
+      - ghp-import
+      - sphinx
+      ## themes
+      - sphinx-book-theme
+      ## error with == 0.13.3
+      - pydata-sphinx-theme==0.13.1
+      ## optionals
+      # sphinx-design
+      - sphinx-copybutton
+      - sphinxcontrib-spelling
+      # sphinxext-rediraffe
+      ## autobuild
+      - sphinx-autobuild
+      ## myst
+      # myst-parser
+      - myst-nb
+      ## others
+      - autodocsumm
```

### Comparing `thermoextrap-0.2.3/src/thermoextrap/__init__.py` & `thermoextrap-0.3.0/src/thermoextrap/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """Classes/routines to deal with thermodynamic extrapolation."""
 
-from . import beta, lnpi, volume, volume_idealgas
-from .core import data, idealgas, models
-from .core.data import (
+# TODO: move data, idealgas, models to top level.
+from . import beta, data, idealgas, lnpi, models, volume, volume_idealgas
+from .core.xrutils import xrwrap_alpha, xrwrap_uv, xrwrap_xv
+from .data import (
     DataCentralMoments,
     DataCentralMomentsVals,
     DataValues,
     DataValuesCentral,
     factory_data_values,
     resample_indices,
 )
 
 # expose some data/models
-from .core.models import (
+from .models import (
     Derivatives,
     ExtrapModel,
     ExtrapWeightedModel,
     InterpModel,
     InterpModelPiecewise,
     MBARModel,
     PerturbModel,
     StateCollection,
 )
-from .core.xrutils import xrwrap_alpha, xrwrap_uv, xrwrap_xv
 
 # updated versioning scheme
 try:
     from importlib.metadata import version as _version
 except ImportError:
     # if the fallback library is missing, we are doomed.
     from importlib_metadata import version as _version  # type: ignore[no-redef]
```

### Comparing `thermoextrap-0.2.3/src/thermoextrap/adaptive_interp.py` & `thermoextrap-0.3.0/src/thermoextrap/adaptive_interp.py`

 * *Files 0% similar despite different names*

```diff
@@ -532,16 +532,16 @@
     See Also
     --------
     thermoextrap.idealgas
     thermoextrap.beta.factory_extrapmodel
     """
 
     from . import beta as xpan_beta
-    from .core import idealgas
-    from .core.data import DataCentralMomentsVals
+    from . import idealgas
+    from .data import DataCentralMomentsVals
 
     # NOTE: this is for reproducible results.
     if seed_from_beta:
         np.random.seed(int(beta * 1000))
 
     xdata, udata = idealgas.generate_data(shape=(nconfig, npart), beta=beta)
     data = DataCentralMomentsVals.from_vals(xv=xdata, uv=udata, order=order)
@@ -570,15 +570,15 @@
         Note that this is redundant with `maxdepth`, but for demonstration
         purposes
     ax : :class:`matplotlib.axes.Axes`, optional
     """
 
     import matplotlib.pyplot as plt
 
-    from .core import idealgas
+    from . import idealgas
 
     if verbose:
         print("depth:", info_dict["depth"])
         print("alphas:", model.alpha0)
 
     if ax is None:
         _, ax = plt.subplots()
```

### Comparing `thermoextrap-0.2.3/src/thermoextrap/beta.py` & `thermoextrap-0.3.0/src/thermoextrap/beta.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 ====================================================================
 """
 
 
 from functools import lru_cache
 from typing import Literal
 
-from .core._docstrings import factory_docfiller_shared
-from .core.models import (
+from .docstrings import DOCFILLER_SHARED
+from .models import (
     Derivatives,
     ExtrapModel,
     PerturbModel,
     SymDerivBase,
     SymFuncBase,
     SymSubs,
     get_default_indexed,
     get_default_symbol,
 )
 
-docfiller_shared = factory_docfiller_shared(names=("default", "beta"))
+docfiller_shared = DOCFILLER_SHARED.levels_to_top("cmomy", "xtrap", "beta").decorate
 
 ##############################################################################
 # recursive deriatives for beta expansion
 ###############################################################################
 
 ####################
 # Central moments
@@ -688,11 +688,11 @@
     perturbmodel : :class:`thermoextrap.models.PerturbModel`
 
 
     See Also
     --------
     ~thermoextrap.models.PerturbModel
     """
-    from .core.data import factory_data_values
+    from .data import factory_data_values
 
     data = factory_data_values(uv=uv, xv=xv, order=0, central=False, **kws)
     return PerturbModel(alpha0=beta, data=data, alpha_name=alpha_name)
```

### Comparing `thermoextrap-0.2.3/src/thermoextrap/core/_attrs_utils.py` & `thermoextrap-0.3.0/src/thermoextrap/core/_attrs_utils.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.3/src/thermoextrap/core/_deprecate.py` & `thermoextrap-0.3.0/src/thermoextrap/core/_deprecate.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.3/src/thermoextrap/core/data.py` & `thermoextrap-0.3.0/src/thermoextrap/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,44 +20,41 @@
 import attrs
 import numpy as np
 import xarray as xr
 from attrs import converters as attc
 from attrs import field
 from attrs import validators as attv
 from custom_inherit import DocInheritMeta
+from module_utilities import cached
 
-from ._attrs_utils import (
+from .core._attrs_utils import (
     MyAttrsMixin,
     _cache_field,
     convert_dims_to_tuple,
     kw_only_field,
 )
-from ._docstrings import factory_docfiller_shared
-from .cached_decorators import gcached
-from .xrutils import xrwrap_uv, xrwrap_xv
+from .core.xrutils import xrwrap_uv, xrwrap_xv
+from .docstrings import DOCFILLER_SHARED
 
 try:
     from cmomy import xCentralMoments
 
     _HAS_CMOMY = True
 except ImportError:
     _HAS_CMOMY = False
 
 
-docfiller_shared = factory_docfiller_shared(
-    names=("default",),
-)
+docfiller_shared = DOCFILLER_SHARED.levels_to_top("cmomy", "xtrap").decorate
 
 __all__ = [
     "DataCentralMoments",
     "DataCentralMomentsVals",
     "DataValues",
     "DataValuesCentral",
     "DataCallbackABC",
-    "AbstractData",
     "factory_data_values",
     "resample_indices",
 ]
 
 
 @docfiller_shared
 def resample_indices(size, nrep, rec_dim="rec", rep_dim="rep", replace=True):
@@ -183,15 +180,14 @@
 
     DataCallback can be subclassed to fine tune things.
     """
 
     @abstractmethod
     def check(self, data):
         """Perform any consistency checks between self and data."""
-        pass
 
     @abstractmethod
     def derivs_args(self, data, derivs_args):
         """
         Adjust derivs args from data class.
 
         should return a tuple
@@ -224,15 +220,14 @@
     Basic version of DataCallbackABC.
 
     Implemented to pass things through unchanged.  Will be used for default construction
     """
 
     def check(self, data):
         """Perform any consistency checks between self and data."""
-        pass
 
     def derivs_args(self, data, derivs_args):
         """
         Adjust derivs args from data class.
 
         should return a tuple
         """
@@ -279,21 +274,19 @@
             raise ValueError("meta must be None or subclass of DataCallbackABC")
         meta.check(data=self)
 
     @property
     @abstractmethod
     def central(self):
         """Whether central (True) or raw (False) moments are used."""
-        pass
 
     @property
     @abstractmethod
     def derivs_args(self):
         """Sequence of arguments to derivative calculation function."""
-        pass
 
     @abstractmethod
     def __len__(self):
         pass
 
     @abstractmethod
     def resample(self, indices=None, nrep=None, **kwargs):
@@ -761,15 +754,15 @@
 
 @attrs.define
 class DataValues(DataValuesBase):
     """Class to hold uv/xv data."""
 
     _CENTRAL = False
 
-    @gcached(prop=False)
+    @cached.meth
     def _mean(self, skipna=None):
         if skipna is None:
             skipna = self.skipna
 
         return build_aves_xu(
             uv=self.uv,
             xv=self.xv,
@@ -777,42 +770,42 @@
             skipna=skipna,
             rec_dim=self.rec_dim,
             umom_dim=self.umom_dim,
             deriv_dim=self.deriv_dim,
             **self.build_aves_kws,
         )
 
-    @gcached()
+    @cached.prop
     def xu(self):
         """Average of `x * u ** n`."""
         out = self._mean()[1]
         if self.compute:
             out = out.compute()
         return out
 
-    @gcached()
+    @cached.prop
     def u(self):
         """Average of `u ** n`."""
         if self.x_isnot_u:
             out = self._mean()[0]
             if self.compute:
                 out = out.compute()
         else:
             out = _xu_to_u(self.xu, self.umom_dim)
 
         return out
 
-    @gcached()
+    @cached.prop
     def u_selector(self):
         """Indexer for `self.u`."""
         return DatasetSelector.from_defaults(
             self.u, deriv_dim=None, mom_dim=self.umom_dim
         )
 
-    @gcached()
+    @cached.prop
     def xu_selector(self):
         """Indexer for `self.xu`."""
         return DatasetSelector.from_defaults(
             self.xu, deriv_dim=self.deriv_dim, mom_dim=self.umom_dim
         )
 
     @property
@@ -826,15 +819,15 @@
 
 @attrs.define
 class DataValuesCentral(DataValuesBase):
     """Data class using values and central moments."""
 
     _CENTRAL = True
 
-    @gcached(prop=False)
+    @cached.meth
     def _mean(self, skipna=None):
         if skipna is None:
             skipna = self.skipna
 
         return build_aves_dxdu(
             uv=self.uv,
             xv=self.xv,
@@ -842,55 +835,55 @@
             skipna=skipna,
             rec_dim=self.rec_dim,
             umom_dim=self.umom_dim,
             deriv_dim=self.deriv_dim,
             **self.build_aves_kws,
         )
 
-    @gcached()
+    @cached.prop
     def xave(self):
         """Averages of `x`."""
         out = self._mean()[0]
         if self.compute:
             out = out.compute()
         return out
 
-    @gcached()
+    @cached.prop
     def dxdu(self):
         """Averages of `dx * du ** n`."""
         out = self._mean()[2]
         if self.compute:
             out = out.compute()
         return out
 
-    @gcached()
+    @cached.prop
     def du(self):
         """Averages of `du ** n`."""
         if self.x_isnot_u:
             out = self._mean()[1]
             if self.compute:
                 out = out.compute()
         else:
             out = _xu_to_u(self.dxdu, dim=self.umom_dim)
 
         return out
 
-    @gcached()
+    @cached.prop
     def du_selector(self):
         return DatasetSelector.from_defaults(
             self.du, deriv_dim=None, mom_dim=self.umom_dim
         )
 
-    @gcached()
+    @cached.prop
     def dxdu_selector(self):
         return DatasetSelector.from_defaults(
             self.dxdu, deriv_dim=self.deriv_dim, mom_dim=self.umom_dim
         )
 
-    @gcached()
+    @cached.prop
     def xave_selector(self):
         if self.deriv_dim is None:
             return self.xave
         else:
             return DatasetSelector.from_defaults(self.xave, dims=[self.deriv_dim])
 
     @property
@@ -1029,95 +1022,95 @@
         See Also
         --------
         cmomy.xCentralMoments.values
 
         """
         return self.dxduave.values
 
-    @gcached(prop=False)
+    @cached.meth
     def rmom(self):
         """Raw co-moments."""
         return self.dxduave.rmom()
 
-    @gcached(prop=False)
+    @cached.meth
     def cmom(self):
         """Central co-moments."""
         return self.dxduave.cmom()
 
-    @gcached()
+    @cached.prop
     def xu(self):
         """Averages of form ``x * u ** n``."""
         return self.rmom().sel(**{self.xmom_dim: 1}, drop=True)
 
-    @gcached()
+    @cached.prop
     def u(self):
         """Averages of form ``u ** n``."""
         if self.x_isnot_u:
             out = self.rmom().sel(**{self.xmom_dim: 0}, drop=True)
             if self.xalpha:
                 out = out.sel(**{self.deriv_dim: 0}, drop=True)
         else:
             out = _xu_to_u(self.xu, self.umom_dim)
 
         return out
 
-    @gcached()
+    @cached.prop
     def xave(self):
         """Averages of form observable ``x``."""
         return self.dxduave.values.sel(
             **{self.umom_dim: 0, self.xmom_dim: 1}, drop=True
         )
 
-    @gcached()
+    @cached.prop
     def dxdu(self):
         """Averages of form ``dx * dx ** n``."""
         return self.cmom().sel(**{self.xmom_dim: 1}, drop=True)
 
-    @gcached()
+    @cached.prop
     def du(self):
         """Averages of ``du ** n``."""
         if self.x_isnot_u:
             out = self.cmom().sel(**{self.xmom_dim: 0}, drop=True)
             if self.xalpha:
                 out = out.sel(**{self.deriv_dim: 0}, drop=True)
         else:
             out = _xu_to_u(self.dxdu, self.umom_dim)
 
         return out
 
-    @gcached()
+    @cached.prop
     def u_selector(self):
         """Indexer for ``u_selector[n] = u ** n``."""
         return DatasetSelector.from_defaults(
             self.u, deriv_dim=None, mom_dim=self.umom_dim
         )
 
-    @gcached()
+    @cached.prop
     def xu_selector(self):
         """Indexer for ``xu_select[n] = x * u ** n``."""
         return DatasetSelector.from_defaults(
             self.xu, deriv_dim=self.deriv_dim, mom_dim=self.umom_dim
         )
 
-    @gcached()
+    @cached.prop
     def xave_selector(self):
         """Selector for ``xave``."""
         if self.deriv_dim is None:
             return self.xave
         else:
             return DatasetSelector(self.xave, dims=[self.deriv_dim])
 
-    @gcached()
+    @cached.prop
     def du_selector(self):
         """Selector for ``du_selector[n] = du ** n``."""
         return DatasetSelector.from_defaults(
             self.du, deriv_dim=None, mom_dim=self.umom_dim
         )
 
-    @gcached()
+    @cached.prop
     def dxdu_selector(self):
         """Selector for ``dxdu_selector[n] = dx * du ** n``."""
         return DatasetSelector.from_defaults(
             self.dxdu, deriv_dim=self.deriv_dim, mom_dim=self.umom_dim
         )
 
     @property
```

### Comparing `thermoextrap-0.2.3/src/thermoextrap/core/idealgas.py` & `thermoextrap-0.3.0/src/thermoextrap/idealgas.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 from functools import lru_cache
 
 import numpy as np
 import sympy as sp
 
-from ._docstrings import DocFiller
+from .docstrings import DocFiller
 
 __all__ = [
     "x_ave",
     "x_var",
     "x_prob",
     "u_prob",
     "x_cdf",
@@ -63,15 +63,17 @@
 vol0 : float
     Reference volume.
 shape : int or tuple of int
     Shape of output.  Ignored if ``r`` is not ``None``.
 """
 
 
-docfiller_shared = DocFiller.from_docstring(_shared_docs, combine_keys="parameters")()
+docfiller_shared = DocFiller.from_docstring(
+    _shared_docs, combine_keys="parameters"
+).decorate
 
 
 # global variables
 beta_sym, vol_sym = sp.symbols("beta_sym vol_sym")
 xave_sym = (1 / beta_sym) - vol_sym / (sp.exp(beta_sym * vol_sym) - 1)
```

### Comparing `thermoextrap-0.2.3/src/thermoextrap/core/models.py` & `thermoextrap-0.3.0/src/thermoextrap/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,35 +12,33 @@
 import pandas as pd
 import sympy as sp
 import xarray as xr
 from attrs import converters as attc
 from attrs import field
 from attrs import validators as attv
 from custom_inherit import DocInheritMeta
+from module_utilities import cached
 from scipy.special import factorial as sp_factorial
 
-from thermoextrap.core.data import AbstractData, kw_only_field
-
-from ._attrs_utils import MyAttrsMixin, _cache_field
-from ._docstrings import factory_docfiller_shared
-from .cached_decorators import gcached
-from .sputils import get_default_indexed, get_default_symbol
-from .xrutils import xrwrap_alpha
+from .core._attrs_utils import MyAttrsMixin, _cache_field
+from .core.sputils import get_default_indexed, get_default_symbol
+from .core.xrutils import xrwrap_alpha
+from .data import AbstractData, kw_only_field
+from .docstrings import DOCFILLER_SHARED
 
 try:
     from pymbar import mbar
 
     _HAS_PYMBAR = True
 except ImportError:
     _HAS_PYMBAR = False
 
 
-docfiller_shared = factory_docfiller_shared(
-    names="default",
-)
+docfiller_shared = DOCFILLER_SHARED.levels_to_top("cmomy", "xtrap").decorate
+
 
 __all__ = [
     "ExtrapModel",
     "ExtrapWeightedModel",
     "InterpModel",
     "InterpModelPiecewise",
     "MBARModel",
@@ -56,15 +54,15 @@
 class SymFuncBase(sp.Function):
     """
     Base class to define a sympy function for user defined deriatives.
 
 
     See Also
     --------
-    :class:`thermoextrap.core.models.SymDerivBase`
+    :class:`thermoextrap.models.SymDerivBase`
 
     """
 
     @classmethod
     def deriv_args(cls):
         """
         Symbol arguments of function.
@@ -74,15 +72,15 @@
         See Also
         --------
         sympy.utilities.lambdify.lambdify
         """
         raise NotImplementedError("must specify in sublcass")
 
     def fdiff(self, argindex=1):
-        """Derivative of function.  This will be used by :class:`thermoextrap.core.models.SymDerivBase`."""
+        """Derivative of function.  This will be used by :class:`thermoextrap.models.SymDerivBase`."""
         raise NotImplementedError("must specify in subclass")
 
     @classmethod
     def eval(cls, beta):
         """
         Evaluate function.
 
@@ -97,15 +95,15 @@
     """
     Base class for working with recursive derivatives in expansions.
 
     Parameters
     ----------
     func : symFunction
         Function to differentiate.  This should (most likely) be an instance
-        of :class:`thermoextrap.core.models.SymFuncBase`
+        of :class:`thermoextrap.models.SymFuncBase`
     args : sequence of Symbol
         Arguments to func
     {expand}
     {post_func}
     """
 
     def __init__(self, func, args=None, expand=True, post_func=None):
@@ -128,29 +126,29 @@
                     )
             func = post_func(func)
 
         self.func = func
         self.args = args
         self.expand = expand
 
-    @gcached(prop=False)
+    @cached.meth
     def __getitem__(self, order):
         if order == 0:
             out = self.func
         else:
             out = self[order - 1].diff(self.beta, 1)
             if self.expand:
                 out = out.expand()
         return out
 
 
 @attrs.define
 class SymSubs:
     """
-    Class to handle substitution on :class:`thermoextrap.core.models.SymDerivBase`.
+    Class to handle substitution on :class:`thermoextrap.models.SymDerivBase`.
 
     Parameters
     ----------
     funcs : sequence of SymFunction
         Symbolic functions to consider.
     subs : Sequence, optional
         Substitutions.
@@ -172,15 +170,15 @@
     subs_all: Mapping | None = field(default=None)
     recursive: bool = field(default=True)
     simplify: bool = field(default=False)
     expand: bool = field(default=True)
 
     _cache: dict = _cache_field()
 
-    @gcached(prop=False)
+    @cached.meth
     def __getitem__(self, order):
         func = self.funcs[order]
 
         if self.subs is not None:
             if self.recursive:
                 for o in range(order, -1, -1):
                     func = func.subs(self.subs[o])
@@ -225,15 +223,15 @@
     args: Sequence | None = field(default=None)
     lambdify_kws: Mapping | None = kw_only_field(
         default=None, converter=attc.default_if_none(factory=dict)
     )
 
     _cache: dict = _cache_field()
 
-    @gcached(prop=False)
+    @cached.meth
     def __getitem__(self, order):
         return sp.lambdify(self.args, self.exprs[order], **self.lambdify_kws)
 
     @classmethod
     def from_u_xu(cls, exprs, **lambdify_kws):
         """Factory for u/xu args."""
         u, xu = get_default_indexed("u", "xu")
@@ -253,15 +251,15 @@
 
 # -log<X>
 class SymMinusLog:
     """Class to compute derivatives of Y = -log(<X>)."""
 
     X, dX = get_default_indexed("X", "dX")
 
-    @gcached(prop=False)
+    @cached.meth
     def __getitem__(self, order):
         if order == 0:
             return -sp.log(self.X[0])
 
         expr = 0
         for k in range(1, order + 1):
             expr += (
@@ -440,15 +438,15 @@
         default=False, converter=attc.default_if_none(False)
     )
     #: Name of `alpha`
     alpha_name: str = kw_only_field(default="alpha", converter=str)
 
     _cache: dict = _cache_field()
 
-    @gcached(prop=False)
+    @cached.meth
     def _derivs(self, order, order_dim, minus_log):
         return self.derivatives.derivs(
             data=self.data,
             order=order,
             norm=False,
             minus_log=minus_log,
             order_dim=order_dim,
@@ -849,15 +847,15 @@
         return out
 
 
 @attrs.define
 class InterpModel(StateCollection):
     """Interpolation model."""
 
-    @gcached(prop=False)
+    @cached.meth
     def coefs(self, order=None, order_dim="porder", minus_log=None):
         if order is None:
             order = self.order
 
         porder = len(self) * (order + 1) - 1
 
         # keep track of these to reconstruct index later
@@ -928,18 +926,18 @@
         out = (prefac * coefs).sum(order_dim)
         return out
 
 
 class InterpModelPiecewise(StateCollection, PiecewiseMixin):
     """Apposed to the multiple model InterpModel, perform a piecewise interpolation."""
 
-    # @gcached(prop=False)
+    # @cached.meth
     # def single_interpmodel(self, state0, state1):
     #     return InterpModel([state0, state1])
-    @gcached(prop=False)
+    @cached.meth
     def single_interpmodel(self, *state_indices):
         state0, state1 = (self[i] for i in state_indices)
         return InterpModel([state0, state1])
 
     def predict(
         self,
         alpha,
@@ -1050,15 +1048,15 @@
 class MBARModel(StateCollection):
     """Sadly, this doesn't work as beautifully."""
 
     def __attrs_pre_init__(self):
         if not _HAS_PYMBAR:
             raise ImportError("need pymbar to use this")
 
-    @gcached(prop=False)
+    @cached.meth
     def _default_params(self, state_dim="state", alpha_name="alpha"):
         # all xvalues:
         xv = xr.concat([m.data.xv for m in self], dim=state_dim)
         uv = xr.concat([m.data.uv for m in self], dim=state_dim)
         alpha0 = xrwrap_alpha([m.alpha0 for m in self], name=alpha_name)
 
         # make sure uv, xv in correct orde
```

### Comparing `thermoextrap-0.2.3/src/thermoextrap/core/stack.py` & `thermoextrap-0.3.0/src/thermoextrap/stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """A set of routines to stack data for gpflow analysis."""
 
 
 import numpy as np
 import pandas as pd
 import xarray as xr
+from module_utilities import cached
 
-from .cached_decorators import gcached
 from .models import StateCollection
 
 
 def stack_dataarray(
     da,
     x_dims,
     y_dims=None,
@@ -266,15 +266,15 @@
         """Maximum order available."""
         return self.da.sizes[self.order_dim] - 1
 
     @property
     def alpha_name(self):
         return self.x_dims[0]
 
-    @gcached(prop=False)
+    @cached.meth
     def _stacked(self, order):
         da = self.da
         if order is not None:
             # select orders up to and including order
             da = da.isel(**{self.order_dim: slice(None, order + 1)})
 
         return stack_dataarray(
@@ -478,16 +478,14 @@
 
 
         See Also
         --------
         `StackedDerivatives.from_derivs`
         """
 
-        from .models import StateCollection
-
         if not isinstance(states, StateCollection):
             states = StateCollection(states)
 
         if resample:
             if resample_kws is None:
                 resample_kws = {}
             states = states.resample(**resample_kws)
@@ -573,15 +571,15 @@
             deriv_kws=self.deriv_kws,
         )
 
     @property
     def order_dim(self):
         return self.x_dims[-1]
 
-    @gcached(prop=False)
+    @cached.meth
     def _stacked(self, order):
         """
         Get stacked data representation.
 
         Parameters
         ----------
         order : int
```

### Comparing `thermoextrap-0.2.3/src/thermoextrap/core/xrutils.py` & `thermoextrap-0.3.0/src/thermoextrap/core/xrutils.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.3/src/thermoextrap/gpr_active/__init__.py` & `thermoextrap-0.3.0/src/thermoextrap/gpr_active/__init__.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.3/src/thermoextrap/gpr_active/active_utils.py` & `thermoextrap-0.3.0/src/thermoextrap/gpr_active/active_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 import sympy as sp
 
 # import tensorflow as tf
 import xarray as xr
 from pymbar import timeseries
 from scipy import integrate, linalg, special
 
-from .. import DataCentralMomentsVals, ExtrapModel
 from .. import beta as xpan_beta
+from ..data import DataCentralMomentsVals
+from ..models import ExtrapModel
 from .gp_models import (
     ConstantMeanWithDerivs,
     DerivativeKernel,
     HeteroscedasticGPR,
     LinearWithDerivs,
 )
```

### Comparing `thermoextrap-0.2.3/src/thermoextrap/gpr_active/gp_models.py` & `thermoextrap-0.3.0/src/thermoextrap/gpr_active/gp_models.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.3/src/thermoextrap/gpr_active/ig_active.py` & `thermoextrap-0.3.0/src/thermoextrap/gpr_active/ig_active.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 learning strategies.
 """
 
 import numpy as np
 import xarray as xr
 
 from .. import beta as xpan_beta
-from ..core import idealgas
-from ..core.data import DataCentralMomentsVals
+from .. import idealgas
+from ..data import DataCentralMomentsVals
 from .active_utils import DataWrapper
 
 
 # Work with fixed ideal gas test set in thermoextrap
 # Define function to create ExtrapModel of ideal gas data
 # This will be handy later on
 def extrap_IG(beta, seed=42):
```

### Comparing `thermoextrap-0.2.3/src/thermoextrap/gpr_active/sine_active.py` & `thermoextrap-0.3.0/src/thermoextrap/gpr_active/sine_active.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.3/src/thermoextrap/legacy/__init__.py` & `thermoextrap-0.3.0/src/thermoextrap/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.3/src/thermoextrap/legacy/extrap.py` & `thermoextrap-0.3.0/src/thermoextrap/legacy/extrap.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.3/src/thermoextrap/legacy/gpr.py` & `thermoextrap-0.3.0/src/thermoextrap/legacy/gpr.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import gpflow
 import numpy as np
 import sympy as sp
 import tensorflow as tf
 import xarray as xr
 from gpflow.ci_utils import ci_niter
 
-from .core.models import StateCollection
+from .models import StateCollection
 
 
 # First define classes needed for a GPR model
 # A general derivative kernel based on a sympy expression
 class DerivativeKernel(gpflow.kernels.Kernel):
     """
         Creates a kernel that can be differentiated based on a sympy expression for the kernel.
```

### Comparing `thermoextrap-0.2.3/src/thermoextrap/legacy/gpr_stack.py` & `thermoextrap-0.3.0/src/thermoextrap/legacy/gpr_stack.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 import gpflow
 import numpy as np
 import sympy as sp
 import tensorflow as tf
 import xarray as xr
 from gpflow.ci_utils import ci_niter
+from module_utilities import cached
 
-# from .models import StateCollection
-from .core.cached_decorators import gcached
-from .core.stack import GPRData, StackedDerivatives, multiindex_to_array
+
+from ..stack import GPRData, StackedDerivatives, multiindex_to_array
 
 __all__ = ("GPRData", "GPRModel", "StackedDerivatives", "factory_gprmodel")
 
 # First define classes needed for a GPR model
 # A general derivative kernel based on a sympy expression
 
 
@@ -218,15 +218,15 @@
             )
             inds_list.append(this_inds)
 
         k_list = tf.dynamic_stitch(inds_list, k_list)
         k_diag = tf.reshape(k_list, (x1.shape[0],))
         return k_diag
 
-    @gcached(prop=False)
+    @cached.meth
     def _lambda_kernel(self, d1, d2):
         expr = sp.diff(self.kernel_expr, self.x_syms[0], d1, self.x_syms[1], d2)
 
         return sp.lambdify(
             (self.x_syms[0], self.x_syms[1], *self.param_syms),
             expr,
             modules="tensorflow",
@@ -299,30 +299,30 @@
     """
 
     def __init__(self, data, kernel_expr, kernel_params={}):
         self.data = data
         self.kernel_expr = kernel_expr
         self.kernel_params = kernel_params
 
-    @gcached(prop=False)
+    @cached.meth
     def kern(self, out_dim):
         return [
             DerivativeKernel(
                 self.kernel_expr,
                 1,  # for now, obs_dims is always 1 while figure out math
                 kernel_params=self.kernel_params,
             )
             for _ in range(out_dim)
         ]
 
-    @gcached(prop=False)
+    @cached.meth
     def het_gauss(self, out_dim):
         return [HeteroscedasticGaussian() for _ in range(out_dim)]
 
-    @gcached(prop=False)
+    @cached.meth
     def gp_params(self, order):
         x, ys = self.data.array_data(order=order)
         out_dim = len(ys)
 
         kernels = self.kern(out_dim)
         likelihoods = self.het_gauss(out_dim)
```

### Comparing `thermoextrap-0.2.3/src/thermoextrap/legacy/ig.py` & `thermoextrap-0.3.0/src/thermoextrap/legacy/ig.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.3/src/thermoextrap/legacy/interp.py` & `thermoextrap-0.3.0/src/thermoextrap/legacy/interp.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.3/src/thermoextrap/legacy/old_scripts.py` & `thermoextrap-0.3.0/src/thermoextrap/legacy/old_scripts.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.3/src/thermoextrap/legacy/recursive_interp.py` & `thermoextrap-0.3.0/src/thermoextrap/legacy/recursive_interp.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.3/src/thermoextrap/legacy/reweight.py` & `thermoextrap-0.3.0/src/thermoextrap/legacy/reweight.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.3/src/thermoextrap/legacy/utilities.py` & `thermoextrap-0.3.0/src/thermoextrap/legacy/utilities.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.3/src/thermoextrap/lnpi.py` & `thermoextrap-0.3.0/src/thermoextrap/lnpi.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,27 +17,24 @@
 import numpy as np
 import xarray as xr
 
 # from attrs import converters as attc
 from attrs import field
 from attrs import validators as attv
 from cmomy import xCentralMoments
+from module_utilities import cached
 
 from . import beta as beta_xpan
-
-# from .beta import ExtrapModel, SymDerivBeta, u_func, u_func_central
-# from .beta import factory_derivatives as factory_derivatives_beta
 from .core._attrs_utils import _cache_field, convert_dims_to_tuple
-from .core._docstrings import factory_docfiller_shared
-from .core.cached_decorators import gcached
-from .core.data import DataCallbackABC
-from .core.models import Derivatives, ExtrapModel, SymFuncBase, SymSubs
 from .core.sputils import get_default_indexed, get_default_symbol
+from .data import DataCallbackABC
+from .docstrings import DOCFILLER_SHARED
+from .models import Derivatives, ExtrapModel, SymFuncBase, SymSubs
 
-docfiller_shared = factory_docfiller_shared(names=("default", "beta"))
+docfiller_shared = DOCFILLER_SHARED.levels_to_top("cmomy", "xtrap", "beta").decorate
 
 
 ################################################################################
 # lnPi correction stuff
 ################################################################################
 class lnPi_func_central(SymFuncBase):
     r"""
@@ -256,15 +253,15 @@
     def lnPi0_ave(self):
         if isinstance(self.lnPi0, xr.DataArray):
             return self.lnPi0
         else:
             # assume lnPi0 is an averaging object ala cmomy
             return self.lnPi0.values
 
-    @gcached()
+    @cached.prop
     def mudotN(self):
         """Dot product of `self.mu` and `self.ncoords`, reduces along `self.dims_comp`."""
         return xr.dot(self.mu, self.ncoords, dims=self.dims_comp)
 
     def resample(self, data, meta_kws=None, **kws):
         """Resample lnPi0 data."""
```

### Comparing `thermoextrap-0.2.3/src/thermoextrap/recursive_interp.py` & `thermoextrap-0.3.0/src/thermoextrap/recursive_interp.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 # import xarray as xr
 from scipy import stats
 
 # TODO: Change this to point to the "new" ideagas.py
 # TODO: rework this code to be cleaner
 # from ..legacy.ig import IGmodel
-from .core import idealgas
+from . import idealgas
 from .core._deprecate import deprecate, deprecate_kwarg
-from .core.data import factory_data_values
-from .core.models import ExtrapModel, InterpModel
+from .data import factory_data_values
+from .models import ExtrapModel, InterpModel
 
 try:
     import matplotlib.pyplot as plt
 
     _HAS_PLT = True
 except ImportError:
     _HAS_PLT = False
```

### Comparing `thermoextrap-0.2.3/src/thermoextrap/volume.py` & `thermoextrap-0.3.0/src/thermoextrap/volume.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,26 +9,25 @@
 
 from functools import lru_cache
 
 import attrs
 import xarray as xr
 from attrs import field
 from attrs import validators as attv
+from module_utilities import cached
 
 from .core._attrs_utils import _cache_field
-from .core._docstrings import factory_docfiller_shared
-from .core.cached_decorators import gcached
-from .core.data import DataCallbackABC, DataValues
-from .core.models import Derivatives, ExtrapModel
 from .core.xrutils import xrwrap_xv
-
-docfiller_shared = factory_docfiller_shared(
-    names=("default", "beta", "volume"),
-)
-
+from .data import DataCallbackABC, DataValues
+from .docstrings import DOCFILLER_SHARED
+from .models import Derivatives, ExtrapModel
+
+docfiller_shared = DOCFILLER_SHARED.levels_to_top(
+    "cmomy", "xtrap", "beta", "volume"
+).decorate
 
 # Need funcs to pass to Coefs class
 # Just needs to be indexable based on order, so...
 # d^n X / d V^n = funcs[n](*args)
 # Could create list of simple functions for each derivative order
 # But here I'm trying something similar to what's in xtrapy already
 # For any general observable, might need to modify Data class to also pass full x values
@@ -111,15 +110,15 @@
     ndim: int = field(default=3, validator=attv.instance_of(int))
 
     _cache: dict = _cache_field()
 
     def check(self, data):
         pass
 
-    @gcached(prop=False)
+    @cached.meth
     def dxdq(self, rec_dim, skipna):
         return self.dxdqv.mean(rec_dim, skipna=skipna)
 
     def resample(self, data, meta_kws, indices, **kws):
         if not isinstance(data, DataValues):
             raise NotImplementedError("resampling only possible with DataValues style.")
         else:
```

### Comparing `thermoextrap-0.2.3/src/thermoextrap/volume_idealgas.py` & `thermoextrap-0.3.0/src/thermoextrap/volume_idealgas.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 Volume expansion for ideal gas (:mod:`~thermoextrap.volume_idealgas`)
 =====================================================================
 """
 
 
 from functools import lru_cache
 
-from .core._docstrings import factory_docfiller_shared
-from .core.models import Derivatives, ExtrapModel
+from .docstrings import DOCFILLER_SHARED
+from .models import Derivatives, ExtrapModel
 
-docfiller_shared = factory_docfiller_shared(names=("default", "beta", "volume"))
+docfiller_shared = DOCFILLER_SHARED.levels_to_top(
+    "cmomy", "xtrap", "beta", "volume"
+).decorate
 
 
 class VolumeDerivFuncsIG:
     """
     Calculates specific derivative values at refV with data x and W.
     Only go to first order for volume extrapolation.
     Here W represents the virial instead of the potential energy.
@@ -98,15 +100,15 @@
     -------
     extrapmodel : ExtrapModel
     """
 
     if order != 1:
         raise ValueError("only first order supported")
 
-    from .core.data import factory_data_values
+    from .data import factory_data_values
 
     data = factory_data_values(
         uv=uv, xv=xv, order=order, central=False, xalpha=False, **kws
     )
     derivatives = factory_derivatives(refV=volume)
     return ExtrapModel(
         alpha0=volume,
```

### Comparing `thermoextrap-0.2.3/src/thermoextrap.egg-info/SOURCES.txt` & `thermoextrap-0.3.0/src/thermoextrap.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,71 @@
 .cruft.json
+.editorconfig
 .gitignore
 .gitmodules
+.markdownlint.yaml
 .pre-commit-config.yaml
+.prettierrc.yaml
 AUTHORS.md
+CHANGELOG.md
 CONTRIBUTING.md
-HISTORY.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 environment.yaml
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
+changelog.d/README.txt
+changelog.d/templates/new_fragment.md.j2
+changelog.d/templates/auto-changelog/macros.jinja2
+changelog.d/templates/auto-changelog/template.jinja2
 environment/conda-spec.txt
 environment/dev-extras.yaml
 environment/dev.yaml
 environment/dist-conda.yaml
 environment/dist-pypi.yaml
 environment/docs-extras.yaml
 environment/docs.yaml
+environment/lint-extras.yaml
+environment/lint.yaml
 environment/test-extras.yaml
 environment/test.yaml
+environment/tools.yaml
+scripts/dist-conda.mk
+scripts/dist-pypi.mk
+scripts/docs-examples-symlinks.sh
+scripts/lint.mk
+scripts/run-prettier.sh
+scripts/tox-ipykernel-display-name.sh
 src/thermoextrap/__init__.py
 src/thermoextrap/adaptive_interp.py
 src/thermoextrap/beta.py
+src/thermoextrap/data.py
+src/thermoextrap/docstrings.py
+src/thermoextrap/idealgas.py
 src/thermoextrap/lnpi.py
+src/thermoextrap/models.py
 src/thermoextrap/recursive_interp.py
+src/thermoextrap/stack.py
 src/thermoextrap/volume.py
 src/thermoextrap/volume_idealgas.py
+src/thermoextrap.egg-info/PKG-INFO
+src/thermoextrap.egg-info/SOURCES.txt
+src/thermoextrap.egg-info/dependency_links.txt
+src/thermoextrap.egg-info/not-zip-safe
+src/thermoextrap.egg-info/requires.txt
+src/thermoextrap.egg-info/top_level.txt
 src/thermoextrap/core/__init__.py
 src/thermoextrap/core/_attrs_utils.py
 src/thermoextrap/core/_deprecate.py
-src/thermoextrap/core/_docstrings.py
-src/thermoextrap/core/cached_decorators.py
-src/thermoextrap/core/data.py
-src/thermoextrap/core/idealgas.py
-src/thermoextrap/core/models.py
 src/thermoextrap/core/sputils.py
-src/thermoextrap/core/stack.py
 src/thermoextrap/core/xrutils.py
-src/thermoextrap/core/external/__init__.py
-src/thermoextrap/core/external/docfiller.py
-src/thermoextrap/core/external/docscrape.py
 src/thermoextrap/gpr_active/__init__.py
 src/thermoextrap/gpr_active/active_utils.py
 src/thermoextrap/gpr_active/gp_models.py
 src/thermoextrap/gpr_active/ig_active.py
 src/thermoextrap/gpr_active/sine_active.py
 src/thermoextrap/legacy/__init__.py
 src/thermoextrap/legacy/extrap.py
```

### Comparing `thermoextrap-0.2.3/tests/conftest.py` & `thermoextrap-0.3.0/tests/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import numpy as np
 import pytest
 import xarray as xr
 
+from module_utilities import cached
+
 import thermoextrap as xtrap
 import thermoextrap.legacy
 
-# import thermoextrap.xpan_beta as betaxtrap
-from thermoextrap.core.cached_decorators import gcached
-
 
 class FixtureData:
     def __init__(self, n, nv, order=5, uoff=0.0, xoff=0.0, seed=0):
         print(
             "init data with:",
             dict(n=n, nv=nv, order=order, uoff=uoff, xoff=xoff, seed=seed),
         )
@@ -25,103 +24,103 @@
         self.u = self.rs.rand(n) + uoff
         self.x = self.rs.rand(n, nv) + xoff
 
         self.ub = self.rs.rand(n) + uoff
         self.xb = self.rs.rand(n, nv) + xoff
 
     # bunch of things to test
-    @gcached()
+    @cached.prop
     def rdata(self):
         return xtrap.factory_data_values(
             uv=self.u, xv=self.x, order=self.order, central=False
         )
 
-    @gcached()
+    @cached.prop
     def cdata(self):
         return xtrap.factory_data_values(
             uv=self.u, xv=self.x, order=self.order, central=True
         )
 
-    @gcached()
+    @cached.prop
     def xdata(self):
         return xtrap.DataCentralMoments.from_vals(
             xv=self.x,
             uv=self.u,
             order=self.order,
             central=True,
             dims=["val"],
         )
 
-    @gcached()
+    @cached.prop
     def xdata_val(self):
         return xtrap.DataCentralMomentsVals.from_vals(
             xv=self.x, uv=self.u, order=self.order, central=True
         )
 
-    @gcached()
+    @cached.prop
     def xrdata(self):
         return xtrap.DataCentralMoments.from_vals(
             xv=self.x,
             uv=self.u,
             order=self.order,
             central=False,
             dims=["val"],
         )
 
-    @gcached()
+    @cached.prop
     def xrdata_val(self):
         return xtrap.DataCentralMomentsVals.from_vals(
             xv=self.x,
             uv=self.u,
             order=self.order,
             central=False,
         )
 
     # bunch of things to test
-    @gcached()
+    @cached.prop
     def rdata(self):
         return xtrap.factory_data_values(
             uv=self.u, xv=self.x, order=self.order, central=False
         )
 
-    @gcached()
+    @cached.prop
     def cdata(self):
         return xtrap.factory_data_values(
             uv=self.u, xv=self.x, order=self.order, central=True
         )
 
-    @gcached()
+    @cached.prop
     def xdata(self):
         return xtrap.DataCentralMoments.from_vals(
             xv=self.x,
             uv=self.u,
             order=self.order,
             central=True,
             dims=["val"],
             axis=0,
         )
 
-    @gcached()
+    @cached.prop
     def xdata_val(self):
         return xtrap.DataCentralMomentsVals.from_vals(
             xv=self.x, uv=self.u, order=self.order, central=True
         )
 
-    @gcached()
+    @cached.prop
     def xrdata(self):
         return xtrap.DataCentralMoments.from_vals(
             xv=self.x,
             uv=self.u,
             order=self.order,
             central=False,
             dims=["val"],
             axis=0,
         )
 
-    @gcached()
+    @cached.prop
     def xrdata_val(self):
         return xtrap.DataCentralMomentsVals.from_vals(
             xv=self.x,
             uv=self.u,
             order=self.order,
             central=False,
         )
@@ -130,15 +129,15 @@
     def beta0(self):
         return 0.5
 
     @property
     def betas(self):
         return [0.3, 0.4]
 
-    @gcached()
+    @cached.prop
     def em(self):
         """extrapolation model fixture"""
 
         em = thermoextrap.legacy.ExtrapModel(maxOrder=self.order)
         em.train(self.beta0, xData=self.x, uData=self.u, saveParams=True)
 
         return em
@@ -147,20 +146,20 @@
     # def fix_ufunc_xufunc(ufunc, xufunc):
 
     #     ufunc_out = lambda x: float(ufunc(x))
     #     xufunc_out = lambda x: xufunc.avgdict[x]
 
     #     return ufunc_out, xufunc_out
 
-    @gcached()
+    @cached.prop
     def u_xu_funcs(self):
         ufunc, xufunc = thermoextrap.legacy.buildAvgFuncs(self.x, self.u, self.order)
         return ufunc, xufunc
 
-    @gcached()
+    @cached.prop
     def derivs_list(self):
         fs = [thermoextrap.legacy.symDerivAvgX(i) for i in range(self.order + 1)]
         ufunc, xufunc = self.u_xu_funcs
 
         return [fs[i](ufunc, xufunc) for i in range(self.order + 1)]
 
     def xr_test_raw(self, b, a=None):
@@ -236,29 +235,29 @@
 
 # class Fixture_Old:
 #     def __init__(self, x, u, order):
 #         self.x = x
 #         self.u = u
 #         self.order = order
 
-#     @gcached()
+#     @cached.prop
 #     def u_xu_funcs(self):
 #         ufunc, xufunc = thermoextrap.legacy.buildAvgFuncs(self.x, self.u, self.order)
 #         return ufunc, xufunc
 
-#     @gcached(prop=False)
+#     @cached.meth
 #     def em(self, alpha0=0.5):
 #         return thermoextrap.legacy.ExtrapModel(self.order, alpha0, self.x, self.u)
 
 
 # class Fixture_New:
 #     def __init__(self, data):
 #         self.data = data
 
-#     @gcached(prop=False)
+#     @cached.meth
 #     def xem(self, alpha0=0.5, minus_log=False):
 #         return xtrap.beta.factory_extrapmodel(alpha0=alpha0, data=self.data,
 #                                              minus_log=minus_log)
 
 #     def xr_test_raw(self, other):
 
 #         self.xr_test(self.data.u, other.u.sel(val=0))
```

### Comparing `thermoextrap-0.2.3/tests/test_GPs.py` & `thermoextrap-0.3.0/tests/test_GPs.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.3/tests/test_active.py` & `thermoextrap-0.3.0/tests/test_active.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.3/tests/test_beta.py` & `thermoextrap-0.3.0/tests/test_beta.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.3/tests/test_data.py` & `thermoextrap-0.3.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.3/tests/test_idealgas.py` & `thermoextrap-0.3.0/tests/test_idealgas.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.3/tests/test_lnPi.py` & `thermoextrap-0.3.0/tests/test_lnPi.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.3/tests/test_stack.py` & `thermoextrap-0.3.0/tests/test_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import pandas as pd
 import pytest
 import xarray as xr
 
 import thermoextrap as xtrap
-from thermoextrap.core import stack
+from thermoextrap import stack
 
 
 @pytest.fixture
 def states():
     shape = (3, 2, 4)
     dims = ["rec", "pair", "position"]
```

### Comparing `thermoextrap-0.2.3/tests/test_u_data.py` & `thermoextrap-0.3.0/tests/test_u_data.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.3/tests/test_u_equations.py` & `thermoextrap-0.3.0/tests/test_u_equations.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 @pytest.fixture(params=n_list)
 def data(request):
     data = namedtuple("data", ["n", "u", "x1", "du", "dxdu", "xu", "ui" "subs"])
 
     n = request.param
     data.n = n
-    data.u, data.x1 = xtrap.core.models.get_default_symbol("u", "x1")
+    data.u, data.x1 = xtrap.models.get_default_symbol("u", "x1")
     data.du, data.dxdu = get_default_indexed("du", "dxdu")
     data.xu, data.ui = get_default_indexed("xu", "u")
 
     subs_central = {data.dxdu[i]: data.du[i + 1] for i in range(1, 2 * n)}
     subs_central[data.x1] = data.u
 
     subs_raw = {data.xu[i]: data.ui[i + 1] for i in range(0, 2 * n)}
```

### Comparing `thermoextrap-0.2.3/tests/test_volume.py` & `thermoextrap-0.3.0/tests/test_volume.py`

 * *Files identical despite different names*

### Comparing `thermoextrap-0.2.3/tox.ini` & `thermoextrap-0.3.0/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,151 +1,142 @@
 [tox]
 isolated_build = True
 requires = tox-conda
 envlist =
         # test
-        py3{8, 9, 10}-tests
-
+        test-py3{8, 9, 10}
 
 [base]
 package_name = thermoextrap
 import_name  = thermoextrap
 build_python = python3.10
 conda_env            = {toxinidir}/environment.yaml
 conda_env_dev        = {toxinidir}/environment/dev.yaml
 conda_env_test       = {toxinidir}/environment/test.yaml
 conda_env_docs       = {toxinidir}/environment/docs.yaml
 conda_env_dist_pypi  = {toxinidir}/environment/dist-pypi.yaml
 conda_env_dist_conda = {toxinidir}/environment/dist-conda.yaml
 conda_spec = {toxinidir}/environment/conda-spec.txt
+conda_env_lint       = {toxinidir}/environment/lint.yaml
 conda_channels =
     wpk-nist
     conda-forge
 conda_deps_test =
 allowlist_externals =
     bash
-    open
-    cat
-    rm
-    echo
-    mkdir
     make
 commands_test_check =
     python --version
     python -c 'import {[base]import_name}; print( {[base]import_name}.__version__)'
     bash -ec 'echo $PWD'
-    echo {posargs:{toxinidir}}
-
 
 [testenv]
+passenv =
+        SETUPTOOLS_SCM_PRETEND_VERSION
+        command
+        mypy_args
+        pyright_args
+        pytype_args
+        release_args
+        project_name
+        TEST_VERSION
 usedevelop =
-    tests: True
+    test: True
 conda_env =
-    tests: {[base]conda_env_test}
+    test: {[base]conda_env_test}
 allowlist_externals =
     {[base]allowlist_externals}
 commands =
     {[base]commands_test_check}
-    pytest {posargs}
+    {posargs:pytest}
 
+[testenv:dev]
+description =
+    Create development environment.
+usedevelop = True
+basepython = {[base]build_python}
+conda_env = {[base]conda_env_dev}
+envdir = {toxworkdir}/dev
+commands =
+    {posargs:bash -ec 'conda list'}
 
-# Build documentation
-[testenv:docs-{build, release, clean, command, spelling, live, open, make}]
+[testenv:docs]
 description =
-    build: build documentation.
-    release: create documentation branch.
-    clean: clean build.
-    spelling: run spell checking on documentation and docstrings.
-    command: run arbitrary command
-    live: use sphinx-autobuild
-    make: run arbitrary make command from docs/Makefile.  Passes in posargs
+    Runs make in docs directory.
+    For example, 'tox -e docs -- html' -> 'make -C docs html'.
+    With 'release' option, you can set the message with 'message=...' in posargs.
 usedevelop = True
 envdir     = {toxworkdir}/docs
 basepython = {[base]build_python}
 conda_env  = {[base]conda_env_docs}
 conda_spec = {[base]conda_spec}
 changedir  = {toxinidir}/docs
 commands =
-    build: bash -c "echo $PWD"
-    build: make {posargs:html}
-    open: open {toxinidir}/docs/_build/html/index.html
-    release: ghp-import -n {posargs:-m 'update docs'} -b nist-pages {toxinidir}/docs/_build/html
-    clean: make allclean
-    spelling: make spelling
-    command: {posargs}
-    live: make livehtml
-    make: make {posargs}
+    make {posargs:html}
 
-# create pypi dist
-[testenv:dist-pypi-{build, testrelease, release}]
+[testenv:dist-pypi]
 description  =
-    build: build distribution.
-    testrelease: upload to testpypi
-    release: upload to pypi
+    Runs make -f scrips/dist-pypi.mk posargs
+    For example, 'tox -e dist-pypi -- build' -> 'make -f scripts/dist-pypi.mk build'
 skip_install = True
 envdir       = {toxworkdir}/dist-pypi
 basepython   = {[base]build_python}
 conda_env    = {[base]conda_env_dist_pypi}
 changedir    = {toxinidir}
 commands     =
-    build: rm -rf {toxinidir}/dist
-    build: python -m build --outdir "{toxinidir}/dist/"
-
-    testrelease: twine upload --repository testpypi {toxinidir}/dist/*
-    release: twine upload {toxinidir}/dist/*
-
+    make -f {toxinidir}/scripts/dist-pypi.mk {posargs:build}
 
-# create conda dist
-[testenv:dist-conda-{recipe, build, command}]
+[testenv:dist-conda]
 description  =
+    Runs make -C dist-conda posargs
     recipe: build conda recipe using grayskull (can optionally pass a local sdist)
     build: build conda distribution
     command: run arbitrary command
 skip_install = True
 envdir       = {toxworkdir}/dist-conda
 basepython   = {[base]build_python}
 conda_env    = {[base]conda_env_dist_conda}
 changedir    = {toxinidir}/dist-conda
 commands     =
-    recipe: rm -rf {toxinidir}/dist-conda/{[base]package_name}
-    recipe: grayskull pypi {posargs:{[base]package_name}}
-    recipe: cat {[base]package_name}/meta.yaml
-
-    build: rm -rf build
-    build: mkdir -p build
-    build: conda mambabuild --output-folder=build --no-anaconda-upload .
-    command: {posargs:python}
+    make -f {toxinidir}/scripts/dist-conda.mk {posargs} project_name={[base]package_name}
 
-
-# test pypi/conda install from local/remote
-[testenv:test-dist-{pypi, conda}-{local,remote}-py3{8,9,10}]
+[testenv:testdist-{pypi, conda}-{local,remote}-py3{8, 9, 10, 11}]
 conda_channels =
     {[base]conda_channels}
-description  =
+description =
     Test install from
     pypi: pypi
     conda: conda
     using either
     local: local
     remote: remote
     versions.
 skip_install = True
 conda_env    = {toxinidir}/environment/test-extras.yaml
 conda_deps =
-    conda-remote: {[base]package_name}
+    conda-remote: {[base]package_name}{env:TEST_VERSION:''}
     conda-local: {posargs}
     conda: pymbar<4.0
 deps =
-    pypi-remote: {[base]package_name}[mbar,gpr]
+    pypi-remote: {[base]package_name}[mbar,gpr]{env:TEST_VERSION:''}
     pypi-local: {posargs}[mbar,gpr]
     conda: tensorflow
     conda: tensorflow-probability
     conda: gpflow
 
-
-# Test pip installed dependencies
-[testenv:test-pip-py3{8,9,10}]
+[testenv:testpip-py3{8, 9, 10, 11}]
 description  =
     Test package against pip installed packages
 usedevelop   = True
 extras = test
 conda_env    = {toxinidir}/environment/test-extras.yaml
+
+[testenv:lint]
+description =
+    Run linters
+    For example, 'tox -e lint -- mypy mypy_args=...' runs 'mypy $mypy_args'
+conda_env = {[base]conda_env_lint}
+usedevelop = True
+envdir     = {toxworkdir}/lint
+basepython = {[base]build_python}
+commands =
+    make -f {toxinidir}/scripts/lint.mk {posargs:mypy}
```

