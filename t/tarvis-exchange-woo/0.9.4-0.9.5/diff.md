# Comparing `tmp/tarvis-exchange-woo-0.9.4.tar.gz` & `tmp/tarvis-exchange-woo-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarvis-exchange-woo-0.9.4.tar", last modified: Fri Apr 28 10:08:03 2023, max compression
+gzip compressed data, was "tarvis-exchange-woo-0.9.5.tar", last modified: Wed May  3 02:15:21 2023, max compression
```

## Comparing `tarvis-exchange-woo-0.9.4.tar` & `tarvis-exchange-woo-0.9.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:08:03.489413 tarvis-exchange-woo-0.9.4/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-04-28 10:07:54.000000 tarvis-exchange-woo-0.9.4/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      404 2023-04-28 10:08:03.489413 tarvis-exchange-woo-0.9.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-28 10:07:54.000000 tarvis-exchange-woo-0.9.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 10:08:03.489413 tarvis-exchange-woo-0.9.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      767 2023-04-28 10:07:54.000000 tarvis-exchange-woo-0.9.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:08:03.485413 tarvis-exchange-woo-0.9.4/tarvis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:08:03.485413 tarvis-exchange-woo-0.9.4/tarvis/exchange/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:08:03.489413 tarvis-exchange-woo-0.9.4/tarvis/exchange/woo/
--rw-r--r--   0 root         (0) root         (0)    10910 2023-04-28 10:07:54.000000 tarvis-exchange-woo-0.9.4/tarvis/exchange/woo/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11285 2023-04-28 10:07:54.000000 tarvis-exchange-woo-0.9.4/tarvis/exchange/woo/wooclient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:08:03.489413 tarvis-exchange-woo-0.9.4/tarvis_exchange_woo.egg-info/
--rw-r--r--   0 root         (0) root         (0)      404 2023-04-28 10:08:03.000000 tarvis-exchange-woo-0.9.4/tarvis_exchange_woo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-28 10:08:03.000000 tarvis-exchange-woo-0.9.4/tarvis_exchange_woo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 10:08:03.000000 tarvis-exchange-woo-0.9.4/tarvis_exchange_woo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-28 10:08:03.000000 tarvis-exchange-woo-0.9.4/tarvis_exchange_woo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-28 10:08:03.000000 tarvis-exchange-woo-0.9.4/tarvis_exchange_woo.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:08:03.489413 tarvis-exchange-woo-0.9.4/test/
--rw-r--r--   0 root         (0) root         (0)    11990 2023-04-28 10:07:54.000000 tarvis-exchange-woo-0.9.4/test/test_exchange_woo_margin.py
--rw-r--r--   0 root         (0) root         (0)    11996 2023-04-28 10:07:54.000000 tarvis-exchange-woo-0.9.4/test/test_exchange_woo_perpetual.py
--rw-r--r--   0 root         (0) root         (0)     6566 2023-04-28 10:07:54.000000 tarvis-exchange-woo-0.9.4/test/test_exchange_woo_spot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:15:21.742359 tarvis-exchange-woo-0.9.5/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-05-03 02:15:10.000000 tarvis-exchange-woo-0.9.5/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      404 2023-05-03 02:15:21.738359 tarvis-exchange-woo-0.9.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       34 2023-05-03 02:15:10.000000 tarvis-exchange-woo-0.9.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 02:15:21.742359 tarvis-exchange-woo-0.9.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      767 2023-05-03 02:15:10.000000 tarvis-exchange-woo-0.9.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:15:21.738359 tarvis-exchange-woo-0.9.5/tarvis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:15:21.738359 tarvis-exchange-woo-0.9.5/tarvis/exchange/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:15:21.738359 tarvis-exchange-woo-0.9.5/tarvis/exchange/woo/
+-rw-r--r--   0 root         (0) root         (0)    10775 2023-05-03 02:15:10.000000 tarvis-exchange-woo-0.9.5/tarvis/exchange/woo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11285 2023-05-03 02:15:10.000000 tarvis-exchange-woo-0.9.5/tarvis/exchange/woo/wooclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:15:21.738359 tarvis-exchange-woo-0.9.5/tarvis_exchange_woo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      404 2023-05-03 02:15:21.000000 tarvis-exchange-woo-0.9.5/tarvis_exchange_woo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-03 02:15:21.000000 tarvis-exchange-woo-0.9.5/tarvis_exchange_woo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 02:15:21.000000 tarvis-exchange-woo-0.9.5/tarvis_exchange_woo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-03 02:15:21.000000 tarvis-exchange-woo-0.9.5/tarvis_exchange_woo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 02:15:21.000000 tarvis-exchange-woo-0.9.5/tarvis_exchange_woo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:15:21.738359 tarvis-exchange-woo-0.9.5/test/
+-rw-r--r--   0 root         (0) root         (0)    11990 2023-05-03 02:15:10.000000 tarvis-exchange-woo-0.9.5/test/test_exchange_woo_margin.py
+-rw-r--r--   0 root         (0) root         (0)    11996 2023-05-03 02:15:10.000000 tarvis-exchange-woo-0.9.5/test/test_exchange_woo_perpetual.py
+-rw-r--r--   0 root         (0) root         (0)     6566 2023-05-03 02:15:10.000000 tarvis-exchange-woo-0.9.5/test/test_exchange_woo_spot.py
```

### Comparing `tarvis-exchange-woo-0.9.4/LICENSE.txt` & `tarvis-exchange-woo-0.9.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tarvis-exchange-woo-0.9.4/setup.py` & `tarvis-exchange-woo-0.9.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = requirements_file.read().splitlines()
 
 with open("README.md") as description_file:
     long_description = description_file.read()
 
 setup(
     name="tarvis-exchange-woo",
-    version="0.9.4",
+    version="0.9.5",
     author="Tarvis Labs",
     author_email="python@tarvislabs.com",
     url="https://tarvislabs.com/",
     description="Tarvis Exchange Library for Woo",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `tarvis-exchange-woo-0.9.4/tarvis/exchange/woo/__init__.py` & `tarvis-exchange-woo-0.9.5/tarvis/exchange/woo/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -144,29 +144,31 @@
             page += 1
 
             for woo_order in woo_orders:
                 symbol = woo_order["symbol"]
                 market_type, quote_asset, base_asset = self._convert_market_to_assets(
                     symbol
                 )
-                order_type = woo_order["type"]
 
-                if (market_type == self._market_type) and (
-                    order_type in self._STANDARD_WOO_ORDER_TYPES
-                ):
+                if market_type == self._market_type:
                     order_id = woo_order["order_id"]
+                    order_type = woo_order["type"]
                     quantity = woo_order.get("quantity")
                     amount = woo_order.get("amount")
                     price = woo_order.get("price")
                     side = woo_order["side"]
                     creation_time = woo_order["created_time"]
                     filled_quantity = woo_order.get("executed", 0)
 
                     side = OrderSide[side]
-                    order_type = self._STANDARD_ORDER_TYPE_TO_TARVIS[order_type]
+                    # noinspection PyBroadException
+                    try:
+                        order_type = self._STANDARD_ORDER_TYPE_TO_TARVIS[order_type]
+                    except:
+                        order_type = OrderType.UNSUPPORTED
                     meta_data = {"order_id": order_id, "order_method": "standard"}
 
                     order = Order(
                         quote_asset,
                         base_asset,
                         side,
                         order_type,
@@ -197,30 +199,30 @@
             page += 1
 
             for woo_order in woo_orders:
                 symbol = woo_order["symbol"]
                 market_type, quote_asset, base_asset = self._convert_market_to_assets(
                     symbol
                 )
-                order_type = woo_order["type"]
-                if order_type == "MARKET":
-                    order_type = OrderType.STOP_LOSS_MARKET
-                else:
-                    order_type = None
 
-                if (market_type == self._market_type) and (order_type is not None):
+                if market_type == self._market_type:
                     order_id = woo_order["algoOrderId"]
                     quantity = woo_order.get("quantity", None)
                     amount = woo_order.get("amount", None)
                     price = woo_order["triggerPrice"]
                     side = woo_order["side"]
+                    order_type = woo_order["type"]
                     creation_time = woo_order["createdTime"]
                     filled_quantity = woo_order.get("totalExecutedQuantity")
 
                     side = OrderSide[side]
+                    if order_type == "MARKET":
+                        order_type = OrderType.STOP_LOSS_MARKET
+                    else:
+                        order_type = OrderType.UNSUPPORTED
                     meta_data = {"order_id": order_id, "order_method": "algo"}
 
                     order = Order(
                         quote_asset,
                         base_asset,
                         side,
                         order_type,
@@ -262,37 +264,30 @@
             algo_type, woo_order_type = self._ALGO_ORDER_TYPE_TO_WOO[order_type]
 
         if order_type == OrderType.STOP_LOSS_MARKET:
             price = str(stop_loss_price)
         elif price is not None:
             price = str(price)
 
-        if increasing_position is not None:
-            reduce_only = not increasing_position
-        else:
-            reduce_only = None
-
         if standard_order:
             self._client.post_order(
                 market,
                 side.name,
                 woo_order_type,
                 order_quantity=str(quantity),
                 order_price=price,
-                reduce_only=reduce_only,
             )
         else:
             self._client.post_algo_order(
                 market,
                 side.name,
                 algo_type,
                 woo_order_type,
                 order_quantity=str(quantity),
                 trigger_price=price,
-                reduce_only=reduce_only,
             )
 
     def cancel_order(self, order: Order):
         market = self._convert_assets_to_market(order.base_asset, order.quote_asset)
         if order.meta_data["order_method"] == "standard":
             self._client.delete_order(order.meta_data["order_id"], market)
         else:
```

### Comparing `tarvis-exchange-woo-0.9.4/tarvis/exchange/woo/wooclient.py` & `tarvis-exchange-woo-0.9.5/tarvis/exchange/woo/wooclient.py`

 * *Files identical despite different names*

### Comparing `tarvis-exchange-woo-0.9.4/test/test_exchange_woo_margin.py` & `tarvis-exchange-woo-0.9.5/test/test_exchange_woo_margin.py`

 * *Files identical despite different names*

### Comparing `tarvis-exchange-woo-0.9.4/test/test_exchange_woo_perpetual.py` & `tarvis-exchange-woo-0.9.5/test/test_exchange_woo_perpetual.py`

 * *Files identical despite different names*

### Comparing `tarvis-exchange-woo-0.9.4/test/test_exchange_woo_spot.py` & `tarvis-exchange-woo-0.9.5/test/test_exchange_woo_spot.py`

 * *Files identical despite different names*

