# Comparing `tmp/budy-api-0.4.0.tar.gz` & `tmp/budy-api-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/budy-api-0.4.0.tar", last modified: Wed Nov 30 07:27:21 2022, max compression
+gzip compressed data, was "dist/budy-api-0.5.0.tar", last modified: Wed May  3 19:24:32 2023, max compression
```

## Comparing `budy-api-0.4.0.tar` & `budy-api-0.5.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-30 07:27:21.000000 budy-api-0.4.0/
--rw-r--r--   0 root         (0) root         (0)     2588 2022-11-30 07:27:15.000000 budy-api-0.4.0/setup.py
--rw-r--r--   0 root         (0) root         (0)     2238 2022-11-30 07:27:15.000000 budy-api-0.4.0/README.md
--rw-r--r--   0 root         (0) root         (0)      997 2022-11-30 07:27:21.000000 budy-api-0.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       67 2022-11-30 07:27:21.000000 budy-api-0.4.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-30 07:27:21.000000 budy-api-0.4.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-30 07:27:21.000000 budy-api-0.4.0/src/budy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-30 07:27:21.000000 budy-api-0.4.0/src/budy/test/
--rw-r--r--   0 root         (0) root         (0)     1173 2022-11-30 07:27:15.000000 budy-api-0.4.0/src/budy/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1850 2022-11-30 07:27:15.000000 budy-api-0.4.0/src/budy/category.py
--rw-r--r--   0 root         (0) root         (0)     1832 2022-11-30 07:27:15.000000 budy-api-0.4.0/src/budy/season.py
--rw-r--r--   0 root         (0) root         (0)     2127 2022-11-30 07:27:15.000000 budy-api-0.4.0/src/budy/address.py
--rw-r--r--   0 root         (0) root         (0)     1491 2022-11-30 07:27:15.000000 budy-api-0.4.0/src/budy/referral.py
--rw-r--r--   0 root         (0) root         (0)     2057 2022-11-30 07:27:15.000000 budy-api-0.4.0/src/budy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1825 2022-11-30 07:27:15.000000 budy-api-0.4.0/src/budy/color.py
--rw-r--r--   0 root         (0) root         (0)     1482 2022-11-30 07:27:15.000000 budy-api-0.4.0/src/budy/subscription.py
--rw-r--r--   0 root         (0) root         (0)     1860 2022-11-30 07:27:15.000000 budy-api-0.4.0/src/budy/collection.py
--rw-r--r--   0 root         (0) root         (0)     1825 2022-11-30 07:27:15.000000 budy-api-0.4.0/src/budy/brand.py
--rw-r--r--   0 root         (0) root         (0)     1839 2022-11-30 07:27:15.000000 budy-api-0.4.0/src/budy/section.py
--rw-r--r--   0 root         (0) root         (0)     1517 2022-11-30 07:27:15.000000 budy-api-0.4.0/src/budy/country.py
--rw-r--r--   0 root         (0) root         (0)     2635 2022-11-30 07:27:15.000000 budy-api-0.4.0/src/budy/product.py
--rw-r--r--   0 root         (0) root         (0)     3637 2022-11-30 07:27:15.000000 budy-api-0.4.0/src/budy/account.py
--rw-r--r--   0 root         (0) root         (0)     4426 2022-11-30 07:27:15.000000 budy-api-0.4.0/src/budy/order.py
--rw-r--r--   0 root         (0) root         (0)     3023 2022-11-30 07:27:15.000000 budy-api-0.4.0/src/budy/bag.py
--rw-r--r--   0 root         (0) root         (0)     1488 2022-11-30 07:27:15.000000 budy-api-0.4.0/src/budy/voucher.py
--rw-r--r--   0 root         (0) root         (0)     4634 2022-11-30 07:27:15.000000 budy-api-0.4.0/src/budy/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-30 07:27:21.000000 budy-api-0.4.0/src/budy_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-30 07:27:21.000000 budy-api-0.4.0/src/budy_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        5 2022-11-30 07:27:21.000000 budy-api-0.4.0/src/budy_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-30 07:27:17.000000 budy-api-0.4.0/src/budy_api.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      605 2022-11-30 07:27:21.000000 budy-api-0.4.0/src/budy_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      997 2022-11-30 07:27:21.000000 budy-api-0.4.0/src/budy_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        7 2022-11-30 07:27:21.000000 budy-api-0.4.0/src/budy_api.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:24:32.000000 budy-api-0.5.0/
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-03 19:24:32.000000 budy-api-0.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:24:32.000000 budy-api-0.5.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:24:32.000000 budy-api-0.5.0/src/budy/
+-rw-r--r--   0 root         (0) root         (0)     2127 2023-05-03 19:24:26.000000 budy-api-0.5.0/src/budy/address.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-05-03 19:24:26.000000 budy-api-0.5.0/src/budy/color.py
+-rw-r--r--   0 root         (0) root         (0)     4676 2023-05-03 19:24:26.000000 budy-api-0.5.0/src/budy/base.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2023-05-03 19:24:26.000000 budy-api-0.5.0/src/budy/season.py
+-rw-r--r--   0 root         (0) root         (0)     1488 2023-05-03 19:24:26.000000 budy-api-0.5.0/src/budy/voucher.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-05-03 19:24:26.000000 budy-api-0.5.0/src/budy/store.py
+-rw-r--r--   0 root         (0) root         (0)     4625 2023-05-03 19:24:26.000000 budy-api-0.5.0/src/budy/order.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-05-03 19:24:26.000000 budy-api-0.5.0/src/budy/country.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-05-03 19:24:26.000000 budy-api-0.5.0/src/budy/category.py
+-rw-r--r--   0 root         (0) root         (0)     1860 2023-05-03 19:24:26.000000 budy-api-0.5.0/src/budy/collection.py
+-rw-r--r--   0 root         (0) root         (0)     1482 2023-05-03 19:24:26.000000 budy-api-0.5.0/src/budy/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     3637 2023-05-03 19:24:26.000000 budy-api-0.5.0/src/budy/account.py
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-05-03 19:24:26.000000 budy-api-0.5.0/src/budy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2635 2023-05-03 19:24:26.000000 budy-api-0.5.0/src/budy/product.py
+-rw-r--r--   0 root         (0) root         (0)     3023 2023-05-03 19:24:26.000000 budy-api-0.5.0/src/budy/bag.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-05-03 19:24:26.000000 budy-api-0.5.0/src/budy/section.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-05-03 19:24:26.000000 budy-api-0.5.0/src/budy/brand.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:24:32.000000 budy-api-0.5.0/src/budy/test/
+-rw-r--r--   0 root         (0) root         (0)     1173 2023-05-03 19:24:26.000000 budy-api-0.5.0/src/budy/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1491 2023-05-03 19:24:26.000000 budy-api-0.5.0/src/budy/referral.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:24:32.000000 budy-api-0.5.0/src/budy_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-03 19:24:32.000000 budy-api-0.5.0/src/budy_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 19:24:32.000000 budy-api-0.5.0/src/budy_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      623 2023-05-03 19:24:32.000000 budy-api-0.5.0/src/budy_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     3468 2023-05-03 19:24:32.000000 budy-api-0.5.0/src/budy_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 19:24:32.000000 budy-api-0.5.0/src/budy_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 19:24:28.000000 budy-api-0.5.0/src/budy_api.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     2755 2023-05-03 19:24:26.000000 budy-api-0.5.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)     2238 2023-05-03 19:24:26.000000 budy-api-0.5.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     3468 2023-05-03 19:24:32.000000 budy-api-0.5.0/PKG-INFO
```

### Comparing `budy-api-0.4.0/setup.py` & `budy-api-0.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 """ The license for the module """
 
 import os
 import setuptools
 
 setuptools.setup(
     name = "budy-api",
-    version = "0.4.0",
+    version = "0.5.0",
     author = "Hive Solutions Lda.",
     author_email = "development@hive.pt",
     description = "Budy API Client",
     license = "Apache License, Version 2.0",
     keywords = "budy api",
     url = "http://budy-api.hive.pt",
     zip_safe = False,
@@ -73,9 +73,11 @@
         "Programming Language :: Python :: 3.1",
         "Programming Language :: Python :: 3.2",
         "Programming Language :: Python :: 3.3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7"
-    ]
+    ],
+    long_description = open(os.path.join(os.path.dirname(__file__), "README.md"), "rb").read().decode("utf-8"),
+    long_description_content_type = "text/markdown"
 )
