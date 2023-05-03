# Comparing `tmp/budy-0.7.9.tar.gz` & `tmp/budy-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/budy-0.7.9.tar", last modified: Mon Mar 20 21:50:20 2023, max compression
+gzip compressed data, was "dist/budy-0.8.0.tar", last modified: Wed May  3 19:23:02 2023, max compression
```

## Comparing `budy-0.7.9.tar` & `budy-0.8.0.tar`

### file list

```diff
@@ -1,102 +1,103 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy/models/
--rw-r--r--   0 root         (0) root         (0)     1304 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/brand.py
--rw-r--r--   0 root         (0) root         (0)     3583 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/country.py
--rw-r--r--   0 root         (0) root         (0)     2220 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/store.py
--rw-r--r--   0 root         (0) root         (0)    14054 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/voucher.py
--rw-r--r--   0 root         (0) root         (0)     2314 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/order_line.py
--rw-r--r--   0 root         (0) root         (0)     1305 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/season.py
--rw-r--r--   0 root         (0) root         (0)     5892 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/bag.py
--rw-r--r--   0 root         (0) root         (0)     1304 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/color.py
--rw-r--r--   0 root         (0) root         (0)     2815 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8248 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/media.py
--rw-r--r--   0 root         (0) root         (0)     2067 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/composition.py
--rw-r--r--   0 root         (0) root         (0)     2425 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/referral.py
--rw-r--r--   0 root         (0) root         (0)     1397 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/live_model.py
--rw-r--r--   0 root         (0) root         (0)    10167 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/bundle_line.py
--rw-r--r--   0 root         (0) root         (0)     1369 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/category.py
--rw-r--r--   0 root         (0) root         (0)     8566 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/account.py
--rw-r--r--   0 root         (0) root         (0)     4880 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/base.py
--rw-r--r--   0 root         (0) root         (0)    39035 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/product.py
--rw-r--r--   0 root         (0) root         (0)     4679 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/section.py
--rw-r--r--   0 root         (0) root         (0)     1919 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/subscription.py
--rw-r--r--   0 root         (0) root         (0)     3207 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/address.py
--rw-r--r--   0 root         (0) root         (0)     1309 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/collection.py
--rw-r--r--   0 root         (0) root         (0)     6046 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/group.py
--rw-r--r--   0 root         (0) root         (0)    13815 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/measurement.py
--rw-r--r--   0 root         (0) root         (0)    17323 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/bundle.py
--rw-r--r--   0 root         (0) root         (0)     4190 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/wishlist.py
--rw-r--r--   0 root         (0) root         (0)     1916 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/wishlist_line.py
--rw-r--r--   0 root         (0) root         (0)    69370 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/order.py
--rw-r--r--   0 root         (0) root         (0)     2512 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/bag_line.py
--rw-r--r--   0 root         (0) root         (0)     4290 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/currency.py
--rw-r--r--   0 root         (0) root         (0)     4115 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/models/exchange_rate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy/controllers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy/controllers/api/
--rw-r--r--   0 root         (0) root         (0)     1988 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/brand.py
--rw-r--r--   0 root         (0) root         (0)     2508 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/country.py
--rw-r--r--   0 root         (0) root         (0)     1636 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/voucher.py
--rw-r--r--   0 root         (0) root         (0)     1518 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/root.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/season.py
--rw-r--r--   0 root         (0) root         (0)     4428 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/bag.py
--rw-r--r--   0 root         (0) root         (0)     1988 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/color.py
--rw-r--r--   0 root         (0) root         (0)     2497 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3427 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/media.py
--rw-r--r--   0 root         (0) root         (0)     1583 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/referral.py
--rw-r--r--   0 root         (0) root         (0)     2032 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/category.py
--rw-r--r--   0 root         (0) root         (0)     2480 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/easypay.py
--rw-r--r--   0 root         (0) root         (0)     5873 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/account.py
--rw-r--r--   0 root         (0) root         (0)     1808 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/base.py
--rw-r--r--   0 root         (0) root         (0)     6299 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/product.py
--rw-r--r--   0 root         (0) root         (0)     2014 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/section.py
--rw-r--r--   0 root         (0) root         (0)     1592 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/subscription.py
--rw-r--r--   0 root         (0) root         (0)     2544 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/address.py
--rw-r--r--   0 root         (0) root         (0)     2048 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/collection.py
--rw-r--r--   0 root         (0) root         (0)    18739 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/order.py
--rw-r--r--   0 root         (0) root         (0)     2589 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/seeplus.py
--rw-r--r--   0 root         (0) root         (0)     2315 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/api/currency.py
--rw-r--r--   0 root         (0) root         (0)     1235 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy/controllers/web/
--rw-r--r--   0 root         (0) root         (0)     1606 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/web/admin.py
--rw-r--r--   0 root         (0) root         (0)     1387 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/web/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1571 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/web/_stripe.py
--rw-r--r--   0 root         (0) root         (0)     2734 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/web/base.py
--rw-r--r--   0 root         (0) root         (0)     2107 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/controllers/web/order.py
--rw-r--r--   0 root         (0) root         (0)     1345 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3069 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy/test/
--rw-r--r--   0 root         (0) root         (0)    14883 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/test/voucher.py
--rw-r--r--   0 root         (0) root         (0)    12257 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/test/bag.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1848 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/test/referral.py
--rw-r--r--   0 root         (0) root         (0)     2805 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/test/account.py
--rw-r--r--   0 root         (0) root         (0)     9252 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/test/product.py
--rw-r--r--   0 root         (0) root         (0)     5692 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/test/measurement.py
--rw-r--r--   0 root         (0) root         (0)     3536 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/test/wishlist.py
--rw-r--r--   0 root         (0) root         (0)    37405 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/test/order.py
--rw-r--r--   0 root         (0) root         (0)     3647 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/test/currency.py
--rw-r--r--   0 root         (0) root         (0)     2238 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/test/exchange_rate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy/templates/
--rw-r--r--   0 root         (0) root         (0)     1112 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/templates/signin.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy/templates/partials/
--rw-r--r--   0 root         (0) root         (0)      452 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/templates/partials/base.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1063 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/templates/partials/internal.html.tpl
--rw-r--r--   0 root         (0) root         (0)       40 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/templates/partials/external.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy/templates/order/
--rw-r--r--   0 root         (0) root         (0)      876 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/templates/order/me.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy/static/js/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-20 21:50:04.000000 budy-0.7.9/src/budy/static/js/main.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-20 21:50:10.000000 budy-0.7.9/src/budy.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     2624 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)    12361 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       32 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-03-20 21:50:20.000000 budy-0.7.9/src/budy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    10669 2023-03-20 21:50:04.000000 budy-0.7.9/README.md
--rw-r--r--   0 root         (0) root         (0)    12361 2023-03-20 21:50:20.000000 budy-0.7.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3127 2023-03-20 21:50:04.000000 budy-0.7.9/setup.py
--rw-r--r--   0 root         (0) root         (0)       67 2023-03-20 21:50:20.000000 budy-0.7.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:23:02.000000 budy-0.8.0/
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-03 19:23:02.000000 budy-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:23:02.000000 budy-0.8.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:23:02.000000 budy-0.8.0/src/budy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:23:02.000000 budy-0.8.0/src/budy/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:23:02.000000 budy-0.8.0/src/budy/static/js/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/static/js/main.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:23:02.000000 budy-0.8.0/src/budy/models/
+-rw-r--r--   0 root         (0) root         (0)     3207 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/address.py
+-rw-r--r--   0 root         (0) root         (0)     1304 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/color.py
+-rw-r--r--   0 root         (0) root         (0)     4880 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/base.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/wishlist_line.py
+-rw-r--r--   0 root         (0) root         (0)     1305 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/season.py
+-rw-r--r--   0 root         (0) root         (0)    14054 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/voucher.py
+-rw-r--r--   0 root         (0) root         (0)     2512 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/bag_line.py
+-rw-r--r--   0 root         (0) root         (0)     6046 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/group.py
+-rw-r--r--   0 root         (0) root         (0)     2378 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/store.py
+-rw-r--r--   0 root         (0) root         (0)    71888 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/order.py
+-rw-r--r--   0 root         (0) root         (0)     3583 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/country.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/category.py
+-rw-r--r--   0 root         (0) root         (0)     4290 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/currency.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/collection.py
+-rw-r--r--   0 root         (0) root         (0)    10167 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/bundle_line.py
+-rw-r--r--   0 root         (0) root         (0)     4115 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/exchange_rate.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     8566 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/account.py
+-rw-r--r--   0 root         (0) root         (0)     2815 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39081 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/product.py
+-rw-r--r--   0 root         (0) root         (0)     5892 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/bag.py
+-rw-r--r--   0 root         (0) root         (0)     4190 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/wishlist.py
+-rw-r--r--   0 root         (0) root         (0)     4679 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/section.py
+-rw-r--r--   0 root         (0) root         (0)     1304 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/brand.py
+-rw-r--r--   0 root         (0) root         (0)     2314 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/order_line.py
+-rw-r--r--   0 root         (0) root         (0)     8248 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/media.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/live_model.py
+-rw-r--r--   0 root         (0) root         (0)    13815 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/measurement.py
+-rw-r--r--   0 root         (0) root         (0)    17323 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/bundle.py
+-rw-r--r--   0 root         (0) root         (0)     2425 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/referral.py
+-rw-r--r--   0 root         (0) root         (0)     2067 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/models/composition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:23:02.000000 budy-0.8.0/src/budy/controllers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:23:02.000000 budy-0.8.0/src/budy/controllers/web/
+-rw-r--r--   0 root         (0) root         (0)     2734 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/web/base.py
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/web/order.py
+-rw-r--r--   0 root         (0) root         (0)     1387 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/web/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/web/_stripe.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/web/admin.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:23:02.000000 budy-0.8.0/src/budy/controllers/api/
+-rw-r--r--   0 root         (0) root         (0)     2544 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/api/address.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/api/easypay.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/api/color.py
+-rw-r--r--   0 root         (0) root         (0)     1808 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/api/base.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/api/season.py
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/api/voucher.py
+-rw-r--r--   0 root         (0) root         (0)     1809 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/api/store.py
+-rw-r--r--   0 root         (0) root         (0)    19173 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/api/order.py
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/api/country.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/api/category.py
+-rw-r--r--   0 root         (0) root         (0)     3190 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/api/seeplus.py
+-rw-r--r--   0 root         (0) root         (0)     2315 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/api/currency.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/api/collection.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/api/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     5873 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/api/account.py
+-rw-r--r--   0 root         (0) root         (0)     2557 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6299 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/api/product.py
+-rw-r--r--   0 root         (0) root         (0)     4428 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/api/bag.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/api/section.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/api/brand.py
+-rw-r--r--   0 root         (0) root         (0)     3427 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/api/media.py
+-rw-r--r--   0 root         (0) root         (0)     1518 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/api/root.py
+-rw-r--r--   0 root         (0) root         (0)     1583 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/controllers/api/referral.py
+-rw-r--r--   0 root         (0) root         (0)     3069 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/main.py
+-rw-r--r--   0 root         (0) root         (0)     1345 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:23:02.000000 budy-0.8.0/src/budy/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:23:02.000000 budy-0.8.0/src/budy/templates/partials/
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/templates/partials/internal.html.tpl
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/templates/partials/external.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      452 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/templates/partials/base.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1112 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/templates/signin.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:23:02.000000 budy-0.8.0/src/budy/templates/order/
+-rw-r--r--   0 root         (0) root         (0)      876 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/templates/order/me.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:23:02.000000 budy-0.8.0/src/budy/test/
+-rw-r--r--   0 root         (0) root         (0)    14883 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/test/voucher.py
+-rw-r--r--   0 root         (0) root         (0)    38933 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/test/order.py
+-rw-r--r--   0 root         (0) root         (0)     3647 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/test/currency.py
+-rw-r--r--   0 root         (0) root         (0)     2238 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/test/exchange_rate.py
+-rw-r--r--   0 root         (0) root         (0)     2805 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/test/account.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9252 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/test/product.py
+-rw-r--r--   0 root         (0) root         (0)    12257 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/test/bag.py
+-rw-r--r--   0 root         (0) root         (0)     3536 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/test/wishlist.py
+-rw-r--r--   0 root         (0) root         (0)     5692 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/test/measurement.py
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-05-03 19:22:46.000000 budy-0.8.0/src/budy/test/referral.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:23:02.000000 budy-0.8.0/src/budy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-03 19:23:02.000000 budy-0.8.0/src/budy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-05-03 19:23:02.000000 budy-0.8.0/src/budy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     2658 2023-05-03 19:23:02.000000 budy-0.8.0/src/budy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)    12361 2023-05-03 19:23:02.000000 budy-0.8.0/src/budy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 19:23:02.000000 budy-0.8.0/src/budy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 19:22:53.000000 budy-0.8.0/src/budy.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     3127 2023-05-03 19:22:46.000000 budy-0.8.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)    10669 2023-05-03 19:22:46.000000 budy-0.8.0/README.md
+-rw-r--r--   0 root         (0) root         (0)    12361 2023-05-03 19:23:02.000000 budy-0.8.0/PKG-INFO
```

### Comparing `budy-0.7.9/src/budy/models/brand.py` & `budy-0.8.0/src/budy/models/brand.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/country.py` & `budy-0.8.0/src/budy/models/country.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/store.py` & `budy-0.8.0/src/budy/models/store.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,19 @@
 """ The license for the module """
 
 import appier
 
 from . import base
 
 class Store(base.BudyBase):
