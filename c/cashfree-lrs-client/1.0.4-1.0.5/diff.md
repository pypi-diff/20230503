# Comparing `tmp/cashfree_lrs_client-1.0.4.tar.gz` & `tmp/cashfree_lrs_client-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashfree_lrs_client-1.0.4.tar", max compression
+gzip compressed data, was "cashfree_lrs_client-1.0.5.tar", max compression
```

## Comparing `cashfree_lrs_client-1.0.4.tar` & `cashfree_lrs_client-1.0.5.tar`

### file list

```diff
@@ -1,113 +1,114 @@
--rw-r--r--   0        0        0     5243 2023-05-01 12:05:34.721164 cashfree_lrs_client-1.0.4/README.md
--rw-r--r--   0        0        0     1702 2023-05-01 12:05:34.745164 cashfree_lrs_client-1.0.4/cashfree_lrs_client/__init__.py
--rw-r--r--   0        0        0       99 2023-05-01 12:05:34.749164 cashfree_lrs_client-1.0.4/cashfree_lrs_client/api/__init__.py
--rw-r--r--   0        0        0    53538 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/api/default_api.py
--rw-r--r--   0        0        0    53367 2023-05-01 12:05:34.697164 cashfree_lrs_client-1.0.4/cashfree_lrs_client/api/lrs_api.py
--rw-r--r--   0        0        0    29632 2023-05-01 12:05:34.757164 cashfree_lrs_client-1.0.4/cashfree_lrs_client/api_client.py
--rw-r--r--   0        0        0      214 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/apis/__init__.py
--rw-r--r--   0        0        0     1655 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/apis/path_to_api.py
--rw-r--r--   0        0        0      246 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/apis/paths/__init__.py
--rw-r--r--   0        0        0      119 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/apis/paths/beneficiaries.py
--rw-r--r--   0        0        0      121 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/apis/paths/fx_rate_details.py
--rw-r--r--   0        0        0      105 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/apis/paths/orders.py
--rw-r--r--   0        0        0      137 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/apis/paths/orders_documents_upload.py
--rw-r--r--   0        0        0      153 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/apis/paths/orders_order_id_documents_upload.py
--rw-r--r--   0        0        0      136 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/apis/paths/orders_order_id_process.py
--rw-r--r--   0        0        0      111 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/apis/paths/remitters.py
--rw-r--r--   0        0        0      109 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/apis/paths/webhooks.py
--rw-r--r--   0        0        0      306 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/apis/tag_to_api.py
--rw-r--r--   0        0        0      308 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/apis/tags/__init__.py
--rw-r--r--   0        0        0     1162 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/apis/tags/lrs_api.py
--rw-r--r--   0        0        0    15922 2023-05-01 12:05:34.745164 cashfree_lrs_client-1.0.4/cashfree_lrs_client/configuration.py
--rw-r--r--   0        0        0     2815 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/docs/CreateBeneficiaryRequest.md
--rw-r--r--   0        0        0     2331 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/docs/CreateOrderRequest.md
--rw-r--r--   0        0        0     1337 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/docs/CreateOrderResponse.md
--rw-r--r--   0        0        0     2583 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/docs/CreateRemitterRequest.md
--rw-r--r--   0        0        0      389 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/docs/Currency.md
--rw-r--r--   0        0        0      859 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/docs/Error.md
--rw-r--r--   0        0        0     1656 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/docs/FetchForexRateRequest.md
--rw-r--r--   0        0        0    59748 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/docs/LrsApi.md
--rw-r--r--   0        0        0      343 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/docs/Purpose.md
--rw-r--r--   0        0        0     1239 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/docs/SetupWebhooksRequest.md
--rw-r--r--   0        0        0      896 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/docs/SuccessMessage.md
--rw-r--r--   0        0        0     5118 2023-05-01 12:05:34.753164 cashfree_lrs_client-1.0.4/cashfree_lrs_client/exceptions.py
--rw-r--r--   0        0        0      353 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/__init__.py
--rw-r--r--   0        0        0      884 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/amount.py
--rw-r--r--   0        0        0      815 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/amount.pyi
--rw-r--r--   0        0        0    14903 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/create_beneficiary_request.py
--rw-r--r--   0        0        0    13066 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/create_beneficiary_request.pyi
--rw-r--r--   0        0        0    11475 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/create_order_request.py
--rw-r--r--   0        0        0    10572 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/create_order_request.pyi
--rw-r--r--   0        0        0     8398 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/create_order_response.py
--rw-r--r--   0        0        0     8166 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/create_order_response.pyi
--rw-r--r--   0        0        0    12349 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/create_remitter_request.py
--rw-r--r--   0        0        0    10785 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/create_remitter_request.pyi
--rw-r--r--   0        0        0     1192 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/currency.py
--rw-r--r--   0        0        0     1031 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/currency.pyi
--rw-r--r--   0        0        0     3384 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/error.py
--rw-r--r--   0        0        0     3384 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/error.pyi
--rw-r--r--   0        0        0     5805 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/fetch_forex_rate_request.py
--rw-r--r--   0        0        0     5697 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/fetch_forex_rate_request.pyi
--rw-r--r--   0        0        0     1368 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/purpose.py
--rw-r--r--   0        0        0     1169 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/purpose.pyi
--rw-r--r--   0        0        0     3663 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/setup_webhooks_request.py
--rw-r--r--   0        0        0     3663 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/setup_webhooks_request.pyi
--rw-r--r--   0        0        0     2477 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/success_message.py
--rw-r--r--   0        0        0     2477 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/success_message.pyi
--rw-r--r--   0        0        0     1119 2023-05-01 12:05:34.749164 cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/__init__.py
--rw-r--r--   0        0        0      714 2023-05-01 12:05:34.449165 cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/country.py
--rw-r--r--   0        0        0     1975 2023-05-01 12:05:14.149045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/create_beneficiary200_response.py
--rw-r--r--   0        0        0     5660 2023-05-01 12:05:34.477165 cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/create_beneficiary_request.py
--rw-r--r--   0        0        0     5041 2023-05-01 12:05:34.489165 cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/create_order_request.py
--rw-r--r--   0        0        0     3426 2023-05-01 12:05:34.501165 cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/create_order_response.py
--rw-r--r--   0        0        0     1951 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/create_remitter200_response.py
--rw-r--r--   0        0        0     5347 2023-05-01 12:05:34.509165 cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/create_remitter_request.py
--rw-r--r--   0        0        0      765 2023-05-01 12:05:34.517165 cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/currency.py
--rw-r--r--   0        0        0     2088 2023-05-01 12:05:34.521165 cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/error.py
--rw-r--r--   0        0        0     3279 2023-05-01 12:05:34.529165 cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/fetch_forex_rate_request.py
--rw-r--r--   0        0        0     2903 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/order_response.py
--rw-r--r--   0        0        0      780 2023-05-01 12:05:34.537165 cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/purpose.py
--rw-r--r--   0        0        0     1943 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/setup_webhooks200_response.py
--rw-r--r--   0        0        0     2361 2023-05-01 12:05:34.541164 cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/setup_webhooks_request.py
--rw-r--r--   0        0        0     1909 2023-05-01 12:05:34.549164 cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/success_message.py
--rw-r--r--   0        0        0      644 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/__init__.py
--rw-r--r--   0        0        0      323 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/beneficiaries/__init__.py
--rw-r--r--   0        0        0    12582 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/beneficiaries/post.py
--rw-r--r--   0        0        0    12396 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/beneficiaries/post.pyi
--rw-r--r--   0        0        0      326 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/fx_rate_details/__init__.py
--rw-r--r--   0        0        0    11760 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/fx_rate_details/post.py
--rw-r--r--   0        0        0    11604 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/fx_rate_details/post.pyi
--rw-r--r--   0        0        0      309 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/orders/__init__.py
--rw-r--r--   0        0        0    13005 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/orders/post.py
--rw-r--r--   0        0        0    12789 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/orders/post.pyi
--rw-r--r--   0        0        0      343 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/orders_documents_upload/__init__.py
--rw-r--r--   0        0        0    12334 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/orders_documents_upload/post.py
--rw-r--r--   0        0        0    12148 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/orders_documents_upload/post.pyi
--rw-r--r--   0        0        0      361 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/orders_order_id_documents_upload/__init__.py
--rw-r--r--   0        0        0    15715 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.py
--rw-r--r--   0        0        0    15469 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.pyi
--rw-r--r--   0        0        0      343 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/orders_order_id_process/__init__.py
--rw-r--r--   0        0        0     8093 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/orders_order_id_process/post.py
--rw-r--r--   0        0        0     7937 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/orders_order_id_process/post.pyi
--rw-r--r--   0        0        0      315 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/remitters/__init__.py
--rw-r--r--   0        0        0    12525 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/remitters/post.py
--rw-r--r--   0        0        0    12339 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/remitters/post.pyi
--rw-r--r--   0        0        0      313 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/webhooks/__init__.py
--rw-r--r--   0        0        0    11939 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/webhooks/post.py
--rw-r--r--   0        0        0    11783 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/webhooks/post.pyi
--rw-r--r--   0        0        0    12643 2023-05-01 12:05:34.761164 cashfree_lrs_client-1.0.4/cashfree_lrs_client/rest.py
--rw-r--r--   0        0        0    97649 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/schemas.py
--rw-r--r--   0        0        0        0 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/test/__init__.py
--rw-r--r--   0        0        0     2694 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/test/test_create_beneficiary_request.py
--rw-r--r--   0        0        0     2292 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/test/test_create_order_request.py
--rw-r--r--   0        0        0     1952 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/test/test_create_order_response.py
--rw-r--r--   0        0        0     2486 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/test/test_create_remitter_request.py
--rw-r--r--   0        0        0      738 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/test/test_currency.py
--rw-r--r--   0        0        0     1439 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/test/test_error.py
--rw-r--r--   0        0        0     1860 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/test/test_fetch_forex_rate_request.py
--rw-r--r--   0        0        0     1845 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/test/test_lrs_api.py
--rw-r--r--   0        0        0      731 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/test/test_purpose.py
--rw-r--r--   0        0        0     1737 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/test/test_setup_webhooks_request.py
--rw-r--r--   0        0        0     1493 2023-05-01 12:05:14.153045 cashfree_lrs_client-1.0.4/cashfree_lrs_client/test/test_success_message.py
--rw-r--r--   0        0        0      683 2023-05-01 12:05:34.737164 cashfree_lrs_client-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     6146 1970-01-01 00:00:00.000000 cashfree_lrs_client-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     5353 2023-05-03 17:46:50.957705 cashfree_lrs_client-1.0.5/README.md
+-rw-r--r--   0        0        0     1759 2023-05-03 17:46:50.997706 cashfree_lrs_client-1.0.5/cashfree_lrs_client/__init__.py
+-rw-r--r--   0        0        0       99 2023-05-03 17:46:51.001706 cashfree_lrs_client-1.0.5/cashfree_lrs_client/api/__init__.py
+-rw-r--r--   0        0        0    53538 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/api/default_api.py
+-rw-r--r--   0        0        0    53935 2023-05-03 17:46:50.933705 cashfree_lrs_client-1.0.5/cashfree_lrs_client/api/lrs_api.py
+-rw-r--r--   0        0        0    30034 2023-05-03 17:46:51.013706 cashfree_lrs_client-1.0.5/cashfree_lrs_client/api_client.py
+-rw-r--r--   0        0        0      844 2023-05-03 17:46:51.013706 cashfree_lrs_client-1.0.5/cashfree_lrs_client/api_response.py
+-rw-r--r--   0        0        0      214 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/__init__.py
+-rw-r--r--   0        0        0     1655 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/path_to_api.py
+-rw-r--r--   0        0        0      246 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/paths/__init__.py
+-rw-r--r--   0        0        0      119 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/paths/beneficiaries.py
+-rw-r--r--   0        0        0      121 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/paths/fx_rate_details.py
+-rw-r--r--   0        0        0      105 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/paths/orders.py
+-rw-r--r--   0        0        0      137 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/paths/orders_documents_upload.py
+-rw-r--r--   0        0        0      153 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/paths/orders_order_id_documents_upload.py
+-rw-r--r--   0        0        0      136 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/paths/orders_order_id_process.py
+-rw-r--r--   0        0        0      111 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/paths/remitters.py
+-rw-r--r--   0        0        0      109 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/paths/webhooks.py
+-rw-r--r--   0        0        0      306 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/tag_to_api.py
+-rw-r--r--   0        0        0      308 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/tags/__init__.py
+-rw-r--r--   0        0        0     1162 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/tags/lrs_api.py
+-rw-r--r--   0        0        0    15922 2023-05-03 17:46:50.989706 cashfree_lrs_client-1.0.5/cashfree_lrs_client/configuration.py
+-rw-r--r--   0        0        0     2815 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/CreateBeneficiaryRequest.md
+-rw-r--r--   0        0        0     2331 2023-05-03 17:46:25.205357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/CreateOrderRequest.md
+-rw-r--r--   0        0        0     1337 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/CreateOrderResponse.md
+-rw-r--r--   0        0        0     2583 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/CreateRemitterRequest.md
+-rw-r--r--   0        0        0      389 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/Currency.md
+-rw-r--r--   0        0        0      859 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/Error.md
+-rw-r--r--   0        0        0     1656 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/FetchForexRateRequest.md
+-rw-r--r--   0        0        0    59748 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/LrsApi.md
+-rw-r--r--   0        0        0      343 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/Purpose.md
+-rw-r--r--   0        0        0     1239 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/SetupWebhooksRequest.md
+-rw-r--r--   0        0        0      896 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/SuccessMessage.md
+-rw-r--r--   0        0        0     5118 2023-05-03 17:46:51.005706 cashfree_lrs_client-1.0.5/cashfree_lrs_client/exceptions.py
+-rw-r--r--   0        0        0      353 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/__init__.py
+-rw-r--r--   0        0        0      884 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/amount.py
+-rw-r--r--   0        0        0      815 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/amount.pyi
+-rw-r--r--   0        0        0    14903 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_beneficiary_request.py
+-rw-r--r--   0        0        0    13066 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_beneficiary_request.pyi
+-rw-r--r--   0        0        0    11475 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_order_request.py
+-rw-r--r--   0        0        0    10572 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_order_request.pyi
+-rw-r--r--   0        0        0     8398 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_order_response.py
+-rw-r--r--   0        0        0     8166 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_order_response.pyi
+-rw-r--r--   0        0        0    12349 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_remitter_request.py
+-rw-r--r--   0        0        0    10785 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_remitter_request.pyi
+-rw-r--r--   0        0        0     1192 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/currency.py
+-rw-r--r--   0        0        0     1031 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/currency.pyi
+-rw-r--r--   0        0        0     3384 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/error.py
+-rw-r--r--   0        0        0     3384 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/error.pyi
+-rw-r--r--   0        0        0     5805 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/fetch_forex_rate_request.py
+-rw-r--r--   0        0        0     5697 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/fetch_forex_rate_request.pyi
+-rw-r--r--   0        0        0     1368 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/purpose.py
+-rw-r--r--   0        0        0     1169 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/purpose.pyi
+-rw-r--r--   0        0        0     3663 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/setup_webhooks_request.py
+-rw-r--r--   0        0        0     3663 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/setup_webhooks_request.pyi
+-rw-r--r--   0        0        0     2477 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/success_message.py
+-rw-r--r--   0        0        0     2477 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/success_message.pyi
+-rw-r--r--   0        0        0     1119 2023-05-03 17:46:51.001706 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-03 17:46:50.657701 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/country.py
+-rw-r--r--   0        0        0     1975 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/create_beneficiary200_response.py
+-rw-r--r--   0        0        0     5660 2023-05-03 17:46:50.689701 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/create_beneficiary_request.py
+-rw-r--r--   0        0        0     5041 2023-05-03 17:46:50.721702 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/create_order_request.py
+-rw-r--r--   0        0        0     3426 2023-05-03 17:46:50.741702 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/create_order_response.py
+-rw-r--r--   0        0        0     1951 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/create_remitter200_response.py
+-rw-r--r--   0        0        0     5347 2023-05-03 17:46:50.757702 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/create_remitter_request.py
+-rw-r--r--   0        0        0      765 2023-05-03 17:46:50.769703 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/currency.py
+-rw-r--r--   0        0        0     2088 2023-05-03 17:46:50.785703 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/error.py
+-rw-r--r--   0        0        0     3279 2023-05-03 17:46:50.793703 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/fetch_forex_rate_request.py
+-rw-r--r--   0        0        0     2903 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/order_response.py
+-rw-r--r--   0        0        0      780 2023-05-03 17:46:50.797703 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/purpose.py
+-rw-r--r--   0        0        0     1943 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/setup_webhooks200_response.py
+-rw-r--r--   0        0        0     2361 2023-05-03 17:46:50.801703 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/setup_webhooks_request.py
+-rw-r--r--   0        0        0     1909 2023-05-03 17:46:50.809703 cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/success_message.py
+-rw-r--r--   0        0        0      644 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/beneficiaries/__init__.py
+-rw-r--r--   0        0        0    12582 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/beneficiaries/post.py
+-rw-r--r--   0        0        0    12396 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/beneficiaries/post.pyi
+-rw-r--r--   0        0        0      326 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/fx_rate_details/__init__.py
+-rw-r--r--   0        0        0    11760 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/fx_rate_details/post.py
+-rw-r--r--   0        0        0    11604 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/fx_rate_details/post.pyi
+-rw-r--r--   0        0        0      309 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders/__init__.py
+-rw-r--r--   0        0        0    13005 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders/post.py
+-rw-r--r--   0        0        0    12789 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders/post.pyi
+-rw-r--r--   0        0        0      343 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_documents_upload/__init__.py
+-rw-r--r--   0        0        0    12334 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_documents_upload/post.py
+-rw-r--r--   0        0        0    12148 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_documents_upload/post.pyi
+-rw-r--r--   0        0        0      361 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_order_id_documents_upload/__init__.py
+-rw-r--r--   0        0        0    15715 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.py
+-rw-r--r--   0        0        0    15469 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.pyi
+-rw-r--r--   0        0        0      343 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_order_id_process/__init__.py
+-rw-r--r--   0        0        0     8093 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_order_id_process/post.py
+-rw-r--r--   0        0        0     7937 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_order_id_process/post.pyi
+-rw-r--r--   0        0        0      315 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/remitters/__init__.py
+-rw-r--r--   0        0        0    12525 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/remitters/post.py
+-rw-r--r--   0        0        0    12339 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/remitters/post.pyi
+-rw-r--r--   0        0        0      313 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/webhooks/__init__.py
+-rw-r--r--   0        0        0    11939 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/webhooks/post.py
+-rw-r--r--   0        0        0    11783 2023-05-03 17:46:25.209357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/webhooks/post.pyi
+-rw-r--r--   0        0        0    12643 2023-05-03 17:46:51.017706 cashfree_lrs_client-1.0.5/cashfree_lrs_client/rest.py
+-rw-r--r--   0        0        0    97649 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/schemas.py
+-rw-r--r--   0        0        0        0 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/__init__.py
+-rw-r--r--   0        0        0     2694 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_create_beneficiary_request.py
+-rw-r--r--   0        0        0     2292 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_create_order_request.py
+-rw-r--r--   0        0        0     1952 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_create_order_response.py
+-rw-r--r--   0        0        0     2486 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_create_remitter_request.py
+-rw-r--r--   0        0        0      738 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_currency.py
+-rw-r--r--   0        0        0     1439 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_error.py
+-rw-r--r--   0        0        0     1860 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_fetch_forex_rate_request.py
+-rw-r--r--   0        0        0     1845 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_lrs_api.py
+-rw-r--r--   0        0        0      731 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_purpose.py
+-rw-r--r--   0        0        0     1737 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_setup_webhooks_request.py
+-rw-r--r--   0        0        0     1493 2023-05-03 17:46:25.213357 cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_success_message.py
+-rw-r--r--   0        0        0      683 2023-05-03 17:46:50.985706 cashfree_lrs_client-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6256 1970-01-01 00:00:00.000000 cashfree_lrs_client-1.0.5/PKG-INFO
```

### Comparing `cashfree_lrs_client-1.0.4/README.md` & `cashfree_lrs_client-1.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # cashfree-lrs-client
 CashFree LRS APIs (v2)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.4
