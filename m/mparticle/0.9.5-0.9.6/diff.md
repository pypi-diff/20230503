# Comparing `tmp/mparticle-0.9.5.tar.gz` & `tmp/mparticle-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mparticle-0.9.5.tar", last modified: Thu Dec  8 21:13:08 2016, max compression
+gzip compressed data, was "dist/mparticle-0.9.6.tar", last modified: Sun Dec 11 20:04:45 2016, max compression
```

## Comparing `mparticle-0.9.5.tar` & `mparticle-0.9.6.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 sdozor   (1837106326) staff       (20)        0 2016-12-08 21:13:08.000000 mparticle-0.9.5/
-drwxr-xr-x   0 sdozor   (1837106326) staff       (20)        0 2016-12-08 21:13:08.000000 mparticle-0.9.5/mparticle/
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     2718 2016-10-28 19:55:35.000000 mparticle-0.9.5/mparticle/__init__.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)    21105 2016-12-08 21:12:52.000000 mparticle-0.9.5/mparticle/api_client.py
-drwxr-xr-x   0 sdozor   (1837106326) staff       (20)        0 2016-12-08 21:13:08.000000 mparticle-0.9.5/mparticle/apis/
--rw-r--r--   0 sdozor   (1837106326) staff       (20)      105 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/apis/__init__.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     9459 2016-10-28 19:55:35.000000 mparticle-0.9.5/mparticle/apis/events_api.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     7415 2016-11-30 22:52:50.000000 mparticle-0.9.5/mparticle/configuration.py
-drwxr-xr-x   0 sdozor   (1837106326) staff       (20)        0 2016-12-08 21:13:08.000000 mparticle-0.9.5/mparticle/models/
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     2322 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/__init__.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     3400 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/api_response.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     3917 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/api_response_errors.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)    11877 2016-12-08 21:09:49.000000 mparticle-0.9.5/mparticle/models/app_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     5755 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/application_information.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)    14460 2016-10-28 19:55:35.000000 mparticle-0.9.5/mparticle/models/application_state_transition_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     4736 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/attribution_info.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)    13514 2016-12-06 22:01:27.000000 mparticle-0.9.5/mparticle/models/batch.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     9721 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/breadcrumb_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)    13770 2016-10-28 19:55:35.000000 mparticle-0.9.5/mparticle/models/commerce_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)    16309 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/crash_report_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)    17239 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/device_current_state.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)    27586 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/device_information.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     4436 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/event_base.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     8289 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/event_data.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     8425 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/first_run_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     4554 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/geo_location.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     8414 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/media_info.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)    13134 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/network_performance_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     9003 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/opt_out_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     9868 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/product.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)    11246 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/product_action.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     4307 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/product_impression.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)    10928 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/profile_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     4873 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/promotion.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     4281 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/promotion_action.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)    14221 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/push_message_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)    10102 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/push_registration_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     9811 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/screen_view_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     9278 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/session_end_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     8561 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/session_start_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     3412 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/shopping_cart.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     5739 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/source_information.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     8767 2016-08-16 16:17:48.000000 mparticle-0.9.5/mparticle/models/user_identities.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     9197 2016-11-30 22:48:05.000000 mparticle-0.9.5/mparticle/rest.py
-drwxr-xr-x   0 sdozor   (1837106326) staff       (20)        0 2016-12-08 21:13:08.000000 mparticle-0.9.5/mparticle.egg-info/
--rw-r--r--   0 sdozor   (1837106326) staff       (20)        1 2016-12-08 21:13:08.000000 mparticle-0.9.5/mparticle.egg-info/dependency_links.txt
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1229 2016-12-08 21:13:08.000000 mparticle-0.9.5/mparticle.egg-info/PKG-INFO
--rw-r--r--   0 sdozor   (1837106326) staff       (20)       52 2016-12-08 21:13:08.000000 mparticle-0.9.5/mparticle.egg-info/requires.txt
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     2586 2016-12-08 21:13:08.000000 mparticle-0.9.5/mparticle.egg-info/SOURCES.txt
--rw-r--r--   0 sdozor   (1837106326) staff       (20)       15 2016-12-08 21:13:08.000000 mparticle-0.9.5/mparticle.egg-info/top_level.txt
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1229 2016-12-08 21:13:08.000000 mparticle-0.9.5/PKG-INFO
--rw-r--r--   0 sdozor   (1837106326) staff       (20)      100 2016-12-08 21:13:08.000000 mparticle-0.9.5/setup.cfg
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1678 2016-12-08 21:12:59.000000 mparticle-0.9.5/setup.py
-drwxr-xr-x   0 sdozor   (1837106326) staff       (20)        0 2016-12-08 21:13:08.000000 mparticle-0.9.5/test/
--rw-r--r--   0 sdozor   (1837106326) staff       (20)        0 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/__init__.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1299 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_api_response.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1349 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_api_response_errors.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     2131 2016-12-08 21:09:49.000000 mparticle-0.9.5/test/test_app_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1387 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_application_information.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1463 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_application_state_transition_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1331 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_attribution_info.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1249 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_batch.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1331 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_breadcrumb_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1315 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_commerce_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1341 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_crash_report_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1357 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_device_current_state.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1347 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_device_information.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1283 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_event_base.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1283 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_event_data.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1486 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_events_api.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1317 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_first_run_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1299 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_geo_location.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1283 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_media_info.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1397 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_network_performance_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1301 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_opt_out_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1265 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_product.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1315 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_product_action.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1347 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_product_impression.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1307 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_profile_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1281 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_promotion.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1331 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_promotion_action.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1341 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_push_message_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1381 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_push_registration_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1333 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_screen_view_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1333 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_session_end_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1349 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_session_start_event.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1307 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_shopping_cart.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1347 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_source_information.py
--rw-r--r--   0 sdozor   (1837106326) staff       (20)     1323 2016-08-16 16:17:48.000000 mparticle-0.9.5/test/test_user_identities.py
+drwxr-xr-x   0 sdozor   (1837106326) staff       (20)        0 2016-12-11 20:04:45.000000 mparticle-0.9.6/
+drwxr-xr-x   0 sdozor   (1837106326) staff       (20)        0 2016-12-11 20:04:45.000000 mparticle-0.9.6/mparticle/
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     2718 2016-10-28 19:55:35.000000 mparticle-0.9.6/mparticle/__init__.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)    21129 2016-12-11 20:00:18.000000 mparticle-0.9.6/mparticle/api_client.py
+drwxr-xr-x   0 sdozor   (1837106326) staff       (20)        0 2016-12-11 20:04:45.000000 mparticle-0.9.6/mparticle/apis/
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)      105 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/apis/__init__.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     9459 2016-10-28 19:55:35.000000 mparticle-0.9.6/mparticle/apis/events_api.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     7415 2016-11-30 22:52:50.000000 mparticle-0.9.6/mparticle/configuration.py
+drwxr-xr-x   0 sdozor   (1837106326) staff       (20)        0 2016-12-11 20:04:45.000000 mparticle-0.9.6/mparticle/models/
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     2322 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/__init__.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     3400 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/api_response.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     3917 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/api_response_errors.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)    11877 2016-12-08 21:09:49.000000 mparticle-0.9.6/mparticle/models/app_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     5755 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/application_information.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)    14460 2016-10-28 19:55:35.000000 mparticle-0.9.6/mparticle/models/application_state_transition_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     4736 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/attribution_info.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)    13514 2016-12-06 22:01:27.000000 mparticle-0.9.6/mparticle/models/batch.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     9721 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/breadcrumb_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)    13770 2016-10-28 19:55:35.000000 mparticle-0.9.6/mparticle/models/commerce_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)    16309 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/crash_report_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)    17239 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/device_current_state.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)    27586 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/device_information.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     4436 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/event_base.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     8289 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/event_data.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     8425 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/first_run_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     4554 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/geo_location.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     8414 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/media_info.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)    13134 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/network_performance_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     9003 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/opt_out_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     9868 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/product.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)    11246 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/product_action.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     4307 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/product_impression.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)    10928 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/profile_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     4873 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/promotion.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     4281 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/promotion_action.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)    14221 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/push_message_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)    10102 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/push_registration_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     9811 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/screen_view_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     9278 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/session_end_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     8561 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/session_start_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     3412 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/shopping_cart.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     5739 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/source_information.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     8767 2016-08-16 16:17:48.000000 mparticle-0.9.6/mparticle/models/user_identities.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     9197 2016-11-30 22:48:05.000000 mparticle-0.9.6/mparticle/rest.py
+drwxr-xr-x   0 sdozor   (1837106326) staff       (20)        0 2016-12-11 20:04:45.000000 mparticle-0.9.6/mparticle.egg-info/
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)        1 2016-12-11 20:04:45.000000 mparticle-0.9.6/mparticle.egg-info/dependency_links.txt
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1229 2016-12-11 20:04:45.000000 mparticle-0.9.6/mparticle.egg-info/PKG-INFO
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)       52 2016-12-11 20:04:45.000000 mparticle-0.9.6/mparticle.egg-info/requires.txt
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     2586 2016-12-11 20:04:45.000000 mparticle-0.9.6/mparticle.egg-info/SOURCES.txt
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)       15 2016-12-11 20:04:45.000000 mparticle-0.9.6/mparticle.egg-info/top_level.txt
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1229 2016-12-11 20:04:45.000000 mparticle-0.9.6/PKG-INFO
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)      100 2016-12-11 20:04:45.000000 mparticle-0.9.6/setup.cfg
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1678 2016-12-11 20:00:18.000000 mparticle-0.9.6/setup.py
+drwxr-xr-x   0 sdozor   (1837106326) staff       (20)        0 2016-12-11 20:04:45.000000 mparticle-0.9.6/test/
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)        0 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/__init__.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1299 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_api_response.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1349 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_api_response_errors.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     2131 2016-12-08 21:09:49.000000 mparticle-0.9.6/test/test_app_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1387 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_application_information.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1463 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_application_state_transition_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1331 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_attribution_info.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1249 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_batch.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1331 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_breadcrumb_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1315 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_commerce_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1341 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_crash_report_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1357 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_device_current_state.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1347 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_device_information.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1283 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_event_base.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1283 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_event_data.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1486 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_events_api.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1317 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_first_run_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1299 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_geo_location.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1283 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_media_info.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1397 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_network_performance_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1301 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_opt_out_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1265 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_product.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1315 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_product_action.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1347 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_product_impression.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1307 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_profile_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1281 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_promotion.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1331 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_promotion_action.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1341 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_push_message_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1381 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_push_registration_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1333 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_screen_view_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1333 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_session_end_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1349 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_session_start_event.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1307 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_shopping_cart.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1347 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_source_information.py
+-rw-r--r--   0 sdozor   (1837106326) staff       (20)     1323 2016-08-16 16:17:48.000000 mparticle-0.9.6/test/test_user_identities.py
```

### Comparing `mparticle-0.9.5/mparticle/__init__.py` & `mparticle-0.9.6/mparticle/__init__.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/api_client.py` & `mparticle-0.9.6/mparticle/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             self.default_headers[header_name] = header_value
         if host is None:
             self.host = self.config.host
         else:
             self.host = host
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'mParticle Python client/0.9.5'
+        self.user_agent = 'mParticle Python client/0.9.6'
 
     @property
     def user_agent(self):
         """
         Gets user agent.
         """
         return self.default_headers['User-Agent']
