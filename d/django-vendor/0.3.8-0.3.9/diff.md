# Comparing `tmp/django-vendor-0.3.8.tar.gz` & `tmp/django-vendor-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-vendor-0.3.8.tar", last modified: Fri Dec  9 21:56:34 2022, max compression
+gzip compressed data, was "django-vendor-0.3.9.tar", last modified: Thu Jan 12 01:45:47 2023, max compression
```

## Comparing `django-vendor-0.3.8.tar` & `django-vendor-0.3.9.tar`

### file list

```diff
@@ -1,119 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 21:56:34.392497 django-vendor-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2022-12-09 21:56:34.392497 django-vendor-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2022-12-09 21:55:47.000000 django-vendor-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 21:56:34.380497 django-vendor-0.3.8/django_vendor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2022-12-09 21:56:34.000000 django-vendor-0.3.8/django_vendor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2022-12-09 21:56:34.000000 django-vendor-0.3.8/django_vendor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-09 21:56:34.000000 django-vendor-0.3.8/django_vendor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 2022-12-09 21:56:34.000000 django-vendor-0.3.8/django_vendor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-09 21:56:34.000000 django-vendor-0.3.8/django_vendor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-09 21:56:34.392497 django-vendor-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2022-12-09 21:55:47.000000 django-vendor-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 21:56:34.380497 django-vendor-0.3.8/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 21:56:34.380497 django-vendor-0.3.8/vendor/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 21:56:34.384497 django-vendor-0.3.8/vendor/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/api/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 21:56:34.384497 django-vendor-0.3.8/vendor/api/v1/authorizenet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/api/v1/authorizenet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11912 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/api/v1/authorizenet/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 21:56:34.384497 django-vendor-0.3.8/vendor/api/v1/stripe/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/api/v1/stripe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13379 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/api/v1/stripe/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 21:56:34.384497 django-vendor-0.3.8/vendor/encrypt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/encrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/encrypt/cleartext.py
--rw-r--r--   0 runner    (1001) docker     (123)    18489 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/integrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 21:56:34.388497 django-vendor-0.3.8/vendor/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    22899 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0002_auto_20200912_0142.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0003_auto_20200915_1839.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0004_offer_offer_description.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0005_auto_20200930_2037.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0006_auto_20201005_2257.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0007_offer_list_bundle_items.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0008_offer_allow_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0009_auto_20201111_0743.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0010_auto_20201112_0138.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0011_auto_20201120_1750.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0012_auto_20201123_1848.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0013_auto_20201202_1759.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0014_term_types_update_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0015_uuid_payments_receipts.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0016_auto_20201203_2011.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0017_auto_20201203_2107.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0018_add_uuid_address_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0019_fill_uuid_address_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0020_lock_uuid_address_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0021_auto_20210408_2303.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0022_offer_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0023_profile_null_false.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0024_offer_deleted.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0025_auto_20210914_0025.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0026_auto_20210914_1209.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0027_bugfix_vendor_notes_invoice_history.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0028_add_trial_date_term_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     8878 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0029_alter_customerprofile_currency_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0030_auto_20220414_1055.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0031_pre_invoice_status_change.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0032_alter_invoice_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0033_payment_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0034_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0035_add_subscription_relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0036_post_payment_status_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0037_auto_20220609_1644.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0038_auto_20220719_0944.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0039_customerprofile_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/0040_auto_20221020_1617.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 21:56:34.388497 django-vendor-0.3.8/vendor/models/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/models/address.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11425 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/models/choice.py
--rw-r--r--   0 runner    (1001) docker     (123)    14688 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/models/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/models/modelmanagers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10336 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/models/offer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/models/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/models/price.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/models/product.py
--rw-r--r--   0 runner    (1001) docker     (123)    10020 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/models/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/models/receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/models/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/models/tax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/models/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/models/wishlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 21:56:34.388497 django-vendor-0.3.8/vendor/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52310 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/processors/authorizenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    20302 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/processors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/processors/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)    47194 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/processors/stripe_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 21:56:34.388497 django-vendor-0.3.8/vendor/signals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/signals/stripe_signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 21:56:34.392497 django-vendor-0.3.8/vendor/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    30579 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42645 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/tests/test_authorizenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    13322 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/tests/test_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    41664 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/tests/test_stripe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 21:56:34.392497 django-vendor-0.3.8/vendor/urls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/urls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/urls/vendor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/urls/vendor_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 21:56:34.392497 django-vendor-0.3.8/vendor/views/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/views/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/views/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    14989 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/views/vendor.py
--rw-r--r--   0 runner    (1001) docker     (123)    22416 2022-12-09 21:55:47.000000 django-vendor-0.3.8/vendor/views/vendor_admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.291328 django-vendor-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-01-12 01:45:47.291328 django-vendor-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-01-12 01:44:51.000000 django-vendor-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.271326 django-vendor-0.3.9/django_vendor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-01-12 01:45:47.000000 django-vendor-0.3.9/django_vendor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-01-12 01:45:47.000000 django-vendor-0.3.9/django_vendor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 01:45:47.000000 django-vendor-0.3.9/django_vendor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-01-12 01:45:47.000000 django-vendor-0.3.9/django_vendor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-12 01:45:47.000000 django-vendor-0.3.9/django_vendor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 01:45:47.291328 django-vendor-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-01-12 01:44:51.000000 django-vendor-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.271326 django-vendor-0.3.9/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.271326 django-vendor-0.3.9/vendor/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.271326 django-vendor-0.3.9/vendor/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/api/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.271326 django-vendor-0.3.9/vendor/api/v1/authorizenet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/api/v1/authorizenet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/api/v1/authorizenet/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.275327 django-vendor-0.3.9/vendor/api/v1/stripe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/api/v1/stripe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13379 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/api/v1/stripe/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.275327 django-vendor-0.3.9/vendor/encrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/encrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/encrypt/cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18432 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/integrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.283327 django-vendor-0.3.9/vendor/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0002_auto_20200912_0142.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0003_auto_20200915_1839.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0004_offer_offer_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0005_auto_20200930_2037.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0006_auto_20201005_2257.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0007_offer_list_bundle_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0008_offer_allow_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0009_auto_20201111_0743.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0010_auto_20201112_0138.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0011_auto_20201120_1750.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0012_auto_20201123_1848.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0013_auto_20201202_1759.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0014_term_types_update_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0015_uuid_payments_receipts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0016_auto_20201203_2011.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0017_auto_20201203_2107.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0018_add_uuid_address_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0019_fill_uuid_address_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0020_lock_uuid_address_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0021_auto_20210408_2303.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0022_offer_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0023_profile_null_false.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0024_offer_deleted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0025_auto_20210914_0025.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0026_auto_20210914_1209.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0027_bugfix_vendor_notes_invoice_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0028_add_trial_date_term_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0029_alter_customerprofile_currency_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0030_auto_20220414_1055.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0031_pre_invoice_status_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0032_alter_invoice_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0033_payment_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0034_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0035_add_subscription_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0036_post_payment_status_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0037_auto_20220609_1644.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0038_auto_20220719_0944.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0039_customerprofile_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0040_auto_20221020_1617.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.287328 django-vendor-0.3.9/vendor/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/modelmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10336 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/wishlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.287328 django-vendor-0.3.9/vendor/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52310 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/processors/authorizenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20302 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/processors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/processors/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48404 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/processors/stripe_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.287328 django-vendor-0.3.9/vendor/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/signals/stripe_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.287328 django-vendor-0.3.9/vendor/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    30579 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42645 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/tests/test_authorizenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13322 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/tests/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41664 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/tests/test_stripe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.291328 django-vendor-0.3.9/vendor/urls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/urls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/urls/vendor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/urls/vendor_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.291328 django-vendor-0.3.9/vendor/views/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/views/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/views/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/views/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/views/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14989 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/views/vendor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18171 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/views/vendor_admin.py
```

### Comparing `django-vendor-0.3.8/PKG-INFO` & `django-vendor-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vendor
-Version: 0.3.8
+Version: 0.3.9
 Summary: Django App Toolkit for selling digital and physical goods online.
 Home-page: https://github.com/renderbox/django-vendor/
 Author: Grant Viklund, Roberto Himmelbauer
 Author-email: renderbox@gmail.com
 License: MIT license
 Keywords: django,app
 Platform: UNKNOWN
