# Comparing `tmp/bigc-0.2.5.tar.gz` & `tmp/bigc-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigc-0.2.5.tar", max compression
+gzip compressed data, was "bigc-0.2.6.tar", max compression
```

## Comparing `bigc-0.2.5.tar` & `bigc-0.2.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1069 2023-04-11 19:29:46.699022 bigc-0.2.5/LICENSE.txt
--rw-r--r--   0        0        0     1596 2023-04-11 19:29:46.699022 bigc-0.2.5/README.md
--rw-r--r--   0        0        0       32 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/__init__.py
--rw-r--r--   0        0        0     1069 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/api.py
--rw-r--r--   0        0        0     6458 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/api_client.py
--rw-r--r--   0        0        0       49 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/data/__init__.py
--rw-r--r--   0        0        0      482 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/data/order_status.py
--rw-r--r--   0        0        0     1639 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/exceptions.py
--rw-r--r--   0        0        0      431 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/resources/__init__.py
--rw-r--r--   0        0        0     1741 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/resources/carts.py
--rw-r--r--   0        0        0     1180 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/resources/categories.py
--rw-r--r--   0        0        0     4116 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/resources/checkouts.py
--rw-r--r--   0        0        0     1178 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/resources/customer_groups.py
--rw-r--r--   0        0        0     2922 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/resources/customers.py
--rw-r--r--   0        0        0     3832 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/resources/orders.py
--rw-r--r--   0        0        0     1414 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/resources/product_variants.py
--rw-r--r--   0        0        0     2682 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/resources/products.py
--rw-r--r--   0        0        0     1205 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/resources/webhooks.py
--rw-r--r--   0        0        0      557 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/utils.py
--rw-r--r--   0        0        0      770 2023-04-11 19:29:46.699022 bigc-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     2420 1970-01-01 00:00:00.000000 bigc-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-03 15:56:06.836948 bigc-0.2.6/LICENSE.txt
+-rw-r--r--   0        0        0     1596 2023-05-03 15:56:06.836948 bigc-0.2.6/README.md
+-rw-r--r--   0        0        0       32 2023-05-03 15:56:06.836948 bigc-0.2.6/bigc/__init__.py
+-rw-r--r--   0        0        0     1069 2023-05-03 15:56:06.836948 bigc-0.2.6/bigc/api.py
+-rw-r--r--   0        0        0     6458 2023-05-03 15:56:06.836948 bigc-0.2.6/bigc/api_client.py
+-rw-r--r--   0        0        0       49 2023-05-03 15:56:06.836948 bigc-0.2.6/bigc/data/__init__.py
+-rw-r--r--   0        0        0      482 2023-05-03 15:56:06.836948 bigc-0.2.6/bigc/data/order_status.py
+-rw-r--r--   0        0        0     1639 2023-05-03 15:56:06.836948 bigc-0.2.6/bigc/exceptions.py
+-rw-r--r--   0        0        0      431 2023-05-03 15:56:06.836948 bigc-0.2.6/bigc/resources/__init__.py
+-rw-r--r--   0        0        0     1741 2023-05-03 15:56:06.836948 bigc-0.2.6/bigc/resources/carts.py
+-rw-r--r--   0        0        0     1180 2023-05-03 15:56:06.836948 bigc-0.2.6/bigc/resources/categories.py
+-rw-r--r--   0        0        0     4116 2023-05-03 15:56:06.836948 bigc-0.2.6/bigc/resources/checkouts.py
+-rw-r--r--   0        0        0     1178 2023-05-03 15:56:06.836948 bigc-0.2.6/bigc/resources/customer_groups.py
+-rw-r--r--   0        0        0     4096 2023-05-03 15:56:06.836948 bigc-0.2.6/bigc/resources/customers.py
+-rw-r--r--   0        0        0     4504 2023-05-03 15:56:06.836948 bigc-0.2.6/bigc/resources/orders.py
+-rw-r--r--   0        0        0     1414 2023-05-03 15:56:06.836948 bigc-0.2.6/bigc/resources/product_variants.py
+-rw-r--r--   0        0        0     2682 2023-05-03 15:56:06.836948 bigc-0.2.6/bigc/resources/products.py
+-rw-r--r--   0        0        0     1205 2023-05-03 15:56:06.836948 bigc-0.2.6/bigc/resources/webhooks.py
+-rw-r--r--   0        0        0      557 2023-05-03 15:56:06.836948 bigc-0.2.6/bigc/utils.py
+-rw-r--r--   0        0        0      770 2023-05-03 15:56:06.836948 bigc-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     2420 1970-01-01 00:00:00.000000 bigc-0.2.6/PKG-INFO
```

### Comparing `bigc-0.2.5/LICENSE.txt` & `bigc-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bigc-0.2.5/README.md` & `bigc-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `bigc-0.2.5/bigc/api.py` & `bigc-0.2.6/bigc/api.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.5/bigc/api_client.py` & `bigc-0.2.6/bigc/api_client.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.5/bigc/exceptions.py` & `bigc-0.2.6/bigc/exceptions.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.5/bigc/resources/carts.py` & `bigc-0.2.6/bigc/resources/carts.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.5/bigc/resources/categories.py` & `bigc-0.2.6/bigc/resources/categories.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.5/bigc/resources/checkouts.py` & `bigc-0.2.6/bigc/resources/checkouts.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.5/bigc/resources/customer_groups.py` & `bigc-0.2.6/bigc/resources/customer_groups.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.5/bigc/resources/customers.py` & `bigc-0.2.6/bigc/resources/products.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,72 @@
 from collections.abc import Iterator
-from typing import Any, Iterable
 from urllib.parse import urlencode, urlparse, urlunparse
 
 from bigc.api_client import BigCommerceAPIClient
-from bigc.exceptions import ResourceNotFoundError
 
 
-class BigCommerceCustomersAPI:
+class BigCommerceProductsAPI:
     def __init__(self, api_client: BigCommerceAPIClient):
         self._api = api_client
 
-    def all(self, *, id_in: Iterable[int] = None, include_formfields: bool = False,
-            include_storecredit: bool = False) -> Iterator[dict]:
-        """Return an iterator for all customers"""
-        url_parts = urlparse('/customers')
-
-        query_dict = {}
-
-        if id_in is not None:
-            query_dict['id:in'] = ','.join(map(str, id_in))
+    def all(self, *, include_variants: bool = False, include_custom_fields: bool = False) -> Iterator[dict]:
+        """Return an iterator for all products"""
+        url_parts = urlparse('/catalog/products')
 
         include = []
-        if include_storecredit:
-            include.append('storecredit')
-        if include_formfields:
-            include.append('formfields')
+        if include_variants:
+            include.append('variants')
+        if include_custom_fields:
+            include.append('custom_fields')
+
+        query_dict = {}
         if include:
             query_dict['include'] = ','.join(include)
-
         url_parts = url_parts._replace(query=urlencode(query_dict))
 
         return self._api.v3.get_many(urlunparse(url_parts))
 
-    def get(self, customer_id: int, *, include_formfields: bool = False,
-            include_storecredit: bool = False) -> dict:
-        """Get a specific customer by its ID"""
-        url_parts = urlparse('/customers')
-
-        query_dict = {'id:in': customer_id}
+    def get(self, product_id: int, *, include_variants: bool = False, include_custom_fields: bool = False) -> dict:
+        """Get a specific product by its ID"""
+        url_parts = urlparse(f'/catalog/products/{product_id}')
 
         include = []
-        if include_storecredit:
-            include.append('storecredit')
-        if include_formfields:
-            include.append('formfields')
+        if include_variants:
+            include.append('variants')
+        if include_custom_fields:
+            include.append('custom_fields')
+
+        query_dict = {}
         if include:
             query_dict['include'] = ','.join(include)
-
         url_parts = url_parts._replace(query=urlencode(query_dict))
 
-        try:
-            return self._api.v3.get(urlunparse(url_parts))[0]
-        except IndexError:
-            raise ResourceNotFoundError()
+        return self._api.v3.get(urlunparse(url_parts))
 
-    def create(self, first_name: str, last_name: str, email: str, **kwargs) -> dict:
-        """Create a single customer"""
+    def create(self, *, name: str, product_type: str, weight: float, price: float, **kwargs) -> dict:
+        """Create a product"""
         payload = {
-            'first_name': first_name,
-            'last_name': last_name,
-            'email': email,
+            'name': name,
+            'type': product_type,
+            'weight': weight,
+            'price': price,
             **kwargs,
         }
-        return self._api.v3.post('/customers', json=[payload])[0]
-
-    def update(self, customer_id: int, data: dict) -> dict:
-        """Update a single customer"""
-        payload = {
-            'id': customer_id,
-            **data,
-        }
-        return self._api.v3.put('/customers', json=[payload])[0]
+        return self._api.v3.post('/catalog/products', json=payload)
 
-    def update_form_field(self, customer_id: int, field_name: str, value: Any) -> dict:
-        """Update a form field value for a single customer"""
-        payload = [{
-            'customer_id': customer_id,
-            'name': field_name,
-            'value': value,
-        }]
-        return self._api.v3.put('/customers/form-field-values', json=payload)[0]
-
-    def delete(self, customer_id: int) -> None:
-        """Delete a specific customer by its ID"""
-        self._api.v3.delete(f'/customers?id:in={customer_id}')
+    def update(self, product_id: int, data: dict) -> dict:
+        """Update a specific product by its ID"""
+        return self._api.v3.put(f'/catalog/products/{product_id}', json=data)
+
+    def delete(self, product_id: int) -> dict:
+        """Delete a specific product by its ID"""
+        return self._api.v3.delete(f'/catalog/products/{product_id}')
+
+    def get_pricing(self, items: list[dict], *, channel_id: int = 1, currency_code: str = 'USD',
+                    customer_group_id: int = 0) -> Iterator[dict]:
+        """Return an iterator for batch product pricing"""
+        return self._api.v3.post('/pricing/products', json={
+            'channel_id': channel_id,
+            'currency_code': currency_code,
+            'customer_group_id': customer_group_id,
+            'items': list(items),
+        })
```

