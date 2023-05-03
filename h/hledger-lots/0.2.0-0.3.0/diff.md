# Comparing `tmp/hledger_lots-0.2.0.tar.gz` & `tmp/hledger_lots-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hledger_lots-0.2.0.tar", last modified: Sun Apr 30 16:22:23 2023, max compression
+gzip compressed data, was "hledger_lots-0.3.0.tar", last modified: Wed May  3 17:00:37 2023, max compression
```

## Comparing `hledger_lots-0.2.0.tar` & `hledger_lots-0.3.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-30 16:22:23.383155 hledger_lots-0.2.0/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5729 2023-04-30 16:22:23.382155 hledger_lots-0.2.0/PKG-INFO
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-30 16:22:23.366155 hledger_lots-0.2.0/docs/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5389 2023-04-30 16:01:03.000000 hledger_lots-0.2.0/docs/README.md
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-30 16:22:23.369155 hledger_lots-0.2.0/hledger_lots/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:22:25.000000 hledger_lots-0.2.0/hledger_lots/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       85 2023-04-18 19:22:25.000000 hledger_lots-0.2.0/hledger_lots/__main__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2957 2023-04-23 02:50:39.000000 hledger_lots-0.2.0/hledger_lots/avg.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2719 2023-04-30 16:01:03.000000 hledger_lots-0.2.0/hledger_lots/avg_info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1393 2023-04-18 19:22:25.000000 hledger_lots-0.2.0/hledger_lots/checks.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)    13624 2023-04-30 16:17:25.000000 hledger_lots-0.2.0/hledger_lots/cli.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3732 2023-04-23 02:50:39.000000 hledger_lots-0.2.0/hledger_lots/fifo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3245 2023-04-30 16:01:03.000000 hledger_lots-0.2.0/hledger_lots/fifo_info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      913 2023-04-30 16:01:03.000000 hledger_lots-0.2.0/hledger_lots/files.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1709 2023-04-18 19:22:25.000000 hledger_lots-0.2.0/hledger_lots/hl.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4318 2023-04-30 16:01:03.000000 hledger_lots-0.2.0/hledger_lots/info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2758 2023-04-24 18:30:26.000000 hledger_lots-0.2.0/hledger_lots/lib.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3749 2023-04-24 18:30:26.000000 hledger_lots-0.2.0/hledger_lots/prices_yahoo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     7340 2023-04-30 16:01:03.000000 hledger_lots-0.2.0/hledger_lots/prompt.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4158 2023-04-30 16:01:03.000000 hledger_lots-0.2.0/hledger_lots/prompt_buy.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3374 2023-04-30 16:01:03.000000 hledger_lots-0.2.0/hledger_lots/prompt_sell.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-30 16:22:23.370155 hledger_lots-0.2.0/hledger_lots.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5729 2023-04-30 16:22:23.000000 hledger_lots-0.2.0/hledger_lots.egg-info/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1081 2023-04-30 16:22:23.000000 hledger_lots-0.2.0/hledger_lots.egg-info/SOURCES.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-04-30 16:22:23.000000 hledger_lots-0.2.0/hledger_lots.egg-info/dependency_links.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-04-30 16:22:23.000000 hledger_lots-0.2.0/hledger_lots.egg-info/entry_points.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       78 2023-04-30 16:22:23.000000 hledger_lots-0.2.0/hledger_lots.egg-info/requires.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       45 2023-04-30 16:22:23.000000 hledger_lots-0.2.0/hledger_lots.egg-info/top_level.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1255 2023-04-30 16:20:54.000000 hledger_lots-0.2.0/pyproject.toml
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-04-30 16:22:23.383155 hledger_lots-0.2.0/setup.cfg
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-30 16:22:23.378155 hledger_lots-0.2.0/tests/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:22:25.000000 hledger_lots-0.2.0/tests/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5566 2023-04-18 19:22:25.000000 hledger_lots-0.2.0/tests/lots_data.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      192 2023-04-18 19:22:25.000000 hledger_lots-0.2.0/tests/test__main__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4562 2023-04-23 02:50:39.000000 hledger_lots-0.2.0/tests/test_avg.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3205 2023-04-30 16:01:03.000000 hledger_lots-0.2.0/tests/test_checks.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2565 2023-04-23 02:50:39.000000 hledger_lots-0.2.0/tests/test_fifo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-04-30 16:01:03.000000 hledger_lots-0.2.0/tests/test_files.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-18 19:22:25.000000 hledger_lots-0.2.0/tests/test_hl.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-18 19:22:25.000000 hledger_lots-0.2.0/tests/test_info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2136 2023-04-18 19:22:25.000000 hledger_lots-0.2.0/tests/test_lib.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-30 16:22:23.365155 hledger_lots-0.2.0/venv/
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-30 16:22:23.382155 hledger_lots-0.2.0/venv/bin/
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-04-18 19:23:23.000000 hledger_lots-0.2.0/venv/bin/rst2html.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-04-18 19:23:23.000000 hledger_lots-0.2.0/venv/bin/rst2html4.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-04-18 19:23:23.000000 hledger_lots-0.2.0/venv/bin/rst2html5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-04-18 19:23:23.000000 hledger_lots-0.2.0/venv/bin/rst2latex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-04-18 19:23:23.000000 hledger_lots-0.2.0/venv/bin/rst2man.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-04-18 19:23:23.000000 hledger_lots-0.2.0/venv/bin/rst2odt.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-04-18 19:23:23.000000 hledger_lots-0.2.0/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-04-18 19:23:23.000000 hledger_lots-0.2.0/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-04-18 19:23:23.000000 hledger_lots-0.2.0/venv/bin/rst2s5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-04-18 19:23:23.000000 hledger_lots-0.2.0/venv/bin/rst2xetex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-04-18 19:23:23.000000 hledger_lots-0.2.0/venv/bin/rst2xml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-04-18 19:23:23.000000 hledger_lots-0.2.0/venv/bin/rstpep2html.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-03 17:00:37.412625 hledger_lots-0.3.0/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5683 2023-05-03 17:00:37.412625 hledger_lots-0.3.0/PKG-INFO
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-03 17:00:37.403625 hledger_lots-0.3.0/docs/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5343 2023-05-03 16:08:12.000000 hledger_lots-0.3.0/docs/README.md
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-03 17:00:37.406625 hledger_lots-0.3.0/hledger_lots/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:22:25.000000 hledger_lots-0.3.0/hledger_lots/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       85 2023-04-18 19:22:25.000000 hledger_lots-0.3.0/hledger_lots/__main__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2957 2023-04-23 02:50:39.000000 hledger_lots-0.3.0/hledger_lots/avg.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2719 2023-04-30 16:01:03.000000 hledger_lots-0.3.0/hledger_lots/avg_info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1393 2023-04-18 19:22:25.000000 hledger_lots-0.3.0/hledger_lots/checks.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)    13625 2023-05-03 16:08:12.000000 hledger_lots-0.3.0/hledger_lots/cli.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1589 2023-05-03 16:08:12.000000 hledger_lots-0.3.0/hledger_lots/commodity_tag.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3732 2023-04-23 02:50:39.000000 hledger_lots-0.3.0/hledger_lots/fifo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3245 2023-04-30 16:01:03.000000 hledger_lots-0.3.0/hledger_lots/fifo_info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      913 2023-04-30 16:01:03.000000 hledger_lots-0.3.0/hledger_lots/files.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1709 2023-04-18 19:22:25.000000 hledger_lots-0.3.0/hledger_lots/hl.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4277 2023-05-03 16:08:12.000000 hledger_lots-0.3.0/hledger_lots/info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2758 2023-04-24 18:30:26.000000 hledger_lots-0.3.0/hledger_lots/lib.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4161 2023-05-03 16:08:12.000000 hledger_lots-0.3.0/hledger_lots/prices_yahoo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     7340 2023-04-30 16:01:03.000000 hledger_lots-0.3.0/hledger_lots/prompt.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4158 2023-04-30 16:01:03.000000 hledger_lots-0.3.0/hledger_lots/prompt_buy.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3374 2023-04-30 16:01:03.000000 hledger_lots-0.3.0/hledger_lots/prompt_sell.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-03 17:00:37.407625 hledger_lots-0.3.0/hledger_lots.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5683 2023-05-03 17:00:37.000000 hledger_lots-0.3.0/hledger_lots.egg-info/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1111 2023-05-03 17:00:37.000000 hledger_lots-0.3.0/hledger_lots.egg-info/SOURCES.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-05-03 17:00:37.000000 hledger_lots-0.3.0/hledger_lots.egg-info/dependency_links.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-05-03 17:00:37.000000 hledger_lots-0.3.0/hledger_lots.egg-info/entry_points.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       78 2023-05-03 17:00:37.000000 hledger_lots-0.3.0/hledger_lots.egg-info/requires.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       45 2023-05-03 17:00:37.000000 hledger_lots-0.3.0/hledger_lots.egg-info/top_level.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1255 2023-05-03 16:56:13.000000 hledger_lots-0.3.0/pyproject.toml
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-05-03 17:00:37.412625 hledger_lots-0.3.0/setup.cfg
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-03 17:00:37.409625 hledger_lots-0.3.0/tests/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:22:25.000000 hledger_lots-0.3.0/tests/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5566 2023-04-18 19:22:25.000000 hledger_lots-0.3.0/tests/lots_data.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      192 2023-04-18 19:22:25.000000 hledger_lots-0.3.0/tests/test__main__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4562 2023-04-23 02:50:39.000000 hledger_lots-0.3.0/tests/test_avg.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3205 2023-04-30 16:01:03.000000 hledger_lots-0.3.0/tests/test_checks.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2565 2023-04-23 02:50:39.000000 hledger_lots-0.3.0/tests/test_fifo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-04-30 16:01:03.000000 hledger_lots-0.3.0/tests/test_files.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-18 19:22:25.000000 hledger_lots-0.3.0/tests/test_hl.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-18 19:22:25.000000 hledger_lots-0.3.0/tests/test_info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2136 2023-04-18 19:22:25.000000 hledger_lots-0.3.0/tests/test_lib.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-03 17:00:37.402625 hledger_lots-0.3.0/venv/
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-03 17:00:37.412625 hledger_lots-0.3.0/venv/bin/
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-04-18 19:23:23.000000 hledger_lots-0.3.0/venv/bin/rst2html.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-04-18 19:23:23.000000 hledger_lots-0.3.0/venv/bin/rst2html4.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-04-18 19:23:23.000000 hledger_lots-0.3.0/venv/bin/rst2html5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-04-18 19:23:23.000000 hledger_lots-0.3.0/venv/bin/rst2latex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-04-18 19:23:23.000000 hledger_lots-0.3.0/venv/bin/rst2man.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-04-18 19:23:23.000000 hledger_lots-0.3.0/venv/bin/rst2odt.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-04-18 19:23:23.000000 hledger_lots-0.3.0/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-04-18 19:23:23.000000 hledger_lots-0.3.0/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-04-18 19:23:23.000000 hledger_lots-0.3.0/venv/bin/rst2s5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-04-18 19:23:23.000000 hledger_lots-0.3.0/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-04-18 19:23:23.000000 hledger_lots-0.3.0/venv/bin/rst2xml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-04-18 19:23:23.000000 hledger_lots-0.3.0/venv/bin/rstpep2html.py
```

### Comparing `hledger_lots-0.2.0/PKG-INFO` & `hledger_lots-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hledger_lots
-Version: 0.2.0
+Version: 0.3.0
 License: MIT License
 Project-URL: homepage, https://github.com/edkedk99/hledger-lots
 Project-URL: documentation, https://edkedk99.github.io/hledger-lots/
 Project-URL: repository, https://github.com/edkedk99/hledger-lots
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -32,17 +32,17 @@
 
 You can choose between two diferrent methods to calculate the cost of selling lots:
 
 - **FIFO**: First In First Out
 - **AVERAGE COST**: Average Cost of all previous purchase. It is as if selling a proportional part of each previous sale.
 
 
