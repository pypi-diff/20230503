# Comparing `tmp/findmyorder-1.1.1.tar.gz` & `tmp/findmyorder-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.1.1.tar", max compression
+gzip compressed data, was "findmyorder-1.1.2.tar", max compression
```

## Comparing `findmyorder-1.1.1.tar` & `findmyorder-1.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-02 08:18:12.266852 findmyorder-1.1.1/LICENSE
--rw-r--r--   0        0        0     1925 2023-05-02 08:18:12.266852 findmyorder-1.1.1/README.md
--rw-r--r--   0        0        0      113 2023-05-02 08:18:13.282859 findmyorder-1.1.1/findmyorder/__init__.py
--rw-r--r--   0        0        0      392 2023-05-02 08:18:12.266852 findmyorder-1.1.1/findmyorder/config.py
--rw-r--r--   0        0        0      312 2023-05-02 08:18:12.266852 findmyorder-1.1.1/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     3851 2023-05-02 08:18:12.266852 findmyorder-1.1.1/findmyorder/main.py
--rw-r--r--   0        0        0     1223 2023-05-02 08:18:13.282859 findmyorder-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     2745 1970-01-01 00:00:00.000000 findmyorder-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-03 14:19:24.563765 findmyorder-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2180 2023-05-03 14:19:24.563765 findmyorder-1.1.2/README.md
+-rw-r--r--   0        0        0      113 2023-05-03 14:19:25.327777 findmyorder-1.1.2/findmyorder/__init__.py
+-rw-r--r--   0        0        0      392 2023-05-03 14:19:24.563765 findmyorder-1.1.2/findmyorder/config.py
+-rw-r--r--   0        0        0      312 2023-05-03 14:19:24.563765 findmyorder-1.1.2/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     3866 2023-05-03 14:19:24.563765 findmyorder-1.1.2/findmyorder/main.py
+-rw-r--r--   0        0        0     1223 2023-05-03 14:19:25.327777 findmyorder-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3000 1970-01-01 00:00:00.000000 findmyorder-1.1.2/PKG-INFO
```

### Comparing `findmyorder-1.1.1/LICENSE` & `findmyorder-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.1.1/README.md` & `findmyorder-1.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 `pip install findmyorder`
 
 # How to use it
 ```
 fmo = FindMyOrder()
 msg_order = "buy EURUSD sl=1000 tp=1000 q=1 comment=FOMC"
 order = await fmo.get_order(msg_order)
-  
+#{'action': 'BUY', 'instrument': 'EURUSD', 'stop_loss': '1000', 'take_profit': '1000', 'quantity': '2', 'order_type': None, 'leverage_type': None, 'comment': None, 'timestamp': datetime.datetime(2023, 5, 3, 12, 10, 28, 731282, tzinfo=datetime.timezone.utc)}
 ```
 ## Example
 [example](https://github.com/mraniki/findmyorder/blob/main/examples/example.py)
 
 ## Real use case
 [TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
```

### Comparing `findmyorder-1.1.1/findmyorder/main.py` & `findmyorder-1.1.2/findmyorder/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,17 +65,17 @@
             comment = Combine(
             Suppress(settings.comment_identifier) + Word(alphas)
                 ).set_results_name("comment")
 
             order_grammar = (
                 action("action")
                 + Optional(instrument,default=None)
-                + Optional(stop_loss,default=1000)
-                + Optional(take_profit,default=1000)
-                + Optional(quantity,default=1)
+                + Optional(int(stop_loss),default=1000)
+                + Optional(int(take_profit),default=1000)
+                + Optional(int(quantity),default=1)
                 + Optional(order_type,default=None)
                 + Optional(leverage_type,default=None)
                 + Optional(comment,default=None)
               )
 
             order = order_grammar.parse_string(
                     instring=mystring,
```

### Comparing `findmyorder-1.1.1/pyproject.toml` & `findmyorder-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.1.1"
+version = "1.1.2"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
```

### Comparing `findmyorder-1.1.1/PKG-INFO` & `findmyorder-1.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.1.1
+Version: 1.1.2
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -40,15 +40,15 @@
 `pip install findmyorder`
 
 # How to use it
 ```
 fmo = FindMyOrder()
 msg_order = "buy EURUSD sl=1000 tp=1000 q=1 comment=FOMC"
 order = await fmo.get_order(msg_order)
-  
+#{'action': 'BUY', 'instrument': 'EURUSD', 'stop_loss': '1000', 'take_profit': '1000', 'quantity': '2', 'order_type': None, 'leverage_type': None, 'comment': None, 'timestamp': datetime.datetime(2023, 5, 3, 12, 10, 28, 731282, tzinfo=datetime.timezone.utc)}
 ```
 ## Example
 [example](https://github.com/mraniki/findmyorder/blob/main/examples/example.py)
 
 ## Real use case
 [TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
```