```

### Comparing `budy-api-0.4.0/README.md` & `budy-api-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `budy-api-0.4.0/src/budy/test/__init__.py` & `budy-api-0.5.0/src/budy/test/__init__.py`

 * *Files identical despite different names*

### Comparing `budy-api-0.4.0/src/budy/category.py` & `budy-api-0.5.0/src/budy/category.py`

 * *Files identical despite different names*

### Comparing `budy-api-0.4.0/src/budy/season.py` & `budy-api-0.5.0/src/budy/season.py`

 * *Files identical despite different names*

### Comparing `budy-api-0.4.0/src/budy/address.py` & `budy-api-0.5.0/src/budy/address.py`

 * *Files identical despite different names*

### Comparing `budy-api-0.4.0/src/budy/referral.py` & `budy-api-0.5.0/src/budy/referral.py`

 * *Files identical despite different names*

### Comparing `budy-api-0.4.0/src/budy/__init__.py` & `budy-api-0.5.0/src/budy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 from . import color
 from . import country
 from . import order
 from . import product
 from . import referral
 from . import season
 from . import section
+from . import store
 from . import subscription
 from . import voucher
 
 from .account import AccountAPI
 from .address import AddressAPI
 from .bag import BagAPI
 from .base import API
@@ -61,9 +62,10 @@
 from .color import ColorAPI
 from .country import CountryAPI
 from .order import OrderAPI
 from .product import ProductAPI
 from .referral import ReferralAPI
 from .season import SeasonAPI
 from .section import SectionAPI
