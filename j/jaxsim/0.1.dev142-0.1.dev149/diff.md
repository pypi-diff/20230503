# Comparing `tmp/jaxsim-0.1.dev142.tar.gz` & `tmp/jaxsim-0.1.dev149.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxsim-0.1.dev142.tar", last modified: Fri Apr 21 10:02:58 2023, max compression
+gzip compressed data, was "jaxsim-0.1.dev149.tar", last modified: Wed May  3 16:14:47 2023, max compression
```

## Comparing `jaxsim-0.1.dev142.tar` & `jaxsim-0.1.dev149.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.693920 jaxsim-0.1.dev142/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.685919 jaxsim-0.1.dev142/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.689920 jaxsim-0.1.dev142/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/.github/workflows/ci_cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-21 10:02:58.697920 jaxsim-0.1.dev142/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-21 10:02:58.697920 jaxsim-0.1.dev142/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.685919 jaxsim-0.1.dev142/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.689920 jaxsim-0.1.dev142/src/jaxsim/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.689920 jaxsim-0.1.dev142/src/jaxsim/high_level/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/high_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/high_level/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/high_level/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/high_level/link.py
--rw-r--r--   0 runner    (1001) docker     (123)    34435 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/high_level/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.689920 jaxsim-0.1.dev142/src/jaxsim/math/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/math/adjoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/math/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/math/cross.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/math/inertia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/math/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/math/plucker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/math/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/math/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/math/skew.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.689920 jaxsim-0.1.dev142/src/jaxsim/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.693920 jaxsim-0.1.dev142/src/jaxsim/parsers/descriptions/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/parsers/descriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/parsers/descriptions/collision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/parsers/descriptions/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/parsers/descriptions/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/parsers/descriptions/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18763 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/parsers/kinematic_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.693920 jaxsim-0.1.dev142/src/jaxsim/parsers/sdf/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/parsers/sdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/parsers/sdf/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/parsers/sdf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.693920 jaxsim-0.1.dev142/src/jaxsim/physics/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.693920 jaxsim-0.1.dev142/src/jaxsim/physics/algos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/algos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/algos/aba.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/algos/crba.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/algos/forward_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/algos/jacobian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/algos/rnea.py
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/algos/soft_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/algos/terrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/algos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.693920 jaxsim-0.1.dev142/src/jaxsim/physics/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/model/ground_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/model/physics_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/model/physics_model_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.693920 jaxsim-0.1.dev142/src/jaxsim/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/simulation/integrators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/simulation/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/simulation/ode_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/simulation/ode_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15110 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/simulation/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/simulation/simulator_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/simulation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.693920 jaxsim-0.1.dev142/src/jaxsim/sixd/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/sixd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.689920 jaxsim-0.1.dev142/src/jaxsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-21 10:02:58.000000 jaxsim-0.1.dev142/src/jaxsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-21 10:02:58.000000 jaxsim-0.1.dev142/src/jaxsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:02:58.000000 jaxsim-0.1.dev142/src/jaxsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:02:58.000000 jaxsim-0.1.dev142/src/jaxsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-21 10:02:58.000000 jaxsim-0.1.dev142/src/jaxsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 10:02:58.000000 jaxsim-0.1.dev142/src/jaxsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:47.010729 jaxsim-0.1.dev149/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:46.990727 jaxsim-0.1.dev149/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:46.994727 jaxsim-0.1.dev149/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/.github/workflows/ci_cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-03 16:14:47.010729 jaxsim-0.1.dev149/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-03 16:14:47.010729 jaxsim-0.1.dev149/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:46.990727 jaxsim-0.1.dev149/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:46.998728 jaxsim-0.1.dev149/src/jaxsim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:46.998728 jaxsim-0.1.dev149/src/jaxsim/high_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/high_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/high_level/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/high_level/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/high_level/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37704 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/high_level/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:47.002728 jaxsim-0.1.dev149/src/jaxsim/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/math/adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/math/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/math/cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/math/inertia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/math/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/math/plucker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/math/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/math/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/math/skew.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:47.002728 jaxsim-0.1.dev149/src/jaxsim/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:47.002728 jaxsim-0.1.dev149/src/jaxsim/parsers/descriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/parsers/descriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/parsers/descriptions/collision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/parsers/descriptions/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/parsers/descriptions/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/parsers/descriptions/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18763 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/parsers/kinematic_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:47.002728 jaxsim-0.1.dev149/src/jaxsim/parsers/rod/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/parsers/rod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/parsers/rod/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/parsers/rod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:47.002728 jaxsim-0.1.dev149/src/jaxsim/physics/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:47.006729 jaxsim-0.1.dev149/src/jaxsim/physics/algos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/algos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/algos/aba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/algos/crba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/algos/forward_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/algos/jacobian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/algos/rnea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/algos/soft_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/algos/terrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/algos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:47.006729 jaxsim-0.1.dev149/src/jaxsim/physics/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/model/ground_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/model/physics_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/model/physics_model_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:47.010729 jaxsim-0.1.dev149/src/jaxsim/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/simulation/integrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/simulation/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/simulation/ode_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/simulation/ode_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15110 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/simulation/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/simulation/simulator_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/simulation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:47.010729 jaxsim-0.1.dev149/src/jaxsim/sixd/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/sixd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:46.998728 jaxsim-0.1.dev149/src/jaxsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-03 16:14:46.000000 jaxsim-0.1.dev149/src/jaxsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-03 16:14:46.000000 jaxsim-0.1.dev149/src/jaxsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 16:14:46.000000 jaxsim-0.1.dev149/src/jaxsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 16:14:46.000000 jaxsim-0.1.dev149/src/jaxsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-03 16:14:46.000000 jaxsim-0.1.dev149/src/jaxsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 16:14:46.000000 jaxsim-0.1.dev149/src/jaxsim.egg-info/top_level.txt
```

### Comparing `jaxsim-0.1.dev142/.github/workflows/ci_cd.yml` & `jaxsim-0.1.dev149/.github/workflows/ci_cd.yml`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/.github/workflows/style.yml` & `jaxsim-0.1.dev149/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/.gitignore` & `jaxsim-0.1.dev149/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/LICENSE` & `jaxsim-0.1.dev149/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/PKG-INFO` & `jaxsim-0.1.dev149/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxsim
-Version: 0.1.dev142
+Version: 0.1.dev149
 Summary: A physics engine in reduced coordinates implemented with JAX.
 Home-page: https://github.com/ami-iit/jaxsim
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/jaxsim/releases
 Project-URL: Source, https://github.com/ami-iit/jaxsim
```

