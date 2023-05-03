# Comparing `tmp/ilpy-0.2.3.tar.gz` & `tmp/ilpy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilpy-0.2.3.tar", last modified: Mon Mar 13 21:41:55 2023, max compression
+gzip compressed data, was "ilpy-0.3.0.tar", last modified: Wed May  3 13:44:00 2023, max compression
```

## Comparing `ilpy-0.2.3.tar` & `ilpy-0.3.0.tar`

### file list

```diff
@@ -1,50 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 21:41:55.340090 ilpy-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-13 21:41:43.000000 ilpy-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-13 21:41:55.340090 ilpy-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-03-13 21:41:43.000000 ilpy-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 21:41:55.332090 ilpy-0.2.3/ilpy/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-13 21:41:43.000000 ilpy-0.2.3/ilpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-03-13 21:41:43.000000 ilpy-0.2.3/ilpy/decl.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 21:41:55.336090 ilpy-0.2.3/ilpy/impl/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-13 21:41:43.000000 ilpy-0.2.3/ilpy/impl/config.h
--rw-r--r--   0 runner    (1001) docker     (123)    47719 2023-03-13 21:41:43.000000 ilpy-0.2.3/ilpy/impl/gurobi_c.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 21:41:55.340090 ilpy-0.2.3/ilpy/impl/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/BackendPreference.h
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/CplexBackend.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/CplexBackend.h
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/GurobiBackend.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/GurobiBackend.h
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/LinearConstraint.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/LinearConstraint.h
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/LinearConstraints.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/LinearConstraints.h
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/LinearObjective.h
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/LinearSolverBackend.h
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/LinearSolverBackendFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/QuadraticObjective.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/QuadraticObjective.h
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/QuadraticSolverBackend.h
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/QuadraticSolverBackendFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/QuadraticSolverParameters.h
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/Relation.h
--rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/ScipBackend.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/ScipBackend.h
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/Sense.h
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/Solution.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/Solution.h
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/SolverFactory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/SolverFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-13 21:41:44.000000 ilpy-0.2.3/ilpy/impl/solvers/VariableType.h
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 21:41:43.000000 ilpy-0.2.3/ilpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-03-13 21:41:43.000000 ilpy-0.2.3/ilpy/wrapper.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-03-13 21:41:43.000000 ilpy-0.2.3/ilpy/wrapper.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 21:41:55.332090 ilpy-0.2.3/ilpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-13 21:41:55.000000 ilpy-0.2.3/ilpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-03-13 21:41:55.000000 ilpy-0.2.3/ilpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 21:41:55.000000 ilpy-0.2.3/ilpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-13 21:41:55.000000 ilpy-0.2.3/ilpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-13 21:41:55.000000 ilpy-0.2.3/ilpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-13 21:41:43.000000 ilpy-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 21:41:55.340090 ilpy-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-03-13 21:41:43.000000 ilpy-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:44:00.908895 ilpy-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-03 13:43:48.000000 ilpy-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 13:43:48.000000 ilpy-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-03 13:43:48.000000 ilpy-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-03 13:44:00.908895 ilpy-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-03 13:43:48.000000 ilpy-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:44:00.900895 ilpy-0.3.0/ilpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/decl.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    16062 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:44:00.900895 ilpy-0.3.0/ilpy/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/config.h
+-rw-r--r--   0 runner    (1001) docker     (123)    61557 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/gurobi_c.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:44:00.908895 ilpy-0.3.0/ilpy/impl/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/BackendPreference.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/Constraint.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/Constraint.h
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/Constraints.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/Constraints.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/CplexBackend.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/CplexBackend.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/GurobiBackend.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/GurobiBackend.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/Objective.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/Objective.h
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/Relation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/ScipBackend.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/ScipBackend.h
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/Sense.h
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/Solution.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/Solution.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/SolverBackend.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/SolverFactory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/SolverFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/VariableType.h
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/wrapper.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/wrapper.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:44:00.900895 ilpy-0.3.0/ilpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-03 13:44:00.000000 ilpy-0.3.0/ilpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-03 13:44:00.000000 ilpy-0.3.0/ilpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:44:00.000000 ilpy-0.3.0/ilpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-03 13:44:00.000000 ilpy-0.3.0/ilpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-03 13:44:00.000000 ilpy-0.3.0/ilpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-03 13:43:48.000000 ilpy-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 13:44:00.908895 ilpy-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-03 13:43:48.000000 ilpy-0.3.0/setup.py
```

### Comparing `ilpy-0.2.3/README.md` & `ilpy-0.3.0/CONTRIBUTING.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,10 @@
-# ilpy
+# Contributing
 
-Unified python wrappers for popular ILP solvers
-
-## Installation
-
-```bash
-conda install -c funkelab ilpy
-```
+ilpy welcomes contributions
 
 ## Local development
 
 ilpy links against SCIP, so you must have SCIP installed in your environment.
 (You can install via conda)
 
 ```bash
@@ -21,38 +15,39 @@
 
 ```bash
 git clone <your-fork>
 cd ilpy
 pip install -e .[dev]
 ```
 
-### Deploying
+## Deploying
+
+> *This is a note for maintainers*
 
-> Only for maintainers
+Bump the version in `__init__.py` and commit it.
 
-bump the version in both `setup.py` and `__init__.py` (unless you later
-setup auto versioning), and commit it.  Then create an annotated tag with:
+Then create an annotated tag with:
 
 ```bash
 git tag -a vX.Y.Z -m "vX.Y.Z"
 ```
 
 Then push the tag to github:
 
 ```bash
 git push upstream --follow-tags
 ```
 
 This will trigger `ci.yaml` to run, which will build a source distribution
 (only) and upload it to pypi.
 
-Once that is done, to deploy to anaconda, open a PR to https://github.com/funkelab/ilpy-feedstock
+Once that is done, to deploy to anaconda, open a PR to <https://github.com/funkelab/ilpy-feedstock>
 that update the version and SHA256 hash in `meta.yaml`.
 (You can find the hash in the files page of the appropriate version release on
-pypi... for example https://pypi.org/project/ilpy/0.2.2/#files)
+pypi... for example <https://pypi.org/project/ilpy/0.2.2/#files>)
 
 ```yaml
 # ...
 {% set version = "<UPDATE VERSION HERE>" %}
 
 source:
   # ...
```

### Comparing `ilpy-0.2.3/ilpy/impl/gurobi_c.h` & `ilpy-0.3.0/ilpy/impl/gurobi_c.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-/* Copyright 2019, Gurobi Optimization, LLC */
+/* Copyright 2022, Gurobi Optimization, LLC */
  
 #ifndef _GUROBI_C_H
 #define _GUROBI_C_H
  
 #ifdef __cplusplus
 extern "C" {
 #endif
  
 #include <stdio.h>
 
+typedef struct _GRBbatch GRBbatch;
 typedef struct _GRBmodel GRBmodel;
 typedef struct _GRBenv GRBenv;
 
 #if defined(_WIN64) && !defined(WIN64)
 #define WIN64
 #endif
 
@@ -21,18 +22,30 @@
 #endif
 
 #if !defined(WIN32) && !defined(WIN64)
 #define __cdecl
 #define __stdcall
 #endif
 
+/* Deprecation macro */
+
+#if __cplusplus >= 201103L
+#  define GRB_DEPRECATED(WHY,X) [[deprecated(WHY)]] X
+#elif defined(__GNUC__) || defined(__clang__)
+#  define GRB_DEPRECATED(WHY,X) X __attribute__((deprecated))
+#elif defined(_MSC_VER)
+#  define GRB_DEPRECATED(WHY,X) __declspec(deprecated) X
+#else
+#  define GRB_DEPRECATED(WHY,X) X
+#endif
+
 /* Version numbers */
 
-#define GRB_VERSION_MAJOR     8
-#define GRB_VERSION_MINOR     1
+#define GRB_VERSION_MAJOR     9
+#define GRB_VERSION_MINOR     5
 #define GRB_VERSION_TECHNICAL 1
 
 /* Default and max priority for Compute Server jobs */
 
 #define DEFAULT_CS_PRIORITY 0
 #define MAX_CS_PRIORITY 100
 
@@ -73,14 +86,15 @@
 #define GRB_ERROR_EXCEED_2B_NONZEROS       10025
 #define GRB_ERROR_INVALID_PIECEWISE_OBJ    10026
 #define GRB_ERROR_UPDATEMODE_CHANGE        10027
 #define GRB_ERROR_CLOUD                    10028
 #define GRB_ERROR_MODEL_MODIFICATION       10029
 #define GRB_ERROR_CSWORKER                 10030
 #define GRB_ERROR_TUNE_MODEL_TYPES         10031
+#define GRB_ERROR_SECURITY                 10032
 
 /* Constraint senses */
 
 #define GRB_LESS_EQUAL    '<'
 #define GRB_GREATER_EQUAL '>'
 #define GRB_EQUAL         '='
 
@@ -108,21 +122,27 @@
 #define GRB_UNDEFINED 1e101
 #define GRB_MAXINT    2000000000
 
 /* Limits */
 
 #define GRB_MAX_NAMELEN    255
 #define GRB_MAX_STRLEN     512
+#define GRB_MAX_TAGLEN    10240
 #define GRB_MAX_CONCURRENT 64
 
+/* Callback */
+
+#define CB_ARGS GRBmodel *model, void *cbdata, int where, void *usrdata
+#define LOGCB_ARGS char *msg, void *logdata
+
 /* Query interface */
 
 int __stdcall
   GRBgetattrinfo(GRBmodel *model, const char *attrname, int *datatypeP,
-                 int *sizeP, int *settableP);
+                 int *attrtypeP, int *settableP);
 int __stdcall
   GRBisattravailable(GRBmodel *model, const char *attrname);
 int __stdcall
   GRBgetintattr(GRBmodel *model, const char *attrname, int *valueP);
 int __stdcall
   GRBsetintattr(GRBmodel *model, const char *attrname, int newvalue);
 int __stdcall
@@ -201,31 +221,40 @@
                      int first, int len, char **newvalues);
 int __stdcall
   GRBgetstrattrlist(GRBmodel *model, const char *attrname,
                     int len, int *ind, char **values);
 int __stdcall
   GRBsetstrattrlist(GRBmodel *model, const char *attrname,
                     int len, int *ind, char **newvalues);
-
-/* Callback */
-#define CB_ARGS GRBmodel *model, void *cbdata, int where, void *usrdata
-
 int __stdcall
   GRBsetcallbackfunc(GRBmodel *model,
                      int (__stdcall *cb)(CB_ARGS),
                      void  *usrdata);
 int __stdcall
+  GRBgetcallbackfuncenv(GRBenv *env,
+                        int (__stdcall **cbP)(CB_ARGS));
+int __stdcall
+  GRBsetcallbackfuncenv(GRBenv *env,
+                        int (__stdcall *cb)(CB_ARGS),
+                        void  *usrdata);
+int __stdcall
   GRBgetcallbackfunc(GRBmodel *model,
                      int (__stdcall **cbP)(CB_ARGS));
 int __stdcall
-  GRBsetlogcallbackfunc(GRBmodel *model,
-                        int (__stdcall *cb)(char *msg));
-int __stdcall
-  GRBsetlogcallbackfuncenv(GRBenv *env,
-                           int (__stdcall *cb)(char *msg));
+  GRBsetlogcallbackfunc(GRBmodel       *model,
+                        int (__stdcall *cb)(LOGCB_ARGS),
+                        void           *logdata);
+int __stdcall
+  GRBsetlogcallbackfuncenv(GRBenv         *env,
+                           int (__stdcall *cb)(LOGCB_ARGS),
+                           void           *logdata);
+int __stdcall
+  GRBgetlogcallbackfuncenv(GRBenv         *env,
+                           int (__stdcall **cbP)(LOGCB_ARGS),
+                           void           **logdataP);
 int __stdcall
   GRBcbget(void *cbdata, int where, int what, void *resultP);
 int __stdcall
   GRBcbsetparam(void *cbdata, const char *paramname, const char *newvalue);
 int __stdcall
   GRBcbsolution(void *cbdata, const double *solution, double *objvalP);
 int __stdcall
@@ -260,49 +289,68 @@
 #define GRB_INT_ATTR_IS_MIP        "IsMIP"         /* Is model a MIP? */
 #define GRB_INT_ATTR_IS_QP         "IsQP"          /* Model has quadratic obj? */
 #define GRB_INT_ATTR_IS_QCP        "IsQCP"         /* Model has quadratic constr? */
 #define GRB_INT_ATTR_IS_MULTIOBJ   "IsMultiObj"    /* Model has multiple objectives? */
 #define GRB_STR_ATTR_SERVER        "Server"        /* Name of Compute Server */
 #define GRB_STR_ATTR_JOBID         "JobID"         /* Compute Server job ID */
 #define GRB_INT_ATTR_LICENSE_EXPIRATION "LicenseExpiration" /* License expiration date */
+#define GRB_INT_ATTR_NUMTAGGED     "NumTagged"     /* number of tagged elements in model */
+#define GRB_INT_ATTR_FINGERPRINT   "Fingerprint"   /* fingerprint computed from the model data and attributes influencing the optimization process */
+
+/* Batch attributes */
+#define GRB_INT_ATTR_BATCHERRORCODE    "BatchErrorCode"
+#define GRB_STR_ATTR_BATCHERRORMESSAGE "BatchErrorMessage"
+#define GRB_STR_ATTR_BATCHID           "BatchID"
+#define GRB_INT_ATTR_BATCHSTATUS       "BatchStatus"
 
 /* Variable attributes */
 
 #define GRB_DBL_ATTR_LB             "LB"              /* Lower bound */
 #define GRB_DBL_ATTR_UB             "UB"              /* Upper bound */
 #define GRB_DBL_ATTR_OBJ            "Obj"             /* Objective coeff */
 #define GRB_CHAR_ATTR_VTYPE         "VType"           /* Integrality type */
-#define GRB_DBL_ATTR_START          "Start"           /* MIP start value */
+#define GRB_DBL_ATTR_START          "Start"           /* MIP start value, depends on startnumber */
 #define GRB_DBL_ATTR_PSTART         "PStart"          /* LP primal solution warm start */
 #define GRB_INT_ATTR_BRANCHPRIORITY "BranchPriority"  /* MIP branch priority */
 #define GRB_STR_ATTR_VARNAME        "VarName"         /* Variable name */
 #define GRB_INT_ATTR_PWLOBJCVX      "PWLObjCvx"       /* Convexity of variable PWL obj */
