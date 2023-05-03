# Comparing `tmp/pyvpsolver-3.1.3.tar.gz` & `tmp/pyvpsolver-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvpsolver-3.1.3.tar", last modified: Sat Oct  2 17:10:34 2021, max compression
+gzip compressed data, was "pyvpsolver-3.1.4.tar", last modified: Wed May  3 16:04:42 2023, max compression
```

## Comparing `pyvpsolver-3.1.3.tar` & `pyvpsolver-3.1.4.tar`

### file list

```diff
@@ -1,100 +1,110 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-02 17:10:34.009888 pyvpsolver-3.1.3/
--rw-r--r--   0 vsts      (1001) docker     (121)     2245 2021-10-02 17:10:30.821648 pyvpsolver-3.1.3/CHANGELOG.md
--rw-r--r--   0 vsts      (1001) docker     (121)    34520 2021-10-02 17:10:30.821648 pyvpsolver-3.1.3/COPYING
--rw-r--r--   0 vsts      (1001) docker     (121)      838 2021-10-02 17:10:30.821648 pyvpsolver-3.1.3/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)     1610 2021-10-02 17:10:34.009888 pyvpsolver-3.1.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     9939 2021-10-02 17:10:30.821648 pyvpsolver-3.1.3/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-02 17:10:34.005887 pyvpsolver-3.1.3/pyvpsolver/
--rw-r--r--   0 vsts      (1001) docker     (121)      999 2021-10-02 17:10:30.881652 pyvpsolver-3.1.3/pyvpsolver/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8986 2021-10-02 17:10:30.881652 pyvpsolver-3.1.3/pyvpsolver/afgraph.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-02 17:10:34.005887 pyvpsolver-3.1.3/pyvpsolver/solvers/
--rw-r--r--   0 vsts      (1001) docker     (121)      991 2021-10-02 17:10:30.881652 pyvpsolver-3.1.3/pyvpsolver/solvers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10914 2021-10-02 17:10:30.881652 pyvpsolver-3.1.3/pyvpsolver/solvers/mvpsolver2013.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3362 2021-10-02 17:10:30.881652 pyvpsolver-3.1.3/pyvpsolver/solvers/mvpsolver2016.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3259 2021-10-02 17:10:30.881652 pyvpsolver-3.1.3/pyvpsolver/solvers/vbpsolver.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-02 17:10:34.005887 pyvpsolver-3.1.3/pyvpsolver/swig/
--rw-r--r--   0 vsts      (1001) docker     (121)      956 2021-10-02 17:10:30.881652 pyvpsolver-3.1.3/pyvpsolver/swig/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2276 2021-10-02 17:10:30.881652 pyvpsolver-3.1.3/pyvpsolver/swig/afg2lp.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2284 2021-10-02 17:10:30.881652 pyvpsolver-3.1.3/pyvpsolver/swig/afg2mps.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2284 2021-10-02 17:10:30.881652 pyvpsolver-3.1.3/pyvpsolver/swig/vbp2afg.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2276 2021-10-02 17:10:30.881652 pyvpsolver-3.1.3/pyvpsolver/swig/vbpsol.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5496 2021-10-02 17:10:30.881652 pyvpsolver-3.1.3/pyvpsolver/utils.py
--rw-r--r--   0 vsts      (1001) docker     (121)    19266 2021-10-02 17:10:30.885652 pyvpsolver-3.1.3/pyvpsolver/vpsolver.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-02 17:10:34.005887 pyvpsolver-3.1.3/pyvpsolver/webapp/
--rw-r--r--   0 vsts      (1001) docker     (121)      888 2021-10-02 17:10:30.885652 pyvpsolver-3.1.3/pyvpsolver/webapp/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7389 2021-10-02 17:10:30.885652 pyvpsolver-3.1.3/pyvpsolver/webapp/app.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-02 17:10:34.005887 pyvpsolver-3.1.3/pyvpsolver/webapp/data/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-02 17:10:34.005887 pyvpsolver-3.1.3/pyvpsolver/webapp/data/examples/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-02 17:10:34.005887 pyvpsolver-3.1.3/pyvpsolver/webapp/data/examples/mvp/
--rw-r--r--   0 vsts      (1001) docker     (121)      135 2021-10-02 17:10:30.885652 pyvpsolver-3.1.3/pyvpsolver/webapp/data/examples/mvp/mvp.mvp
--rw-r--r--   0 vsts      (1001) docker     (121)      201 2021-10-02 17:10:30.885652 pyvpsolver-3.1.3/pyvpsolver/webapp/data/examples/mvp/vsbpp.mvp
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-02 17:10:34.005887 pyvpsolver-3.1.3/pyvpsolver/webapp/data/examples/vbp/
--rwxr-xr-x   0 vsts      (1001) docker     (121)      280 2021-10-02 17:10:30.885652 pyvpsolver-3.1.3/pyvpsolver/webapp/data/examples/vbp/bpp.vbp
--rwxr-xr-x   0 vsts      (1001) docker     (121)       54 2021-10-02 17:10:30.885652 pyvpsolver-3.1.3/pyvpsolver/webapp/data/examples/vbp/csp.vbp
--rwxr-xr-x   0 vsts      (1001) docker     (121)     3238 2021-10-02 17:10:30.885652 pyvpsolver-3.1.3/pyvpsolver/webapp/data/examples/vbp/vbp.vbp
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-02 17:10:34.005887 pyvpsolver-3.1.3/pyvpsolver/webapp/static/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-02 17:10:34.005887 pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-02 17:10:34.005887 pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/css/
--rwxr-xr-x   0 vsts      (1001) docker     (121)   117024 2021-10-02 17:10:30.885652 pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/css/bootstrap-theme-readable.css
--rw-r--r--   0 vsts      (1001) docker     (121)    26132 2021-10-02 17:10:30.885652 pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/css/bootstrap-theme.css
--rw-r--r--   0 vsts      (1001) docker     (121)    47721 2021-10-02 17:10:30.885652 pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/css/bootstrap-theme.css.map
--rw-r--r--   0 vsts      (1001) docker     (121)    23357 2021-10-02 17:10:30.885652 pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/css/bootstrap-theme.min.css
--rw-r--r--   0 vsts      (1001) docker     (121)   147430 2021-10-02 17:10:30.885652 pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/css/bootstrap.css
--rw-r--r--   0 vsts      (1001) docker     (121)   390518 2021-10-02 17:10:30.889653 pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/css/bootstrap.css.map
--rw-r--r--   0 vsts      (1001) docker     (121)   122540 2021-10-02 17:10:30.889653 pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-02 17:10:34.005887 pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/fonts/
--rw-r--r--   0 vsts      (1001) docker     (121)    20127 2021-10-02 17:10:30.889653 pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 vsts      (1001) docker     (121)   108738 2021-10-02 17:10:30.889653 pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 vsts      (1001) docker     (121)    45404 2021-10-02 17:10:30.889653 pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 vsts      (1001) docker     (121)    23424 2021-10-02 17:10:30.889653 pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 vsts      (1001) docker     (121)    18028 2021-10-02 17:10:30.889653 pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-02 17:10:34.005887 pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/js/
--rw-r--r--   0 vsts      (1001) docker     (121)    68890 2021-10-02 17:10:30.889653 pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/js/bootstrap.js
--rw-r--r--   0 vsts      (1001) docker     (121)    36816 2021-10-02 17:10:30.889653 pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/js/bootstrap.min.js
--rw-r--r--   0 vsts      (1001) docker     (121)      484 2021-10-02 17:10:30.889653 pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/js/npm.js
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-02 17:10:34.005887 pyvpsolver-3.1.3/pyvpsolver/webapp/static/css/
--rw-r--r--   0 vsts      (1001) docker     (121)      191 2021-10-02 17:10:30.889653 pyvpsolver-3.1.3/pyvpsolver/webapp/static/css/app.css
--rw-r--r--   0 vsts      (1001) docker     (121)   122540 2021-10-02 17:10:30.889653 pyvpsolver-3.1.3/pyvpsolver/webapp/static/css/bootstrap.min.css
--rwxr-xr-x   0 vsts      (1001) docker     (121)     1406 2021-10-02 17:10:30.889653 pyvpsolver-3.1.3/pyvpsolver/webapp/static/favicon.ico
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-02 17:10:34.009888 pyvpsolver-3.1.3/pyvpsolver/webapp/static/js/
--rw-r--r--   0 vsts      (1001) docker     (121)      742 2021-10-02 17:10:30.889653 pyvpsolver-3.1.3/pyvpsolver/webapp/static/js/app.js
--rw-r--r--   0 vsts      (1001) docker     (121)   284184 2021-10-02 17:10:30.889653 pyvpsolver-3.1.3/pyvpsolver/webapp/static/js/jquery-1.11.2.js
--rw-r--r--   0 vsts      (1001) docker     (121)   142010 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/pyvpsolver/webapp/static/js/jquery-1.11.2.min.map
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-02 17:10:34.009888 pyvpsolver-3.1.3/pyvpsolver/webapp/templates/
--rw-r--r--   0 vsts      (1001) docker     (121)     3737 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/pyvpsolver/webapp/templates/input.html
--rw-r--r--   0 vsts      (1001) docker     (121)      114 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/requirements.txt
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-02 17:10:34.009888 pyvpsolver-3.1.3/scripts/
--rwxr-xr-x   0 vsts      (1001) docker     (121)     1024 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/scripts/afg2lp
--rwxr-xr-x   0 vsts      (1001) docker     (121)     1026 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/scripts/afg2mps
--rwxr-xr-x   0 vsts      (1001) docker     (121)     1273 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/scripts/afg2svg
--rwxr-xr-x   0 vsts      (1001) docker     (121)     1026 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/scripts/vbp2afg
--rwxr-xr-x   0 vsts      (1001) docker     (121)     1024 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/scripts/vbpsol
--rwxr-xr-x   0 vsts      (1001) docker     (121)     4545 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/scripts/vpsolver_coinor.sh
--rwxr-xr-x   0 vsts      (1001) docker     (121)     4550 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/scripts/vpsolver_cplex.sh
--rwxr-xr-x   0 vsts      (1001) docker     (121)     5181 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/scripts/vpsolver_glpk.sh
--rwxr-xr-x   0 vsts      (1001) docker     (121)     4461 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/scripts/vpsolver_gurobi.sh
--rwxr-xr-x   0 vsts      (1001) docker     (121)     4659 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/scripts/vpsolver_lpsolve.sh
--rwxr-xr-x   0 vsts      (1001) docker     (121)     4521 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/scripts/vpsolver_scip.sh
--rw-r--r--   0 vsts      (1001) docker     (121)     4232 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-02 17:10:34.009888 pyvpsolver-3.1.3/src/
--rw-r--r--   0 vsts      (1001) docker     (121)     5171 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/src/afg2lp.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5996 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/src/afg2mps.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    18771 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/src/arcflow.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2509 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/src/arcflow.hpp
--rw-r--r--   0 vsts      (1001) docker     (121)     8290 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/src/arcflowsol.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1893 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/src/arcflowsol.hpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1238 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/src/common.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1842 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/src/common.hpp
--rw-r--r--   0 vsts      (1001) docker     (121)      830 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/src/config.hpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2553 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/src/graph.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1717 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/src/graph.hpp
--rw-r--r--   0 vsts      (1001) docker     (121)     9775 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/src/instance.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2129 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/src/instance.hpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2485 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/src/vbp2afg.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2895 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/src/vbpsol.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6539 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/src/vpsolver.cpp
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-10-02 17:10:34.009888 pyvpsolver-3.1.3/swig/
--rw-r--r--   0 vsts      (1001) docker     (121)   138796 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/swig/afg2lp_wrap.cxx
--rw-r--r--   0 vsts      (1001) docker     (121)   138800 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/swig/afg2mps_wrap.cxx
--rw-r--r--   0 vsts      (1001) docker     (121)   138800 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/swig/vbp2afg_wrap.cxx
--rw-r--r--   0 vsts      (1001) docker     (121)   138796 2021-10-02 17:10:30.893653 pyvpsolver-3.1.3/swig/vbpsol_wrap.cxx
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 16:04:42.117420 pyvpsolver-3.1.4/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2360 2023-05-03 16:04:31.000000 pyvpsolver-3.1.4/CHANGELOG.md
+-rw-r--r--   0 vsts      (1001) docker     (122)     1521 2023-05-03 16:04:31.000000 pyvpsolver-3.1.4/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      179 2023-05-03 16:04:31.000000 pyvpsolver-3.1.4/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1415 2023-05-03 16:04:42.117420 pyvpsolver-3.1.4/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     9777 2023-05-03 16:04:31.000000 pyvpsolver-3.1.4/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 16:04:42.105420 pyvpsolver-3.1.4/pyvpsolver/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 16:04:42.105420 pyvpsolver-3.1.4/pyvpsolver/.vscode/
+-rw-r--r--   0 vsts      (1001) docker     (122)      942 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/.vscode/settings.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      206 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8272 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/afgraph.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 16:04:42.105420 pyvpsolver-3.1.4/pyvpsolver/solvers/
+-rw-r--r--   0 vsts      (1001) docker     (122)      198 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/solvers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10201 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/solvers/mvpsolver2013.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2569 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/solvers/mvpsolver2016.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2490 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/solvers/vbpsolver.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4728 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18329 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/vpsolver.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 16:04:42.105420 pyvpsolver-3.1.4/pyvpsolver/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6557 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/app.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 16:04:42.101420 pyvpsolver-3.1.4/pyvpsolver/webapp/data/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 16:04:42.105420 pyvpsolver-3.1.4/pyvpsolver/webapp/data/examples/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 16:04:42.105420 pyvpsolver-3.1.4/pyvpsolver/webapp/data/examples/mvp/
+-rw-r--r--   0 vsts      (1001) docker     (122)      135 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/data/examples/mvp/mvp.mvp
+-rw-r--r--   0 vsts      (1001) docker     (122)      201 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/data/examples/mvp/vsbpp.mvp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 16:04:42.109420 pyvpsolver-3.1.4/pyvpsolver/webapp/data/examples/vbp/
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      280 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/data/examples/vbp/bpp.vbp
+-rwxr-xr-x   0 vsts      (1001) docker     (122)       54 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/data/examples/vbp/csp.vbp
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     3238 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/data/examples/vbp/vbp.vbp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 16:04:42.109420 pyvpsolver-3.1.4/pyvpsolver/webapp/static/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 16:04:42.105420 pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 16:04:42.109420 pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/css/
+-rwxr-xr-x   0 vsts      (1001) docker     (122)   117024 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/css/bootstrap-theme-readable.css
+-rw-r--r--   0 vsts      (1001) docker     (122)    26132 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/css/bootstrap-theme.css
+-rw-r--r--   0 vsts      (1001) docker     (122)    47721 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/css/bootstrap-theme.css.map
+-rw-r--r--   0 vsts      (1001) docker     (122)    23357 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/css/bootstrap-theme.min.css
+-rw-r--r--   0 vsts      (1001) docker     (122)   147430 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/css/bootstrap.css
+-rw-r--r--   0 vsts      (1001) docker     (122)   390518 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0 vsts      (1001) docker     (122)   122540 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 16:04:42.109420 pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/fonts/
+-rw-r--r--   0 vsts      (1001) docker     (122)    20127 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 vsts      (1001) docker     (122)   108738 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 vsts      (1001) docker     (122)    45404 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 vsts      (1001) docker     (122)    23424 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 vsts      (1001) docker     (122)    18028 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 16:04:42.109420 pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/js/
+-rw-r--r--   0 vsts      (1001) docker     (122)    68890 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/js/bootstrap.js
+-rw-r--r--   0 vsts      (1001) docker     (122)    36816 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0 vsts      (1001) docker     (122)      484 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/js/npm.js
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 16:04:42.109420 pyvpsolver-3.1.4/pyvpsolver/webapp/static/css/
+-rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/static/css/app.css
+-rw-r--r--   0 vsts      (1001) docker     (122)   122540 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/static/css/bootstrap.min.css
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1406 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/static/favicon.ico
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 16:04:42.113420 pyvpsolver-3.1.4/pyvpsolver/webapp/static/js/
+-rw-r--r--   0 vsts      (1001) docker     (122)      742 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/static/js/app.js
+-rw-r--r--   0 vsts      (1001) docker     (122)   284184 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/static/js/jquery-1.11.2.js
+-rw-r--r--   0 vsts      (1001) docker     (122)   142010 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/static/js/jquery-1.11.2.min.map
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 16:04:42.113420 pyvpsolver-3.1.4/pyvpsolver/webapp/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3737 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/pyvpsolver/webapp/templates/input.html
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 16:04:42.105420 pyvpsolver-3.1.4/pyvpsolver.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1415 2023-05-03 16:04:42.000000 pyvpsolver-3.1.4/pyvpsolver.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     2719 2023-05-03 16:04:42.000000 pyvpsolver-3.1.4/pyvpsolver.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-03 16:04:42.000000 pyvpsolver-3.1.4/pyvpsolver.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      100 2023-05-03 16:04:42.000000 pyvpsolver-3.1.4/pyvpsolver.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       55 2023-05-03 16:04:42.000000 pyvpsolver-3.1.4/pyvpsolver.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      114 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/requirements.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 16:04:42.113420 pyvpsolver-3.1.4/scripts/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 16:04:42.113420 pyvpsolver-3.1.4/scripts/.vscode/
+-rw-r--r--   0 vsts      (1001) docker     (122)      942 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/scripts/.vscode/settings.json
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      140 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/scripts/afg2ampl
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      138 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/scripts/afg2lp
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      139 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/scripts/afg2mps
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      407 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/scripts/afg2svg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      139 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/scripts/vbp2afg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      138 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/scripts/vbpsol
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1224 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/scripts/vpsolver_ampl.sh
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     4683 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/scripts/vpsolver_base.sh
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      867 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/scripts/vpsolver_coinor.sh
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      872 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/scripts/vpsolver_cplex.sh
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1503 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/scripts/vpsolver_glpk.sh
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      783 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/scripts/vpsolver_gurobi.sh
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      981 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/scripts/vpsolver_lpsolve.sh
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      843 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/scripts/vpsolver_scip.sh
+-rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-05-03 16:04:42.117420 pyvpsolver-3.1.4/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     4469 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 16:04:42.117420 pyvpsolver-3.1.4/src/
+-rw-r--r--   0 vsts      (1001) docker     (122)     4131 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/src/afg2ampl.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     3395 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/src/afg2lp.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4223 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/src/afg2mps.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    15002 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/src/arcflow.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1680 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/src/arcflow.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     5895 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/src/arcflowsol.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1086 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/src/arcflowsol.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      350 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/src/common.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1220 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/src/common.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      830 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/src/config.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1551 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/src/graph.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      976 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/src/graph.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     7186 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/src/instance.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1251 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/src/instance.hpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1378 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/src/vbp2afg.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1805 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/src/vbpsol.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)     4834 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/src/vpsolver.cpp
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-03 16:04:42.117420 pyvpsolver-3.1.4/swig/
+-rw-r--r--   0 vsts      (1001) docker     (122)   138804 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/swig/afg2ampl_wrap.cxx
+-rw-r--r--   0 vsts      (1001) docker     (122)   138796 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/swig/afg2lp_wrap.cxx
+-rw-r--r--   0 vsts      (1001) docker     (122)   138800 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/swig/afg2mps_wrap.cxx
+-rw-r--r--   0 vsts      (1001) docker     (122)   138800 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/swig/vbp2afg_wrap.cxx
+-rw-r--r--   0 vsts      (1001) docker     (122)   138796 2023-05-03 16:04:32.000000 pyvpsolver-3.1.4/swig/vbpsol_wrap.cxx
```

### Comparing `pyvpsolver-3.1.3/CHANGELOG.md` & `pyvpsolver-3.1.4/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # Change Log
 All notable changes to this project will be documented in this file.
 This project adheres to [Semantic Versioning](http://semver.org/).
 
+## [3.1.4] - 2023-05-03
+
+### Added
+- Wheels for Python up to 3.11.
+
+### Fixed
+- Fixed compilation error on Linux.
+
 ## [3.1.3] - 2021-10-02
 
 ### Added
 - Basic CMake support.
 - Binary wheels for all platforms.
 
 ## [3.1.2] - 2016-06-28
```

### Comparing `pyvpsolver-3.1.3/PKG-INFO` & `pyvpsolver-3.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,49 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyvpsolver
-Version: 3.1.3
+Version: 3.1.4
 Summary: Arc-flow Vector Packing Solver (VPSolver)
 Home-page: https://github.com/fdabrandao/vpsolver
 Author: Filipe Brandao
 Author-email: fdabrandao@gmail.com
-License: AGPLv3+
-Description: 
-        VPSolver
-        --------
-        VPSolver is a vector packing solver based on an arc-flow formulation
-        with graph compression. VPSolver generates very strong models that can
-        be solved using general-purpose mixed-integer programming solvers such
-        as Gurobi and GLPK. For modelling other problems easily, VPSolver
-        includes a Python API and a modelling toolbox (PyMPL).
-        
-        Setup
-        `````
-        
-        .. code:: bash
-        
-            $ pip install pyvpsolver
-        
-        System requirements
-        ```````````````````
-        
-        * UNIX-like operating system or a UNIX-like environment such as Cygwin
-        * g++ >= 4.8; bash >= 3.0
-        
-        Links
-        `````
-        
-        * `VPSolver wiki <https://github.com/fdabrandao/vpsolver/wiki>`_
-        * `GiHub repository <https://github.com/fdabrandao/vpsolver>`_
-        * `BitBucket repository <https://bitbucket.org/fdabrandao/vpsolver>`_
-        
+Maintainer: Filipe Brandao
+Maintainer-email: fdabrandao@gmail.com
+License: BSD-3
 Platform: unix
 Platform: linux
 Platform: osx
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering
+License-File: LICENSE
+
+
+VPSolver
+--------
+VPSolver is a vector packing solver based on an arc-flow formulation
+with graph compression. VPSolver generates very strong models that can
+be solved using general-purpose mixed-integer programming solvers such
+as Gurobi and GLPK. For modelling other problems easily, VPSolver
+includes a Python API and a modelling toolbox (PyMPL).
+
+Setup
+`````
+
+.. code:: bash
+
+    $ pip install pyvpsolver
+
+System requirements
+```````````````````
+
+* UNIX-like operating system or a UNIX-like environment such as Cygwin
+* g++ >= 4.8; bash >= 3.0
+
+Links
+`````
+
+* `VPSolver wiki <https://github.com/fdabrandao/vpsolver/wiki>`_
+* `GiHub repository <https://github.com/fdabrandao/vpsolver>`_
+* `BitBucket repository <https://bitbucket.org/fdabrandao/vpsolver>`_
```

### Comparing `pyvpsolver-3.1.3/README.md` & `pyvpsolver-3.1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,69 @@
 ## Arc-flow Vector Packing Solver (VPSolver)
 
-Copyright (C) 2013-2016, Filipe Brandão  
-Faculdade de Ciências, Universidade do Porto  
-Porto, Portugal. All rights reserved. E-mail: <fdabrandao@dcc.fc.up.pt>.
+Copyright (C) 2013-2022, Filipe Brandão <fdabrandao@gmail.com>
 
 ---
 [VPSolver](https://github.com/fdabrandao/vpsolver) is a multiple-choice vector packing solver based on an arc-flow formulation with graph compression (see, e.g., [\[1\]](#references)). VPSolver generates very strong models (equivalent to Gilmore and Gomory's) that can be solved using general-purpose mixed-integer programming
-solvers such as Gurobi and GLPK (see, e.g., [\[2\]](#references) and [\[3\]](#references)). VPSolver does not explicitly require any MIP
-solver in particular, though a good  MIP solver may be necessary for solving
-large models.
-
-![](https://img.shields.io/badge/license-AGPLv3+-blue.svg)
-[![](https://travis-ci.org/fdabrandao/vpsolver.svg?branch=master)](https://travis-ci.org/fdabrandao/vpsolver)
-[![Coverage Status](https://coveralls.io/repos/github/fdabrandao/vpsolver/badge.svg?branch=develop)](https://coveralls.io/github/fdabrandao/vpsolver)
+solvers such as Gurobi and GLPK (see, e.g., [\[2\]](#references) and [\[3\]](#references)). VPSolver does not explicitly require any MIP solver in particular, though a good  MIP solver may be necessary for solving large models.
 
-For modelling other problems easily, VPSolver includes a [Python API](https://github.com/fdabrandao/vpsolver/wiki/Python-API), a modelling toolbox ([PyMPL](https://github.com/fdabrandao/pympl/)), and a [Web App](#vpsolver-web-app). VPSolver has been successfully compiled and run on Linux and Mac OS X. VPSolver also runs on a large variety of platforms including Windows using a [Docker container](#docker).
+![](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)
+[![Build Status](https://dev.azure.com/fdabrandao0236/vpsolver/_apis/build/status/fdabrandao.vpsolver?branchName=master)](https://dev.azure.com/fdabrandao0236/vpsolver/_build/latest?definitionId=1&branchName=master)
+
+For modelling other problems easily, VPSolver includes a [Python API](https://github.com/fdabrandao/vpsolver/wiki/Python-API), a modelling toolbox ([PyMPL](https://github.com/fdabrandao/pympl/)), and a [Web App](#vpsolver-web-app). VPSolver has been successfully compiled and run on Linux, macOS, and Windows. VPSolver can also be used in [Docker containers](#docker).
 
 For more details, please refer to the [project wiki](https://github.com/fdabrandao/vpsolver/wiki) or to the [manual](https://github.com/fdabrandao/vpsolver/tree/master/docs/vpsolver_manual.pdf).
 
 #### Repositories
-* Project Homepage: <http://vpsolver.dcc.fc.up.pt>
+* Project Homepage: <http://vpsolver.fdabrandao.pt>
 * GiHub repository: <https://github.com/fdabrandao/vpsolver>
 * BitBucket repository: <https://bitbucket.org/fdabrandao/vpsolver>
 * Docker repository: <https://hub.docker.com/r/fdabrandao/vpsolver>
 * PyPI repository: <https://pypi.python.org/pypi/pyvpsolver>
 
 ## Requirements
 #### Mandatory
 
-* MIP solver: Gurobi, CPLEX, GLPK, COIN-OR, SCIP, lp_solve, ...  
-* UNIX-like operating system or a UNIX-like environment such as [Cygwin](https://www.cygwin.com/)
-* `g++ >= 4.8`; `make >= 3.0`; `bash >= 3.0`
-      
-#### Optional
+- To use vpsolver scripts for various solvers:
+  * MIP solver: Gurobi, CPLEX, GLPK, COIN-OR, SCIP, lp_solve, ...
+  * UNIX-like operating system or a UNIX-like environment such as [Cygwin](https://www.cygwin.com/) on Windows
+  * `g++`, `clang`, or `Visual Studio`; `cmake >= 3.3`; `bash >= 3.0`
+
+- To build the vpsolver executable linked to Gurobi:
+  * `gurobi`
+  * `cmake >= 3.3`
 
+#### Optional
 For the [Python API](https://github.com/fdabrandao/vpsolver/wiki/Python-API) and Web App:
 
 * `python-2.7` or `python-3.x`
 * `python-pip`
 * `python-dev`
 * `glpk-utils`
  
 #### Platforms
 It has been successfully compiled and run on the following platforms:
 
 * **Linux**
-* **Mac OS X**
-* On a large variety of platforms including **Windows** using a [Docker container](#docker)
-* It also runs on **Windows** using [Cygwin](https://www.cygwin.com/) (a Unix-like environment and command-line interface)
+* **macOS**
+* **Windows** (note that vpsolver scripts require bash)
 
 ## Setup
 Without the python interface: 
 
 ```bash
-$ ./configure CXXFLAGS="" LDFLAGS=""
-$ make
-$ sudo make install
-```
-Note: In order to compile only the components that do not require Gurobi, use `./configure GUROBI_HOME=""`. In order to link the optional components that require Gurobi, the environment variable `$GUROBI_HOME` must be set, and some additional flags may also need to be set (e.g., `./configure LDFLAGS="-L${GUROBI_HOME}/lib/ -lgurobi_stdc++"`).
+$ mkdir build
+$ cd build/
+$ cmake ..
+$ cmake --build . --config Release
+```
+Note: In order to compile the components that require Gurobi, you need to have set the environment variable `GUROBI_HOME` or specify the location of the Gurobi installation in the third step:
+- Linux: `cmake .. -DGUROBI_DIR=/opt/gurobi952/linux64/`
+- macOS: `cmake .. -DGUROBI_DIR=/Library/gurobi952/macos_universal2/`
+- Windows: `cmake .. -DGUROBI_DIR=C:\\gurobi952\\win64`
 
 With the python interface: 
 
 ```
 $ pip install -r requirements.txt
 $ pip install . --upgrade
 $ cd examples; py.test -v --cov pyvpsolver
@@ -214,12 +216,12 @@
 Arc-flow Formulation with Graph Compression._ Technical Report DCC-2013-09,
 Faculdade de Ciências da Universidade do Porto, Universidade do Porto, Portugal. [arXiv:1502.02899](http://arxiv.org/abs/1502.02899).
 
 * [6] Brandão, F. (2012). _Bin Packing and Related Problems: Pattern-Based Approaches._ 
 Master’s thesis, Faculdade de Ciências da Universidade do Porto, Portugal.
 
 * [7] Computational results on several benchmark test data sets:  
-http://www.dcc.fc.up.pt/~fdabrandao/research/vpsolver/results/
+https://research.fdabrandao.pt/research/vpsolver/results/
 
 
 ***
-Copyright © 2013-2016 [Filipe Brandão](http://www.dcc.fc.up.pt/~fdabrandao/) < [fdabrandao@dcc.fc.up.pt](mailto:fdabrandao@dcc.fc.up.pt) >. All rights reserved.
+Copyright © 2013-2022 [Filipe Brandão](https://fdabrandao.pt) < [fdabrandao@gmail.com](mailto:fdabrandao@gmail.com) >. All rights reserved.
```

### Comparing `pyvpsolver-3.1.3/pyvpsolver/afgraph.py` & `pyvpsolver-3.1.4/pyvpsolver/afgraph.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,9 @@
 """
 This code is part of the Arc-flow Vector Packing Solver (VPSolver).
-
-Copyright (C) 2013-2016, Filipe Brandao
-Faculdade de Ciencias, Universidade do Porto
-Porto, Portugal. All rights reserved. E-mail: <fdabrandao@dcc.fc.up.pt>.
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU Affero General Public License as
-published by the Free Software Foundation, either version 3 of the
-License, or (at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU Affero General Public License for more details.
-
-You should have received a copy of the GNU Affero General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 from builtins import zip
 from builtins import map
 from builtins import range
 from builtins import sorted
 from builtins import object
 
@@ -45,17 +28,27 @@
         if self.LOSS is not None:
             self.LOSS = fa(self.LOSS)
         if self.S is not None:
             self.S = fv(self.S)
         if self.Ts is not None:
             self.Ts = [fv(t) for t in self.Ts]
 
-    def draw(self, svg_file, show_labels=False, ignore=None, back=None,
-             loss=None, weights=None, capacities=None, lpaths=False,
-             graph_attrs=None, verbose=False):
+    def draw(
+        self,
+        svg_file,
+        show_labels=False,
+        ignore=None,
+        back=None,
+        loss=None,
+        weights=None,
+        capacities=None,
+        lpaths=False,
+        graph_attrs=None,
+        verbose=False,
+    ):
         """Draw the arc-flow graph in .svg format."""
         V, A = self.V, self.A
         if loss is None:
             loss = self.LOSS
         if back is None:
             back = set((u, v) for (u, v, i) in self.A if v == self.S)
 
@@ -64,34 +57,36 @@
             assert capacities is not None
             lp_source = self.lpaths_source(weights, capacities)
             lp_targets = self.lpaths_targets(weights, capacities)
             newlabels = {
                 v: "{}:\nL({})\nU({})".format(
                     str(v),
                     ",".join(map(str, lp_source[v])),
-                    ",".join(map(str, lp_targets[v]))
+                    ",".join(map(str, lp_targets[v])),
                 )
                 for v in V
             }
             if ignore is not None:
                 ignore = [
-                    (newlabels.get(u, u), newlabels.get(v, v))
-                    for (u, v) in ignore
+                    (newlabels.get(u, u), newlabels.get(v, v)) for (u, v) in ignore
                 ]
             if back is not None:
-                back = [
-                    (newlabels.get(u, u), newlabels.get(v, v))
-                    for (u, v) in back
-                ]
+                back = [(newlabels.get(u, u), newlabels.get(v, v)) for (u, v) in back]
             V, A = relabel_graph(V, A, lambda v: newlabels.get(v, v))
 
         draw_graph(
-            svg_file, sort_vertices(V), sort_arcs(A),
-            show_labels=show_labels, ignore=ignore, back=back, loss=loss,
-            graph_attrs=graph_attrs, verbose=verbose
+            svg_file,
+            sort_vertices(V),
+            sort_arcs(A),
+            show_labels=show_labels,
+            ignore=ignore,
+            back=back,
+            loss=loss,
+            graph_attrs=graph_attrs,
+            verbose=verbose,
         )
 
     def vname(self, u, v, i, vnames=None):
         """Return the variable name attributed to the arc."""
         if vnames is None:
             vnames = self.names
         if (u, v, i) in vnames:
@@ -104,25 +99,25 @@
         """Compute longest paths to the source."""
         ndims = len(capacities[0])
         radj = {u: [] for u in self.V}
         for u, v, lbl in self.A:
             if v != self.S:
                 radj[v].append((u, lbl))
 
-        zero = tuple([0]*ndims)
-        minlabel = tuple([0]*ndims)
+        zero = tuple([0] * ndims)
+        minlabel = tuple([0] * ndims)
 
         def lp_source(u, labels):
             if u in labels:
                 return labels[u]
             lbl = minlabel
             for v, it in radj[u]:
                 wi = weights.get(it, zero)
                 vlbl = lp_source(v, labels)
-                lbl = tuple(max(lbl[d], vlbl[d]+wi[d]) for d in range(ndims))
+                lbl = tuple(max(lbl[d], vlbl[d] + wi[d]) for d in range(ndims))
             labels[u] = lbl
             return lbl
 
         labels = {}
         for t in self.Ts:
             lp_source(t, labels)
         return labels
@@ -131,25 +126,25 @@
         """Compute longest paths to the targets."""
         ndims = len(capacities[0])
         adj = {u: [] for u in self.V}
         for u, v, lbl in self.A:
             if v != self.S:
                 adj[u].append((v, lbl))
 
-        zero = tuple([0]*ndims)
-        maxlabel = tuple([inf]*ndims)
+        zero = tuple([0] * ndims)
+        maxlabel = tuple([inf] * ndims)
 
         def lp_targets(u, labels):
             if u in labels:
                 return labels[u]
             lbl = maxlabel
             for v, it in adj[u]:
                 wi = weights.get(it, zero)
                 vlbl = lp_targets(v, labels)
-                lbl = tuple(min(lbl[d], vlbl[d]-wi[d]) for d in range(ndims))
+                lbl = tuple(min(lbl[d], vlbl[d] - wi[d]) for d in range(ndims))
             labels[u] = lbl
             return lbl
 
         labels = {t: Wt for t, Wt in zip(self.Ts, capacities)}
         lp_targets(self.S, labels)
         return labels
 
@@ -241,15 +236,15 @@
                     patt += labels.get(arc, [])
                 solution.append((f, patt))
             else:
                 for v, arc in adj[u]:
                     # v != node_a to avoid cycles
                     if v != node_a and flow[arc] > 0:
                         ff = min(f, flow[arc])
-                        go(v, ff, path+[arc])
+                        go(v, ff, path + [arc])
                         f -= ff
 
         go(node_a, flow_limit, [])
 
         # group identical patterns
         rep = {}
         for (r, p) in solution:
```

### Comparing `pyvpsolver-3.1.3/pyvpsolver/solvers/mvpsolver2013.py` & `pyvpsolver-3.1.4/pyvpsolver/solvers/mvpsolver2013.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 """
 This code is part of the Arc-flow Vector Packing Solver (VPSolver).
-
-Copyright (C) 2013-2016, Filipe Brandao
-Faculdade de Ciencias, Universidade do Porto
-Porto, Portugal. All rights reserved. E-mail: <fdabrandao@dcc.fc.up.pt>.
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU Affero General Public License as
-published by the Free Software Foundation, either version 3 of the
-License, or (at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU Affero General Public License for more details.
-
-You should have received a copy of the GNU Affero General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 from __future__ import print_function
 from __future__ import division
 from builtins import zip
 from builtins import range
 
 import os
 import sys
 from .. import VPSolver, VBP, AFG
 from .. import AFGraph
 from pympl import Model
 
 
-def solve(Ws, Cs, Qs, ws, b, transitive_reduction=True,
-          svg_file="", lp_file="", mps_file="",
-          script=None, script_options=None, stats=None, verbose=None):
+def solve(
+    Ws,
+    Cs,
+    Qs,
+    ws,
+    b,
+    transitive_reduction=True,
+    svg_file="",
+    lp_file="",
+    mps_file="",
+    script=None,
+    script_options=None,
+    stats=None,
+    verbose=None,
+):
     """
     Solve multiple-choice vector bin packing instances
     using the method proposed in:
     Brandao, F. and Pedroso, J. P. (2013). Multiple-choice Vector
     Bin Packing: Arc-flow Formulation with Graph Compression. Technical Report
     DCC-2013-13, Faculdade de Ciencias da Universidade do Porto, Universidade
     do Porto, Portugal.
@@ -68,25 +63,23 @@
                 bbi[j] = 0
                 continue
         symb = "G{0}:".format(i)
         instances[i] = VBP(Ws[i], ww, bbi, verbose=False)
         graphs[i] = AFG(instances[i], verbose=verbose).graph()
         loss = graphs[i].LOSS
         graphs[i].relabel(
-            lambda u: "{0}{1}".format(symb, u),
-            lambda lbl: lbl if lbl != loss else LOSS
+            lambda u: "{0}{1}".format(symb, u), lambda lbl: lbl if lbl != loss else LOSS
         )
         Ss[i] = graphs[i].S
         Ts[i] = graphs[i].Ts[0]
         graphs[i].A.remove((Ts[i], Ss[i], LOSS))
         if svg_file.endswith(".svg"):
             try:
                 graphs[i].draw(
-                    svg_file.replace(".svg", "{0}.svg".format(i+1)),
-                    verbose=verbose
+                    svg_file.replace(".svg", "{0}.svg".format(i + 1)), verbose=verbose
                 )
             except Exception as e:
                 VPSolver.log(e, verbose)
 
     S, T = "S", "T"
     V = sum([g.V for g in graphs], [])
     A = sum([g.A for g in graphs], [])
@@ -106,26 +99,26 @@
     for (u, v, i) in A:
         adj[v].append((u, i))
 
     VPSolver.log("Final compression steps:", verbose)
 
     nv1, na1 = len(V), len(A)
     VPSolver.log("  #V1: {0} #A1: {1}".format(nv1, na1), verbose=stats)
-    zero = tuple([0]*ndims)
+    zero = tuple([0] * ndims)
 
     def compress(u):
         if u == S:
             return zero
         if u in newlbl:
             return newlbl[u]
         lbl = zero
         for v, i in adj[u]:
             wi = ww[i] if i != LOSS else zero
             vlbl = compress(v)
-            lbl = tuple(max(lbl[d], vlbl[d]+wi[d]) for d in range(ndims))
+            lbl = tuple(max(lbl[d], vlbl[d] + wi[d]) for d in range(ndims))
         newlbl[u] = lbl
         return lbl
 
     # Relabel the graph using the longest path from the source:
     newlbl = {}
     compress(T)
     newlbl[S] = S
@@ -143,17 +136,15 @@
         for (u, v, i) in graph.A:
             if isinstance(u, tuple):
                 if v in Ts:
                     if u not in tadj:
                         tadj[u] = []
                     tadj[u].append(Ts.index(v))
 
-        graph.A = [
-            (u, v, i) for (u, v, i) in graph.A if v not in Ts
-        ]
+        graph.A = [(u, v, i) for (u, v, i) in graph.A if v not in Ts]
         V, A = set(graph.V), set(graph.A)
 
         def fits(w1, w2):
             return all(x <= y for x, y in zip(w1, w2))
 
         dominatedby = {i: [] for i in range(nbtypes)}
         for i in range(nbtypes):
@@ -189,22 +180,22 @@
 
         graph.V, graph.A = V, A
 
     # Relabel the graph with indices:
     newlbl = {}
     for u in graph.get_vertices_sorted():
         if isinstance(u, tuple):
-            newlbl[u] = len(newlbl)+1
+            newlbl[u] = len(newlbl) + 1
     graph.relabel(lambda u: newlbl.get(u, u))
     V, A = graph.V, graph.A
 
     nv2, na2 = len(V), len(A)
     VPSolver.log("  #V2: {0} #A2: {1}".format(nv2, na2), verbose=stats)
-    VPSolver.log("  #V2/#V1 = {0:.2f}".format(nv2/nv1), verbose=stats)
-    VPSolver.log("  #A2/#A1 = {0:.2f}".format(na2/na1), verbose=stats)
+    VPSolver.log("  #V2/#V1 = {0:.2f}".format(nv2 / nv1), verbose=stats)
+    VPSolver.log("  #A2/#A1 = {0:.2f}".format(na2 / na1), verbose=stats)
 
     if svg_file.endswith(".svg"):
         try:
             graph.draw(svg_file.replace(".svg", ".final.svg"), verbose=verbose)
         except Exception as e:
             VPSolver.log(e, verbose)
 
@@ -217,24 +208,25 @@
             At.append((u, v, i))
             used.add((u, v, k))
     A = At
     graph = AFGraph(V, A, S, [T], LOSS)
 
     nv3, na3 = len(V), len(A)
     VPSolver.log("  #V3: {0} #A3: {1}".format(nv3, na3), verbose=stats)
-    VPSolver.log("  #V3/#V1 = {0:.2f}".format(nv3/nv1), verbose=stats)
-    VPSolver.log("  #A3/#A1 = {0:.2f}".format(na3/na1), verbose=stats)
+    VPSolver.log("  #V3/#V1 = {0:.2f}".format(nv3 / nv1), verbose=stats)
+    VPSolver.log("  #A3/#A1 = {0:.2f}".format(na3 / na1), verbose=stats)
 
     # Generate the model:
     varl, cons = graph.get_flow_cons()
     assocs = graph.get_assocs()
     for i in range(len(b)):
         lincomb = [
             (var, 1)
-            for it, (j, t) in enumerate(itlabel) if j == i
+            for it, (j, t) in enumerate(itlabel)
+            if j == i
             for var in assocs[it]
         ]
         if b[i] > 1:
             cons.append((lincomb, ">=", b[i]))
         else:
             cons.append((lincomb, "=", b[i]))
 
@@ -274,18 +266,15 @@
     out, varvalues = VPSolver.script_wsol(script, model_file, verbose=verbose)
     os.remove(model_file)
 
     VPSolver.log("#V1: {0} #A1: {1}".format(nv1, na1), verbose)
     VPSolver.log("#V2: {0} #A2: {1}".format(nv2, na2), verbose)
     VPSolver.log("#V3: {0} #A3: {1}".format(nv3, na3), verbose)
     VPSolver.log(
-        "#V3/#V1: {0:.2f} #A3/#A1: {1:.2f}".format(
-            nv3/nv1, na3/na1
-        ),
-        verbose
+        "#V3/#V1: {0:.2f} #A3/#A1: {1:.2f}".format(nv3 / nv1, na3 / na1), verbose
     )
 
     labels = {}
     for (u, v, i) in A:
         if i != LOSS:
             labels[u, v, i] = [itlabel[i]]
 
@@ -293,18 +282,17 @@
     graph.set_flow(varvalues)
     graph.set_labels(labels)
     for i in range(nbtypes):
         lst_sol.append(graph.extract_solution(S, "<-", Ts[i]))
 
     validate_solution(lst_sol, nbtypes, ndims, Ws, ws, b)
 
-    c1 = sum(sum(r for r, patt in lst_sol[i])*Cs[i] for i in range(nbtypes))
+    c1 = sum(sum(r for r, patt in lst_sol[i]) * Cs[i] for i in range(nbtypes))
     c2 = sum(
-        varvalues.get(graph.vname(Ts[i], T, LOSS), 0) * Cs[i]
-        for i in range(nbtypes)
+        varvalues.get(graph.vname(Ts[i], T, LOSS), 0) * Cs[i] for i in range(nbtypes)
     )
     assert c1 == c2
 
     return c1, lst_sol
 
 
 def validate_solution(lst_solutions, nbtypes, ndims, Ws, ws, b):
@@ -334,16 +322,21 @@
     else:
         obj, lst_sol = solution, arg2
     if obj is not None:
         print("Objective:", obj, file=fout)
     print("Solution:", file=fout)
     for i, sol in enumerate(lst_sol):
         cnt = sum(m for m, p in sol)
-        print("Bins of type {0}: {1} {2}".format(
-            i+i0, cnt, ["bins", "bin"][cnt == 1]
-        ), file=fout)
+        print(
+            "Bins of type {0}: {1} {2}".format(i + i0, cnt, ["bins", "bin"][cnt == 1]),
+            file=fout,
+        )
         for mult, patt in sol:
-            print("{0} x [{1}]".format(
-                mult, ", ".join(
-                    ["i={0} opt={1}".format(it+i0, opt+i0) for it, opt in patt]
-                )
-            ), file=fout)
+            print(
+                "{0} x [{1}]".format(
+                    mult,
+                    ", ".join(
+                        ["i={0} opt={1}".format(it + i0, opt + i0) for it, opt in patt]
+                    ),
+                ),
+                file=fout,
+            )
```

### Comparing `pyvpsolver-3.1.3/pyvpsolver/solvers/mvpsolver2016.py` & `pyvpsolver-3.1.4/pyvpsolver/solvers/mvpsolver2016.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,9 @@
 """
 This code is part of the Arc-flow Vector Packing Solver (VPSolver).
-
-Copyright (C) 2013-2016, Filipe Brandao
-Faculdade de Ciencias, Universidade do Porto
-Porto, Portugal. All rights reserved. E-mail: <fdabrandao@dcc.fc.up.pt>.
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU Affero General Public License as
-published by the Free Software Foundation, either version 3 of the
-License, or (at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU Affero General Public License for more details.
-
-You should have received a copy of the GNU Affero General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 from __future__ import print_function
 
 import sys
 from .. import VPSolver, MVP, AFG, MPS
```

### Comparing `pyvpsolver-3.1.3/pyvpsolver/utils.py` & `pyvpsolver-3.1.4/pyvpsolver/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,9 @@
 """
 This code is part of the Arc-flow Vector Packing Solver (VPSolver).
-
-Copyright (C) 2013-2016, Filipe Brandao
-Faculdade de Ciencias, Universidade do Porto
-Porto, Portugal. All rights reserved. E-mail: <fdabrandao@dcc.fc.up.pt>.
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU Affero General Public License as
-published by the Free Software Foundation, either version 3 of the
-License, or (at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU Affero General Public License for more details.
-
-You should have received a copy of the GNU Affero General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 from __future__ import print_function
 from __future__ import division
 from builtins import zip
 from builtins import str
 from builtins import map
 from builtins import range
@@ -74,45 +57,58 @@
 def sort_arcs(A, reverse=False):
     """Return the list of arcs sorted."""
     return sorted(
         A, key=lambda a: tuple((repr(type(k)), k) for k in a), reverse=reverse
     )
 
 
-def draw_graph(svg_file, V, A, show_labels=False, ignore=None, back=None,
-               loss=None, graph_attrs=None, verbose=False):
+def draw_graph(
+    svg_file,
+    V,
+    A,
+    show_labels=False,
+    ignore=None,
+    back=None,
+    loss=None,
+    graph_attrs=None,
+    verbose=False,
+):
     """Draw an arc-flow graph in .svg format."""
     from pygraphviz.agraph import AGraph
+
     if ignore is None:
         ignore = []
     if back is None:
         back = []
     if loss is None:
         loss = []
     elif not isinstance(loss, (tuple, list)):
         loss = [loss]
     g = AGraph(
-        rankdir="LR", directed=True, bgcolor="white",
-        ranksep="1.0", nodesep="0.10",
-        strict=False
+        rankdir="LR",
+        directed=True,
+        bgcolor="white",
+        ranksep="1.0",
+        nodesep="0.10",
+        strict=False,
     )
     if graph_attrs is not None:
         for attr, value in graph_attrs.items():
             g.graph_attr[attr] = value
     g.node_attr["shape"] = "ellipse"
     g.node_attr["color"] = "black"
     g.node_attr["fontcolor"] = "black"
     g.node_attr["penwidth"] = "2.0"
 
     lbls = sorted(
         set(i for (u, v, i) in A if i not in loss),
-        key=lambda lbl: (repr(type(lbl)), lbl)
+        key=lambda lbl: (repr(type(lbl)), lbl),
     )
 
-    colors = Colors.uniquecolors(len(lbls)+1, v=0.5, p=0.0)
+    colors = Colors.uniquecolors(len(lbls) + 1, v=0.5, p=0.0)
 
     used = set()
     for (u, v, i) in A:
         if (u, v) in ignore:
             continue
         used.add(u)
         used.add(v)
@@ -143,23 +139,22 @@
     Based on code from StackOverflow: http://stackoverflow.com/a/2142206
     """
 
     @staticmethod
     def rgbcode(t):
         """Convert (r, g, b) tuples to hexadecimal."""
         r, g, b = t
-        r = int(r*255)
-        g = int(g*255)
-        b = int(b*255)
+        r = int(r * 255)
+        g = int(g * 255)
+        b = int(b * 255)
         return "#{0:0>2x}{1:0>2x}{2:0>2x}".format(r, g, b)
 
     @staticmethod
     def rgbcolor(h, f, v, p):
-        """Convert colors specified by h-value and f-value to RGB three-tuples.
-        """
+        """Convert colors specified by h-value and f-value to RGB three-tuples."""
         # q = 1 - f
         # t = f
         if h == 0:
             return v, f, p
         elif h == 1:
             return 1 - f, v, p
         elif h == 2:
@@ -172,14 +167,12 @@
             return v, p, 1 - f
 
     @staticmethod
     def uniquecolors(n, v=0.5, p=0.0):
         """Generate a list of distinct colors, each of which is
         represented as an RGB three-tuple."""
         import math
-        hues = list(360.0/n*i for i in range(n))
-        hs = list(math.floor(hue/60) % 6 for hue in hues)
-        fs = list((hue/60) % 1 for hue in hues)
-        return [
-            Colors.rgbcode(Colors.rgbcolor(h, f, v, p))
-            for h, f in zip(hs, fs)
-        ]
+
+        hues = list(360.0 / n * i for i in range(n))
+        hs = list(math.floor(hue / 60) % 6 for hue in hues)
+        fs = list((hue / 60) % 1 for hue in hues)
+        return [Colors.rgbcode(Colors.rgbcolor(h, f, v, p)) for h, f in zip(hs, fs)]
```

### Comparing `pyvpsolver-3.1.3/pyvpsolver/vpsolver.py` & `pyvpsolver-3.1.4/pyvpsolver/vpsolver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,9 @@
 """
 This code is part of the Arc-flow Vector Packing Solver (VPSolver).
-
-Copyright (C) 2013-2016, Filipe Brandao
-Faculdade de Ciencias, Universidade do Porto
-Porto, Portugal. All rights reserved. E-mail: <fdabrandao@dcc.fc.up.pt>.
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU Affero General Public License as
-published by the Free Software Foundation, either version 3 of the
-License, or (at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU Affero General Public License for more details.
-
-You should have received a copy of the GNU Affero General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 from __future__ import print_function
 from builtins import zip
 from builtins import str
 from builtins import map
 from builtins import range
 from builtins import object
@@ -45,16 +28,16 @@
     def __init__(self, W, w, b, binary=False, vtype="I", verbose=False):
         self.vbp_file = VPSolver.new_tmp_file(".vbp")
         with open(self.vbp_file, "w") as fdst:
             print(len(W), file=fdst)  # ndims
             print(" ".join(map(str, W)), file=fdst)  # W
             print(len(w), file=fdst)  # m
             for i in range(len(w)):  # items
-                row = list(w[i])+[b[i]]
-                assert len(row) == len(W)+1
+                row = list(w[i]) + [b[i]]
+                assert len(row) == len(W) + 1
                 print(" ".join(map(str, row)), file=fdst)
             print("BINARY{{{:d}}};".format(binary), file=fdst)
             print("VTYPE{{{}}};".format(vtype), file=fdst)
         if verbose:
             print(utils.get_content(self.vbp_file))
         self.m = len(b)
         self.ndims = len(W)
@@ -105,28 +88,27 @@
 
 
 class MVP(object):
     """
     Wrapper for .mvp files.
     """
 
-    def __init__(
-            self, Ws, Cs, Qs, ws, b, binary=False, vtype="I", verbose=False):
+    def __init__(self, Ws, Cs, Qs, ws, b, binary=False, vtype="I", verbose=False):
         self.mvp_file = VPSolver.new_tmp_file(".mvp")
         with open(self.mvp_file, "w") as fdst:
             ndims = len(Ws[0])
             print(ndims, file=fdst)  # ndims
             print(len(Ws), file=fdst)  # nbtypes
             assert len(Ws) == len(Cs)
             assert len(Ws) == len(Qs)
             for Wi, Ci, Qi in zip(Ws, Cs, Qs):  # Ws, Cs, Qs
                 assert len(Wi) == ndims
                 if Qi == utils.inf:
                     Qi = -1
-                print(" ".join(map(str, list(Wi)+[Ci]+[Qi])), file=fdst)
+                print(" ".join(map(str, list(Wi) + [Ci] + [Qi])), file=fdst)
             assert len(ws) == len(b)
             print(len(ws), file=fdst)  # m
             for i in range(len(ws)):  # items
                 print("{} {}".format(len(ws[i]), b[i]), file=fdst)
                 for j, w in enumerate(ws[i]):
                     assert len(w) == ndims
                     print(" ".join(map(str, w)), file=fdst)
@@ -137,17 +119,15 @@
         self.m = len(b)
         self.ndims = ndims
         self.binary = binary
         self.vtype = vtype
         self.Ws, self.Cs, self.Qs = Ws, Cs, Qs
         self.ws, self.b = ws, b
         self.labels = [
-            (i, j)
-            for i in range(len(self.ws))
-            for j in range(len(self.ws[i]))
+            (i, j) for i in range(len(self.ws)) for j in range(len(self.ws[i]))
         ]
 
     @classmethod
     def from_str(cls, content, verbose=False):
         lst = utils.get_instance_data(content)
         ndims = lst.pop(0)
         nbtypes = lst.pop(0)
@@ -206,17 +186,15 @@
     """
 
     def __init__(self, instance, verbose=None):
         if instance is not None:
             assert isinstance(instance, (VBP, MVP))
             self.instance = instance
             self.afg_file = VPSolver.new_tmp_file(".afg")
-            self.output = VPSolver.vbp2afg(
-                instance, self.filename, verbose=verbose
-            )
+            self.output = VPSolver.vbp2afg(instance, self.filename, verbose=verbose)
 
     @classmethod
     def from_file(cls, afg_file, verbose=None):
         obj = cls(None)
         obj.instance = MVP.from_file(afg_file)
         obj.afg_file = VPSolver.new_tmp_file(".afg")
         shutil.copyfile(afg_file, obj.afg_file)
@@ -228,39 +206,43 @@
         labels = self.instance.labels
         S = int(utils.get_opt("S", content))
         Ts = list(map(int, utils.get_opt("Ts", content).split(",")))
         arcs = list(map(int, utils.get_opt("ARCS", content).split()))
         LOSS = int(utils.get_opt("LOSS", content))
         V, A = set([]), []
         for i in range(0, len(arcs), 3):
-            u, v, i = arcs[i:i+3]
+            u, v, i = arcs[i : i + 3]
             V.add(u)
             V.add(v)
             A.append((u, v, labels[i] if i != LOSS else LOSS))
         graph = AFGraph(V, A, S, Ts, LOSS)
         lbls = {S: "S"}
         if len(Ts) == 1:
             lbls[Ts[0]] = "T"
         else:
-            for t, new in zip(Ts, ["T{}".format(i+1) for i in range(len(Ts))]):
+            for t, new in zip(Ts, ["T{}".format(i + 1) for i in range(len(Ts))]):
                 lbls[t] = new
         graph.relabel(lambda u: lbls.get(u, u))
         return graph
 
     def draw(self, svg_file, lpaths=False, graph_attrs=None, verbose=False):
         """Draw the arc-flow graph in .svg format."""
         if lpaths:
             weights = self.instance.weights()
             capacities = self.instance.capacities()
         else:
             weights = None
             capacities = None
         self.graph().draw(
-            svg_file, weights=weights, capacities=capacities, lpaths=lpaths,
-            graph_attrs=graph_attrs, verbose=verbose
+            svg_file,
+            weights=weights,
+            capacities=capacities,
+            lpaths=lpaths,
+            graph_attrs=graph_attrs,
+            verbose=verbose,
         )
 
     @property
     def filename(self):
         """Return the filename."""
         return self.afg_file
 
@@ -276,17 +258,15 @@
     Wrapper for .mps files.
     """
 
     def __init__(self, graph, verbose=None):
         assert isinstance(graph, AFG)
         self.afg_graph = graph
         self.mps_file = VPSolver.new_tmp_file(".mps")
-        self.output = VPSolver.afg2mps(
-            graph.filename, self.filename, verbose=verbose
-        )
+        self.output = VPSolver.afg2mps(graph.filename, self.filename, verbose=verbose)
 
     @property
     def filename(self):
         """Return the filename."""
         return self.mps_file
 
     def __del__(self):
@@ -301,17 +281,15 @@
     Wrapper for .lp files.
     """
 
     def __init__(self, graph, verbose=None):
         assert isinstance(graph, AFG)
         self.afg_graph = graph
         self.lp_file = VPSolver.new_tmp_file(".lp")
-        self.output = VPSolver.afg2lp(
-            graph.filename, self.filename, verbose=verbose
-        )
+        self.output = VPSolver.afg2lp(graph.filename, self.filename, verbose=verbose)
 
     @property
     def filename(self):
         """Return the filename."""
         return self.lp_file
 
     def __del__(self):
@@ -379,18 +357,19 @@
     @staticmethod
     def run(cmd, tee=None, grep=None, grepv=None, verbose=None):
         """Run a system command."""
         if verbose is None:
             verbose = VPSolver.VERBOSE
 
         proc = subprocess.Popen(
-            cmd, shell=True,
+            cmd,
+            shell=True,
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
-            preexec_fn=os.setsid
+            preexec_fn=os.setsid,
         )
         VPSolver.PLIST.append(proc)
 
         def pipe_output(fin, fout_list, grep=None, grepv=None):
             while True:
                 line = fin.readline().decode("utf-8")
                 if not line:
@@ -421,36 +400,32 @@
             raise RuntimeError("failed to run '{}'".format(cmd))
 
     @staticmethod
     def parse_vbpsol(vpsol_output):
         """Transform 'vbpsol' solutions into python data."""
         marker = "PYSOL="
         if marker in vpsol_output:
-            vpsol_output = vpsol_output[vpsol_output.find(marker)+len(marker):]
-            vpsol_output = vpsol_output[:vpsol_output.find("\n")]
+            vpsol_output = vpsol_output[vpsol_output.find(marker) + len(marker) :]
+            vpsol_output = vpsol_output[: vpsol_output.find("\n")]
             obj, sol = eval(vpsol_output)
             return obj, sol
         else:
             return None
 
     @staticmethod
     def vbpsol(afg_file, sol_file, print_inst=False, pyout=True, verbose=None):
         """Call 'vbpsol' to extract a vector packing solution."""
         if isinstance(afg_file, AFG):
             afg_file = afg_file.filename
         out_file = VPSolver.new_tmp_file()
-        opts = "{print_inst:d} {pyout:d}".format(
-            print_inst=print_inst, pyout=pyout
-        )
+        opts = "{print_inst:d} {pyout:d}".format(print_inst=print_inst, pyout=pyout)
         VPSolver.run(
-            "{} {} {} {}".format(
-                VPSolver.VBPSOL_EXEC, afg_file, sol_file, opts
-            ),
+            "{} {} {} {}".format(VPSolver.VBPSOL_EXEC, afg_file, sol_file, opts),
             tee=out_file,
-            verbose=verbose
+            verbose=verbose,
         )
         output = utils.get_content(out_file)
         os.remove(out_file)
         return VPSolver.parse_vbpsol(output)
 
     @staticmethod
     def vpsolver(instance_file, print_inst=False, pyout=True, verbose=None):
@@ -459,87 +434,85 @@
             instance_file = instance_file.filename
         content = utils.get_content(instance_file)
         method = int(utils.get_opt("METHOD", content, -3))
         binary = int(utils.get_opt("BINARY", content, 0))
         vtype = utils.get_opt("VTYPE", content, "I")
         out_file = VPSolver.new_tmp_file()
         opts = "{method:d} {binary:d} {vtype} {print_inst:d} {pyout:d}".format(
-            method=method, binary=binary, vtype=vtype,
-            print_inst=print_inst, pyout=pyout
+            method=method,
+            binary=binary,
+            vtype=vtype,
+            print_inst=print_inst,
+            pyout=pyout,
         )
         VPSolver.run(
             "{} {} {}".format(VPSolver.VPSOLVER_EXEC, instance_file, opts),
             tee=out_file,
-            verbose=verbose
+            verbose=verbose,
         )
         output = utils.get_content(out_file)
         os.remove(out_file)
         return output, VPSolver.parse_vbpsol(output)
 
     @staticmethod
     def vbp2afg(instance_file, afg_file, opts="", verbose=None):
         """Call 'vbp2afg' to create an arc-flow graph for a .vbp instance."""
         if isinstance(instance_file, (VBP, MVP)):
             instance_file = instance_file.filename
         out_file = VPSolver.new_tmp_file()
         VPSolver.run(
-            "{} {} {} {}".format(
-                VPSolver.VBP2AFG_EXEC, instance_file, afg_file, opts
-            ),
+            "{} {} {} {}".format(VPSolver.VBP2AFG_EXEC, instance_file, afg_file, opts),
             tee=out_file,
-            verbose=verbose
+            verbose=verbose,
         )
         output = utils.get_content(out_file)
         os.remove(out_file)
         return output
 
     @staticmethod
     def afg2mps(afg_file, mps_file, opts="", verbose=None):
         """Call 'afg2mps' to create a .mps model for an arc-flow graph."""
         if isinstance(afg_file, AFG):
             afg_file = afg_file.filename
         out_file = VPSolver.new_tmp_file()
         VPSolver.run(
-            "{} {} {} {}".format(
-                VPSolver.AFG2MPS_EXEC, afg_file, mps_file, opts
-            ),
+            "{} {} {} {}".format(VPSolver.AFG2MPS_EXEC, afg_file, mps_file, opts),
             tee=out_file,
-            verbose=verbose
+            verbose=verbose,
         )
         output = utils.get_content(out_file)
         os.remove(out_file)
         return output
 
     @staticmethod
     def afg2lp(afg_file, lp_file, opts="", verbose=None):
         """Call 'afg2lp' to create a .lp model for an arc-flow graph."""
         if isinstance(afg_file, AFG):
             afg_file = afg_file.filename
         out_file = VPSolver.new_tmp_file()
         VPSolver.run(
-            "{} {} {} {}".format(
-                VPSolver.AFG2LP_EXEC, afg_file, lp_file, opts
-            ),
+            "{} {} {} {}".format(VPSolver.AFG2LP_EXEC, afg_file, lp_file, opts),
             tee=out_file,
-            verbose=verbose
+            verbose=verbose,
         )
         output = utils.get_content(out_file)
         os.remove(out_file)
         return output
 
     @staticmethod
     def afg2svg(afg_file, svg_file, verbose=None):
         """Draw a .afg arc-flow graph in .svg format."""
         if isinstance(afg_file, AFG):
             afg_file = afg_file.filename
         AFG.from_file(afg_file).draw(svg_file)
 
     @staticmethod
-    def script(script_name, arg1=None, arg2=None, options=None, pyout=True,
-               verbose=None):
+    def script(
+        script_name, arg1=None, arg2=None, options=None, pyout=True, verbose=None
+    ):
         """Call a VPSolver script and return a vector packing solution."""
         cmd = script_name
         for arg in [arg1, arg2]:
             if isinstance(arg, MPS):
                 cmd += " --mps {}".format(arg.filename)
             elif isinstance(arg, LP):
                 cmd += " --lp {}".format(arg.filename)
@@ -559,39 +532,40 @@
                 elif arg.endswith(".vbp"):
                     cmd += " --vbp {}".format(arg)
                 elif arg.endswith(".mvp"):
                     cmd += " --mvp {}".format(arg)
                 else:
                     raise Exception("Invalid file extension!")
         if options is not None:
-            cmd += " --options \"{}\"".format(options)
+            cmd += ' --options "{}"'.format(options)
         if pyout is True:
             cmd += " --pyout"
         out_file = VPSolver.new_tmp_file()
         VPSolver.run(cmd, tee=out_file, verbose=verbose)
         output = utils.get_content(out_file)
         os.remove(out_file)
         return output, VPSolver.parse_vbpsol(output)
 
     @staticmethod
     def script_wsol(script_name, model, options=None, verbose=None):
         """Call a solver script and return the solution."""
         from pympl import Tools
+
         if verbose is None:
             verbose = VPSolver.VERBOSE
         if isinstance(model, (LP, MPS)):
             model = model.filename
         return Tools.script(
-            script_name=script_name, model=model, options=options,
-            verbose=verbose
+            script_name=script_name, model=model, options=options, verbose=verbose
         )
 
 
 def signal_handler(signal_, frame):
     """Signal handler for a cleaner exit."""
     print("signal received: {}".format(signal_))
     VPSolver.clear()
     sys.exit(1)
 
+
 signal.signal(signal.SIGINT, signal_handler)
 signal.signal(signal.SIGHUP, signal_handler)
 signal.signal(signal.SIGTERM, signal_handler)
```

### Comparing `pyvpsolver-3.1.3/pyvpsolver/webapp/app.py` & `pyvpsolver-3.1.4/pyvpsolver/webapp/app.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,10 @@
 #!/usr/bin/env python
 """
 This code is part of the Arc-flow Vector Packing Solver (VPSolver).
-
-Copyright (C) 2013-2016, Filipe Brandao
-Faculdade de Ciencias, Universidade do Porto
-Porto, Portugal. All rights reserved. E-mail: <fdabrandao@dcc.fc.up.pt>.
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU Affero General Public License as
-published by the Free Software Foundation, either version 3 of the
-License, or (at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU Affero General Public License for more details.
-
-You should have received a copy of the GNU Affero General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 from __future__ import print_function
 from builtins import str
 from builtins import object
 
 import os
 import sys
@@ -58,15 +41,16 @@
 
 
 @app.route("/favicon.ico")
 def favicon():
     """Favicon route."""
     return flask.send_from_directory(
         os.path.join(app.root_path, "static"),
-        "favicon.ico", mimetype='image/vnd.microsoft.icon'
+        "favicon.ico",
+        mimetype="image/vnd.microsoft.icon",
     )
 
 
 @app.route("/")
 def index():
     """Render the index page."""
     return redirect(url_for("vbp"))
@@ -80,17 +64,15 @@
 
 @app.route("/vbp/", defaults={"example": None})
 @app.route("/vbp/<example>")
 def vbp(example):
     """Render the input page for VBP."""
     title = "Vector Packing"
 
-    example_folder = os.path.join(
-        os.path.dirname(__file__), "data", "examples", "vbp"
-    )
+    example_folder = os.path.join(os.path.dirname(__file__), "data", "examples", "vbp")
     examples = [
         ("/vbp/", "", None),
         ("/vbp/bpp", "BPP", "bpp.vbp"),
         ("/vbp/csp", "CSP", "csp.vbp"),
         ("/vbp/vbp", "VBP", "vbp.vbp"),
     ]
 
@@ -122,17 +104,15 @@
 
 @app.route("/mvp/", defaults={"example": None})
 @app.route("/mvp/<example>")
 def mvp(example):
     """Render the input page for MVP."""
     title = "Multiple-choice Vector Packing"
 
-    example_folder = os.path.join(
-        os.path.dirname(__file__), "data", "examples", "mvp"
-    )
+    example_folder = os.path.join(os.path.dirname(__file__), "data", "examples", "mvp")
     examples = [
         ("/mvp/", "", None),
         ("/mvp/vsbpp", "VSBPP", "vsbpp.mvp"),
         ("/mvp/mvp", "MVP", "mvp.mvp"),
     ]
 
     input_data = ""
@@ -169,14 +149,15 @@
         """Signal handler for cleaner exit."""
         for p in VPSolver.PLIST:
             try:
                 os.killpg(p.pid, signal.SIGTERM)
             except Exception as e:
                 pass
         sys.exit(0)
+
     signal.signal(signal.SIGTERM, signal_handler)
 
     sys.stdout = output
     sys.stderr = output
     input_ = form["input"].strip("\n")
     if DEBUG:
         print("Input:\n{0}\n\nOutput:".format(input_))
@@ -234,26 +215,25 @@
 
 
 @app.route("/solve/<app_name>", methods=["POST"])
 def solve(app_name):
     """Render the solver page."""
     try:
         args = (app_name, request.method, request.form, request.args)
-        return Response(
-            IterativeOutput(solve_worker, args), mimetype="text/plain"
-        )
+        return Response(IterativeOutput(solve_worker, args), mimetype="text/plain")
     except Exception as e:
         return json.dumps({"error": str(e)})
     finally:
         pass
 
 
 def get_ip_address():
     """Return the ip address of 'eth0'."""
     import socket
+
     s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     s.connect(("8.8.8.8", 80))
     return s.getsockname()[0]
 
 
 if __name__ == "__main__":
     print("URL: http://{0}:{1}/".format(get_ip_address(), PORT))
```

### Comparing `pyvpsolver-3.1.3/pyvpsolver/webapp/data/examples/vbp/vbp.vbp` & `pyvpsolver-3.1.4/pyvpsolver/webapp/data/examples/vbp/vbp.vbp`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/css/bootstrap-theme-readable.css` & `pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/css/bootstrap-theme-readable.css`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/css/bootstrap-theme.css` & `pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/css/bootstrap-theme.css.map` & `pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/css/bootstrap-theme.min.css` & `pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/css/bootstrap.css` & `pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/css/bootstrap.css.map` & `pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/css/bootstrap.min.css` & `pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/fonts/glyphicons-halflings-regular.eot` & `pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/fonts/glyphicons-halflings-regular.svg` & `pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/fonts/glyphicons-halflings-regular.ttf` & `pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/fonts/glyphicons-halflings-regular.woff` & `pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/fonts/glyphicons-halflings-regular.woff2` & `pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/js/bootstrap.js` & `pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/pyvpsolver/webapp/static/bootstrap/js/bootstrap.min.js` & `pyvpsolver-3.1.4/pyvpsolver/webapp/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/pyvpsolver/webapp/static/css/bootstrap.min.css` & `pyvpsolver-3.1.4/pyvpsolver/webapp/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/pyvpsolver/webapp/static/favicon.ico` & `pyvpsolver-3.1.4/pyvpsolver/webapp/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/pyvpsolver/webapp/static/js/app.js` & `pyvpsolver-3.1.4/pyvpsolver/webapp/static/js/app.js`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/pyvpsolver/webapp/static/js/jquery-1.11.2.js` & `pyvpsolver-3.1.4/pyvpsolver/webapp/static/js/jquery-1.11.2.js`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/pyvpsolver/webapp/static/js/jquery-1.11.2.min.map` & `pyvpsolver-3.1.4/pyvpsolver/webapp/static/js/jquery-1.11.2.min.map`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/pyvpsolver/webapp/templates/input.html` & `pyvpsolver-3.1.4/pyvpsolver/webapp/templates/input.html`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/setup.py` & `pyvpsolver-3.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,14 +80,25 @@
         "src/instance.cpp", "src/graph.cpp",
         "src/arcflow.cpp", "src/common.cpp"
     ],
     extra_compile_args=compile_args(),
     undef_macros=['NDEBUG'],
 )
 
+_afg2ampl = Extension(
+    "_afg2ampl",
+    sources=[
+        "swig/afg2ampl_wrap.cxx", "src/afg2ampl.cpp",
+        "src/instance.cpp", "src/graph.cpp",
+        "src/arcflow.cpp", "src/common.cpp"
+    ],
+    extra_compile_args=compile_args(),
+    undef_macros=['NDEBUG'],
+)
+
 _afg2lp = Extension(
     "_afg2lp",
     sources=[
         "swig/afg2lp_wrap.cxx", "src/afg2lp.cpp",
         "src/instance.cpp", "src/graph.cpp",
         "src/arcflow.cpp", "src/common.cpp"
     ],
@@ -122,17 +133,17 @@
 with open("pyvpsolver/__init__.py", "rb") as f:
     version = str(ast.literal_eval(_version_re.search(
         f.read().decode("utf-8")).group(1)))
 
 setup(
     name="pyvpsolver",
     version=version,
-    license="AGPLv3+",
+    license="BSD-3",
     author="Filipe Brandao",
-    author_email="fdabrandao@dcc.fc.up.pt",
+    author_email="fdabrandao@gmail.com",
     maintainer='Filipe Brandao',
     maintainer_email='fdabrandao@gmail.com',
     url="https://github.com/fdabrandao/vpsolver",
     description="Arc-flow Vector Packing Solver (VPSolver)",
     long_description=__doc__,
     packages=["pyvpsolver"],
     package_data={"": ls_dir("pyvpsolver/")},
@@ -140,12 +151,12 @@
     scripts=[os.path.join("scripts", f) for f in ls_dir("scripts/")],
     install_requires=open("requirements.txt").read().split("\n"),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
+        "License :: OSI Approved :: BSD License",
         "Topic :: Scientific/Engineering"
     ],
-    ext_modules=[_vbp2afg, _afg2lp, _afg2mps, _vbpsol],
+    ext_modules=[_vbp2afg, _afg2ampl, _afg2lp, _afg2mps, _vbpsol],
 )
```

### Comparing `pyvpsolver-3.1.3/src/config.hpp` & `pyvpsolver-3.1.4/src/config.hpp`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/swig/afg2lp_wrap.cxx` & `pyvpsolver-3.1.4/swig/afg2lp_wrap.cxx`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/swig/afg2mps_wrap.cxx` & `pyvpsolver-3.1.4/swig/afg2mps_wrap.cxx`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/swig/vbp2afg_wrap.cxx` & `pyvpsolver-3.1.4/swig/vbp2afg_wrap.cxx`

 * *Files identical despite different names*

### Comparing `pyvpsolver-3.1.3/swig/vbpsol_wrap.cxx` & `pyvpsolver-3.1.4/swig/vbpsol_wrap.cxx`

 * *Files identical despite different names*