```

### Comparing `django-vendor-0.3.8/README.md` & `django-vendor-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/django_vendor.egg-info/PKG-INFO` & `django-vendor-0.3.9/django_vendor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vendor
-Version: 0.3.8
+Version: 0.3.9
 Summary: Django App Toolkit for selling digital and physical goods online.
 Home-page: https://github.com/renderbox/django-vendor/
 Author: Grant Viklund, Roberto Himmelbauer
 Author-email: renderbox@gmail.com
 License: MIT license
 Keywords: django,app
 Platform: UNKNOWN
```

### Comparing `django-vendor-0.3.8/django_vendor.egg-info/SOURCES.txt` & `django-vendor-0.3.9/django_vendor.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -92,11 +92,13 @@
 vendor/tests/test_authorizenet.py
 vendor/tests/test_processor.py
 vendor/tests/test_stripe.py
 vendor/urls/__init__.py
 vendor/urls/vendor.py
 vendor/urls/vendor_admin.py
 vendor/views/__init__.py
+vendor/views/config.py
+vendor/views/integration.py
 vendor/views/mixin.py
 vendor/views/report.py
 vendor/views/vendor.py
 vendor/views/vendor_admin.py
```

### Comparing `django-vendor-0.3.8/setup.py` & `django-vendor-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/admin.py` & `django-vendor-0.3.9/vendor/admin.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/api/v1/authorizenet/views.py` & `django-vendor-0.3.9/vendor/api/v1/authorizenet/views.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/api/v1/stripe/views.py` & `django-vendor-0.3.9/vendor/api/v1/stripe/views.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/api/v1/urls.py` & `django-vendor-0.3.9/vendor/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/api/v1/views.py` & `django-vendor-0.3.9/vendor/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/apps.py` & `django-vendor-0.3.9/vendor/apps.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/config.py` & `django-vendor-0.3.9/vendor/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,33 @@
 # App Settings
 from django.conf import settings
 from django import forms
 from django.db.models import TextChoices
 from django.contrib.sites.models import Site