+    """
+    Represents a physical store entity that can be used
+    for the operations like instore pick-up, affecting
+    the checkout process.
+    """
 
     name = appier.field(
         index = True,
         default = True
     )
 
     address = appier.field(
```

### Comparing `budy-0.7.9/src/budy/models/voucher.py` & `budy-0.8.0/src/budy/models/voucher.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/order_line.py` & `budy-0.8.0/src/budy/models/order_line.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/season.py` & `budy-0.8.0/src/budy/models/season.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/bag.py` & `budy-0.8.0/src/budy/models/bag.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/color.py` & `budy-0.8.0/src/budy/models/color.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/__init__.py` & `budy-0.8.0/src/budy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/media.py` & `budy-0.8.0/src/budy/models/media.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/composition.py` & `budy-0.8.0/src/budy/models/composition.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/referral.py` & `budy-0.8.0/src/budy/models/referral.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/live_model.py` & `budy-0.8.0/src/budy/models/live_model.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/bundle_line.py` & `budy-0.8.0/src/budy/models/bundle_line.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/category.py` & `budy-0.8.0/src/budy/models/category.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/account.py` & `budy-0.8.0/src/budy/models/account.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/base.py` & `budy-0.8.0/src/budy/models/base.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/product.py` & `budy-0.8.0/src/budy/models/product.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,25 +116,25 @@
     )
 
     quantity_hand = appier.field(
         type = commons.Decimal,
         index = True,
         observations = """The total quantity that is currently
         available (on hand) for the current product, if not
-        set the product is considered to have unlimited quantity
-        (inventory is not controller)"""
+        set (none) the product is considered to have unlimited quantity
+        (inventory is not controlled)"""
     )
 
     quantity_reserved = appier.field(
         type = commons.Decimal,
         index = True,
         observations = """The total quantity that is currently
         reserved (not available) for the current product, if not
-        set the product is considered to not have reservation
-        control enabled"""
+        set (none) the product is considered to not have reservation
+        control disabled (no reservations are possible)"""
     )
 
     price = appier.field(
         type = commons.Decimal,
         index = True,
         initial = commons.Decimal(0.0),
         observations = """Main retail price to be used for
```

### Comparing `budy-0.7.9/src/budy/models/section.py` & `budy-0.8.0/src/budy/models/section.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/subscription.py` & `budy-0.8.0/src/budy/models/subscription.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/address.py` & `budy-0.8.0/src/budy/models/address.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/collection.py` & `budy-0.8.0/src/budy/models/collection.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/group.py` & `budy-0.8.0/src/budy/models/group.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/measurement.py` & `budy-0.8.0/src/budy/models/measurement.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/bundle.py` & `budy-0.8.0/src/budy/models/bundle.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/wishlist.py` & `budy-0.8.0/src/budy/models/wishlist.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/wishlist_line.py` & `budy-0.8.0/src/budy/models/wishlist_line.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/order.py` & `budy-0.8.0/src/budy/models/order.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,20 @@
         index = "hashed",
         initial = commons.Decimal(0.0),
         safe = True,
         observations = """The total value already used via the
         redeeming of the vouchers associated with the current order"""
     )
 
+    inventory_decremented = appier.field(
+        type = bool,
+        observations = """Controls if the inventory stock levels
+        have been decrement according to current order's lines"""
+    )
+
     lines = appier.field(
         type = appier.references(
             "OrderLine",
             name = "id"
         ),
         eager = True
     )