-#define GRB_DBL_ATTR_VARHINTVAL     "VarHintVal"
-#define GRB_INT_ATTR_VARHINTPRI     "VarHintPri"
-#define GRB_INT_ATTR_PARTITION      "Partition"
+#define GRB_DBL_ATTR_VARHINTVAL     "VarHintVal"      /* variable hint value */
+#define GRB_INT_ATTR_VARHINTPRI     "VarHintPri"      /* variable hint priority */
+#define GRB_INT_ATTR_PARTITION      "Partition"       /* user specified variable partition */
+#define GRB_INT_ATTR_POOLIGNORE     "PoolIgnore"      /* Ignore variable for solution identity check in solution pool */
+#define GRB_STR_ATTR_VTAG           "VTag"            /* variable tags */
 
 /* Constraint attributes */
 
+#define GRB_STR_ATTR_CTAG       "CTag"       /* linear constraint tags */
 #define GRB_DBL_ATTR_RHS        "RHS"        /* RHS */
 #define GRB_DBL_ATTR_DSTART     "DStart"     /* LP dual solution warm start */
 #define GRB_CHAR_ATTR_SENSE     "Sense"      /* Sense ('<', '>', or '=') */
 #define GRB_STR_ATTR_CONSTRNAME "ConstrName" /* Constraint name */
 #define GRB_INT_ATTR_LAZY       "Lazy"       /* Lazy constraint? */
 
 /* Quadratic constraint attributes */
 
+#define GRB_STR_ATTR_QCTAG    "QCTag"   /* quadratic constraint tags */
 #define GRB_DBL_ATTR_QCRHS    "QCRHS"   /* QC RHS */
 #define GRB_CHAR_ATTR_QCSENSE "QCSense" /* QC sense ('<', '>', or '=') */
 #define GRB_STR_ATTR_QCNAME   "QCName"  /* QC name */
 
 /* General constraint attributes */
 
 #define GRB_INT_ATTR_GENCONSTRTYPE  "GenConstrType"  /* Type of general constraint */
 #define GRB_STR_ATTR_GENCONSTRNAME  "GenConstrName"  /* Name of general constraint */
 
+/* General function constraint attributes */
+
+#define GRB_INT_ATTR_FUNCPIECES      "FuncPieces"       /* An option for PWL translation */
+#define GRB_DBL_ATTR_FUNCPIECEERROR  "FuncPieceError"    /* An option for PWL translation */
+#define GRB_DBL_ATTR_FUNCPIECELENGTH "FuncPieceLength"  /* An option for PWL translation */
+#define GRB_DBL_ATTR_FUNCPIECERATIO  "FuncPieceRatio"   /* An option for PWL translation */
+
 /* Model statistics */
 
 #define GRB_DBL_ATTR_MAX_COEFF      "MaxCoeff"     /* Max (abs) nz coeff in A */
 #define GRB_DBL_ATTR_MIN_COEFF      "MinCoeff"     /* Min (abs) nz coeff in A */
 #define GRB_DBL_ATTR_MAX_BOUND      "MaxBound"     /* Max (abs) finite var bd */
 #define GRB_DBL_ATTR_MIN_BOUND      "MinBound"     /* Min (abs) var bd */
 #define GRB_DBL_ATTR_MAX_OBJ_COEFF  "MaxObjCoeff"  /* Max (abs) obj coeff */
@@ -317,34 +365,36 @@
 #define GRB_DBL_ATTR_MIN_QCLCOEFF   "MinQCLCoeff"  /* Min (abs) nz coeff in linear part of Q */
 #define GRB_DBL_ATTR_MAX_QCRHS      "MaxQCRHS"     /* Max (abs) rhs of Q */
 #define GRB_DBL_ATTR_MIN_QCRHS      "MinQCRHS"     /* Min (abs) rhs of Q */
 
 /* Model solution attributes */
 
 #define GRB_DBL_ATTR_RUNTIME       "Runtime"     /* Run time for optimization */
+#define GRB_DBL_ATTR_WORK          "Work"        /* Work for optimization */
 #define GRB_INT_ATTR_STATUS        "Status"      /* Optimization status */
 #define GRB_DBL_ATTR_OBJVAL        "ObjVal"      /* Solution objective */
 #define GRB_DBL_ATTR_OBJBOUND      "ObjBound"    /* Best bound on solution */
 #define GRB_DBL_ATTR_OBJBOUNDC     "ObjBoundC"   /* Continuous bound */
 #define GRB_DBL_ATTR_POOLOBJBOUND  "PoolObjBound" /* Best bound on pool solution */
-#define GRB_DBL_ATTR_POOLOBJVAL    "PoolObjVal"  /* Solution objective for solutionnumber */
+#define GRB_DBL_ATTR_POOLOBJVAL    "PoolObjVal"  /* Solution objective, depends on solutionnumber */
 #define GRB_DBL_ATTR_MIPGAP        "MIPGap"      /* MIP optimality gap */
 #define GRB_INT_ATTR_SOLCOUNT      "SolCount"    /* # of solutions found */
 #define GRB_DBL_ATTR_ITERCOUNT     "IterCount"   /* Iters performed (simplex) */
 #define GRB_INT_ATTR_BARITERCOUNT  "BarIterCount" /* Iters performed (barrier) */
 #define GRB_DBL_ATTR_NODECOUNT     "NodeCount"    /* Nodes explored (B&C) */
 #define GRB_DBL_ATTR_OPENNODECOUNT "OpenNodeCount" /* Unexplored nodes (B&C) */
 #define GRB_INT_ATTR_HASDUALNORM   "HasDualNorm"  /* 0, no basis,
                                                      1, has basis, so can be computed
                                                      2, available */
+#define GRB_INT_ATTR_CONCURRENTWINMETHOD  "ConcurrentWinMethod"      /* method that solved LP using concurrent */
 
 /* Variable attributes related to the current solution */
 
 #define GRB_DBL_ATTR_X         "X"         /* Solution value */
-#define GRB_DBL_ATTR_XN        "Xn"        /* Alternate MIP solution */
+#define GRB_DBL_ATTR_XN        "Xn"        /* Alternate MIP solution, depends on solutionnumber */
 #define GRB_DBL_ATTR_BARX      "BarX"      /* Best barrier iterate */
 #define GRB_DBL_ATTR_RC        "RC"        /* Reduced costs */
 #define GRB_DBL_ATTR_VDUALNORM "VDualNorm" /* Dual norm square */
 #define GRB_INT_ATTR_VBASIS    "VBasis"    /* Variable basis status */
 
 /* Constraint attributes related to the current solution */
 
@@ -353,14 +403,15 @@
 #define GRB_DBL_ATTR_SLACK     "Slack"     /* Constraint slack */
 #define GRB_DBL_ATTR_QCSLACK   "QCSlack"   /* QC Constraint slack */
 #define GRB_DBL_ATTR_CDUALNORM "CDualNorm" /* Dual norm square */
 #define GRB_INT_ATTR_CBASIS    "CBasis"    /* Constraint basis status */
 
 /* Solution quality attributes */
 
+#define GRB_DBL_ATTR_MAX_VIO                "MaxVio"
 #define GRB_DBL_ATTR_BOUND_VIO              "BoundVio"
 #define GRB_DBL_ATTR_BOUND_SVIO             "BoundSVio"
 #define GRB_INT_ATTR_BOUND_VIO_INDEX        "BoundVioIndex"
 #define GRB_INT_ATTR_BOUND_SVIO_INDEX       "BoundSVioIndex"
 #define GRB_DBL_ATTR_BOUND_VIO_SUM          "BoundVioSum"
 #define GRB_DBL_ATTR_BOUND_SVIO_SUM         "BoundSVioSum"
 #define GRB_DBL_ATTR_CONSTR_VIO             "ConstrVio"
@@ -414,14 +465,21 @@
 #define GRB_INT_ATTR_IIS_LB        "IISLB"        /* Boolean: Is var LB in IIS? */
 #define GRB_INT_ATTR_IIS_UB        "IISUB"        /* Boolean: Is var UB in IIS? */
 #define GRB_INT_ATTR_IIS_CONSTR    "IISConstr"    /* Boolean: Is constr in IIS? */
 #define GRB_INT_ATTR_IIS_SOS       "IISSOS"       /* Boolean: Is SOS in IIS? */
 #define GRB_INT_ATTR_IIS_QCONSTR   "IISQConstr"   /* Boolean: Is QConstr in IIS? */
 #define GRB_INT_ATTR_IIS_GENCONSTR "IISGenConstr" /* Boolean: Is general constr in IIS? */
 
+#define GRB_INT_ATTR_IIS_LBFORCE        "IISLBForce"        /* Force var LB to be (1) or to not be (0) in final IIS */
+#define GRB_INT_ATTR_IIS_UBFORCE        "IISUBForce"        /* Force var UB to be (1) or to not be (0) in final IIS */
+#define GRB_INT_ATTR_IIS_CONSTRFORCE    "IISConstrForce"    /* Force constr to be (1) or to not be (0) in final IIS */
+#define GRB_INT_ATTR_IIS_SOSFORCE       "IISSOSForce"       /* Force SOS to be (1) or to not be (0) in final IIS */
+#define GRB_INT_ATTR_IIS_QCONSTRFORCE   "IISQConstrForce"   /* Force QConstr to be (1) or to not be (0) in final IIS */
+#define GRB_INT_ATTR_IIS_GENCONSTRFORCE "IISGenConstrForce" /* Force general constr to be (1) or to not be (0) in final IIS */
+
 /* Tuning */
 
 #define GRB_INT_ATTR_TUNE_RESULTCOUNT "TuneResultCount"
 
 /* Advanced simplex features */
 
 #define GRB_DBL_ATTR_FARKASDUAL  "FarkasDual"
@@ -431,40 +489,71 @@
 #define GRB_INT_ATTR_UNBDVAR     "UnbdVar"
 
 /* Presolve attribute */
 
 #define GRB_INT_ATTR_VARPRESTAT "VarPreStat"
 #define GRB_DBL_ATTR_PREFIXVAL  "PreFixVal"
 
-/* Multi objective attribute, controlled by parameter ObjNumber (= i) */
-
+/* Multi objective attribute, controlled by parameter ObjNumber (= i)
+ *
+ * Note if you add an new attribute, adjust the const array
+ * OBJNUMATTRNAMES and define OBJNUMATTRS in attrcache.c.
+ */
 #define GRB_DBL_ATTR_OBJN         "ObjN"         /* ith objective */
-#define GRB_DBL_ATTR_OBJNVAL      "ObjNVal"      /* Solution objective for Multi-objectives */
+#define GRB_DBL_ATTR_OBJNVAL      "ObjNVal"      /* Solution objective for Multi-objectives, also depends on solutionnumber */
 #define GRB_DBL_ATTR_OBJNCON      "ObjNCon"      /* constant term */
 #define GRB_DBL_ATTR_OBJNWEIGHT   "ObjNWeight"   /* weight */
 #define GRB_INT_ATTR_OBJNPRIORITY "ObjNPriority" /* priority */
 #define GRB_DBL_ATTR_OBJNRELTOL   "ObjNRelTol"   /* relative tolerance */
 #define GRB_DBL_ATTR_OBJNABSTOL   "ObjNAbsTol"   /* absolute tolerance */
 #define GRB_STR_ATTR_OBJNNAME     "ObjNName"     /* name */
+
+/* Scenario attributes, controlled by parameter ScenarioNumber (= i)
+ *
+ * Note if you add an new attribute, adjust the const array
+ * SCENARIONUMATTRNAMES and define SCENARIONUMATTRS in attrcache.c.
+ */
+
+#define GRB_DBL_ATTR_SCENNLB       "ScenNLB"       /* lower bound in scenario i */
+#define GRB_DBL_ATTR_SCENNUB       "ScenNUB"       /* upper bound in scenario i */
+#define GRB_DBL_ATTR_SCENNOBJ      "ScenNObj"      /* objective in scenario i */
+#define GRB_DBL_ATTR_SCENNRHS      "ScenNRHS"      /* right hand side in scenario i */
+#define GRB_STR_ATTR_SCENNNAME     "ScenNName"     /* name of scenario i */
+#define GRB_DBL_ATTR_SCENNX        "ScenNX"        /* solution value in scenario i */
+#define GRB_DBL_ATTR_SCENNOBJBOUND "ScenNObjBound" /* objective bound for scenario i */
+#define GRB_DBL_ATTR_SCENNOBJVAL   "ScenNObjVal"   /* objective value for scenario i */
+
 #define GRB_INT_ATTR_NUMOBJ       "NumObj"       /* number of objectives */
+#define GRB_INT_ATTR_NUMSCENARIOS "NumScenarios" /* number of scenarios */
 #define GRB_INT_ATTR_NUMSTART     "NumStart"     /* number of MIP starts */
 
+
 /* Alternate define */
 
 #define GRB_DBL_ATTR_Xn "Xn"
 
 /* General constraints */
 
 #define GRB_GENCONSTR_MAX         0
 #define GRB_GENCONSTR_MIN         1
 #define GRB_GENCONSTR_ABS         2
 #define GRB_GENCONSTR_AND         3
 #define GRB_GENCONSTR_OR          4
-#define GRB_GENCONSTR_INDICATOR   5
-
+#define GRB_GENCONSTR_NORM        5
+#define GRB_GENCONSTR_INDICATOR   6
+#define GRB_GENCONSTR_PWL         7
+#define GRB_GENCONSTR_POLY        8
+#define GRB_GENCONSTR_EXP         9
+#define GRB_GENCONSTR_EXPA       10
+#define GRB_GENCONSTR_LOG        11
+#define GRB_GENCONSTR_LOGA       12
+#define GRB_GENCONSTR_POW        13
+#define GRB_GENCONSTR_SIN        14
+#define GRB_GENCONSTR_COS        15
+#define GRB_GENCONSTR_TAN        16
 
 /*
    CALLBACKS
 */
 
 /* For callback */
 
@@ -473,14 +562,15 @@
 #define GRB_CB_SIMPLEX   2
 #define GRB_CB_MIP       3
 #define GRB_CB_MIPSOL    4
 #define GRB_CB_MIPNODE   5
 #define GRB_CB_MESSAGE   6
 #define GRB_CB_BARRIER   7
 #define GRB_CB_MULTIOBJ  8
+#define GRB_CB_IIS       9
 
 /* Supported names for callback */
 
 #define GRB_CB_PRE_COLDEL  1000
 #define GRB_CB_PRE_ROWDEL  1001
 #define GRB_CB_PRE_SENCHG  1002
 #define GRB_CB_PRE_BNDCHG  1003
