# Comparing `tmp/moneycounter-1.2.2.tar.gz` & `tmp/moneycounter-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneycounter-1.2.2.tar", last modified: Fri Mar 24 22:03:11 2023, max compression
+gzip compressed data, was "moneycounter-1.2.3.tar", last modified: Wed May  3 00:32:03 2023, max compression
```

## Comparing `moneycounter-1.2.2.tar` & `moneycounter-1.2.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 ms         (501) staff       (20)        0 2023-03-24 22:03:11.561915 moneycounter-1.2.2/
-drwxr-xr-x   0 ms         (501) staff       (20)        0 2023-03-24 22:03:11.557316 moneycounter-1.2.2/.github/
-drwxr-xr-x   0 ms         (501) staff       (20)        0 2023-03-24 22:03:11.559490 moneycounter-1.2.2/.github/workflows/
--rw-r--r--   0 ms         (501) staff       (20)      560 2023-03-21 16:43:58.000000 moneycounter-1.2.2/.github/workflows/ci_testing.yml
--rw-r--r--   0 ms         (501) staff       (20)      277 2022-12-20 17:19:48.000000 moneycounter-1.2.2/.github/workflows/prune.yml
--rw-r--r--   0 ms         (501) staff       (20)       85 2023-03-23 22:44:45.000000 moneycounter-1.2.2/.gitignore
--rw-r--r--   0 ms         (501) staff       (20)     2248 2023-03-24 22:03:11.562028 moneycounter-1.2.2/PKG-INFO
--rw-r--r--   0 ms         (501) staff       (20)     1520 2023-03-02 13:52:40.000000 moneycounter-1.2.2/README.md
--rw-r--r--   0 ms         (501) staff       (20)      186 2022-12-21 19:34:58.000000 moneycounter-1.2.2/pypi.md
--rw-r--r--   0 ms         (501) staff       (20)      913 2023-03-24 22:02:56.000000 moneycounter-1.2.2/pyproject.toml
--rw-r--r--   0 ms         (501) staff       (20)      145 2023-03-21 16:43:58.000000 moneycounter-1.2.2/requirements.txt
--rw-r--r--   0 ms         (501) staff       (20)      418 2023-03-24 22:03:11.562295 moneycounter-1.2.2/setup.cfg
-drwxr-xr-x   0 ms         (501) staff       (20)        0 2023-03-24 22:03:11.557535 moneycounter-1.2.2/src/
-drwxr-xr-x   0 ms         (501) staff       (20)        0 2023-03-24 22:03:11.559896 moneycounter-1.2.2/src/moneycounter/
--rw-r--r--   0 ms         (501) staff       (20)       57 2023-03-24 22:02:56.000000 moneycounter-1.2.2/src/moneycounter/__init__.py
--rw-r--r--   0 ms         (501) staff       (20)     6462 2023-03-24 19:50:19.000000 moneycounter-1.2.2/src/moneycounter/pnl.py
-drwxr-xr-x   0 ms         (501) staff       (20)        0 2023-03-24 22:03:11.560595 moneycounter-1.2.2/src/moneycounter.egg-info/
--rw-r--r--   0 ms         (501) staff       (20)     2248 2023-03-24 22:03:11.000000 moneycounter-1.2.2/src/moneycounter.egg-info/PKG-INFO
--rw-r--r--   0 ms         (501) staff       (20)      462 2023-03-24 22:03:11.000000 moneycounter-1.2.2/src/moneycounter.egg-info/SOURCES.txt
--rw-r--r--   0 ms         (501) staff       (20)        1 2023-03-24 22:03:11.000000 moneycounter-1.2.2/src/moneycounter.egg-info/dependency_links.txt
--rw-r--r--   0 ms         (501) staff       (20)       27 2023-03-24 22:03:11.000000 moneycounter-1.2.2/src/moneycounter.egg-info/requires.txt
--rw-r--r--   0 ms         (501) staff       (20)       13 2023-03-24 22:03:11.000000 moneycounter-1.2.2/src/moneycounter.egg-info/top_level.txt
-drwxr-xr-x   0 ms         (501) staff       (20)        0 2023-03-24 22:03:11.561159 moneycounter-1.2.2/tests/
--rw-r--r--   0 ms         (501) staff       (20)     3998 2023-03-24 21:51:08.000000 moneycounter-1.2.2/tests/pnl_tests.py
--rw-r--r--   0 ms         (501) staff       (20)      944 2023-03-24 22:02:56.000000 moneycounter-1.2.2/tests/realized_tests.py
--rw-r--r--   0 ms         (501) staff       (20)      844 2023-03-21 16:43:58.000000 moneycounter-1.2.2/tests/test_base.py
--rw-r--r--   0 ms         (501) staff       (20)     7553 2023-03-24 22:02:56.000000 moneycounter-1.2.2/tests/trades.csv
+drwxr-xr-x   0 ms         (501) staff       (20)        0 2023-05-03 00:32:03.176882 moneycounter-1.2.3/
+drwxr-xr-x   0 ms         (501) staff       (20)        0 2023-05-03 00:32:03.171866 moneycounter-1.2.3/.github/
+drwxr-xr-x   0 ms         (501) staff       (20)        0 2023-05-03 00:32:03.174049 moneycounter-1.2.3/.github/workflows/
+-rw-r--r--   0 ms         (501) staff       (20)      560 2023-03-21 16:43:58.000000 moneycounter-1.2.3/.github/workflows/ci_testing.yml
+-rw-r--r--   0 ms         (501) staff       (20)      277 2022-12-20 17:19:48.000000 moneycounter-1.2.3/.github/workflows/prune.yml
+-rw-r--r--   0 ms         (501) staff       (20)       85 2023-03-23 22:44:45.000000 moneycounter-1.2.3/.gitignore
+-rw-r--r--   0 ms         (501) staff       (20)     2248 2023-05-03 00:32:03.176982 moneycounter-1.2.3/PKG-INFO
+-rw-r--r--   0 ms         (501) staff       (20)     1520 2023-03-02 13:52:40.000000 moneycounter-1.2.3/README.md
+-rw-r--r--   0 ms         (501) staff       (20)      186 2022-12-21 19:34:58.000000 moneycounter-1.2.3/pypi.md
+-rw-r--r--   0 ms         (501) staff       (20)      913 2023-05-03 00:31:18.000000 moneycounter-1.2.3/pyproject.toml
+-rw-r--r--   0 ms         (501) staff       (20)      145 2023-03-21 16:43:58.000000 moneycounter-1.2.3/requirements.txt
+-rw-r--r--   0 ms         (501) staff       (20)      418 2023-05-03 00:32:03.177261 moneycounter-1.2.3/setup.cfg
+drwxr-xr-x   0 ms         (501) staff       (20)        0 2023-05-03 00:32:03.172078 moneycounter-1.2.3/src/
+drwxr-xr-x   0 ms         (501) staff       (20)        0 2023-05-03 00:32:03.174754 moneycounter-1.2.3/src/moneycounter/
+-rw-r--r--   0 ms         (501) staff       (20)       57 2023-03-24 22:02:56.000000 moneycounter-1.2.3/src/moneycounter/__init__.py
+-rw-r--r--   0 ms         (501) staff       (20)     6468 2023-05-03 00:31:18.000000 moneycounter-1.2.3/src/moneycounter/pnl.py
+drwxr-xr-x   0 ms         (501) staff       (20)        0 2023-05-03 00:32:03.175630 moneycounter-1.2.3/src/moneycounter.egg-info/
+-rw-r--r--   0 ms         (501) staff       (20)     2248 2023-05-03 00:32:03.000000 moneycounter-1.2.3/src/moneycounter.egg-info/PKG-INFO
+-rw-r--r--   0 ms         (501) staff       (20)      462 2023-05-03 00:32:03.000000 moneycounter-1.2.3/src/moneycounter.egg-info/SOURCES.txt
+-rw-r--r--   0 ms         (501) staff       (20)        1 2023-05-03 00:32:03.000000 moneycounter-1.2.3/src/moneycounter.egg-info/dependency_links.txt
+-rw-r--r--   0 ms         (501) staff       (20)       27 2023-05-03 00:32:03.000000 moneycounter-1.2.3/src/moneycounter.egg-info/requires.txt
+-rw-r--r--   0 ms         (501) staff       (20)       13 2023-05-03 00:32:03.000000 moneycounter-1.2.3/src/moneycounter.egg-info/top_level.txt
+drwxr-xr-x   0 ms         (501) staff       (20)        0 2023-05-03 00:32:03.176628 moneycounter-1.2.3/tests/
+-rw-r--r--   0 ms         (501) staff       (20)     4253 2023-05-03 00:31:18.000000 moneycounter-1.2.3/tests/pnl_tests.py
+-rw-r--r--   0 ms         (501) staff       (20)      944 2023-03-24 22:02:56.000000 moneycounter-1.2.3/tests/realized_tests.py
+-rw-r--r--   0 ms         (501) staff       (20)     1224 2023-05-03 00:31:18.000000 moneycounter-1.2.3/tests/test_base.py
+-rw-r--r--   0 ms         (501) staff       (20)     7553 2023-03-24 22:02:56.000000 moneycounter-1.2.3/tests/trades.csv
```

### Comparing `moneycounter-1.2.2/.github/workflows/ci_testing.yml` & `moneycounter-1.2.3/.github/workflows/ci_testing.yml`

 * *Files identical despite different names*

### Comparing `moneycounter-1.2.2/PKG-INFO` & `moneycounter-1.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneycounter
-Version: 1.2.2
+Version: 1.2.3
 Summary: Portfolio Analytics Utilities
 Author-email: Marc Schwarzschild <ms@TheBrookhavenGroup.com>
 Maintainer-email: Marc Schwarzschild <ms@TheBrookhavenGroup.com>
 License: MIT
 Project-URL: homepage, https://github.com/schwarzschild/moneycounter
 Project-URL: repository, https://github.com/schwarzschild/moneycounter
 Project-URL: documentation, https://github.com/schwarzschild/moneycounter