@@ -220,15 +226,18 @@
     )
 
     store = appier.field(
         type = appier.reference(
             "Store",
             name = "id"
         ),
-        eager = True
+        eager = True,
+        observations = """If set defines the store in which
+        the order should be delivered, in principle the shipping
+        address should be set to the address of the store"""
     )
 
     shipping_address = appier.field(
         type = appier.reference(
             "Address",
             name = "id"
         ),
@@ -958,20 +967,22 @@
     @appier.operation(name = "Mark Paid")
     def mark_paid_s(self):
         self.verify_paid()
         self.status = "paid"
         self.paid = True
         self.date = time.time()
         self.set_reference_f_s()
+        self.decrement_inventory_s()
         self.save()
 
     @appier.operation(name = "Unmark Paid")
     def unmark_paid_s(self):
         self.status = "waiting_payment"
         self.paid = False
+        self.increment_inventory_s()
         self.save()
 
     @appier.operation(name = "Mark Invoiced")
     def mark_invoiced_s(self):
         self.verify_invoiced()
         self.status = "invoiced"
         self.save()
@@ -1058,14 +1069,48 @@
 
     @appier.operation(name = "Fix Closed Lines")
     def fix_closed_s(self):
         if not self.is_closed(): return
         self.close_lines_s()
 
     @appier.operation(
+        name = "Decrement Inventory",
+        description = """Decrements the inventory stock levels
+        according to order lines""",
+        parameters = (("Force", "force", bool, False),),
+        level = 2
+    )
+    def decrement_inventory_s(self, force = False):
+        if self.inventory_decremented and not force: return
+        for line in self.lines:
+            if line.merchandise.quantity_hand == None: continue
+            line.merchandise.quantity_hand =\
+                max(line.merchandise.quantity_hand - line.quantity, 0)
+            line.merchandise.save()
+        self.inventory_decremented = True
+        self.save()
+
+    @appier.operation(
+        name = "Increment Inventory",
+        description = """Increments the inventory stock levels
+        according to order lines (reverses the decrement stock
+        operation, restoring the stock back)""",
+        parameters = (("Force", "force", bool, False),),
+        level = 2
+    )
+    def increment_inventory_s(self, force = False):
+        if not self.inventory_decremented and not force: return
+        for line in self.lines:
+            if line.merchandise.quantity_hand == None: continue
+            line.merchandise.quantity_hand += line.quantity
+            line.merchandise.save()
+        self.inventory_decremented = False
+        self.save()
+
+    @appier.operation(
         name = "Import Omni",
         parameters = (
             ("Invoice", "invoice", bool, True),
             ("Strict", "strict", bool, True),
             ("Sync Prices", "sync_prices", bool, True)
         ),
         level = 2
@@ -1422,29 +1467,31 @@
             message = "Order already imported in Seeplus"
         )
 
         customer = dict()
         if self.account:
             customer = dict(
                 code = str(self.account.id),
-                name = self.account.full_name,
-                email = self.account.email,
-                mobile = self.account.phone_number
+                name = self.account.full_name
             )
+            if self.account.email:
+                customer["email"] = self.account.email
+            if self.account.phone_number:
+                customer["mobile"] = self.account.phone_number
 
         products = []
 
         # iterates over the complete set of order lines to set their
         # values in the product sequence structure for Seeplus
         for line in self.lines:
             products.append(
                 dict(
                     product = line.product.product_id,
                     qty = int(line.quantity),
-                    comment = line.description
+                    comment = line.description or "-"
                 )
             )
 
         order_payload = dict(
             origin = origin,
             code = self.reference,
             orderDate = datetime.datetime.utcfromtimestamp(self.created).strftime("%Y-%m-%dT%H:%M:%SZ"),
@@ -1454,31 +1501,43 @@
                 location = fulfilment,
                 expectedAt = datetime.datetime.now().strftime("%Y-%m-%dT%H:%M:%SZ"),
             ),
             deliveryPickup = dict(
                 location = delivery,
                 scheduledAt = datetime.datetime.now().strftime("%Y-%m-%dT%H:%M:%SZ")
             ),
-            comment = self.description
+            comment = self.description or "-"
         )
 
