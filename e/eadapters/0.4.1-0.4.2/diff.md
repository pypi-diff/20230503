# Comparing `tmp/eadapters-0.4.1.tar.gz` & `tmp/eadapters-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eadapters-0.4.1.tar", last modified: Sat Jun 25 11:52:18 2022, max compression
+gzip compressed data, was "dist/eadapters-0.4.2.tar", last modified: Wed May  3 19:25:26 2023, max compression
```

## Comparing `eadapters-0.4.1.tar` & `eadapters-0.4.2.tar`

### file list

```diff
@@ -1,85 +1,87 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 11:52:18.000000 eadapters-0.4.1/
--rw-r--r--   0 root         (0) root         (0)     1422 2022-06-25 11:52:12.000000 eadapters-0.4.1/setup.py
--rw-r--r--   0 root         (0) root         (0)     1032 2022-06-25 11:52:18.000000 eadapters-0.4.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 11:52:18.000000 eadapters-0.4.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 11:52:18.000000 eadapters-0.4.1/src/eadapters.egg-info/
--rw-r--r--   0 root         (0) root         (0)       10 2022-06-25 11:52:18.000000 eadapters-0.4.1/src/eadapters.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1032 2022-06-25 11:52:18.000000 eadapters-0.4.1/src/eadapters.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        9 2022-06-25 11:52:18.000000 eadapters-0.4.1/src/eadapters.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     2732 2022-06-25 11:52:18.000000 eadapters-0.4.1/src/eadapters.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-25 11:52:18.000000 eadapters-0.4.1/src/eadapters.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-25 11:52:14.000000 eadapters-0.4.1/src/eadapters.egg-info/not-zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 11:52:18.000000 eadapters-0.4.1/src/eadapters/
--rw-r--r--   0 root         (0) root         (0)     2754 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 11:52:18.000000 eadapters-0.4.1/src/eadapters/models/
--rw-r--r--   0 root         (0) root         (0)      108 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/color.py
--rw-r--r--   0 root         (0) root         (0)     1173 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/order_line.py
--rw-r--r--   0 root         (0) root         (0)      144 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/merchant.py
--rw-r--r--   0 root         (0) root         (0)     2150 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/base.py
--rw-r--r--   0 root         (0) root         (0)      107 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/voucher.py
--rw-r--r--   0 root         (0) root         (0)      108 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/referral.py
--rw-r--r--   0 root         (0) root         (0)      111 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/category.py
--rw-r--r--   0 root         (0) root         (0)      296 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/group.py
--rw-r--r--   0 root         (0) root         (0)      107 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/payment.py
--rw-r--r--   0 root         (0) root         (0)      109 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/season.py
--rw-r--r--   0 root         (0) root         (0)     2180 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/order.py
--rw-r--r--   0 root         (0) root         (0)     1704 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/bag_line.py
--rw-r--r--   0 root         (0) root         (0)      182 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/currency.py
--rw-r--r--   0 root         (0) root         (0)      108 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/brand.py
--rw-r--r--   0 root         (0) root         (0)      114 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/shipping_option.py
--rw-r--r--   0 root         (0) root         (0)      106 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/credit.py
--rw-r--r--   0 root         (0) root         (0)      439 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/country.py
--rw-r--r--   0 root         (0) root         (0)      371 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/wishlist_line.py
--rw-r--r--   0 root         (0) root         (0)     1102 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/credit_card.py
--rw-r--r--   0 root         (0) root         (0)     2877 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/product.py
--rw-r--r--   0 root         (0) root         (0)     2494 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/account.py
--rw-r--r--   0 root         (0) root         (0)     2146 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/graphic.py
--rw-r--r--   0 root         (0) root         (0)      105 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/state.py
--rw-r--r--   0 root         (0) root         (0)      333 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/payment_method.py
--rw-r--r--   0 root         (0) root         (0)      110 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/section.py
--rw-r--r--   0 root         (0) root         (0)      343 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/wishlist.py
--rw-r--r--   0 root         (0) root         (0)      113 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/collection.py
--rw-r--r--   0 root         (0) root         (0)      106 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/_return.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 11:52:18.000000 eadapters-0.4.1/src/eadapters/models/budy/
--rw-r--r--   0 root         (0) root         (0)     4144 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_common.py
--rw-r--r--   0 root         (0) root         (0)      269 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_voucher.py
--rw-r--r--   0 root         (0) root         (0)      681 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_country.py
--rw-r--r--   0 root         (0) root         (0)      195 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_shipping_option.py
--rw-r--r--   0 root         (0) root         (0)      499 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_subscription.py
--rw-r--r--   0 root         (0) root         (0)      548 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_address.py
--rw-r--r--   0 root         (0) root         (0)      169 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_category.py
--rw-r--r--   0 root         (0) root         (0)      275 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_referral.py
--rw-r--r--   0 root         (0) root         (0)     1039 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_bag_line.py
--rw-r--r--   0 root         (0) root         (0)     1053 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_order_line.py
--rw-r--r--   0 root         (0) root         (0)     3642 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_order.py
--rw-r--r--   0 root         (0) root         (0)      177 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_collection.py
--rw-r--r--   0 root         (0) root         (0)      169 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_wishlist.py
--rw-r--r--   0 root         (0) root         (0)      163 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_return.py
--rw-r--r--   0 root         (0) root         (0)      165 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_payment.py
--rw-r--r--   0 root         (0) root         (0)      157 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_brand.py
--rw-r--r--   0 root         (0) root         (0)      157 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_group.py
--rw-r--r--   0 root         (0) root         (0)      161 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_credit.py
--rw-r--r--   0 root         (0) root         (0)      154 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_card_payment_method.py
--rw-r--r--   0 root         (0) root         (0)     2096 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_bag.py
--rw-r--r--   0 root         (0) root         (0)      169 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_merchant.py
--rw-r--r--   0 root         (0) root         (0)      161 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_season.py
--rw-r--r--   0 root         (0) root         (0)      165 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_section.py
--rw-r--r--   0 root         (0) root         (0)      187 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_wishlist_line.py
--rw-r--r--   0 root         (0) root         (0)      191 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_payment_method.py
--rw-r--r--   0 root         (0) root         (0)      157 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_state.py
--rw-r--r--   0 root         (0) root         (0)     1392 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_product.py
--rw-r--r--   0 root         (0) root         (0)      153 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_city.py
--rw-r--r--   0 root         (0) root         (0)      157 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_color.py
--rw-r--r--   0 root         (0) root         (0)     1955 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4335 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/budy/bd_account.py
--rw-r--r--   0 root         (0) root         (0)      348 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/card_payment_method.py
--rw-r--r--   0 root         (0) root         (0)      435 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/bag.py
--rw-r--r--   0 root         (0) root         (0)      104 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/city.py
--rw-r--r--   0 root         (0) root         (0)     1525 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/address.py
--rw-r--r--   0 root         (0) root         (0)      149 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/subscription.py
--rw-r--r--   0 root         (0) root         (0)     1936 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9879 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/base.py
--rw-r--r--   0 root         (0) root         (0)      229 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18967 2022-06-25 11:52:12.000000 eadapters-0.4.1/src/eadapters/budy_a.py
--rw-r--r--   0 root         (0) root         (0)      905 2022-06-25 11:52:12.000000 eadapters-0.4.1/README.md
--rw-r--r--   0 root         (0) root         (0)       67 2022-06-25 11:52:18.000000 eadapters-0.4.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:25:26.000000 eadapters-0.4.2/
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-03 19:25:26.000000 eadapters-0.4.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:25:26.000000 eadapters-0.4.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:25:26.000000 eadapters-0.4.2/src/eadapters.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-03 19:25:26.000000 eadapters-0.4.2/src/eadapters.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-03 19:25:26.000000 eadapters-0.4.2/src/eadapters.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     2800 2023-05-03 19:25:26.000000 eadapters-0.4.2/src/eadapters.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1032 2023-05-03 19:25:26.000000 eadapters-0.4.2/src/eadapters.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 19:25:26.000000 eadapters-0.4.2/src/eadapters.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 19:25:21.000000 eadapters-0.4.2/src/eadapters.egg-info/not-zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:25:26.000000 eadapters-0.4.2/src/eadapters/
+-rw-r--r--   0 root         (0) root         (0)    10178 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/base.py
+-rw-r--r--   0 root         (0) root         (0)    19541 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/budy_a.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:25:26.000000 eadapters-0.4.2/src/eadapters/models/
+-rw-r--r--   0 root         (0) root         (0)     1525 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/address.py
+-rw-r--r--   0 root         (0) root         (0)      108 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/color.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:25:26.000000 eadapters-0.4.2/src/eadapters/models/budy/
+-rw-r--r--   0 root         (0) root         (0)      548 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_address.py
+-rw-r--r--   0 root         (0) root         (0)      499 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_subscription.py
+-rw-r--r--   0 root         (0) root         (0)      157 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_brand.py
+-rw-r--r--   0 root         (0) root         (0)      161 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_season.py
+-rw-r--r--   0 root         (0) root         (0)      269 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_voucher.py
+-rw-r--r--   0 root         (0) root         (0)      169 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_category.py
+-rw-r--r--   0 root         (0) root         (0)      153 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_city.py
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_shipping_option.py
+-rw-r--r--   0 root         (0) root         (0)     1392 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_product.py
+-rw-r--r--   0 root         (0) root         (0)      169 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_wishlist.py
+-rw-r--r--   0 root         (0) root         (0)      191 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_payment_method.py
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_bag_line.py
+-rw-r--r--   0 root         (0) root         (0)      621 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_store.py
+-rw-r--r--   0 root         (0) root         (0)      165 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_payment.py
+-rw-r--r--   0 root         (0) root         (0)      177 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_collection.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_order_line.py
+-rw-r--r--   0 root         (0) root         (0)      163 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_return.py
+-rw-r--r--   0 root         (0) root         (0)     4144 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_common.py
+-rw-r--r--   0 root         (0) root         (0)     4335 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_account.py
+-rw-r--r--   0 root         (0) root         (0)      157 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_color.py
+-rw-r--r--   0 root         (0) root         (0)      169 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_merchant.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_country.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      165 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_section.py
+-rw-r--r--   0 root         (0) root         (0)      275 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_referral.py
+-rw-r--r--   0 root         (0) root         (0)      157 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_state.py
+-rw-r--r--   0 root         (0) root         (0)     2096 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_bag.py
+-rw-r--r--   0 root         (0) root         (0)      154 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_card_payment_method.py
+-rw-r--r--   0 root         (0) root         (0)      187 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_wishlist_line.py
+-rw-r--r--   0 root         (0) root         (0)     3791 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_order.py
+-rw-r--r--   0 root         (0) root         (0)      157 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_group.py
+-rw-r--r--   0 root         (0) root         (0)      161 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_credit.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/base.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/graphic.py
+-rw-r--r--   0 root         (0) root         (0)      348 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/card_payment_method.py
+-rw-r--r--   0 root         (0) root         (0)      371 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/wishlist_line.py
+-rw-r--r--   0 root         (0) root         (0)      109 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/season.py
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/voucher.py
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/bag_line.py
+-rw-r--r--   0 root         (0) root         (0)      296 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/group.py
+-rw-r--r--   0 root         (0) root         (0)      274 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/store.py
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/order.py
+-rw-r--r--   0 root         (0) root         (0)      439 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/country.py
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/category.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/currency.py
+-rw-r--r--   0 root         (0) root         (0)      144 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/merchant.py
+-rw-r--r--   0 root         (0) root         (0)      113 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/collection.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/credit_card.py
+-rw-r--r--   0 root         (0) root         (0)      114 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/shipping_option.py
+-rw-r--r--   0 root         (0) root         (0)      106 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/credit.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/account.py
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/payment.py
+-rw-r--r--   0 root         (0) root         (0)     1984 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      106 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/_return.py
+-rw-r--r--   0 root         (0) root         (0)     2877 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/product.py
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/state.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/city.py
+-rw-r--r--   0 root         (0) root         (0)      333 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/payment_method.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/bag.py
+-rw-r--r--   0 root         (0) root         (0)      343 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/wishlist.py
+-rw-r--r--   0 root         (0) root         (0)      110 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/section.py
+-rw-r--r--   0 root         (0) root         (0)      108 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/brand.py
+-rw-r--r--   0 root         (0) root         (0)     1173 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/order_line.py
+-rw-r--r--   0 root         (0) root         (0)      108 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/referral.py
+-rw-r--r--   0 root         (0) root         (0)      229 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2754 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/factory.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2023-05-03 19:25:18.000000 eadapters-0.4.2/setup.py
+-rw-r--r--   0 root         (0) root         (0)      905 2023-05-03 19:25:18.000000 eadapters-0.4.2/README.md
+-rw-r--r--   0 root         (0) root         (0)     1032 2023-05-03 19:25:26.000000 eadapters-0.4.2/PKG-INFO
```

### Comparing `eadapters-0.4.1/setup.py` & `eadapters-0.4.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 import os
 import setuptools
 
 setuptools.setup(
     name = "eadapters",
-    version = "0.4.1",
+    version = "0.4.2",
     author = "Hive Solutions Lda.",
     author_email = "development@hive.pt",
     description = "E-Commerce Adapters",
     license = "Apache License, Version 2.0",
     keywords = "e-commerce adapters logic",
     url = "http://eadapters.hive.pt",
     zip_safe = False,
@@ -19,15 +19,15 @@
         "eadapters.models",
         "eadapters.models.budy"
     ],
     package_dir = {
         "" : os.path.normpath("src")
     },
     install_requires = [
-        "budy_api"
+        "budy-api"
     ],
     classifiers = [
         "Development Status :: 5 - Production/Stable",
         "Topic :: Utilities",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
```

### Comparing `eadapters-0.4.1/PKG-INFO` & `eadapters-0.4.2/src/eadapters.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: eadapters
-Version: 0.4.1
+Version: 0.4.2
 Summary: E-Commerce Adapters
 Home-page: http://eadapters.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: UNKNOWN
 Keywords: e-commerce adapters logic
```

### Comparing `eadapters-0.4.1/src/eadapters.egg-info/PKG-INFO` & `eadapters-0.4.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: eadapters
-Version: 0.4.1
+Version: 0.4.2
 Summary: E-Commerce Adapters
 Home-page: http://eadapters.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: UNKNOWN
 Keywords: e-commerce adapters logic
```

### Comparing `eadapters-0.4.1/src/eadapters.egg-info/SOURCES.txt` & `eadapters-0.4.2/src/eadapters.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 src/eadapters/models/payment_method.py
 src/eadapters/models/product.py
 src/eadapters/models/referral.py
 src/eadapters/models/season.py
 src/eadapters/models/section.py
 src/eadapters/models/shipping_option.py
 src/eadapters/models/state.py
+src/eadapters/models/store.py
 src/eadapters/models/subscription.py
 src/eadapters/models/voucher.py
 src/eadapters/models/wishlist.py
 src/eadapters/models/wishlist_line.py
 src/eadapters/models/budy/__init__.py
 src/eadapters/models/budy/bd_account.py
 src/eadapters/models/budy/bd_address.py
@@ -68,11 +69,12 @@
 src/eadapters/models/budy/bd_product.py
 src/eadapters/models/budy/bd_referral.py
 src/eadapters/models/budy/bd_return.py
 src/eadapters/models/budy/bd_season.py
 src/eadapters/models/budy/bd_section.py
 src/eadapters/models/budy/bd_shipping_option.py
 src/eadapters/models/budy/bd_state.py
+src/eadapters/models/budy/bd_store.py
 src/eadapters/models/budy/bd_subscription.py
 src/eadapters/models/budy/bd_voucher.py
 src/eadapters/models/budy/bd_wishlist.py
 src/eadapters/models/budy/bd_wishlist_line.py
```

### Comparing `eadapters-0.4.1/src/eadapters/factory.py` & `eadapters-0.4.2/src/eadapters/factory.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.1/src/eadapters/models/order_line.py` & `eadapters-0.4.2/src/eadapters/models/order_line.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.1/src/eadapters/models/base.py` & `eadapters-0.4.2/src/eadapters/models/base.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.1/src/eadapters/models/order.py` & `eadapters-0.4.2/src/eadapters/models/order.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.1/src/eadapters/models/bag_line.py` & `eadapters-0.4.2/src/eadapters/models/bag_line.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.1/src/eadapters/models/credit_card.py` & `eadapters-0.4.2/src/eadapters/models/credit_card.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.1/src/eadapters/models/product.py` & `eadapters-0.4.2/src/eadapters/models/product.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.1/src/eadapters/models/account.py` & `eadapters-0.4.2/src/eadapters/models/account.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.1/src/eadapters/models/graphic.py` & `eadapters-0.4.2/src/eadapters/models/graphic.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.1/src/eadapters/models/budy/bd_common.py` & `eadapters-0.4.2/src/eadapters/models/budy/bd_common.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.1/src/eadapters/models/budy/bd_country.py` & `eadapters-0.4.2/src/eadapters/models/budy/bd_country.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.1/src/eadapters/models/budy/bd_address.py` & `eadapters-0.4.2/src/eadapters/models/budy/bd_address.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.1/src/eadapters/models/budy/bd_bag_line.py` & `eadapters-0.4.2/src/eadapters/models/budy/bd_bag_line.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.1/src/eadapters/models/budy/bd_order_line.py` & `eadapters-0.4.2/src/eadapters/models/budy/bd_order_line.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.1/src/eadapters/models/budy/bd_order.py` & `eadapters-0.4.2/src/eadapters/models/budy/bd_order.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,19 @@
     def _get(cls, id):
         api = cls._get_api_g()
         order = api.get_order(id)
         order = cls.wrap(order)
         return order
 
     @bd_common.handle_error
+    def set_store_s(self, store_id):
+        api = self._get_api()
+        api.set_store_order(self.key, store_id)
+
+    @bd_common.handle_error
     def set_shipping_address_s(self, address):
         api = self._get_api()
         api.set_shipping_address_order(self.key, address)
 
     @bd_common.handle_error
     def set_billing_address_s(self, address):
         api = self._get_api()
```

### Comparing `eadapters-0.4.1/src/eadapters/models/budy/bd_bag.py` & `eadapters-0.4.2/src/eadapters/models/budy/bd_bag.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.1/src/eadapters/models/budy/bd_product.py` & `eadapters-0.4.2/src/eadapters/models/budy/bd_product.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.1/src/eadapters/models/budy/__init__.py` & `eadapters-0.4.2/src/eadapters/models/budy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from . import bd_order_line
 from . import bd_payment_method
 from . import bd_payment
 from . import bd_product
 from . import bd_referral
 from . import bd_shipping_option
 from . import bd_state
+from . import bd_store
 from . import bd_subscription
 from . import bd_voucher
 from . import bd_account
 from . import bd_wishlist_line
 from . import bd_wishlist
 
 from .bd_address import BDAddress
@@ -53,12 +54,13 @@
 from .bd_order_line import BDOrderLine
 from .bd_payment import BDPayment
 from .bd_product import BDProduct
 from .bd_referral import BDReferral
 from .bd_payment_method import BDPaymentMethod
 from .bd_shipping_option import BDShippingOption
 from .bd_state import BDState
+from .bd_store import BDStore
 from .bd_subscription import BDSubscription
 from .bd_voucher import BDVoucher
 from .bd_account import BDAccount
 from .bd_wishlist_line import BDWishlistLine
 from .bd_wishlist import BDWishlist
```

### Comparing `eadapters-0.4.1/src/eadapters/models/budy/bd_account.py` & `eadapters-0.4.2/src/eadapters/models/budy/bd_account.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.1/src/eadapters/models/address.py` & `eadapters-0.4.2/src/eadapters/models/address.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.1/src/eadapters/models/__init__.py` & `eadapters-0.4.2/src/eadapters/models/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from . import payment
 from . import product
 from . import referral
 from . import season
 from . import section
 from . import shipping_option
 from . import state
+from . import store
 from . import subscription
 from . import voucher
 from . import wishlist_line
 from . import wishlist
 
 from .budy import *
 
@@ -62,11 +63,12 @@
 from .payment import EPayment
 from .product import EProduct
 from .referral import EReferral
 from .season import ESeason
 from .section import ESection
 from .shipping_option import EShippingOption
 from .state import EState
+from .store import EStore
 from .subscription import ESubscription
 from .voucher import EVoucher
 from .wishlist_line import EWishlistLine
 from .wishlist import EWishlist
```

### Comparing `eadapters-0.4.1/src/eadapters/base.py` & `eadapters-0.4.2/src/eadapters/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,20 @@
 
     def list_states(self, *args, **kwargs):
         raise appier.NotImplementedError()
 
     def list_cities(self, country_id, *args, **kwargs):
         raise appier.NotImplementedError()
 
+    def list_stores(self, *args, **kwargs):
+        raise appier.NotImplementedError()
+
+    def get_store(self, id, *args, **kwargs):
+        raise appier.NotImplementedError()
+
     def list_products(self, *args, **kwargs):
         raise appier.NotImplementedError()
 
     def get_product(self, id, *args, **kwargs):
         raise appier.NotImplementedError()
 
     def search_products(self, *args, **kwargs):
@@ -204,14 +210,17 @@
 
     def end_pay_order(self, id, payment_data, *args, **kwargs):
         raise appier.NotImplementedError()
 
     def cancel_order(self, id, cancel_data, *args, **kwargs):
         raise appier.NotImplementedError()
 
+    def set_store_order(self, store_id, order_id, *args, **kwargs):
+        raise appier.NotImplementedError()
+
     def set_shipping_address_order(self, address_id, order_id, account_id = None, *args, **kwargs):
         raise appier.NotImplementedError()
 
     def set_billing_address_order(self, address_id, order_id, account_id = None, *args, **kwargs):
         raise appier.NotImplementedError()
 
     def set_store_shipping_order(self, order_id, *args, **kwargs):
```

### Comparing `eadapters-0.4.1/src/eadapters/budy_a.py` & `eadapters-0.4.2/src/eadapters/budy_a.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,27 @@
             currency = currency.currency_code,
             locale = locale
         )
 
     def list_countries(self, *args, **kwargs):
         return models.BDCountry.list(*args, **kwargs)
 