@@ -488,54 +578,65 @@
 
 #define GRB_CB_SPX_ITRCNT  2000
 #define GRB_CB_SPX_OBJVAL  2001
 #define GRB_CB_SPX_PRIMINF 2002
 #define GRB_CB_SPX_DUALINF 2003
 #define GRB_CB_SPX_ISPERT  2004
 
-#define GRB_CB_MIP_OBJBST  3000
-#define GRB_CB_MIP_OBJBND  3001
-#define GRB_CB_MIP_NODCNT  3002
-#define GRB_CB_MIP_SOLCNT  3003
-#define GRB_CB_MIP_CUTCNT  3004
-#define GRB_CB_MIP_NODLFT  3005
-#define GRB_CB_MIP_ITRCNT  3006
-#define GRB_CB_MIP_OBJBNDC 3007
-
-#define GRB_CB_MIPSOL_SOL     4001
-#define GRB_CB_MIPSOL_OBJ     4002
-#define GRB_CB_MIPSOL_OBJBST  4003
-#define GRB_CB_MIPSOL_OBJBND  4004
-#define GRB_CB_MIPSOL_NODCNT  4005
-#define GRB_CB_MIPSOL_SOLCNT  4006
-#define GRB_CB_MIPSOL_OBJBNDC 4007
-
-#define GRB_CB_MIPNODE_STATUS  5001
-#define GRB_CB_MIPNODE_REL     5002
-#define GRB_CB_MIPNODE_OBJBST  5003
-#define GRB_CB_MIPNODE_OBJBND  5004
-#define GRB_CB_MIPNODE_NODCNT  5005
-#define GRB_CB_MIPNODE_SOLCNT  5006
-#define GRB_CB_MIPNODE_BRVAR   5007
-#define GRB_CB_MIPNODE_OBJBNDC 5008
+#define GRB_CB_MIP_OBJBST         3000
+#define GRB_CB_MIP_OBJBND         3001
+#define GRB_CB_MIP_NODCNT         3002
+#define GRB_CB_MIP_SOLCNT         3003
+#define GRB_CB_MIP_CUTCNT         3004
+#define GRB_CB_MIP_NODLFT         3005
+#define GRB_CB_MIP_ITRCNT         3006
+#define GRB_CB_MIP_OPENSCENARIOS  3007
+#define GRB_CB_MIP_PHASE          3008
+
+#define GRB_CB_MIPSOL_SOL            4001
+#define GRB_CB_MIPSOL_OBJ            4002
+#define GRB_CB_MIPSOL_OBJBST         4003
+#define GRB_CB_MIPSOL_OBJBND         4004
+#define GRB_CB_MIPSOL_NODCNT         4005
+#define GRB_CB_MIPSOL_SOLCNT         4006
+#define GRB_CB_MIPSOL_OPENSCENARIOS  4007
+#define GRB_CB_MIPSOL_PHASE          4008
+
+#define GRB_CB_MIPNODE_STATUS         5001
+#define GRB_CB_MIPNODE_REL            5002
+#define GRB_CB_MIPNODE_OBJBST         5003
+#define GRB_CB_MIPNODE_OBJBND         5004
+#define GRB_CB_MIPNODE_NODCNT         5005
+#define GRB_CB_MIPNODE_SOLCNT         5006
+#define GRB_CB_MIPNODE_BRVAR          5007
+#define GRB_CB_MIPNODE_OPENSCENARIOS  5008
+#define GRB_CB_MIPNODE_PHASE          5009
 
 #define GRB_CB_MSG_STRING  6001
 #define GRB_CB_RUNTIME     6002
+#define GRB_CB_WORK        6003
 
 #define GRB_CB_BARRIER_ITRCNT  7001
 #define GRB_CB_BARRIER_PRIMOBJ 7002
 #define GRB_CB_BARRIER_DUALOBJ 7003
 #define GRB_CB_BARRIER_PRIMINF 7004
 #define GRB_CB_BARRIER_DUALINF 7005
 #define GRB_CB_BARRIER_COMPL   7006
 
 #define GRB_CB_MULTIOBJ_OBJCNT  8001
 #define GRB_CB_MULTIOBJ_SOLCNT  8002
 #define GRB_CB_MULTIOBJ_SOL     8003
 
+#define GRB_CB_IIS_CONSTRMIN    9001
+#define GRB_CB_IIS_CONSTRMAX    9002
+#define GRB_CB_IIS_CONSTRGUESS  9003
+#define GRB_CB_IIS_BOUNDMIN     9004
+#define GRB_CB_IIS_BOUNDMAX     9005
+#define GRB_CB_IIS_BOUNDGUESS   9006
+
 #define GRB_FEASRELAX_LINEAR      0
 #define GRB_FEASRELAX_QUADRATIC   1
 #define GRB_FEASRELAX_CARDINALITY 2
 
 int __stdcall
   GRBgetcoeff(GRBmodel *model, int constr, int var, double *valP);
 int __stdcall
@@ -564,61 +665,101 @@
 int __stdcall
   GRBgetgenconstrAnd(GRBmodel *model, int genconstr, int *resvarP,
                      int *nvarsP, int *vars);
 int __stdcall
   GRBgetgenconstrOr(GRBmodel *model, int genconstr, int *resvarP,
                     int *nvarsP, int *vars);
 int __stdcall
+  GRBgetgenconstrNorm(GRBmodel *model, int genconstr, int *resvarP,
+                      int *nvarsP, int *vars, double *whichP);
+int __stdcall
   GRBgetgenconstrIndicator(GRBmodel *model, int genconstr, int *binvarP, int *binvalP,
                            int *nvarsP, int *vars, double *vals,
                            char *senseP, double *rhsP);
 int __stdcall
+  GRBgetgenconstrPWL(GRBmodel *model, int genconstr, int *xvarP, int *yvarP,
+                     int *nptsP, double *xpts, double *ypts);
+int __stdcall
+  GRBgetgenconstrPoly(GRBmodel *model, int genconstr, int *xvarP,
+                      int *yvarP, int *plenP, double *p);
+int __stdcall
+  GRBgetgenconstrExpA(GRBmodel *model, int genconstr, int *xvarP,
+                      int *yvarP, double *aP);
+int __stdcall
+  GRBgetgenconstrLogA(GRBmodel *model, int genconstr, int *xvarP,
+                      int *yvarP, double *aP);
+int __stdcall
+  GRBgetgenconstrPow(GRBmodel *model, int genconstr, int *xvarP,
+                     int *yvarP, double *aP);
+int __stdcall
+  GRBgetgenconstrExp(GRBmodel *model, int genconstr, int *xvarP, int *yvarP);
+int __stdcall
+  GRBgetgenconstrLog(GRBmodel *model, int genconstr, int *xvarP, int *yvarP);
+int __stdcall
+  GRBgetgenconstrSin(GRBmodel *model, int genconstr, int *xvarP, int *yvarP);
+int __stdcall
+  GRBgetgenconstrCos(GRBmodel *model, int genconstr, int *xvarP, int *yvarP);
+int __stdcall
+  GRBgetgenconstrTan(GRBmodel *model, int genconstr, int *xvarP, int *yvarP);
+int __stdcall
   GRBgetq(GRBmodel *model, int *numqnzP, int *qrow, int *qcol, double *qval);
 int __stdcall
   GRBgetqconstr(GRBmodel *model, int qconstr,
                 int *numlnzP, int *lind, double *lval,
                 int *numqnzP, int *qrow, int *qcol, double *qval);
 int __stdcall
   GRBgetvarbyname(GRBmodel *model, const char *name, int *indexP);
 int __stdcall
   GRBgetconstrbyname(GRBmodel *model, const char *name, int *indexP);
 int __stdcall
+  GRBgetqconstrbyname(GRBmodel *model, const char *name, int *indexP);
+int __stdcall
   GRBgetpwlobj(GRBmodel *model, int var, int *pointsP,
                double *x, double *y);
 
 int __stdcall
   GRBoptimize(GRBmodel *model);
 int __stdcall
   GRBoptimizeasync(GRBmodel *model);
+int __stdcall
+  GRBoptimizebatch(GRBmodel *model, char *batchid);
 
 GRBmodel * __stdcall
   GRBcopymodel(GRBmodel *model);
-GRBmodel * __stdcall
-  GRBfixedmodel(GRBmodel *model);
+int __stdcall
+  GRBfixmodel(GRBmodel *model, GRBmodel **fixedP);
 int __stdcall
   GRBfeasrelax(GRBmodel *model, int relaxobjtype, int minrelax,
                double *lbpen, double *ubpen, double *rhspen,
                double *feasobjP);
+int __stdcall
+  GRBsinglescenariomodel(GRBmodel *model, GRBmodel **singlescenarioP);
 
 /* Undocumented routines */
 
 int __stdcall
   GRBgetcbwhatinfo(void *cbdata, int what, int *typeP, int *sizeP);
-GRBmodel * __stdcall
-  GRBrelaxmodel(GRBmodel *model);
+int __stdcall
+  GRBrelaxmodel(GRBmodel *model, GRBmodel **relaxedP);
 int __stdcall
   GRBconverttofixed(GRBmodel *model);
+int __stdcall
+  GRBpresolvemodel(GRBmodel *model, GRBmodel **presolvedP);
+int __stdcall
+  GRBiismodel(GRBmodel *model, GRBmodel **iisP);
+int __stdcall
+  GRBfeasibility(GRBmodel *model, GRBmodel **feasP);
+int __stdcall
+  GRBlinearizemodel(GRBmodel *model, GRBmodel **linearizedP);
+int __stdcall
+  GRBresultmodel(GRBmodel *model, char *type, GRBmodel **resultP);
 GRBmodel * __stdcall
-  GRBpresolvemodel(GRBmodel *model);
-GRBmodel * __stdcall
-  GRBiismodel(GRBmodel *model);
-GRBmodel * __stdcall
-  GRBfeasibility(GRBmodel *model);
-GRBmodel * __stdcall
-  GRBlinearizemodel(GRBmodel *model);
+  GRBfixedmodel(GRBmodel *model);
+int __stdcall
+  GRBdualmodel(GRBmodel *model, GRBmodel **dualP);
 
 #define MALLOCCB_ARGS size_t size, void *syscbusrdata
 #define CALLOCCB_ARGS size_t nmemb, size_t size, void *syscbusrdata
 #define REALLOCCB_ARGS void *ptr, size_t size, void *syscbusrdata
 #define FREECB_ARGS void *ptr, void *syscbusrdata
 #define THREADCREATECB_ARGS void **threadP, void (*start_routine)(void *), void *arg, void *syscbusrdata
 #define THREADJOINCB_ARGS void *thread, void *syscbusrdata
@@ -629,27 +770,43 @@
                   void * (__stdcall *calloccb)(CALLOCCB_ARGS),
                   void * (__stdcall *realloccb)(REALLOCCB_ARGS),
                   void (__stdcall *freecb)(FREECB_ARGS),
                   int (__stdcall *threadcreatecb)(THREADCREATECB_ARGS),
                   void (__stdcall *threadjoincb)(THREADJOINCB_ARGS),
                   void *syscbusrdata);
 
+
+int __stdcall
+  GRBemptyenvadv(GRBenv **envP, int apitype, int major, int minor, int tech,
+                 void * (__stdcall *malloccb)(MALLOCCB_ARGS),
+                 void * (__stdcall *calloccb)(CALLOCCB_ARGS),
+                 void * (__stdcall *realloccb)(REALLOCCB_ARGS),
+                 void   (__stdcall *freecb)(FREECB_ARGS),
+                 int    (__stdcall *threadcreatecb)(THREADCREATECB_ARGS),
+                 void   (__stdcall *threadjoincb)(THREADJOINCB_ARGS),
+                 void              *syscbusrdata);
+
 int __stdcall
   GRBreadmodel(GRBenv *env, const char *filename, GRBmodel **modelP);
 int __stdcall
   GRBread(GRBmodel *model, const char *filename);
 int __stdcall
   GRBwrite(GRBmodel *model, const char *filename);
 int __stdcall
   GRBismodelfile(const char *filename);
 int __stdcall
+  GRBisattrfile(const char *filename);
+int __stdcall
   GRBfiletype(const char *filename);
 int __stdcall
