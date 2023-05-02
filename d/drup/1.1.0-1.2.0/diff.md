# Comparing `tmp/drup-1.1.0.tar.gz` & `tmp/drup-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drup-1.1.0.tar", last modified: Wed Apr 19 14:24:29 2023, max compression
+gzip compressed data, was "drup-1.2.0.tar", last modified: Sun Apr 30 00:08:06 2023, max compression
```

## Comparing `drup-1.1.0.tar` & `drup-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 14:24:29.025900 drup-1.1.0/
--rw-rw-r--   0 root         (0) root         (0)     1072 2023-04-16 13:21:59.000000 drup-1.1.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       69 2023-04-16 18:45:20.000000 drup-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7194 2023-04-19 14:24:29.025705 drup-1.1.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     6474 2023-04-19 14:21:56.000000 drup-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 14:24:29.016339 drup-1.1.0/drup.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     7194 2023-04-19 14:24:29.000000 drup-1.1.0/drup.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      280 2023-04-19 14:24:29.000000 drup-1.1.0/drup.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-04-19 14:24:29.000000 drup-1.1.0/drup.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-04-19 14:24:29.000000 drup-1.1.0/drup.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)        5 2023-04-19 14:24:29.000000 drup-1.1.0/drup.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      777 2023-04-19 13:50:15.000000 drup-1.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 14:24:29.026050 drup-1.1.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1215 2023-04-19 14:21:56.000000 drup-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 14:24:29.012321 drup-1.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 14:24:29.025257 drup-1.1.0/src/drup/
--rw-rw-r--   0 root         (0) root         (0)      456 2023-04-19 13:50:15.000000 drup-1.1.0/src/drup/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1295 2023-04-19 14:21:56.000000 drup-1.1.0/src/drup/cli.py
--r-xr-xr-x   0 root         (0) root         (0)  2098368 2023-04-19 14:24:29.000000 drup-1.1.0/src/drup/librupchecker.so
--rw-rw-r--   0 root         (0) root         (0)     3956 2023-04-19 13:50:15.000000 drup-1.1.0/src/drup/wrappers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 00:08:06.297852 drup-1.2.0/
+-rw-rw-r--   0 root         (0) root         (0)     1072 2023-04-16 13:21:59.000000 drup-1.2.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       70 2023-04-29 15:45:45.000000 drup-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7647 2023-04-30 00:08:06.297597 drup-1.2.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     6927 2023-04-29 20:56:46.000000 drup-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 00:08:06.277074 drup-1.2.0/drup.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     7647 2023-04-30 00:08:06.000000 drup-1.2.0/drup.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      281 2023-04-30 00:08:06.000000 drup-1.2.0/drup.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-04-30 00:08:06.000000 drup-1.2.0/drup.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       39 2023-04-30 00:08:06.000000 drup-1.2.0/drup.egg-info/entry_points.txt
+-rw-rw-r--   0 root         (0) root         (0)        5 2023-04-30 00:08:06.000000 drup-1.2.0/drup.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      777 2023-04-29 15:45:45.000000 drup-1.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-30 00:08:06.297932 drup-1.2.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      916 2023-04-29 15:45:45.000000 drup-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 00:08:06.272545 drup-1.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 00:08:06.296919 drup-1.2.0/src/drup/
+-rw-rw-r--   0 root         (0) root         (0)     4302 2023-04-30 00:01:24.000000 drup-1.2.0/src/drup/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1118 2023-04-29 20:20:50.000000 drup-1.2.0/src/drup/cli.py
+-r-xr-xr-x   0 root         (0) root         (0)  4294704 2023-04-30 00:08:06.000000 drup-1.2.0/src/drup/libdrupchecker.so
+-rw-rw-r--   0 root         (0) root         (0)    16811 2023-04-29 21:10:50.000000 drup-1.2.0/src/drup/wrappers.py
```

### Comparing `drup-1.1.0/LICENSE` & `drup-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drup-1.1.0/PKG-INFO` & `drup-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drup
-Version: 1.1.0
+Version: 1.2.0
 Summary: Checks DRUP proofs against DIMACS source. Extracted from verified Why3 code.
 Author-email: Matt Fredrikson <mfredrik@cmu.edu>
 Project-URL: Homepage, https://github.com/cmu-transparency/verified_rup
 Project-URL: Bug Tracker, https://github.com/cmu-transparency/verified_rup/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: OCaml
 Classifier: License :: OSI Approved :: MIT License
@@ -13,33 +13,33 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # A Verified DRUP Proof Checker
 