-from django.core.exceptions import ObjectDoesNotExist
 from django.utils.translation import gettext_lazy as _
 
 from siteconfigs.config import SiteConfigBaseClass
-from siteconfigs.models import SiteConfigModel
 
-from vendor.utils import get_site_from_request
+
+class SiteSelectForm(forms.Form):
+    site = forms.ModelChoiceField(queryset=Site.objects.all())
 
 
 class SupportedPaymentProcessor(TextChoices):
     PROMO_CODE_BASE = ("base.PaymentProcessorBase", _("Default Processor"))
     AUTHORIZE_NET = ("authorizenet.AuthorizeNetProcessor", _("Authorize.Net"))
     STRIPE = ("stripe_processor.StripeProcessor", _("Stripe"))
 
 
-class PaymentProcessorForm(forms.Form):
+class PaymentProcessorForm(SiteSelectForm):
     payment_processor = forms.CharField(label=_("Payment Processor"), widget=forms.Select(choices=SupportedPaymentProcessor.choices))
 
 
-class PaymentProcessorSiteSelectForm(PaymentProcessorForm):
-    site = forms.CharField(label=_("Site"))
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        self.fields['site'].widget = forms.Select(choices=[(site.pk, site.domain) for site in Site.objects.all()])
-
-
 class PaymentProcessorSiteConfig(SiteConfigBaseClass):
-    label = _("Promo Code Processor")
+    label = _("Payment Processor")
     default = {"payment_processor": "base.PaymentProcessorBase"}
     form_class = PaymentProcessorForm
     key = ""
     instance = None
 
     def __init__(self, site=None):
         
@@ -49,45 +40,78 @@
         if not self.instance:
             self.default['payment_processor'] = VENDOR_PAYMENT_PROCESSOR
 
     def get_form(self):
         return self.form_class(initial=self.get_initials())
 
     def get_initials(self):
+        initial = super().get_initials()
+        initial['site'] = (self.site.pk, self.site.domain)
+        
         if self.instance:
-            return {'payment_processor': [choice for choice in SupportedPaymentProcessor.choices if choice[0] == self.instance.value['payment_processor']][0]}
-
-        return {'payment_processor': SupportedPaymentProcessor.choices[0]}
+            initial['payment_processor'] = [choice for choice in SupportedPaymentProcessor.choices if choice[0] == self.instance.value['payment_processor']][0]
+        else:
+            initial['payment_processor'] = SupportedPaymentProcessor.choices[0]
+        
+        return initial
 
     def get_selected_processor(self):
         if self.instance:
             return [choice for choice in SupportedPaymentProcessor.choices if choice[0] == self.instance.value['payment_processor']][0]
 
         return SupportedPaymentProcessor.choices[0]  # Return Default Processors
 
 
-class PaymentProcessorSiteSelectSiteConfig(PaymentProcessorSiteConfig):
-    label = _("Promo Code Processor")
-    default = {"payment_processor": "base.PromoProcessorBase"}
-    form_class = PaymentProcessorSiteSelectForm
-    key = ""
+class StripeConnectAccountForm(SiteSelectForm):
+    account_number = forms.CharField(max_length=120)
+
+
+class StripeConnectAccountConfig(SiteConfigBaseClass):
+    label = _("Stripe Connect Account")
+    default = {'stripe_connect_account': None}
+    form_class = StripeConnectAccountForm
+    key = ''
     instance = None
 
-    def get_initials(self):
-        initial = super().get_initials()
-        initial['site'] = (self.site.pk, self.site.domain)
+    def __init__(self, site=None):
+        
+        if site is None:
+            site = Site.objects.get_current()
+
+        self.key = ".".join([__name__, __class__.__name__])
+        super().__init__(site, self.key)
         
-        return initial
+
+class VendorSiteCommissionForm(SiteSelectForm):
+    commission = forms.IntegerField(min_value=0, max_value=100)
+
+
+class VendorSiteCommissionConfig(SiteConfigBaseClass):
+    label = _("Vendor Site Commission")
+    default = {'commission': None}
+    form_class = VendorSiteCommissionForm
+    key = ''
+    instance = None
+
+    def __init__(self, site=None):
+        
+        if site is None:
+            site = Site.objects.get_current()
+
+        self.key = ".".join([__name__, __class__.__name__])
+        super().__init__(site, self.key)
 
 
 VENDOR_PRODUCT_MODEL = getattr(settings, "VENDOR_PRODUCT_MODEL", "vendor.Product")
 
 VENDOR_PAYMENT_PROCESSOR = getattr(settings, "VENDOR_PAYMENT_PROCESSOR", "dummy.DummyProcessor")
 
 DEFAULT_CURRENCY = getattr(settings, "DEFAULT_CURRENCY", "usd")
 
 AVAILABLE_CURRENCIES = getattr(settings, "AVAILABLE_CURRENCIES", {'usd': _('USD Dollars')})
 
 VENDOR_STATE = getattr(settings, "VENDOR_STATE", "DEBUG")
 
 # Encryption settings
 VENDOR_DATA_ENCODER = getattr(settings, "VENDOR_DATA_ENCODER", "vendor.encrypt.cleartext")
