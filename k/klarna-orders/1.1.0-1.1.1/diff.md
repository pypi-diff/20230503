# Comparing `tmp/klarna-orders-1.1.0.tar.gz` & `tmp/klarna-orders-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klarna-orders-1.1.0.tar", last modified: Tue Apr 18 00:08:27 2023, max compression
+gzip compressed data, was "klarna-orders-1.1.1.tar", last modified: Tue Apr 18 06:44:36 2023, max compression
```

## Comparing `klarna-orders-1.1.0.tar` & `klarna-orders-1.1.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:08:27.616397 klarna-orders-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-18 00:08:27.616397 klarna-orders-1.1.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     7475 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 00:08:27.616397 klarna-orders-1.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1113 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:08:27.612398 klarna-orders-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:08:27.612398 klarna-orders-1.1.0/src/klarna/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1864 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/authorizations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:08:27.612398 klarna-orders-1.1.0/src/klarna/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:08:27.612398 klarna-orders-1.1.0/src/klarna/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      659 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/operations/cancelauthorization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      643 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/operations/createcreditsession.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1068 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/operations/createorder.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1490 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/operations/purchasetoken.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      845 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/operations/readcreditsession.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      867 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/operations/updatecreditsession.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:08:27.616397 klarna-orders-1.1.0/src/klarna/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1567 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4549 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/address.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/asset_urls.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      995 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1413 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/authorized_payment_method.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5395 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/create_order_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3823 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/customer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3167 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/customer_read.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      844 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/customer_read_create_token.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1940 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/customer_token_creation_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2075 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/customer_token_creation_response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1733 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/errorv2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1282 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/merchant_session.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/merchant_urls.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1830 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/options.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2075 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/order.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4993 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/order_line.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1496 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/payment_method_category.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2258 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/product_identifiers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      336 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7597 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/session.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7433 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/session_create.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9509 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/session_read.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/subscription.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2840 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/orders.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3581 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5485 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/sessions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2864 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:08:27.616397 klarna-orders-1.1.0/src/klarna/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:08:27.616397 klarna-orders-1.1.0/src/klarna_orders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-18 00:08:27.000000 klarna-orders-1.1.0/src/klarna_orders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-18 00:08:27.000000 klarna-orders-1.1.0/src/klarna_orders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 00:08:27.000000 klarna-orders-1.1.0/src/klarna_orders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-18 00:08:27.000000 klarna-orders-1.1.0/src/klarna_orders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 00:08:27.000000 klarna-orders-1.1.0/src/klarna_orders.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:44:36.675290 klarna-orders-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-18 06:44:36.675290 klarna-orders-1.1.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7475 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 06:44:36.679290 klarna-orders-1.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1113 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:44:36.667290 klarna-orders-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:44:36.667290 klarna-orders-1.1.1/src/klarna/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1864 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/authorizations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:44:36.667290 klarna-orders-1.1.1/src/klarna/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:44:36.671290 klarna-orders-1.1.1/src/klarna/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      659 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/operations/cancelauthorization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      643 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/operations/createcreditsession.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1068 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/operations/createorder.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1490 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/operations/purchasetoken.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      845 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/operations/readcreditsession.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      867 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/operations/updatecreditsession.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:44:36.675290 klarna-orders-1.1.1/src/klarna/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1567 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4549 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/shared/address.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/shared/asset_urls.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      995 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/shared/attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1413 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/shared/authorized_payment_method.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5395 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/shared/create_order_request.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3823 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/shared/customer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3167 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/shared/customer_read.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      844 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/shared/customer_read_create_token.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1940 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/shared/customer_token_creation_request.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2075 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/shared/customer_token_creation_response.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1733 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/shared/errorv2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1282 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/shared/merchant_session.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/shared/merchant_urls.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1830 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/shared/options.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2075 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/shared/order.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4993 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/shared/order_line.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1496 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/shared/payment_method_category.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2258 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/shared/product_identifiers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      336 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7597 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/shared/session.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7433 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/shared/session_create.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9509 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/shared/session_read.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/models/shared/subscription.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2840 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/orders.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3581 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5485 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/sessions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2864 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:44:36.675290 klarna-orders-1.1.1/src/klarna/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-18 06:44:22.000000 klarna-orders-1.1.1/src/klarna/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:44:36.675290 klarna-orders-1.1.1/src/klarna_orders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-18 06:44:36.000000 klarna-orders-1.1.1/src/klarna_orders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-18 06:44:36.000000 klarna-orders-1.1.1/src/klarna_orders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 06:44:36.000000 klarna-orders-1.1.1/src/klarna_orders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-18 06:44:36.000000 klarna-orders-1.1.1/src/klarna_orders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 06:44:36.000000 klarna-orders-1.1.1/src/klarna_orders.egg-info/top_level.txt
```

### Comparing `klarna-orders-1.1.0/LICENSE.md` & `klarna-orders-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/PKG-INFO` & `klarna-orders-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klarna-orders
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy-Klarna
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: klarna-orders Version: 1.1.0 Summary: Python Client
+Metadata-Version: 2.1 Name: klarna-orders Version: 1.1.1 Summary: Python Client
 SDK Generated by Speakeasy Home-page: UNKNOWN Author: Speakeasy-Klarna License:
 UNKNOWN Platform: UNKNOWN Requires-Python: >=3.9 Description-Content-Type:
 text/markdown License-File: LICENSE.md
   [https://user-images.githubusercontent.com/6267663/230347878-f2873a58-f578-
                           4e95-86e0-7bebfd78f4f1.svg]
                            ****** Python SDK ******
                 An effortless integration. Designed for growth.