```

### Comparing `moneycounter-1.2.2/README.md` & `moneycounter-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `moneycounter-1.2.2/pyproject.toml` & `moneycounter-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,13 +13,13 @@
 classifiers = [
     "Topic :: Office/Business :: Financial",
     "Topic :: Office/Business :: Financial :: Accounting",
     "Topic :: Office/Business :: Financial :: Investment"
     ]
 license = {text = "MIT"}
 dependencies = ["pandas==1.5.2", "pytz==2022.7"]
-version = "1.2.2"
+version = "1.2.3"
 
 [project.urls]
 homepage = "https://github.com/schwarzschild/moneycounter"
 repository = "https://github.com/schwarzschild/moneycounter"
 documentation = "https://github.com/schwarzschild/moneycounter"
```

### Comparing `moneycounter-1.2.2/src/moneycounter/pnl.py` & `moneycounter-1.2.3/src/moneycounter/pnl.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,16 +33,16 @@
     df['csum'] = df.q.cumsum()
 
     split_trades = df[split_trades_flags]
 
     for index, row in split_trades.iterrows():
         denominator = row.csum - row.q
         factor = row.csum / denominator
-        df.iloc[:index].q *= factor
-        df.iloc[:index].p /= factor
+        df.loc[:index, 'q'] *= factor
+        df.loc[:index, 'p'] /= factor
 
     df = df[~split_trades_flags]
     df.drop(['csum'], axis=1)
 
     df.reset_index(drop=True, inplace=True)
 
     return df