### Comparing `bigc-0.2.5/bigc/resources/orders.py` & `bigc-0.2.6/bigc/resources/orders.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,14 +46,31 @@
         """Return an iterator for all order products in an order"""
         return self._api.v2.get_many(f'/orders/{order_id}/products')
 
     def get_product(self, order_id: int, product_id: int) -> dict:
         """Get a specific order product in an order by ID"""
         return self._api.v2.get(f'/orders/{order_id}/products/{product_id}')
 
+    def get_refund_quote(self, order_id: int, *, items: list, **kwargs) -> dict:
+        """Get a refund quote for an order by ID"""
+        payload = {
+            "items": items,
+            **kwargs,
+        }
+        return self._api.v3.post(f'/orders/{order_id}/payment_actions/refund_quotes', json=payload)
+
+    def create_refund(self, order_id: int, *, items: list, payments: list[dict], **kwargs) -> dict:
+        """Create a refund for an order by ID"""
+        payload = {
+            "items": items,
+            "payments": payments,
+            **kwargs,
+        }
+        return self._api.v3.post(f'/orders/{order_id}/payment_actions/refunds', json=payload)
+
     def all_refunds(self, order_id: Optional[int]) -> Iterator[dict]:
         """Return an iterator for all refunds, optionally filtered by order"""
         if order_id:
             endpoint = f'/orders/{order_id}/payment_actions/refunds'
         else:
             endpoint = '/orders/payment_actions/refunds'
         return self._api.v3.get_many(endpoint)