-        # @TODO perform the remote call here
-        #order = api.create_order(order_payload)
+        # imports the order into the Seeplus infrastructure and obtains
+        # the Seeplus version of the order for reference
+        order = api.create_order(order_payload)
+
+        # captures the timestamp value that is going to be used in the update
+        # operation of the Seeplus system
+        status_timestamp = time.time()
 
-        import pprint
-        pprint.pprint(order_payload)
+        # sets the initial Seeplus updates sequence with the initial
+        # status update operation, this will be used as a log
+        seeplus_updates = [
+            dict(
+                status = order["status"],
+                timestamp = status_timestamp
+            )
+        ]
 
         # updates the complete set of metadata related with the Seeplus
         # import operation so that the order is properly "marked" and
         # the linking can be properly "explorer"
         self.meta.update(
-            seeplus_timestamp = time.time(),
-            seeplus_update = time.time(),
             seeplus_id = order["id"],
-            seeplus_status = order["status"]
+            seeplus_status = order["status"],
+            seeplus_timestamp = status_timestamp,
+            seeplus_update = status_timestamp,
+            seeplus_updates = seeplus_updates
         )
         self.save()
 
     @appier.link(name = "Export Lines CSV")
     def lines_csv_url(self, absolute = False):
         return appier.get_app().url_for(
             "order_api.lines_csv",
```

### Comparing `budy-0.7.9/src/budy/models/bag_line.py` & `budy-0.8.0/src/budy/models/bag_line.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/currency.py` & `budy-0.8.0/src/budy/models/currency.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/models/exchange_rate.py` & `budy-0.8.0/src/budy/models/exchange_rate.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/api/brand.py` & `budy-0.8.0/src/budy/controllers/api/brand.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/api/country.py` & `budy-0.8.0/src/budy/controllers/api/country.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/api/voucher.py` & `budy-0.8.0/src/budy/controllers/api/voucher.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/api/root.py` & `budy-0.8.0/src/budy/controllers/api/root.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/api/season.py` & `budy-0.8.0/src/budy/controllers/api/season.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/api/bag.py` & `budy-0.8.0/src/budy/controllers/api/bag.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/api/color.py` & `budy-0.8.0/src/budy/controllers/api/color.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/api/__init__.py` & `budy-0.8.0/src/budy/controllers/api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 from . import media
 from . import order
 from . import product
 from . import referral
 from . import root
 from . import section
 from . import seeplus
+from . import store
 from . import subscription
 from . import voucher
 
 from .account import AccountAPIController
 from .address import AddressAPIController
 from .bag import BagAPIController
 from .base import BaseAPIController
@@ -70,9 +71,10 @@
 from .order import OrderAPIController
 from .product import ProductAPIController
 from .referral import ReferralAPIController
 from .root import RootAPIController
 from .season import SeasonAPIController
 from .section import SectionAPIController
 from .seeplus import SeeplusAPIController
+from .store import StoreAPIController
 from .subscription import SubscriptionAPIController
 from .voucher import VoucherAPIController
```

### Comparing `budy-0.7.9/src/budy/controllers/api/media.py` & `budy-0.8.0/src/budy/controllers/api/media.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/api/referral.py` & `budy-0.8.0/src/budy/controllers/api/referral.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/api/category.py` & `budy-0.8.0/src/budy/controllers/api/category.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/api/easypay.py` & `budy-0.8.0/src/budy/controllers/api/easypay.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/api/account.py` & `budy-0.8.0/src/budy/controllers/api/account.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/api/base.py` & `budy-0.8.0/src/budy/controllers/api/base.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/api/product.py` & `budy-0.8.0/src/budy/controllers/api/product.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/api/section.py` & `budy-0.8.0/src/budy/controllers/api/section.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/api/subscription.py` & `budy-0.8.0/src/budy/controllers/api/subscription.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/api/address.py` & `budy-0.8.0/src/budy/controllers/api/address.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/api/collection.py` & `budy-0.8.0/src/budy/controllers/api/collection.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/api/order.py` & `budy-0.8.0/src/budy/controllers/api/order.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,14 +269,26 @@
                 "lines.product.images",
                 "lines.product.brand"
             ),
             map = True
         )
         return order
 