-### Update Price
+### Automatic Price Download
 
-After having the correct cost and result for selling a commodity, we want to follow the investment performance using market data. This package can download market price history from [Yahoo Finance](https://finance.yahoo.com/) and append [price directive](https://hledger.org/1.29/hledger.html#p-directive) to the journal just by following the required format when naming the commodity. More information [here](market_prices/)
+One simple command to automatically download market price from [Yahoo Finance](https://finance.yahoo.com/) for choosen commodities as explained [here](market_prices/). 
 
 ### Reports
 
 To get information about the commodities, there is more 2 commands:
 
 | command                          | description                                          |
 |----------------------------------|------------------------------------------------------|
@@ -67,17 +67,18 @@
 
 ```python
 pip install --upgrade hledger-lots
 ```
 
 ## Workflow
 
-1. Add purchase using the command [buy](usage/#buy) or edit the journal as usual using "@" notation. **Don't bother creating subaccounts or tags with unique lot name**. See the some examples [here](examples/data.journal)
-2. When you sell, use the command [sell](usage/#sell) instead of adding the transactions manually. Hledger-lots will generate the correct transaction and append to the selected journal if you confirm the transaction is correct. *See transaction tags with interesting indicators about the current trade*
-3. View financial indicators for a specific commodity using [view](usage/#view) or a summary of all commodities using [list](usage/$list). Optionally update market prices from [Yahoo Finance](https://finance.yahoo.com/) using the flag *--apend-prices-to [file path]*
+1. Add purchase using the command [buy](usage/#hledger-lots-buy) or edit the journal as usual using "@" notation. **Don't bother creating subaccounts or tags with unique lot name**. See the some examples [here](examples/data.journal)
+2. Download market price history as [price directive](https://hledger.org/1.29/hledger.html#p-directive) using the command [prices](usage/#hledger-lots-prices)
+3. View financial indicators for a specific commodity using [view](usage/#hledger-lots-view) or a summary of all commodities using [list](usage/$list). Optionally update market prices from [Yahoo Finance](https://finance.yahoo.com/) using the flag *--apend-prices-to [file path]*
+4. When you sell, use the command [sell](usage/#hledger-lots-sell) instead of adding the transactions manually. Hledger-lots will generate the correct transaction and append to the selected journal if you confirm the transaction is correct. *See transaction tags with interesting indicators about the current trade*
 
 > By default the sale is created using *FIFO* method. Use the option flag "--avg-cost" to change it to *Average Cost*
 
 
 ## Indicators
   
 ### Basic Indicators
```

### Comparing `hledger_lots-0.2.0/docs/README.md` & `hledger_lots-0.3.0/docs/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 
 You can choose between two diferrent methods to calculate the cost of selling lots:
 
 - **FIFO**: First In First Out
 - **AVERAGE COST**: Average Cost of all previous purchase. It is as if selling a proportional part of each previous sale.
 
 
-### Update Price
+### Automatic Price Download
 
-After having the correct cost and result for selling a commodity, we want to follow the investment performance using market data. This package can download market price history from [Yahoo Finance](https://finance.yahoo.com/) and append [price directive](https://hledger.org/1.29/hledger.html#p-directive) to the journal just by following the required format when naming the commodity. More information [here](market_prices/)
+One simple command to automatically download market price from [Yahoo Finance](https://finance.yahoo.com/) for choosen commodities as explained [here](market_prices/). 
 
 ### Reports
 
 To get information about the commodities, there is more 2 commands:
 
 | command                          | description                                          |
 |----------------------------------|------------------------------------------------------|
@@ -57,17 +57,18 @@
 
 ```python
 pip install --upgrade hledger-lots
 ```
 
 ## Workflow
 
-1. Add purchase using the command [buy](usage/#buy) or edit the journal as usual using "@" notation. **Don't bother creating subaccounts or tags with unique lot name**. See the some examples [here](examples/data.journal)
-2. When you sell, use the command [sell](usage/#sell) instead of adding the transactions manually. Hledger-lots will generate the correct transaction and append to the selected journal if you confirm the transaction is correct. *See transaction tags with interesting indicators about the current trade*
-3. View financial indicators for a specific commodity using [view](usage/#view) or a summary of all commodities using [list](usage/$list). Optionally update market prices from [Yahoo Finance](https://finance.yahoo.com/) using the flag *--apend-prices-to [file path]*
+1. Add purchase using the command [buy](usage/#hledger-lots-buy) or edit the journal as usual using "@" notation. **Don't bother creating subaccounts or tags with unique lot name**. See the some examples [here](examples/data.journal)
+2. Download market price history as [price directive](https://hledger.org/1.29/hledger.html#p-directive) using the command [prices](usage/#hledger-lots-prices)
+3. View financial indicators for a specific commodity using [view](usage/#hledger-lots-view) or a summary of all commodities using [list](usage/$list). Optionally update market prices from [Yahoo Finance](https://finance.yahoo.com/) using the flag *--apend-prices-to [file path]*
+4. When you sell, use the command [sell](usage/#hledger-lots-sell) instead of adding the transactions manually. Hledger-lots will generate the correct transaction and append to the selected journal if you confirm the transaction is correct. *See transaction tags with interesting indicators about the current trade*
 
 > By default the sale is created using *FIFO* method. Use the option flag "--avg-cost" to change it to *Average Cost*
 
 
 ## Indicators
   
 ### Basic Indicators
```

### Comparing `hledger_lots-0.2.0/hledger_lots/avg.py` & `hledger_lots-0.3.0/hledger_lots/avg.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/hledger_lots/avg_info.py` & `hledger_lots-0.3.0/hledger_lots/avg_info.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/hledger_lots/checks.py` & `hledger_lots-0.3.0/hledger_lots/checks.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/hledger_lots/cli.py` & `hledger_lots-0.3.0/hledger_lots/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import os
-from pathlib import Path
 from typing import Literal, Optional, Tuple
 
 import rich_click as click
 
 from .avg_info import AllAvgInfo, AvgInfo
 from .fifo_info import AllFifoInfo, FifoInfo
 from .files import get_file, get_files_comm
 from .info import AllInfo
 from .lib import default_fn_bool
-from .prices_yahoo import get_hledger_prices
+from .prices_yahoo import YahooPrices
 from .prompt import get_append_file
 from .prompt_buy import PromptBuy
 from .prompt_sell import PromptSell
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 click.rich_click.USE_MARKDOWN = True
@@ -231,45 +230,32 @@
     help="Description to be filtered out from calculation. Needed when closing journal with '--show-costs' option. Works like: not:desc:<value>. Will not be prompted if absent. If closed with default description, the value of this option should be: 'opening|closing balances'. Can be set with env HLEDGER_LOTS_NO_DESC",
 )
 @click.option(
     "--check/--no-check",
     default=default_fn_bool("HLEDGER_LOTS_CHECK", False),
     help="Enable/Disable check on the commodities previous transactions to ensure it is following the choosen method. Can be set with env HLEDGER_LOTS_CHECK=true|false. Default to false. Inthe future it will default to true",
 )
-@click.option(
-    "-p",
-    "--append-prices-to",
-    type=click.Path(),
-    default=lambda: os.environ.get("HLEDGER_APPEND_PRICES_TO", None),
-    prompt=False,
-    required=False,
-    help="Download market price and append to this option file value. Check the doc for info on how to set it up. Can be set with env HLEDGER_APPEND_PRICES_TO",
-)
 @click.pass_context
 def view(
     ctx: click.Context,
     avg_cost: bool,
     commodity: str,
     no_desc: str,
     check: bool,
-    append_prices_to: Path,
     file: Tuple[str, ...],
 ):
     """
     Report lots for a commodity.\r
 
     Show a report with lots for a commodity considering eventual past sale using FIFO or AVERAGE COST accounting principles.
 
     Also show some indicators about the lots and performance if there is prices in the journal after the last purchase. See the docs for details
     """
     journals = get_file(ctx, file)
 
-    if append_prices_to:
-        get_hledger_prices(journals, append_prices_to)
-
     if avg_cost:
         info = AvgInfo(journals, commodity, check, no_desc)
     else:
         info = FifoInfo(journals, commodity, check, no_desc)
 
     click.echo(info.table)
     click.echo(info.info_txt)
@@ -306,45 +292,32 @@
     help="Description to be filtered out from calculation. Needed when closing journal with '--show-costs' option. Works like: not:desc:<value>. Will not be prompted if absent. If closed with default description, the value of this option should be: 'opening|closing balances'. Can be set with env HLEDGER_LOTS_NO_DESC",
 )
 @click.option(
     "--check/--no-check",
     default=default_fn_bool("HLEDGER_LOTS_CHECK", False),
     help="Enable/Disable check on the commodities previous transactions to ensure it is following the choosen method. Can be set with env HLEDGER_LOTS_CHECK=tru|false. Default to false. Inthe future it will default to true",
 )
-@click.option(
-    "-p",
-    "--append-prices-to",
-    type=click.Path(),
-    default=lambda: os.environ.get("HLEDGER_APPEND_PRICES_TO", None),
-    prompt=False,
-    required=False,
-    help="Download market price and append to this option file value. Check the doc for info on how to set it up. Can be set with env HLEDGER_LOTS_APPEND_PRICES_TO",
-)
 @click.pass_context
 def list_commodities(
     ctx: click.Context,
     avg_cost: bool,
     output_format: str,
     no_desc: Literal["plain", "pretty", "csv"],
     check: bool,
-    append_prices_to: Path,
     file: Tuple[str, ...],
 ):
     """
     List indicators for all your commodities in a tabular format sorted from higher to lower **XIRR**. It is advised to use full-screen of the terminal. See the docs for a list of indicators and output examples.
 
     It can output in three formats: *plain, pretty and csv*.
     """
 
     journals = get_file(ctx, file)
     lots_info = AllInfo(journals, no_desc)
 
-    if append_prices_to:
-        get_hledger_prices(journals, append_prices_to)
-
     lots_info = (
         AllAvgInfo(journals, no_desc, check)
         if avg_cost
         else AllFifoInfo(journals, no_desc, check)
     )
 
     if output_format == "pretty":
@@ -354,11 +327,45 @@
         table = infos_io.read()
     else:
         table = lots_info.infos_table("plain")
 
     click.echo(table)
 
 
+@click.command()
+@click.option(
+    "-f",
+    "--file",
+    required=False,
+    multiple=True,
+    help="Inform the journal file path. If \"-\", read from stdin. Without this flag read from $LEDGER_FILE or ~/.hledger.journal in this order  or '-f-'.",
+)
+@click.pass_context
+def prices(
+    ctx: click.Context,  # pyright:ignore
+    file: Tuple[str, ...],
+):
+    """
+    Download market prices from Yahoo Finance and print as **price directives**. Use *BASH* redirection to append to the journal or copy/paste the data.
+
+    ### Setup
+    Add a \"yahoo_ticker\" tag to the *commodity directive* with the value of the ticker in Yahoo Finance to download prices
+
+    ### Example
+
+    ```text
+    commodity AAPL       ; yahoo_ticker:AAPL
+    commodity \"PETR4\"    ; yahoo_ticker:PETR4.SA
+    commodity BTC        ; yahoo_ticker:BTC-USD
+    ```
+
+
+    """
+    yahoo_prices = YahooPrices(file)
+    yahoo_prices.print_prices()
+
+
 cli.add_command(buy)
 cli.add_command(sell)
 cli.add_command(view)
 cli.add_command(list_commodities)
+cli.add_command(prices)
```

### Comparing `hledger_lots-0.2.0/hledger_lots/fifo.py` & `hledger_lots-0.3.0/hledger_lots/fifo.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/hledger_lots/fifo_info.py` & `hledger_lots-0.3.0/hledger_lots/fifo_info.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/hledger_lots/files.py` & `hledger_lots-0.3.0/hledger_lots/files.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/hledger_lots/hl.py` & `hledger_lots-0.3.0/hledger_lots/hl.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/hledger_lots/info.py` & `hledger_lots-0.3.0/hledger_lots/info.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,17 +47,15 @@
 
     if prices_str == "":
         return (None, None)
 
     prices_list = [row.split(" ", 3) for row in prices_str.split("\n") if row != ""]
 
     date_list = [
-        (row[1], re.sub(r"[^0-9.]", "", row[3]))
-        for row in prices_list
-        if row[2] == adjust_commodity(commodity)
+        (row[1], re.sub(r"[^0-9.]", "", row[3])) for row in prices_list if len(row) > 0
     ]
 
     if len(date_list) == 0:
         return (None, None)
 
     last_date_str = date_list[-1][0]
     last_date = datetime.strptime(last_date_str, "%Y-%m-%d").date()
```

### Comparing `hledger_lots-0.2.0/hledger_lots/lib.py` & `hledger_lots-0.3.0/hledger_lots/lib.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/hledger_lots/prices_yahoo.py` & `hledger_lots-0.3.0/hledger_lots/prices_yahoo.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,122 +1,132 @@
-import re
 import sys
 from dataclasses import dataclass
 from datetime import date, datetime, timedelta
 from pathlib import Path
-from typing import List, Optional, Tuple
+from typing import Dict, List, Tuple
 
 import yfinance as yf
 from requests.exceptions import HTTPError
 from requests_cache import CachedSession
 
+from .commodity_tag import CommodityDirective, CommodityTag
 from .files import get_files_comm
 from .hl import hledger2txn
-from .info import get_commodities, get_last_price
+from .info import get_last_price
 
 
 @dataclass
 class Price:
     name: str
     date: date
     price: float
     cur: str
 
 
-def get_start_date(txn_first_date: date, last_market_date: Optional[date]):
-    if not last_market_date:
-        last_date = txn_first_date
-    elif last_market_date < txn_first_date:
-        last_date = txn_first_date
-    else:
-        last_date = last_market_date
-
-    start_date = last_date + timedelta(days=1)
-    start_date_str = start_date.strftime("%Y-%m-%d")
-    return start_date_str
-
-
-def filter_yahoo(com: List[str]):
-    y_match = (re.search(r"^(y\.)(.*)", item) for item in com)
-    y_match = (item for item in y_match if item)
-    y_match = [match.groups()[1] for match in y_match]
-    return y_match
-
-
-def prices2hledger(prices: List[Price]):
-    prices_list = [
-        f"P {price.date.strftime('%Y-%m-%d')} \"y.{price.name}\" {price.price} {price.cur}"
-        for price in prices
-        if price
-    ]
-    prices_str = "\n".join(prices_list)
-    return prices_str
-
-
-def get_yahoo_prices(
-    ticker_name: str,
-    start_date: str,
-    end_date: str,
-    session: CachedSession,
-):
-    ticker = yf.Ticker(ticker_name, session=session)
-    info = ticker.info
-
-    if start_date:
-        df = ticker.history(start=start_date, end=end_date, raise_errors=True)
-    else:
-        df = ticker.history(period="1d", raise_errors=True)
-
-    prices = [
-        Price(
-            ticker_name,
-            row[0].to_pydatetime().date(),  # type:ignore
-            row[1]["Close"],  # type: ignore
-            info["currency"],
-        )
-        for row in df.iterrows()
-    ]
-    return prices
-
-
-def get_hledger_prices(files: Tuple[str, ...], append_prices_to: Path):
-    files_comm = get_files_comm(files)
-    commodities = get_commodities(files)
-    tickers = filter_yahoo(commodities)
-    tickers_str = " ".join(tickers)
-    print(
-        f"stderr: Downloading price history for tickers: {tickers_str}", file=sys.stderr
-    )
-
-    session_path = Path.home() / "yfinance.cache"
-    session = CachedSession(str(session_path))
-    today = datetime.today()
-    yesterday = today - timedelta(days=1)
-    yesterday_str = yesterday.strftime("%Y-%m-%d")
-    with open(append_prices_to, "a") as f:
-        f.write("\n")
-        for ticker in tickers:
-            commodity = f"y.{ticker}"
-            txns = hledger2txn(files, commodity)
-            txn_first_date_str = txns[0].date
-            txn_first_date = datetime.strptime(txn_first_date_str, "%Y-%m-%d").date()
-
-            last_market_date = get_last_price(files_comm, commodity)[0]
-            start_date = get_start_date(txn_first_date, last_market_date)
-            days_past = today.date() - datetime.strptime(start_date, "%Y-%m-%d").date()
-
-            if days_past.days > 0:
-                try:
-                    prices = get_yahoo_prices(
-                        ticker, start_date, yesterday_str, session
-                    )
-                    prices_hledger = prices2hledger(prices)
-                    f.write(prices_hledger + "\n")
-                except HTTPError:
-                    print(f"stderr: {ticker} not found", file=sys.stderr)
-                except Exception:
-                    print(
-                        f"stderr: Nothing downloaded for {ticker} between {start_date} and {yesterday_str}",
-                        file=sys.stderr,
-                    )
+class YahooPrices:
+    TAG = "yahoo_ticker"
 
-        f.write("\n")
+    def __init__(self, files: Tuple[str, ...]) -> None:
+        self.files = files
+        self.files_comm = get_files_comm(files)
+
+        self.session_path = Path.home() / "yfinance.cache"
+        self.session = CachedSession(str(self.session_path))
+        self.today = datetime.today()
+        yesterday = self.today - timedelta(days=1)
+        self.yesterday_str = yesterday.strftime("%Y-%m-%d")
+
+        commodity_directive = CommodityDirective(self.files)
+        self.commodities = commodity_directive.get_commodity_tag(self.TAG)
+
+    def get_start_date(self, commodity: CommodityTag):
+        txns = hledger2txn(self.files, commodity["commodity"])
+        first_date_str = txns[0].date
+        first_date = datetime.strptime(first_date_str, "%Y-%m-%d").date()
+        last_market_date = get_last_price(self.files_comm, commodity["commodity"])[0]
+
+        if not last_market_date:
+            last_date = first_date
+        elif last_market_date < first_date:
+            last_date = first_date
+        else:
+            last_date = last_market_date
+
+        start_date = last_date + timedelta(days=1)
+        past = date.today() - start_date
+        if past.days < 1:
+            return
+
+        return start_date
+
+    def prices2hledger(self, prices: List[Price]):
+        prices_list = [
+            f"P {price.date.strftime('%Y-%m-%d')} \"{price.name}\" {price.price} {price.cur}"
+            for price in prices
+            if price
+        ]
+        prices_str = "\n".join(prices_list)
+        return prices_str
+
+    def get_prices(
+        self,
+        commodity: CommodityTag,
+        start_date: str,
+    ) -> List[Price]:
+        ticker = yf.Ticker(commodity["value"], session=self.session)
+
+        try:
+            info: Dict[str, str] = ticker.info
+        except HTTPError:
+            print(f"; stderr: Can't download commodity {commodity}", file=sys.stderr)
+            return []
+
+        if not start_date:
+            return []
+
+        df = ticker.history(start=start_date, end=self.yesterday_str, raise_errors=True)
+
+        prices = [
+            Price(
+                commodity["commodity"],
+                row[0].to_pydatetime().date(),  # type:ignore
+                row[1]["Close"],  # type: ignore
+                info["currency"],
+            )
+            for row in df.iterrows()
+        ]
+        return prices
+
+    def get_commodity_prices(self, commodity: CommodityTag):
+        start_date = self.get_start_date(commodity)
+        if not start_date:
+            print(f"; stderr: No new data for {commodity}", file=sys.stderr)
+            return
+
+        start_date_str = start_date.strftime("%Y-%m-%d")
+        try:
+            prices = [
+                price for price in self.get_prices(commodity, start_date_str) if price
+            ]
+            return prices
+        except HTTPError:
+            print(f"; stderr: {commodity['value']} not found", file=sys.stderr)
+        except Exception:
+            print(
+                f"; stderr: Nothing downloaded for {commodity['value']} between {start_date} and {self.yesterday_str}",
+                file=sys.stderr,
+            )
+
+    def print_prices(self):
+        if len(self.commodities) == 0:
+            print(
+                f"\n\n; stderr: No commodities directives with tag {self.TAG}",
+                file=sys.stderr,
+            )
+            return
+
+        for commodity in self.commodities:
+            prices = self.get_commodity_prices(commodity)
+            if prices:
+                print("\n")
+                hledger_prices = self.prices2hledger(prices)
+                print(hledger_prices)
```

### Comparing `hledger_lots-0.2.0/hledger_lots/prompt.py` & `hledger_lots-0.3.0/hledger_lots/prompt.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/hledger_lots/prompt_buy.py` & `hledger_lots-0.3.0/hledger_lots/prompt_buy.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/hledger_lots/prompt_sell.py` & `hledger_lots-0.3.0/hledger_lots/prompt_sell.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/hledger_lots.egg-info/PKG-INFO` & `hledger_lots-0.3.0/hledger_lots.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hledger-lots
-Version: 0.2.0
+Version: 0.3.0
 License: MIT License
 Project-URL: homepage, https://github.com/edkedk99/hledger-lots
 Project-URL: documentation, https://edkedk99.github.io/hledger-lots/
 Project-URL: repository, https://github.com/edkedk99/hledger-lots
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -32,17 +32,17 @@
 
 You can choose between two diferrent methods to calculate the cost of selling lots:
 
 - **FIFO**: First In First Out
 - **AVERAGE COST**: Average Cost of all previous purchase. It is as if selling a proportional part of each previous sale.
 
 
-### Update Price
+### Automatic Price Download
 
-After having the correct cost and result for selling a commodity, we want to follow the investment performance using market data. This package can download market price history from [Yahoo Finance](https://finance.yahoo.com/) and append [price directive](https://hledger.org/1.29/hledger.html#p-directive) to the journal just by following the required format when naming the commodity. More information [here](market_prices/)
+One simple command to automatically download market price from [Yahoo Finance](https://finance.yahoo.com/) for choosen commodities as explained [here](market_prices/). 
 
 ### Reports
 
 To get information about the commodities, there is more 2 commands:
 
 | command                          | description                                          |
 |----------------------------------|------------------------------------------------------|
@@ -67,17 +67,18 @@
 
 ```python
 pip install --upgrade hledger-lots
 ```
 
 ## Workflow
 
-1. Add purchase using the command [buy](usage/#buy) or edit the journal as usual using "@" notation. **Don't bother creating subaccounts or tags with unique lot name**. See the some examples [here](examples/data.journal)
-2. When you sell, use the command [sell](usage/#sell) instead of adding the transactions manually. Hledger-lots will generate the correct transaction and append to the selected journal if you confirm the transaction is correct. *See transaction tags with interesting indicators about the current trade*
-3. View financial indicators for a specific commodity using [view](usage/#view) or a summary of all commodities using [list](usage/$list). Optionally update market prices from [Yahoo Finance](https://finance.yahoo.com/) using the flag *--apend-prices-to [file path]*
+1. Add purchase using the command [buy](usage/#hledger-lots-buy) or edit the journal as usual using "@" notation. **Don't bother creating subaccounts or tags with unique lot name**. See the some examples [here](examples/data.journal)
+2. Download market price history as [price directive](https://hledger.org/1.29/hledger.html#p-directive) using the command [prices](usage/#hledger-lots-prices)
+3. View financial indicators for a specific commodity using [view](usage/#hledger-lots-view) or a summary of all commodities using [list](usage/$list). Optionally update market prices from [Yahoo Finance](https://finance.yahoo.com/) using the flag *--apend-prices-to [file path]*
+4. When you sell, use the command [sell](usage/#hledger-lots-sell) instead of adding the transactions manually. Hledger-lots will generate the correct transaction and append to the selected journal if you confirm the transaction is correct. *See transaction tags with interesting indicators about the current trade*
 
 > By default the sale is created using *FIFO* method. Use the option flag "--avg-cost" to change it to *Average Cost*
 
 
 ## Indicators
   
 ### Basic Indicators
```

### Comparing `hledger_lots-0.2.0/hledger_lots.egg-info/SOURCES.txt` & `hledger_lots-0.3.0/hledger_lots.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 docs/README.md
 hledger_lots/__init__.py
 hledger_lots/__main__.py
 hledger_lots/avg.py
 hledger_lots/avg_info.py
 hledger_lots/checks.py
 hledger_lots/cli.py
+hledger_lots/commodity_tag.py
 hledger_lots/fifo.py
 hledger_lots/fifo_info.py
 hledger_lots/files.py
 hledger_lots/hl.py
 hledger_lots/info.py
 hledger_lots/lib.py
 hledger_lots/prices_yahoo.py
```

### Comparing `hledger_lots-0.2.0/pyproject.toml` & `hledger_lots-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 keyword = ["hledger","PTA", "investments", "accounting", "lots"]
 classifiers = [""]
 author = "Eduardo"
 author_email = "edkedk99@hotmail.com"
 
 [project]
 name = "hledger_lots"
-version = "0.2.0"
+version = "0.3.0"
 readme= "docs/README.md"
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 dependencies = [
 	     "click",
 	     "rich_click",
 	     "tabulate",
```

### Comparing `hledger_lots-0.2.0/tests/lots_data.py` & `hledger_lots-0.3.0/tests/lots_data.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/tests/test_avg.py` & `hledger_lots-0.3.0/tests/test_avg.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/tests/test_checks.py` & `hledger_lots-0.3.0/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/tests/test_fifo.py` & `hledger_lots-0.3.0/tests/test_fifo.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/tests/test_hl.py` & `hledger_lots-0.3.0/tests/test_hl.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/tests/test_info.py` & `hledger_lots-0.3.0/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/tests/test_lib.py` & `hledger_lots-0.3.0/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/venv/bin/rst2html.py` & `hledger_lots-0.3.0/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/venv/bin/rst2html4.py` & `hledger_lots-0.3.0/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/venv/bin/rst2html5.py` & `hledger_lots-0.3.0/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/venv/bin/rst2latex.py` & `hledger_lots-0.3.0/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/venv/bin/rst2man.py` & `hledger_lots-0.3.0/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/venv/bin/rst2odt.py` & `hledger_lots-0.3.0/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/venv/bin/rst2odt_prepstyles.py` & `hledger_lots-0.3.0/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/venv/bin/rst2pseudoxml.py` & `hledger_lots-0.3.0/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/venv/bin/rst2s5.py` & `hledger_lots-0.3.0/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/venv/bin/rst2xetex.py` & `hledger_lots-0.3.0/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/venv/bin/rst2xml.py` & `hledger_lots-0.3.0/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.2.0/venv/bin/rstpep2html.py` & `hledger_lots-0.3.0/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

