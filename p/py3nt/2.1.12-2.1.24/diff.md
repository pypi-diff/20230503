# Comparing `tmp/py3nt-2.1.12.tar.gz` & `tmp/py3nt-2.1.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3nt-2.1.12.tar", max compression
+gzip compressed data, was "py3nt-2.1.24.tar", max compression
```

## Comparing `py3nt-2.1.12.tar` & `py3nt-2.1.24.tar`

### file list

```diff
@@ -1,22 +1,25 @@
--rw-r--r--   0        0        0     1070 2023-02-19 22:28:44.113951 py3nt-2.1.12/LICENSE
--rw-r--r--   0        0        0      617 2023-02-19 22:28:44.113951 py3nt-2.1.12/README.md
--rw-r--r--   0        0        0        0 2023-02-19 22:28:44.113951 py3nt-2.1.12/py3nt/__init__.py
--rw-r--r--   0        0        0        0 2023-03-09 15:51:18.031217 py3nt-2.1.12/py3nt/congruence/__init__.py
--rw-r--r--   0        0        0     1409 2023-03-21 23:42:26.680828 py3nt-2.1.12/py3nt/congruence/quadratic.py
--rw-r--r--   0        0        0        0 2023-02-19 22:28:44.113951 py3nt-2.1.12/py3nt/core/__init__.py
--rw-r--r--   0        0        0     1732 2023-03-09 20:20:58.566920 py3nt-2.1.12/py3nt/core/base.py
--rw-r--r--   0        0        0     5632 2023-03-21 23:06:02.838079 py3nt-2.1.12/py3nt/core/factorize.py
--rw-r--r--   0        0        0     2969 2023-03-21 23:06:02.838079 py3nt-2.1.12/py3nt/core/primality_test.py
--rw-r--r--   0        0        0     2170 2023-03-09 20:20:58.566920 py3nt-2.1.12/py3nt/core/sieve.py
--rw-r--r--   0        0        0     3080 2023-03-09 20:20:58.570921 py3nt-2.1.12/py3nt/defaults.py
--rw-r--r--   0        0        0        0 2023-02-19 22:28:44.113951 py3nt-2.1.12/py3nt/functions/__init__.py
--rw-r--r--   0        0        0        0 2023-02-19 22:28:44.113951 py3nt-2.1.12/py3nt/functions/binary/__init__.py
--rw-r--r--   0        0        0        0 2023-02-19 22:28:44.113951 py3nt-2.1.12/py3nt/functions/unary/__init__.py
--rw-r--r--   0        0        0     2669 2023-03-12 20:48:49.542871 py3nt-2.1.12/py3nt/functions/unary/divisor_functions.py
--rw-r--r--   0        0        0     3675 2023-03-15 21:59:50.300329 py3nt-2.1.12/py3nt/functions/unary/totient.py
--rw-r--r--   0        0        0        0 2023-02-19 22:28:44.113951 py3nt-2.1.12/py3nt/numbers/__init__.py
--rw-r--r--   0        0        0     3848 2023-03-21 23:06:02.838079 py3nt-2.1.12/py3nt/numbers/integer.py
--rw-r--r--   0        0        0        0 2023-03-12 20:48:49.542871 py3nt-2.1.12/py3nt/polynomial/__init__.py
--rw-r--r--   0        0        0     3052 2023-03-18 18:37:08.431706 py3nt-2.1.12/py3nt/polynomial/binomial.py
--rw-r--r--   0        0        0     1076 2023-03-21 23:42:26.680828 py3nt-2.1.12/pyproject.toml
--rw-r--r--   0        0        0     1280 1970-01-01 00:00:00.000000 py3nt-2.1.12/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-02-19 22:28:44.113951 py3nt-2.1.24/LICENSE
+-rw-r--r--   0        0        0      618 2023-05-02 22:53:03.713718 py3nt-2.1.24/README.md
+-rw-r--r--   0        0        0        0 2023-02-19 22:28:44.113951 py3nt-2.1.24/py3nt/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-09 15:51:18.031217 py3nt-2.1.24/py3nt/congruence/__init__.py
+-rw-r--r--   0        0        0     3431 2023-04-14 10:01:16.597194 py3nt-2.1.24/py3nt/congruence/basics.py
+-rw-r--r--   0        0        0     2727 2023-04-17 20:57:24.753193 py3nt-2.1.24/py3nt/congruence/binomial.py
+-rw-r--r--   0        0        0     5778 2023-04-12 17:28:30.908112 py3nt-2.1.24/py3nt/congruence/primitives.py
+-rw-r--r--   0        0        0     1409 2023-03-21 23:42:26.680828 py3nt-2.1.24/py3nt/congruence/quadratic.py
+-rw-r--r--   0        0        0        0 2023-02-19 22:28:44.113951 py3nt-2.1.24/py3nt/core/__init__.py
+-rw-r--r--   0        0        0     1732 2023-03-09 20:20:58.566920 py3nt-2.1.24/py3nt/core/base.py
+-rw-r--r--   0        0        0     6157 2023-04-12 17:28:30.908112 py3nt-2.1.24/py3nt/core/factorize.py
+-rw-r--r--   0        0        0     2969 2023-03-21 23:06:02.838079 py3nt-2.1.24/py3nt/core/primality_test.py
+-rw-r--r--   0        0        0     2393 2023-04-17 20:57:24.753193 py3nt-2.1.24/py3nt/core/sieve.py
+-rw-r--r--   0        0        0     3080 2023-03-09 20:20:58.570921 py3nt-2.1.24/py3nt/defaults.py
+-rw-r--r--   0        0        0        0 2023-02-19 22:28:44.113951 py3nt-2.1.24/py3nt/functions/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-19 22:28:44.113951 py3nt-2.1.24/py3nt/functions/binary/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-19 22:28:44.113951 py3nt-2.1.24/py3nt/functions/unary/__init__.py
+-rw-r--r--   0        0        0     4506 2023-03-25 01:28:37.229355 py3nt-2.1.24/py3nt/functions/unary/divisor_functions.py
+-rw-r--r--   0        0        0     3675 2023-03-15 21:59:50.300329 py3nt-2.1.24/py3nt/functions/unary/totient.py
+-rw-r--r--   0        0        0        0 2023-02-19 22:28:44.113951 py3nt-2.1.24/py3nt/numbers/__init__.py
+-rw-r--r--   0        0        0     4576 2023-04-06 12:23:34.926464 py3nt-2.1.24/py3nt/numbers/integer.py
+-rw-r--r--   0        0        0        0 2023-03-12 20:48:49.542871 py3nt-2.1.24/py3nt/polynomial/__init__.py
+-rw-r--r--   0        0        0     3052 2023-03-18 18:37:08.431706 py3nt-2.1.24/py3nt/polynomial/binomial.py
+-rw-r--r--   0        0        0     1076 2023-05-02 22:53:22.629986 py3nt-2.1.24/pyproject.toml
+-rw-r--r--   0        0        0     1281 1970-01-01 00:00:00.000000 py3nt-2.1.24/PKG-INFO
```

### Comparing `py3nt-2.1.12/LICENSE` & `py3nt-2.1.24/LICENSE`

 * *Files identical despite different names*

### Comparing `py3nt-2.1.12/README.md` & `py3nt-2.1.24/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-# `pynt` A Number Theory Library for Python 3
+# `py3nt` A Number Theory Library for Python 3
 
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/math-projects/pynt/develop.svg)](https://results.pre-commit.ci/latest/github/math-projects/pynt/develop)
 ![Workflow for Codecov Action](https://github.com/math-projects/pynt/actions/workflows/codecov.yml/badge.svg)
 [![codecov](https://codecov.io/gh/math-projects/pynt/branch/develop/graph/badge.svg?token=12WCFBI23W)](https://codecov.io/gh/math-projects/pynt)
 [![Documentation Status](https://readthedocs.org/projects/py3nt/badge/?version=latest)](https://py3nt.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `py3nt-2.1.12/py3nt/congruence/quadratic.py` & `py3nt-2.1.24/py3nt/congruence/quadratic.py`

 * *Files identical despite different names*

### Comparing `py3nt-2.1.12/py3nt/core/base.py` & `py3nt-2.1.24/py3nt/core/base.py`

 * *Files identical despite different names*

### Comparing `py3nt-2.1.12/py3nt/core/factorize.py` & `py3nt-2.1.24/py3nt/core/factorize.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,42 @@
     LARGEST_SMALL_NUMBER,
     LOGN_PRIME_FACTOR_FIELD,
     MAX_LOGN_FACTORIZATION_LIMIT,
 )
 from py3nt.numbers.integer import Integer
 
 
+def is_prime_power(n: int) -> tuple[int, int]:
+    """Check if :math:`n` is a prime power or not.
+
+    Parameters
+    ----------
+    n : ``int``
+        A positive integer.
+
+    Returns
+    -------
+    tuple[int, int]
+        :math:`(p, e)` where :math:`n=p^{e}`.
+    """
+
+    if n < 2:
+        return (0, 0)
+
+    lim: int = int(np.log2(n))
+
+    for i in range(1, lim + 1):
+        root = Integer(n).kthroot(k=i)
+        if root**i == n:
+            if is_prime(root):
+                return (root, i)
+
+    return (0, lim)
+
+
 @dataclass
 class NaiveSqrtFactorization(BaseFactorization):
     """
     Factorize small numbers in sqrt(n) complexity.
 
     Methods
     -------
```

### Comparing `py3nt-2.1.12/py3nt/core/primality_test.py` & `py3nt-2.1.24/py3nt/core/primality_test.py`

 * *Files identical despite different names*

### Comparing `py3nt-2.1.12/py3nt/core/sieve.py` & `py3nt-2.1.24/py3nt/core/sieve.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 import numpy as np
 
 from py3nt.core.base import BaseSieve
 
 
 @dataclass
 class SieveOfEratosthenes(BaseSieve):
-    """
+    r"""
     Sieve of Eratosthenes for generating primes.
+    Usually used for factorizing by division of primes not exceeding :math:`\sqrt{n}`.
+    So, in most cases ``limit`` should be set to :math:`\ceil{\sqrt{n}}`.
 
     Methods
     -------
     generate_primes:
         Generate primes up to ``limit`` using sieve of Eratosthenes.
     """
 
@@ -34,16 +36,17 @@
                 self.primes_[prime_count] = i
                 prime_count += 1
                 flags[i * i : self.limit + 1 : i * 2] = 1
 
 
 @dataclass
 class SieveOfEratosthenesOptimized(BaseSieve):
-    """
-    We can store smallest prime factors for logn factorization.
+    r"""
+    We can store smallest prime factors for :math:`\log{n}` factorization.
+    Therefore, :math:`n` must be in sieve range.
 
     Methods
     -------
     generate_primes:
         Generate primes using pre-stored prime factors of positive integers.
     """
```

### Comparing `py3nt-2.1.12/py3nt/defaults.py` & `py3nt-2.1.24/py3nt/defaults.py`

 * *Files identical despite different names*

### Comparing `py3nt-2.1.12/py3nt/functions/unary/divisor_functions.py` & `py3nt-2.1.24/py3nt/functions/unary/divisor_functions.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,16 +4,21 @@
 
 import numpy as np
 
 from py3nt.core.factorize import FactorizationFactory
 from py3nt.polynomial.binomial import homogeneous_binomial
 
 
-def sigma_kth(n: int, k: int, factorizer: Optional[FactorizationFactory]) -> int:
-    r"""Calculate the number of divisors.
+def sigma_kth(
+    n: int,
+    k: int,
+    factorizer: Optional[FactorizationFactory],
+    factorization: Optional[dict[int, int]] = None,
+) -> int:
+    r"""Calculate the divisor sum function :math:`\sigma_{k}(n)=\sum_{d\mid n}d^{k}`.
 
     Parameters
     ----------
     n : ``int``
         A positive integer.
     k: ``int``
         A positive integer.
@@ -24,18 +29,19 @@
 
     Returns
     -------
     ``int``
         Divisor sigma function :math:`\sum_{d\mid n}d^{k}`.
     """
 
-    if factorizer:
-        factorization = factorizer.factorize(n=n)
-        print(n, k, factorization)
+    if not factorization:
+        if factorizer:
+            factorization = factorizer.factorize(n=n)
 
+    if factorization:
         if k == 0:
             return np.prod(a=np.array(list(factorization.values())) + 1)
 
         divisor_sigma = 1
         for prime, multiplicity in factorization.items():
             divisor_sigma *= homogeneous_binomial(a=pow(prime, k), b=1, n=multiplicity + 1)
 
@@ -50,15 +56,19 @@
             j = n // i
             if i != j:
                 divisor_sigma += pow(j, k)
 
     return divisor_sigma
 
 
-def number_of_divisors(n: int, factorizer: Optional[FactorizationFactory]) -> int:
+def number_of_divisors(
+    n: int,
+    factorizer: Optional[FactorizationFactory],
+    factorization: Optional[dict[int, int]] = None,
+) -> int:
     """
 
     Parameters
     ----------
     n : ``int``
         A positive integer.
     factorizer : ``FactorizationFactory``
@@ -68,18 +78,22 @@
 
     Returns
     -------
     ``int``
         Number of divisors of :math:`n`.
     """
 
-    return sigma_kth(n=n, k=0, factorizer=factorizer)
+    return sigma_kth(n=n, k=0, factorizer=factorizer, factorization=factorization)
 
 
-def sum_of_divisors(n: int, factorizer: Optional[FactorizationFactory]) -> int:
+def sum_of_divisors(
+    n: int,
+    factorizer: Optional[FactorizationFactory],
+    factorization: Optional[dict[int, int]] = None,
+) -> int:
     """
 
     Parameters
     ----------
     n : ``int``
         A positive integer.
     factorizer : ``FactorizationFactory``
@@ -89,8 +103,64 @@
 
     Returns
     -------
     ``int``
         Sum of divisors of :math:`n`.
     """
 
-    return sigma_kth(n=n, k=1, factorizer=factorizer)
+    return sigma_kth(n=n, k=1, factorizer=factorizer, factorization=factorization)
+
+
+def generate_divisors(
+    n: int,
+    factorizer: Optional[FactorizationFactory] = None,
+    factorization: Optional[dict[int, int]] = None,
+) -> np.ndarray:
+    r"""Generate all positive divisors of a positive integer.
+
+    Parameters
+    ----------
+    n : ``int``
+        A positive integer.
+    factorizer : ``Optional[FactorizationFactory], optional``
+        If specified, ``factorizer`` is used to factorize :math:`n`, by default ``None``.
+    factorization : ``Optional[dict[int, int]]``, optional
+        If specified, used as prime factorization of :math:`n`, by default ``None``.
+        Cannot be ``None`` if ``factorizer`` is also ``None``.
+
+    Returns
+    -------
+    ``np.ndarray``
+        An unsorted numpy array of divisors: :math:`{d\in\mathbb{N}:d\mid n}`.
+
+    Raises
+    ------
+    ``ValueError``
+        If both ``factorizer`` and ``factorizer`` are ``None``.
+    """
+
+    if not factorization:
+        if not factorizer:
+            raise ValueError("`factorizer` cannot be None")
+
+        factorization = factorizer.factorize(n=n)
+
+    divisors = np.empty(
+        shape=(number_of_divisors(n=n, factorization=factorization, factorizer=None)),
+        dtype=int,
+    )
+
+    tau = 1
+    divisors[0] = 1
+
+    for prime, multiplicity in factorization.items():
+        cur = 1
+        tau_tmp = tau
+
+        for _ in range(multiplicity):
+            cur *= prime
+
+            for i in range(tau_tmp):
+                divisors[tau] = divisors[i] * cur
+                tau += 1
+
+    return divisors
```

### Comparing `py3nt-2.1.12/py3nt/functions/unary/totient.py` & `py3nt-2.1.24/py3nt/functions/unary/totient.py`

 * *Files identical despite different names*

### Comparing `py3nt-2.1.12/py3nt/numbers/integer.py` & `py3nt-2.1.24/py3nt/numbers/integer.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,14 +54,46 @@
             if cur > modulus:
                 cur -= modulus
 
         remainder %= modulus
 
         return remainder
 
+    def kthroot(self, k: int) -> int:
+        r"""
+
+        Parameters
+        ----------
+        k : ``int``
+            A positive integer.
+
+        Returns
+        -------
+        ``int``
+            A positive integer :math:`r` such that :math:`r^{k}\leq n<r^{k+1}`.
+        """
+
+        high = 1
+        while pow(high, k) < self:
+            high <<= 1
+        low = high >> 1
+        while high - low > 1:
+            mid = (low + high) >> 1
+            cur = pow(mid, k)
+            if cur < self:
+                low = mid
+            elif self < cur:
+                high = mid
+            else:
+                return mid
+        if pow(high, k) == self:
+            return high
+        else:
+            return low
+
     def __pow__(self, exponent: int, modulus=None):
         if not modulus:
             return pow(int(self), int(exponent))
 
         return pow(int(self), int(exponent), int(modulus))
 
     def pollard_rho_factor(self, a: int, c: int, max_iter: int = 5) -> int:
```

### Comparing `py3nt-2.1.12/py3nt/polynomial/binomial.py` & `py3nt-2.1.24/py3nt/polynomial/binomial.py`

 * *Files identical despite different names*

### Comparing `py3nt-2.1.12/pyproject.toml` & `py3nt-2.1.24/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py3nt"
-version = "2.1.12"
+version = "2.1.24"
 description = "A Number Theory Library for Python 3"
 authors = ["Masum Billal <billalmasum93@gmail.com>"]
 
 license = "MIT"
 
 readme = "README.md"
 repository = "https://github.com/math-projects/pynt"
```

### Comparing `py3nt-2.1.12/PKG-INFO` & `py3nt-2.1.24/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3nt
-Version: 2.1.12
+Version: 2.1.24
 Summary: A Number Theory Library for Python 3
 Home-page: https://github.com/math-projects/pynt
 License: MIT
 Author: Masum Billal
 Author-email: billalmasum93@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.2)
 Requires-Dist: sympy (>=1.11)
 Project-URL: Repository, https://github.com/math-projects/pynt
 Description-Content-Type: text/markdown
 
-# `pynt` A Number Theory Library for Python 3
+# `py3nt` A Number Theory Library for Python 3
 
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/math-projects/pynt/develop.svg)](https://results.pre-commit.ci/latest/github/math-projects/pynt/develop)
 ![Workflow for Codecov Action](https://github.com/math-projects/pynt/actions/workflows/codecov.yml/badge.svg)
 [![codecov](https://codecov.io/gh/math-projects/pynt/branch/develop/graph/badge.svg?token=12WCFBI23W)](https://codecov.io/gh/math-projects/pynt)
 [![Documentation Status](https://readthedocs.org/projects/py3nt/badge/?version=latest)](https://py3nt.readthedocs.io/en/latest/?badge=latest)
```