+    @appier.route("/api/orders/<str:key>/store", "PUT", json = True)
+    @appier.ensure(token = "user")
+    def set_store(self, key):
+        data = appier.request_json()
+        store_id = data["store_id"]
+        store = budy.Store.get(id = store_id)
+        order = budy.Order.get(key = key, rules = False)
+        order.store = store
+        order.save()
+        order = order.reload(map = True)
+        return order
+
     @appier.route("/api/orders/<str:key>/shipping_address", "PUT", json = True)
     @appier.ensure(token = "user")
     def set_shipping_address(self, key):
         address = budy.Address.new()
         address.save()
         order = budy.Order.get(key = key, rules = False)
         order.shipping_address = address
```

### Comparing `budy-0.7.9/src/budy/controllers/api/seeplus.py` & `budy-0.8.0/src/budy/controllers/api/seeplus.py`

 * *Files 17% similar despite different names*

```diff
@@ -45,36 +45,51 @@
 
 from . import root
 
 class SeeplusAPIController(root.RootAPIController):
 
     @appier.route("/api/seeplus/update", "POST", json = True)
     def update(self):
-        key = self.request.get_header("X-Seeplus-Key", None)
+        key = self.field("token", None)
+        key = self.field("key", key)
+        key = self.request.get_header("X-Seeplus-Key", key)
         _key = appier.conf("SEEPLUS_KEY", None)
         if _key and not _key == key:
             raise appier.SecurityError(
                 message = "Mismatch in Seeplus key",
-                code = 401 
+                code = 401
             )
         object = appier.get_object()
         event = object.get("event", "OrderManagement.StatusChanged")
         data = object.get("data", {})
         result = "Ignored"
         if event == "OrderManagement.StatusChanged":
             self._status_change_s(data)
             result = "Handled"
         return dict(result = result)
 
     def _status_change_s(self, data):
         reference = data["code"]
         status = data["status"]
         order = budy.Order.get(reference = reference)