- GRBisrecordfile(const char *filename);
-
+  GRBisrecordfile(const char *filename);
+int __stdcall
+  GRBgetjsonsolution(GRBmodel *model, char **buffP);
+int __stdcall
+  GRBloadjson(GRBenv *env, const char *fname, char **buffP);
 int __stdcall
   GRBnewmodel(GRBenv *env, GRBmodel **modelP, const char *Pname, int numvars,
               double *obj, double *lb, double *ub, char *vtype,
               char **varnames);
 
 int __stdcall
   GRBloadmodel(GRBenv *env, GRBmodel **modelP, const char *Pname,
@@ -722,18 +879,52 @@
 int __stdcall
   GRBaddgenconstrAnd(GRBmodel *model, const char *name,
                      int resvar, int nvars, const int *vars);
 int __stdcall
   GRBaddgenconstrOr(GRBmodel *model, const char *name,
                     int resvar, int nvars, const int *vars);
 int __stdcall
-  GRBaddgenconstrIndicator(GRBmodel *lp, const char *name,
+  GRBaddgenconstrNorm(GRBmodel *model, const char *name,
+                      int resvar, int nvars, const int *vars, double which);
+int __stdcall
+  GRBaddgenconstrIndicator(GRBmodel *model, const char *name,
                            int binvar, int binval, int nvars, const int *vars,
                            const double *vals, char sense, double rhs);
 int __stdcall
+  GRBaddgenconstrPWL(GRBmodel *model, const char *name,
+                     int xvar, int yvar, int npts,
+                     const double *xpts, const double *ypts);
+int __stdcall
+  GRBaddgenconstrPoly(GRBmodel *model, const char *name, int xvar, int yvar,
+                      int plen, const double *p, const char *options);
+int __stdcall
+  GRBaddgenconstrExpA(GRBmodel *model, const char *name, int xvar,
+                      int yvar, double a, const char *options);
+int __stdcall
+  GRBaddgenconstrLogA(GRBmodel *model, const char *name, int xvar,
+                      int yvar, double a, const char *options);
+int __stdcall
+  GRBaddgenconstrPow(GRBmodel *model, const char *name, int xvar,
+                     int yvar, double a, const char *options);
+int __stdcall
+  GRBaddgenconstrExp(GRBmodel *model, const char *name, int xvar,
+                     int yvar, const char *options);
+int __stdcall
+  GRBaddgenconstrLog(GRBmodel *model, const char *name, int xvar,
+                     int yvar, const char *options);
+int __stdcall
+  GRBaddgenconstrSin(GRBmodel *model, const char *name, int xvar,
+                     int yvar, const char *options);
+int __stdcall
+  GRBaddgenconstrCos(GRBmodel *model, const char *name, int xvar,
+                     int yvar, const char *options);
+int __stdcall
+  GRBaddgenconstrTan(GRBmodel *model, const char *name, int xvar,
+                     int yvar, const char *options);
+int __stdcall
   GRBaddqconstr(GRBmodel *model, int numlnz, int *lind, double *lval,
                 int numqnz, int *qrow, int *qcol, double *qval,
                 char sense, double rhs, const char *QCname);
 int __stdcall
   GRBaddcone(GRBmodel *model, int nummembers, int *members);
 int __stdcall
   GRBaddqpterms(GRBmodel *model, int numqnz, int *qrow, int *qcol,
@@ -773,15 +964,15 @@
 int __stdcall
   GRBcomputeIIS(GRBmodel *model);
 
 /* simplex advanced routines */
 
 typedef struct _GRBsvec
 {
-  int     len; /* sparse vector length */
+  int     len; /* sparse vector length. -1: It is a dense vector. */
   int    *ind; /* indices array of the sparse vector */
   double *val; /* value array of the sparse vector */
 } GRBsvec;
 
 int __stdcall
   GRBFSolve(GRBmodel *model, GRBsvec *b, GRBsvec *x);
 
@@ -802,15 +993,15 @@
 
 int __stdcall
   GRBgetBasisHead(GRBmodel *model, int *bhead);
 
 int __stdcall
   GRBcbstoponemultiobj(GRBmodel *model, void *cbdata, int objnum);
 
-/* Model status codes (after call to GRBoptimize()) */
+/* Model status codes */
 
 #define GRB_LOADED          1
 #define GRB_OPTIMAL         2
 #define GRB_INFEASIBLE      3
 #define GRB_INF_OR_UNBD     4
 #define GRB_UNBOUNDED       5
 #define GRB_CUTOFF          6
@@ -819,14 +1010,15 @@
 #define GRB_TIME_LIMIT      9
 #define GRB_SOLUTION_LIMIT 10
 #define GRB_INTERRUPTED    11
 #define GRB_NUMERIC        12
 #define GRB_SUBOPTIMAL     13
 #define GRB_INPROGRESS     14
 #define GRB_USER_OBJ_LIMIT 15
+#define GRB_WORK_LIMIT     16
 
 /* Basis status info */
 
 #define GRB_BASIC           0
 #define GRB_NONBASIC_LOWER -1
 #define GRB_NONBASIC_UPPER -2
 #define GRB_SUPERBASIC     -3
@@ -844,14 +1036,16 @@
 
 #define GRB_INT_PAR_BARITERLIMIT   "BarIterLimit"
 #define GRB_DBL_PAR_CUTOFF         "Cutoff"
 #define GRB_DBL_PAR_ITERATIONLIMIT "IterationLimit"
 #define GRB_DBL_PAR_NODELIMIT      "NodeLimit"
 #define GRB_INT_PAR_SOLUTIONLIMIT  "SolutionLimit"
 #define GRB_DBL_PAR_TIMELIMIT      "TimeLimit"
+#define GRB_DBL_PAR_WORKLIMIT      "WorkLimit"
+#define GRB_DBL_PAR_MEMLIMIT       "MemLimit"
 #define GRB_DBL_PAR_BESTOBJSTOP    "BestObjStop"
 #define GRB_DBL_PAR_BESTBDSTOP     "BestBdStop"
 
 /* Tolerances */
 
 #define GRB_DBL_PAR_FEASIBILITYTOL "FeasibilityTol"
 #define GRB_DBL_PAR_INTFEASTOL     "IntFeasTol"
@@ -868,48 +1062,54 @@
 #define GRB_DBL_PAR_OBJSCALE       "ObjScale"
 #define GRB_INT_PAR_SCALEFLAG      "ScaleFlag"
 #define GRB_INT_PAR_SIMPLEXPRICING "SimplexPricing"
 #define GRB_INT_PAR_QUAD           "Quad"
 #define GRB_INT_PAR_NORMADJUST     "NormAdjust"
 #define GRB_INT_PAR_SIFTING        "Sifting"
 #define GRB_INT_PAR_SIFTMETHOD     "SiftMethod"
+#define GRB_INT_PAR_LPWARMSTART    "LPWarmStart"
+#define GRB_INT_PAR_NETWORKALG     "NetworkAlg"
 
 /* Barrier */
 
 #define GRB_DBL_PAR_BARCONVTOL     "BarConvTol"
 #define GRB_INT_PAR_BARCORRECTORS  "BarCorrectors"
 #define GRB_INT_PAR_BARHOMOGENEOUS "BarHomogeneous"
 #define GRB_INT_PAR_BARORDER       "BarOrder"
 #define GRB_DBL_PAR_BARQCPCONVTOL  "BarQCPConvTol"
 #define GRB_INT_PAR_CROSSOVER      "Crossover"
 #define GRB_INT_PAR_CROSSOVERBASIS "CrossoverBasis"
 
 /* MIP */
 
-#define GRB_INT_PAR_BRANCHDIR         "BranchDir"
-#define GRB_INT_PAR_DEGENMOVES        "DegenMoves"
-#define GRB_INT_PAR_DISCONNECTED      "Disconnected"
-#define GRB_DBL_PAR_HEURISTICS        "Heuristics"
-#define GRB_DBL_PAR_IMPROVESTARTGAP   "ImproveStartGap"
-#define GRB_DBL_PAR_IMPROVESTARTTIME  "ImproveStartTime"
-#define GRB_DBL_PAR_IMPROVESTARTNODES "ImproveStartNodes"
-#define GRB_INT_PAR_MINRELNODES       "MinRelNodes"
-#define GRB_INT_PAR_MIPFOCUS          "MIPFocus"
-#define GRB_STR_PAR_NODEFILEDIR       "NodefileDir"
-#define GRB_DBL_PAR_NODEFILESTART     "NodefileStart"
-#define GRB_INT_PAR_NODEMETHOD        "NodeMethod"
-#define GRB_INT_PAR_NORELHEURISTIC    "NoRelHeuristic"
-#define GRB_INT_PAR_PUMPPASSES        "PumpPasses"
-#define GRB_INT_PAR_RINS              "RINS"
-#define GRB_INT_PAR_STARTNODELIMIT    "StartNodeLimit"
-#define GRB_INT_PAR_SUBMIPNODES       "SubMIPNodes"
-#define GRB_INT_PAR_SYMMETRY          "Symmetry"
-#define GRB_INT_PAR_VARBRANCH         "VarBranch"
-#define GRB_INT_PAR_SOLUTIONNUMBER    "SolutionNumber"
-#define GRB_INT_PAR_ZEROOBJNODES      "ZeroObjNodes"
+#define GRB_INT_PAR_BRANCHDIR          "BranchDir"
+#define GRB_INT_PAR_DEGENMOVES         "DegenMoves"
+#define GRB_INT_PAR_DISCONNECTED       "Disconnected"
+#define GRB_DBL_PAR_HEURISTICS         "Heuristics"
+#define GRB_DBL_PAR_IMPROVESTARTGAP    "ImproveStartGap"
+#define GRB_DBL_PAR_IMPROVESTARTTIME   "ImproveStartTime"
+#define GRB_DBL_PAR_IMPROVESTARTNODES  "ImproveStartNodes"
+#define GRB_INT_PAR_INTEGRALITYFOCUS   "IntegralityFocus"
+#define GRB_INT_PAR_MINRELNODES        "MinRelNodes"
+#define GRB_INT_PAR_MIPFOCUS           "MIPFocus"
+#define GRB_INT_PAR_NLPHEUR            "NLPHeur"
+#define GRB_STR_PAR_NODEFILEDIR        "NodefileDir"
+#define GRB_DBL_PAR_NODEFILESTART      "NodefileStart"
+#define GRB_INT_PAR_NODEMETHOD         "NodeMethod"
+#define GRB_DBL_PAR_NORELHEURTIME      "NoRelHeurTime"
+#define GRB_DBL_PAR_NORELHEURWORK      "NoRelHeurWork"
+#define GRB_INT_PAR_PUMPPASSES         "PumpPasses"
+#define GRB_INT_PAR_RINS               "RINS"
+#define GRB_STR_PAR_SOLFILES           "SolFiles"
+#define GRB_INT_PAR_STARTNODELIMIT     "StartNodeLimit"
+#define GRB_INT_PAR_SUBMIPNODES        "SubMIPNodes"
+#define GRB_INT_PAR_SYMMETRY           "Symmetry"
+#define GRB_INT_PAR_VARBRANCH          "VarBranch"
+#define GRB_INT_PAR_SOLUTIONNUMBER     "SolutionNumber"
+#define GRB_INT_PAR_ZEROOBJNODES       "ZeroObjNodes"
 
 /* MIP cuts */
 
 #define GRB_INT_PAR_CUTS            "Cuts"
 
 #define GRB_INT_PAR_CLIQUECUTS      "CliqueCuts"
 #define GRB_INT_PAR_COVERCUTS       "CoverCuts"
@@ -922,104 +1122,146 @@
 #define GRB_INT_PAR_MIRCUTS         "MIRCuts"
 #define GRB_INT_PAR_STRONGCGCUTS    "StrongCGCuts"
 #define GRB_INT_PAR_MODKCUTS        "ModKCuts"
 #define GRB_INT_PAR_ZEROHALFCUTS    "ZeroHalfCuts"
 #define GRB_INT_PAR_NETWORKCUTS     "NetworkCuts"
 #define GRB_INT_PAR_SUBMIPCUTS      "SubMIPCuts"
 #define GRB_INT_PAR_INFPROOFCUTS    "InfProofCuts"
+#define GRB_INT_PAR_RLTCUTS         "RLTCuts"
+#define GRB_INT_PAR_RELAXLIFTCUTS   "RelaxLiftCuts"
+#define GRB_INT_PAR_BQPCUTS         "BQPCuts"
+#define GRB_INT_PAR_PSDCUTS         "PSDCuts"
+#define GRB_INT_PAR_LIFTPROJECTCUTS "LiftProjectCuts"
 
 #define GRB_INT_PAR_CUTAGGPASSES    "CutAggPasses"
 #define GRB_INT_PAR_CUTPASSES       "CutPasses"
 #define GRB_INT_PAR_GOMORYPASSES    "GomoryPasses"
 
 /* Distributed algorithms */
 
 #define GRB_STR_PAR_WORKERPOOL      "WorkerPool"
 #define GRB_STR_PAR_WORKERPASSWORD  "WorkerPassword"
 
+/* Licensing and Compute Server */
+#define GRB_STR_PAR_COMPUTESERVER     "ComputeServer"
+#define GRB_STR_PAR_TOKENSERVER       "TokenServer"
+#define GRB_STR_PAR_SERVERPASSWORD    "ServerPassword"
+#define GRB_INT_PAR_SERVERTIMEOUT     "ServerTimeout"
+#define GRB_STR_PAR_CSROUTER          "CSRouter"
+#define GRB_STR_PAR_CSGROUP           "CSGroup"
+#define GRB_DBL_PAR_CSQUEUETIMEOUT    "CSQueueTimeout"
+#define GRB_INT_PAR_CSPRIORITY        "CSPriority"
+#define GRB_INT_PAR_CSIDLETIMEOUT     "CSIdleTimeout"
+#define GRB_INT_PAR_CSTLSINSECURE     "CSTLSInsecure"
+#define GRB_INT_PAR_TSPORT            "TSPort"
+#define GRB_STR_PAR_CLOUDACCESSID     "CloudAccessID"
+#define GRB_STR_PAR_CLOUDSECRETKEY    "CloudSecretKey"
+#define GRB_STR_PAR_CLOUDPOOL         "CloudPool"
+#define GRB_STR_PAR_CLOUDHOST         "CloudHost"
+#define GRB_STR_PAR_CSMANAGER         "CSManager"
+#define GRB_STR_PAR_CSAUTHTOKEN       "CSAuthToken"
+#define GRB_STR_PAR_CSAPIACCESSID     "CSAPIAccessID"
+#define GRB_STR_PAR_CSAPISECRET       "CSAPISecret"
+#define GRB_INT_PAR_CSBATCHMODE       "CSBatchMode"
+#define GRB_STR_PAR_USERNAME          "Username"
+#define GRB_STR_PAR_CSAPPNAME         "CSAppName"
+#define GRB_INT_PAR_CSCLIENTLOG       "CSClientLog"
+#define GRB_STR_PAR_WLSACCESSID       "WLSAccessID"
+#define GRB_STR_PAR_WLSSECRET         "WLSSecret"
+#define GRB_INT_PAR_WLSTOKENDURATION  "WLSTokenDuration"
+#define GRB_STR_PAR_WLSTOKEN          "WLSToken"
+#define GRB_INT_PAR_LICENSEID         "LicenseID"
+
+
 /* Other */
 
 #define GRB_INT_PAR_AGGREGATE         "Aggregate"
 #define GRB_INT_PAR_AGGFILL           "AggFill"
 #define GRB_INT_PAR_CONCURRENTMIP     "ConcurrentMIP"
 #define GRB_INT_PAR_CONCURRENTJOBS    "ConcurrentJobs"
 #define GRB_INT_PAR_DISPLAYINTERVAL   "DisplayInterval"
 #define GRB_INT_PAR_DISTRIBUTEDMIPJOBS "DistributedMIPJobs"
 #define GRB_INT_PAR_DUALREDUCTIONS    "DualReductions"
 #define GRB_DBL_PAR_FEASRELAXBIGM     "FeasRelaxBigM"
 #define GRB_INT_PAR_IISMETHOD         "IISMethod"
 #define GRB_INT_PAR_INFUNBDINFO       "InfUnbdInfo"
+#define GRB_INT_PAR_JSONSOLDETAIL     "JSONSolDetail"
 #define GRB_INT_PAR_LAZYCONSTRAINTS   "LazyConstraints"
 #define GRB_STR_PAR_LOGFILE           "LogFile"
 #define GRB_INT_PAR_LOGTOCONSOLE      "LogToConsole"
 #define GRB_INT_PAR_MIQCPMETHOD       "MIQCPMethod"
+#define GRB_INT_PAR_NONCONVEX         "NonConvex"
 #define GRB_INT_PAR_NUMERICFOCUS      "NumericFocus"
 #define GRB_INT_PAR_OUTPUTFLAG        "OutputFlag"
 #define GRB_INT_PAR_PRECRUSH          "PreCrush"
 #define GRB_INT_PAR_PREDEPROW         "PreDepRow"
 #define GRB_INT_PAR_PREDUAL           "PreDual"
 #define GRB_INT_PAR_PREPASSES         "PrePasses"
 #define GRB_INT_PAR_PREQLINEARIZE     "PreQLinearize"
 #define GRB_INT_PAR_PRESOLVE          "Presolve"
 #define GRB_DBL_PAR_PRESOS1BIGM       "PreSOS1BigM"
 #define GRB_DBL_PAR_PRESOS2BIGM       "PreSOS2BigM"
+#define GRB_INT_PAR_PRESOS1ENCODING   "PreSOS1Encoding"
+#define GRB_INT_PAR_PRESOS2ENCODING   "PreSOS2Encoding"
 #define GRB_INT_PAR_PRESPARSIFY       "PreSparsify"
 #define GRB_INT_PAR_PREMIQCPFORM      "PreMIQCPForm"
 #define GRB_INT_PAR_QCPDUAL           "QCPDual"
 #define GRB_INT_PAR_RECORD            "Record"
 #define GRB_STR_PAR_RESULTFILE        "ResultFile"
 #define GRB_INT_PAR_SEED              "Seed"
 #define GRB_INT_PAR_THREADS           "Threads"
 #define GRB_DBL_PAR_TUNETIMELIMIT     "TuneTimeLimit"
 #define GRB_INT_PAR_TUNERESULTS       "TuneResults"
 #define GRB_INT_PAR_TUNECRITERION     "TuneCriterion"
 #define GRB_INT_PAR_TUNETRIALS        "TuneTrials"
 #define GRB_INT_PAR_TUNEOUTPUT        "TuneOutput"
 #define GRB_INT_PAR_TUNEJOBS          "TuneJobs"
+#define GRB_DBL_PAR_TUNECLEANUP       "TuneCleanup"
+#define GRB_DBL_PAR_TUNETARGETMIPGAP  "TuneTargetMIPGap"
+#define GRB_DBL_PAR_TUNETARGETTIME    "TuneTargetTime"
+#define GRB_INT_PAR_TUNEMETRIC        "TuneMetric"
 #define GRB_INT_PAR_UPDATEMODE        "UpdateMode"
 #define GRB_INT_PAR_OBJNUMBER         "ObjNumber"
 #define GRB_INT_PAR_MULTIOBJMETHOD    "MultiObjMethod"
 #define GRB_INT_PAR_MULTIOBJPRE       "MultiObjPre"
+#define GRB_INT_PAR_SCENARIONUMBER    "ScenarioNumber"
 #define GRB_INT_PAR_POOLSOLUTIONS     "PoolSolutions"
 #define GRB_DBL_PAR_POOLGAP           "PoolGap"
+#define GRB_DBL_PAR_POOLGAPABS        "PoolGapAbs"
 #define GRB_INT_PAR_POOLSEARCHMODE    "PoolSearchMode"
 #define GRB_INT_PAR_IGNORENAMES       "IgnoreNames"
 #define GRB_INT_PAR_STARTNUMBER       "StartNumber"
 #define GRB_INT_PAR_PARTITIONPLACE    "PartitionPlace"
-#define GRB_STR_PAR_COMPUTESERVER     "ComputeServer"
-#define GRB_STR_PAR_TOKENSERVER       "TokenServer"
-#define GRB_STR_PAR_SERVERPASSWORD    "ServerPassword"
-#define GRB_INT_PAR_SERVERTIMEOUT     "ServerTimeout"
-#define GRB_STR_PAR_CSROUTER          "CSRouter"
-#define GRB_STR_PAR_CSGROUP           "CSGroup"
-#define GRB_DBL_PAR_CSQUEUETIMEOUT    "CSQueueTimeout"
-#define GRB_INT_PAR_CSPRIORITY        "CSPriority"
-#define GRB_INT_PAR_CSIDLETIMEOUT     "CSIdleTimeout"
-#define GRB_INT_PAR_CSTLSINSECURE     "TLSInsecure"
-#define GRB_INT_PAR_TSPORT            "TSPort"
-#define GRB_STR_PAR_CLOUDACCESSID     "CloudAccessID"
-#define GRB_STR_PAR_CLOUDSECRETKEY    "CloudSecretKey"
-#define GRB_STR_PAR_CLOUDPOOL         "CloudPool"
-#define GRB_STR_PAR_CLOUDHOST         "CloudHost"
+#define GRB_INT_PAR_FUNCPIECES        "FuncPieces"
+#define GRB_DBL_PAR_FUNCPIECELENGTH   "FuncPieceLength"
+#define GRB_DBL_PAR_FUNCPIECEERROR    "FuncPieceError"
+#define GRB_DBL_PAR_FUNCPIECERATIO    "FuncPieceRatio"
+#define GRB_DBL_PAR_FUNCMAXVAL        "FuncMaxVal"
 #define GRB_STR_PAR_DUMMY             "Dummy"
 
+/* Deprecated */
+
+#define GRB_STR_PAR_JOBID             "JobID"
+
+
 /* Parameter enumerations */
 
 /* All *CUTS parameters */
 #define GRB_CUTS_AUTO          -1
 #define GRB_CUTS_OFF            0
 #define GRB_CUTS_CONSERVATIVE   1
 #define GRB_CUTS_AGGRESSIVE     2
 #define GRB_CUTS_VERYAGGRESSIVE 3
 
 #define GRB_PRESOLVE_AUTO        -1
 #define GRB_PRESOLVE_OFF          0
 #define GRB_PRESOLVE_CONSERVATIVE 1
 #define GRB_PRESOLVE_AGGRESSIVE   2
 
+#define GRB_METHOD_NONE                            -1
 #define GRB_METHOD_AUTO                            -1
 #define GRB_METHOD_PRIMAL                           0
 #define GRB_METHOD_DUAL                             1
 #define GRB_METHOD_BARRIER                          2
 #define GRB_METHOD_CONCURRENT                       3
 #define GRB_METHOD_DETERMINISTIC_CONCURRENT         4
 #define GRB_METHOD_DETERMINISTIC_CONCURRENT_SIMPLEX 5
@@ -1051,20 +1293,26 @@
 
 #define GRB_PARTITION_EARLY     16
 #define GRB_PARTITION_ROOTSTART 8
 #define GRB_PARTITION_ROOTEND   4
 #define GRB_PARTITION_NODES     2
 #define GRB_PARTITION_CLEANUP   1
 
+#define GRB_PHASE_MIP_NOREL   0
+#define GRB_PHASE_MIP_SEARCH  1
+#define GRB_PHASE_MIP_IMPROVE 2
+
 int __stdcall
   GRBcheckmodel(GRBmodel *model);
 void __stdcall
   GRBsetsignal(GRBmodel *model);
 void __stdcall
   GRBterminate(GRBmodel *model);
+void __stdcall
+  GRBcbproceed(GRBmodel *model);
 int __stdcall
   GRBreplay(const char *filename);
 int __stdcall
   GRBsetobjective(GRBmodel *model, int sense, double constant,
                   int lnz, int *lind, double *lval,
                   int qnz, int *qrow, int *qcol, double *qval);
 int __stdcall
@@ -1083,36 +1331,41 @@
 
 
 /* The following four routines are deprecated in Gurobi 2.0.
    Use the 'LogFile' parameter to control logging instead. */
 
 int __stdcall
   GRBgetlogfile(GRBenv *env, FILE **logfileP);
-int __stdcall
-  GRBsetlogfile(GRBenv *env, FILE *logfile);
 
 
 /* Parameter routines */
 
 int __stdcall
+  GRBfixtuneparam(GRBenv *env, const char *paramname);
+int __stdcall
   GRBgetintparam(GRBenv *env, const char *paramname, int *valueP);
 int __stdcall
   GRBgetdblparam(GRBenv *env, const char *paramname, double *valueP);
 int __stdcall
   GRBgetstrparam(GRBenv *env, const char *paramname, char *valueP);
 int __stdcall
+  GRBgetlongstrparam(GRBenv *env, const char *paramname, char *valueP,
+                     int size, int *requiredlenP);
+int __stdcall
   GRBgetintparaminfo(GRBenv *env, const char *paramname, int *valueP,
                      int *minP, int *maxP, int *defP);
 int __stdcall
   GRBgetdblparaminfo(GRBenv *env, const char *paramname, double *valueP,
                      double *minP, double *maxP, double *defP);
 int __stdcall
   GRBgetstrparaminfo(GRBenv *env, const char *paramname, char *valueP,
                      char *defP);
 int __stdcall
+  GRBgetparamflags(GRBenv *env, const char *parname, unsigned int *valueP);
+int __stdcall
   GRBsetparam(GRBenv *env, const char *paramname, const char *value);
 int __stdcall
   GRBsetintparam(GRBenv *env, const char *paramname, int value);
 int __stdcall
   GRBsetdblparam(GRBenv *env, const char *paramname, double value);
 int __stdcall
   GRBsetstrparam(GRBenv *env, const char *paramname, const char *value);
@@ -1138,50 +1391,42 @@
 /* Environment routines */
 
 int __stdcall
   GRBloadenv(GRBenv **envP, const char *logfilename);
 int __stdcall
   GRBemptyenv(GRBenv **envP);
 int __stdcall
-  GRBemptyenvadv(GRBenv **envP, int apitype, int major, int minor, int tech);
-int __stdcall
   GRBstartenv(GRBenv *env);
 int __stdcall
   GRBloadenvadv(GRBenv **envP, const char *logfilename,
                 int apitype, int major, int minor, int tech,
                 const char *server, const char *router,
                 const char *password, const char *group,
                 int priority, int idletimeout,
                 const char *accessid, const char *secretkey,
-                int (__stdcall *cb)(CB_ARGS), void *usrdata);
-int __stdcall
-  GRBloadenvadv2(GRBenv **envP, const char *logfilename,
-                 int apitype, int major, int minor, int tech,
-                 const char *server, const char *router,
-                 const char *password, const char *group,
-                 int priority, int idletimeout,
-                 const char *accessid, const char *secretkey,
-                 int (__stdcall *cb)(CB_ARGS), void *usrdata,
-                 int (__stdcall *logcb)(char *msg));
+                int (__stdcall *cb)(CB_ARGS), void *usrdata,
+                int (__stdcall *logcb)(LOGCB_ARGS), void *logdata);
+GRB_DEPRECATED("Replaced by GRBemptyenv() and parameter settings",
 int __stdcall
   GRBloadclientenv(GRBenv **envP, const char *logfilename,
                    const char *computeserver, const char *router,
-                   const char *password, const char *group, int tls_insecure,
-                   int priority, double timeout);
+                   const char *password, const char *group, int CStlsinsecure,
+                   int priority, double timeout));
 int __stdcall
   GRBloadclientenvadv(GRBenv **envP, const char *logfilename,
                       const char *computeserver, const char *router,
-                      const char *password, const char *group, int tls_insecure,
+                      const char *password, const char *group, int CStlsinsecure,
                       int priority, double timeout, int apitype,
                       int major, int minor, int tech,
                       int (__stdcall *cb)(CB_ARGS), void *usrdata);
+GRB_DEPRECATED("Replaced by GRBemptyenv() and parameter settings",
 int __stdcall
   GRBloadcloudenv(GRBenv **envP, const char *logfilename,
                   const char *accessID, const char *secretKey,
-                  const char *pool, int priority);
+                  const char *pool, int priority));
 int __stdcall
   GRBloadcloudenvadv(GRBenv **envP, const char *logfilename,
                      const char *accessID, const char *secretKey,
                      const char *pool, int priority, int apitype, int major,
                      int minor, int tech,
                      int (__stdcall *cb)(CB_ARGS), void *usrdata);
 GRBenv *__stdcall
