# Comparing `tmp/fastel-2.7.8.tar.gz` & `tmp/fastel-2.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastel-2.7.8.tar", max compression
+gzip compressed data, was "fastel-2.7.9.tar", max compression
```

## Comparing `fastel-2.7.8.tar` & `fastel-2.7.9.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0     1077 2022-11-25 09:09:26.372462 fastel-2.7.8/LICENSE
--rw-r--r--   0        0        0      695 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/__init__.py
--rw-r--r--   0        0        0        0 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/ads/__init__.py
--rw-r--r--   0        0        0        0 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/ads/facebook/__init__.py
--rw-r--r--   0        0        0     4543 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/ads/facebook/conversion.py
--rw-r--r--   0        0        0     1459 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/auth/__init__.py
--rw-r--r--   0        0        0    11636 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/authorizers.py
--rw-r--r--   0        0        0      152 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/cart/__init__.py
--rw-r--r--   0        0        0     8188 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/cart/base.py
--rw-r--r--   0        0        0    10098 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/cart/cart.py
--rw-r--r--   0        0        0      165 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/cart/collections.py
--rw-r--r--   0        0        0     6890 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/cart/datastructures.py
--rw-r--r--   0        0        0      494 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/cart/exceptions.py
--rw-r--r--   0        0        0     3750 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/cart/product_item.py
--rw-r--r--   0        0        0     1900 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/cart/product_items.py
--rw-r--r--   0        0        0     1715 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/cart/utils.py
--rw-r--r--   0        0        0     2646 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/collections.py
--rw-r--r--   0        0        0     5859 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/config.py
--rw-r--r--   0        0        0      670 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/exceptions.py
--rw-r--r--   0        0        0      634 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/jwt/__init__.py
--rw-r--r--   0        0        0      835 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/jwt/decode_static.py
--rw-r--r--   0        0        0      986 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/jwt/jwt_encoder.py
--rw-r--r--   0        0        0     3372 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/jwt/jwt_payload.py
--rw-r--r--   0        0        0     1571 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/jwt/kms_encode.py
--rw-r--r--   0        0        0     1219 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/jwt/pem_coder.py
--rw-r--r--   0        0        0      114 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/logistics/__init__.py
--rw-r--r--   0        0        0     1083 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/logistics/common/__init__.py
--rw-r--r--   0        0        0    27219 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/logistics/common/helpers.py
--rw-r--r--   0        0        0      956 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/logistics/common/models/__init__.py
--rw-r--r--   0        0        0        0 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/logistics/ecpay/__init__.py
--rw-r--r--   0        0        0     4842 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/logistics/ecpay/gateway.py
--rw-r--r--   0        0        0     3833 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/logistics/ecpay/models/__init__.py
--rw-r--r--   0        0        0      459 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/logistics/sf/__init__.py
--rw-r--r--   0        0        0     8545 2022-11-25 09:09:26.372462 fastel-2.7.8/fastel/logistics/sf/cryptor.py
--rw-r--r--   0        0        0     3487 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/logistics/sf/gateway.py
--rw-r--r--   0        0        0      729 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/logistics/sf/ierror.py
--rw-r--r--   0        0        0     2871 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/logistics/sf/models/__init__.py
--rw-r--r--   0        0        0       55 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/logistics/tcat/__init__.py
--rw-r--r--   0        0        0     5234 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/logistics/tcat/models.py
--rw-r--r--   0        0        0     2500 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/logistics/tcat/tcat.py
--rw-r--r--   0        0        0     2102 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/logistics/trackingmore/__init__.py
--rw-r--r--   0        0        0       70 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/notif/__init__.py
--rw-r--r--   0        0        0     4442 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/notif/notifier.py
--rw-r--r--   0        0        0       10 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/__init__.py
--rw-r--r--   0        0        0        9 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/common/__init__.py
--rw-r--r--   0        0        0    40035 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/common/helpers.py
--rw-r--r--   0        0        0        9 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/common/models/__init__.py
--rw-r--r--   0        0        0      825 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/common/models/callback.py
--rw-r--r--   0        0        0      363 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/common/models/invoice.py
--rw-r--r--   0        0        0     1419 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/common/models/order.py
--rw-r--r--   0        0        0     4682 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/cryptors.py
--rw-r--r--   0        0        0     6734 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/ecpay/__init__.py
--rw-r--r--   0        0        0     3651 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/ecpay/gateway.py
--rw-r--r--   0        0        0     6804 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/ecpay/invoice.py
--rw-r--r--   0        0        0        8 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/ecpay/models/__init__.py
--rw-r--r--   0        0        0     2250 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/ecpay/models/checkout.py
--rw-r--r--   0        0        0     2213 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/ecpay/models/invoice.py
--rw-r--r--   0        0        0      240 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/ecpay/models/refund.py
--rw-r--r--   0        0        0        0 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/linepay/__init__.py
--rw-r--r--   0        0        0      473 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/linepay/exceptions.py
--rw-r--r--   0        0        0     4045 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/linepay/gateway.py
--rw-r--r--   0        0        0       10 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/linepay/models/__init__.py
--rw-r--r--   0        0        0     1636 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/linepay/models/checkout.py
--rw-r--r--   0        0        0        8 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/neweb/__init__.py
--rw-r--r--   0        0        0     3931 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/neweb/gateway.py
--rw-r--r--   0        0        0        8 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/neweb/models/__init__.py
--rw-r--r--   0        0        0     4036 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/neweb/models/callback.py
--rw-r--r--   0        0        0     1152 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/neweb/models/checkout.py
--rw-r--r--   0        0        0     1646 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/neweb/models/invoice.py
--rw-r--r--   0        0        0      255 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/neweb/models/refund.py
--rw-r--r--   0        0        0      447 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/payment/utils.py
--rw-r--r--   0        0        0        0 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/py.typed
--rw-r--r--   0        0        0      364 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/social/__init__.py
--rw-r--r--   0        0        0     1071 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/social/apple.py
--rw-r--r--   0        0        0     2486 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/social/facebook.py
--rw-r--r--   0        0        0     2746 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/social/google.py
--rw-r--r--   0        0        0     1713 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/social/line.py
--rw-r--r--   0        0        0       29 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/test.py
--rw-r--r--   0        0        0      228 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/utils/__init__.py
--rw-r--r--   0        0        0      852 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/utils/debug_logger.py
--rw-r--r--   0        0        0      618 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/utils/doc.py
--rw-r--r--   0        0        0      653 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/utils/password.py
--rw-r--r--   0        0        0     1458 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/utils/requests.py
--rw-r--r--   0        0        0      354 2022-11-25 09:09:26.376462 fastel-2.7.8/fastel/utils/skip_warmup_call.py
--rw-r--r--   0        0        0      862 2022-11-25 09:09:26.376462 fastel-2.7.8/pyproject.toml
--rw-r--r--   0        0        0     1611 2022-11-25 09:10:42.827336 fastel-2.7.8/setup.py
--rw-r--r--   0        0        0      978 2022-11-25 09:10:42.827734 fastel-2.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1077 2022-11-25 09:30:04.160811 fastel-2.7.9/LICENSE
+-rw-r--r--   0        0        0      695 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/ads/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/ads/facebook/__init__.py
+-rw-r--r--   0        0        0     4543 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/ads/facebook/conversion.py
+-rw-r--r--   0        0        0     1459 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/auth/__init__.py
+-rw-r--r--   0        0        0    11636 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/authorizers.py
+-rw-r--r--   0        0        0      152 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/cart/__init__.py
+-rw-r--r--   0        0        0     8188 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/cart/base.py
+-rw-r--r--   0        0        0    10098 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/cart/cart.py
+-rw-r--r--   0        0        0      165 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/cart/collections.py
+-rw-r--r--   0        0        0     6890 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/cart/datastructures.py
+-rw-r--r--   0        0        0      494 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/cart/exceptions.py
+-rw-r--r--   0        0        0     3750 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/cart/product_item.py
+-rw-r--r--   0        0        0     1900 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/cart/product_items.py
+-rw-r--r--   0        0        0     1715 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/cart/utils.py
+-rw-r--r--   0        0        0     2646 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/collections.py
+-rw-r--r--   0        0        0     5859 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/config.py
+-rw-r--r--   0        0        0      670 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/exceptions.py
+-rw-r--r--   0        0        0      634 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/jwt/__init__.py
+-rw-r--r--   0        0        0      835 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/jwt/decode_static.py
+-rw-r--r--   0        0        0      986 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/jwt/jwt_encoder.py
+-rw-r--r--   0        0        0     3372 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/jwt/jwt_payload.py
+-rw-r--r--   0        0        0     1571 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/jwt/kms_encode.py
+-rw-r--r--   0        0        0     1219 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/jwt/pem_coder.py
+-rw-r--r--   0        0        0      114 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/logistics/__init__.py
+-rw-r--r--   0        0        0     1083 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/logistics/common/__init__.py
+-rw-r--r--   0        0        0    27219 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/logistics/common/helpers.py
+-rw-r--r--   0        0        0      956 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/logistics/common/models/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/logistics/ecpay/__init__.py
+-rw-r--r--   0        0        0     4842 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/logistics/ecpay/gateway.py
+-rw-r--r--   0        0        0     3833 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/logistics/ecpay/models/__init__.py
+-rw-r--r--   0        0        0      459 2022-11-25 09:30:04.160811 fastel-2.7.9/fastel/logistics/sf/__init__.py
+-rw-r--r--   0        0        0     8545 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/logistics/sf/cryptor.py
+-rw-r--r--   0        0        0     3487 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/logistics/sf/gateway.py
+-rw-r--r--   0        0        0      729 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/logistics/sf/ierror.py
+-rw-r--r--   0        0        0     2871 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/logistics/sf/models/__init__.py
+-rw-r--r--   0        0        0       55 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/logistics/tcat/__init__.py
+-rw-r--r--   0        0        0     5234 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/logistics/tcat/models.py
+-rw-r--r--   0        0        0     2500 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/logistics/tcat/tcat.py
+-rw-r--r--   0        0        0     2102 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/logistics/trackingmore/__init__.py
+-rw-r--r--   0        0        0       70 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/notif/__init__.py
+-rw-r--r--   0        0        0     4442 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/notif/notifier.py
+-rw-r--r--   0        0        0       10 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/__init__.py
+-rw-r--r--   0        0        0        9 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/common/__init__.py
+-rw-r--r--   0        0        0    40035 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/common/helpers.py
+-rw-r--r--   0        0        0        9 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/common/models/__init__.py
+-rw-r--r--   0        0        0      825 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/common/models/callback.py
+-rw-r--r--   0        0        0      363 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/common/models/invoice.py
+-rw-r--r--   0        0        0     1419 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/common/models/order.py
+-rw-r--r--   0        0        0     4682 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/cryptors.py
+-rw-r--r--   0        0        0     6734 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/ecpay/__init__.py
+-rw-r--r--   0        0        0     3651 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/ecpay/gateway.py
+-rw-r--r--   0        0        0     6804 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/ecpay/invoice.py
+-rw-r--r--   0        0        0        8 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/ecpay/models/__init__.py
+-rw-r--r--   0        0        0     2250 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/ecpay/models/checkout.py
+-rw-r--r--   0        0        0     2213 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/ecpay/models/invoice.py
+-rw-r--r--   0        0        0      240 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/ecpay/models/refund.py
+-rw-r--r--   0        0        0        0 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/linepay/__init__.py
+-rw-r--r--   0        0        0      473 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/linepay/exceptions.py
+-rw-r--r--   0        0        0     4045 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/linepay/gateway.py
+-rw-r--r--   0        0        0       10 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/linepay/models/__init__.py
+-rw-r--r--   0        0        0     1636 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/linepay/models/checkout.py
+-rw-r--r--   0        0        0        8 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/neweb/__init__.py
+-rw-r--r--   0        0        0     3931 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/neweb/gateway.py
+-rw-r--r--   0        0        0        8 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/neweb/models/__init__.py
+-rw-r--r--   0        0        0     4036 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/neweb/models/callback.py
+-rw-r--r--   0        0        0     1152 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/neweb/models/checkout.py
+-rw-r--r--   0        0        0     1646 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/neweb/models/invoice.py
+-rw-r--r--   0        0        0      255 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/neweb/models/refund.py
+-rw-r--r--   0        0        0      517 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/payment/utils.py
+-rw-r--r--   0        0        0        0 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/py.typed
+-rw-r--r--   0        0        0      364 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/social/__init__.py
+-rw-r--r--   0        0        0     1071 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/social/apple.py
+-rw-r--r--   0        0        0     2486 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/social/facebook.py
+-rw-r--r--   0        0        0     2746 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/social/google.py
+-rw-r--r--   0        0        0     1713 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/social/line.py
+-rw-r--r--   0        0        0       29 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/test.py
+-rw-r--r--   0        0        0      228 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/utils/__init__.py
+-rw-r--r--   0        0        0      852 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/utils/debug_logger.py
+-rw-r--r--   0        0        0      618 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/utils/doc.py
+-rw-r--r--   0        0        0      653 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/utils/password.py
+-rw-r--r--   0        0        0     1458 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/utils/requests.py
+-rw-r--r--   0        0        0      354 2022-11-25 09:30:04.164811 fastel-2.7.9/fastel/utils/skip_warmup_call.py
+-rw-r--r--   0        0        0      862 2022-11-25 09:30:04.164811 fastel-2.7.9/pyproject.toml
+-rw-r--r--   0        0        0     1611 2022-11-25 09:31:09.656827 fastel-2.7.9/setup.py
+-rw-r--r--   0        0        0      978 2022-11-25 09:31:09.657109 fastel-2.7.9/PKG-INFO
```

### Comparing `fastel-2.7.8/LICENSE` & `fastel-2.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/__init__.py` & `fastel-2.7.9/fastel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     StaticJWTAuth,
     StaticSecretAuth,
 )
 from fastel.cart.exceptions import CartException, cart_exception_handler
 from fastel.collections import set_collections
 from fastel.exceptions import APIException, api_exception_handler
 