-- Package version: 1.0.4
+- API version: 1.0.5
+- Package version: 1.0.5
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 For more information, please visit [https://docs.cashfree.com](https://docs.cashfree.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -91,15 +91,17 @@
 with cashfree_lrs_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = cashfree_lrs_client.LrsApi(api_client)
     files = None # List[bytearray] | Upload multiple document at a time. Accepted file type - .pdf. Maximum file size - 20 MB
 
     try:
         # Upload Documents in Bulk
-        api_instance.bulk_documents_upload(files)
+        api_response = api_instance.bulk_documents_upload(files)
+        print("The response of LrsApi->bulk_documents_upload:\n")
+        pprint(api_response)
     except ApiException as e:
         print("Exception when calling LrsApi->bulk_documents_upload: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
```

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/__init__.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 # flake8: noqa
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.4
+    The version of the OpenAPI document: 1.0.5
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-__version__ = "1.0.4"
+__version__ = "1.0.5"
 
 # import apis into sdk package
 from cashfree_lrs_client.api.lrs_api import LrsApi
 
 # import ApiClient
+from cashfree_lrs_client.api_response import ApiResponse
 from cashfree_lrs_client.api_client import ApiClient
 from cashfree_lrs_client.configuration import Configuration
 from cashfree_lrs_client.exceptions import OpenApiException
 from cashfree_lrs_client.exceptions import ApiTypeError
 from cashfree_lrs_client.exceptions import ApiValueError
 from cashfree_lrs_client.exceptions import ApiKeyError
 from cashfree_lrs_client.exceptions import ApiAttributeError
```

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/api/default_api.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/api/lrs_api.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/api/lrs_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.4
+    The version of the OpenAPI document: 1.0.5
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -28,14 +28,15 @@
 from cashfree_lrs_client.models.create_order_response import CreateOrderResponse
 from cashfree_lrs_client.models.create_remitter_request import CreateRemitterRequest
 from cashfree_lrs_client.models.fetch_forex_rate_request import FetchForexRateRequest
 from cashfree_lrs_client.models.setup_webhooks_request import SetupWebhooksRequest
 from cashfree_lrs_client.models.success_message import SuccessMessage
 
 from cashfree_lrs_client.api_client import ApiClient
+from cashfree_lrs_client.api_response import ApiResponse
 from cashfree_lrs_client.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class LrsApi(object):
@@ -47,79 +48,78 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def bulk_documents_upload(self, files : Annotated[conlist(Union[StrictBytes, StrictStr]), Field(..., description="Upload multiple document at a time. Accepted file type - .pdf. Maximum file size - 20 MB")], **kwargs) -> None:  # noqa: E501
+    def bulk_documents_upload(self, files : Annotated[conlist(Union[StrictBytes, StrictStr]), Field(..., description="Upload multiple document at a time. Accepted file type - .pdf. Maximum file size - 20 MB")], **kwargs) -> object:  # noqa: E501
         """Upload Documents in Bulk  # noqa: E501
 
         Use this API to Upload documents before Order creation  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.bulk_documents_upload(files, async_req=True)
         >>> result = thread.get()
 
         :param files: Upload multiple document at a time. Accepted file type - .pdf. Maximum file size - 20 MB (required)
         :type files: List[bytearray]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: object
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the bulk_documents_upload_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.bulk_documents_upload_with_http_info(files, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def bulk_documents_upload_with_http_info(self, files : Annotated[conlist(Union[StrictBytes, StrictStr]), Field(..., description="Upload multiple document at a time. Accepted file type - .pdf. Maximum file size - 20 MB")], **kwargs):  # noqa: E501
+    def bulk_documents_upload_with_http_info(self, files : Annotated[conlist(Union[StrictBytes, StrictStr]), Field(..., description="Upload multiple document at a time. Accepted file type - .pdf. Maximum file size - 20 MB")], **kwargs) -> ApiResponse:  # noqa: E501
         """Upload Documents in Bulk  # noqa: E501
 
         Use this API to Upload documents before Order creation  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.bulk_documents_upload_with_http_info(files, async_req=True)
         >>> result = thread.get()
 
         :param files: Upload multiple document at a time. Accepted file type - .pdf. Maximum file size - 20 MB (required)
         :type files: List[bytearray]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'files'
         ]
@@ -173,15 +173,18 @@
                 ['multipart/form-data']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['X-Client-ID', 'X-Client-Secret', 'X-API-Version']  # noqa: E501
 
-        _response_types_map = {}
+        _response_types_map = {
+            '200': "object",
+            '413': "Error",
+        }
 
         return self.api_client.call_api(
             '/orders/documents/upload', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
@@ -207,52 +210,51 @@
         >>> thread = api.create_beneficiary(create_beneficiary_request, async_req=True)
         >>> result = thread.get()
 
         :param create_beneficiary_request:
         :type create_beneficiary_request: CreateBeneficiaryRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: SuccessMessage
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the create_beneficiary_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.create_beneficiary_with_http_info(create_beneficiary_request, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_beneficiary_with_http_info(self, create_beneficiary_request : Optional[CreateBeneficiaryRequest] = None, **kwargs):  # noqa: E501
+    def create_beneficiary_with_http_info(self, create_beneficiary_request : Optional[CreateBeneficiaryRequest] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Create Beneficiary  # noqa: E501
 
         Use this API to create beneficiaries with Cashfree Payments from your backend.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_beneficiary_with_http_info(create_beneficiary_request, async_req=True)
         >>> result = thread.get()
 
         :param create_beneficiary_request:
         :type create_beneficiary_request: CreateBeneficiaryRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -355,52 +357,51 @@
         >>> thread = api.create_order(create_order_request, async_req=True)
         >>> result = thread.get()
 
         :param create_order_request:
         :type create_order_request: CreateOrderRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: CreateOrderResponse
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the create_order_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.create_order_with_http_info(create_order_request, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_order_with_http_info(self, create_order_request : Optional[CreateOrderRequest] = None, **kwargs):  # noqa: E501
+    def create_order_with_http_info(self, create_order_request : Optional[CreateOrderRequest] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Create LRS Order  # noqa: E501
 
         Use this API to create orders with Cashfree Payments.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_order_with_http_info(create_order_request, async_req=True)
         >>> result = thread.get()
 
         :param create_order_request:
         :type create_order_request: CreateOrderRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -504,52 +505,51 @@
         >>> thread = api.create_remitter(create_remitter_request, async_req=True)
         >>> result = thread.get()
 
         :param create_remitter_request:
         :type create_remitter_request: CreateRemitterRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: SuccessMessage
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the create_remitter_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.create_remitter_with_http_info(create_remitter_request, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_remitter_with_http_info(self, create_remitter_request : Optional[CreateRemitterRequest] = None, **kwargs):  # noqa: E501
+    def create_remitter_with_http_info(self, create_remitter_request : Optional[CreateRemitterRequest] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Create Remitter  # noqa: E501
 
         Use this API to create remmiter account with Cashfree Payments for LRS transactions.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_remitter_with_http_info(create_remitter_request, async_req=True)
         >>> result = thread.get()
 
         :param create_remitter_request:
         :type create_remitter_request: CreateRemitterRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -652,52 +652,51 @@
         >>> thread = api.fetch_forex_rate(fetch_forex_rate_request, async_req=True)
         >>> result = thread.get()
 
         :param fetch_forex_rate_request: 
         :type fetch_forex_rate_request: FetchForexRateRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the fetch_forex_rate_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.fetch_forex_rate_with_http_info(fetch_forex_rate_request, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def fetch_forex_rate_with_http_info(self, fetch_forex_rate_request : Optional[FetchForexRateRequest] = None, **kwargs):  # noqa: E501
+    def fetch_forex_rate_with_http_info(self, fetch_forex_rate_request : Optional[FetchForexRateRequest] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Fetch FX Rate  # noqa: E501
 
         Use this API to get the foreign exchange rate.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.fetch_forex_rate_with_http_info(fetch_forex_rate_request, async_req=True)
         >>> result = thread.get()
 
         :param fetch_forex_rate_request: 
         :type fetch_forex_rate_request: FetchForexRateRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -797,52 +796,51 @@
         >>> thread = api.process_order(order_id, async_req=True)
         >>> result = thread.get()
 
         :param order_id: The subject Order ID (required)
         :type order_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the process_order_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.process_order_with_http_info(order_id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def process_order_with_http_info(self, order_id : Annotated[StrictStr, Field(..., description="The subject Order ID")], **kwargs):  # noqa: E501
+    def process_order_with_http_info(self, order_id : Annotated[StrictStr, Field(..., description="The subject Order ID")], **kwargs) -> ApiResponse:  # noqa: E501
         """Process Order  # noqa: E501
 
         Use this API to process an order.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.process_order_with_http_info(order_id, async_req=True)
         >>> result = thread.get()
 
         :param order_id: The subject Order ID (required)
         :type order_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -931,52 +929,51 @@
         >>> thread = api.setup_webhooks(setup_webhooks_request, async_req=True)
         >>> result = thread.get()
 
         :param setup_webhooks_request: 
         :type setup_webhooks_request: SetupWebhooksRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: SuccessMessage
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the setup_webhooks_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.setup_webhooks_with_http_info(setup_webhooks_request, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def setup_webhooks_with_http_info(self, setup_webhooks_request : Optional[SetupWebhooksRequest] = None, **kwargs):  # noqa: E501
+    def setup_webhooks_with_http_info(self, setup_webhooks_request : Optional[SetupWebhooksRequest] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Setup Webhooks  # noqa: E501
 
         Use this API to configure webhook URLs to receive updates about payments, refunds, and orders.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.setup_webhooks_with_http_info(setup_webhooks_request, async_req=True)
         >>> result = thread.get()
 
         :param setup_webhooks_request: 
         :type setup_webhooks_request: SetupWebhooksRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -1080,32 +1077,30 @@
 
         :param order_id: The subject Order ID (required)
         :type order_id: str
         :param files: Upload multiple document at a time. Accepted file type - .pdf. Maximum file size - 20 MB (required)
         :type files: List[bytearray]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: object
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the upload_documents_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.upload_documents_with_http_info(order_id, files, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def upload_documents_with_http_info(self, order_id : Annotated[StrictStr, Field(..., description="The subject Order ID")], files : Annotated[conlist(Union[StrictBytes, StrictStr]), Field(..., description="Upload multiple document at a time. Accepted file type - .pdf. Maximum file size - 20 MB")], **kwargs):  # noqa: E501
+    def upload_documents_with_http_info(self, order_id : Annotated[StrictStr, Field(..., description="The subject Order ID")], files : Annotated[conlist(Union[StrictBytes, StrictStr]), Field(..., description="Upload multiple document at a time. Accepted file type - .pdf. Maximum file size - 20 MB")], **kwargs) -> ApiResponse:  # noqa: E501
         """Upload Documents  # noqa: E501
 
         Use this API to Upload documents on your Order ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.upload_documents_with_http_info(order_id, files, async_req=True)
@@ -1113,21 +1108,22 @@
 
         :param order_id: The subject Order ID (required)
         :type order_id: str
         :param files: Upload multiple document at a time. Accepted file type - .pdf. Maximum file size - 20 MB (required)
         :type files: List[bytearray]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
```

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/api_client.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.4
+    The version of the OpenAPI document: 1.0.5
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -22,14 +22,15 @@
 import os
 import re
 import tempfile
 
 from urllib.parse import quote
 
 from cashfree_lrs_client.configuration import Configuration
+from cashfree_lrs_client.api_response import ApiResponse
 import cashfree_lrs_client.models
 from cashfree_lrs_client import rest
 from cashfree_lrs_client.exceptions import ApiValueError, ApiException
 
 
 class ApiClient(object):
     """Generic API client for OpenAPI client library builds.
@@ -72,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.4/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.5/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
@@ -218,44 +219,44 @@
         except ApiException as e:
             if e.body:
                 e.body = e.body.decode('utf-8')
             raise e
 
         self.last_response = response_data
 
-        return_data = response_data
-
-        if not _preload_content:
-            return return_data
-
-        response_type = response_types_map.get(str(response_data.status), None)
-
-        if response_type == "bytearray":
-            response_data.data = response_data.data
-        else:
-            match = None
-            content_type = response_data.getheader('content-type')
-            if content_type is not None:
-                match = re.search(r"charset=([a-zA-Z\-\d]+)[\s;]?", content_type)
-            encoding = match.group(1) if match else "utf-8"
-            response_data.data = response_data.data.decode(encoding)
-
-        # deserialize response data
-        if response_type == "bytearray":
-            return_data = response_data.data
-        elif response_type:
-            return_data = self.deserialize(response_data, response_type)
-        else:
-            return_data = None
+        return_data = None # assuming derialization is not needed
+        # data needs deserialization or returns HTTP data (deserialized) only
+        if _preload_content or _return_http_data_only:
+          response_type = response_types_map.get(str(response_data.status), None)
+
+          if response_type == "bytearray":
+              response_data.data = response_data.data
+          else:
+              match = None
+              content_type = response_data.getheader('content-type')
+              if content_type is not None:
+                  match = re.search(r"charset=([a-zA-Z\-\d]+)[\s;]?", content_type)
+              encoding = match.group(1) if match else "utf-8"
+              response_data.data = response_data.data.decode(encoding)
+
+          # deserialize response data
+          if response_type == "bytearray":
+              return_data = response_data.data
+          elif response_type:
+              return_data = self.deserialize(response_data, response_type)
+          else:
+              return_data = None
 
         if _return_http_data_only:
-            return (return_data)
+            return return_data
         else:
-            return (return_data, response_data.status,
-                    response_data.getheaders())
+            return ApiResponse(status_code = response_data.status,
+                           data = return_data,
+                           headers = response_data.getheaders(),
+                           raw_data = response_data.data)
 
     def sanitize_for_serialization(self, obj):
         """Builds a JSON POST object.
 
         If obj is None, return None.
         If obj is str, int, long, float, bool, return directly.
         If obj is datetime.datetime, datetime.date
@@ -355,16 +356,16 @@
             return self.__deserialize_model(data, klass)
 
     def call_api(self, resource_path, method,
                  path_params=None, query_params=None, header_params=None,
                  body=None, post_params=None, files=None,
                  response_types_map=None, auth_settings=None,
                  async_req=None, _return_http_data_only=None,
-                 collection_formats=None,_preload_content=True,
-                  _request_timeout=None, _host=None, _request_auth=None):
+                 collection_formats=None, _preload_content=True,
+                 _request_timeout=None, _host=None, _request_auth=None):
         """Makes the HTTP request (synchronous) and returns deserialized data.
 
         To make an async_req request, set the async_req parameter.
 
         :param resource_path: Path to method endpoint.
         :param method: Method to call.
         :param path_params: Path parameters in the url.
@@ -375,21 +376,22 @@
         :param post_params dict: Request post form parameters,
             for `application/x-www-form-urlencoded`, `multipart/form-data`.
         :param auth_settings list: Auth Settings names for the request.
         :param response: Response data type.
         :param files dict: key -> filename, value -> filepath,
             for `multipart/form-data`.
         :param async_req bool: execute request asynchronously
-        :param _return_http_data_only: response data without head status code
-                                       and headers
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :param collection_formats: dict of collection formats for path, query,
             header, and post parameters.
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
```

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/apis/path_to_api.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/apis/tags/lrs_api.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/apis/tags/lrs_api.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/configuration.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.4
+    The version of the OpenAPI document: 1.0.5
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -407,16 +407,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0.4\n"\
-               "SDK Package Version: 1.0.4".\
+               "Version of the API: 1.0.5\n"\
+               "SDK Package Version: 1.0.5".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/docs/CreateBeneficiaryRequest.md` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/CreateBeneficiaryRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/docs/CreateOrderRequest.md` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/CreateOrderRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/docs/CreateOrderResponse.md` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/CreateOrderResponse.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/docs/CreateRemitterRequest.md` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/CreateRemitterRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/docs/Error.md` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/Error.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/docs/FetchForexRateRequest.md` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/FetchForexRateRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/docs/LrsApi.md` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/LrsApi.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/docs/SetupWebhooksRequest.md` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/SetupWebhooksRequest.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/docs/SuccessMessage.md` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/docs/SuccessMessage.md`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/exceptions.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.4
+    The version of the OpenAPI document: 1.0.5
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/amount.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/amount.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/amount.pyi` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/amount.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/create_beneficiary_request.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_beneficiary_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/create_beneficiary_request.pyi` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_beneficiary_request.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/create_order_request.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_order_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/create_order_request.pyi` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_order_request.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/create_order_response.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_order_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/create_order_response.pyi` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_order_response.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/create_remitter_request.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_remitter_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/create_remitter_request.pyi` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/create_remitter_request.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/currency.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/currency.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/currency.pyi` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/currency.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/error.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/error.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/error.pyi` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/error.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/fetch_forex_rate_request.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/fetch_forex_rate_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/fetch_forex_rate_request.pyi` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/fetch_forex_rate_request.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/purpose.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/purpose.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/purpose.pyi` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/purpose.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/setup_webhooks_request.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/setup_webhooks_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/setup_webhooks_request.pyi` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/setup_webhooks_request.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/success_message.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/success_message.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/model/success_message.pyi` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/model/success_message.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/__init__.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.4
+    The version of the OpenAPI document: 1.0.5
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/country.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/country.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.4
+    The version of the OpenAPI document: 1.0.5
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/create_beneficiary200_response.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/create_beneficiary200_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/create_beneficiary_request.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/create_beneficiary_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.4
+    The version of the OpenAPI document: 1.0.5
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/create_order_request.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/create_order_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.4
+    The version of the OpenAPI document: 1.0.5
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/create_order_response.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/create_order_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.4
+    The version of the OpenAPI document: 1.0.5
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/create_remitter200_response.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/create_remitter200_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/create_remitter_request.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/create_remitter_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.4
+    The version of the OpenAPI document: 1.0.5
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/currency.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/currency.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.4
+    The version of the OpenAPI document: 1.0.5
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/error.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/error.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.4
+    The version of the OpenAPI document: 1.0.5
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/fetch_forex_rate_request.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/fetch_forex_rate_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.4
+    The version of the OpenAPI document: 1.0.5
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/order_response.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/order_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/purpose.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/purpose.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.4
+    The version of the OpenAPI document: 1.0.5
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/setup_webhooks200_response.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/setup_webhooks200_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/setup_webhooks_request.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/setup_webhooks_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.4
+    The version of the OpenAPI document: 1.0.5
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/models/success_message.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/models/success_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.4
+    The version of the OpenAPI document: 1.0.5
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/__init__.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/beneficiaries/post.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/beneficiaries/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/beneficiaries/post.pyi` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/beneficiaries/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/fx_rate_details/post.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/fx_rate_details/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/fx_rate_details/post.pyi` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/fx_rate_details/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/orders/post.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/orders/post.pyi` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/orders_documents_upload/post.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_documents_upload/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/orders_documents_upload/post.pyi` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_documents_upload/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.pyi` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_order_id_documents_upload/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/orders_order_id_process/post.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_order_id_process/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/orders_order_id_process/post.pyi` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/orders_order_id_process/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/remitters/post.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/remitters/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/remitters/post.pyi` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/remitters/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/webhooks/post.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/webhooks/post.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/paths/webhooks/post.pyi` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/paths/webhooks/post.pyi`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/rest.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Cashfree LRS
 
     CashFree LRS APIs (v2)  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.4
+    The version of the OpenAPI document: 1.0.5
     Contact: nextgenapi@cashfree.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/schemas.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/schemas.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/test/test_create_beneficiary_request.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_create_beneficiary_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/test/test_create_order_request.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_create_order_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/test/test_create_order_response.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_create_order_response.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/test/test_create_remitter_request.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_create_remitter_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/test/test_currency.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_currency.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/test/test_error.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_error.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/test/test_fetch_forex_rate_request.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_fetch_forex_rate_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/test/test_lrs_api.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_lrs_api.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/test/test_purpose.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_purpose.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/test/test_setup_webhooks_request.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_setup_webhooks_request.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/cashfree_lrs_client/test/test_success_message.py` & `cashfree_lrs_client-1.0.5/cashfree_lrs_client/test/test_success_message.py`

 * *Files identical despite different names*

### Comparing `cashfree_lrs_client-1.0.4/pyproject.toml` & `cashfree_lrs_client-1.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cashfree_lrs_client"
-version = "1.0.4"
+version = "1.0.5"
 description = "Cashfree LRS"
 authors = ["CashFree Care <nextgenapi@cashfree.com>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_REPO_ID/GIT_USER_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Cashfree LRS"]
```

### Comparing `cashfree_lrs_client-1.0.4/PKG-INFO` & `cashfree_lrs_client-1.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashfree-lrs-client
-Version: 1.0.4
+Version: 1.0.5
 Summary: Cashfree LRS
 Home-page: https://github.com/GIT_REPO_ID/GIT_USER_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,Cashfree LRS
 Author: CashFree Care
 Author-email: nextgenapi@cashfree.com
 Requires-Python: >=3.7,<4.0
@@ -23,16 +23,16 @@
 Description-Content-Type: text/markdown
 
 # cashfree-lrs-client
 CashFree LRS APIs (v2)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.4
-- Package version: 1.0.4
+- API version: 1.0.5
+- Package version: 1.0.5
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 For more information, please visit [https://docs.cashfree.com](https://docs.cashfree.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -115,15 +115,17 @@
 with cashfree_lrs_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = cashfree_lrs_client.LrsApi(api_client)
     files = None # List[bytearray] | Upload multiple document at a time. Accepted file type - .pdf. Maximum file size - 20 MB
 
     try:
         # Upload Documents in Bulk
-        api_instance.bulk_documents_upload(files)
+        api_response = api_instance.bulk_documents_upload(files)
+        print("The response of LrsApi->bulk_documents_upload:\n")
+        pprint(api_response)
     except ApiException as e:
         print("Exception when calling LrsApi->bulk_documents_upload: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
```