@@ -1190,53 +1435,118 @@
   GRBgetconcurrentenv(GRBmodel *model, int num);
 void __stdcall
   GRBdiscardconcurrentenvs(GRBmodel *model);
 GRBenv *__stdcall
   GRBgetmultiobjenv(GRBmodel *model, int num);
 void __stdcall
   GRBdiscardmultiobjenvs(GRBmodel *model);
+GRBenv *__stdcall
+  GRBgettuneenv(GRBenv *env, int num);
+void __stdcall
+  GRBdiscardtuneenvs(GRBenv *env);
 void __stdcall
   GRBreleaselicense(GRBenv *env);
 void __stdcall
   GRBfreeenv(GRBenv *env);
 const char * __stdcall
   GRBgeterrormsg(GRBenv *env);
 const char * __stdcall
   GRBgetmerrormsg(GRBmodel *model);
+void __stdcall
+  GRBgetcommstats(GRBenv *env, double *recvtimeP, double *recvbytesP,
+                  double *recvmsgsP, double *sendtimeP,
+                  double *sendbytesP, double *sendmsgsP);
 
 /* Version info */
 
 void __stdcall
   GRBversion(int *majorP, int *minorP, int *technicalP);
 
 char * __stdcall
   GRBplatform(void);
 
+char * __stdcall
+  GRBplatformext(void);
+
 int __stdcall
   GRBlisttokens(void);
 
 /* Tuning */
 
+void __stdcall
+  GRBprinttuneparams(void);
 int __stdcall
   GRBtunemodel(GRBmodel *model);
 int __stdcall
-  GRBtunemodels(int nummodels, GRBmodel **models,
-                GRBmodel *ignore, GRBmodel *hint);
+  GRBtunemodels(GRBenv *env, int nummodels, GRBmodel **models);
 int __stdcall
   GRBgettuneresult(GRBmodel *model, int i);
 int __stdcall
   GRBgettunelog(GRBmodel *model, int i, char **logP);
+
+/* Used in Matlab API */
+void __stdcall
+  GRBsortIDi(int len, int *ind, double *val);
+
+/* batch-related routines */
+int __stdcall
+  GRBabortbatch(GRBbatch *batch);
+int __stdcall
+  GRBdiscardbatch(GRBbatch *batch);
+int __stdcall
+  GRBretrybatch(GRBbatch *batch);
+int __stdcall
+  GRBfreebatch(GRBbatch *batch);
+int __stdcall
+  GRBgetbatch(GRBenv *env, const char *batchID, GRBbatch **batchP);
 int __stdcall
