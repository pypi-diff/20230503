# Comparing `tmp/drup-1.2.0.tar.gz` & `tmp/drup-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drup-1.2.0.tar", last modified: Sun Apr 30 00:08:06 2023, max compression
+gzip compressed data, was "drup-1.2.1.tar", last modified: Tue May  2 22:46:01 2023, max compression
```

## Comparing `drup-1.2.0.tar` & `drup-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 00:08:06.297852 drup-1.2.0/
--rw-rw-r--   0 root         (0) root         (0)     1072 2023-04-16 13:21:59.000000 drup-1.2.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       70 2023-04-29 15:45:45.000000 drup-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7647 2023-04-30 00:08:06.297597 drup-1.2.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     6927 2023-04-29 20:56:46.000000 drup-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 00:08:06.277074 drup-1.2.0/drup.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     7647 2023-04-30 00:08:06.000000 drup-1.2.0/drup.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      281 2023-04-30 00:08:06.000000 drup-1.2.0/drup.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-04-30 00:08:06.000000 drup-1.2.0/drup.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       39 2023-04-30 00:08:06.000000 drup-1.2.0/drup.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)        5 2023-04-30 00:08:06.000000 drup-1.2.0/drup.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      777 2023-04-29 15:45:45.000000 drup-1.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-30 00:08:06.297932 drup-1.2.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      916 2023-04-29 15:45:45.000000 drup-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 00:08:06.272545 drup-1.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 00:08:06.296919 drup-1.2.0/src/drup/
--rw-rw-r--   0 root         (0) root         (0)     4302 2023-04-30 00:01:24.000000 drup-1.2.0/src/drup/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1118 2023-04-29 20:20:50.000000 drup-1.2.0/src/drup/cli.py
--r-xr-xr-x   0 root         (0) root         (0)  4294704 2023-04-30 00:08:06.000000 drup-1.2.0/src/drup/libdrupchecker.so
--rw-rw-r--   0 root         (0) root         (0)    16811 2023-04-29 21:10:50.000000 drup-1.2.0/src/drup/wrappers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 22:46:01.344947 drup-1.2.1/
+-rw-rw-r--   0 root         (0) root         (0)     1072 2023-04-16 13:21:59.000000 drup-1.2.1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       70 2023-04-29 15:45:45.000000 drup-1.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10819 2023-05-02 22:46:01.344707 drup-1.2.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    10018 2023-05-01 15:34:52.000000 drup-1.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 22:46:01.328640 drup-1.2.1/drup.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)    10819 2023-05-02 22:46:01.000000 drup-1.2.1/drup.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      281 2023-05-02 22:46:01.000000 drup-1.2.1/drup.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-05-02 22:46:01.000000 drup-1.2.1/drup.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       39 2023-05-02 22:46:01.000000 drup-1.2.1/drup.egg-info/entry_points.txt
+-rw-rw-r--   0 root         (0) root         (0)        5 2023-05-02 22:46:01.000000 drup-1.2.1/drup.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      849 2023-05-02 22:45:31.000000 drup-1.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 22:46:01.345025 drup-1.2.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      916 2023-04-29 15:45:45.000000 drup-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 22:46:01.324800 drup-1.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 22:46:01.344112 drup-1.2.1/src/drup/
+-rw-rw-r--   0 root         (0) root         (0)     4302 2023-05-02 22:43:44.000000 drup-1.2.1/src/drup/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1118 2023-04-29 20:20:50.000000 drup-1.2.1/src/drup/cli.py
+-r-xr-xr-x   0 root         (0) root         (0)  4294704 2023-05-02 22:46:01.000000 drup-1.2.1/src/drup/libdrupchecker.so
+-rw-rw-r--   0 root         (0) root         (0)    16811 2023-04-29 21:10:50.000000 drup-1.2.1/src/drup/wrappers.py
```

### Comparing `drup-1.2.0/LICENSE` & `drup-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drup-1.2.0/README.md` & `drup-1.2.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,34 @@
+Metadata-Version: 2.1
+Name: drup
+Version: 1.2.1
+Summary: Checks DRUP proofs against DIMACS source. Extracted from verified Why3 code.
+Author-email: Matt Fredrikson <mfredrik@cmu.edu>
+Project-URL: Homepage, https://github.com/cmu-transparency/verified_rup
+Project-URL: Documentation, https://fairlyaccountable.org/verified_rup/drup.html
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
 
 As the title suggests, a verified implementation of a checker for propositional unsatisfiability proofs in the  [DRUP format](https://satcompetition.github.io/2022/certificates.html) that is produced by many solvers.
 The core of the checker is written in [Why3](https://why3.lri.fr/), which is extracted to OCaml, compiled natively, and exported as a C library with Python bindings.
 
 * The checker also supports RAT clauses, so DRAT proofs are accepted.
 * The current implementation is not optimized, and will be considerably slower than [DRAT-trim](https://github.com/marijnheule/drat-trim) on large proofs (see [performance](#performance) below).
 * Accordingly, the frontend does not accept proofs in binary format.
 
-The verification can be checked by running `src/librupchecker/rup_pure.mlw` in Why3. 
-Most of the verification conditions complete with the `Auto level 0` tactic, and the rest either with a few levels of splitting followed by `Auto 0` or `Auto 1`, or simply with `Auto 2`.
-It was developed using Why3 1.5.1, Alt-Ergo 2.4.0, Z3 4.8.6, and CVC4 1.8.
-Verification has not been attempted with earlier versions of Why3 or the provers.
-
 ## Installation
 
 If you use a recent Linux distribution on x86_64, you should be able to install the compiled wheel from PyPI:
 ```bash
 $ pip install drup
 ```
 Otherwise, you need to have OCaml (>= 4.12), Ctypes (>=0.20), Why3 (>= 1.5.1), and Dune (>=2.9.3) installed.
@@ -58,60 +71,54 @@
   -v, --verbose     Print detailed information about failed checks
 
 For more information visit https://github.com/cmu-transparency/verified_rup
 ```
 
 ### As a Python module
 
-See the documentation for details of the API.
-The primary function is `drup.check_proof`, or alternatively, `drup.check_derivation` to check each step of the proof, ignoring the absence of an empty clause).
-```python
-def check_proof(formula : Cnf, proof : Proof, verbose : bool = False) -> CheckerResult:
-  """Check a sequence of RUP and RAT clauses against a CNF. Inputs are Python iterables
-  of clauses, where each clause is an iterable of signed Python ints.
-
-  Args:
-    formula (Cnf): Cnf as an iterable of clauses.
-    proof (Proof): Iterable of RUP or RAT clauses.
-    verbose (bool, optional): Return detailed information
-      if the check fails. Defaults to False.
-
-  Returns:
-    CheckerResult: CheckerResult struct representing the result of the check.
-  
-  Raises:
-    ValueError: If the formula or proof cannot be formatted.
-  """
-```
-This takes a CNF and Proof as an iterable of iterables of signed integers, and returns a `CheckerResult`.
-```python
-class CheckerResult:
+See the [documentation](https://fairlyaccountable.org/verified_rup/drup.html) for details of the API.
+The primary function is `drup.check_proof`, or alternatively, `drup.check_derivation` to check each step of the proof, ignoring the absence of an empty clause). There are corresponding convenience functions `check_proof_from_strings` and `check_proof_from_files`, similarly for `check_derivation`.
 
-  '''
-  Result of a proof check.
+The following example uses [CNFgen](https://massimolauria.net/cnfgen/) to generate a PHP instance,
+and [PySAT](https://pysathq.github.io/) to solve it and generate a DRUP proof.
+To illustrate the verbose output given for failed checks, only the first ten clauses of the proof are checked against the proof.
 
-  Attributes:
+```python
+import drup
+import cnfgen
+from pysat.formula import CNF
+from pysat.solvers import Solver
 
-    outcome (`Outcome`): The outcome of the check. If the check
-      succeeded, this will be Outcome.VALID. If the check failed,
-      this will be Outcome.INVALID.
+dimacs = cnfgen.BinaryPigeonholePrinciple(4, 3).dimacs()
+cnf = CNF(from_string=dimacs).clauses
+g4 = Solver(name='g4', with_proof=True, bootstrap_with=cnf)
+g4.solve()
+proof = [[int(l) for l in c.split(' ')[:-1]] for c in g4.get_proof()]
 
-    steps (`Optional[Cnf]`): Completed proof steps prior to an invalid step, 
-      if the proof was invalid.
+drup.check_proof(cnf[:10], proof, verbose=True)
+```
 
-    rup_info (`Optional[RupInfo]`): Information on a failed RUP check,
-      if the proof was invalid.
+This gives a `CheckerResult` object with the following information:
 
-    rat_info (`Optional[RatInfo]`): Information on a failed RAT check,
-      if the proof was invalid. The RAT clause in this object will
-      be the same as the RUP clause in `rup_info`.
-  '''
+```python
+CheckerResult(
+	Outcome.INVALID, 
+	[], 
+	RupInfo([4, 6, 7, 8], [-4, -6, -7, -8, 3, 5]), 
+	RatInfo(
+		[4, 6, 7, 8], 
+		[-4, -3], 
+		RupInfo([6, 7, 8, -3], [-6, -7, -8, 5, 3, -4])
+	)
+)
 ```
-There are corresponding convenience functions `check_proof_from_strings` and `check_proof_from_files`, similarly for `check_derivation`.
 
+The `RupInfo` component relates that RUP verification failed on the first clause of the proof, `4 6 7 8 0`, after propagating the literals `-4, -6, -7, -8, 3, 5`, and failing to find more opposites to propagate.
+Likewise, the `RatInfo` component relates that RAT verification on this clause failed when checking the pivot on clause `-4 -3 0`.
+The resolvent of these clauses, `6 7 8 -3 0`, failed RUP verification after propagating `-6 -7 -8 5 3 -4`.
 
 ## Performance
 
 At present, the implementation of RUP checking is not optimized, and drop lines are ignored.
 Unit propagation does not take advantage of watched literals, and does not use mutable data structures.
 Nonetheless, the performance compares well to that of [DRAT-trim](https://github.com/marijnheule/drat-trim) on small proofs (<200 variables, a few hundred clauses).
 
@@ -128,10 +135,86 @@
 | 150    | 811.8           | 102.7        | 0.407             | 0.326                  |
 | 200    | 1079.5          | 227.9        | 1.916             | 0.292                  |
 
 ### References
 
 [[1]](https://openreview.net/forum?id=HJMC_iA5tm) Daniel Selsam, Matthew Lamm, Benedikt Bünz, Percy Liang, Leonardo de Moura, David L. Dill. *Learning a SAT Solver from Single-Bit Supervision*. International Conference on Learning Representations (ICLR), 2019.
 
+## Verification
+
+The verification can be examined by running `src/librupchecker/rup_pure.mlw` in Why3, or by checking the Why3 session in `src/librupchecker/rup_pure/why3session.xml`. 
+The proof was developed using Why3 1.5.1, Alt-Ergo 2.4.0, Z3 4.8.6, and CVC4 1.8.
+Verification has not been attempted with earlier versions of Why3 or the provers.
+
+The primary contract on the proof checker is as follows:
+```ocaml
+requires { no_redundant_clauses cnf /\ no_trivial_clauses cnf }
+requires { no_redundant_clauses pf /\ no_trivial_clauses pf }
+ensures { match result with
+			| Valid -> valid_proof cnf pf
+			| _ -> proof_failure orig result
+			end }
+```
+The bindings used by this library take care of removing redundant and trivial clauses.
+The `valid_proof` predicate is a straightforward translation of DRAT certification requirements.
+A `proof_failure` result provides additional assurances about the verbose output of the checker.
+```ocaml
+predicate proof_failure (cnf : cnf) (result : result) =
+    match result with
+    | Valid -> false
+    | InvalidEmpty steps rup_info -> rup_failure (steps ++ cnf) rup_info
+    | InvalidStep steps rup_info rat_info -> 
+        rup_failure (steps ++ cnf) rup_info /\ rat_failure (steps ++ cnf) rat_info
+    end
+```
+An `InvalidEmpty` result indicates all of the listed `steps` are valid, but the empty clause was not derived, as witnessed by the provided `rup_info`.
+This is only returned when all of the steps in the proof are valid except an empty clause at the end.
+The `rup_info` component ensures that the empty clause is not RUP, and that the unit chain used to conclude this is exhaustive.
+
+```ocaml
+predicate rup_failure (cnf : cnf) (info : rup_info) =
+    not (rup cnf info.rup_clause) /\
+    match info.rup_clause with
+    | Nil -> 
+        let cnf' = bcp cnf info.chain in
+        is_unit_chain cnf info.chain /\ 
+        forall chain' . is_unit_chain cnf' chain' -> 
+                        forall c . mem c (bcp cnf' chain') <-> mem c cnf'
+    | Cons _ _ -> 
+        let cnf' = bcp (cnf ++ (negate_clause info.rup_clause)) info.chain in
+        is_unit_chain (cnf ++ (negate_clause info.rup_clause)) info.chain /\ 
+        forall chain' . is_unit_chain cnf' chain' -> 
+                        forall c . mem c (bcp cnf' chain') <-> mem c cnf'
+    end
+```
+
+An `InvalidStep` result indicates that the `steps` are valid up to some non-empty step.
+The next step in the certificate following `steps` is invalid, as witnessed by the provided `rup_info` and `rat_info`.
+In addition to the assurances on `rup_info` described above, `rat_info` provides that the identified pivot clause is not RUP.
+
+```ocaml
+predicate rat_failure (cnf : cnf) (info : rat_info) =
+    not (rat cnf info.rat_clause) /\
+    match info.rat_clause with
+    | Nil -> false
+    | Cons l _ ->
+        mem info.pivot_clause (pivot_clauses cnf l) /\
+        info.pivot_info.rup_clause = resolve info.rat_clause info.pivot_clause l /\
+        rup_failure cnf info.pivot_info
+    end
+```
+
+The derivation checker provides a similar contract, but rather than ensuring `valid_proof` on success, it provides `valid_derivation`.
+
+```ocaml
+predicate valid_derivation (cnf : cnf) (pf : proof) =
+    match pf with
+    | Nil -> true
+    | Cons c cs -> (rup cnf c \/ rat cnf c) /\ valid_derivation (Cons c cnf) cs
+    end
+```
+
+This is the same condition as `valid_proof`, but in the `Nil` case, the checker does not require that the empty clause is not RUP.
+
 ## Acknowledgements
 
-Many thanks to [Frank Pfenning](http://www.cs.cmu.edu/~fp/), [Joseph Reeves](https://www.cs.cmu.edu/~jereeves/), and [Marijn Huele](https://www.cs.cmu.edu/~mheule/) for the ongoing insightful discussions that led to this project.
+Many thanks to [Frank Pfenning](http://www.cs.cmu.edu/~fp/), [Joseph Reeves](https://www.cs.cmu.edu/~jereeves/), and [Marijn Huele](https://www.cs.cmu.edu/~mheule/) for the ongoing insightful discussions that led to this project.
```

### Comparing `drup-1.2.0/pyproject.toml` & `drup-1.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "drup"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="Matt Fredrikson", email="mfredrik@cmu.edu" },
 ]
 description = "Checks DRUP proofs against DIMACS source. Extracted from verified Why3 code."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: OCaml",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS :: MacOS X",
     "Topic :: Scientific/Engineering :: Mathematics"
-
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/cmu-transparency/verified_rup"
+"Documentation" = "https://fairlyaccountable.org/verified_rup/drup.html"
 "Bug Tracker" = "https://github.com/cmu-transparency/verified_rup/issues"
```

### Comparing `drup-1.2.0/setup.py` & `drup-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `drup-1.2.0/src/drup/__init__.py` & `drup-1.2.1/src/drup/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 .. include:: ../../README.md
 """
 
-__version__ = '1.2.0'
+__version__ = '1.2.1'
 
 import os
 import sys
 import ctypes
 
 _basedir = os.path.abspath(os.path.dirname(__file__))
 _checker = ctypes.cdll.LoadLibrary(os.path.join(_basedir, "libdrupchecker.so"))
```

### Comparing `drup-1.2.0/src/drup/cli.py` & `drup-1.2.1/src/drup/cli.py`

 * *Files identical despite different names*

### Comparing `drup-1.2.0/src/drup/libdrupchecker.so` & `drup-1.2.1/src/drup/libdrupchecker.so`

 * *Files identical despite different names*

### Comparing `drup-1.2.0/src/drup/wrappers.py` & `drup-1.2.1/src/drup/wrappers.py`

 * *Files identical despite different names*