-__version__ = "2.7.8"
+__version__ = "2.7.9"
 __all__ = [
     "APIException",
     "api_exception_handler",
     "ClientIdAuth",
     "ClientSecretAuth",
     "Credential",
     "JWBaseAuth",
```

### Comparing `fastel-2.7.8/fastel/ads/facebook/conversion.py` & `fastel-2.7.9/fastel/ads/facebook/conversion.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/auth/__init__.py` & `fastel-2.7.9/fastel/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/authorizers.py` & `fastel-2.7.9/fastel/authorizers.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/cart/base.py` & `fastel-2.7.9/fastel/cart/base.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/cart/cart.py` & `fastel-2.7.9/fastel/cart/cart.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/cart/datastructures.py` & `fastel-2.7.9/fastel/cart/datastructures.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/cart/product_item.py` & `fastel-2.7.9/fastel/cart/product_item.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/cart/product_items.py` & `fastel-2.7.9/fastel/cart/product_items.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/cart/utils.py` & `fastel-2.7.9/fastel/cart/utils.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/collections.py` & `fastel-2.7.9/fastel/collections.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/config.py` & `fastel-2.7.9/fastel/config.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/exceptions.py` & `fastel-2.7.9/fastel/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/jwt/__init__.py` & `fastel-2.7.9/fastel/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/jwt/decode_static.py` & `fastel-2.7.9/fastel/jwt/decode_static.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/jwt/jwt_encoder.py` & `fastel-2.7.9/fastel/jwt/jwt_encoder.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/jwt/jwt_payload.py` & `fastel-2.7.9/fastel/jwt/jwt_payload.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/jwt/kms_encode.py` & `fastel-2.7.9/fastel/jwt/kms_encode.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/jwt/pem_coder.py` & `fastel-2.7.9/fastel/jwt/pem_coder.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/logistics/common/__init__.py` & `fastel-2.7.9/fastel/logistics/common/__init__.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/logistics/common/helpers.py` & `fastel-2.7.9/fastel/logistics/common/helpers.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/logistics/common/models/__init__.py` & `fastel-2.7.9/fastel/logistics/common/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/logistics/ecpay/gateway.py` & `fastel-2.7.9/fastel/logistics/ecpay/gateway.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/logistics/ecpay/models/__init__.py` & `fastel-2.7.9/fastel/logistics/ecpay/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/logistics/sf/cryptor.py` & `fastel-2.7.9/fastel/logistics/sf/cryptor.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/logistics/sf/gateway.py` & `fastel-2.7.9/fastel/logistics/sf/gateway.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/logistics/sf/ierror.py` & `fastel-2.7.9/fastel/logistics/sf/ierror.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/logistics/sf/models/__init__.py` & `fastel-2.7.9/fastel/logistics/sf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/logistics/tcat/models.py` & `fastel-2.7.9/fastel/logistics/tcat/models.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/logistics/tcat/tcat.py` & `fastel-2.7.9/fastel/logistics/tcat/tcat.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/logistics/trackingmore/__init__.py` & `fastel-2.7.9/fastel/logistics/trackingmore/__init__.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/notif/notifier.py` & `fastel-2.7.9/fastel/notif/notifier.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/payment/common/helpers.py` & `fastel-2.7.9/fastel/payment/common/helpers.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/payment/common/models/callback.py` & `fastel-2.7.9/fastel/payment/common/models/callback.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/payment/common/models/order.py` & `fastel-2.7.9/fastel/payment/common/models/order.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/payment/cryptors.py` & `fastel-2.7.9/fastel/payment/cryptors.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/payment/ecpay/__init__.py` & `fastel-2.7.9/fastel/payment/ecpay/__init__.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/payment/ecpay/gateway.py` & `fastel-2.7.9/fastel/payment/ecpay/gateway.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/payment/ecpay/invoice.py` & `fastel-2.7.9/fastel/payment/ecpay/invoice.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/payment/ecpay/models/checkout.py` & `fastel-2.7.9/fastel/payment/ecpay/models/checkout.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/payment/ecpay/models/invoice.py` & `fastel-2.7.9/fastel/payment/ecpay/models/invoice.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/payment/linepay/gateway.py` & `fastel-2.7.9/fastel/payment/linepay/gateway.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/payment/linepay/models/checkout.py` & `fastel-2.7.9/fastel/payment/linepay/models/checkout.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/payment/neweb/gateway.py` & `fastel-2.7.9/fastel/payment/neweb/gateway.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/payment/neweb/models/callback.py` & `fastel-2.7.9/fastel/payment/neweb/models/callback.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/payment/neweb/models/checkout.py` & `fastel-2.7.9/fastel/payment/neweb/models/checkout.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/payment/neweb/models/invoice.py` & `fastel-2.7.9/fastel/payment/neweb/models/invoice.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/social/apple.py` & `fastel-2.7.9/fastel/social/apple.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/social/facebook.py` & `fastel-2.7.9/fastel/social/facebook.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/social/google.py` & `fastel-2.7.9/fastel/social/google.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/social/line.py` & `fastel-2.7.9/fastel/social/line.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/utils/debug_logger.py` & `fastel-2.7.9/fastel/utils/debug_logger.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/utils/doc.py` & `fastel-2.7.9/fastel/utils/doc.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/utils/password.py` & `fastel-2.7.9/fastel/utils/password.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/fastel/utils/requests.py` & `fastel-2.7.9/fastel/utils/requests.py`

 * *Files identical despite different names*

### Comparing `fastel-2.7.8/pyproject.toml` & `fastel-2.7.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastel"
-version = "2.7.8"
+version = "2.7.9"
 description = "RevtelTech Backend SDK"
 authors = ["Chien <a0186163@gmail.com>"]
 exclude = ["example/*"]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 fastapi = ">=0.63.0"
```

### Comparing `fastel-2.7.8/setup.py` & `fastel-2.7.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
  'pycrypto>=2.6.1,<3.0.0',
  'pydantic[email]>=1.8.2,<2.0.0',
  'pymongo>=3.12.0,<4.0.0',
  'pytz>=2022.1,<2023.0']
 
 setup_kwargs = {
     'name': 'fastel',
-    'version': '2.7.8',
+    'version': '2.7.9',
     'description': 'RevtelTech Backend SDK',
     'long_description': None,
     'author': 'Chien',
     'author_email': 'a0186163@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `fastel-2.7.8/PKG-INFO` & `fastel-2.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastel
-Version: 2.7.8
+Version: 2.7.9
 Summary: RevtelTech Backend SDK
 Author: Chien
 Author-email: a0186163@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
```