-  GRBtunemodeladv(GRBmodel *model, GRBmodel *ignore, GRBmodel *hint);
+  GRBgetbatchjsonsolution(GRBbatch *batch, char **jsonsolP);
+int __stdcall
+  GRBgetbatchintattr(GRBbatch *batch, const char *attrname, int *valueP);
+int __stdcall
+  GRBgetbatchstrattr(GRBbatch *batch, const char *attrname, char **valueP);
+int __stdcall
+  GRBgetbatchattrname(GRBenv *env, int n, char **attrnameP);
+int __stdcall
+  GRBgetbatchattrflags(GRBbatch *batch, const char *attrname, unsigned *flagsP);
+int __stdcall GRBgetbatchattrinfo(GRBbatch *batch, const char *attrname, int *datatypeP, int *settableP);
+int __stdcall
+  GRBupdatebatch(GRBbatch *batch);
+int __stdcall
+  GRBwritebatchjsonsolution(GRBbatch *batch, const char *filename);
+int __stdcall
+  GRBgetnumbatchattributes(GRBenv *env);
+GRBenv *__stdcall
+  GRBgetbatchenv(GRBbatch *batch);
+
+/* dummy wrapper for free function */
+void __stdcall
+  GRBfree(void *ptr);
+/* Batch object status codes */
+
+#define GRB_BATCH_STATUS_UNKNOWN 0
+#define GRB_BATCH_CREATED        1
+#define GRB_BATCH_SUBMITTED      2
+#define GRB_BATCH_ABORTED        3
+#define GRB_BATCH_FAILED         4
+#define GRB_BATCH_COMPLETED      5
+
+
 /* Async interface */
 
 int __stdcall
   GRBsync(GRBmodel *model);
 
 int __stdcall
   GRBpingserver(const char *server, const char *password);
+
+
+/* pre-fetching attributes from Compute Server */
+
+int __stdcall
+  GRBprefetchattr(GRBmodel *model, const char *attrname);
  
 #ifdef __cplusplus
 }
 #endif
  
 #endif
```

### Comparing `ilpy-0.2.3/ilpy/impl/solvers/CplexBackend.cpp` & `ilpy-0.3.0/ilpy/impl/solvers/CplexBackend.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 #ifdef HAVE_CPLEX
 
 #include <string>
 #include <vector>
 
 #include <ilcplex/ilocplex.h>
 
-#include "LinearConstraints.h"
-#include "QuadraticObjective.h"
-#include "QuadraticSolverBackend.h"
+#include "Constraints.h"
+#include "Objective.h"
+#include "SolverBackend.h"
 #include "Sense.h"
 #include "Solution.h"
 #include "CplexBackend.h"
 
 CplexBackend::CplexBackend(const Parameter& parameter) :
     _parameter(parameter),
     model_(env_),
@@ -67,21 +67,21 @@
 
 //        char t = (type == Binary ? 'B' : (type == Integer ? 'I' : 'C'));
 //        _variables[v].set(GRB_CharAttr_VType, t);
 //    }
 }
 
 void