+
+
```

### Comparing `django-vendor-0.3.8/vendor/forms.py` & `django-vendor-0.3.9/vendor/forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from vendor.config import VENDOR_PRODUCT_MODEL
 from vendor.models import Address, Offer, Price, offer_term_details_default, CustomerProfile, Payment, Subscription
 from vendor.models.choice import PaymentTypes, TermType, Country, USAStateChoices, SubscriptionStatus
 from vendor.utils import get_site_from_request
 
 
+from vendor.config import SiteSelectForm
 Product = apps.get_model(VENDOR_PRODUCT_MODEL)
 
 COUNTRY_CHOICE = getattr(settings, 'VENDOR_COUNTRY_CHOICE', Country)
 COUNTRY_DEFAULT = getattr(settings, 'VENDOR_COUNTRY_DEFAULT', Country.US)
 
 
 def get_available_country_choices():
@@ -388,17 +389,14 @@
         if end_date and end_date < start_date:
             self.add_error('end_date', _('End Date cannot be before Start Date'))
             del(cleaned_data['end_date'])
 
         return cleaned_data
 
 
-class SiteSelectForm(forms.Form):
-    site = forms.ModelChoiceField(queryset=Site.objects.all())
-
 class OfferSiteSelectForm(SiteSelectForm):
     offer = forms.ModelChoiceField(queryset=None, required=False)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         if 'site' in self.initial or 'site' in self.data:
```

### Comparing `django-vendor-0.3.8/vendor/integrations.py` & `django-vendor-0.3.9/vendor/integrations.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0001_initial.py` & `django-vendor-0.3.9/vendor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0003_auto_20200915_1839.py` & `django-vendor-0.3.9/vendor/migrations/0003_auto_20200915_1839.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0005_auto_20200930_2037.py` & `django-vendor-0.3.9/vendor/migrations/0005_auto_20200930_2037.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0006_auto_20201005_2257.py` & `django-vendor-0.3.9/vendor/migrations/0006_auto_20201005_2257.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0008_offer_allow_multiple.py` & `django-vendor-0.3.9/vendor/migrations/0008_offer_allow_multiple.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0009_auto_20201111_0743.py` & `django-vendor-0.3.9/vendor/migrations/0009_auto_20201111_0743.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0010_auto_20201112_0138.py` & `django-vendor-0.3.9/vendor/migrations/0010_auto_20201112_0138.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0011_auto_20201120_1750.py` & `django-vendor-0.3.9/vendor/migrations/0011_auto_20201120_1750.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0012_auto_20201123_1848.py` & `django-vendor-0.3.9/vendor/migrations/0012_auto_20201123_1848.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0013_auto_20201202_1759.py` & `django-vendor-0.3.9/vendor/migrations/0013_auto_20201202_1759.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0014_term_types_update_value.py` & `django-vendor-0.3.9/vendor/migrations/0014_term_types_update_value.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0015_uuid_payments_receipts.py` & `django-vendor-0.3.9/vendor/migrations/0015_uuid_payments_receipts.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0016_auto_20201203_2011.py` & `django-vendor-0.3.9/vendor/migrations/0016_auto_20201203_2011.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0017_auto_20201203_2107.py` & `django-vendor-0.3.9/vendor/migrations/0017_auto_20201203_2107.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0018_add_uuid_address_profile.py` & `django-vendor-0.3.9/vendor/migrations/0018_add_uuid_address_profile.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0019_fill_uuid_address_profile.py` & `django-vendor-0.3.9/vendor/migrations/0019_fill_uuid_address_profile.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0020_lock_uuid_address_profile.py` & `django-vendor-0.3.9/vendor/migrations/0020_lock_uuid_address_profile.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0021_auto_20210408_2303.py` & `django-vendor-0.3.9/vendor/migrations/0021_auto_20210408_2303.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0023_profile_null_false.py` & `django-vendor-0.3.9/vendor/migrations/0023_profile_null_false.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0025_auto_20210914_0025.py` & `django-vendor-0.3.9/vendor/migrations/0025_auto_20210914_0025.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0026_auto_20210914_1209.py` & `django-vendor-0.3.9/vendor/migrations/0026_auto_20210914_1209.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0027_bugfix_vendor_notes_invoice_history.py` & `django-vendor-0.3.9/vendor/migrations/0027_bugfix_vendor_notes_invoice_history.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0028_add_trial_date_term_details.py` & `django-vendor-0.3.9/vendor/migrations/0028_add_trial_date_term_details.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0029_alter_customerprofile_currency_and_more.py` & `django-vendor-0.3.9/vendor/migrations/0029_alter_customerprofile_currency_and_more.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0030_auto_20220414_1055.py` & `django-vendor-0.3.9/vendor/migrations/0030_auto_20220414_1055.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0031_pre_invoice_status_change.py` & `django-vendor-0.3.9/vendor/migrations/0031_pre_invoice_status_change.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0033_payment_status.py` & `django-vendor-0.3.9/vendor/migrations/0033_payment_status.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0034_subscription.py` & `django-vendor-0.3.9/vendor/migrations/0034_subscription.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0035_add_subscription_relation.py` & `django-vendor-0.3.9/vendor/migrations/0035_add_subscription_relation.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0036_post_payment_status_change.py` & `django-vendor-0.3.9/vendor/migrations/0036_post_payment_status_change.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0037_auto_20220609_1644.py` & `django-vendor-0.3.9/vendor/migrations/0037_auto_20220609_1644.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0038_auto_20220719_0944.py` & `django-vendor-0.3.9/vendor/migrations/0038_auto_20220719_0944.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/migrations/0040_auto_20221020_1617.py` & `django-vendor-0.3.9/vendor/migrations/0040_auto_20221020_1617.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/models/__init__.py` & `django-vendor-0.3.9/vendor/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/models/address.py` & `django-vendor-0.3.9/vendor/models/address.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/models/base.py` & `django-vendor-0.3.9/vendor/models/base.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/models/choice.py` & `django-vendor-0.3.9/vendor/models/choice.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/models/invoice.py` & `django-vendor-0.3.9/vendor/models/invoice.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/models/modelmanagers.py` & `django-vendor-0.3.9/vendor/models/modelmanagers.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/models/offer.py` & `django-vendor-0.3.9/vendor/models/offer.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/models/payment.py` & `django-vendor-0.3.9/vendor/models/payment.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/models/price.py` & `django-vendor-0.3.9/vendor/models/price.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/models/profile.py` & `django-vendor-0.3.9/vendor/models/profile.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/models/receipt.py` & `django-vendor-0.3.9/vendor/models/receipt.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/models/subscription.py` & `django-vendor-0.3.9/vendor/models/subscription.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/models/tax.py` & `django-vendor-0.3.9/vendor/models/tax.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/models/utils.py` & `django-vendor-0.3.9/vendor/models/utils.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/models/validator.py` & `django-vendor-0.3.9/vendor/models/validator.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/models/wishlist.py` & `django-vendor-0.3.9/vendor/models/wishlist.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/processors/__init__.py` & `django-vendor-0.3.9/vendor/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/processors/authorizenet.py` & `django-vendor-0.3.9/vendor/processors/authorizenet.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/processors/base.py` & `django-vendor-0.3.9/vendor/processors/base.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/processors/stripe_processor.py` & `django-vendor-0.3.9/vendor/processors/stripe_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 """
 Payment processor for Stripe.
 """
-import django.dispatch
 import json
 import logging
 import stripe
-import uuid
 
 from math import modf
 from django.conf import settings
-from django.contrib.sites.models import Site
 from django.utils import timezone
-from vendor.config import DEFAULT_CURRENCY
+from vendor.config import DEFAULT_CURRENCY, StripeConnectAccountConfig, VendorSiteCommissionConfig
 from vendor.integrations import StripeIntegration
 from vendor.models import Offer, CustomerProfile
 from vendor.models.choice import (
     Country,
-    SubscriptionStatus,
-    TransactionTypes,
-    PaymentTypes,
     TermType,
     TermDetailUnits,
-    InvoiceStatus,
-    PurchaseStatus
 )
 from vendor.processors.base import PaymentProcessorBase
 
 
 logger = logging.getLogger(__name__)
 
 class StripeQueryBuilder:
@@ -316,18 +308,41 @@
         if len(fraction_str) < 2:
             fraction_str = "0" + fraction_str
 
         stripe_amount = int("".join([whole_str, fraction_str]))
             
         return stripe_amount
 
+    def get_stripe_connect_account(self):
+        stripe_connect = StripeConnectAccountConfig(self.site)
+
+        if stripe_connect.instance:
+            return stripe_connect.get_key_value('stripe_connect_account')
+
+        return None
+
+    def get_application_fee_percent(self):
+        vendor_site_commission = VendorSiteCommissionConfig(self.site)
+
+        if vendor_site_commission.instance:
+            return vendor_site_commission.get_key_value('commission')
+
+        return None
+
+    def get_application_fee_amount(self):
+        vendor_site_commission = VendorSiteCommissionConfig(self.site)
+
+        if vendor_site_commission.instance:
+            return self.convert_decimal_to_integer((vendor_site_commission.get_key_value('commission')*self.invoice.total)/100)
+
+        return None
+
     ##########
     # CRUD Stripe Object
     ##########