### Comparing `jaxsim-0.1.dev142/README.md` & `jaxsim-0.1.dev149/README.md`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/setup.cfg` & `jaxsim-0.1.dev149/setup.cfg`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/__init__.py` & `jaxsim-0.1.dev149/src/jaxsim/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/high_level/joint.py` & `jaxsim-0.1.dev149/src/jaxsim/high_level/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/high_level/link.py` & `jaxsim-0.1.dev149/src/jaxsim/high_level/link.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/high_level/model.py` & `jaxsim-0.1.dev149/src/jaxsim/high_level/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import dataclasses
 import pathlib
-from typing import Any, Dict, List, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import jax.experimental.ode
 import jax.numpy as jnp
 import jax_dataclasses
 import numpy as np
 
 import jaxsim
 import jaxsim.physics.algos.aba
 import jaxsim.physics.algos.crba
 import jaxsim.physics.algos.forward_kinematics
 import jaxsim.physics.algos.rnea
 import jaxsim.physics.model.physics_model
 import jaxsim.physics.model.physics_model_state
 import jaxsim.typing as jtp
-from jaxsim import high_level, physics, sixd
+from jaxsim import high_level, logging, physics, sixd
 from jaxsim.physics.algos import soft_contacts
 from jaxsim.physics.algos.terrain import FlatTerrain, Terrain
 from jaxsim.simulation import ode_data, ode_integration
 from jaxsim.simulation.ode_integration import IntegratorType
 from jaxsim.utils import JaxsimDataclass, Mutability
 
 from .common import VelRepr