@@ -86,15 +86,15 @@
 
     sells = df[df.q < 0]
 
     for index, row in sells.iterrows():
         q = -row.q
         flags = csum > q
         i = df[flags].index[0]
-        df.q.iloc[:i] = 0
+        df.loc[:i, 'q'] = 0
         residual = csum.iloc[i] - q
         if not is_near_zero(residual):
             df.at[i, 'q'] = residual
         df.at[index, 'q'] = 0
 
         csum = df.q.cumsum()
```

### Comparing `moneycounter-1.2.2/src/moneycounter.egg-info/PKG-INFO` & `moneycounter-1.2.3/src/moneycounter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneycounter
-Version: 1.2.2
+Version: 1.2.3
 Summary: Portfolio Analytics Utilities
 Author-email: Marc Schwarzschild <ms@TheBrookhavenGroup.com>
 Maintainer-email: Marc Schwarzschild <ms@TheBrookhavenGroup.com>
 License: MIT
 Project-URL: homepage, https://github.com/schwarzschild/moneycounter
 Project-URL: repository, https://github.com/schwarzschild/moneycounter
 Project-URL: documentation, https://github.com/schwarzschild/moneycounter
```

### Comparing `moneycounter-1.2.2/tests/pnl_tests.py` & `moneycounter-1.2.3/tests/pnl_tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from test_base import TradesBaseTest
+from test_base import TradesBaseTest, fake_trades
 from src.moneycounter.pnl import unrealized, wap_calc, pnl_calc, split_adjust, fifo_remove, pnl
 
 
 class PnLTests(TradesBaseTest):
 
     def test_pnl(self):
         for a, t, r, u in (('ACCNT1', 'TICKER1', 700, -3090),
@@ -95,7 +95,17 @@
             flag = df.q >= 0
         flag = flag.any()
         self.assertFalse(flag, msg='Make sure closed trades were removed.')
 
     def test_fifo_remove(self):
         self.fifo_remove_helper('ACCNT7')
         self.fifo_remove_helper('ACCNT8')
+
+
+class BigTests(TradesBaseTest):
+    def test_wap(self):
+        print('Making fake trades.')
+        # df = fake_trades(1_000_000)
+        df = fake_trades(10)
+        print('Calculating WAP.')
+        wap = wap_calc(df)
+        print(wap)
```

### Comparing `moneycounter-1.2.2/tests/realized_tests.py` & `moneycounter-1.2.3/tests/realized_tests.py`

 * *Files identical despite different names*

### Comparing `moneycounter-1.2.2/tests/trades.csv` & `moneycounter-1.2.3/tests/trades.csv`

 * *Files identical despite different names*