+        seeplus_status = order.meta.get("seeplus_status", None)
         seeplus_timestamp = order.meta.get("seeplus_timestamp", None)
+        seeplus_updates = order.meta.get("seeplus_updates", [])
         if not seeplus_timestamp: raise appier.OperationalError(
             message = "Order not imported in Seeplus"
         )
+        if status == seeplus_status: raise appier.OperationalError(
+            message = "Order already in status '%s'" % status
+        )
+        status_timestamp = time.time()
+        seeplus_updates.append(
+            dict(
+                status = status,
+                timestamp = status_timestamp
+            )
+        )
         order.meta.update(
             seeplus_status = status,
-            seeplus_update = time.time()
+            seeplus_update = status_timestamp,
+            seeplus_updates = seeplus_updates
         )
         order.save()
```

### Comparing `budy-0.7.9/src/budy/controllers/api/currency.py` & `budy-0.8.0/src/budy/controllers/api/currency.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/__init__.py` & `budy-0.8.0/src/budy/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/web/admin.py` & `budy-0.8.0/src/budy/controllers/web/admin.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/web/__init__.py` & `budy-0.8.0/src/budy/controllers/web/__init__.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/web/_stripe.py` & `budy-0.8.0/src/budy/controllers/web/_stripe.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/web/base.py` & `budy-0.8.0/src/budy/controllers/web/base.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/controllers/web/order.py` & `budy-0.8.0/src/budy/controllers/web/order.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/__init__.py` & `budy-0.8.0/src/budy/__init__.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/main.py` & `budy-0.8.0/src/budy/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     def get_seeplus_api(self):
         import seeplus
         if self.seeplus_api: return self.seeplus_api
         self.seeplus_api = seeplus.API()
         return self.seeplus_api
 
     def _version(self):
-        return "0.7.9"
+        return "0.8.0"
 
     def _description(self):
         return "Budy"
 
     def _observations(self):
         return "Simple and easy to use E-commerce engine"
```

### Comparing `budy-0.7.9/src/budy/test/voucher.py` & `budy-0.8.0/src/budy/test/voucher.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/test/bag.py` & `budy-0.8.0/src/budy/test/bag.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/test/__init__.py` & `budy-0.8.0/src/budy/test/__init__.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/test/referral.py` & `budy-0.8.0/src/budy/test/referral.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/test/account.py` & `budy-0.8.0/src/budy/test/account.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/test/product.py` & `budy-0.8.0/src/budy/test/product.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/test/measurement.py` & `budy-0.8.0/src/budy/test/measurement.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/test/wishlist.py` & `budy-0.8.0/src/budy/test/wishlist.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/test/order.py` & `budy-0.8.0/src/budy/test/order.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,16 @@
         adapter = appier.get_adapter()
         adapter.drop_db()
 
     def test_basic(self):
         product = budy.Product(
             short_description = "product",
             gender = "Male",
-            price = 10.0
+            price = 10.0,
+            quantity_hand = 5.0
         )
         product.save()
 
         self.assertEqual(product.short_description, "product")
         self.assertEqual(product.gender, "Male")
         self.assertEqual(product.price, 10.0)
 
@@ -75,14 +76,15 @@
         self.assertEqual(type(order.total), commons.Decimal)
         self.assertEqual(len(order.lines), 0)
         self.assertEqual(order.id, 1)
         self.assertEqual(order.reference, "BD-000001")
         self.assertEqual(order.currency, None)
         self.assertEqual(order.total >= 0.0, True)
         self.assertEqual(order.paid, False)
+        self.assertEqual(order.inventory_decremented, False)
         self.assertEqual(order.date, None)
         self.assertEqual(order.notifications, [])
 
         self.assertRaises(appier.AssertionError, order.verify_base)
         self.assertRaises(appier.AssertionError, order.verify_shippable)
         self.assertRaises(appier.AssertionError, order.mark_paid_s)
 
@@ -133,19 +135,25 @@
         order.email = "username@email.com"
         order.save()
 
         order.mark_waiting_payment_s()
 
         self.assertEqual(order.status, "waiting_payment")
         self.assertEqual(order.paid, False)
+        self.assertEqual(order.inventory_decremented, False)
 
         order.mark_paid_s()
 
         self.assertEqual(order.status, "paid")
         self.assertEqual(order.paid, True)
+        self.assertEqual(order.inventory_decremented, True)
+
+        product = product.reload()
+
+        self.assertEqual(product.quantity_hand, 3)
 
         self.assertRaises(appier.AssertionError, order.mark_paid_s)
 
     def test_referral(self):
         order = budy.Order()
         order.save()
 
@@ -386,29 +394,31 @@
             payment_data = dict(type = "simple"),
             payment_function = _pay_dummy
         )
 
         self.assertEqual(order.is_valid(), True)
         self.assertEqual(order_line.is_valid_quantity(), True)
         self.assertEqual(order.paid, False)
+        self.assertEqual(order.inventory_decremented, False)
         self.assertEqual(order.status, "waiting_payment")
 
         self.assertRaises(
             appier.SecurityError,
             lambda: order.pay_s(
                 payment_data = dict(type = "simple"),
                 payment_function = _pay_dummy
             )
         )
 
     def test_voucher_use(self):
         product = budy.Product(
             short_description = "product",
             gender = "Male",
-            price = 10.0
+            price = 10.0,
+            quantity_hand = 5.0
         )
         product.save()
 
         order = budy.Order()
         order.save()
 
         order_line = budy.OrderLine(quantity = 2.0)