@@ -118,86 +118,156 @@
     data: ModelData = jax_dataclasses.field(default=None, repr=False)
 
     # ========================
     # Initialization and state
     # ========================
 
     @staticmethod
-    def build_from_sdf(
-        sdf: Union[str, pathlib.Path],
-        model_name: str = None,
+    def build_from_model_description(
+        model_description: Union[str, pathlib.Path],
+        model_name: Optional[str] = None,
         vel_repr: VelRepr = VelRepr.Mixed,
         gravity: jtp.Array = jaxsim.physics.default_gravity(),
-        is_urdf: bool = False,
-        considered_joints: List[str] = None,
+        is_urdf: Optional[bool] = None,
+        considered_joints: Optional[List[str]] = None,
     ) -> "Model":
-        import jaxsim.parsers.sdf
+        """
+        Build a Model object from a model description.
+
+        Args:
+            model_description: Either a path to a file or a string containing the URDF/SDF description.
+            model_name: The optional name of the model that overrides the one in the description.
+            vel_repr: The velocity representation to use.
+            gravity: The 3D gravity vector.
+            is_urdf: Whether the model description is a URDF or an SDF. This is
+                automatically inferred if the model description is a path to a file.
+            considered_joints: The list of joints to consider. If None, all joints are considered.
 
-        if is_urdf:
-            raise ValueError("Converting URDF to SDF is not yet supported")
+        Returns:
+            The built Model object.
+        """
 
-        model_description = jaxsim.parsers.sdf.build_model_from_sdf(sdf=sdf)
+        import jaxsim.parsers.rod
 
+        # Parse the input resource (either a path to file or a string with the URDF/SDF)
+        # and build the -intermediate- model description
+        model_description = jaxsim.parsers.rod.build_model_description(
+            model_description=model_description, is_urdf=is_urdf
+        )
+
+        # Lump links together if not all joints are considered.
+        # Note: this procedure assigns a zero position to all joints not considered.
         if considered_joints is not None:
             model_description = model_description.reduce(
                 considered_joints=considered_joints
             )
 
+        # Create the physics model from the model description
         physics_model = jaxsim.physics.model.physics_model.PhysicsModel.build_from(
             model_description=model_description, gravity=gravity
         )
 
+        # Build and return the high-level model
         return Model.build(
             physics_model=physics_model,
             model_name=model_name,
             vel_repr=vel_repr,
         )
 
     @staticmethod
+    def build_from_sdf(
+        sdf: Union[str, pathlib.Path],
+        model_name: Optional[str] = None,
+        vel_repr: VelRepr = VelRepr.Mixed,
+        gravity: jtp.Array = jaxsim.physics.default_gravity(),
+        is_urdf: Optional[bool] = None,
+        considered_joints: Optional[List[str]] = None,
+    ) -> "Model":
+        """
+        Build a Model object from an SDF description.
+        This is a deprecated method, use build_from_model_description instead.
+        """
+
+        msg = "Model.{} is deprecated, use Model.{} instead."
+        logging.warning(
+            msg=msg.format("build_from_sdf", "build_from_model_description")
+        )
+
+        return Model.build_from_model_description(
+            model_description=sdf,
+            model_name=model_name,
+            vel_repr=vel_repr,
+            gravity=gravity,
+            is_urdf=is_urdf,
+            considered_joints=considered_joints,
+        )
+
+    @staticmethod
     def build(
         physics_model: jaxsim.physics.model.physics_model.PhysicsModel,
-        model_name: str = None,
+        model_name: Optional[str] = None,
         vel_repr: VelRepr = VelRepr.Mixed,
     ) -> "Model":
+        """
+        Build a Model object from a physics model.
+
+        Args:
+            physics_model: The physics model.
+            model_name: The optional name of the model that overrides the one in the physics model.
+            vel_repr: The velocity representation to use.
+
+        Returns:
+            The built Model object.
+        """
+
+        # Set the model name (if not provided, use the one from the model description)
         model_name = (
             model_name if model_name is not None else physics_model.description.name
         )
 
+        # Sort all the joints by their index
         sorted_links = {
             l.name: high_level.link.Link(link_description=l)
             for l in sorted(
                 physics_model.description.links_dict.values(), key=lambda l: l.index
             )
         }
 
+        # Sort all the joints by their index
         sorted_joints = {
             j.name: high_level.joint.Joint(joint_description=j)
             for j in sorted(
                 physics_model.description.joints_dict.values(),
                 key=lambda j: j.index,
             )
         }
 
+        # Build the high-level model
         model = Model(
             physics_model=physics_model,
             model_name=model_name,
             velocity_representation=vel_repr,
             _links=sorted_links,
             _joints=sorted_joints,
         )
 
+        # Zero the model data
         with model.editable(validate=False) as model:
             model.zero()
 
+        # Check model validity
         if not model.valid():
             raise RuntimeError
 
+        # Return the high-level model
         return model
 
     def __post_init__(self):
+        """Post-init logic. Use the static methods to build high-level models."""
+
         original_mutability = self._mutability()
         self._set_mutability(Mutability.MUTABLE_NO_VALIDATION)
 
         for l in self._links.values():
             l.mutable(validate=False).parent_model = self
 
         for j in self._joints.values():
@@ -210,29 +280,40 @@
         self._joints: Dict[str, high_level.joint.Joint] = {
             k: v for k, v in sorted(self._joints.items(), key=lambda kv: kv[1].index())
         }
 
         self._set_mutability(original_mutability)
 
     def reduce(self, considered_joints: List[str]) -> None:
+        """
+        Reduce the model by lumping together the links connected by removed joints.
+
+        Args:
+            considered_joints: The list of joints to consider.
+        """
+
+        # Reduce the model description
         reduced_model_description = self.physics_model.description.reduce(
             considered_joints=considered_joints
         )
 
+        # Create the physics model from the reduced model description
         physics_model = jaxsim.physics.model.physics_model.PhysicsModel.build_from(
             model_description=reduced_model_description,
             gravity=self.physics_model.gravity[0:3],
         )
 
+        # Build the reduced high-level model
         reduced_model = Model.build(
             physics_model=physics_model,
             model_name=self.name(),
             vel_repr=self.velocity_representation,
         )
 
+        # Replace the current model with the reduced one
         original_mutability = self._mutability()
         self._set_mutability(mutability=self._mutability().MUTABLE_NO_VALIDATION)
         self.physics_model = reduced_model.physics_model
         self.data = reduced_model.data
         self._links = reduced_model._links
         self._joints = reduced_model._joints
         self._set_mutability(original_mutability)
```

### Comparing `jaxsim-0.1.dev142/src/jaxsim/logging.py` & `jaxsim-0.1.dev149/src/jaxsim/logging.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/math/adjoint.py` & `jaxsim-0.1.dev149/src/jaxsim/math/adjoint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/math/conv.py` & `jaxsim-0.1.dev149/src/jaxsim/math/conv.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/math/cross.py` & `jaxsim-0.1.dev149/src/jaxsim/math/cross.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/math/inertia.py` & `jaxsim-0.1.dev149/src/jaxsim/math/inertia.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/math/joint.py` & `jaxsim-0.1.dev149/src/jaxsim/math/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/math/plucker.py` & `jaxsim-0.1.dev149/src/jaxsim/math/plucker.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/math/quaternion.py` & `jaxsim-0.1.dev149/src/jaxsim/math/quaternion.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/math/rotation.py` & `jaxsim-0.1.dev149/src/jaxsim/math/rotation.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/math/skew.py` & `jaxsim-0.1.dev149/src/jaxsim/math/skew.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/parsers/descriptions/collision.py` & `jaxsim-0.1.dev149/src/jaxsim/parsers/descriptions/collision.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/parsers/descriptions/joint.py` & `jaxsim-0.1.dev149/src/jaxsim/parsers/descriptions/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/parsers/descriptions/link.py` & `jaxsim-0.1.dev149/src/jaxsim/parsers/descriptions/link.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/parsers/descriptions/model.py` & `jaxsim-0.1.dev149/src/jaxsim/parsers/descriptions/model.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/parsers/kinematic_graph.py` & `jaxsim-0.1.dev149/src/jaxsim/parsers/kinematic_graph.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/parsers/sdf/parser.py` & `jaxsim-0.1.dev149/src/jaxsim/parsers/rod/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,55 +1,77 @@
 import dataclasses
 import pathlib
-from pathlib import Path
 from typing import Dict, List, NamedTuple, Optional, Union
 
 import jax.numpy as jnp
 import numpy as np
 import rod
 
 from jaxsim import logging
 from jaxsim.math.quaternion import Quaternion
 from jaxsim.parsers import descriptions, kinematic_graph
 
 from . import utils as utils
 
 
 class SDFData(NamedTuple):
+    """
+    Data extracted from an SDF resource useful to build a JaxSim model.
+    """
+
     model_name: str
 
     fixed_base: bool
     base_link_name: str
 
     link_descriptions: List[descriptions.LinkDescription]
     joint_descriptions: List[descriptions.JointDescription]
     collision_shapes: List[descriptions.CollisionShape]
 
     sdf_model: Optional[rod.Model] = None
     model_pose: kinematic_graph.RootPose = kinematic_graph.RootPose()
 
 
-def extract_data_from_sdf(
-    sdf: Union[pathlib.Path, str], model_name: Optional[str] = None
+def extract_model_data(
+    model_description: Union[pathlib.Path, str],
+    model_name: Optional[str] = None,
+    is_urdf: Optional[bool] = None,
 ) -> SDFData:
+    """
+    Extract data from an SDF/URDF resource useful to build a JaxSim model.
+
+    Args:
+        model_description: Either a path to an SDF/URDF file or a string containing its content.
+        model_name: The name of the model to extract from the SDF resource.
+        is_urdf: Whether the SDF resource is a URDF file. Needed only if model_description
+            is a URDF string.
+
+    Returns:
+        The extracted model data.
+    """
+
     # Parse the SDF resource
-    sdf_element = rod.Sdf.load(sdf=sdf)
+    sdf_element = rod.Sdf.load(sdf=model_description, is_urdf=is_urdf)
 
     if len(sdf_element.models()) == 0:
         raise RuntimeError("Failed to find any model in SDF resource")
 
     # Assume the SDF resource has only one model, or the desired model name is given
     sdf_models = {m.name: m for m in sdf_element.models()}
     sdf_model = (
         sdf_element.models()[0] if len(sdf_models) == 1 else sdf_models[model_name]
     )
 
     # Log model name
     logging.debug(msg=f"Found model '{sdf_model.name}' in SDF resource")
 
+    # Jaxsim supports only models compatible with URDF, i.e. those having all links
+    # directly attached to their parent joint without additional roto-translations.
+    sdf_model.switch_frame_convention(frame_convention=rod.FrameConvention.Urdf)
+
     # Log type of base link
     logging.debug(
         msg="Model '{}' is {}".format(
             sdf_model.name,
             "fixed-base" if sdf_model.is_fixed_base() else "floating-base",
         )
     )
@@ -271,17 +293,32 @@
         fixed_base=sdf_model.is_fixed_base(),
         base_link_name=sdf_model.get_canonical_link(),
         model_pose=model_pose,
         sdf_model=sdf_model,
     )
 
 
-def build_model_from_sdf(sdf: Union[Path, str]) -> descriptions.ModelDescription:
-    # Parse data from the SDF
-    sdf_data = extract_data_from_sdf(sdf=sdf)
+def build_model_description(
+    model_description: Union[pathlib.Path, str], is_urdf: Optional[bool] = False
+) -> descriptions.ModelDescription:
+    """
+    Builds a model description from an SDF/URDF resource.
+
+    Args:
+        model_description: Either a path to an SDF/URDF file or a string containing its content.
+        is_urdf: Whether the SDF resource is a URDF file. Needed only if model_description
+            is a URDF string.
+    Returns:
+        The parsed model description.
+    """
+
+    # Parse data from the SDF assuming it contains a single model
+    sdf_data = extract_model_data(
+        model_description=model_description, model_name=None, is_urdf=is_urdf
+    )
 
     # Build the model description.
     # Note: if the model is fixed-base, the fixed joint between world and the first
     #       link is removed and the pose of the first link is updated.
     model = descriptions.ModelDescription.build_model_from(
         name=sdf_data.model_name,
         links=sdf_data.link_descriptions,
```

### Comparing `jaxsim-0.1.dev142/src/jaxsim/parsers/sdf/utils.py` & `jaxsim-0.1.dev149/src/jaxsim/parsers/rod/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,14 +6,24 @@
 import numpy.typing as npt
 import rod
 
 from jaxsim.parsers import descriptions
 
 
 def from_sdf_inertial(inertial: rod.Inertial) -> npt.NDArray:
+    """
+    Extract the 6D inertia matrix from an SDF inertial element.
+
+    Args:
+        inertial: The SDF inertial element.
+
+    Returns:
+        The 6D inertia matrix of the link expressed in the link frame.
+    """
+
     from jaxsim.math.inertia import Inertia
     from jaxsim.sixd import se3
 
     # Extract the "mass" element
     m = inertial.mass
 
     # Extract the "inertia" element
@@ -32,32 +42,43 @@
             [ixx, ixy, ixz],
             [ixy, iyy, iyz],
             [ixz, iyz, izz],
         ]
     )
 
     # Build the 6x6 generalized inertia at the CoM