```

### Comparing `bigc-0.2.5/bigc/resources/product_variants.py` & `bigc-0.2.6/bigc/resources/product_variants.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.5/bigc/resources/webhooks.py` & `bigc-0.2.6/bigc/resources/webhooks.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.5/bigc/utils.py` & `bigc-0.2.6/bigc/utils.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.5/pyproject.toml` & `bigc-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bigc"
-version = "0.2.5"
+version = "0.2.6"
 description = "Unofficial client for the BigCommerce API"
 license = "MIT"
 authors = ["Ryan Thomson <ryan@medshift.com>", "Dillon Hartley <dillon@medshift.com>", "Adam Walsh <adam@medshift.com>"]
 readme = "README.md"
 homepage = "https://github.com/MedShift/bigc"
 repository = "https://github.com/MedShift/bigc.git"
 keywords = ["bigcommerce", "api", "client"]
```

### Comparing `bigc-0.2.5/PKG-INFO` & `bigc-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigc
-Version: 0.2.5
+Version: 0.2.6
 Summary: Unofficial client for the BigCommerce API
 Home-page: https://github.com/MedShift/bigc
 License: MIT
 Keywords: bigcommerce,api,client
 Author: Ryan Thomson
 Author-email: ryan@medshift.com
 Requires-Python: >=3.9,<4.0
```

