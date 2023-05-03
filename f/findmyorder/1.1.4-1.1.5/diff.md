# Comparing `tmp/findmyorder-1.1.4.tar.gz` & `tmp/findmyorder-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.1.4.tar", max compression
+gzip compressed data, was "findmyorder-1.1.5.tar", max compression
```

## Comparing `findmyorder-1.1.4.tar` & `findmyorder-1.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-03 15:09:53.553183 findmyorder-1.1.4/LICENSE
--rw-r--r--   0        0        0     2180 2023-05-03 15:09:53.553183 findmyorder-1.1.4/README.md
--rw-r--r--   0        0        0      113 2023-05-03 15:09:54.493189 findmyorder-1.1.4/findmyorder/__init__.py
--rw-r--r--   0        0        0      392 2023-05-03 15:09:53.557183 findmyorder-1.1.4/findmyorder/config.py
--rw-r--r--   0        0        0      383 2023-05-03 15:09:53.557183 findmyorder-1.1.4/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     3866 2023-05-03 15:09:53.557183 findmyorder-1.1.4/findmyorder/main.py
--rw-r--r--   0        0        0     1280 2023-05-03 15:09:54.493189 findmyorder-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     3000 1970-01-01 00:00:00.000000 findmyorder-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-03 18:16:53.660112 findmyorder-1.1.5/LICENSE
+-rw-r--r--   0        0        0     2180 2023-05-03 18:16:53.660112 findmyorder-1.1.5/README.md
+-rw-r--r--   0        0        0      113 2023-05-03 18:16:54.392123 findmyorder-1.1.5/findmyorder/__init__.py
+-rw-r--r--   0        0        0      392 2023-05-03 18:16:53.660112 findmyorder-1.1.5/findmyorder/config.py
+-rw-r--r--   0        0        0      383 2023-05-03 18:16:53.660112 findmyorder-1.1.5/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     3894 2023-05-03 18:16:53.660112 findmyorder-1.1.5/findmyorder/main.py
+-rw-r--r--   0        0        0     1280 2023-05-03 18:16:54.392123 findmyorder-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3000 1970-01-01 00:00:00.000000 findmyorder-1.1.5/PKG-INFO
```

### Comparing `findmyorder-1.1.4/LICENSE` & `findmyorder-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.1.4/README.md` & `findmyorder-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.1.4/findmyorder/main.py` & `findmyorder-1.1.5/findmyorder/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,16 +66,16 @@
             Suppress(settings.comment_identifier) + Word(alphas)
                 ).set_results_name("comment")
 
             order_grammar = (
                 action("action")
                 + Optional(instrument,default=None)
                 + Optional(int(stop_loss),default=1000)
-                + Optional(int(take_profit),default=1000)
-                + Optional(int(quantity),default=1)
+                + Optional(take_profit,default=1000)
+                + Optional(quantity,default=1)
                 + Optional(order_type,default=None)
                 + Optional(leverage_type,default=None)
                 + Optional(comment,default=None)
               )
 
             order = order_grammar.parse_string(
                     instring=mystring,
@@ -97,14 +97,15 @@
         try:
             logging.debug("get_order %s", msg)
 
             if await self.search(msg):
                 logging.info("get_order found in %s", msg)
                 order = await self.identify_order(msg)
                 logging.info("order: %s", order)
+                #add check if no dict
                 order["timestamp"] = datetime.now(timezone.utc)
                 return order
             return None
 
         except Exception as e:
             logging.exception("GetOrderError: %s", e)
             return None
```

### Comparing `findmyorder-1.1.4/pyproject.toml` & `findmyorder-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.1.4"
+version = "1.1.5"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
```

### Comparing `findmyorder-1.1.4/PKG-INFO` & `findmyorder-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.1.4
+Version: 1.1.5
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