```

### Comparing `klarna-orders-1.1.0/README.md` & `klarna-orders-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/setup.py` & `klarna-orders-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="klarna-orders",
-    version="1.1.0",
+    version="1.1.1",
     author="Speakeasy-Klarna",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.07",
```

### Comparing `klarna-orders-1.1.0/src/klarna/authorizations.py` & `klarna-orders-1.1.1/src/klarna/authorizations.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/operations/__init__.py` & `klarna-orders-1.1.1/src/klarna/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/operations/cancelauthorization.py` & `klarna-orders-1.1.1/src/klarna/models/operations/cancelauthorization.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/operations/createcreditsession.py` & `klarna-orders-1.1.1/src/klarna/models/operations/createcreditsession.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/operations/createorder.py` & `klarna-orders-1.1.1/src/klarna/models/operations/createorder.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/operations/purchasetoken.py` & `klarna-orders-1.1.1/src/klarna/models/operations/purchasetoken.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/operations/readcreditsession.py` & `klarna-orders-1.1.1/src/klarna/models/operations/readcreditsession.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/operations/updatecreditsession.py` & `klarna-orders-1.1.1/src/klarna/models/operations/updatecreditsession.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/shared/__init__.py` & `klarna-orders-1.1.1/src/klarna/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/shared/address.py` & `klarna-orders-1.1.1/src/klarna/models/shared/address.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/shared/asset_urls.py` & `klarna-orders-1.1.1/src/klarna/models/shared/asset_urls.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/shared/attachment.py` & `klarna-orders-1.1.1/src/klarna/models/shared/attachment.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/shared/authorized_payment_method.py` & `klarna-orders-1.1.1/src/klarna/models/shared/authorized_payment_method.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/shared/create_order_request.py` & `klarna-orders-1.1.1/src/klarna/models/shared/create_order_request.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/shared/customer.py` & `klarna-orders-1.1.1/src/klarna/models/shared/customer.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/shared/customer_read.py` & `klarna-orders-1.1.1/src/klarna/models/shared/customer_read.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/shared/customer_read_create_token.py` & `klarna-orders-1.1.1/src/klarna/models/shared/customer_read_create_token.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/shared/customer_token_creation_request.py` & `klarna-orders-1.1.1/src/klarna/models/shared/customer_token_creation_request.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/shared/customer_token_creation_response.py` & `klarna-orders-1.1.1/src/klarna/models/shared/customer_token_creation_response.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/shared/errorv2.py` & `klarna-orders-1.1.1/src/klarna/models/shared/errorv2.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/shared/merchant_session.py` & `klarna-orders-1.1.1/src/klarna/models/shared/merchant_session.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/shared/merchant_urls.py` & `klarna-orders-1.1.1/src/klarna/models/shared/merchant_urls.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/shared/options.py` & `klarna-orders-1.1.1/src/klarna/models/shared/options.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/shared/order.py` & `klarna-orders-1.1.1/src/klarna/models/shared/order.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/shared/order_line.py` & `klarna-orders-1.1.1/src/klarna/models/shared/order_line.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/shared/payment_method_category.py` & `klarna-orders-1.1.1/src/klarna/models/shared/payment_method_category.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/shared/product_identifiers.py` & `klarna-orders-1.1.1/src/klarna/models/shared/product_identifiers.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/shared/session.py` & `klarna-orders-1.1.1/src/klarna/models/shared/session.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/shared/session_create.py` & `klarna-orders-1.1.1/src/klarna/models/shared/session_create.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/shared/session_read.py` & `klarna-orders-1.1.1/src/klarna/models/shared/session_read.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/models/shared/subscription.py` & `klarna-orders-1.1.1/src/klarna/models/shared/subscription.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/orders.py` & `klarna-orders-1.1.1/src/klarna/orders.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/sdk.py` & `klarna-orders-1.1.1/src/klarna/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     tokens: Tokens
     r"""Operations related to token"""
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "1.1.0"
-    _gen_version: str = "2.18.0"
+    _sdk_version: str = "1.1.1"
+    _gen_version: str = "2.18.1"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
```

### Comparing `klarna-orders-1.1.0/src/klarna/sessions.py` & `klarna-orders-1.1.1/src/klarna/sessions.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/tokens.py` & `klarna-orders-1.1.1/src/klarna/tokens.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/utils/retries.py` & `klarna-orders-1.1.1/src/klarna/utils/retries.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna/utils/utils.py` & `klarna-orders-1.1.1/src/klarna/utils/utils.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.1.0/src/klarna_orders.egg-info/PKG-INFO` & `klarna-orders-1.1.1/src/klarna_orders.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klarna-orders
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy-Klarna
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: klarna-orders Version: 1.1.0 Summary: Python Client
+Metadata-Version: 2.1 Name: klarna-orders Version: 1.1.1 Summary: Python Client
 SDK Generated by Speakeasy Home-page: UNKNOWN Author: Speakeasy-Klarna License:
 UNKNOWN Platform: UNKNOWN Requires-Python: >=3.9 Description-Content-Type:
 text/markdown License-File: LICENSE.md
   [https://user-images.githubusercontent.com/6267663/230347878-f2873a58-f578-
                           4e95-86e0-7bebfd78f4f1.svg]
                            ****** Python SDK ******
                 An effortless integration. Designed for growth.
```

### Comparing `klarna-orders-1.1.0/src/klarna_orders.egg-info/SOURCES.txt` & `klarna-orders-1.1.1/src/klarna_orders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