+from .store import StoreAPI
 from .subscription import SubscriptionAPI
 from .voucher import VoucherAPI
```

### Comparing `budy-api-0.4.0/src/budy/color.py` & `budy-api-0.5.0/src/budy/color.py`

 * *Files identical despite different names*

### Comparing `budy-api-0.4.0/src/budy/subscription.py` & `budy-api-0.5.0/src/budy/subscription.py`

 * *Files identical despite different names*

### Comparing `budy-api-0.4.0/src/budy/collection.py` & `budy-api-0.5.0/src/budy/collection.py`

 * *Files identical despite different names*

### Comparing `budy-api-0.4.0/src/budy/brand.py` & `budy-api-0.5.0/src/budy/brand.py`

 * *Files identical despite different names*

### Comparing `budy-api-0.4.0/src/budy/section.py` & `budy-api-0.5.0/src/budy/section.py`

 * *Files identical despite different names*

### Comparing `budy-api-0.4.0/src/budy/country.py` & `budy-api-0.5.0/src/budy/country.py`

 * *Files identical despite different names*

### Comparing `budy-api-0.4.0/src/budy/product.py` & `budy-api-0.5.0/src/budy/product.py`

 * *Files identical despite different names*

### Comparing `budy-api-0.4.0/src/budy/account.py` & `budy-api-0.5.0/src/budy/account.py`

 * *Files identical despite different names*

### Comparing `budy-api-0.4.0/src/budy/order.py` & `budy-api-0.5.0/src/budy/order.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,19 @@
         return contents
 
     def get_order(self, key):
         url = self.base_url + "orders/%s" % key
         contents = self.get(url, auth = False)
         return contents
 
+    def set_store_order(self, key, store_id):
+        url = self.base_url + "orders/%s/store" % key
+        contents = self.put(url, data_j = dict(store_id = store_id))
+        return contents
+
     def set_shipping_address_order(self, key, payload):
         url = self.base_url + "orders/%s/shipping_address" % key
         contents = self.put(url, data_j = payload)
         return contents
 
     def set_billing_address_order(self, key, payload):
         url = self.base_url + "orders/%s/billing_address" % key
```

### Comparing `budy-api-0.4.0/src/budy/bag.py` & `budy-api-0.5.0/src/budy/bag.py`

 * *Files identical despite different names*

### Comparing `budy-api-0.4.0/src/budy/voucher.py` & `budy-api-0.5.0/src/budy/voucher.py`

 * *Files identical despite different names*

### Comparing `budy-api-0.4.0/src/budy/base.py` & `budy-api-0.5.0/src/budy/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
 import appier
 
 from . import bag
 from . import color
 from . import order
 from . import brand
+from . import store
 from . import season
 from . import account
 from . import address
 from . import country
 from . import product
 from . import section
 from . import voucher
@@ -61,14 +62,15 @@
 
 class API(
     appier.API,
     bag.BagAPI,
     color.ColorAPI,
     order.OrderAPI,
     brand.BrandAPI,
+    store.StoreAPI,
     season.SeasonAPI,
     account.AccountAPI,
     address.AddressAPI,
     country.CountryAPI,
     product.ProductAPI,
     section.SectionAPI,
     voucher.VoucherAPI,
```