+    def list_stores(self, *args, **kwargs):
+        api = self._get_api()
+        self._normalize(kwargs)
+        stores = api.list_stores(*args, **kwargs)
+        stores = models.BDStore.wrap(stores)
+        return stores
+
+    def get_store(self, id, *args, **kwargs):
+        api = self._get_api()
+        store = api.get_store(id)
+        store = models.BDStore.wrap(store)
+        return store
+
     def list_products(self, *args, **kwargs):
         api = self._get_api()
         self._normalize(kwargs)
         products = api.list_products(*args, **kwargs)
         products = models.BDProduct.wrap(products)
         return products
 
@@ -369,14 +382,18 @@
         order = models.BDOrder.get_l(key = id)
         return order.end_pay_s(payment_data)
 
     def cancel_order(self, id, cancel_data, *args, **kwargs):
         order = models.BDOrder.get_l(key = id)
         return order.cancel_s(cancel_data)
 
+    def set_store_order(self, store_id, order_id, *args, **kwargs):
+        order = models.BDOrder.get_l(key = order_id)
+        order.set_store_s(store_id)
+
     def set_shipping_address_order(self, address_id, order_id, account_id = None, *args, **kwargs):
         account = models.BDAccount.me()
         address = account.get_address(address_id)
         order = models.BDOrder.get_l(key = order_id)
         address = address.unwrap(default = True)
         order.set_shipping_address_s(address)
```

### Comparing `eadapters-0.4.1/README.md` & `eadapters-0.4.2/README.md`

 * *Files identical despite different names*