@@ -449,14 +459,15 @@
         self.assertEqual(voucher.used_amount, 1.0)
         self.assertEqual(voucher.open_amount, 0.0)
         self.assertEqual(voucher.usage_count, 1)
 
         self.assertEqual(order.is_valid(), True)
         self.assertEqual(order_line.is_valid_quantity(), True)
         self.assertEqual(order.paid, False)
+        self.assertEqual(order.inventory_decremented, False)
         self.assertEqual(order.status, "waiting_payment")
 
         order.end_pay_s(
             payment_data = dict(type = "simple"),
             strict = False
         )
 
@@ -466,14 +477,19 @@
         self.assertEqual(voucher.open_amount, 0.0)
         self.assertEqual(voucher.usage_count, 1)
 
         self.assertEqual(order.is_valid(), True)
         self.assertEqual(order_line.is_valid_quantity(), True)
         self.assertEqual(order.paid, True)
         self.assertEqual(order.status, "paid")
+        self.assertEqual(order.inventory_decremented, True)
+
+        product = product.reload()
+
+        self.assertEqual(product.quantity_hand, 3.0)
 
         order.date = None
         order.status = "created"
         order.unmark_paid_s()
 
         voucher = budy.Voucher(amount = 1.0)
         voucher.save()
@@ -490,14 +506,15 @@
         self.assertEqual(voucher.used_amount, 1.0)
         self.assertEqual(voucher.open_amount, 0.0)
         self.assertEqual(voucher.usage_count, 1)
 
         self.assertEqual(order.is_valid(), True)
         self.assertEqual(order_line.is_valid_quantity(), True)
         self.assertEqual(order.paid, False)
+        self.assertEqual(order.inventory_decremented, False)
         self.assertEqual(order.status, "waiting_payment")
 
         order.cancel_s()
 
         voucher = voucher.reload()
 
         self.assertEqual(voucher.is_valid(), True)
@@ -505,14 +522,15 @@
         self.assertEqual(voucher.used_amount, 0.0)
         self.assertEqual(voucher.open_amount, 1.0)
         self.assertEqual(voucher.usage_count, 0)
 
         self.assertEqual(order.is_valid(), True)
         self.assertEqual(order_line.is_valid_quantity(), True)
         self.assertEqual(order.paid, False)
+        self.assertEqual(order.inventory_decremented, False)
         self.assertEqual(order.status, "canceled")
 
         order.date = None
         order.status = "created"
         order.unmark_paid_s()
 
         voucher = budy.Voucher(amount = 1.0)
@@ -535,29 +553,35 @@
         self.assertEqual(voucher.used_amount, 1.0)
         self.assertEqual(voucher.open_amount, 0.0)
         self.assertEqual(voucher.usage_count, 1)
 
         self.assertEqual(order.is_valid(), True)
         self.assertEqual(order_line.is_valid_quantity(), True)
         self.assertEqual(order.paid, True)
+        self.assertEqual(order.inventory_decremented, True)
         self.assertEqual(order.status, "paid")
 
+        product = product.reload()
+
+        self.assertEqual(product.quantity_hand, 3.0)
+
         order.cancel_s()
 
         voucher = voucher.reload()
 
         self.assertEqual(voucher.is_valid(), False)
         self.assertEqual(voucher.amount, 1.0)
         self.assertEqual(voucher.used_amount, 1.0)
         self.assertEqual(voucher.open_amount, 0.0)
         self.assertEqual(voucher.usage_count, 1)
 
         self.assertEqual(order.is_valid(), True)
         self.assertEqual(order_line.is_valid_quantity(), True)
         self.assertEqual(order.paid, True)