-As the title suggests, a verified implementation of a checker for propositional unsatisfiability proofs in the  [DRUP format](https://satcompetition.github.io/2022/certificates.html) that is produced by several solvers.
+As the title suggests, a verified implementation of a checker for propositional unsatisfiability proofs in the  [DRUP format](https://satcompetition.github.io/2022/certificates.html) that is produced by many solvers.
 The core of the checker is written in [Why3](https://why3.lri.fr/), which is extracted to OCaml, compiled natively, and exported as a C library with Python bindings.
 
-* The checker also supports RAT clauses, so DRAT proofs are also accepted.
+* The checker also supports RAT clauses, so DRAT proofs are accepted.
 * The current implementation is not optimized, and will be considerably slower than [DRAT-trim](https://github.com/marijnheule/drat-trim) on large proofs (see [performance](#performance) below).
 * Accordingly, the frontend does not accept proofs in binary format.
 
 The verification can be checked by running `src/librupchecker/rup_pure.mlw` in Why3. 
 Most of the verification conditions complete with the `Auto level 0` tactic, and the rest either with a few levels of splitting followed by `Auto 0` or `Auto 1`, or simply with `Auto 2`.
 It was developed using Why3 1.5.1, Alt-Ergo 2.4.0, Z3 4.8.6, and CVC4 1.8.
 Verification has not been attempted with earlier versions of Why3 or the provers.
 
 ## Installation
 
 If you use a recent Linux distribution on x86_64, you should be able to install the compiled wheel from PyPI:
 ```bash
 $ pip install drup
 ```
-Otherwise, you need to have OCaml (>= 4.12), Why3 (>= 1.5.1), and Dune (>=2.9.3) installed.
+Otherwise, you need to have OCaml (>= 4.12), Ctypes (>=0.20), Why3 (>= 1.5.1), and Dune (>=2.9.3) installed.
 The most straightforward way to install these is to use [opam](https://opam.ocaml.org/doc/Install.html), which is available in most package systems, and then install Why3 and Dune (a sufficiently recent version of OCaml should already be installed with Opam): 
 ```bash
 $ opam install why3 dune
 ```
 If you do not intend to check the verification of the library or develop it further, then you do not need to install Why3's IDE or any of the solvers that it supports.
 
 Once OCaml and Why3 are installed, make sure that Python `build` is installed:
@@ -57,105 +57,98 @@
 ## Usage
 
 ### Command line interface
 
 The package provides a command line interface for checking proofs stored in files:
 ```bash
 $ drup --help
+usage: drup [-h] [-d] [-v] dimacs drup
 
-usage: drup [-h] dimacs drup
-
-Checks DRUP & DRAT proofs against DIMACS source. 
-Returns 0 if the proof is valid, -1 if not, or a negative error code if the input is invalid.
+Checks DRUP & DRAT proofs against DIMACS source. Returns 0 if the proof is valid, -1 if not, or a negative error code if the input is invalid.
 
 positional arguments:
-  dimacs      Path to a DIMACS CNF formula
-  drup        Path to a DRUP/DRAT proof
+  dimacs            Path to a DIMACS CNF formula
+  drup              Path to a DRUP/DRAT proof
+
+optional arguments:
+  -h, --help        show this help message and exit
+  -d, --derivation  Check each step, ignore absence of empty clause
+  -v, --verbose     Print detailed information about failed checks
 
-options:
-  -h, --help  show this help message and exit
+For more information visit https://github.com/cmu-transparency/verified_rup
 ```
 
-### As a C library
+### As a Python module
 
-If you do not intend to use the Python bindings, then you will find the C shared object in the Python package directory:
-```bash
-$(PYTHON_PATH)/site-packages/rup/librupchecker.{so|dll}
-```
-The C library exposes wrappers around the core checker, which you can declare external in your C code as follows:
-```C
-int check_derivation_from_strings(const char *dimacs, const char *cs);
-int check_from_file(const char *dimacs_path, const char *drup_path);
-int check_from_strings(const char *dimacs, const char *drup);
-int check_step_from_strings(const char *dimacs, const char *c);
-```
-Before any of these can be called, the library must be initialized with a call to `do_startup` passing the current `argv`, which calls `caml_startup`:
-```C
-int do_startup(char **argv);
+See the documentation for details of the API.
+The primary function is `drup.check_proof`, or alternatively, `drup.check_derivation` to check each step of the proof, ignoring the absence of an empty clause).
+```python
+def check_proof(formula : Cnf, proof : Proof, verbose : bool = False) -> CheckerResult:
+  """Check a sequence of RUP and RAT clauses against a CNF. Inputs are Python iterables
+  of clauses, where each clause is an iterable of signed Python ints.
+
+  Args:
+    formula (Cnf): Cnf as an iterable of clauses.
+    proof (Proof): Iterable of RUP or RAT clauses.
+    verbose (bool, optional): Return detailed information
+      if the check fails. Defaults to False.
+
+  Returns:
+    CheckerResult: CheckerResult struct representing the result of the check.
+  
+  Raises:
+    ValueError: If the formula or proof cannot be formatted.
+  """
 ```
-Either function returns `0` if the proof is valid, and `-1` otherwise.
+This takes a CNF and Proof as an iterable of iterables of signed integers, and returns a `CheckerResult`.
+```python
+class CheckerResult:
 
-### As a Python module
+  '''
+  Result of a proof check.
 
-The Python bindings expose these same functions, but will call `do_startup` automatically when the package is imported, so there is no need to call it manually.
-If the arguments given to the Python bindings cannot be opened (in the case of files) or parsed, then they raise `ValueError`.
-If the proof is valid, then the Python bindings return `True`, and `False` otherwise.
+  Attributes:
 
-As described, the package is straightforward to use:
-```python
-import drup
+    outcome (`Outcome`): The outcome of the check. If the check
+      succeeded, this will be Outcome.VALID. If the check failed,
+      this will be Outcome.INVALID.
+
+    steps (`Optional[Cnf]`): Completed proof steps prior to an invalid step, 
+      if the proof was invalid.
+
+    rup_info (`Optional[RupInfo]`): Information on a failed RUP check,
+      if the proof was invalid.
 
-cnf = """
-p cnf 4 8
- 1  2 -3 0
--1 -2  3 0
- 2  3 -4 0
--2 -3  4 0
- 1  3  4 0
--1 -3 -4 0
--1  2  4 0
- 1 -2 -4 0
-"""
-
-pf = """
-1 2 0
-1 0
-2 0
-0
-"""
-
-if drup.check_from_strings(cnf, pf):
-    print("Valid")
-else:
-    print("Invalid")
+    rat_info (`Optional[RatInfo]`): Information on a failed RAT check,
+      if the proof was invalid. The RAT clause in this object will
+      be the same as the RUP clause in `rup_info`.
+  '''
 ```
+There are corresponding convenience functions `check_proof_from_strings` and `check_proof_from_files`, similarly for `check_derivation`.
+
 
 ## Performance
 
 At present, the implementation of RUP checking is not optimized, and drop lines are ignored.
 Unit propagation does not take advantage of watched literals, and does not use mutable data structures.
 Nonetheless, the performance compares well to that of [DRAT-trim](https://github.com/marijnheule/drat-trim) on small proofs (<200 variables, a few hundred clauses).
 
 We measure this on random unsatisfiable instances generated by the procedure described in [[1]](#references).
 To evaluate the performance of DRAT-trim without the overhead of creating and tearing down a new process for each instance, we compiled it into a library with the same `check_from_strings` interface as the C library, and called it using [ctypes](https://docs.python.org/3/library/ctypes.html).
 In the table below, each configuration is run on 10,000 instances, with proofs generated by [Glucose 4](https://www.labri.fr/perso/lsimon/research/glucose/).
 
-<center>
-
 | # vars | # clauses (avg) | pf len (avg) | `drup (sec, avg)` | `drat-trim (sec, avg)` |
 | ------ | --------------- | ------------ | ----------------- | ---------------------- |
 | 25     | 147.7           | 7.3          | 0.001             | 0.085                  |
 | 50     | 280.5           | 14.2         | 0.006             | 0.179                  |
 | 75     | 413.5           | 26.3         | 0.022             | 0.217                  |
 | 100    | 548.2           | 40.6         | 0.068             | 0.172                  |
 | 150    | 811.8           | 102.7        | 0.407             | 0.326                  |
 | 200    | 1079.5          | 227.9        | 1.916             | 0.292                  |
 
-</center>
-
 ### References
 
 [[1]](https://openreview.net/forum?id=HJMC_iA5tm) Daniel Selsam, Matthew Lamm, Benedikt Bünz, Percy Liang, Leonardo de Moura, David L. Dill. *Learning a SAT Solver from Single-Bit Supervision*. International Conference on Learning Representations (ICLR), 2019.
 
 ## Acknowledgements
 
 Many thanks to [Frank Pfenning](http://www.cs.cmu.edu/~fp/), [Joseph Reeves](https://www.cs.cmu.edu/~jereeves/), and [Marijn Huele](https://www.cs.cmu.edu/~mheule/) for the ongoing insightful discussions that led to this project.
```

### Comparing `drup-1.1.0/README.md` & `drup-1.2.0/drup.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,45 @@
+Metadata-Version: 2.1
+Name: drup
+Version: 1.2.0
+Summary: Checks DRUP proofs against DIMACS source. Extracted from verified Why3 code.
+Author-email: Matt Fredrikson <mfredrik@cmu.edu>
+Project-URL: Homepage, https://github.com/cmu-transparency/verified_rup
+Project-URL: Bug Tracker, https://github.com/cmu-transparency/verified_rup/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: OCaml
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # A Verified DRUP Proof Checker
 
-As the title suggests, a verified implementation of a checker for propositional unsatisfiability proofs in the  [DRUP format](https://satcompetition.github.io/2022/certificates.html) that is produced by several solvers.
+As the title suggests, a verified implementation of a checker for propositional unsatisfiability proofs in the  [DRUP format](https://satcompetition.github.io/2022/certificates.html) that is produced by many solvers.
 The core of the checker is written in [Why3](https://why3.lri.fr/), which is extracted to OCaml, compiled natively, and exported as a C library with Python bindings.
 
-* The checker also supports RAT clauses, so DRAT proofs are also accepted.
+* The checker also supports RAT clauses, so DRAT proofs are accepted.
 * The current implementation is not optimized, and will be considerably slower than [DRAT-trim](https://github.com/marijnheule/drat-trim) on large proofs (see [performance](#performance) below).
 * Accordingly, the frontend does not accept proofs in binary format.
 
 The verification can be checked by running `src/librupchecker/rup_pure.mlw` in Why3. 
 Most of the verification conditions complete with the `Auto level 0` tactic, and the rest either with a few levels of splitting followed by `Auto 0` or `Auto 1`, or simply with `Auto 2`.
 It was developed using Why3 1.5.1, Alt-Ergo 2.4.0, Z3 4.8.6, and CVC4 1.8.
 Verification has not been attempted with earlier versions of Why3 or the provers.
 
 ## Installation
 
 If you use a recent Linux distribution on x86_64, you should be able to install the compiled wheel from PyPI:
 ```bash
 $ pip install drup
 ```
-Otherwise, you need to have OCaml (>= 4.12), Why3 (>= 1.5.1), and Dune (>=2.9.3) installed.
+Otherwise, you need to have OCaml (>= 4.12), Ctypes (>=0.20), Why3 (>= 1.5.1), and Dune (>=2.9.3) installed.
 The most straightforward way to install these is to use [opam](https://opam.ocaml.org/doc/Install.html), which is available in most package systems, and then install Why3 and Dune (a sufficiently recent version of OCaml should already be installed with Opam): 
 ```bash
 $ opam install why3 dune
 ```
 If you do not intend to check the verification of the library or develop it further, then you do not need to install Why3's IDE or any of the solvers that it supports.
 
 Once OCaml and Why3 are installed, make sure that Python `build` is installed:
@@ -40,105 +57,98 @@
 ## Usage
 
 ### Command line interface
 
 The package provides a command line interface for checking proofs stored in files:
 ```bash
 $ drup --help
+usage: drup [-h] [-d] [-v] dimacs drup
 
-usage: drup [-h] dimacs drup
-
-Checks DRUP & DRAT proofs against DIMACS source. 
-Returns 0 if the proof is valid, -1 if not, or a negative error code if the input is invalid.
+Checks DRUP & DRAT proofs against DIMACS source. Returns 0 if the proof is valid, -1 if not, or a negative error code if the input is invalid.
 
 positional arguments:
-  dimacs      Path to a DIMACS CNF formula
-  drup        Path to a DRUP/DRAT proof
+  dimacs            Path to a DIMACS CNF formula
+  drup              Path to a DRUP/DRAT proof
 
-options:
-  -h, --help  show this help message and exit
+optional arguments:
+  -h, --help        show this help message and exit
+  -d, --derivation  Check each step, ignore absence of empty clause
+  -v, --verbose     Print detailed information about failed checks
+
+For more information visit https://github.com/cmu-transparency/verified_rup
 ```
 
-### As a C library
+### As a Python module
 
-If you do not intend to use the Python bindings, then you will find the C shared object in the Python package directory:
-```bash
-$(PYTHON_PATH)/site-packages/rup/librupchecker.{so|dll}
-```
-The C library exposes wrappers around the core checker, which you can declare external in your C code as follows:
-```C
-int check_derivation_from_strings(const char *dimacs, const char *cs);
-int check_from_file(const char *dimacs_path, const char *drup_path);
-int check_from_strings(const char *dimacs, const char *drup);
-int check_step_from_strings(const char *dimacs, const char *c);
-```
-Before any of these can be called, the library must be initialized with a call to `do_startup` passing the current `argv`, which calls `caml_startup`:
-```C
-int do_startup(char **argv);
+See the documentation for details of the API.
+The primary function is `drup.check_proof`, or alternatively, `drup.check_derivation` to check each step of the proof, ignoring the absence of an empty clause).
+```python
+def check_proof(formula : Cnf, proof : Proof, verbose : bool = False) -> CheckerResult:
+  """Check a sequence of RUP and RAT clauses against a CNF. Inputs are Python iterables
+  of clauses, where each clause is an iterable of signed Python ints.
+
+  Args:
+    formula (Cnf): Cnf as an iterable of clauses.
+    proof (Proof): Iterable of RUP or RAT clauses.
+    verbose (bool, optional): Return detailed information
+      if the check fails. Defaults to False.
+
+  Returns:
+    CheckerResult: CheckerResult struct representing the result of the check.
+  
+  Raises:
+    ValueError: If the formula or proof cannot be formatted.
+  """
 ```
-Either function returns `0` if the proof is valid, and `-1` otherwise.
+This takes a CNF and Proof as an iterable of iterables of signed integers, and returns a `CheckerResult`.
+```python
+class CheckerResult:
 
-### As a Python module
+  '''
+  Result of a proof check.
 
-The Python bindings expose these same functions, but will call `do_startup` automatically when the package is imported, so there is no need to call it manually.
-If the arguments given to the Python bindings cannot be opened (in the case of files) or parsed, then they raise `ValueError`.
-If the proof is valid, then the Python bindings return `True`, and `False` otherwise.
+  Attributes:
 
-As described, the package is straightforward to use:
-```python
-import drup
+    outcome (`Outcome`): The outcome of the check. If the check
+      succeeded, this will be Outcome.VALID. If the check failed,
+      this will be Outcome.INVALID.
+
+    steps (`Optional[Cnf]`): Completed proof steps prior to an invalid step, 
+      if the proof was invalid.
+
+    rup_info (`Optional[RupInfo]`): Information on a failed RUP check,
+      if the proof was invalid.
 
-cnf = """
-p cnf 4 8
- 1  2 -3 0
--1 -2  3 0
- 2  3 -4 0
--2 -3  4 0
- 1  3  4 0
--1 -3 -4 0
--1  2  4 0
- 1 -2 -4 0
-"""
-
-pf = """
-1 2 0
-1 0
-2 0
-0
-"""
-
-if drup.check_from_strings(cnf, pf):
-    print("Valid")
-else:
-    print("Invalid")
+    rat_info (`Optional[RatInfo]`): Information on a failed RAT check,
+      if the proof was invalid. The RAT clause in this object will
+      be the same as the RUP clause in `rup_info`.
+  '''
 ```
+There are corresponding convenience functions `check_proof_from_strings` and `check_proof_from_files`, similarly for `check_derivation`.
+
 
 ## Performance
 
 At present, the implementation of RUP checking is not optimized, and drop lines are ignored.
 Unit propagation does not take advantage of watched literals, and does not use mutable data structures.
 Nonetheless, the performance compares well to that of [DRAT-trim](https://github.com/marijnheule/drat-trim) on small proofs (<200 variables, a few hundred clauses).
 
 We measure this on random unsatisfiable instances generated by the procedure described in [[1]](#references).
 To evaluate the performance of DRAT-trim without the overhead of creating and tearing down a new process for each instance, we compiled it into a library with the same `check_from_strings` interface as the C library, and called it using [ctypes](https://docs.python.org/3/library/ctypes.html).
 In the table below, each configuration is run on 10,000 instances, with proofs generated by [Glucose 4](https://www.labri.fr/perso/lsimon/research/glucose/).
 
-<center>
-
 | # vars | # clauses (avg) | pf len (avg) | `drup (sec, avg)` | `drat-trim (sec, avg)` |
 | ------ | --------------- | ------------ | ----------------- | ---------------------- |
 | 25     | 147.7           | 7.3          | 0.001             | 0.085                  |
 | 50     | 280.5           | 14.2         | 0.006             | 0.179                  |
 | 75     | 413.5           | 26.3         | 0.022             | 0.217                  |
 | 100    | 548.2           | 40.6         | 0.068             | 0.172                  |
 | 150    | 811.8           | 102.7        | 0.407             | 0.326                  |
 | 200    | 1079.5          | 227.9        | 1.916             | 0.292                  |
 
-</center>
-
 ### References
 
 [[1]](https://openreview.net/forum?id=HJMC_iA5tm) Daniel Selsam, Matthew Lamm, Benedikt Bünz, Percy Liang, Leonardo de Moura, David L. Dill. *Learning a SAT Solver from Single-Bit Supervision*. International Conference on Learning Representations (ICLR), 2019.
 
 ## Acknowledgements
 
-Many thanks to [Frank Pfenning](http://www.cs.cmu.edu/~fp/), [Joseph Reeves](https://www.cs.cmu.edu/~jereeves/), and [Marijn Huele](https://www.cs.cmu.edu/~mheule/) for the ongoing insightful discussions that led to this project.
+Many thanks to [Frank Pfenning](http://www.cs.cmu.edu/~fp/), [Joseph Reeves](https://www.cs.cmu.edu/~jereeves/), and [Marijn Huele](https://www.cs.cmu.edu/~mheule/) for the ongoing insightful discussions that led to this project.
```

### Comparing `drup-1.1.0/drup.egg-info/PKG-INFO` & `drup-1.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,28 @@
-Metadata-Version: 2.1
-Name: drup
-Version: 1.1.0
-Summary: Checks DRUP proofs against DIMACS source. Extracted from verified Why3 code.
-Author-email: Matt Fredrikson <mfredrik@cmu.edu>
-Project-URL: Homepage, https://github.com/cmu-transparency/verified_rup
-Project-URL: Bug Tracker, https://github.com/cmu-transparency/verified_rup/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: OCaml
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # A Verified DRUP Proof Checker
 
-As the title suggests, a verified implementation of a checker for propositional unsatisfiability proofs in the  [DRUP format](https://satcompetition.github.io/2022/certificates.html) that is produced by several solvers.
+As the title suggests, a verified implementation of a checker for propositional unsatisfiability proofs in the  [DRUP format](https://satcompetition.github.io/2022/certificates.html) that is produced by many solvers.
 The core of the checker is written in [Why3](https://why3.lri.fr/), which is extracted to OCaml, compiled natively, and exported as a C library with Python bindings.
 
-* The checker also supports RAT clauses, so DRAT proofs are also accepted.
+* The checker also supports RAT clauses, so DRAT proofs are accepted.
 * The current implementation is not optimized, and will be considerably slower than [DRAT-trim](https://github.com/marijnheule/drat-trim) on large proofs (see [performance](#performance) below).
 * Accordingly, the frontend does not accept proofs in binary format.
 
 The verification can be checked by running `src/librupchecker/rup_pure.mlw` in Why3. 
 Most of the verification conditions complete with the `Auto level 0` tactic, and the rest either with a few levels of splitting followed by `Auto 0` or `Auto 1`, or simply with `Auto 2`.
 It was developed using Why3 1.5.1, Alt-Ergo 2.4.0, Z3 4.8.6, and CVC4 1.8.
 Verification has not been attempted with earlier versions of Why3 or the provers.
 
 ## Installation
 
 If you use a recent Linux distribution on x86_64, you should be able to install the compiled wheel from PyPI:
 ```bash
 $ pip install drup
 ```
-Otherwise, you need to have OCaml (>= 4.12), Why3 (>= 1.5.1), and Dune (>=2.9.3) installed.
+Otherwise, you need to have OCaml (>= 4.12), Ctypes (>=0.20), Why3 (>= 1.5.1), and Dune (>=2.9.3) installed.
 The most straightforward way to install these is to use [opam](https://opam.ocaml.org/doc/Install.html), which is available in most package systems, and then install Why3 and Dune (a sufficiently recent version of OCaml should already be installed with Opam): 
 ```bash
 $ opam install why3 dune
 ```
 If you do not intend to check the verification of the library or develop it further, then you do not need to install Why3's IDE or any of the solvers that it supports.
 
 Once OCaml and Why3 are installed, make sure that Python `build` is installed:
@@ -57,105 +40,98 @@
 ## Usage
 
 ### Command line interface
 
 The package provides a command line interface for checking proofs stored in files:
 ```bash
 $ drup --help
+usage: drup [-h] [-d] [-v] dimacs drup
 
-usage: drup [-h] dimacs drup
-
-Checks DRUP & DRAT proofs against DIMACS source. 
-Returns 0 if the proof is valid, -1 if not, or a negative error code if the input is invalid.
+Checks DRUP & DRAT proofs against DIMACS source. Returns 0 if the proof is valid, -1 if not, or a negative error code if the input is invalid.
 
 positional arguments:
-  dimacs      Path to a DIMACS CNF formula
-  drup        Path to a DRUP/DRAT proof
+  dimacs            Path to a DIMACS CNF formula
+  drup              Path to a DRUP/DRAT proof
 
-options:
-  -h, --help  show this help message and exit
+optional arguments:
+  -h, --help        show this help message and exit
+  -d, --derivation  Check each step, ignore absence of empty clause
+  -v, --verbose     Print detailed information about failed checks
+
+For more information visit https://github.com/cmu-transparency/verified_rup
 ```
 
-### As a C library
+### As a Python module
 
-If you do not intend to use the Python bindings, then you will find the C shared object in the Python package directory:
-```bash
-$(PYTHON_PATH)/site-packages/rup/librupchecker.{so|dll}
-```
-The C library exposes wrappers around the core checker, which you can declare external in your C code as follows:
-```C
-int check_derivation_from_strings(const char *dimacs, const char *cs);
-int check_from_file(const char *dimacs_path, const char *drup_path);
-int check_from_strings(const char *dimacs, const char *drup);
-int check_step_from_strings(const char *dimacs, const char *c);
-```
-Before any of these can be called, the library must be initialized with a call to `do_startup` passing the current `argv`, which calls `caml_startup`:
-```C
-int do_startup(char **argv);
+See the documentation for details of the API.
+The primary function is `drup.check_proof`, or alternatively, `drup.check_derivation` to check each step of the proof, ignoring the absence of an empty clause).
+```python
+def check_proof(formula : Cnf, proof : Proof, verbose : bool = False) -> CheckerResult:
+  """Check a sequence of RUP and RAT clauses against a CNF. Inputs are Python iterables
+  of clauses, where each clause is an iterable of signed Python ints.
+
+  Args:
+    formula (Cnf): Cnf as an iterable of clauses.
+    proof (Proof): Iterable of RUP or RAT clauses.
+    verbose (bool, optional): Return detailed information
+      if the check fails. Defaults to False.
+
+  Returns:
+    CheckerResult: CheckerResult struct representing the result of the check.
+  
+  Raises:
+    ValueError: If the formula or proof cannot be formatted.
+  """
 ```
-Either function returns `0` if the proof is valid, and `-1` otherwise.
+This takes a CNF and Proof as an iterable of iterables of signed integers, and returns a `CheckerResult`.
+```python
+class CheckerResult:
 
-### As a Python module
+  '''
+  Result of a proof check.
 
-The Python bindings expose these same functions, but will call `do_startup` automatically when the package is imported, so there is no need to call it manually.
-If the arguments given to the Python bindings cannot be opened (in the case of files) or parsed, then they raise `ValueError`.
-If the proof is valid, then the Python bindings return `True`, and `False` otherwise.
+  Attributes:
 
-As described, the package is straightforward to use:
-```python
-import drup
+    outcome (`Outcome`): The outcome of the check. If the check
+      succeeded, this will be Outcome.VALID. If the check failed,
+      this will be Outcome.INVALID.
+
+    steps (`Optional[Cnf]`): Completed proof steps prior to an invalid step, 
+      if the proof was invalid.
+
+    rup_info (`Optional[RupInfo]`): Information on a failed RUP check,
+      if the proof was invalid.
 
-cnf = """
-p cnf 4 8
- 1  2 -3 0
--1 -2  3 0
- 2  3 -4 0
--2 -3  4 0
- 1  3  4 0
--1 -3 -4 0
--1  2  4 0
- 1 -2 -4 0
-"""
-
-pf = """
-1 2 0
-1 0
-2 0
-0
-"""
-
-if drup.check_from_strings(cnf, pf):
-    print("Valid")
-else:
-    print("Invalid")
+    rat_info (`Optional[RatInfo]`): Information on a failed RAT check,
+      if the proof was invalid. The RAT clause in this object will
+      be the same as the RUP clause in `rup_info`.
+  '''
 ```
+There are corresponding convenience functions `check_proof_from_strings` and `check_proof_from_files`, similarly for `check_derivation`.
+
 
 ## Performance
 
 At present, the implementation of RUP checking is not optimized, and drop lines are ignored.
 Unit propagation does not take advantage of watched literals, and does not use mutable data structures.
 Nonetheless, the performance compares well to that of [DRAT-trim](https://github.com/marijnheule/drat-trim) on small proofs (<200 variables, a few hundred clauses).
 
 We measure this on random unsatisfiable instances generated by the procedure described in [[1]](#references).
 To evaluate the performance of DRAT-trim without the overhead of creating and tearing down a new process for each instance, we compiled it into a library with the same `check_from_strings` interface as the C library, and called it using [ctypes](https://docs.python.org/3/library/ctypes.html).
 In the table below, each configuration is run on 10,000 instances, with proofs generated by [Glucose 4](https://www.labri.fr/perso/lsimon/research/glucose/).
 
-<center>
-
 | # vars | # clauses (avg) | pf len (avg) | `drup (sec, avg)` | `drat-trim (sec, avg)` |
 | ------ | --------------- | ------------ | ----------------- | ---------------------- |
 | 25     | 147.7           | 7.3          | 0.001             | 0.085                  |
 | 50     | 280.5           | 14.2         | 0.006             | 0.179                  |
 | 75     | 413.5           | 26.3         | 0.022             | 0.217                  |
 | 100    | 548.2           | 40.6         | 0.068             | 0.172                  |
 | 150    | 811.8           | 102.7        | 0.407             | 0.326                  |
 | 200    | 1079.5          | 227.9        | 1.916             | 0.292                  |
 
-</center>
-
 ### References
 
 [[1]](https://openreview.net/forum?id=HJMC_iA5tm) Daniel Selsam, Matthew Lamm, Benedikt Bünz, Percy Liang, Leonardo de Moura, David L. Dill. *Learning a SAT Solver from Single-Bit Supervision*. International Conference on Learning Representations (ICLR), 2019.
 
 ## Acknowledgements
 
-Many thanks to [Frank Pfenning](http://www.cs.cmu.edu/~fp/), [Joseph Reeves](https://www.cs.cmu.edu/~jereeves/), and [Marijn Huele](https://www.cs.cmu.edu/~mheule/) for the ongoing insightful discussions that led to this project.
+Many thanks to [Frank Pfenning](http://www.cs.cmu.edu/~fp/), [Joseph Reeves](https://www.cs.cmu.edu/~jereeves/), and [Marijn Huele](https://www.cs.cmu.edu/~mheule/) for the ongoing insightful discussions that led to this project.
```

### Comparing `drup-1.1.0/pyproject.toml` & `drup-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "drup"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="Matt Fredrikson", email="mfredrik@cmu.edu" },
 ]
 description = "Checks DRUP proofs against DIMACS source. Extracted from verified Why3 code."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `drup-1.1.0/setup.py` & `drup-1.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,35 +4,26 @@
 import subprocess
 import setuptools
 
 from pathlib import Path
 from setuptools import setup, Extension
 from setuptools.command.sdist import sdist as _sdist
 
-def extract_checker():
-    cmd = [
-        "why3", "extract", "-D", "ocaml64", 
-        "src/librupchecker/rup_pure.mlw", "-o", "src/librupchecker/rup.ml"
-    ]
-    subprocess.run(cmd, check=True, stdout=sys.stdout, stderr=sys.stderr)
-
 def build_checker():
     cmd = ["dune", "build"]
     subprocess.run(cmd, check=True, stdout=sys.stdout, stderr=sys.stderr)
 
 class SDist(_sdist):
     def run(self) -> None:
-        extract_checker()
         build_checker()
-        shutil.copy("_build/default/src/librupchecker/checker.so", "src/drup/librupchecker.so")
+        shutil.copy("_build/default/src/librupchecker/libdrupchecker.so", "src/drup/libdrupchecker.so")
         super().run()
         cmd = ["dune", "clean"]
         subprocess.run(cmd, check=False, stdout=sys.stdout, stderr=sys.stderr)
-        os.unlink("src/drup/librupchecker.so")
-        os.unlink("src/librupchecker/rup.ml")
+        os.unlink("src/drup/libdrupchecker.so")
 
 setup(
     cmdclass={'sdist': SDist},
     packages=['drup'],
     package_dir={'drup': 'src/drup'},
     ext_modules=[Extension(name="drup.librupchecker", sources=[])],
 	entry_points = {
```