@@ -116,15 +116,15 @@
 
         # headers parameters
         header_params = header_params or {}
         header_params.update(self.default_headers)
         if self.cookie:
             header_params['Cookie'] = self.cookie
         if header_params:
-            header_params = ApiClient.  (header_params)
+            header_params = ApiClient.sanitize_for_serialization(header_params)
 
         # path parameters
         if path_params:
             path_params = ApiClient.sanitize_for_serialization(path_params)
             for k, v in iteritems(path_params):
                 replacement = quote(str(self.to_path_value(v)))
                 resource_path = resource_path.\
```

### Comparing `mparticle-0.9.5/mparticle/apis/events_api.py` & `mparticle-0.9.6/mparticle/apis/events_api.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/configuration.py` & `mparticle-0.9.6/mparticle/configuration.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/__init__.py` & `mparticle-0.9.6/mparticle/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/api_response.py` & `mparticle-0.9.6/mparticle/models/api_response.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/api_response_errors.py` & `mparticle-0.9.6/mparticle/models/api_response_errors.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/app_event.py` & `mparticle-0.9.6/mparticle/models/app_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/application_information.py` & `mparticle-0.9.6/mparticle/models/application_information.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/application_state_transition_event.py` & `mparticle-0.9.6/mparticle/models/application_state_transition_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/attribution_info.py` & `mparticle-0.9.6/mparticle/models/attribution_info.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/batch.py` & `mparticle-0.9.6/mparticle/models/batch.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/breadcrumb_event.py` & `mparticle-0.9.6/mparticle/models/breadcrumb_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/commerce_event.py` & `mparticle-0.9.6/mparticle/models/commerce_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/crash_report_event.py` & `mparticle-0.9.6/mparticle/models/crash_report_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/device_current_state.py` & `mparticle-0.9.6/mparticle/models/device_current_state.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/device_information.py` & `mparticle-0.9.6/mparticle/models/device_information.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/event_base.py` & `mparticle-0.9.6/mparticle/models/event_base.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/event_data.py` & `mparticle-0.9.6/mparticle/models/event_data.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/first_run_event.py` & `mparticle-0.9.6/mparticle/models/first_run_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/geo_location.py` & `mparticle-0.9.6/mparticle/models/geo_location.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/media_info.py` & `mparticle-0.9.6/mparticle/models/media_info.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/network_performance_event.py` & `mparticle-0.9.6/mparticle/models/network_performance_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/opt_out_event.py` & `mparticle-0.9.6/mparticle/models/opt_out_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/product.py` & `mparticle-0.9.6/mparticle/models/product.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/product_action.py` & `mparticle-0.9.6/mparticle/models/product_action.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/product_impression.py` & `mparticle-0.9.6/mparticle/models/product_impression.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/profile_event.py` & `mparticle-0.9.6/mparticle/models/profile_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/promotion.py` & `mparticle-0.9.6/mparticle/models/promotion.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/promotion_action.py` & `mparticle-0.9.6/mparticle/models/promotion_action.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/push_message_event.py` & `mparticle-0.9.6/mparticle/models/push_message_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/push_registration_event.py` & `mparticle-0.9.6/mparticle/models/push_registration_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/screen_view_event.py` & `mparticle-0.9.6/mparticle/models/screen_view_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/session_end_event.py` & `mparticle-0.9.6/mparticle/models/session_end_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/session_start_event.py` & `mparticle-0.9.6/mparticle/models/session_start_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/shopping_cart.py` & `mparticle-0.9.6/mparticle/models/shopping_cart.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/source_information.py` & `mparticle-0.9.6/mparticle/models/source_information.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/models/user_identities.py` & `mparticle-0.9.6/mparticle/models/user_identities.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle/rest.py` & `mparticle-0.9.6/mparticle/rest.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/mparticle.egg-info/PKG-INFO` & `mparticle-0.9.6/mparticle.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mparticle
-Version: 0.9.5
+Version: 0.9.6
 Summary: Python client for the mParticle platform
 Home-page: https://github.com/mParticle/mparticle-python-sdk
 Author: Sam Dozor
 Author-email: support@mparticle.com
 License: Apache 2.0
 Description: `Package Documentation <https://github.com/mParticle/mparticle-python-sdk/wiki>`_