+        self.assertEqual(order.inventory_decremented, True)
         self.assertEqual(order.status, "canceled")
 
     def test_discount(self):
         product = budy.Product(
             short_description = "product",
             gender = "Male",
             price = 10.0
@@ -927,15 +951,16 @@
         self.assertEqual(order.payable, 24.0)
         self.assertEqual(order.discountable, 24.0)
 
     def test_free(self):
         product = budy.Product(
             short_description = "product",
             gender = "Male",
-            price = 10.0
+            price = 10.0,
+            quantity_hand = 5.0
         )
         product.save()
 
         order = budy.Order()
         order.save()
 
         order_line = budy.OrderLine(quantity = 2.0)
@@ -968,35 +993,41 @@
 
         self.assertEqual(order.sub_total, 20.0)
         self.assertEqual(order.discount, 20.0)
         self.assertEqual(order.total, 0.0)
         self.assertEqual(order.payable, 0.0)
         self.assertEqual(order.discountable, 20.0)
         self.assertEqual(order.paid, False)
+        self.assertEqual(order.inventory_decremented, False)
         self.assertEqual(isinstance(order.sub_total, commons.Decimal), True)
         self.assertEqual(isinstance(order.discount, commons.Decimal), True)
         self.assertEqual(isinstance(order.total, commons.Decimal), True)
         self.assertEqual(isinstance(order.payable, commons.Decimal), True)
         self.assertEqual(isinstance(order.discountable, commons.Decimal), True)
 
         order.pay_s()
 
         self.assertEqual(order.sub_total, 20.0)
         self.assertEqual(order.discount, 20.0)
         self.assertEqual(order.total, 0.0)
         self.assertEqual(order.payable, 0.0)
         self.assertEqual(order.discountable, 20.0)
         self.assertEqual(order.paid, True)
+        self.assertEqual(order.inventory_decremented, True)
         self.assertEqual(order.payment_data, {})
         self.assertEqual(isinstance(order.sub_total, commons.Decimal), True)
         self.assertEqual(isinstance(order.discount, commons.Decimal), True)
         self.assertEqual(isinstance(order.total, commons.Decimal), True)
         self.assertEqual(isinstance(order.payable, commons.Decimal), True)
         self.assertEqual(isinstance(order.discountable, commons.Decimal), True)
 
+        product = product.reload()
+
+        self.assertEqual(product.quantity_hand, 3.0)
+
     def test_closed(self):
         order = budy.Order()
         order.save()
 
         product = budy.Product(
             short_description = "product",
             gender = "Male",
@@ -1030,15 +1061,16 @@
         self.assertEqual(order.is_open(), False)
         self.assertEqual(order.is_closed(), True)
 
     def test_payment_method(self):
         product = budy.Product(
             short_description = "product",
             gender = "Male",
-            price = 10.0
+            price = 10.0,
+            quantity_hand = 5.0
         )
         product.save()
 
         order = budy.Order()
         order.save()
 
         order_line = budy.OrderLine(quantity = 2.0)
@@ -1063,14 +1095,15 @@
         order.billing_address = address
         order.email = "username@email.com"
         order.save()
 
         self.assertEqual(order.is_valid(), True)
         self.assertEqual(order_line.is_valid_quantity(), True)
         self.assertEqual(order.paid, False)
+        self.assertEqual(order.inventory_decremented, False)
         self.assertEqual(order.status, "created")
 
         self.assertRaises(
             appier.SecurityError,
             lambda: order.pay_s(payment_data = dict(type = "simple"))
         )
 
@@ -1078,14 +1111,15 @@
             payment_data = dict(type = "simple"),
             strict = False
         )
 
         self.assertEqual(order.is_valid(), True)
         self.assertEqual(order_line.is_valid_quantity(), True)
         self.assertEqual(order.paid, False)
+        self.assertEqual(order.inventory_decremented, False)
         self.assertEqual(order.status, "waiting_payment")
 
         self.assertRaises(
             appier.SecurityError,
             lambda: order.end_pay_s(
                 payment_data = dict(type = "simple"),
                 strict = True
@@ -1095,16 +1129,21 @@
         order.end_pay_s(
             payment_data = dict(type = "simple")
         )
 
         self.assertEqual(order.is_valid(), True)
         self.assertEqual(order_line.is_valid_quantity(), True)
         self.assertEqual(order.paid, True)
+        self.assertEqual(order.inventory_decremented, True)
         self.assertEqual(order.status, "paid")
 
+        product = product.reload()
+
+        self.assertEqual(product.quantity_hand, 3.0)
+
     def test__build_notes(self):
         product = budy.Product(
             short_description = "product",
             gender = "Male",
             price = 10.0
         )
         product.save()
```

### Comparing `budy-0.7.9/src/budy/test/currency.py` & `budy-0.8.0/src/budy/test/currency.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/test/exchange_rate.py` & `budy-0.8.0/src/budy/test/exchange_rate.py`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/templates/signin.html.tpl` & `budy-0.8.0/src/budy/templates/signin.html.tpl`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/templates/partials/internal.html.tpl` & `budy-0.8.0/src/budy/templates/partials/internal.html.tpl`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy/templates/order/me.html.tpl` & `budy-0.8.0/src/budy/templates/order/me.html.tpl`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/src/budy.egg-info/SOURCES.txt` & `budy-0.8.0/src/budy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 src/budy/controllers/api/order.py
 src/budy/controllers/api/product.py
 src/budy/controllers/api/referral.py
 src/budy/controllers/api/root.py
 src/budy/controllers/api/season.py
 src/budy/controllers/api/section.py
 src/budy/controllers/api/seeplus.py
+src/budy/controllers/api/store.py
 src/budy/controllers/api/subscription.py
 src/budy/controllers/api/voucher.py
 src/budy/controllers/web/__init__.py
 src/budy/controllers/web/_stripe.py
 src/budy/controllers/web/admin.py
 src/budy/controllers/web/base.py
 src/budy/controllers/web/order.py
```

### Comparing `budy-0.7.9/src/budy.egg-info/PKG-INFO` & `budy-0.8.0/src/budy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: budy
-Version: 0.7.9
+Version: 0.8.0
 Summary: Budy E-commerce System
 Home-page: http://budy.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Budy](http://budy.hive.pt)
```

### Comparing `budy-0.7.9/README.md` & `budy-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `budy-0.7.9/PKG-INFO` & `budy-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: budy
-Version: 0.7.9
+Version: 0.8.0
 Summary: Budy E-commerce System
 Home-page: http://budy.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Budy](http://budy.hive.pt)
```

### Comparing `budy-0.7.9/setup.py` & `budy-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 """ The license for the module """
 
 import os
 import setuptools
 
 setuptools.setup(
     name = "budy",
-    version = "0.7.9",
+    version = "0.8.0",
     author = "Hive Solutions Lda.",
     author_email = "development@hive.pt",
     description = "Budy E-commerce System",
     license = "Apache License, Version 2.0",
     keywords = "budy e-commerce engine web json",
     url = "http://budy.hive.pt",
     zip_safe = False,
```