-
     def stripe_create_object(self, stripe_object_class, object_data):
         stripe_object = self.stripe_call(stripe_object_class.create, object_data)
 
         return stripe_object
 
     def stripe_query_object(self, stripe_object_class, query, limit=100, page=None):
         if isinstance(query, dict):
@@ -418,14 +433,21 @@
             else:
                 break
 
         return object_list
         
     # Stripe Object Builders
     ##########
+    def build_transfer_data(self):
+        return {
+            'destination': self.get_stripe_connect_account(),
+            # Not required if you are using the application_fee parameter
+            # 'amount_percent': 100 - self.get_application_fee_percent()
+        }
+
     def build_customer(self, customer_profile):
         return {
             'name': f"{customer_profile.user.first_name} {customer_profile.user.last_name}",
             'email': customer_profile.user.email,
             'metadata': {'site': customer_profile.site}
         }
     
@@ -504,15 +526,17 @@
                 'email': self.invoice.profile.user.email
             }
         }
 
     def build_payment_intent(self, amount, currency=DEFAULT_CURRENCY):
         return {
             'amount': amount,
-            'currency': currency
+            'currency': currency,
+            'application_fee_percent': self.get_application_fee_amount(),
+            'transfer_data': self.get_stripe_connect_account()
         }
 
     def build_setup_intent(self, payment_method_id):
         return {
             'customer': self.invoice.profile.meta['stripe_id'],
             'confirm': True,
             'payment_method_types': ['card'],
@@ -523,16 +547,17 @@
     def build_subscription(self, subscription, payment_method_id):
         return {
             'customer': self.invoice.profile.meta['stripe_id'],
             'coupon': subscription.offer.meta['stripe'].get('coupon_id'),
             'items': [{'price': subscription.offer.meta['stripe']['price_id']}],
             'default_payment_method': payment_method_id,
             'metadata': {'site': self.invoice.site},
-            'trial_period_days': subscription.offer.get_trial_days()
-
+            'trial_period_days': subscription.offer.get_trial_days(),
+            'application_fee_percent': self.get_application_fee_percent(),
+            'transfer_data': self.build_transfer_data()
         }
 
     def build_invoice_line_item(self, order_item, invoice_id):
         line_item = {
             'customer': self.invoice.profile.meta.get('stripe_id'),
             'invoice': invoice_id,
             'price': order_item.offer.meta['stripe'].get('price_id'),
@@ -548,15 +573,14 @@
             'customer': self.invoice.profile.meta.get('stripe_id'),
             'currency': currency,
         }
 
     ##########
     # Customers
     ##########
-
     def get_stripe_customers(self, site, expand=None):
         """
         Returns all Stripe created customers for this site
         """
 
         clause = self.query_builder.make_clause_template(
             field='metadata',
```

### Comparing `django-vendor-0.3.8/vendor/signals/stripe_signals.py` & `django-vendor-0.3.9/vendor/signals/stripe_signals.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/tests/__init__.py` & `django-vendor-0.3.9/vendor/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/tests/test_authorizenet.py` & `django-vendor-0.3.9/vendor/tests/test_authorizenet.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/tests/test_processor.py` & `django-vendor-0.3.9/vendor/tests/test_processor.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/tests/test_stripe.py` & `django-vendor-0.3.9/vendor/tests/test_stripe.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/urls/vendor.py` & `django-vendor-0.3.9/vendor/urls/vendor.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/urls/vendor_admin.py` & `django-vendor-0.3.9/vendor/urls/vendor_admin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from django.urls import path
 
 from vendor.views import vendor_admin as admin_views
+from vendor.views import config as config_views
+from vendor.views import integration as integrations_views
 from vendor.views import report as report_views
 
 app_name = "vendor_admin"
 
 urlpatterns = [
     path('', admin_views.AdminDashboardView.as_view(), name="manager-dashboard"),
     path('products/', admin_views.AdminProductListView.as_view(), name="manager-product-list"),
@@ -20,18 +22,29 @@
     path('subscription/<uuid:uuid_subscription>/add/payment/<uuid:uuid_profile>/', admin_views.AdminSubscriptionAddPaymentView.as_view(), name="manager-subscription-add-payment"),
     path('subscription/create/', admin_views.AdminSubscriptionCreateView.as_view(), name="manager-subscription-create"),
     path('profiles/', admin_views.AdminProfileListView.as_view(), name="manager-profiles"),
     path('profile/<uuid:uuid>', admin_views.AdminProfileDetailView.as_view(), name="manager-profile"),
     path('product/<uuid:uuid>/renew', admin_views.AdminManualSubscriptionRenewal.as_view(), name="manager-product-renew"),
     path('payments/no/receipt/', admin_views.PaymentWithNoReceiptListView.as_view(), name="manager-payment-no-receipt"),
     path('payments/no/orderitems/', admin_views.PaymentWithNoOrderItemsListView.as_view(), name="manager-payment-no-receipt"),
-    path("processors/", admin_views.PaymentProcessorSiteConfigsListView.as_view(), name="vendor-processor-lists"),
-    path("processor/site/", admin_views.PaymentProcessorSiteFormView.as_view(), name="vendor-site-processor"),
-    path("processor/new/site/", admin_views.PaymentProcessorSiteSelectFormView.as_view(), name="vendor-new-site-processor"),
-    path("processor/edit/<domain>/site/processors/", admin_views.PaymentProcessorSiteSelectFormView.as_view(), name="vendor-sites-processors"),
-    path("authorizenet/integration/", admin_views.AuthorizeNetIntegrationView.as_view(), name="authorizenet-integration"),
-    path("stripe/integration/", admin_views.StripeIntegrationView.as_view(), name="stripe-integration"),
 
-    # reports
+    # Reports
     path('reports/receipts/download/', report_views.ReceiptListCSV.as_view(), name="manager-receipt-download"),
     path('reports/invoices/download/', report_views.InvoiceListCSV.as_view(), name="manager-invoice-download"),
+
+    # Integrations
+    path("authorizenet/integration/", integrations_views.AuthorizeNetIntegrationView.as_view(), name="authorizenet-integration"),
+    path("stripe/integration/", integrations_views.StripeIntegrationView.as_view(), name="stripe-integration"),
+
+    # Configs
+    path('config/stripe/connect/list/', config_views.StripeConnectAccountConfigListView.as_view(), name="manager-config-stripe-connect-list"),
+    path('config/stripe/connect/create/', config_views.StripeConnectAccountCreateConfigView.as_view(), name="manager-config-stripe-connect-create"),
+    path('config/stripe/connect/update/<int:pk>/', config_views.StripeConnectAccountUpdateConfigView.as_view(), name="manager-config-stripe-connect-update"),
+    path('config/commission/list/', config_views.VendorSiteCommissionConfigListView.as_view(), name="manager-config-commission-list"),
+    path('config/commission/create/', config_views.VendorSiteCommissionCreateConfigView.as_view(), name="manager-config-commission-create"),
+    path('config/commission/update/<int:pk>/', config_views.VendorSiteCommissionUpdateConfigView.as_view(), name="manager-config-commission-update"),
+    # path('config/vendor/commission/', config_views.InvoiceListCSV.as_view(), name="manager-invoice-download"),
+    path("config/processor/list/", config_views.PaymentProcessorSiteConfigsListView.as_view(), name="manager-config-processor-list"),
+    path("config/processor/create/", config_views.PaymentProcessorCreateConfigView.as_view(), name="manager-config-processor-create"),
+    path("config/processor/update/<int:pk>", config_views.PaymentProcessorUpdateConfigView.as_view(), name="manager-config-processor-update"),
+    
 ]
```

### Comparing `django-vendor-0.3.8/vendor/utils.py` & `django-vendor-0.3.9/vendor/utils.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/views/__init__.py` & `django-vendor-0.3.9/vendor/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/views/mixin.py` & `django-vendor-0.3.9/vendor/views/mixin.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/views/report.py` & `django-vendor-0.3.9/vendor/views/report.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/views/vendor.py` & `django-vendor-0.3.9/vendor/views/vendor.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.8/vendor/views/vendor_admin.py` & `django-vendor-0.3.9/vendor/views/vendor_admin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 import logging
 
 from django.apps import apps
 from django.contrib import messages
 from django.contrib.auth.mixins import LoginRequiredMixin
-from django.contrib.sites.models import Site
 from django.db import IntegrityError, DatabaseError, transaction
 from django.db.models import Count, Q
-from django.shortcuts import redirect, render, get_object_or_404
-from django.urls import reverse, reverse_lazy
-from django.views.generic import View, TemplateView
+from django.shortcuts import redirect, render
+from django.urls import reverse_lazy
+from django.views.generic import TemplateView
 from django.views.generic.detail import DetailView
-from django.views.generic.edit import CreateView, UpdateView, FormView, ProcessFormView, FormMixin, ModelFormMixin
+from django.views.generic.edit import CreateView, UpdateView
 from django.views.generic.list import ListView
 from django.utils import timezone
 from django.utils.translation import gettext as _
 
-from vendor.config import VENDOR_PRODUCT_MODEL, PaymentProcessorSiteConfig,\
-    PaymentProcessorSiteSelectSiteConfig, PaymentProcessorForm, PaymentProcessorSiteSelectForm
+from vendor.config import VENDOR_PRODUCT_MODEL, SiteSelectForm
 
 from vendor.forms import OfferForm, PriceFormSet, CreditCardForm, AddressForm,\
-    AuthorizeNetIntegrationForm, StripeIntegrationForm, SubscriptionForm,\
-    SiteSelectForm, SubscriptionAddPaymentForm, OfferSiteSelectForm
+    SubscriptionForm, SiteSelectForm, SubscriptionAddPaymentForm, OfferSiteSelectForm
 
-from vendor.integrations import AuthorizeNetIntegration, StripeIntegration
 from vendor.models import Invoice, Offer, Receipt, CustomerProfile, Payment, Subscription
-from vendor.models.choice import TermType, PaymentTypes, InvoiceStatus, PurchaseStatus, SubscriptionStatus
+from vendor.models.choice import PaymentTypes, InvoiceStatus, PurchaseStatus
 from vendor.views.mixin import PassRequestToFormKwargsMixin, SiteOnRequestFilterMixin, TableFilterMixin, get_site_from_request
 from vendor.processors import get_site_payment_processor
 from vendor.utils import get_subscription_start_date, get_payment_scheduled_end_date
-from siteconfigs.models import SiteConfigModel
 
 Product = apps.get_model(VENDOR_PRODUCT_MODEL)
 logger = logging.getLogger(__name__)
 
 
 #############
 # Admin Views
@@ -496,111 +491,7 @@
         site = get_site_from_request(self.request)
         return Payment.objects.filter(invoice__site=site, success=True).annotate(order_item_count=Count('invoice__order_items')).filter(order_item_count=0)
 
     def get_context_data(self, *args, **kwargs):
         context = super().get_context_data(**kwargs)
         context['title'] = _("Payments with no Order Items")
         return context
-
-
-class PaymentProcessorSiteConfigsListView(ListView):
-    template_name = 'vendor/manage/processor_site_config_list.html'
-    model = SiteConfigModel
-
-    def get_queryset(self):
-        payment_processor = PaymentProcessorSiteConfig()
-
-        return SiteConfigModel.objects.filter(key=payment_processor.key)
-
-
-class PaymentProcessorSiteFormView(SiteOnRequestFilterMixin, FormView):
-    template_name = 'vendor/manage/processor_site_config.html'
-    form_class = PaymentProcessorForm
-
-    def get_success_url(self):
-        return reverse('vendor_admin:vendor-site-processor')
-
-    def get_context_data(self, *args, **kwargs):
-        context = super().get_context_data(*args, **kwargs)
-
-        site = get_site_from_request(self.request)
-        processor_config = PaymentProcessorSiteConfig(site)
-        context['form'] = processor_config.get_form()
-
-        return context
-
-    def form_valid(self, form):
-        site = get_site_from_request(self.request)
-        processor_config = PaymentProcessorSiteConfig(site)
-        processor_config.save(form.cleaned_data["payment_processor"], "payment_processor")
-
-        return redirect('vendor_admin:vendor-processor-lists')
-
-
-class PaymentProcessorSiteSelectFormView(FormView):
-    template_name = 'vendor/manage/processor_site_config.html'
-    form_class = PaymentProcessorSiteSelectForm
-
-    def get_success_url(self):
-        return reverse('vendor_admin:processor-lists')
-
-    def get_context_data(self, *args, **kwargs):
-        context = super().get_context_data(*args, **kwargs)
-
-        if self.kwargs.get('domain'):
-            site = Site.objects.get(domain=self.kwargs.get('domain'))
-            processor_config = PaymentProcessorSiteSelectSiteConfig(site)
-        else:
-            processor_config = PaymentProcessorSiteSelectSiteConfig()
-        context['form'] = processor_config.get_form()
-
-        return context
-
-    def form_valid(self, form):
-        site = Site.objects.get(pk=form.cleaned_data['site'])
-        processor_config = PaymentProcessorSiteSelectSiteConfig(site)
-        processor_config.save(form.cleaned_data["payment_processor"], "payment_processor")
-        
-        return redirect('vendor_admin:vendor-processor-lists')
-
-
-class AuthorizeNetIntegrationView(FormView):
-    template_name = "vendor/integration_form.html"
-    form_class = AuthorizeNetIntegrationForm
-    success_url = reverse_lazy('authorizenet-integration')
-
-    def get_context_data(self, *args, **kwargs):
-        context = super().get_context_data(**kwargs)
-        authorizenet_integration = AuthorizeNetIntegration(get_site_from_request(self.request))
-        context['integration_name'] = _("AuthorizeNet Integration")
-
-        context['form'] = AuthorizeNetIntegrationForm(instance=authorizenet_integration.instance)
-
-        return context
-    
-    def form_valid(self, form):
-        authorizenet_integration = AuthorizeNetIntegration(get_site_from_request(self.request))
-        authorizenet_integration.save(form.cleaned_data)
-
-        return super().form_valid(form)
-
-
-class StripeIntegrationView(FormView):
-    template_name = "vendor/integration_form.html"
-    form_class = StripeIntegrationForm
-    success_url = reverse_lazy('stripe-integration')
-
-    def get_context_data(self, *args, **kwargs):
-        context = super().get_context_data(**kwargs)
-        stripe_integration = StripeIntegration(get_site_from_request(self.request))
-        context['integration_name'] = _("Stripe Integration")
-
-        context['form'] = StripeIntegrationForm(instance=stripe_integration.instance)
-
-        return context
-    
-    def form_valid(self, form):
-        stripe_integration = StripeIntegration(get_site_from_request(self.request))
-        stripe_integration.save(form.cleaned_data)
-
-        return super().form_valid(form)
-
```