-    I_generalized = Inertia.to_sixd(mass=m, com=np.zeros(3), I=I_CoM)
+    M_CoM = Inertia.to_sixd(mass=m, com=np.zeros(3), I=I_CoM)
 
     # Compute the transform from the inertial frame (CoM) to the link frame
     L_H_CoM = inertial.pose.transform() if inertial.pose is not None else np.eye(4)
 
     # We need its inverse
     CoM_H_L = se3.SE3.from_matrix(matrix=L_H_CoM).inverse()
     CoM_X_L: npt.NDArray = CoM_H_L.adjoint()
 
-    # Express the CoM inertia matrix in the link frame
-    I_expressed_in_link_frame = CoM_X_L.T @ I_generalized @ CoM_X_L
+    # Express the CoM inertia matrix in the link frame L
+    M_L = CoM_X_L.T @ M_CoM @ CoM_X_L
 
-    return jnp.array(I_expressed_in_link_frame)
+    return jnp.array(M_L)
 
 
 def axis_to_jtype(
     axis: rod.Axis, type: str
 ) -> Union[descriptions.JointType, descriptions.JointDescriptor]:
+    """
+    Convert an SDF axis to a joint type.
+
+    Args:
+        axis: The SDF axis.
+        type: The SDF joint type.
+
+    Returns:
+        The corresponding joint type description.
+    """
+
     if type == "fixed":
         return descriptions.JointType.F
 
     if not (axis.xyz is not None and axis.xyz.xyz is not None):
         raise ValueError("Failed to read axis xyz data")
 
     axis_xyz = np.array(axis.xyz.xyz)