```

### Comparing `mparticle-0.9.5/mparticle.egg-info/SOURCES.txt` & `mparticle-0.9.6/mparticle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/PKG-INFO` & `mparticle-0.9.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mparticle
-Version: 0.9.5
+Version: 0.9.6
 Summary: Python client for the mParticle platform
 Home-page: https://github.com/mParticle/mparticle-python-sdk
 Author: Sam Dozor
 Author-email: support@mparticle.com
 License: Apache 2.0
 Description: `Package Documentation <https://github.com/mParticle/mparticle-python-sdk/wiki>`_
```

### Comparing `mparticle-0.9.5/setup.py` & `mparticle-0.9.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages
 
 NAME = "mparticle"
-VERSION = "0.9.5"
+VERSION = "0.9.6"
 
 
 
 # To install the library, run the following
 #
 # python setup.py install
 #
```

### Comparing `mparticle-0.9.5/test/test_api_response.py` & `mparticle-0.9.6/test/test_api_response.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_api_response_errors.py` & `mparticle-0.9.6/test/test_api_response_errors.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_app_event.py` & `mparticle-0.9.6/test/test_app_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_application_information.py` & `mparticle-0.9.6/test/test_application_information.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_application_state_transition_event.py` & `mparticle-0.9.6/test/test_application_state_transition_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_attribution_info.py` & `mparticle-0.9.6/test/test_attribution_info.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_batch.py` & `mparticle-0.9.6/test/test_batch.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_breadcrumb_event.py` & `mparticle-0.9.6/test/test_breadcrumb_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_commerce_event.py` & `mparticle-0.9.6/test/test_commerce_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_crash_report_event.py` & `mparticle-0.9.6/test/test_crash_report_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_device_current_state.py` & `mparticle-0.9.6/test/test_device_current_state.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_device_information.py` & `mparticle-0.9.6/test/test_device_information.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_event_base.py` & `mparticle-0.9.6/test/test_event_base.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_event_data.py` & `mparticle-0.9.6/test/test_event_data.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_events_api.py` & `mparticle-0.9.6/test/test_events_api.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_first_run_event.py` & `mparticle-0.9.6/test/test_first_run_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_geo_location.py` & `mparticle-0.9.6/test/test_geo_location.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_media_info.py` & `mparticle-0.9.6/test/test_media_info.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_network_performance_event.py` & `mparticle-0.9.6/test/test_network_performance_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_opt_out_event.py` & `mparticle-0.9.6/test/test_opt_out_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_product.py` & `mparticle-0.9.6/test/test_product.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_product_action.py` & `mparticle-0.9.6/test/test_product_action.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_product_impression.py` & `mparticle-0.9.6/test/test_product_impression.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_profile_event.py` & `mparticle-0.9.6/test/test_profile_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_promotion.py` & `mparticle-0.9.6/test/test_promotion.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_promotion_action.py` & `mparticle-0.9.6/test/test_promotion_action.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_push_message_event.py` & `mparticle-0.9.6/test/test_push_message_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_push_registration_event.py` & `mparticle-0.9.6/test/test_push_registration_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_screen_view_event.py` & `mparticle-0.9.6/test/test_screen_view_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_session_end_event.py` & `mparticle-0.9.6/test/test_session_end_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_session_start_event.py` & `mparticle-0.9.6/test/test_session_start_event.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_shopping_cart.py` & `mparticle-0.9.6/test/test_shopping_cart.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_source_information.py` & `mparticle-0.9.6/test/test_source_information.py`

 * *Files identical despite different names*

### Comparing `mparticle-0.9.5/test/test_user_identities.py` & `mparticle-0.9.6/test/test_user_identities.py`

 * *Files identical despite different names*