-CplexBackend::setObjective(const LinearObjective& objective) {
+CplexBackend::setObjective(const Objective& objective) {
 
-    setObjective((QuadraticObjective)objective);
+    setObjective((Objective)objective);
 }
 
 void
-CplexBackend::setObjective(const QuadraticObjective& objective) {
+CplexBackend::setObjective(const Objective& objective) {
     try {
 
 
        if(!firstRun_){
         model_.remove(obj_);
        }
 
@@ -123,27 +123,27 @@
 
     } catch (IloCplex::Exception e) {
 
     }
 }
 
 void
-CplexBackend::setConstraints(const LinearConstraints& constraints) {
+CplexBackend::setConstraints(const Constraints& constraints) {
 
     // remove previous constraints
     for (ConstraintVector::iterator constraint = _constraints.begin(); constraint != _constraints.end(); constraint++)
         model_.remove(*constraint);
     _constraints.clear();
 
     // allocate memory for new constraints
     _constraints.reserve(constraints.size());
 
     try {
         IloExtractableArray cplex_constraints(env_);
-        for (LinearConstraints::const_iterator constraint = constraints.begin(); constraint != constraints.end(); constraint++) {
+        for (Constraints::const_iterator constraint = constraints.begin(); constraint != constraints.end(); constraint++) {
             IloRange linearConstraint = createConstraint(*constraint);
             _constraints.push_back(linearConstraint);
             cplex_constraints.add(linearConstraint);
         }
 
         // add all constraints as batch to the model
         model_.add(cplex_constraints);
@@ -151,28 +151,28 @@
     } catch (IloCplex::Exception e) {
 
 		std::cerr << "error: " << e.getMessage() << std::endl;
     }
 }
 
 void
-CplexBackend::addConstraint(const LinearConstraint& constraint) {
+CplexBackend::addConstraint(const Constraint& constraint) {
 
     try {
 		// add to the model
         _constraints.push_back(model_.add(createConstraint(constraint)));
 
     } catch (IloCplex::Exception e) {
 
 		std::cerr << "error: " << e.getMessage() << std::endl;
     }
 }
 
 IloRange
-CplexBackend::createConstraint(const LinearConstraint& constraint) {
+CplexBackend::createConstraint(const Constraint& constraint) {
 
 
     // create the lhs expression
     IloExpr linearExpr(env_);
 
     // set the coefficients
     typedef std::map<unsigned int, double>::const_iterator CoefIt;
```

### Comparing `ilpy-0.2.3/ilpy/impl/solvers/CplexBackend.h` & `ilpy-0.3.0/ilpy/impl/solvers/CplexBackend.h`

 * *Files 10% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 
 #include <string>
 #include <vector>
 
 #include <ilcplex/ilocplex.h>
 
-#include "LinearConstraints.h"
-#include "QuadraticObjective.h"
-#include "QuadraticSolverBackend.h"
+#include "Constraints.h"
+#include "Objective.h"
+#include "SolverBackend.h"
 #include "Sense.h"
 #include "Solution.h"
 
 
 
 /**
  * Cplex interface to solve the following (integer) quadratic program:
@@ -27,15 +27,15 @@
  *      optionally: x_i \in {0,1} for all i
  *
  * Where (A,b) describes all linear equality constraints, (C,d) all linear
  * inequality constraints and x is the solution vector. a is a real-valued
  * vector denoting the coefficients of the objective and Q a PSD matrix giving
  * the quadratic coefficients of the objective.
  */
-class CplexBackend : public QuadraticSolverBackend {
+class CplexBackend : public SolverBackend {
 
 public:
 
     struct Parameter {
 
         Parameter() :
             mipGap(0.0001),
@@ -73,21 +73,19 @@
             VariableType variableType);
 
     void initialize(
             unsigned int                                numVariables,
             VariableType                                defaultVariableType,
             const std::map<unsigned int, VariableType>& specialVariableTypes);
 
-    void setObjective(const LinearObjective& objective);
+    void setObjective(const Objective& objective);
 
-    void setObjective(const QuadraticObjective& objective);
+    void setConstraints(const Constraints& constraints);
 
-    void setConstraints(const LinearConstraints& constraints);
-
-    void addConstraint(const LinearConstraint& constraint);
+    void addConstraint(const Constraint& constraint);
 
     void setTimeout(double timeout) { timeout_ = timeout; }
 
     void setOptimalityGap(double gap, bool absolute=false) {
 
         _parameter.mipGap = gap;
         _parameter.absoluteGap = absolute;
@@ -113,15 +111,15 @@
     // set the optimality gap
     void setMIPGap(double gap, bool absolute);
 
     // set the mpi focus
     void setMIPFocus(unsigned int focus);
 
     // create a CPLEX constraint from a linear constraint
-    IloRange createConstraint(const LinearConstraint &constraint);
+    IloRange createConstraint(const Constraint &constraint);
 
     /**
      * Enable solver output.
      */
     void setVerbose(bool verbose);
 
     // size of a and x
```

### Comparing `ilpy-0.2.3/ilpy/impl/solvers/GurobiBackend.cpp` & `ilpy-0.3.0/ilpy/impl/solvers/GurobiBackend.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -88,21 +88,15 @@
 	GRB_CHECK(GRBupdatemodel(_model));
 
 	delete[] vtypes;
 	delete[] lbs;
 }
 
 void
-GurobiBackend::setObjective(const LinearObjective& objective) {
-
-	setObjective((QuadraticObjective)objective);
-}
-
-void
-GurobiBackend::setObjective(const QuadraticObjective& objective) {
+GurobiBackend::setObjective(const Objective& objective) {
 
 	// set sense of objective
 	if (objective.getSense() == Minimize) {
 		GRB_CHECK(GRBsetintattr(_model, GRB_INT_ATTR_MODELSENSE, +1));
 	} else {
 		GRB_CHECK(GRBsetintattr(_model, GRB_INT_ATTR_MODELSENSE, -1));
 	}
@@ -134,15 +128,15 @@
 		}
 	}
 
 	GRB_CHECK(GRBupdatemodel(_model));
 }
 
 void
-GurobiBackend::setConstraints(const LinearConstraints& constraints) {
+GurobiBackend::setConstraints(const Constraints& constraints) {
 
 	// delete all previous constraints
 
 	if (_numConstraints > 0) {
 
 		int* constraintIndicies = new int[_numConstraints];
 		for (unsigned int i = 0; i < _numConstraints; i++)
@@ -150,76 +144,109 @@
 		GRB_CHECK(GRBdelconstrs(_model, _numConstraints, constraintIndicies));
 
 		GRB_CHECK(GRBupdatemodel(_model));
 	}
 
 	_numConstraints = constraints.size();
 	unsigned int j = 0;
-	for (const LinearConstraint& constraint : constraints) {
+	for (const Constraint& constraint : constraints) {
 
 		addConstraint(constraint);
 
 		j++;
 	}
 
 	GRB_CHECK(GRBupdatemodel(_model));
 }
 
 void
-GurobiBackend::addConstraint(const LinearConstraint& constraint) {
+GurobiBackend::addConstraint(const Constraint& constraint) {
 
-	int numNz = constraint.getCoefficients().size();
+	// set the linear coefficients
+	int numlNz = constraint.getCoefficients().size();
 
-	int*    inds = new int[numNz];
-	double* vals = new double[numNz];
+	int*    linds = new int[numlNz];
+	double* lvals = new double[numlNz];
 
-	// set the coefficients
 	int i = 0;
 	for (auto& pair : constraint.getCoefficients()) {
 
-		inds[i] = pair.first;
-		vals[i] = pair.second;
+		linds[i] = pair.first;
+		lvals[i] = pair.second;
 		i++;
 	}
 
-	GRB_CHECK(GRBaddconstr(
+	// set the quadratic coefficients
+	int numqNz = constraint.getQuadraticCoefficients().size();
+
+	int*    qrows = new int[numqNz];
+	int*    qcols = new int[numqNz];
+	double* qvals = new double[numqNz];
+
+	int qi = 0;
+	for (auto& pair : constraint.getQuadraticCoefficients()) {
+
+		qrows[qi] = pair.first.first;
+		qcols[qi] = pair.first.second;
+		qvals[qi] = pair.second;
+		qi++;
+	}
+
+	GRB_CHECK(GRBaddqconstr(
 			_model,
-			numNz,
-			inds,
-			vals,
+			numlNz,
+			linds,
+			lvals,
+			numqNz,
+			qrows,
+			qcols,
+			qvals,
 			(constraint.getRelation() == LessEqual ? GRB_LESS_EQUAL :
 					(constraint.getRelation() == GreaterEqual ? GRB_GREATER_EQUAL :
 							GRB_EQUAL)),
 			constraint.getValue(),
 			NULL /* optional name */));
 
-	delete[] inds;
-	delete[] vals;
+	delete[] linds;
+	delete[] lvals;
+	delete[] qrows;
+	delete[] qcols;
+	delete[] qvals;
 }
 
 bool
 GurobiBackend::solve(Solution& x, std::string& msg) {
 
 	GRB_CHECK(GRBupdatemodel(_model));
 
+	GRBenv* modelenv = GRBgetenv(_model);
+
 	if (_timeout > 0) {
 
-		GRBenv* modelenv = GRBgetenv(_model);
 		GRB_CHECK(GRBsetdblparam(modelenv, GRB_DBL_PAR_TIMELIMIT, _timeout));
 	}
 
 	if (_gap >= 0) {
 
-		GRBenv* modelenv = GRBgetenv(_model);
 		if (_absoluteGap)
 			GRB_CHECK(GRBsetdblparam(modelenv, GRB_DBL_PAR_MIPGAPABS, _gap));
 		else
 			GRB_CHECK(GRBsetdblparam(modelenv, GRB_DBL_PAR_MIPGAP, _gap));
 	}
 
+	// Sets the strategy for handling non-convex quadratic objectives
+	// or non-convex quadratic constraints. 
+	// 0 = an error is reported if the original user model contains non-convex
+	//     quadratic constructs.
+	// 1 = an error is reported if non-convex quadratic constructs could not be
+	//     discarded or linearized during presolve.
+	// 2 = non-convex quadratic problems are solved by means of translating them
+	//     into bilinear form and applying spatial branching.
+	GRB_CHECK(GRBsetintparam(modelenv, GRB_INT_PAR_NONCONVEX, 2));
+
 	GRB_CHECK(GRBoptimize(_model));
 
 	int status;
 	GRB_CHECK(GRBgetintattr(_model, GRB_INT_ATTR_STATUS, &status));
 
 	if (status != GRB_OPTIMAL) {
```

### Comparing `ilpy-0.2.3/ilpy/impl/solvers/GurobiBackend.h` & `ilpy-0.3.0/ilpy/impl/solvers/GurobiBackend.h`

 * *Files 23% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 #include <string>
 
 extern "C" {
 #include <gurobi_c.h>
 }
 
-#include "LinearConstraints.h"
-#include "QuadraticObjective.h"
-#include "QuadraticSolverBackend.h"
+#include "Constraints.h"
+#include "Objective.h"
+#include "SolverBackend.h"
 #include "Sense.h"
 #include "Solution.h"
 
 /**
  * Gurobi interface to solve the following (integer) quadratic program:
  *
  * min  <a,x> + xQx
@@ -24,15 +24,15 @@
  *      optionally: x_i \in {0,1} for all i
  *
  * Where (A,b) describes all linear equality constraints, (C,d) all linear
  * inequality constraints and x is the solution vector. a is a real-valued
  * vector denoting the coefficients of the objective and Q a PSD matrix giving
  * the quadratic coefficients of the objective.
  */
-class GurobiBackend : public QuadraticSolverBackend {
+class GurobiBackend : public SolverBackend {
 
 public:
 
 	GurobiBackend();
 
 	virtual ~GurobiBackend();
 
@@ -45,21 +45,19 @@
 			VariableType variableType);
 
 	void initialize(
 			unsigned int                                numVariables,
 			VariableType                                defaultVariableType,
 			const std::map<unsigned int, VariableType>& specialVariableTypes);
 
-	void setObjective(const LinearObjective& objective);
+	void setObjective(const Objective& objective);
 
-	void setObjective(const QuadraticObjective& objective);
+	void setConstraints(const Constraints& constraints);
 
-	void setConstraints(const LinearConstraints& constraints);
-
-	void addConstraint(const LinearConstraint& constraint);
+	void addConstraint(const Constraint& constraint);
 
 	void setTimeout(double timeout) { _timeout = timeout; }
 
 	void setOptimalityGap(double gap, bool absolute=false) {
 
 		_gap = gap;
 		_absoluteGap = absolute;
```

### Comparing `ilpy-0.2.3/ilpy/impl/solvers/LinearConstraint.cpp` & `ilpy-0.3.0/ilpy/impl/solvers/Constraint.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,45 @@
-#include "LinearConstraint.h"
+#include "Constraint.h"
 
-LinearConstraint::LinearConstraint() :
+Constraint::Constraint() :
 	_relation(LessEqual) {}
 
 void
-LinearConstraint::setCoefficient(unsigned int varNum, double coef) {
+Constraint::setCoefficient(unsigned int varNum, double coef) {
 
 	if (coef == 0) {
 
-		std::map<unsigned int, double>::iterator i = _coefs.find(varNum);
-		if (i != _coefs.end())
-			_coefs.erase(_coefs.find(varNum));
+		_coefs.erase(varNum);
 
 	} else {
 
 		_coefs[varNum] = coef;
 	}
 }
 
 void
-LinearConstraint::setRelation(Relation relation) {
+Constraint::setQuadraticCoefficient(unsigned int varNum1, unsigned int varNum2, double coef) {
+
+	if (coef == 0) {
+
+		_quadraticCoefs.erase(std::make_pair(varNum1, varNum2));
+
+	} else {
+
+		_quadraticCoefs[std::make_pair(varNum1, varNum2)] = coef;
+	}
+}
+
+void
+Constraint::setRelation(Relation relation) {
 
 	_relation = relation;
 }
 
-bool LinearConstraint::isViolated(const Solution & solution){
+bool Constraint::isViolated(const Solution & solution){
 
     double s = 0;
 
     for(const auto & kv : _coefs){
         const auto var = kv.first;
         const auto coef = kv.second;
         const auto sol = solution[var];
@@ -43,42 +54,52 @@
     else{
         return s != _value;
     }
 }
 
 
 void
-LinearConstraint::setValue(double value) {
+Constraint::setValue(double value) {
 
 	_value = value;
 }
 
 const std::map<unsigned int, double>&
-LinearConstraint::getCoefficients() const {
+Constraint::getCoefficients() const {
 
 	return _coefs;
 }
 
+const std::map<std::pair<unsigned int, unsigned int>, double>&
+Constraint::getQuadraticCoefficients() const {
+
+	return _quadraticCoefs;
+}
+
 const Relation&
-LinearConstraint::getRelation() const {
+Constraint::getRelation() const {
 
 	return _relation;
 }
 
 double
-LinearConstraint::getValue() const {
+Constraint::getValue() const {
 
 	return _value;
 }
 
-std::ostream& operator<<(std::ostream& out, const LinearConstraint& constraint) {
+std::ostream& operator<<(std::ostream& out, const Constraint& constraint) {
 
 	typedef std::map<unsigned int, double>::value_type pair_t;
 	for (const pair_t& pair : constraint.getCoefficients())
 		out << pair.second << "*" << pair.first << " ";
 
+	typedef std::map<std::pair<unsigned int, unsigned int>, double>::value_type pair2_t;
+	for (pair2_t p : constraint.getQuadraticCoefficients())
+		out << p.second << "*" << p.first.first << "*" << p.first.second << " ";
+
 	out << (constraint.getRelation() == LessEqual ? "<=" : (constraint.getRelation() == GreaterEqual ? ">=" : "=="));
 
 	out << " " << constraint.getValue();
 
 	return out;
 }
```

### Comparing `ilpy-0.2.3/ilpy/impl/solvers/LinearConstraints.h` & `ilpy-0.3.0/ilpy/impl/solvers/Constraints.h`

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,73 @@
-#ifndef INFERENCE_LINEAR_CONSTRAINTS_H__
-#define INFERENCE_LINEAR_CONSTRAINTS_H__
+#ifndef INFERENCE_CONSTRAINTS_H__
+#define INFERENCE_CONSTRAINTS_H__
 
-#include "LinearConstraint.h"
+#include "Constraint.h"
 
-class LinearConstraints {
+class Constraints {
 
-	typedef std::vector<LinearConstraint> linear_constraints_type;
+	typedef std::vector<Constraint> constraints_type;
 
 public:
 
-	typedef linear_constraints_type::iterator       iterator;
+	typedef constraints_type::iterator       iterator;
 
-	typedef linear_constraints_type::const_iterator const_iterator;
+	typedef constraints_type::const_iterator const_iterator;
 
 	/**
-	 * Create a new set of linear constraints and allocate enough memory to hold
-	 * 'size' linear constraints. More or less constraints can be added, but
+	 * Create a new set of constraints and allocate enough memory to hold
+	 * 'size' constraints. More or less constraints can be added, but
 	 * memory might be wasted (if more allocated then necessary) or unnecessary
 	 * reallocations might occur (if more added than allocated).
 	 *
-	 * @param size The number of linear constraints to reserve memory for.
+	 * @param size The number of constraints to reserve memory for.
 	 */
-	LinearConstraints(size_t size = 0);
+	Constraints(size_t size = 0);
 
 	/**
-	 * Remove all constraints from this set of linear constraints.
+	 * Remove all constraints from this set of constraints.
 	 */
-	void clear() { _linearConstraints.clear(); }
+	void clear() { _constraints.clear(); }
 
 	/**
-	 * Add a linear constraint.
+	 * Add a constraint.
 	 *
-	 * @param linearConstraint The linear constraint to add.
+	 * @param constraint The constraint to add.
 	 */
-	void add(const LinearConstraint& linearConstraint);
+	void add(const Constraint& constraint);
 
 	/**
-	 * Add a set of linear constraints.
+	 * Add a set of constraints.
 	 *
-	 * @param linearConstraints The set of linear constraints to add.
+	 * @param constraints The set of constraints to add.
 	 */
-	void addAll(const LinearConstraints& linearConstraints);
+	void addAll(const Constraints& constraints);
 
 	/**
-	 * @return The number of linear constraints in this set.
+	 * @return The number of constraints in this set.
 	 */
-	unsigned int size() const { return _linearConstraints.size(); }
+	unsigned int size() const { return _constraints.size(); }
 
-	const const_iterator begin() const { return _linearConstraints.begin(); }
+	const const_iterator begin() const { return _constraints.begin(); }
 
-	iterator begin() { return _linearConstraints.begin(); }
+	iterator begin() { return _constraints.begin(); }
 
-	const const_iterator end() const { return _linearConstraints.end(); }
+	const const_iterator end() const { return _constraints.end(); }
 
-	iterator end() { return _linearConstraints.end(); }
+	iterator end() { return _constraints.end(); }
 
-	const LinearConstraint& operator[](size_t i) const { return _linearConstraints[i]; }
+	const Constraint& operator[](size_t i) const { return _constraints[i]; }
 
-	LinearConstraint& operator[](size_t i) { return _linearConstraints[i]; }
+	Constraint& operator[](size_t i) { return _constraints[i]; }
 
 	/**
-	 * Get a linst of indices of linear constraints that use the given 
-	 * variables.
+	 * Get a linst of indices of constraints that use the given variables.
 	 */
 	std::vector<unsigned int> getConstraints(const std::vector<unsigned int>& variableIds);
 
 private:
 
-	linear_constraints_type _linearConstraints;
+	constraints_type _constraints;
 };
 
-#endif // INFERENCE_LINEAR_CONSTRAINTS_H__
+#endif // INFERENCE_CONSTRAINTS_H__
```

### Comparing `ilpy-0.2.3/ilpy/impl/solvers/LinearSolverBackend.h` & `ilpy-0.3.0/ilpy/impl/solvers/SolverBackend.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-#ifndef INFERENCE_LINEAR_SOLVER_BACKEND_H__
-#define INFERENCE_LINEAR_SOLVER_BACKEND_H__
+#ifndef INFERENCE_SOLVER_BACKEND_H__
+#define INFERENCE_SOLVER_BACKEND_H__
 
-#include "LinearObjective.h"
-#include "LinearConstraints.h"
+#include "Objective.h"
+#include "Constraints.h"
 #include "Solution.h"
 #include "VariableType.h"
 
-class LinearSolverBackend {
+class SolverBackend {
 
 public:
 
-	virtual ~LinearSolverBackend() {}
+	virtual ~SolverBackend() {}
 
 	/**
 	 * Initialise the linear solver for the given type of variables.
 	 *
 	 * @param numVariables The number of variables in the problem.
 	 * @param variableType The type of the variables (Continuous, Integer,
 	 *                     Binary).
@@ -43,29 +43,29 @@
 			const std::map<unsigned int, VariableType>& specialVariableTypes) = 0;
 
 	/**
 	 * Set the objective.
 	 *
 	 * @param objective A linear objective.
 	 */
-	virtual void setObjective(const LinearObjective& objective) = 0;
+	virtual void setObjective(const Objective& objective) = 0;
 
 	/**
 	 * Set the linear (in)equality constraints.
 	 *
 	 * @param constraints A set of linear constraints.
 	 */
-	virtual void setConstraints(const LinearConstraints& constraints) = 0;
+	virtual void setConstraints(const Constraints& constraints) = 0;
 
 	/**
 	 * Add a single constraint.
 	 *
 	 * @param constraint A linear constraints.
 	 */
-	virtual void addConstraint(const LinearConstraint& constraint) = 0;
+	virtual void addConstraint(const Constraint& constraint) = 0;
 
 	/**
 	 * Set a timeout in seconds for subsequent solve calls.
 	 */
 	virtual void setTimeout(double timeout) = 0;
 
 	/**
@@ -107,9 +107,9 @@
 	 * @param value The optimal value of the objective.
 	 * @param message A status message from the solver.
 	 * @return true, if the optimal value was found.
 	 */
 	virtual bool solve(Solution& solution, std::string& message) = 0;
 };
 
-#endif // INFERENCE_LINEAR_SOLVER_BACKEND_H__
+#endif // INFERENCE_SOLVER_BACKEND_H__
```

### Comparing `ilpy-0.2.3/ilpy/impl/solvers/QuadraticObjective.cpp` & `ilpy-0.3.0/ilpy/impl/solvers/Objective.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -1,81 +1,86 @@
-#include "QuadraticObjective.h"
+#include "Objective.h"
 
-QuadraticObjective::QuadraticObjective(unsigned int size) :
+Objective::Objective(unsigned int size) :
 	_sense(Minimize),
 	_constant(0) {
 
 	resize(size);
 }
 
 void
-QuadraticObjective::setConstant(double constant) {
+Objective::setConstant(double constant) {
 
 	_constant = constant;
 }
 
 double
-QuadraticObjective::getConstant() const {
+Objective::getConstant() const {
 
 	return _constant;
 }
 
 void
-QuadraticObjective::setCoefficient(unsigned int varNum, double coef) {
+Objective::setCoefficient(unsigned int varNum, double coef) {
 
 	if (varNum >= size())
 		resize(varNum + 1);
 
 	_coefs[varNum] = coef;
 }
 
 const std::vector<double>&
-QuadraticObjective::getCoefficients() const {
+Objective::getCoefficients() const {
 
 	return _coefs;
 }
 
 void
-QuadraticObjective::setQuadraticCoefficient(unsigned int varNum1, unsigned int varNum2, double coef) {
+Objective::setQuadraticCoefficient(unsigned int varNum1, unsigned int varNum2, double coef) {
+
+	if (varNum1 >= size())
+		resize(varNum1 + 1);
+	if (varNum2 >= size())
+		resize(varNum2 + 1);
 
 	if (coef == 0) {
 
-		_quadraticCoefs.erase(_quadraticCoefs.find(std::make_pair(varNum1, varNum2)));
+		_quadraticCoefs.erase(std::make_pair(varNum1, varNum2));
 
 	} else {
 
 		_quadraticCoefs[std::make_pair(varNum1, varNum2)] = coef;
 	}
 }
 
 const std::map<std::pair<unsigned int, unsigned int>, double>&
-QuadraticObjective::getQuadraticCoefficients() const {
+Objective::getQuadraticCoefficients() const {
 
 	return _quadraticCoefs;
 }
 
 void
-QuadraticObjective::setSense(Sense sense) {
+Objective::setSense(Sense sense) {
 
 	_sense = sense;
 }
 
 Sense
-QuadraticObjective::getSense() const {
+Objective::getSense() const {
 
 	return _sense;
 }
 
 void
-QuadraticObjective::resize(unsigned int size) {
+Objective::resize(unsigned int size) {
 
 	_coefs.resize(size, 0.0);
 }
 
-std::ostream& operator<<(std::ostream& out, const QuadraticObjective& objective) {
+std::ostream& operator<<(std::ostream& out, const Objective& objective) {
 
 	for (unsigned int i = 0; i < objective.size(); i++)
 		out << objective.getCoefficients()[i] << "*" << i << " ";
 
 	typedef std::map<std::pair<unsigned int, unsigned int>, double>::value_type pair_t;
 	for (pair_t p : objective.getQuadraticCoefficients())
 		out << p.second << "*" << p.first.first << "*" << p.first.second << " ";
```

### Comparing `ilpy-0.2.3/ilpy/impl/solvers/QuadraticObjective.h` & `ilpy-0.3.0/ilpy/impl/solvers/Objective.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-#ifndef INFERENCE_QUADRATIC_OBJECTIVE_H__
-#define INFERENCE_QUADRATIC_OBJECTIVE_H__
+#ifndef INFERENCE_OBJECTIVE_H__
+#define INFERENCE_OBJECTIVE_H__
 
 #include <map>
 #include <vector>
 #include <utility>
 #include <ostream>
 
 #include "Sense.h"
 
-class QuadraticObjective {
+class Objective {
 
 public:
 
 	/**
 	 * Create a new quadratic objective for 'size' varibales.
 	 *
 	 * @param size The number of coefficients in the objective.
 	 */
-	explicit QuadraticObjective(unsigned int size = 0);
+	explicit Objective(unsigned int size = 0);
 
 	/**
 	 * Set the constant value of the expression.
 	 *
 	 * @param constant The value of the constant part of the objective.
 	 */
 	void setConstant(double constant);
@@ -101,11 +101,11 @@
 
 	// linear coefficients are assumed to be dense, therefore we use a vector
 	std::vector<double> _coefs;
 
 	std::map<std::pair<unsigned int, unsigned int>, double> _quadraticCoefs;
 };
 
-std::ostream& operator<<(std::ostream& out, const QuadraticObjective& objective);
+std::ostream& operator<<(std::ostream& out, const Objective& objective);
 
-#endif // INFERENCE_QUADRATIC_OBJECTIVE_H__
+#endif // INFERENCE_OBJECTIVE_H__
```

### Comparing `ilpy-0.2.3/ilpy/impl/solvers/ScipBackend.cpp` & `ilpy-0.3.0/ilpy/impl/solvers/ScipBackend.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 #ifdef HAVE_SCIP
 
 #include <sstream>
 
 #include <scip/scipdefplugins.h>
 #include <scip/cons_linear.h>
+#include <scip/cons_quadratic.h>
 
 #include "ScipBackend.h"
 
 ScipBackend::ScipBackend() :
 		_scip(0) {
 
 	SCIP_CALL_ABORT(SCIPcreate(&_scip));
@@ -65,21 +66,15 @@
 	}
 
 	for (SCIP_VAR* v : _variables)
 		SCIP_CALL_ABORT(SCIPreleaseVar(_scip, &v));
 }
 
 void
-ScipBackend::setObjective(const LinearObjective& objective) {
-
-	setObjective((QuadraticObjective)objective);
-}
-
-void
-ScipBackend::setObjective(const QuadraticObjective& objective) {
+ScipBackend::setObjective(const Objective& objective) {
 
 	// set sense of objective
 	if (objective.getSense() == Minimize)
 		SCIP_CALL_ABORT(SCIPsetObjsense(_scip, SCIP_OBJSENSE_MINIMIZE));
 	else
 		SCIP_CALL_ABORT(SCIPsetObjsense(_scip, SCIP_OBJSENSE_MAXIMIZE));
 
@@ -124,40 +119,48 @@
 			// decrease reference count (we are done with z_ij)
 			SCIP_CALL_ABORT(SCIPreleaseVar(_scip, &z_ij));
 		}
 	}
 }
 
 void
-ScipBackend::setConstraints(const LinearConstraints& constraints) {
+ScipBackend::setConstraints(const Constraints& constraints) {
 
 	// remove previous constraints
 	freeConstraints();
 
 	// allocate memory for new constraints
 	_constraints.reserve(constraints.size());
 
 	unsigned int j = 0;
-	for (const LinearConstraint& constraint : constraints) {
+	for (const Constraint& constraint : constraints) {
 
 		addConstraint(constraint);
 
 		j++;
 	}
 }
 
 void
-ScipBackend::addConstraint(const LinearConstraint& constraint) {
+ScipBackend::addConstraint(const Constraint& constraint) {
 
 	// create a list of variables and their coefficients
-	std::vector<SCIP_VAR*> vars;
-	std::vector<SCIP_Real> coefs;
+	std::vector<SCIP_VAR*> linvars;
+	std::vector<SCIP_Real> lincoefs;
+	std::vector<SCIP_VAR*> quadvars1;
+	std::vector<SCIP_VAR*> quadvars2;
+	std::vector<SCIP_Real> quadcoefs;
 	for (auto& p : constraint.getCoefficients()) {
-		vars.push_back(_variables[p.first]);
-		coefs.push_back(p.second);
+		linvars.push_back(_variables[p.first]);
+		lincoefs.push_back(p.second);
+	}
+	for (auto& pq : constraint.getQuadraticCoefficients()) {
+		quadvars1.push_back(_variables[pq.first.first]);
+		quadvars2.push_back(_variables[pq.first.second]);
+		quadcoefs.push_back(pq.second);
 	}
 
 	// create the SCIP constraint lhs <= linear expr <= rhs
 	SCIP_CONS* c;
 	std::string name("c");
 	name += std::to_string(_constraints.size());
 
@@ -165,21 +168,25 @@
 	SCIP_Real lhs = constraint.getValue();
 	SCIP_Real rhs = constraint.getValue();
 	if (constraint.getRelation() == LessEqual)
 		lhs = -SCIPinfinity(_scip);
 	if (constraint.getRelation() == GreaterEqual)
 		rhs = SCIPinfinity(_scip);
 
-	SCIP_CALL_ABORT(SCIPcreateConsBasicLinear(
+	SCIP_CALL_ABORT(SCIPcreateConsBasicQuadratic(
 			_scip,
 			&c,
 			name.c_str(),
-			vars.size(),
-			&vars[0],
-			&coefs[0],
+			linvars.size(),
+			&linvars[0],
+			&lincoefs[0],
+			quadvars1.size(),
+			&quadvars1[0],
+			&quadvars2[0],
+			&quadcoefs[0],
 			lhs,
 			rhs));
 
 	_constraints.push_back(c);
 
 	SCIP_CALL_ABORT(SCIPaddCons(_scip, c));
 	SCIP_CALL_ABORT(SCIPreleaseCons(_scip, &c));
@@ -232,19 +239,16 @@
 
 	return true;
 }
 
 void
 ScipBackend::setVerbose(bool verbose) {
 
-	// setup GRB environment
-	//if (verbose)
-		//_model.getEnv().set(GRB_IntParam_OutputFlag, 1);
-	//else
-		//_model.getEnv().set(GRB_IntParam_OutputFlag, 0);
+	int level = verbose ? 4 : 0;
+	SCIP_CALL_ABORT(SCIPsetIntParam(_scip, "display/verblevel", level));
 }
 
 void
 ScipBackend::addMulEqualConstraint(unsigned int i, unsigned int j, SCIP_VAR* z_ij) {
 
 	// add the following quadratic constraint:
 	// x_i * x_j - z_ij = 0
```

### Comparing `ilpy-0.2.3/ilpy/impl/solvers/ScipBackend.h` & `ilpy-0.3.0/ilpy/impl/solvers/ScipBackend.h`

 * *Files 17% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 #include <config.h>
 #ifdef HAVE_SCIP
 
 #include <string>
 
 #include <scip/scip.h>
 
-#include "LinearConstraints.h"
-#include "QuadraticObjective.h"
-#include "QuadraticSolverBackend.h"
+#include "Constraints.h"
+#include "Objective.h"
+#include "SolverBackend.h"
 #include "Sense.h"
 #include "Solution.h"
 
 /**
  * Scip interface to solve the following (integer) quadratic program:
  *
  * min  <a,x> + xQx
@@ -23,15 +23,15 @@
  *      optionally: x_i \in {0,1} for all i
  *
  * Where (A,b) describes all linear equality constraints, (C,d) all linear
  * inequality constraints and x is the solution vector. a is a real-valued
  * vector denoting the coefficients of the objective and Q a PSD matrix giving
  * the quadratic coefficients of the objective.
  */
-class ScipBackend : public QuadraticSolverBackend {
+class ScipBackend : public SolverBackend {
 
 public:
 
 	ScipBackend();
 
 	virtual ~ScipBackend();
 
@@ -44,21 +44,19 @@
 			VariableType variableType);
 
 	void initialize(
 			unsigned int                                numVariables,
 			VariableType                                defaultVariableType,
 			const std::map<unsigned int, VariableType>& specialVariableTypes);
 
-	void setObjective(const LinearObjective& objective);
+	void setObjective(const Objective& objective);
 
-	void setObjective(const QuadraticObjective& objective);
+	void setConstraints(const Constraints& constraints);
 
-	void setConstraints(const LinearConstraints& constraints);
-
-	void addConstraint(const LinearConstraint& constraint);
+	void addConstraint(const Constraint& constraint);
 
 	void setTimeout(double timeout);
 
 	void setOptimalityGap(double gap, bool absolute=false);
 
 	void setNumThreads(unsigned int numThreads);
```

### Comparing `ilpy-0.2.3/ilpy/impl/solvers/Solution.h` & `ilpy-0.3.0/ilpy/impl/solvers/Solution.h`

 * *Files identical despite different names*

### Comparing `ilpy-0.2.3/ilpy.egg-info/SOURCES.txt` & `ilpy-0.3.0/ilpy.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,41 @@
+CONTRIBUTING.md
+LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 ilpy/__init__.py
+ilpy/_functional.py
 ilpy/decl.pxd
+ilpy/expressions.py
 ilpy/py.typed
 ilpy/wrapper.pyi
 ilpy/wrapper.pyx
 ilpy.egg-info/PKG-INFO
 ilpy.egg-info/SOURCES.txt
 ilpy.egg-info/dependency_links.txt
 ilpy.egg-info/requires.txt
 ilpy.egg-info/top_level.txt
 ilpy/impl/config.h
 ilpy/impl/gurobi_c.h
 ilpy/impl/solvers/BackendPreference.h
-ilpy/impl/solvers/CMakeLists.txt
+ilpy/impl/solvers/Constraint.cpp
+ilpy/impl/solvers/Constraint.h
+ilpy/impl/solvers/Constraints.cpp
+ilpy/impl/solvers/Constraints.h
 ilpy/impl/solvers/CplexBackend.cpp
 ilpy/impl/solvers/CplexBackend.h
 ilpy/impl/solvers/GurobiBackend.cpp
 ilpy/impl/solvers/GurobiBackend.h
-ilpy/impl/solvers/LinearConstraint.cpp
-ilpy/impl/solvers/LinearConstraint.h
-ilpy/impl/solvers/LinearConstraints.cpp
-ilpy/impl/solvers/LinearConstraints.h
-ilpy/impl/solvers/LinearObjective.h
-ilpy/impl/solvers/LinearSolverBackend.h
-ilpy/impl/solvers/LinearSolverBackendFactory.h
-ilpy/impl/solvers/QuadraticObjective.cpp
-ilpy/impl/solvers/QuadraticObjective.h
-ilpy/impl/solvers/QuadraticSolverBackend.h
-ilpy/impl/solvers/QuadraticSolverBackendFactory.h
-ilpy/impl/solvers/QuadraticSolverParameters.h
+ilpy/impl/solvers/Objective.cpp
+ilpy/impl/solvers/Objective.h
 ilpy/impl/solvers/Relation.h
 ilpy/impl/solvers/ScipBackend.cpp
 ilpy/impl/solvers/ScipBackend.h
 ilpy/impl/solvers/Sense.h
 ilpy/impl/solvers/Solution.cpp
 ilpy/impl/solvers/Solution.h
+ilpy/impl/solvers/SolverBackend.h
 ilpy/impl/solvers/SolverFactory.cpp
 ilpy/impl/solvers/SolverFactory.h
 ilpy/impl/solvers/VariableType.h
```

### Comparing `ilpy-0.2.3/setup.py` & `ilpy-0.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,47 @@
 import os
-
 from ctypes import util
 
 from Cython.Build import cythonize
 from setuptools import setup
 from setuptools.extension import Extension
 
+# enable test coverage tracing if CYTHON_TRACE is set to a non-zero value
+CYTHON_TRACE = int(os.getenv("CYTHON_TRACE", "0") not in ("0", "False"))
+
 libraries = ["libscip"] if os.name == "nt" else ["scip"]
-include_dirs = ['ilpy/impl']
+include_dirs = ["ilpy/impl"]
 library_dirs = []
 compile_args = ["-O3", "-std=c++11", "-DHAVE_SCIP"]
 
 # include conda environment windows include/lib if it exists
 # this will be done automatically by conda build, but is useful if someone
 # tries to build this directly with pip install in a conda environment
 if os.name == "nt" and "CONDA_PREFIX" in os.environ:
     include_dirs.append(os.path.join(os.environ["CONDA_PREFIX"], "Library", "include"))
     library_dirs.append(os.path.join(os.environ["CONDA_PREFIX"], "Library", "lib"))
 
 # look for various gurobi versions, which are annoyingly
 # suffixed with the version number, and wildcards don't work
 for v in ["100"]:
-    GUROBI_LIB = f"libgurobi{v}" if os.name == 'nt' else f"gurobi{v}"
+    GUROBI_LIB = f"libgurobi{v}" if os.name == "nt" else f"gurobi{v}"
     if (gurolib := util.find_library(GUROBI_LIB)) is not None:
         print("FOUND GUROBI library: ", gurolib)
         libraries.append(GUROBI_LIB)
         compile_args.append("-DHAVE_GUROBI")
         break
 else:
     print("WARNING: GUROBI library not found")
 
 
-setup(
-        name='ilpy',
-        version='0.2.3',
-        description='Python wrappers for popular MIP solvers.',
-        url='https://github.com/funkelab/ilpy',
-        author='Jan Funke',
-        author_email='funkej@janelia.hhmi.org',
-        license='MIT',
-        packages=[
-            'ilpy'
-        ],
-        ext_modules=cythonize([
-            Extension(
-                'ilpy.wrapper',
-                sources=[
-                    'ilpy/wrapper.pyx',
-                ],
-                extra_compile_args=compile_args,
-                include_dirs=include_dirs,
-                libraries=libraries,
-                library_dirs=library_dirs,
-                language='c++')
-        ]),
-        extras_require={
-          "dev": ["flake8", "pytest", "pytest-cov"],
-        },
-        package_data={
-            "ilpy": ["py.typed", "*.pyi"]
-        },
+wrapper = Extension(
+    "ilpy.wrapper",
+    sources=["ilpy/wrapper.pyx"],
+    extra_compile_args=compile_args,
+    include_dirs=include_dirs,
+    libraries=libraries,
+    library_dirs=library_dirs,
+    language="c++",
+    define_macros=[("CYTHON_TRACE", CYTHON_TRACE)],
 )
+
+setup(ext_modules=cythonize([wrapper], compiler_directives={"linetrace": CYTHON_TRACE}))
```