@@ -92,14 +113,25 @@
 
     raise ValueError("Joint not supported", axis_xyz, type)
 
 
 def create_box_collision(
     collision: rod.Collision, link_description: descriptions.LinkDescription
 ) -> descriptions.BoxCollision:
+    """
+    Create a box collision from an SDF collision element.
+
+    Args:
+        collision: The SDF collision element.
+        link_description: The link description.
+
+    Returns:
+        The box collision description.
+    """
+
     x, y, z = collision.geometry.box.size
 
     center = np.array([x / 2, y / 2, z / 2])
 
     box_corners = (
         np.vstack(
             [
@@ -136,14 +168,25 @@
         collidable_points=collidable_points, center=center_wrt_link
     )
 
 
 def create_sphere_collision(
     collision: rod.Collision, link_description: descriptions.LinkDescription
 ) -> descriptions.SphereCollision:
+    """
+    Create a sphere collision from an SDF collision element.
+
+    Args:
+        collision: The SDF collision element.
+        link_description: The link description.
+
+    Returns:
+        The sphere collision description.
+    """
+
     # From https://stackoverflow.com/a/26127012
     def fibonacci_sphere(samples: int) -> npt.NDArray:
         points = []
         phi = np.pi * (3.0 - np.sqrt(5.0))  # golden angle in radians
 
         for i in range(samples):
             y = 1 - (i / float(samples - 1)) * 2  # y goes from 1 to -1
```

### Comparing `jaxsim-0.1.dev142/src/jaxsim/physics/algos/aba.py` & `jaxsim-0.1.dev149/src/jaxsim/physics/algos/aba.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/physics/algos/crba.py` & `jaxsim-0.1.dev149/src/jaxsim/physics/algos/crba.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/physics/algos/forward_kinematics.py` & `jaxsim-0.1.dev149/src/jaxsim/physics/algos/forward_kinematics.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/physics/algos/jacobian.py` & `jaxsim-0.1.dev149/src/jaxsim/physics/algos/jacobian.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/physics/algos/rnea.py` & `jaxsim-0.1.dev149/src/jaxsim/physics/algos/rnea.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/physics/algos/soft_contacts.py` & `jaxsim-0.1.dev149/src/jaxsim/physics/algos/soft_contacts.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/physics/algos/terrain.py` & `jaxsim-0.1.dev149/src/jaxsim/physics/algos/terrain.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/physics/algos/utils.py` & `jaxsim-0.1.dev149/src/jaxsim/physics/algos/utils.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/physics/model/ground_contact.py` & `jaxsim-0.1.dev149/src/jaxsim/physics/model/ground_contact.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/physics/model/physics_model.py` & `jaxsim-0.1.dev149/src/jaxsim/physics/model/physics_model.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/physics/model/physics_model_state.py` & `jaxsim-0.1.dev149/src/jaxsim/physics/model/physics_model_state.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/simulation/integrators.py` & `jaxsim-0.1.dev149/src/jaxsim/simulation/integrators.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/simulation/ode.py` & `jaxsim-0.1.dev149/src/jaxsim/simulation/ode.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/simulation/ode_data.py` & `jaxsim-0.1.dev149/src/jaxsim/simulation/ode_data.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/simulation/ode_integration.py` & `jaxsim-0.1.dev149/src/jaxsim/simulation/ode_integration.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/simulation/simulator.py` & `jaxsim-0.1.dev149/src/jaxsim/simulation/simulator.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/simulation/simulator_callbacks.py` & `jaxsim-0.1.dev149/src/jaxsim/simulation/simulator_callbacks.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/typing.py` & `jaxsim-0.1.dev149/src/jaxsim/typing.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim/utils.py` & `jaxsim-0.1.dev149/src/jaxsim/utils.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev142/src/jaxsim.egg-info/PKG-INFO` & `jaxsim-0.1.dev149/src/jaxsim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxsim
-Version: 0.1.dev142
+Version: 0.1.dev149
 Summary: A physics engine in reduced coordinates implemented with JAX.
 Home-page: https://github.com/ami-iit/jaxsim
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/jaxsim/releases
 Project-URL: Source, https://github.com/ami-iit/jaxsim
```

### Comparing `jaxsim-0.1.dev142/src/jaxsim.egg-info/SOURCES.txt` & `jaxsim-0.1.dev149/src/jaxsim.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 src/jaxsim/parsers/__init__.py
 src/jaxsim/parsers/kinematic_graph.py
 src/jaxsim/parsers/descriptions/__init__.py
 src/jaxsim/parsers/descriptions/collision.py
 src/jaxsim/parsers/descriptions/joint.py
 src/jaxsim/parsers/descriptions/link.py
 src/jaxsim/parsers/descriptions/model.py
-src/jaxsim/parsers/sdf/__init__.py
-src/jaxsim/parsers/sdf/parser.py
-src/jaxsim/parsers/sdf/utils.py
+src/jaxsim/parsers/rod/__init__.py
+src/jaxsim/parsers/rod/parser.py
+src/jaxsim/parsers/rod/utils.py
 src/jaxsim/physics/__init__.py
 src/jaxsim/physics/algos/__init__.py
 src/jaxsim/physics/algos/aba.py
 src/jaxsim/physics/algos/crba.py
 src/jaxsim/physics/algos/forward_kinematics.py
 src/jaxsim/physics/algos/jacobian.py
 src/jaxsim/physics/algos/rnea.py
```

