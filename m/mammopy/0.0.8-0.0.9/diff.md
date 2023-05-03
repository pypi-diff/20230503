# Comparing `tmp/mammopy-0.0.8.tar.gz` & `tmp/mammopy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mammopy-0.0.8.tar", max compression
+gzip compressed data, was "mammopy-0.0.9.tar", max compression
```

## Comparing `mammopy-0.0.8.tar` & `mammopy-0.0.9.tar`

### file list

```diff
@@ -1,200 +1,187 @@
--rw-r--r--   0        0        0      260 2023-04-26 06:08:18.350875 mammopy-0.0.8/mammopy/__init__.py
--rw-r--r--   0        0        0  1842751 2023-03-22 12:02:48.321183 mammopy-0.0.8/mammopy/EE0B064D.jpg
--rw-r--r--   0        0        0     3368 2023-04-25 10:32:45.945031 mammopy-0.0.8/mammopy/examples_codes.ipynb
--rw-r--r--   0        0        0     9407 2023-04-25 08:57:54.514381 mammopy-0.0.8/mammopy/mammopy.py
--rw-r--r--   0        0        0      231 2023-04-25 10:57:41.217743 mammopy-0.0.8/mammopy/segmentation_models/__init__.py
--rw-r--r--   0        0        0      298 2023-03-15 07:44:18.000000 mammopy-0.0.8/mammopy/segmentation_models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      284 2023-03-15 07:44:18.000000 mammopy-0.0.8/mammopy/segmentation_models/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      347 2023-03-15 07:44:18.000000 mammopy-0.0.8/mammopy/segmentation_models/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      264 2023-04-25 10:02:24.145454 mammopy-0.0.8/mammopy/segmentation_models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      296 2023-03-22 11:45:31.970280 mammopy-0.0.8/mammopy/segmentation_models/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      250 2023-03-15 07:44:18.000000 mammopy-0.0.8/mammopy/segmentation_models/__pycache__/__version__.cpython-310.pyc
--rw-r--r--   0        0        0      239 2023-03-15 07:44:18.000000 mammopy-0.0.8/mammopy/segmentation_models/__pycache__/__version__.cpython-36.pyc
--rw-r--r--   0        0        0      232 2023-03-15 07:44:18.000000 mammopy-0.0.8/mammopy/segmentation_models/__pycache__/__version__.cpython-37.pyc
--rw-r--r--   0        0        0      250 2023-04-25 08:12:45.279552 mammopy-0.0.8/mammopy/segmentation_models/__pycache__/__version__.cpython-38.pyc
--rw-r--r--   0        0        0      248 2023-03-22 11:45:33.085944 mammopy-0.0.8/mammopy/segmentation_models/__pycache__/__version__.cpython-39.pyc
--rw-r--r--   0        0        0      148 2023-03-15 07:44:18.000000 mammopy-0.0.8/mammopy/segmentation_models/base/__init__.py
--rw-r--r--   0        0        0      330 2023-03-15 07:44:18.000000 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      304 2023-03-15 07:44:18.000000 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      312 2023-03-15 07:44:18.000000 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      330 2023-04-25 08:12:43.927739 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      328 2023-03-22 11:45:31.983165 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      881 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/heads.cpython-310.pyc
--rw-r--r--   0        0        0      845 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/heads.cpython-36.pyc
--rw-r--r--   0        0        0      855 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/heads.cpython-37.pyc
--rw-r--r--   0        0        0      879 2023-04-25 08:12:43.958739 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/heads.cpython-38.pyc
--rw-r--r--   0        0        0      877 2023-03-22 11:45:31.997169 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/heads.cpython-39.pyc
--rw-r--r--   0        0        0      940 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/initialization.cpython-310.pyc
--rw-r--r--   0        0        0      909 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/initialization.cpython-36.pyc
--rw-r--r--   0        0        0      919 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/initialization.cpython-37.pyc
--rw-r--r--   0        0        0      930 2023-04-25 08:12:43.939737 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/initialization.cpython-38.pyc
--rw-r--r--   0        0        0      928 2023-03-22 11:45:31.990419 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/initialization.cpython-39.pyc
--rw-r--r--   0        0        0     1630 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/model.cpython-310.pyc
--rw-r--r--   0        0        0     1558 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/model.cpython-36.pyc
--rw-r--r--   0        0        0     1566 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/model.cpython-37.pyc
--rw-r--r--   0        0        0     1599 2023-04-25 08:12:43.931739 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/model.cpython-38.pyc
--rw-r--r--   0        0        0     1618 2023-03-22 11:45:31.987385 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/model.cpython-39.pyc
--rw-r--r--   0        0        0     3963 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/modules.cpython-310.pyc
--rw-r--r--   0        0        0     4162 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/modules.cpython-36.pyc
--rw-r--r--   0        0        0     4024 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/modules.cpython-37.pyc
--rw-r--r--   0        0        0     3979 2023-04-25 08:12:43.949740 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/modules.cpython-38.pyc
--rw-r--r--   0        0        0     4003 2023-03-22 11:45:31.993781 mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/modules.cpython-39.pyc
--rw-r--r--   0        0        0      532 2023-03-15 07:44:18.000000 mammopy-0.0.8/mammopy/segmentation_models/base/heads.py
--rw-r--r--   0        0        0      848 2023-03-15 07:44:18.000000 mammopy-0.0.8/mammopy/segmentation_models/base/initialization.py
--rw-r--r--   0        0        0     1294 2023-03-15 07:44:18.000000 mammopy-0.0.8/mammopy/segmentation_models/base/model.py
--rw-r--r--   0        0        0     3561 2023-03-15 07:44:18.000000 mammopy-0.0.8/mammopy/segmentation_models/base/modules.py
--rw-r--r--   0        0        0     2341 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__init__.py
--rw-r--r--   0        0        0     2219 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2165 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0     2179 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0     2213 2023-04-25 08:12:43.961742 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2219 2023-03-22 11:45:32.000169 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1813 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_base.cpython-310.pyc
--rw-r--r--   0        0        0     1768 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_base.cpython-36.pyc
--rw-r--r--   0        0        0     1778 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_base.cpython-37.pyc
--rw-r--r--   0        0        0     1814 2023-04-25 08:12:44.602047 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_base.cpython-38.pyc
--rw-r--r--   0        0        0     1812 2023-03-22 11:45:32.684714 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_base.cpython-39.pyc
--rw-r--r--   0        0        0      572 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-310.pyc
--rw-r--r--   0        0        0      538 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-36.pyc
--rw-r--r--   0        0        0      546 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-37.pyc
--rw-r--r--   0        0        0      576 2023-04-25 08:12:45.212550 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-38.pyc
--rw-r--r--   0        0        0      568 2023-03-22 11:45:33.060100 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-39.pyc
--rw-r--r--   0        0        0     1399 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_utils.cpython-310.pyc
--rw-r--r--   0        0        0     1374 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_utils.cpython-36.pyc
--rw-r--r--   0        0        0     1361 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_utils.cpython-37.pyc
--rw-r--r--   0        0        0     1385 2023-04-25 08:12:44.613052 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_utils.cpython-38.pyc
--rw-r--r--   0        0        0     1385 2023-03-22 11:45:32.686716 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_utils.cpython-39.pyc
--rw-r--r--   0        0        0     4841 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/densenet.cpython-310.pyc
--rw-r--r--   0        0        0     4841 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/densenet.cpython-36.pyc
--rw-r--r--   0        0        0     4766 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/densenet.cpython-37.pyc
--rw-r--r--   0        0        0     4828 2023-04-25 08:12:44.655048 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/densenet.cpython-38.pyc
--rw-r--r--   0        0        0     4830 2023-03-22 11:45:32.699122 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/densenet.cpython-39.pyc
--rw-r--r--   0        0        0     4420 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/dpn.cpython-310.pyc
--rw-r--r--   0        0        0     4606 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/dpn.cpython-36.pyc
--rw-r--r--   0        0        0     4347 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/dpn.cpython-37.pyc
--rw-r--r--   0        0        0     4405 2023-04-25 08:12:44.624100 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/dpn.cpython-38.pyc
--rw-r--r--   0        0        0     4411 2023-03-22 11:45:32.691122 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/dpn.cpython-39.pyc
--rw-r--r--   0        0        0     4660 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/efficientnet.cpython-310.pyc
--rw-r--r--   0        0        0     4924 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/efficientnet.cpython-36.pyc
--rw-r--r--   0        0        0     4670 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/efficientnet.cpython-37.pyc
--rw-r--r--   0        0        0     4646 2023-04-25 08:12:44.685048 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/efficientnet.cpython-38.pyc
--rw-r--r--   0        0        0     4656 2023-03-22 11:45:32.707477 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/efficientnet.cpython-39.pyc
--rw-r--r--   0        0        0     3782 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-310.pyc
--rw-r--r--   0        0        0     3770 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-36.pyc
--rw-r--r--   0        0        0     3733 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-37.pyc
--rw-r--r--   0        0        0     3769 2023-04-25 08:12:44.664048 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-38.pyc
--rw-r--r--   0        0        0     3775 2023-03-22 11:45:32.701816 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-39.pyc
--rw-r--r--   0        0        0     3662 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-310.pyc
--rw-r--r--   0        0        0     3663 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-36.pyc
--rw-r--r--   0        0        0     3611 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-37.pyc
--rw-r--r--   0        0        0     3649 2023-04-25 08:12:44.675049 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-38.pyc
--rw-r--r--   0        0        0     3655 2023-03-22 11:45:32.704271 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-39.pyc
--rw-r--r--   0        0        0     3227 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/mobilenet.cpython-310.pyc
--rw-r--r--   0        0        0     3190 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/mobilenet.cpython-36.pyc
--rw-r--r--   0        0        0     3170 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/mobilenet.cpython-37.pyc
--rw-r--r--   0        0        0     3214 2023-04-25 08:12:44.698094 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/mobilenet.cpython-38.pyc
--rw-r--r--   0        0        0     3218 2023-03-22 11:45:32.713478 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/mobilenet.cpython-39.pyc
--rw-r--r--   0        0        0     6363 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/resnet.cpython-310.pyc
--rw-r--r--   0        0        0     6535 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/resnet.cpython-36.pyc
--rw-r--r--   0        0        0     6227 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/resnet.cpython-37.pyc
--rw-r--r--   0        0        0     6321 2023-04-25 08:12:43.973129 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/resnet.cpython-38.pyc
--rw-r--r--   0        0        0     6352 2023-03-22 11:45:32.004166 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/resnet.cpython-39.pyc
--rw-r--r--   0        0        0     3893 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/senet.cpython-310.pyc
--rw-r--r--   0        0        0     3961 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/senet.cpython-36.pyc
--rw-r--r--   0        0        0     3808 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/senet.cpython-37.pyc
--rw-r--r--   0        0        0     3866 2023-04-25 08:12:44.644048 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/senet.cpython-38.pyc
--rw-r--r--   0        0        0     3884 2023-03-22 11:45:32.696123 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/senet.cpython-39.pyc
--rw-r--r--   0        0        0     5720 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-310.pyc
--rw-r--r--   0        0        0     5949 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-36.pyc
--rw-r--r--   0        0        0     5609 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-37.pyc
--rw-r--r--   0        0        0     5707 2023-04-25 08:12:44.719133 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-38.pyc
--rw-r--r--   0        0        0     5711 2023-03-22 11:45:32.719478 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-39.pyc
--rw-r--r--   0        0        0     4260 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/vgg.cpython-310.pyc
--rw-r--r--   0        0        0     4204 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/vgg.cpython-36.pyc
--rw-r--r--   0        0        0     3990 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/vgg.cpython-37.pyc
--rw-r--r--   0        0        0     4052 2023-04-25 08:12:44.634047 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/vgg.cpython-38.pyc
--rw-r--r--   0        0        0     4258 2023-03-22 11:45:32.693124 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/vgg.cpython-39.pyc
--rw-r--r--   0        0        0     2200 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/xception.cpython-310.pyc
--rw-r--r--   0        0        0     2191 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/xception.cpython-36.pyc
--rw-r--r--   0        0        0     2154 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/xception.cpython-37.pyc
--rw-r--r--   0        0        0     2206 2023-04-25 08:12:44.708776 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/xception.cpython-38.pyc
--rw-r--r--   0        0        0     2200 2023-03-22 11:45:32.715477 mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/xception.cpython-39.pyc
--rw-r--r--   0        0        0     1372 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/_base.py
--rw-r--r--   0        0        0      476 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/_preprocessing.py
--rw-r--r--   0        0        0     1565 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/_utils.py
--rw-r--r--   0        0        0     5317 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/densenet.py
--rw-r--r--   0        0        0     6009 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/dpn.py
--rw-r--r--   0        0        0     6470 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/efficientnet.py
--rw-r--r--   0        0        0     3551 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/inceptionresnetv2.py
--rw-r--r--   0        0        0     3544 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/inceptionv4.py
--rw-r--r--   0        0        0     2933 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/mobilenet.py
--rw-r--r--   0        0        0     9265 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/resnet.py
--rw-r--r--   0        0        0     5849 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/senet.py
--rw-r--r--   0        0        0     9053 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/timm_efficientnet.py
--rw-r--r--   0        0        0     5637 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/vgg.py
--rw-r--r--   0        0        0     1979 2023-03-15 07:44:20.000000 mammopy-0.0.8/mammopy/segmentation_models/encoders/xception.py
--rw-r--r--   0        0        0       23 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/unet/__init__.py
--rw-r--r--   0        0        0      209 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      183 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      191 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      209 2023-04-25 08:12:43.911859 mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      207 2023-03-22 11:45:31.973166 mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3090 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/decoder.cpython-310.pyc
--rw-r--r--   0        0        0     3032 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/decoder.cpython-36.pyc
--rw-r--r--   0        0        0     3043 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/decoder.cpython-37.pyc
--rw-r--r--   0        0        0     3070 2023-04-25 08:12:43.925737 mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/decoder.cpython-38.pyc
--rw-r--r--   0        0        0     3066 2023-03-22 11:45:31.980558 mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/decoder.cpython-39.pyc
--rw-r--r--   0        0        0     3874 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/model.cpython-310.pyc
--rw-r--r--   0        0        0     3787 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/model.cpython-36.pyc
--rw-r--r--   0        0        0     3760 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/model.cpython-37.pyc
--rw-r--r--   0        0        0     3818 2023-04-25 08:12:43.914740 mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/model.cpython-38.pyc
--rw-r--r--   0        0        0     3816 2023-03-22 11:45:31.976868 mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/model.cpython-39.pyc
--rw-r--r--   0        0        0     3862 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/unet/decoder.py
--rw-r--r--   0        0        0     4306 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/unet/model.py
--rw-r--r--   0        0        0       64 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      239 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      247 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      265 2023-04-25 08:12:45.215555 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      263 2023-03-22 11:45:33.063104 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3523 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     3565 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/base.cpython-36.pyc
--rw-r--r--   0        0        0     3575 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/base.cpython-37.pyc
--rw-r--r--   0        0        0     3613 2023-04-25 08:12:45.253548 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/base.cpython-38.pyc
--rw-r--r--   0        0        0     3611 2023-03-22 11:45:33.076361 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     4638 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/functional.cpython-310.pyc
--rw-r--r--   0        0        0     5051 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/functional.cpython-36.pyc
--rw-r--r--   0        0        0     5047 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/functional.cpython-37.pyc
--rw-r--r--   0        0        0     4680 2023-04-25 08:12:45.264554 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/functional.cpython-38.pyc
--rw-r--r--   0        0        0     4668 2023-03-22 11:45:33.080398 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/functional.cpython-39.pyc
--rw-r--r--   0        0        0     4132 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/losses.cpython-310.pyc
--rw-r--r--   0        0        0     4323 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/losses.cpython-36.pyc
--rw-r--r--   0        0        0     4320 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/losses.cpython-37.pyc
--rw-r--r--   0        0        0     4199 2023-04-25 08:12:45.244551 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/losses.cpython-38.pyc
--rw-r--r--   0        0        0     4207 2023-03-22 11:45:33.073360 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/losses.cpython-39.pyc
--rw-r--r--   0        0        0     2280 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/meter.cpython-310.pyc
--rw-r--r--   0        0        0     2234 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/meter.cpython-36.pyc
--rw-r--r--   0        0        0     2242 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/meter.cpython-37.pyc
--rw-r--r--   0        0        0     2282 2023-04-25 08:12:45.234549 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/meter.cpython-38.pyc
--rw-r--r--   0        0        0     2280 2023-03-22 11:45:33.070365 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/meter.cpython-39.pyc
--rw-r--r--   0        0        0     2874 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/metrics.cpython-310.pyc
--rw-r--r--   0        0        0     3367 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/metrics.cpython-36.pyc
--rw-r--r--   0        0        0     3375 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/metrics.cpython-37.pyc
--rw-r--r--   0        0        0     3131 2023-04-25 08:12:45.276549 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/metrics.cpython-38.pyc
--rw-r--r--   0        0        0     3139 2023-03-22 11:45:33.083399 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/metrics.cpython-39.pyc
--rw-r--r--   0        0        0     5903 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/train.cpython-310.pyc
--rw-r--r--   0        0        0     5989 2023-03-15 07:44:24.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/train.cpython-36.pyc
--rw-r--r--   0        0        0     5988 2023-03-15 07:44:24.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/train.cpython-37.pyc
--rw-r--r--   0        0        0     5960 2023-04-25 08:12:45.225902 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/train.cpython-38.pyc
--rw-r--r--   0        0        0     5984 2023-03-22 11:45:33.067362 mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/train.cpython-39.pyc
--rw-r--r--   0        0        0     2513 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/base.py
--rw-r--r--   0        0        0     5051 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/functional.py
--rw-r--r--   0        0        0     3475 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/losses.py
--rw-r--r--   0        0        0     1719 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/meter.py
--rw-r--r--   0        0        0     3026 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/metrics.py
--rw-r--r--   0        0        0     6382 2023-03-15 07:44:22.000000 mammopy-0.0.8/mammopy/segmentation_models/utils/train.py
--rw-r--r--   0        0        0        0 2023-04-25 09:47:19.866178 mammopy-0.0.8/mammopy/visualization/__init__.py
--rw-r--r--   0        0        0      668 2023-04-25 09:48:26.981166 mammopy-0.0.8/mammopy/visualization/canny_edges.py
--rw-r--r--   0        0        0      585 2023-04-26 06:14:21.722445 mammopy-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1540 2023-04-25 07:38:47.273277 mammopy-0.0.8/README.md
--rw-r--r--   0        0        0     2410 1970-01-01 00:00:00.000000 mammopy-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       49 2023-04-26 12:06:48.850675 mammopy-0.0.9/mammopy/__init__.py
+-rw-r--r--   0        0        0     9405 2023-04-26 12:06:26.079065 mammopy-0.0.9/mammopy/main_code.py
+-rw-r--r--   0        0        0      749 2023-04-26 12:07:31.052164 mammopy-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1540 2023-04-26 12:08:07.243703 mammopy-0.0.9/README.md
+-rw-r--r--   0        0        0      267 2023-03-15 07:44:18.000000 mammopy-0.0.9/segmentation_models/__init__.py
+-rw-r--r--   0        0        0       66 2023-03-15 07:44:18.000000 mammopy-0.0.9/segmentation_models/__version__.py
+-rw-r--r--   0        0        0      148 2023-03-15 07:44:18.000000 mammopy-0.0.9/segmentation_models/base/__init__.py
+-rw-r--r--   0        0        0      330 2023-03-15 07:44:18.000000 mammopy-0.0.9/segmentation_models/base/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      304 2023-03-15 07:44:18.000000 mammopy-0.0.9/segmentation_models/base/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      312 2023-03-15 07:44:18.000000 mammopy-0.0.9/segmentation_models/base/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      317 2023-04-26 08:52:14.170870 mammopy-0.0.9/segmentation_models/base/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      328 2023-03-22 11:45:31.983165 mammopy-0.0.9/segmentation_models/base/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      881 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/base/__pycache__/heads.cpython-310.pyc
+-rw-r--r--   0        0        0      845 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/base/__pycache__/heads.cpython-36.pyc
+-rw-r--r--   0        0        0      855 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/base/__pycache__/heads.cpython-37.pyc
+-rw-r--r--   0        0        0      866 2023-04-26 08:52:14.188869 mammopy-0.0.9/segmentation_models/base/__pycache__/heads.cpython-38.pyc
+-rw-r--r--   0        0        0      877 2023-03-22 11:45:31.997169 mammopy-0.0.9/segmentation_models/base/__pycache__/heads.cpython-39.pyc
+-rw-r--r--   0        0        0      940 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/base/__pycache__/initialization.cpython-310.pyc
+-rw-r--r--   0        0        0      909 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/base/__pycache__/initialization.cpython-36.pyc
+-rw-r--r--   0        0        0      919 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/base/__pycache__/initialization.cpython-37.pyc
+-rw-r--r--   0        0        0      917 2023-04-26 08:52:14.178869 mammopy-0.0.9/segmentation_models/base/__pycache__/initialization.cpython-38.pyc
+-rw-r--r--   0        0        0      928 2023-03-22 11:45:31.990419 mammopy-0.0.9/segmentation_models/base/__pycache__/initialization.cpython-39.pyc
+-rw-r--r--   0        0        0     1630 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/base/__pycache__/model.cpython-310.pyc
+-rw-r--r--   0        0        0     1558 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/base/__pycache__/model.cpython-36.pyc
+-rw-r--r--   0        0        0     1566 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/base/__pycache__/model.cpython-37.pyc
+-rw-r--r--   0        0        0     1586 2023-04-26 08:52:14.174872 mammopy-0.0.9/segmentation_models/base/__pycache__/model.cpython-38.pyc
+-rw-r--r--   0        0        0     1618 2023-03-22 11:45:31.987385 mammopy-0.0.9/segmentation_models/base/__pycache__/model.cpython-39.pyc
+-rw-r--r--   0        0        0     3963 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/base/__pycache__/modules.cpython-310.pyc
+-rw-r--r--   0        0        0     4162 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/base/__pycache__/modules.cpython-36.pyc
+-rw-r--r--   0        0        0     4024 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/base/__pycache__/modules.cpython-37.pyc
+-rw-r--r--   0        0        0     3966 2023-04-26 08:52:14.183869 mammopy-0.0.9/segmentation_models/base/__pycache__/modules.cpython-38.pyc
+-rw-r--r--   0        0        0     4003 2023-03-22 11:45:31.993781 mammopy-0.0.9/segmentation_models/base/__pycache__/modules.cpython-39.pyc
+-rw-r--r--   0        0        0      532 2023-03-15 07:44:18.000000 mammopy-0.0.9/segmentation_models/base/heads.py
+-rw-r--r--   0        0        0      848 2023-03-15 07:44:18.000000 mammopy-0.0.9/segmentation_models/base/initialization.py
+-rw-r--r--   0        0        0     1294 2023-03-15 07:44:18.000000 mammopy-0.0.9/segmentation_models/base/model.py
+-rw-r--r--   0        0        0     3561 2023-03-15 07:44:18.000000 mammopy-0.0.9/segmentation_models/base/modules.py
+-rw-r--r--   0        0        0     2341 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__init__.py
+-rw-r--r--   0        0        0     2219 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2165 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0     2179 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     2200 2023-04-26 08:52:14.191866 mammopy-0.0.9/segmentation_models/encoders/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2219 2023-03-22 11:45:32.000169 mammopy-0.0.9/segmentation_models/encoders/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1813 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/_base.cpython-310.pyc
+-rw-r--r--   0        0        0     1768 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/_base.cpython-36.pyc
+-rw-r--r--   0        0        0     1778 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/_base.cpython-37.pyc
+-rw-r--r--   0        0        0     1801 2023-04-26 08:52:14.824390 mammopy-0.0.9/segmentation_models/encoders/__pycache__/_base.cpython-38.pyc
+-rw-r--r--   0        0        0     1812 2023-03-22 11:45:32.684714 mammopy-0.0.9/segmentation_models/encoders/__pycache__/_base.cpython-39.pyc
+-rw-r--r--   0        0        0      572 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/_preprocessing.cpython-310.pyc
+-rw-r--r--   0        0        0      538 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/_preprocessing.cpython-36.pyc
+-rw-r--r--   0        0        0      546 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/_preprocessing.cpython-37.pyc
+-rw-r--r--   0        0        0      563 2023-04-26 08:52:15.278509 mammopy-0.0.9/segmentation_models/encoders/__pycache__/_preprocessing.cpython-38.pyc
+-rw-r--r--   0        0        0      568 2023-03-22 11:45:33.060100 mammopy-0.0.9/segmentation_models/encoders/__pycache__/_preprocessing.cpython-39.pyc
+-rw-r--r--   0        0        0     1399 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     1374 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/_utils.cpython-36.pyc
+-rw-r--r--   0        0        0     1361 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/_utils.cpython-37.pyc
+-rw-r--r--   0        0        0     1372 2023-04-26 08:52:14.827391 mammopy-0.0.9/segmentation_models/encoders/__pycache__/_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     1385 2023-03-22 11:45:32.686716 mammopy-0.0.9/segmentation_models/encoders/__pycache__/_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     4841 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/densenet.cpython-310.pyc
+-rw-r--r--   0        0        0     4841 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/densenet.cpython-36.pyc
+-rw-r--r--   0        0        0     4766 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/densenet.cpython-37.pyc
+-rw-r--r--   0        0        0     4815 2023-04-26 08:52:14.842392 mammopy-0.0.9/segmentation_models/encoders/__pycache__/densenet.cpython-38.pyc
+-rw-r--r--   0        0        0     4830 2023-03-22 11:45:32.699122 mammopy-0.0.9/segmentation_models/encoders/__pycache__/densenet.cpython-39.pyc
+-rw-r--r--   0        0        0     4420 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/dpn.cpython-310.pyc
+-rw-r--r--   0        0        0     4606 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/dpn.cpython-36.pyc
+-rw-r--r--   0        0        0     4347 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/dpn.cpython-37.pyc
+-rw-r--r--   0        0        0     4392 2023-04-26 08:52:14.832391 mammopy-0.0.9/segmentation_models/encoders/__pycache__/dpn.cpython-38.pyc
+-rw-r--r--   0        0        0     4411 2023-03-22 11:45:32.691122 mammopy-0.0.9/segmentation_models/encoders/__pycache__/dpn.cpython-39.pyc
+-rw-r--r--   0        0        0     4660 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/efficientnet.cpython-310.pyc
+-rw-r--r--   0        0        0     4924 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/efficientnet.cpython-36.pyc
+-rw-r--r--   0        0        0     4670 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/efficientnet.cpython-37.pyc
+-rw-r--r--   0        0        0     4633 2023-04-26 08:52:14.852512 mammopy-0.0.9/segmentation_models/encoders/__pycache__/efficientnet.cpython-38.pyc
+-rw-r--r--   0        0        0     4656 2023-03-22 11:45:32.707477 mammopy-0.0.9/segmentation_models/encoders/__pycache__/efficientnet.cpython-39.pyc
+-rw-r--r--   0        0        0     3782 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-310.pyc
+-rw-r--r--   0        0        0     3770 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-36.pyc
+-rw-r--r--   0        0        0     3733 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-37.pyc
+-rw-r--r--   0        0        0     3756 2023-04-26 08:52:14.844390 mammopy-0.0.9/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-38.pyc
+-rw-r--r--   0        0        0     3775 2023-03-22 11:45:32.701816 mammopy-0.0.9/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-39.pyc
+-rw-r--r--   0        0        0     3662 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/inceptionv4.cpython-310.pyc
+-rw-r--r--   0        0        0     3663 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/inceptionv4.cpython-36.pyc
+-rw-r--r--   0        0        0     3611 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/inceptionv4.cpython-37.pyc
+-rw-r--r--   0        0        0     3636 2023-04-26 08:52:14.848394 mammopy-0.0.9/segmentation_models/encoders/__pycache__/inceptionv4.cpython-38.pyc
+-rw-r--r--   0        0        0     3655 2023-03-22 11:45:32.704271 mammopy-0.0.9/segmentation_models/encoders/__pycache__/inceptionv4.cpython-39.pyc
+-rw-r--r--   0        0        0     3227 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/mobilenet.cpython-310.pyc
+-rw-r--r--   0        0        0     3190 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/mobilenet.cpython-36.pyc
+-rw-r--r--   0        0        0     3170 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/mobilenet.cpython-37.pyc
+-rw-r--r--   0        0        0     3201 2023-04-26 08:52:14.859392 mammopy-0.0.9/segmentation_models/encoders/__pycache__/mobilenet.cpython-38.pyc
+-rw-r--r--   0        0        0     3218 2023-03-22 11:45:32.713478 mammopy-0.0.9/segmentation_models/encoders/__pycache__/mobilenet.cpython-39.pyc
+-rw-r--r--   0        0        0     6363 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/resnet.cpython-310.pyc
+-rw-r--r--   0        0        0     6535 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/resnet.cpython-36.pyc
+-rw-r--r--   0        0        0     6227 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/resnet.cpython-37.pyc
+-rw-r--r--   0        0        0     6308 2023-04-26 08:52:14.195868 mammopy-0.0.9/segmentation_models/encoders/__pycache__/resnet.cpython-38.pyc
+-rw-r--r--   0        0        0     6352 2023-03-22 11:45:32.004166 mammopy-0.0.9/segmentation_models/encoders/__pycache__/resnet.cpython-39.pyc
+-rw-r--r--   0        0        0     3893 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/senet.cpython-310.pyc
+-rw-r--r--   0        0        0     3961 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/senet.cpython-36.pyc
+-rw-r--r--   0        0        0     3808 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/senet.cpython-37.pyc
+-rw-r--r--   0        0        0     3853 2023-04-26 08:52:14.838393 mammopy-0.0.9/segmentation_models/encoders/__pycache__/senet.cpython-38.pyc
+-rw-r--r--   0        0        0     3884 2023-03-22 11:45:32.696123 mammopy-0.0.9/segmentation_models/encoders/__pycache__/senet.cpython-39.pyc
+-rw-r--r--   0        0        0     5720 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-310.pyc
+-rw-r--r--   0        0        0     5949 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-36.pyc
+-rw-r--r--   0        0        0     5609 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-37.pyc
+-rw-r--r--   0        0        0     5694 2023-04-26 08:52:14.865391 mammopy-0.0.9/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-38.pyc
+-rw-r--r--   0        0        0     5711 2023-03-22 11:45:32.719478 mammopy-0.0.9/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-39.pyc
+-rw-r--r--   0        0        0     4260 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/vgg.cpython-310.pyc
+-rw-r--r--   0        0        0     4204 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/vgg.cpython-36.pyc
+-rw-r--r--   0        0        0     3990 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/vgg.cpython-37.pyc
+-rw-r--r--   0        0        0     4039 2023-04-26 08:52:14.835392 mammopy-0.0.9/segmentation_models/encoders/__pycache__/vgg.cpython-38.pyc
+-rw-r--r--   0        0        0     4258 2023-03-22 11:45:32.693124 mammopy-0.0.9/segmentation_models/encoders/__pycache__/vgg.cpython-39.pyc
+-rw-r--r--   0        0        0     2200 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/xception.cpython-310.pyc
+-rw-r--r--   0        0        0     2191 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/xception.cpython-36.pyc
+-rw-r--r--   0        0        0     2154 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/encoders/__pycache__/xception.cpython-37.pyc
+-rw-r--r--   0        0        0     2193 2023-04-26 08:52:14.861391 mammopy-0.0.9/segmentation_models/encoders/__pycache__/xception.cpython-38.pyc
+-rw-r--r--   0        0        0     2200 2023-03-22 11:45:32.715477 mammopy-0.0.9/segmentation_models/encoders/__pycache__/xception.cpython-39.pyc
+-rw-r--r--   0        0        0     1372 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/_base.py
+-rw-r--r--   0        0        0      476 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/_preprocessing.py
+-rw-r--r--   0        0        0     1565 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/_utils.py
+-rw-r--r--   0        0        0     5317 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/densenet.py
+-rw-r--r--   0        0        0     6009 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/dpn.py
+-rw-r--r--   0        0        0     6470 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/efficientnet.py
+-rw-r--r--   0        0        0     3551 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/inceptionresnetv2.py
+-rw-r--r--   0        0        0     3544 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/inceptionv4.py
+-rw-r--r--   0        0        0     2933 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/mobilenet.py
+-rw-r--r--   0        0        0     9265 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/resnet.py
+-rw-r--r--   0        0        0     5849 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/senet.py
+-rw-r--r--   0        0        0     9053 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/timm_efficientnet.py
+-rw-r--r--   0        0        0     5637 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/vgg.py
+-rw-r--r--   0        0        0     1979 2023-03-15 07:44:20.000000 mammopy-0.0.9/segmentation_models/encoders/xception.py
+-rw-r--r--   0        0        0       23 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/unet/__init__.py
+-rw-r--r--   0        0        0      209 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/unet/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      183 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/unet/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      191 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/unet/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      196 2023-04-26 08:52:14.157876 mammopy-0.0.9/segmentation_models/unet/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      207 2023-03-22 11:45:31.973166 mammopy-0.0.9/segmentation_models/unet/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3090 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/unet/__pycache__/decoder.cpython-310.pyc
+-rw-r--r--   0        0        0     3032 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/unet/__pycache__/decoder.cpython-36.pyc
+-rw-r--r--   0        0        0     3043 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/unet/__pycache__/decoder.cpython-37.pyc
+-rw-r--r--   0        0        0     3057 2023-04-26 08:52:14.167874 mammopy-0.0.9/segmentation_models/unet/__pycache__/decoder.cpython-38.pyc
+-rw-r--r--   0        0        0     3066 2023-03-22 11:45:31.980558 mammopy-0.0.9/segmentation_models/unet/__pycache__/decoder.cpython-39.pyc
+-rw-r--r--   0        0        0     3874 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/unet/__pycache__/model.cpython-310.pyc
+-rw-r--r--   0        0        0     3787 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/unet/__pycache__/model.cpython-36.pyc
+-rw-r--r--   0        0        0     3760 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/unet/__pycache__/model.cpython-37.pyc
+-rw-r--r--   0        0        0     3805 2023-04-26 08:52:14.162873 mammopy-0.0.9/segmentation_models/unet/__pycache__/model.cpython-38.pyc
+-rw-r--r--   0        0        0     3816 2023-03-22 11:45:31.976868 mammopy-0.0.9/segmentation_models/unet/__pycache__/model.cpython-39.pyc
+-rw-r--r--   0        0        0     3862 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/unet/decoder.py
+-rw-r--r--   0        0        0     4306 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/unet/model.py
+-rw-r--r--   0        0        0       64 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      239 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      247 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      252 2023-04-26 08:52:15.281508 mammopy-0.0.9/segmentation_models/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      263 2023-03-22 11:45:33.063104 mammopy-0.0.9/segmentation_models/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3523 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     3565 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/__pycache__/base.cpython-36.pyc
+-rw-r--r--   0        0        0     3575 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/__pycache__/base.cpython-37.pyc
+-rw-r--r--   0        0        0     3600 2023-04-26 08:52:15.296509 mammopy-0.0.9/segmentation_models/utils/__pycache__/base.cpython-38.pyc
+-rw-r--r--   0        0        0     3611 2023-03-22 11:45:33.076361 mammopy-0.0.9/segmentation_models/utils/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     4638 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/__pycache__/functional.cpython-310.pyc
+-rw-r--r--   0        0        0     5051 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/__pycache__/functional.cpython-36.pyc
+-rw-r--r--   0        0        0     5047 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/__pycache__/functional.cpython-37.pyc
+-rw-r--r--   0        0        0     4667 2023-04-26 08:52:15.300650 mammopy-0.0.9/segmentation_models/utils/__pycache__/functional.cpython-38.pyc
+-rw-r--r--   0        0        0     4668 2023-03-22 11:45:33.080398 mammopy-0.0.9/segmentation_models/utils/__pycache__/functional.cpython-39.pyc
+-rw-r--r--   0        0        0     4132 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/__pycache__/losses.cpython-310.pyc
+-rw-r--r--   0        0        0     4323 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/__pycache__/losses.cpython-36.pyc
+-rw-r--r--   0        0        0     4320 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/__pycache__/losses.cpython-37.pyc
+-rw-r--r--   0        0        0     4186 2023-04-26 08:52:15.293512 mammopy-0.0.9/segmentation_models/utils/__pycache__/losses.cpython-38.pyc
+-rw-r--r--   0        0        0     4207 2023-03-22 11:45:33.073360 mammopy-0.0.9/segmentation_models/utils/__pycache__/losses.cpython-39.pyc
+-rw-r--r--   0        0        0     2280 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/__pycache__/meter.cpython-310.pyc
+-rw-r--r--   0        0        0     2234 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/__pycache__/meter.cpython-36.pyc
+-rw-r--r--   0        0        0     2242 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/__pycache__/meter.cpython-37.pyc
+-rw-r--r--   0        0        0     2269 2023-04-26 08:52:15.290507 mammopy-0.0.9/segmentation_models/utils/__pycache__/meter.cpython-38.pyc
+-rw-r--r--   0        0        0     2280 2023-03-22 11:45:33.070365 mammopy-0.0.9/segmentation_models/utils/__pycache__/meter.cpython-39.pyc
+-rw-r--r--   0        0        0     2874 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/__pycache__/metrics.cpython-310.pyc
+-rw-r--r--   0        0        0     3367 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/__pycache__/metrics.cpython-36.pyc
+-rw-r--r--   0        0        0     3375 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/__pycache__/metrics.cpython-37.pyc
+-rw-r--r--   0        0        0     3118 2023-04-26 08:52:15.304514 mammopy-0.0.9/segmentation_models/utils/__pycache__/metrics.cpython-38.pyc
+-rw-r--r--   0        0        0     3139 2023-03-22 11:45:33.083399 mammopy-0.0.9/segmentation_models/utils/__pycache__/metrics.cpython-39.pyc
+-rw-r--r--   0        0        0     5903 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/__pycache__/train.cpython-310.pyc
+-rw-r--r--   0        0        0     5989 2023-03-15 07:44:24.000000 mammopy-0.0.9/segmentation_models/utils/__pycache__/train.cpython-36.pyc
+-rw-r--r--   0        0        0     5988 2023-03-15 07:44:24.000000 mammopy-0.0.9/segmentation_models/utils/__pycache__/train.cpython-37.pyc
+-rw-r--r--   0        0        0     5947 2023-04-26 08:52:15.286906 mammopy-0.0.9/segmentation_models/utils/__pycache__/train.cpython-38.pyc
+-rw-r--r--   0        0        0     5984 2023-03-22 11:45:33.067362 mammopy-0.0.9/segmentation_models/utils/__pycache__/train.cpython-39.pyc
+-rw-r--r--   0        0        0     2513 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/base.py
+-rw-r--r--   0        0        0     5051 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/functional.py
+-rw-r--r--   0        0        0     3475 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/losses.py
+-rw-r--r--   0        0        0     1719 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/meter.py
+-rw-r--r--   0        0        0     3026 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/metrics.py
+-rw-r--r--   0        0        0     6382 2023-03-15 07:44:22.000000 mammopy-0.0.9/segmentation_models/utils/train.py
+-rw-r--r--   0        0        0     2410 1970-01-01 00:00:00.000000 mammopy-0.0.9/PKG-INFO
```

### Comparing `mammopy-0.0.8/mammopy/mammopy.py` & `mammopy-0.0.9/mammopy/main_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,588 +1,588 @@
-00000000: 0d0a 696d 706f 7274 206f 730d 0a69 6d70  ..import os..imp
-00000010: 6f72 7420 6e75 6d70 7920 6173 206e 700d  ort numpy as np.
-00000020: 0a69 6d70 6f72 7420 7265 7175 6573 7473  .import requests
-00000030: 0d0a 6672 6f6d 2070 6174 686c 6962 2069  ..from pathlib i
-00000040: 6d70 6f72 7420 5061 7468 0d0a 6672 6f6d  mport Path..from
-00000050: 2073 6b69 6d61 6765 2069 6d70 6f72 7420   skimage import 
-00000060: 6665 6174 7572 650d 0a69 6d70 6f72 7420  feature..import 
-00000070: 746f 7263 680d 0a69 6d70 6f72 7420 6d61  torch..import ma
-00000080: 7470 6c6f 746c 6962 2e70 7970 6c6f 7420  tplotlib.pyplot 
-00000090: 6173 2070 6c74 0d0a 696d 706f 7274 2074  as plt..import t
-000000a0: 6f72 6368 2e6e 6e20 6173 206e 6e0d 0a69  orch.nn as nn..i
-000000b0: 6d70 6f72 7420 6f73 2c20 696f 2c20 7079  mport os, io, py
-000000c0: 6469 636f 6d0d 0a69 6d70 6f72 7420 7469  dicom..import ti
-000000d0: 6d65 0d0a 6672 6f6d 2074 6f72 6368 7669  me..from torchvi
-000000e0: 7369 6f6e 2069 6d70 6f72 7420 7472 616e  sion import tran
-000000f0: 7366 6f72 6d73 0d0a 6672 6f6d 2050 494c  sforms..from PIL
-00000100: 2069 6d70 6f72 7420 496d 6167 650d 0a0d   import Image...
-00000110: 0a4d 4153 4b5f 434f 4c4f 5253 203d 205b  .MASK_COLORS = [
-00000120: 2272 6564 222c 2022 6772 6565 6e22 2c20  "red", "green", 
-00000130: 2262 6c75 6522 2c20 2279 656c 6c6f 7722  "blue", "yellow"
-00000140: 2c20 226d 6167 656e 7461 222c 2022 6379  , "magenta", "cy
-00000150: 616e 225d 0d0a 0d0a 0d0a 6465 6620 6d61  an"]......def ma
-00000160: 736b 5f74 6f5f 7267 6261 286d 6173 6b2c  sk_to_rgba(mask,
-00000170: 2063 6f6c 6f72 3d22 7265 6422 293a 0d0a   color="red"):..
-00000180: 2020 2020 2222 220d 0a20 2020 2043 6f6e      """..    Con
-00000190: 7665 7274 7320 6269 6e61 7279 2073 6567  verts binary seg
-000001a0: 6d65 6e74 6174 696f 6e20 6d61 736b 2066  mentation mask f
-000001b0: 726f 6d20 7768 6974 6520 746f 2072 6564  rom white to red
-000001c0: 2063 6f6c 6f72 2e0d 0a20 2020 2041 6c73   color...    Als
-000001d0: 6f20 6164 6473 2061 6c70 6861 2063 6861  o adds alpha cha
-000001e0: 6e6e 656c 2074 6f20 6d61 6b65 2062 6c61  nnel to make bla
-000001f0: 636b 2062 6163 6b67 726f 756e 6420 7472  ck background tr
-00000200: 616e 7370 6172 656e 742e 0d0a 2020 2020  ansparent...    
-00000210: 4172 6773 3a0d 0a20 2020 2020 2020 206d  Args:..        m
-00000220: 6173 6b20 286e 756d 7079 2e6e 6461 7272  ask (numpy.ndarr
-00000230: 6179 293a 205b 6465 7363 7269 7074 696f  ay): [descriptio
-00000240: 6e5d 0d0a 2020 2020 2020 2020 636f 6c6f  n]..        colo
-00000250: 7220 2873 7472 2c20 6f70 7469 6f6e 616c  r (str, optional
-00000260: 293a 2043 6865 636b 2060 4d41 534b 5f43  ): Check `MASK_C
-00000270: 4f4c 4f52 5360 2066 6f72 2061 7661 696c  OLORS` for avail
-00000280: 6162 6c65 2063 6f6c 6f72 732e 2044 6566  able colors. Def
-00000290: 6175 6c74 7320 746f 2022 7265 6422 2e0d  aults to "red"..
-000002a0: 0a20 2020 2052 6574 7572 6e73 3a0d 0a20  .    Returns:.. 
-000002b0: 2020 2020 2020 206e 756d 7079 2e6e 6461         numpy.nda
-000002c0: 7272 6179 3a20 5b64 6573 6372 6970 7469  rray: [descripti
-000002d0: 6f6e 5d0d 0a20 2020 2022 2222 0d0a 2020  on]..    """..  
-000002e0: 2020 6173 7365 7274 2063 6f6c 6f72 2069    assert color i
-000002f0: 6e20 4d41 534b 5f43 4f4c 4f52 530d 0a20  n MASK_COLORS.. 
-00000300: 2020 2061 7373 6572 7420 6d61 736b 2e6e     assert mask.n
-00000310: 6469 6d20 3d3d 2033 206f 7220 6d61 736b  dim == 3 or mask
-00000320: 2e6e 6469 6d20 3d3d 2032 0d0a 0d0a 2020  .ndim == 2....  
-00000330: 2020 6820 3d20 6d61 736b 2e73 6861 7065    h = mask.shape
-00000340: 5b30 5d0d 0a20 2020 2077 203d 206d 6173  [0]..    w = mas
-00000350: 6b2e 7368 6170 655b 315d 0d0a 2020 2020  k.shape[1]..    
-00000360: 7a65 726f 7320 3d20 6e70 2e7a 6572 6f73  zeros = np.zeros
-00000370: 2828 682c 2077 2929 0d0a 2020 2020 6f6e  ((h, w))..    on
-00000380: 6573 203d 206d 6173 6b2e 7265 7368 6170  es = mask.reshap
-00000390: 6528 682c 2077 290d 0a20 2020 2069 6620  e(h, w)..    if 
-000003a0: 636f 6c6f 7220 3d3d 2022 7265 6422 3a0d  color == "red":.
-000003b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000003c0: 6e70 2e73 7461 636b 2828 6f6e 6573 2c20  np.stack((ones, 
-000003d0: 7a65 726f 732c 207a 6572 6f73 2c20 6f6e  zeros, zeros, on
-000003e0: 6573 292c 2061 7869 733d 2d31 290d 0a20  es), axis=-1).. 
-000003f0: 2020 2065 6c69 6620 636f 6c6f 7220 3d3d     elif color ==
-00000400: 2022 6772 6565 6e22 3a0d 0a20 2020 2020   "green":..     
-00000410: 2020 2072 6574 7572 6e20 6e70 2e73 7461     return np.sta
-00000420: 636b 2828 7a65 726f 732c 206f 6e65 732c  ck((zeros, ones,
-00000430: 207a 6572 6f73 2c20 6f6e 6573 292c 2061   zeros, ones), a
-00000440: 7869 733d 2d31 290d 0a20 2020 2065 6c69  xis=-1)..    eli
-00000450: 6620 636f 6c6f 7220 3d3d 2022 626c 7565  f color == "blue
-00000460: 223a 0d0a 2020 2020 2020 2020 7265 7475  ":..        retu
-00000470: 726e 206e 702e 7374 6163 6b28 287a 6572  rn np.stack((zer
-00000480: 6f73 2c20 7a65 726f 732c 206f 6e65 732c  os, zeros, ones,
-00000490: 206f 6e65 7329 2c20 6178 6973 3d2d 3129   ones), axis=-1)
-000004a0: 0d0a 2020 2020 656c 6966 2063 6f6c 6f72  ..    elif color
-000004b0: 203d 3d20 2279 656c 6c6f 7722 3a0d 0a20   == "yellow":.. 
-000004c0: 2020 2020 2020 2072 6574 7572 6e20 6e70         return np
-000004d0: 2e73 7461 636b 2828 6f6e 6573 2c20 6f6e  .stack((ones, on
-000004e0: 6573 2c20 7a65 726f 732c 206f 6e65 7329  es, zeros, ones)
-000004f0: 2c20 6178 6973 3d2d 3129 0d0a 2020 2020  , axis=-1)..    
-00000500: 656c 6966 2063 6f6c 6f72 203d 3d20 226d  elif color == "m
-00000510: 6167 656e 7461 223a 0d0a 2020 2020 2020  agenta":..      
-00000520: 2020 7265 7475 726e 206e 702e 7374 6163    return np.stac
-00000530: 6b28 286f 6e65 732c 207a 6572 6f73 2c20  k((ones, zeros, 
-00000540: 6f6e 6573 2c20 6f6e 6573 292c 2061 7869  ones, ones), axi
-00000550: 733d 2d31 290d 0a20 2020 2065 6c69 6620  s=-1)..    elif 
-00000560: 636f 6c6f 7220 3d3d 2022 6379 616e 223a  color == "cyan":
-00000570: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00000580: 206e 702e 7374 6163 6b28 287a 6572 6f73   np.stack((zeros
-00000590: 2c20 6f6e 6573 2c20 6f6e 6573 2c20 6f6e  , ones, ones, on
-000005a0: 6573 292c 2061 7869 733d 2d31 290d 0a0d  es), axis=-1)...
-000005b0: 0a0d 0a0d 0a64 6566 206c 6f61 645f 6d6f  .....def load_mo
-000005c0: 6465 6c28 6d6f 6465 6c5f 7061 7468 293a  del(model_path):
-000005d0: 0d0a 2020 2020 2222 220d 0a20 2020 204c  ..    """..    L
-000005e0: 6f61 6473 2061 2070 7265 2d74 7261 696e  oads a pre-train
-000005f0: 6564 206d 6f64 656c 2066 726f 6d20 6120  ed model from a 
-00000600: 6769 7665 6e20 7061 7468 2e0d 0a20 2020  given path...   
-00000610: 2041 7267 733a 0d0a 2020 2020 2d20 6d6f   Args:..    - mo
-00000620: 6465 6c5f 7061 7468 3a20 7374 722c 2074  del_path: str, t
-00000630: 6865 2070 6174 6820 746f 2074 6865 2070  he path to the p
-00000640: 7265 2d74 7261 696e 6564 206d 6f64 656c  re-trained model
-00000650: 2e20 0d0a 2020 2020 2020 2020 2020 2020  . ..            
-00000660: 2020 2020 2020 4966 206d 6f64 656c 5f70        If model_p
-00000670: 6174 6820 3d20 2762 6173 6527 2c20 7468  ath = 'base', th
-00000680: 656e 2074 6865 2064 6566 6175 6c74 2070  en the default p
-00000690: 7265 2d74 7261 696e 6564 206d 6f64 656c  re-trained model
-000006a0: 2077 696c 6c20 6265 206c 6f61 6465 642e   will be loaded.
-000006b0: 0d0a 2020 2020 0d0a 2020 2020 5265 7475  ..    ..    Retu
-000006c0: 726e 733a 0d0a 2020 2020 2d20 6d6f 6465  rns:..    - mode
-000006d0: 6c3a 2074 6f72 6368 2e6e 6e2e 4d6f 6475  l: torch.nn.Modu
-000006e0: 6c65 2c20 7468 6520 7072 652d 7472 6169  le, the pre-trai
-000006f0: 6e65 6420 6d6f 6465 6c20 6c6f 6164 6564  ned model loaded
-00000700: 2066 726f 6d20 7468 6520 7370 6563 6966   from the specif
-00000710: 6965 6420 7061 7468 2e0d 0a20 2020 2052  ied path...    R
-00000720: 6169 7365 733a 0d0a 2020 2020 2d20 5479  aises:..    - Ty
-00000730: 7065 4572 726f 723a 2069 6620 7468 6520  peError: if the 
-00000740: 696e 7075 7420 6d6f 6465 6c5f 7061 7468  input model_path
-00000750: 2069 7320 6e6f 7420 2762 6173 6527 2e0d   is not 'base'..
-00000760: 0a20 2020 2022 2222 0d0a 2020 2020 0d0a  .    """..    ..
-00000770: 2020 2020 6966 206d 6f64 656c 5f70 6174      if model_pat
-00000780: 6820 3d3d 2027 6261 7365 273a 0d0a 2020  h == 'base':..  
-00000790: 2020 2020 2020 2320 4465 6669 6e65 2074        # Define t
-000007a0: 6865 2070 6174 6820 746f 2074 6865 2064  he path to the d
-000007b0: 6566 6175 6c74 2070 7265 2d74 7261 696e  efault pre-train
-000007c0: 6564 206d 6f64 656c 2077 6569 6768 7473  ed model weights
-000007d0: 0d0a 2020 2020 2020 2020 6d6f 6465 6c5f  ..        model_
-000007e0: 7765 6967 6874 735f 7061 7468 203d 2022  weights_path = "
-000007f0: 7765 6967 6874 732e 7074 6822 0d0a 2020  weights.pth"..  
-00000800: 2020 2020 2020 7061 7468 203d 2050 6174        path = Pat
-00000810: 6828 6d6f 6465 6c5f 7765 6967 6874 735f  h(model_weights_
-00000820: 7061 7468 290d 0a0d 0a20 2020 2020 2020  path)....       
-00000830: 2023 2049 6620 7468 6520 6d6f 6465 6c20   # If the model 
-00000840: 7765 6967 6874 7320 6669 6c65 2064 6f65  weights file doe
-00000850: 7320 6e6f 7420 6578 6973 742c 2064 6f77  s not exist, dow
-00000860: 6e6c 6f61 6420 6974 2066 726f 6d20 4472  nload it from Dr
-00000870: 6f70 626f 780d 0a20 2020 2020 2020 2069  opbox..        i
-00000880: 6620 6e6f 7420 7061 7468 2e69 735f 6669  f not path.is_fi
-00000890: 6c65 2829 3a0d 0a20 2020 2020 2020 2020  le():..         
-000008a0: 2020 2075 726c 203d 2022 6874 7470 733a     url = "https:
-000008b0: 2f2f 7777 772e 6472 6f70 626f 782e 636f  //www.dropbox.co
-000008c0: 6d2f 732f 3337 7274 6564 7777 6473 6c7a  m/s/37rtedwwdslz
-000008d0: 3977 362f 616c 6c5f 6461 7461 7365 7473  9w6/all_datasets
-000008e0: 2e70 7468 3f64 6c3d 3122 0d0a 2020 2020  .pth?dl=1"..    
-000008f0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-00000900: 203d 2072 6571 7565 7374 732e 6765 7428   = requests.get(
-00000910: 7572 6c29 0d0a 2020 2020 2020 2020 2020  url)..          
-00000920: 2020 6f70 656e 2822 7765 6967 6874 732e    open("weights.
-00000930: 7074 6822 2c20 2277 6222 292e 7772 6974  pth", "wb").writ
-00000940: 6528 7265 7370 6f6e 7365 2e63 6f6e 7465  e(response.conte
-00000950: 6e74 290d 0a20 2020 2020 2020 200d 0a20  nt)..        .. 
-00000960: 2020 2020 2020 2023 204c 6f61 6420 7468         # Load th
-00000970: 6520 7072 652d 7472 6169 6e65 6420 6d6f  e pre-trained mo
-00000980: 6465 6c20 616e 6420 7365 7420 7468 6520  del and set the 
-00000990: 6465 7669 6365 2074 6f20 4350 550d 0a20  device to CPU.. 
-000009a0: 2020 2020 2020 206d 6f64 656c 203d 2074         model = t
-000009b0: 6f72 6368 2e6c 6f61 6428 6d6f 6465 6c5f  orch.load(model_
-000009c0: 7765 6967 6874 735f 7061 7468 2c20 6d61  weights_path, ma
-000009d0: 705f 6c6f 6361 7469 6f6e 3d74 6f72 6368  p_location=torch
-000009e0: 2e64 6576 6963 6528 2263 7075 2229 290d  .device("cpu")).
-000009f0: 0a20 2020 2020 2020 2023 2043 6f6e 7665  .        # Conve
-00000a00: 7274 2074 6865 206d 6f64 656c 2074 6f20  rt the model to 
-00000a10: 6265 2063 6f6d 7061 7469 626c 6520 7769  be compatible wi
-00000a20: 7468 206d 756c 7469 706c 6520 4750 5573  th multiple GPUs
-00000a30: 2c20 6966 2061 7661 696c 6162 6c65 0d0a  , if available..
-00000a40: 2020 2020 2020 2020 6d6f 6465 6c20 3d20          model = 
-00000a50: 6e6e 2e44 6174 6150 6172 616c 6c65 6c28  nn.DataParallel(
-00000a60: 6d6f 6465 6c2e 6d6f 6475 6c65 290d 0a20  model.module).. 
-00000a70: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00000a80: 2072 6574 7572 6e20 6d6f 6465 6c0d 0a20   return model.. 
-00000a90: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00000aa0: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
-00000ab0: 7228 224d 6f64 656c 206e 6f74 2069 6d70  r("Model not imp
-00000ac0: 6c65 6d65 6e74 6564 2229 0d0a 0d0a 2020  lemented")....  
-00000ad0: 2020 2020 2020 0d0a 0d0a 6465 6620 696d        ....def im
-00000ae0: 6167 655f 7465 6e73 6f72 2869 6d67 293a  age_tensor(img):
-00000af0: 0d0a 2020 2020 2222 220d 0a20 2020 2043  ..    """..    C
-00000b00: 6f6e 7665 7274 7320 6120 5049 4c20 496d  onverts a PIL Im
-00000b10: 6167 6520 6f72 204e 756d 5079 2061 7272  age or NumPy arr
-00000b20: 6179 2074 6f20 6120 5079 546f 7263 6820  ay to a PyTorch 
-00000b30: 7465 6e73 6f72 2e0d 0a20 2020 2041 7267  tensor...    Arg
-00000b40: 733a 0d0a 2020 2020 2d20 696d 673a 2050  s:..    - img: P
-00000b50: 494c 2e49 6d61 6765 206f 7220 6e70 2e6e  IL.Image or np.n
-00000b60: 6461 7272 6179 2c20 7468 6520 696d 6167  darray, the imag
-00000b70: 6520 746f 2062 6520 636f 6e76 6572 7465  e to be converte
-00000b80: 6420 746f 2061 2050 7954 6f72 6368 2074  d to a PyTorch t
-00000b90: 656e 736f 722e 0d0a 2020 2020 5265 7475  ensor...    Retu
-00000ba0: 726e 733a 0d0a 2020 2020 2d20 696d 6167  rns:..    - imag
-00000bb0: 653a 2074 6f72 6368 2e54 656e 736f 722c  e: torch.Tensor,
-00000bc0: 2074 6865 2063 6f6e 7665 7274 6564 2050   the converted P
-00000bd0: 7954 6f72 6368 2074 656e 736f 722e 0d0a  yTorch tensor...
-00000be0: 2020 2020 5261 6973 6573 3a0d 0a20 2020      Raises:..   
-00000bf0: 202d 2054 7970 6545 7272 6f72 3a20 6966   - TypeError: if
-00000c00: 2074 6865 2069 6e70 7574 2069 6d61 6765   the input image
-00000c10: 2069 7320 6e6f 7420 6120 5049 4c2e 496d   is not a PIL.Im
-00000c20: 6167 6520 6f72 206e 702e 6e64 6172 7261  age or np.ndarra
-00000c30: 792e 0d0a 2020 2020 2222 220d 0a20 2020  y...    """..   
-00000c40: 200d 0a20 2020 2069 6620 7479 7065 2869   ..    if type(i
-00000c50: 6d67 2920 6e6f 7420 696e 205b 6e70 2e6e  mg) not in [np.n
-00000c60: 6461 7272 6179 2c20 496d 6167 652e 496d  darray, Image.Im
-00000c70: 6167 655d 3a0d 0a20 2020 2020 2020 2072  age]:..        r
-00000c80: 6169 7365 2054 7970 6545 7272 6f72 2822  aise TypeError("
-00000c90: 496e 7075 7420 6d75 7374 2062 6520 6e70  Input must be np
-00000ca0: 2e6e 6461 7272 6179 206f 7220 5049 4c2e  .ndarray or PIL.
-00000cb0: 496d 6167 6522 290d 0a0d 0a20 2020 2023  Image")....    #
-00000cc0: 2044 6566 696e 6520 6120 5079 546f 7263   Define a PyTorc
-00000cd0: 6820 7465 6e73 6f72 2074 7261 6e73 666f  h tensor transfo
-00000ce0: 726d 6572 2070 6970 656c 696e 650d 0a20  rmer pipeline.. 
-00000cf0: 2020 2074 6f72 6368 5f74 656e 736f 7220     torch_tensor 
-00000d00: 3d20 7472 616e 7366 6f72 6d73 2e43 6f6d  = transforms.Com
-00000d10: 706f 7365 280d 0a20 2020 2020 2020 205b  pose(..        [
-00000d20: 7472 616e 7366 6f72 6d73 2e52 6573 697a  transforms.Resiz
-00000d30: 6528 2832 3536 2c20 3235 3629 292c 2074  e((256, 256)), t
-00000d40: 7261 6e73 666f 726d 732e 546f 5465 6e73  ransforms.ToTens
-00000d50: 6f72 2829 5d0d 0a20 2020 2029 0d0a 0d0a  or()]..    )....
-00000d60: 2020 2020 6966 2074 7970 6528 696d 6729      if type(img)
-00000d70: 203d 3d20 496d 6167 652e 496d 6167 653a   == Image.Image:
-00000d80: 0d0a 2020 2020 2020 2020 2320 436f 6e76  ..        # Conv
-00000d90: 6572 7420 5049 4c20 696d 6167 6520 746f  ert PIL image to
-00000da0: 2050 7954 6f72 6368 2074 656e 736f 720d   PyTorch tensor.
-00000db0: 0a20 2020 2020 2020 2069 6d61 6765 203d  .        image =
-00000dc0: 2074 6f72 6368 5f74 656e 736f 7228 696d   torch_tensor(im
-00000dd0: 6729 0d0a 2020 2020 2020 2020 696d 6167  g)..        imag
-00000de0: 6520 3d20 696d 6167 652e 756e 7371 7565  e = image.unsque
-00000df0: 657a 6528 3029 0d0a 2020 2020 2020 2020  eze(0)..        
-00000e00: 7072 696e 7428 2274 656e 736f 7222 2c20  print("tensor", 
-00000e10: 7479 7065 2869 6d61 6765 2929 0d0a 2020  type(image))..  
-00000e20: 2020 2020 2020 7265 7475 726e 2069 6d61        return ima
-00000e30: 6765 0d0a 2020 2020 656c 6966 2074 7970  ge..    elif typ
-00000e40: 6528 696d 6729 203d 3d20 6e70 2e6e 6461  e(img) == np.nda
-00000e50: 7272 6179 3a0d 0a20 2020 2020 2020 2023  rray:..        #
-00000e60: 2043 6f6e 7665 7274 204e 756d 5079 2061   Convert NumPy a
-00000e70: 7272 6179 2074 6f20 5247 4220 5049 4c20  rray to RGB PIL 
-00000e80: 696d 6167 6520 616e 6420 7468 656e 2074  image and then t
-00000e90: 6f20 5079 546f 7263 6820 7465 6e73 6f72  o PyTorch tensor
-00000ea0: 0d0a 2020 2020 2020 2020 7069 6c5f 696d  ..        pil_im
-00000eb0: 6167 6520 3d20 496d 6167 652e 6672 6f6d  age = Image.from
-00000ec0: 6172 7261 7928 696d 6729 2e63 6f6e 7665  array(img).conve
-00000ed0: 7274 2822 5247 4222 290d 0a20 2020 2020  rt("RGB")..     
-00000ee0: 2020 2069 6d61 6765 203d 2074 6f72 6368     image = torch
-00000ef0: 5f74 656e 736f 7228 7069 6c5f 696d 6167  _tensor(pil_imag
-00000f00: 6529 0d0a 2020 2020 2020 2020 696d 6167  e)..        imag
-00000f10: 6520 3d20 696d 6167 652e 756e 7371 7565  e = image.unsque
-00000f20: 657a 6528 3029 0d0a 2020 2020 2020 2020  eze(0)..        
-00000f30: 7072 696e 7428 2274 656e 736f 7222 2c20  print("tensor", 
-00000f40: 7479 7065 2869 6d61 6765 2929 0d0a 2020  type(image))..  
-00000f50: 2020 2020 2020 7265 7475 726e 2069 6d61        return ima
-00000f60: 6765 0d0a 2020 2020 656c 7365 3a0d 0a20  ge..    else:.. 
-00000f70: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
-00000f80: 6545 7272 6f72 2822 496e 7075 7420 6d75  eError("Input mu
-00000f90: 7374 2062 6520 6e70 2e6e 6461 7272 6179  st be np.ndarray
-00000fa0: 206f 7220 5049 4c2e 496d 6167 6522 290d   or PIL.Image").
-00000fb0: 0a0d 0a0d 0a0d 0a64 6566 2070 6572 6365  .......def perce
-00000fc0: 6e74 6167 655f 6465 6e73 6974 7928 6d6f  ntage_density(mo
-00000fd0: 6465 6c2c 2069 6d61 6765 5f70 6174 6829  del, image_path)
-00000fe0: 3a0d 0a20 2020 2022 2222 0d0a 2020 2020  :..    """..    
-00000ff0: 436f 6d70 7574 6573 2074 6865 2070 6572  Computes the per
-00001000: 6365 6e74 6167 6520 6f66 206d 616d 6d6f  centage of mammo
-00001010: 6772 616d 2064 656e 7369 7479 2069 6e20  gram density in 
-00001020: 616e 2069 6e70 7574 2069 6d61 6765 2e0d  an input image..
-00001030: 0a20 2020 2041 7267 733a 0d0a 2020 2020  .    Args:..    
-00001040: 2020 2020 6d6f 6465 6c20 2873 7472 293a      model (str):
-00001050: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
-00001060: 2070 7265 2d74 7261 696e 6564 206d 6f64   pre-trained mod
-00001070: 656c 2074 6f20 7573 652e 0d0a 2020 2020  el to use...    
-00001080: 2020 2020 696d 6167 655f 7061 7468 2028      image_path (
-00001090: 7374 7229 3a20 5468 6520 7061 7468 2074  str): The path t
-000010a0: 6f20 7468 6520 696e 7075 7420 696d 6167  o the input imag
-000010b0: 6520 6669 6c65 2e0d 0a20 2020 2052 6574  e file...    Ret
-000010c0: 7572 6e73 3a0d 0a20 2020 2020 2020 2064  urns:..        d
-000010d0: 6963 743a 2041 2064 6963 7469 6f6e 6172  ict: A dictionar
-000010e0: 7920 636f 6e74 6169 6e69 6e67 2074 6865  y containing the
-000010f0: 2072 6573 756c 7473 206f 6620 7468 6520   results of the 
-00001100: 636f 6d70 7574 6174 696f 6e2e 2054 6865  computation. The
-00001110: 2064 6963 7469 6f6e 6172 790d 0a20 2020   dictionary..   
-00001120: 2020 2020 2068 6173 2074 6865 2066 6f6c       has the fol
-00001130: 6c6f 7769 6e67 206b 6579 733a 0d0a 2020  lowing keys:..  
-00001140: 2020 2020 2020 2020 2020 2d20 6e6f 6e5f            - non_
-00001150: 6465 6e73 655f 6172 6561 3a20 5468 6520  dense_area: The 
-00001160: 746f 7461 6c20 6e75 6d62 6572 206f 6620  total number of 
-00001170: 7069 7865 6c73 2069 6e20 7468 6520 696e  pixels in the in
-00001180: 7075 7420 696d 6167 6520 7468 6174 2063  put image that c
-00001190: 6f72 7265 7370 6f6e 7365 200d 0a20 2020  orresponse ..   
-000011a0: 2020 2020 2020 2020 2074 6f20 6e6f 6e2d           to non-
-000011b0: 6465 6e73 6520 7469 7373 7565 2e20 2869  dense tissue. (i
-000011c0: 2e65 2e2c 206e 6f6e 2d66 6962 726f 676c  .e., non-fibrogl
-000011d0: 616e 6475 6c61 7229 0d0a 2020 2020 2020  andular)..      
-000011e0: 2020 2020 2020 2d20 6465 6e73 655f 6172        - dense_ar
-000011f0: 6561 3a20 5468 6520 746f 7461 6c20 6e75  ea: The total nu
-00001200: 6d62 6572 206f 6620 7069 7865 6c73 2069  mber of pixels i
-00001210: 6e20 7468 6520 696e 7075 7420 696d 6167  n the input imag
-00001220: 6520 7468 6174 2063 6f72 7265 7370 6f6e  e that correspon
-00001230: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
-00001240: 746f 2064 656e 7365 2074 6973 7375 652e  to dense tissue.
-00001250: 2028 692e 652e 2c20 6669 6272 6f67 6c61   (i.e., fibrogla
-00001260: 6e64 756c 6172 290d 0a20 2020 2020 2020  ndular)..       
-00001270: 2020 2020 202d 2070 6572 6365 6e74 6167       - percentag
-00001280: 655f 6465 6e73 6974 793a 2054 6865 2070  e_density: The p
-00001290: 6572 6365 6e74 6167 6520 6f66 206d 616d  ercentage of mam
-000012a0: 6d6f 6772 616d 2064 656e 7369 7479 2069  mogram density i
-000012b0: 6e20 7468 6520 696e 7075 7420 696d 6167  n the input imag
-000012c0: 652e 0d0a 2020 2020 5261 6973 6573 3a0d  e...    Raises:.
-000012d0: 0a20 2020 2020 2020 2054 7970 6545 7272  .        TypeErr
-000012e0: 6f72 3a20 4966 2060 6d6f 6465 6c60 2069  or: If `model` i
-000012f0: 7320 6e6f 7420 6120 7374 7269 6e67 206f  s not a string o
-00001300: 7220 6069 6d61 6765 5f70 6174 6860 2069  r `image_path` i
-00001310: 7320 6e6f 7420 6120 7374 7269 6e67 2e0d  s not a string..
-00001320: 0a20 2020 2020 2020 2056 616c 7565 4572  .        ValueEr
-00001330: 726f 723a 2049 6620 606d 6f64 656c 6020  ror: If `model` 
-00001340: 6973 206e 6f74 2061 2076 616c 6964 2070  is not a valid p
-00001350: 7265 2d74 7261 696e 6564 206d 6f64 656c  re-trained model
-00001360: 206e 616d 6520 6f72 2060 696d 6167 655f   name or `image_
-00001370: 7061 7468 600d 0a20 2020 2020 2020 2064  path`..        d
-00001380: 6f65 7320 6e6f 7420 706f 696e 7420 746f  oes not point to
-00001390: 2061 2076 616c 6964 2069 6d61 6765 2066   a valid image f
-000013a0: 696c 652e 0d0a 2020 2020 2222 220d 0a0d  ile...    """...
-000013b0: 0a20 2020 2023 204c 6f61 6420 7468 6520  .    # Load the 
-000013c0: 7072 652d 7472 6169 6e65 6420 6d6f 6465  pre-trained mode
-000013d0: 6c20 7765 6967 6874 730d 0a20 2020 2023  l weights..    #
-000013e0: 6d6f 6465 6c20 3d20 6c6f 6164 5f6d 6f64  model = load_mod
-000013f0: 656c 286d 6f64 656c 290d 0a0d 0a20 2020  el(model)....   
-00001400: 2023 204c 6f61 6420 7468 6520 696e 7075   # Load the inpu
-00001410: 7420 696d 6167 6520 616e 6420 636f 6e76  t image and conv
-00001420: 6572 7420 6974 2074 6f20 6120 5079 546f  ert it to a PyTo
-00001430: 7263 6820 7465 6e73 6f72 0d0a 2020 2020  rch tensor..    
-00001440: 696d 6167 6520 3d20 496d 6167 652e 6f70  image = Image.op
-00001450: 656e 2869 6d61 6765 5f70 6174 6829 2e63  en(image_path).c
-00001460: 6f6e 7665 7274 2827 5247 4227 290d 0a20  onvert('RGB').. 
-00001470: 2020 2069 6d67 203d 2069 6d61 6765 5f74     img = image_t
-00001480: 656e 736f 7228 696d 6167 6529 0d0a 0d0a  ensor(image)....
-00001490: 2020 2020 2320 436f 6d70 7574 6520 7468      # Compute th
-000014a0: 6520 6d61 6d6d 6f67 7261 6d20 6465 6e73  e mammogram dens
-000014b0: 6974 790d 0a20 2020 2072 6573 756c 7420  ity..    result 
-000014c0: 3d20 7b7d 0d0a 2020 2020 7072 6564 312c  = {}..    pred1,
-000014d0: 2070 7265 6432 203d 206d 6f64 656c 2e6d   pred2 = model.m
-000014e0: 6f64 756c 652e 7072 6564 6963 7428 696d  odule.predict(im
-000014f0: 6729 0d0a 2020 2020 0d0a 2020 2020 7072  g)..    ..    pr
-00001500: 6564 3120 3d20 7072 6564 315b 305d 2e63  ed1 = pred1[0].c
-00001510: 7075 2829 2e6e 756d 7079 2829 2e74 7261  pu().numpy().tra
-00001520: 6e73 706f 7365 2831 2c20 322c 2030 290d  nspose(1, 2, 0).
-00001530: 0a20 2020 2070 7265 6431 203d 2070 7265  .    pred1 = pre
-00001540: 6431 5b3a 2c20 3a2c 2030 5d0d 0a0d 0a20  d1[:, :, 0].... 
-00001550: 2020 2070 7265 6432 203d 2070 7265 6432     pred2 = pred2
-00001560: 5b30 5d2e 6370 7528 292e 6e75 6d70 7928  [0].cpu().numpy(
-00001570: 292e 7472 616e 7370 6f73 6528 312c 2032  ).transpose(1, 2
-00001580: 2c20 3029 0d0a 2020 2020 7072 6564 3220  , 0)..    pred2 
-00001590: 3d20 7072 6564 325b 3a2c 203a 2c20 305d  = pred2[:, :, 0]
-000015a0: 0d0a 0d0a 2020 2020 6272 6561 7374 5f61  ....    breast_a
-000015b0: 7265 6120 3d20 6e70 2e73 756d 286e 702e  rea = np.sum(np.
-000015c0: 6172 7261 7928 7072 6564 3129 203d 3d20  array(pred1) == 
-000015d0: 3129 0d0a 2020 2020 6465 6e73 655f 6172  1)..    dense_ar
-000015e0: 6561 203d 206e 702e 7375 6d28 6e70 2e61  ea = np.sum(np.a
-000015f0: 7272 6179 2870 7265 6432 2920 3d3d 2031  rray(pred2) == 1
-00001600: 290d 0a20 2020 2064 656e 7369 7479 203d  )..    density =
-00001610: 2028 6465 6e73 655f 6172 6561 202f 2062   (dense_area / b
-00001620: 7265 6173 745f 6172 6561 2920 2a20 3130  reast_area) * 10
-00001630: 300d 0a20 2020 200d 0a20 2020 2023 2050  0..    ..    # P
-00001640: 6f70 756c 6174 6520 7468 6520 7265 7375  opulate the resu
-00001650: 6c74 2064 6963 7469 6f6e 6172 7920 7769  lt dictionary wi
-00001660: 7468 2074 6865 2063 6f6d 7075 7465 6420  th the computed 
-00001670: 7661 6c75 6573 0d0a 2020 2020 7265 7375  values..    resu
-00001680: 6c74 5b22 6e6f 6e5f 6465 6e73 655f 6172  lt["non_dense_ar
-00001690: 6561 225d 203d 2062 7265 6173 745f 6172  ea"] = breast_ar
-000016a0: 6561 0d0a 2020 2020 7265 7375 6c74 5b22  ea..    result["
-000016b0: 6465 6e73 655f 6172 6561 225d 203d 2064  dense_area"] = d
-000016c0: 656e 7365 5f61 7265 610d 0a20 2020 2072  ense_area..    r
-000016d0: 6573 756c 745b 2270 6572 6365 6e74 6167  esult["percentag
-000016e0: 655f 6465 6e73 6974 7922 5d20 3d20 6465  e_density"] = de
-000016f0: 6e73 6974 790d 0a20 2020 200d 0a20 2020  nsity..    ..   
-00001700: 2072 6574 7572 6e20 7265 7375 6c74 0d0a   return result..
-00001710: 0d0a 6465 6620 6361 6e6e 795f 6564 6765  ..def canny_edge
-00001720: 7328 696d 6167 655f 6172 7261 7929 3a0d  s(image_array):.
-00001730: 0a20 2020 2022 2222 0d0a 2020 2020 4465  .    """..    De
-00001740: 7465 6374 2065 6467 6573 2075 7369 6e67  tect edges using
-00001750: 2074 6865 2043 616e 6e79 2061 6c67 6f72   the Canny algor
-00001760: 6974 686d 2e0d 0a20 2020 200d 0a20 2020  ithm...    ..   
-00001770: 2050 6172 616d 6574 6572 733a 0d0a 2020   Parameters:..  
-00001780: 2020 696d 6167 655f 6172 7261 7920 286e    image_array (n
-00001790: 756d 7079 2e6e 6461 7272 6179 293a 2054  umpy.ndarray): T
-000017a0: 6865 2069 6e70 7574 2069 6d61 6765 2061  he input image a
-000017b0: 7272 6179 0d0a 2020 2020 0d0a 2020 2020  rray..    ..    
-000017c0: 5265 7475 726e 733a 0d0a 2020 2020 6564  Returns:..    ed
-000017d0: 6765 7320 286e 756d 7079 2e6e 6461 7272  ges (numpy.ndarr
-000017e0: 6179 293a 2041 2062 696e 6172 7920 6564  ay): A binary ed
-000017f0: 6765 206d 6170 2077 6974 6820 6465 7465  ge map with dete
-00001800: 6374 6564 2065 6467 6573 206d 6172 6b65  cted edges marke
-00001810: 6420 7769 7468 2031 2e0d 0a20 2020 200d  d with 1...    .
-00001820: 0a20 2020 2052 6169 7365 733a 0d0a 2020  .    Raises:..  
-00001830: 2020 5479 7065 4572 726f 723a 2049 6620    TypeError: If 
-00001840: 7468 6520 696e 7075 7420 696d 6167 6520  the input image 
-00001850: 6973 206e 6f74 2061 206e 756d 7079 2061  is not a numpy a
-00001860: 7272 6179 2e0d 0a20 2020 2022 2222 0d0a  rray...    """..
-00001870: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
-00001880: 7461 6e63 6528 696d 6167 655f 6172 7261  tance(image_arra
-00001890: 792c 206e 702e 6e64 6172 7261 7929 3a0d  y, np.ndarray):.
-000018a0: 0a20 2020 2020 2020 2072 6169 7365 2054  .        raise T
-000018b0: 7970 6545 7272 6f72 2822 496e 7075 7420  ypeError("Input 
-000018c0: 696d 6167 6520 6d75 7374 2062 6520 6120  image must be a 
-000018d0: 6e75 6d70 7920 6172 7261 792e 2229 0d0a  numpy array.")..
-000018e0: 2020 2020 0d0a 2020 2020 2320 4465 7465      ..    # Dete
-000018f0: 6374 2065 6467 6573 2075 7369 6e67 2043  ct edges using C
-00001900: 616e 6e79 2061 6c67 6f72 6974 686d 2077  anny algorithm w
-00001910: 6974 6820 7369 676d 6120 7661 6c75 6520  ith sigma value 
-00001920: 6f66 2033 2e0d 0a20 2020 2065 6467 6573  of 3...    edges
-00001930: 203d 2066 6561 7475 7265 2e63 616e 6e79   = feature.canny
-00001940: 2869 6d61 6765 5f61 7272 6179 2c20 7369  (image_array, si
-00001950: 676d 613d 3329 0d0a 2020 2020 0d0a 2020  gma=3)..    ..  
-00001960: 2020 7265 7475 726e 2065 6467 6573 0d0a    return edges..
-00001970: 0d0a 2020 2020 0d0a 6465 6620 7669 7375  ..    ..def visu
-00001980: 616c 697a 6528 6d6f 6465 6c2c 2069 6d61  alize(model, ima
-00001990: 6765 5f70 6174 682c 6272 6561 7374 5f73  ge_path,breast_s
-000019a0: 6567 6d65 6e74 6174 696f 6e3d 5472 7565  egmentation=True
-000019b0: 2c20 6465 6e73 655f 7365 676d 656e 7461  , dense_segmenta
-000019c0: 7469 6f6e 3d54 7275 6529 3a0d 0a20 2020  tion=True):..   
-000019d0: 2022 2222 0d0a 2020 2020 5468 6973 2066   """..    This f
-000019e0: 756e 6374 696f 6e20 6973 2075 7365 6420  unction is used 
-000019f0: 746f 2076 6973 7561 6c69 7a65 2074 6865  to visualize the
-00001a00: 2073 6567 6d65 6e74 6174 696f 6e20 7265   segmentation re
-00001a10: 7375 6c74 7320 6f66 206d 616d 6d6f 6772  sults of mammogr
-00001a20: 6170 6879 2069 6d61 6765 7320 7573 696e  aphy images usin
-00001a30: 6720 6120 6465 6570 206c 6561 726e 696e  g a deep learnin
-00001a40: 6720 6d6f 6465 6c2e 0d0a 2020 2020 4172  g model...    Ar
-00001a50: 6773 3a0d 0a20 2020 202d 206d 6f64 656c  gs:..    - model
-00001a60: 3a20 5079 546f 7263 6820 6d6f 6465 6c20  : PyTorch model 
-00001a70: 7573 6564 2066 6f72 2073 6567 6d65 6e74  used for segment
-00001a80: 6174 696f 6e2e 0d0a 2020 2020 2d20 696d  ation...    - im
-00001a90: 6167 655f 7061 7468 3a20 5061 7468 2074  age_path: Path t
-00001aa0: 6f20 7468 6520 6d61 6d6d 6f67 7261 7068  o the mammograph
-00001ab0: 7920 696d 6167 652e 0d0a 2020 2020 2d20  y image...    - 
-00001ac0: 6272 6561 7374 5f73 6567 6d65 6e74 6174  breast_segmentat
-00001ad0: 696f 6e3a 2042 6f6f 6c65 616e 2069 6e64  ion: Boolean ind
-00001ae0: 6963 6174 696e 6720 7768 6574 6865 7220  icating whether 
-00001af0: 746f 2064 6973 706c 6179 2074 6865 2062  to display the b
-00001b00: 7265 6173 7420 6172 6561 2063 6f6e 746f  reast area conto
-00001b10: 7572 206f 7220 6e6f 742e 0d0a 2020 2020  ur or not...    
-00001b20: 2d20 6465 6e73 655f 7365 676d 656e 7461  - dense_segmenta
-00001b30: 7469 6f6e 3a20 426f 6f6c 6561 6e20 696e  tion: Boolean in
-00001b40: 6469 6361 7469 6e67 2077 6865 7468 6572  dicating whether
-00001b50: 2074 6f20 6469 7370 6c61 7920 7468 6520   to display the 
-00001b60: 6465 6e73 6520 7469 7373 7565 2073 6567  dense tissue seg
-00001b70: 6d65 6e74 6174 696f 6e20 6f72 206e 6f74  mentation or not
-00001b80: 2e0d 0a20 2020 2052 6574 7572 6e73 3a0d  ...    Returns:.
-00001b90: 0a20 2020 202d 204e 6f6e 650d 0a20 2020  .    - None..   
-00001ba0: 2052 6169 7365 733a 0d0a 2020 2020 2d20   Raises:..    - 
-00001bb0: 5479 7065 4572 726f 723a 2049 6620 6d6f  TypeError: If mo
-00001bc0: 6465 6c20 6973 206e 6f74 2061 2050 7954  del is not a PyT
-00001bd0: 6f72 6368 206d 6f64 656c 206f 7220 6966  orch model or if
-00001be0: 2069 6d61 6765 5f70 6174 6820 6973 206e   image_path is n
-00001bf0: 6f74 2061 2073 7472 696e 672e 0d0a 2020  ot a string...  
-00001c00: 2020 2d20 5661 6c75 6545 7272 6f72 3a20    - ValueError: 
-00001c10: 4966 2062 7265 6173 745f 7365 676d 656e  If breast_segmen
-00001c20: 7461 7469 6f6e 2061 6e64 2064 656e 7365  tation and dense
-00001c30: 5f73 6567 6d65 6e74 6174 696f 6e20 6172  _segmentation ar
-00001c40: 6520 626f 7468 2046 616c 7365 2e0d 0a20  e both False... 
-00001c50: 2020 2022 2222 0d0a 2020 2020 0d0a 2020     """..    ..  
-00001c60: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-00001c70: 6e63 6528 6d6f 6465 6c2c 2074 6f72 6368  nce(model, torch
-00001c80: 2e6e 6e2e 4d6f 6475 6c65 293a 0d0a 2020  .nn.Module):..  
-00001c90: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
-00001ca0: 4572 726f 7228 224d 6f64 656c 206d 7573  Error("Model mus
-00001cb0: 7420 6265 2061 2050 7954 6f72 6368 206d  t be a PyTorch m
-00001cc0: 6f64 656c 2e22 290d 0a20 2020 2069 6620  odel.")..    if 
-00001cd0: 6e6f 7420 6973 696e 7374 616e 6365 2869  not isinstance(i
-00001ce0: 6d61 6765 5f70 6174 682c 2073 7472 293a  mage_path, str):
-00001cf0: 0d0a 2020 2020 2020 2020 7261 6973 6520  ..        raise 
-00001d00: 5479 7065 4572 726f 7228 2249 6d61 6765  TypeError("Image
-00001d10: 2070 6174 6820 6d75 7374 2062 6520 6120   path must be a 
-00001d20: 7374 7269 6e67 2e22 290d 0a20 2020 2069  string.")..    i
-00001d30: 6620 6e6f 7420 6272 6561 7374 5f73 6567  f not breast_seg
-00001d40: 6d65 6e74 6174 696f 6e20 616e 6420 6e6f  mentation and no
-00001d50: 7420 6465 6e73 655f 7365 676d 656e 7461  t dense_segmenta
-00001d60: 7469 6f6e 3a0d 0a20 2020 2020 2020 2072  tion:..        r
-00001d70: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00001d80: 2241 7420 6c65 6173 7420 6f6e 6520 6f66  "At least one of
-00001d90: 2062 7265 6173 745f 7365 676d 656e 7461   breast_segmenta
-00001da0: 7469 6f6e 2061 6e64 2064 656e 7365 5f73  tion and dense_s
-00001db0: 6567 6d65 6e74 6174 696f 6e20 6d75 7374  egmentation must
-00001dc0: 2062 6520 5472 7565 2e22 290d 0a0d 0a20   be True.").... 
-00001dd0: 2020 2023 204c 6f61 6420 616e 6420 7072     # Load and pr
-00001de0: 6570 726f 6365 7373 2074 6865 2069 6d61  eprocess the ima
-00001df0: 6765 0d0a 2020 2020 696d 6167 6520 3d20  ge..    image = 
-00001e00: 496d 6167 652e 6f70 656e 2869 6d61 6765  Image.open(image
-00001e10: 5f70 6174 6829 2e63 6f6e 7665 7274 2827  _path).convert('
-00001e20: 5247 4227 290d 0a20 2020 2069 6d67 203d  RGB')..    img =
-00001e30: 2069 6d61 6765 5f74 656e 736f 7228 696d   image_tensor(im
-00001e40: 6167 6529 0d0a 0d0a 2020 2020 2320 4d61  age)....    # Ma
-00001e50: 6b65 2070 7265 6469 6374 696f 6e73 2075  ke predictions u
-00001e60: 7369 6e67 2074 6865 206d 6f64 656c 0d0a  sing the model..
-00001e70: 2020 2020 7072 6564 312c 2070 7265 6432      pred1, pred2
-00001e80: 203d 206d 6f64 656c 2e6d 6f64 756c 652e   = model.module.
-00001e90: 7072 6564 6963 7428 696d 6729 0d0a 0d0a  predict(img)....
-00001ea0: 2020 2020 2320 436f 6e76 6572 7420 7072      # Convert pr
-00001eb0: 6564 6963 7469 6f6e 7320 746f 206e 756d  edictions to num
-00001ec0: 7079 2061 7272 6179 730d 0a20 2020 2069  py arrays..    i
-00001ed0: 6d67 203d 2069 6d67 5b30 5d2e 6370 7528  mg = img[0].cpu(
-00001ee0: 292e 6e75 6d70 7928 292e 7472 616e 7370  ).numpy().transp
-00001ef0: 6f73 6528 312c 2032 2c20 3029 0d0a 2020  ose(1, 2, 0)..  
-00001f00: 2020 696d 6720 3d20 696d 675b 3a2c 203a    img = img[:, :
-00001f10: 2c20 305d 0d0a 0d0a 2020 2020 7072 6564  , 0]....    pred
-00001f20: 3120 3d20 7072 6564 315b 305d 2e63 7075  1 = pred1[0].cpu
-00001f30: 2829 2e6e 756d 7079 2829 2e74 7261 6e73  ().numpy().trans
-00001f40: 706f 7365 2831 2c20 322c 2030 290d 0a20  pose(1, 2, 0).. 
-00001f50: 2020 2070 7265 6431 203d 2070 7265 6431     pred1 = pred1
-00001f60: 5b3a 2c20 3a2c 2030 5d0d 0a0d 0a20 2020  [:, :, 0]....   
-00001f70: 2070 7265 6432 203d 2070 7265 6432 5b30   pred2 = pred2[0
-00001f80: 5d2e 6370 7528 292e 6e75 6d70 7928 292e  ].cpu().numpy().
-00001f90: 7472 616e 7370 6f73 6528 312c 2032 2c20  transpose(1, 2, 
-00001fa0: 3029 0d0a 2020 2020 7072 6564 3220 3d20  0)..    pred2 = 
-00001fb0: 7072 6564 325b 3a2c 203a 2c20 305d 0d0a  pred2[:, :, 0]..
-00001fc0: 0d0a 2020 2020 2320 4765 6e65 7261 7465  ..    # Generate
-00001fd0: 2062 7265 6173 7420 6172 6561 2063 6f6e   breast area con
-00001fe0: 746f 7572 2075 7369 6e67 2043 616e 6e79  tour using Canny
-00001ff0: 2065 6467 6520 6465 7465 6374 696f 6e0d   edge detection.
-00002000: 0a20 2020 2062 7265 6173 745f 636f 6e74  .    breast_cont
-00002010: 6f75 7220 3d20 6361 6e6e 795f 6564 6765  our = canny_edge
-00002020: 7328 7072 6564 3129 0d0a 0d0a 2020 2020  s(pred1)....    
-00002030: 2320 4469 7370 6c61 7920 7468 6520 7365  # Display the se
-00002040: 676d 656e 7461 7469 6f6e 2072 6573 756c  gmentation resul
-00002050: 7473 0d0a 2020 2020 6966 2062 7265 6173  ts..    if breas
-00002060: 745f 7365 676d 656e 7461 7469 6f6e 2061  t_segmentation a
-00002070: 6e64 206e 6f74 2064 656e 7365 5f73 6567  nd not dense_seg
-00002080: 6d65 6e74 6174 696f 6e3a 0d0a 2020 2020  mentation:..    
-00002090: 2020 2020 706c 742e 7469 746c 6528 2742      plt.title('B
-000020a0: 7265 6173 7420 6172 6561 2063 6f6e 746f  reast area conto
-000020b0: 7572 2729 0d0a 2020 2020 2020 2020 706c  ur')..        pl
-000020c0: 742e 696d 7368 6f77 2869 6d67 2c20 636d  t.imshow(img, cm
-000020d0: 6170 3d27 6772 6179 2729 0d0a 2020 2020  ap='gray')..    
-000020e0: 2020 2020 706c 742e 696d 7368 6f77 286d      plt.imshow(m
-000020f0: 6173 6b5f 746f 5f72 6762 6128 6272 6561  ask_to_rgba(brea
-00002100: 7374 5f63 6f6e 746f 7572 2c20 636f 6c6f  st_contour, colo
-00002110: 723d 2772 6564 2729 2c20 636d 6170 3d27  r='red'), cmap='
-00002120: 6772 6179 2729 0d0a 2020 2020 2020 2020  gray')..        
-00002130: 706c 742e 6178 6973 2827 6f66 6627 290d  plt.axis('off').
-00002140: 0a20 2020 2020 2020 2070 6c74 2e73 686f  .        plt.sho
-00002150: 7728 290d 0a0d 0a20 2020 2069 6620 6465  w()....    if de
-00002160: 6e73 655f 7365 676d 656e 7461 7469 6f6e  nse_segmentation
-00002170: 2061 6e64 206e 6f74 2062 7265 6173 745f   and not breast_
-00002180: 7365 676d 656e 7461 7469 6f6e 3a0d 0a20  segmentation:.. 
-00002190: 2020 2020 2020 2070 6c74 2e74 6974 6c65         plt.title
-000021a0: 2827 4465 6e73 6520 7469 7373 7565 7327  ('Dense tissues'
-000021b0: 290d 0a20 2020 2020 2020 2070 6c74 2e69  )..        plt.i
-000021c0: 6d73 686f 7728 696d 672c 2063 6d61 703d  mshow(img, cmap=
-000021d0: 2767 7261 7927 290d 0a20 2020 2020 2020  'gray')..       
-000021e0: 2070 6c74 2e69 6d73 686f 7728 6d61 736b   plt.imshow(mask
-000021f0: 5f74 6f5f 7267 6261 2870 7265 6432 2c20  _to_rgba(pred2, 
-00002200: 636f 6c6f 723d 2767 7265 656e 2729 2c20  color='green'), 
-00002210: 636d 6170 3d27 6772 6179 2729 0d0a 2020  cmap='gray')..  
-00002220: 2020 2020 2020 706c 742e 6178 6973 2827        plt.axis('
-00002230: 6f66 6627 290d 0a20 2020 2020 2020 2070  off')..        p
-00002240: 6c74 2e73 686f 7728 290d 0a0d 0a20 2020  lt.show()....   
-00002250: 2069 6620 6272 6561 7374 5f73 6567 6d65   if breast_segme
-00002260: 6e74 6174 696f 6e20 616e 6420 6465 6e73  ntation and dens
-00002270: 655f 7365 676d 656e 7461 7469 6f6e 3a0d  e_segmentation:.
-00002280: 0a20 2020 2020 2020 2066 6967 2c20 6178  .        fig, ax
-00002290: 6573 203d 2070 6c74 2e73 7562 706c 6f74  es = plt.subplot
-000022a0: 7328 312c 2032 2c20 6669 6773 697a 653d  s(1, 2, figsize=
-000022b0: 2832 302c 2031 3529 2c20 7371 7565 657a  (20, 15), squeez
-000022c0: 653d 4661 6c73 6529 0d0a 2020 2020 0d0a  e=False)..    ..
-000022d0: 2020 2020 2020 2020 6178 6573 5b30 2c20          axes[0, 
-000022e0: 305d 2e73 6574 5f74 6974 6c65 2827 496d  0].set_title('Im
-000022f0: 6167 6527 2c20 666f 6e74 7369 7a65 3d32  age', fontsize=2
-00002300: 3529 0d0a 2020 2020 2020 2020 6178 6573  5)..        axes
-00002310: 5b30 2c20 315d 2e73 6574 5f74 6974 6c65  [0, 1].set_title
-00002320: 2822 4272 6561 7374 2061 6e64 2064 656e  ("Breast and den
-00002330: 7365 2074 6973 7375 6520 7365 676d 656e  se tissue segmen
-00002340: 7461 7469 6f6e 222c 2066 6f6e 7473 697a  tation", fontsiz
-00002350: 653d 3235 290d 0a20 2020 2020 200d 0a20  e=25)..      .. 
-00002360: 2020 2020 2020 2061 7865 735b 302c 2030         axes[0, 0
-00002370: 5d2e 696d 7368 6f77 2869 6d67 2c20 636d  ].imshow(img, cm
-00002380: 6170 3d27 6772 6179 2729 0d0a 2020 2020  ap='gray')..    
-00002390: 2020 2020 6178 6573 5b30 2c20 305d 2e73      axes[0, 0].s
-000023a0: 6574 5f61 7869 735f 6f66 6628 290d 0a0d  et_axis_off()...
-000023b0: 0a20 2020 2020 2020 2061 7865 735b 302c  .        axes[0,
-000023c0: 2031 5d2e 696d 7368 6f77 2869 6d67 2c20   1].imshow(img, 
-000023d0: 636d 6170 3d27 6772 6179 2729 0d0a 2020  cmap='gray')..  
-000023e0: 2020 2020 2020 6178 6573 5b30 2c20 315d        axes[0, 1]
-000023f0: 2e69 6d73 686f 7728 6d61 736b 5f74 6f5f  .imshow(mask_to_
-00002400: 7267 6261 2862 7265 6173 745f 636f 6e74  rgba(breast_cont
-00002410: 6f75 722c 2063 6f6c 6f72 3d27 6772 6565  our, color='gree
-00002420: 6e27 292c 2063 6d61 703d 2767 7261 7927  n'), cmap='gray'
-00002430: 290d 0a20 2020 2020 2020 2061 7865 735b  )..        axes[
-00002440: 302c 2031 5d2e 696d 7368 6f77 286d 6173  0, 1].imshow(mas
-00002450: 6b5f 746f 5f72 6762 6128 7072 6564 322c  k_to_rgba(pred2,
-00002460: 2063 6f6c 6f72 3d27 7265 6427 292c 2063   color='red'), c
-00002470: 6d61 703d 2767 7261 7927 2c20 616c 7068  map='gray', alph
-00002480: 613d 302e 3529 0d0a 2020 2020 2020 2020  a=0.5)..        
-00002490: 6178 6573 5b30 2c20 315d 2e73 6574 5f61  axes[0, 1].set_a
-000024a0: 7869 735f 6f66 6628 290d 0a0d 0a20 2020  xis_off()....   
-000024b0: 2020 2020 2070 6c74 2e73 686f 7728 29         plt.show()
+00000000: 696d 706f 7274 206f 730d 0a69 6d70 6f72  import os..impor
+00000010: 7420 6e75 6d70 7920 6173 206e 700d 0a69  t numpy as np..i
+00000020: 6d70 6f72 7420 7265 7175 6573 7473 0d0a  mport requests..
+00000030: 6672 6f6d 2070 6174 686c 6962 2069 6d70  from pathlib imp
+00000040: 6f72 7420 5061 7468 0d0a 6672 6f6d 2073  ort Path..from s
+00000050: 6b69 6d61 6765 2069 6d70 6f72 7420 6665  kimage import fe
+00000060: 6174 7572 650d 0a69 6d70 6f72 7420 746f  ature..import to
+00000070: 7263 680d 0a69 6d70 6f72 7420 6d61 7470  rch..import matp
+00000080: 6c6f 746c 6962 2e70 7970 6c6f 7420 6173  lotlib.pyplot as
+00000090: 2070 6c74 0d0a 696d 706f 7274 2074 6f72   plt..import tor
+000000a0: 6368 2e6e 6e20 6173 206e 6e0d 0a69 6d70  ch.nn as nn..imp
+000000b0: 6f72 7420 6f73 2c20 696f 2c20 7079 6469  ort os, io, pydi
+000000c0: 636f 6d0d 0a69 6d70 6f72 7420 7469 6d65  com..import time
+000000d0: 0d0a 6672 6f6d 2074 6f72 6368 7669 7369  ..from torchvisi
+000000e0: 6f6e 2069 6d70 6f72 7420 7472 616e 7366  on import transf
+000000f0: 6f72 6d73 0d0a 6672 6f6d 2050 494c 2069  orms..from PIL i
+00000100: 6d70 6f72 7420 496d 6167 650d 0a0d 0a4d  mport Image....M
+00000110: 4153 4b5f 434f 4c4f 5253 203d 205b 2272  ASK_COLORS = ["r
+00000120: 6564 222c 2022 6772 6565 6e22 2c20 2262  ed", "green", "b
+00000130: 6c75 6522 2c20 2279 656c 6c6f 7722 2c20  lue", "yellow", 
+00000140: 226d 6167 656e 7461 222c 2022 6379 616e  "magenta", "cyan
+00000150: 225d 0d0a 0d0a 0d0a 6465 6620 6d61 736b  "]......def mask
+00000160: 5f74 6f5f 7267 6261 286d 6173 6b2c 2063  _to_rgba(mask, c
+00000170: 6f6c 6f72 3d22 7265 6422 293a 0d0a 2020  olor="red"):..  
+00000180: 2020 2222 220d 0a20 2020 2043 6f6e 7665    """..    Conve
+00000190: 7274 7320 6269 6e61 7279 2073 6567 6d65  rts binary segme
+000001a0: 6e74 6174 696f 6e20 6d61 736b 2066 726f  ntation mask fro
+000001b0: 6d20 7768 6974 6520 746f 2072 6564 2063  m white to red c
+000001c0: 6f6c 6f72 2e0d 0a20 2020 2041 6c73 6f20  olor...    Also 
+000001d0: 6164 6473 2061 6c70 6861 2063 6861 6e6e  adds alpha chann
+000001e0: 656c 2074 6f20 6d61 6b65 2062 6c61 636b  el to make black
+000001f0: 2062 6163 6b67 726f 756e 6420 7472 616e   background tran
+00000200: 7370 6172 656e 742e 0d0a 2020 2020 4172  sparent...    Ar
+00000210: 6773 3a0d 0a20 2020 2020 2020 206d 6173  gs:..        mas
+00000220: 6b20 286e 756d 7079 2e6e 6461 7272 6179  k (numpy.ndarray
+00000230: 293a 205b 6465 7363 7269 7074 696f 6e5d  ): [description]
+00000240: 0d0a 2020 2020 2020 2020 636f 6c6f 7220  ..        color 
+00000250: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
+00000260: 2043 6865 636b 2060 4d41 534b 5f43 4f4c   Check `MASK_COL
+00000270: 4f52 5360 2066 6f72 2061 7661 696c 6162  ORS` for availab
+00000280: 6c65 2063 6f6c 6f72 732e 2044 6566 6175  le colors. Defau
+00000290: 6c74 7320 746f 2022 7265 6422 2e0d 0a20  lts to "red"... 
+000002a0: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
+000002b0: 2020 2020 206e 756d 7079 2e6e 6461 7272       numpy.ndarr
+000002c0: 6179 3a20 5b64 6573 6372 6970 7469 6f6e  ay: [description
+000002d0: 5d0d 0a20 2020 2022 2222 0d0a 2020 2020  ]..    """..    
+000002e0: 6173 7365 7274 2063 6f6c 6f72 2069 6e20  assert color in 
+000002f0: 4d41 534b 5f43 4f4c 4f52 530d 0a20 2020  MASK_COLORS..   
+00000300: 2061 7373 6572 7420 6d61 736b 2e6e 6469   assert mask.ndi
+00000310: 6d20 3d3d 2033 206f 7220 6d61 736b 2e6e  m == 3 or mask.n
+00000320: 6469 6d20 3d3d 2032 0d0a 0d0a 2020 2020  dim == 2....    
+00000330: 6820 3d20 6d61 736b 2e73 6861 7065 5b30  h = mask.shape[0
+00000340: 5d0d 0a20 2020 2077 203d 206d 6173 6b2e  ]..    w = mask.
+00000350: 7368 6170 655b 315d 0d0a 2020 2020 7a65  shape[1]..    ze
+00000360: 726f 7320 3d20 6e70 2e7a 6572 6f73 2828  ros = np.zeros((
+00000370: 682c 2077 2929 0d0a 2020 2020 6f6e 6573  h, w))..    ones
+00000380: 203d 206d 6173 6b2e 7265 7368 6170 6528   = mask.reshape(
+00000390: 682c 2077 290d 0a20 2020 2069 6620 636f  h, w)..    if co
+000003a0: 6c6f 7220 3d3d 2022 7265 6422 3a0d 0a20  lor == "red":.. 
+000003b0: 2020 2020 2020 2072 6574 7572 6e20 6e70         return np
+000003c0: 2e73 7461 636b 2828 6f6e 6573 2c20 7a65  .stack((ones, ze
+000003d0: 726f 732c 207a 6572 6f73 2c20 6f6e 6573  ros, zeros, ones
+000003e0: 292c 2061 7869 733d 2d31 290d 0a20 2020  ), axis=-1)..   
+000003f0: 2065 6c69 6620 636f 6c6f 7220 3d3d 2022   elif color == "
+00000400: 6772 6565 6e22 3a0d 0a20 2020 2020 2020  green":..       
+00000410: 2072 6574 7572 6e20 6e70 2e73 7461 636b   return np.stack
+00000420: 2828 7a65 726f 732c 206f 6e65 732c 207a  ((zeros, ones, z
+00000430: 6572 6f73 2c20 6f6e 6573 292c 2061 7869  eros, ones), axi
+00000440: 733d 2d31 290d 0a20 2020 2065 6c69 6620  s=-1)..    elif 
+00000450: 636f 6c6f 7220 3d3d 2022 626c 7565 223a  color == "blue":
+00000460: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00000470: 206e 702e 7374 6163 6b28 287a 6572 6f73   np.stack((zeros
+00000480: 2c20 7a65 726f 732c 206f 6e65 732c 206f  , zeros, ones, o
+00000490: 6e65 7329 2c20 6178 6973 3d2d 3129 0d0a  nes), axis=-1)..
+000004a0: 2020 2020 656c 6966 2063 6f6c 6f72 203d      elif color =
+000004b0: 3d20 2279 656c 6c6f 7722 3a0d 0a20 2020  = "yellow":..   
+000004c0: 2020 2020 2072 6574 7572 6e20 6e70 2e73       return np.s
+000004d0: 7461 636b 2828 6f6e 6573 2c20 6f6e 6573  tack((ones, ones
+000004e0: 2c20 7a65 726f 732c 206f 6e65 7329 2c20  , zeros, ones), 
+000004f0: 6178 6973 3d2d 3129 0d0a 2020 2020 656c  axis=-1)..    el
+00000500: 6966 2063 6f6c 6f72 203d 3d20 226d 6167  if color == "mag
+00000510: 656e 7461 223a 0d0a 2020 2020 2020 2020  enta":..        
+00000520: 7265 7475 726e 206e 702e 7374 6163 6b28  return np.stack(
+00000530: 286f 6e65 732c 207a 6572 6f73 2c20 6f6e  (ones, zeros, on
+00000540: 6573 2c20 6f6e 6573 292c 2061 7869 733d  es, ones), axis=
+00000550: 2d31 290d 0a20 2020 2065 6c69 6620 636f  -1)..    elif co
+00000560: 6c6f 7220 3d3d 2022 6379 616e 223a 0d0a  lor == "cyan":..
+00000570: 2020 2020 2020 2020 7265 7475 726e 206e          return n
+00000580: 702e 7374 6163 6b28 287a 6572 6f73 2c20  p.stack((zeros, 
+00000590: 6f6e 6573 2c20 6f6e 6573 2c20 6f6e 6573  ones, ones, ones
+000005a0: 292c 2061 7869 733d 2d31 290d 0a0d 0a0d  ), axis=-1).....
+000005b0: 0a0d 0a64 6566 206c 6f61 645f 6d6f 6465  ...def load_mode
+000005c0: 6c28 6d6f 6465 6c5f 7061 7468 293a 0d0a  l(model_path):..
+000005d0: 2020 2020 2222 220d 0a20 2020 204c 6f61      """..    Loa
+000005e0: 6473 2061 2070 7265 2d74 7261 696e 6564  ds a pre-trained
+000005f0: 206d 6f64 656c 2066 726f 6d20 6120 6769   model from a gi
+00000600: 7665 6e20 7061 7468 2e0d 0a20 2020 2041  ven path...    A
+00000610: 7267 733a 0d0a 2020 2020 2d20 6d6f 6465  rgs:..    - mode
+00000620: 6c5f 7061 7468 3a20 7374 722c 2074 6865  l_path: str, the
+00000630: 2070 6174 6820 746f 2074 6865 2070 7265   path to the pre
+00000640: 2d74 7261 696e 6564 206d 6f64 656c 2e20  -trained model. 
+00000650: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000660: 2020 2020 4966 206d 6f64 656c 5f70 6174      If model_pat
+00000670: 6820 3d20 2762 6173 6527 2c20 7468 656e  h = 'base', then
+00000680: 2074 6865 2064 6566 6175 6c74 2070 7265   the default pre
+00000690: 2d74 7261 696e 6564 206d 6f64 656c 2077  -trained model w
+000006a0: 696c 6c20 6265 206c 6f61 6465 642e 0d0a  ill be loaded...
+000006b0: 2020 2020 0d0a 2020 2020 5265 7475 726e      ..    Return
+000006c0: 733a 0d0a 2020 2020 2d20 6d6f 6465 6c3a  s:..    - model:
+000006d0: 2074 6f72 6368 2e6e 6e2e 4d6f 6475 6c65   torch.nn.Module
+000006e0: 2c20 7468 6520 7072 652d 7472 6169 6e65  , the pre-traine
+000006f0: 6420 6d6f 6465 6c20 6c6f 6164 6564 2066  d model loaded f
+00000700: 726f 6d20 7468 6520 7370 6563 6966 6965  rom the specifie
+00000710: 6420 7061 7468 2e0d 0a20 2020 2052 6169  d path...    Rai
+00000720: 7365 733a 0d0a 2020 2020 2d20 5479 7065  ses:..    - Type
+00000730: 4572 726f 723a 2069 6620 7468 6520 696e  Error: if the in
+00000740: 7075 7420 6d6f 6465 6c5f 7061 7468 2069  put model_path i
+00000750: 7320 6e6f 7420 2762 6173 6527 2e0d 0a20  s not 'base'... 
+00000760: 2020 2022 2222 0d0a 2020 2020 0d0a 2020     """..    ..  
+00000770: 2020 6966 206d 6f64 656c 5f70 6174 6820    if model_path 
+00000780: 3d3d 2027 6261 7365 273a 0d0a 2020 2020  == 'base':..    
+00000790: 2020 2020 2320 4465 6669 6e65 2074 6865      # Define the
+000007a0: 2070 6174 6820 746f 2074 6865 2064 6566   path to the def
+000007b0: 6175 6c74 2070 7265 2d74 7261 696e 6564  ault pre-trained
+000007c0: 206d 6f64 656c 2077 6569 6768 7473 0d0a   model weights..
+000007d0: 2020 2020 2020 2020 6d6f 6465 6c5f 7765          model_we
+000007e0: 6967 6874 735f 7061 7468 203d 2022 7765  ights_path = "we
+000007f0: 6967 6874 732e 7074 6822 0d0a 2020 2020  ights.pth"..    
+00000800: 2020 2020 7061 7468 203d 2050 6174 6828      path = Path(
+00000810: 6d6f 6465 6c5f 7765 6967 6874 735f 7061  model_weights_pa
+00000820: 7468 290d 0a0d 0a20 2020 2020 2020 2023  th)....        #
+00000830: 2049 6620 7468 6520 6d6f 6465 6c20 7765   If the model we
+00000840: 6967 6874 7320 6669 6c65 2064 6f65 7320  ights file does 
+00000850: 6e6f 7420 6578 6973 742c 2064 6f77 6e6c  not exist, downl
+00000860: 6f61 6420 6974 2066 726f 6d20 4472 6f70  oad it from Drop
+00000870: 626f 780d 0a20 2020 2020 2020 2069 6620  box..        if 
+00000880: 6e6f 7420 7061 7468 2e69 735f 6669 6c65  not path.is_file
+00000890: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+000008a0: 2075 726c 203d 2022 6874 7470 733a 2f2f   url = "https://
+000008b0: 7777 772e 6472 6f70 626f 782e 636f 6d2f  www.dropbox.com/
+000008c0: 732f 3337 7274 6564 7777 6473 6c7a 3977  s/37rtedwwdslz9w
+000008d0: 362f 616c 6c5f 6461 7461 7365 7473 2e70  6/all_datasets.p
+000008e0: 7468 3f64 6c3d 3122 0d0a 2020 2020 2020  th?dl=1"..      
+000008f0: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
+00000900: 2072 6571 7565 7374 732e 6765 7428 7572   requests.get(ur
+00000910: 6c29 0d0a 2020 2020 2020 2020 2020 2020  l)..            
+00000920: 6f70 656e 2822 7765 6967 6874 732e 7074  open("weights.pt
+00000930: 6822 2c20 2277 6222 292e 7772 6974 6528  h", "wb").write(
+00000940: 7265 7370 6f6e 7365 2e63 6f6e 7465 6e74  response.content
+00000950: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
+00000960: 2020 2020 2023 204c 6f61 6420 7468 6520       # Load the 
+00000970: 7072 652d 7472 6169 6e65 6420 6d6f 6465  pre-trained mode
+00000980: 6c20 616e 6420 7365 7420 7468 6520 6465  l and set the de
+00000990: 7669 6365 2074 6f20 4350 550d 0a20 2020  vice to CPU..   
+000009a0: 2020 2020 206d 6f64 656c 203d 2074 6f72       model = tor
+000009b0: 6368 2e6c 6f61 6428 6d6f 6465 6c5f 7765  ch.load(model_we
+000009c0: 6967 6874 735f 7061 7468 2c20 6d61 705f  ights_path, map_
+000009d0: 6c6f 6361 7469 6f6e 3d74 6f72 6368 2e64  location=torch.d
+000009e0: 6576 6963 6528 2263 7075 2229 290d 0a20  evice("cpu")).. 
+000009f0: 2020 2020 2020 2023 2043 6f6e 7665 7274         # Convert
+00000a00: 2074 6865 206d 6f64 656c 2074 6f20 6265   the model to be
+00000a10: 2063 6f6d 7061 7469 626c 6520 7769 7468   compatible with
+00000a20: 206d 756c 7469 706c 6520 4750 5573 2c20   multiple GPUs, 
+00000a30: 6966 2061 7661 696c 6162 6c65 0d0a 2020  if available..  
+00000a40: 2020 2020 2020 6d6f 6465 6c20 3d20 6e6e        model = nn
+00000a50: 2e44 6174 6150 6172 616c 6c65 6c28 6d6f  .DataParallel(mo
+00000a60: 6465 6c2e 6d6f 6475 6c65 290d 0a20 2020  del.module)..   
+00000a70: 2020 2020 200d 0a20 2020 2020 2020 2072       ..        r
+00000a80: 6574 7572 6e20 6d6f 6465 6c0d 0a20 2020  eturn model..   
+00000a90: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00000aa0: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
+00000ab0: 224d 6f64 656c 206e 6f74 2069 6d70 6c65  "Model not imple
+00000ac0: 6d65 6e74 6564 2229 0d0a 0d0a 2020 2020  mented")....    
+00000ad0: 2020 2020 0d0a 0d0a 6465 6620 696d 6167      ....def imag
+00000ae0: 655f 7465 6e73 6f72 2869 6d67 293a 0d0a  e_tensor(img):..
+00000af0: 2020 2020 2222 220d 0a20 2020 2043 6f6e      """..    Con
+00000b00: 7665 7274 7320 6120 5049 4c20 496d 6167  verts a PIL Imag
+00000b10: 6520 6f72 204e 756d 5079 2061 7272 6179  e or NumPy array
+00000b20: 2074 6f20 6120 5079 546f 7263 6820 7465   to a PyTorch te
+00000b30: 6e73 6f72 2e0d 0a20 2020 2041 7267 733a  nsor...    Args:
+00000b40: 0d0a 2020 2020 2d20 696d 673a 2050 494c  ..    - img: PIL
+00000b50: 2e49 6d61 6765 206f 7220 6e70 2e6e 6461  .Image or np.nda
+00000b60: 7272 6179 2c20 7468 6520 696d 6167 6520  rray, the image 
+00000b70: 746f 2062 6520 636f 6e76 6572 7465 6420  to be converted 
+00000b80: 746f 2061 2050 7954 6f72 6368 2074 656e  to a PyTorch ten
+00000b90: 736f 722e 0d0a 2020 2020 5265 7475 726e  sor...    Return
+00000ba0: 733a 0d0a 2020 2020 2d20 696d 6167 653a  s:..    - image:
+00000bb0: 2074 6f72 6368 2e54 656e 736f 722c 2074   torch.Tensor, t
+00000bc0: 6865 2063 6f6e 7665 7274 6564 2050 7954  he converted PyT
+00000bd0: 6f72 6368 2074 656e 736f 722e 0d0a 2020  orch tensor...  
+00000be0: 2020 5261 6973 6573 3a0d 0a20 2020 202d    Raises:..    -
+00000bf0: 2054 7970 6545 7272 6f72 3a20 6966 2074   TypeError: if t
+00000c00: 6865 2069 6e70 7574 2069 6d61 6765 2069  he input image i
+00000c10: 7320 6e6f 7420 6120 5049 4c2e 496d 6167  s not a PIL.Imag
+00000c20: 6520 6f72 206e 702e 6e64 6172 7261 792e  e or np.ndarray.
+00000c30: 0d0a 2020 2020 2222 220d 0a20 2020 200d  ..    """..    .
+00000c40: 0a20 2020 2069 6620 7479 7065 2869 6d67  .    if type(img
+00000c50: 2920 6e6f 7420 696e 205b 6e70 2e6e 6461  ) not in [np.nda
+00000c60: 7272 6179 2c20 496d 6167 652e 496d 6167  rray, Image.Imag
+00000c70: 655d 3a0d 0a20 2020 2020 2020 2072 6169  e]:..        rai
+00000c80: 7365 2054 7970 6545 7272 6f72 2822 496e  se TypeError("In
+00000c90: 7075 7420 6d75 7374 2062 6520 6e70 2e6e  put must be np.n
+00000ca0: 6461 7272 6179 206f 7220 5049 4c2e 496d  darray or PIL.Im
+00000cb0: 6167 6522 290d 0a0d 0a20 2020 2023 2044  age")....    # D
+00000cc0: 6566 696e 6520 6120 5079 546f 7263 6820  efine a PyTorch 
+00000cd0: 7465 6e73 6f72 2074 7261 6e73 666f 726d  tensor transform
+00000ce0: 6572 2070 6970 656c 696e 650d 0a20 2020  er pipeline..   
+00000cf0: 2074 6f72 6368 5f74 656e 736f 7220 3d20   torch_tensor = 
+00000d00: 7472 616e 7366 6f72 6d73 2e43 6f6d 706f  transforms.Compo
+00000d10: 7365 280d 0a20 2020 2020 2020 205b 7472  se(..        [tr
+00000d20: 616e 7366 6f72 6d73 2e52 6573 697a 6528  ansforms.Resize(
+00000d30: 2832 3536 2c20 3235 3629 292c 2074 7261  (256, 256)), tra
+00000d40: 6e73 666f 726d 732e 546f 5465 6e73 6f72  nsforms.ToTensor
+00000d50: 2829 5d0d 0a20 2020 2029 0d0a 0d0a 2020  ()]..    )....  
+00000d60: 2020 6966 2074 7970 6528 696d 6729 203d    if type(img) =
+00000d70: 3d20 496d 6167 652e 496d 6167 653a 0d0a  = Image.Image:..
+00000d80: 2020 2020 2020 2020 2320 436f 6e76 6572          # Conver
+00000d90: 7420 5049 4c20 696d 6167 6520 746f 2050  t PIL image to P
+00000da0: 7954 6f72 6368 2074 656e 736f 720d 0a20  yTorch tensor.. 
+00000db0: 2020 2020 2020 2069 6d61 6765 203d 2074         image = t
+00000dc0: 6f72 6368 5f74 656e 736f 7228 696d 6729  orch_tensor(img)
+00000dd0: 0d0a 2020 2020 2020 2020 696d 6167 6520  ..        image 
+00000de0: 3d20 696d 6167 652e 756e 7371 7565 657a  = image.unsqueez
+00000df0: 6528 3029 0d0a 2020 2020 2020 2020 7072  e(0)..        pr
+00000e00: 696e 7428 2274 656e 736f 7222 2c20 7479  int("tensor", ty
+00000e10: 7065 2869 6d61 6765 2929 0d0a 2020 2020  pe(image))..    
+00000e20: 2020 2020 7265 7475 726e 2069 6d61 6765      return image
+00000e30: 0d0a 2020 2020 656c 6966 2074 7970 6528  ..    elif type(
+00000e40: 696d 6729 203d 3d20 6e70 2e6e 6461 7272  img) == np.ndarr
+00000e50: 6179 3a0d 0a20 2020 2020 2020 2023 2043  ay:..        # C
+00000e60: 6f6e 7665 7274 204e 756d 5079 2061 7272  onvert NumPy arr
+00000e70: 6179 2074 6f20 5247 4220 5049 4c20 696d  ay to RGB PIL im
+00000e80: 6167 6520 616e 6420 7468 656e 2074 6f20  age and then to 
+00000e90: 5079 546f 7263 6820 7465 6e73 6f72 0d0a  PyTorch tensor..
+00000ea0: 2020 2020 2020 2020 7069 6c5f 696d 6167          pil_imag
+00000eb0: 6520 3d20 496d 6167 652e 6672 6f6d 6172  e = Image.fromar
+00000ec0: 7261 7928 696d 6729 2e63 6f6e 7665 7274  ray(img).convert
+00000ed0: 2822 5247 4222 290d 0a20 2020 2020 2020  ("RGB")..       
+00000ee0: 2069 6d61 6765 203d 2074 6f72 6368 5f74   image = torch_t
+00000ef0: 656e 736f 7228 7069 6c5f 696d 6167 6529  ensor(pil_image)
+00000f00: 0d0a 2020 2020 2020 2020 696d 6167 6520  ..        image 
+00000f10: 3d20 696d 6167 652e 756e 7371 7565 657a  = image.unsqueez
+00000f20: 6528 3029 0d0a 2020 2020 2020 2020 7072  e(0)..        pr
+00000f30: 696e 7428 2274 656e 736f 7222 2c20 7479  int("tensor", ty
+00000f40: 7065 2869 6d61 6765 2929 0d0a 2020 2020  pe(image))..    
+00000f50: 2020 2020 7265 7475 726e 2069 6d61 6765      return image
+00000f60: 0d0a 2020 2020 656c 7365 3a0d 0a20 2020  ..    else:..   
+00000f70: 2020 2020 2072 6169 7365 2054 7970 6545       raise TypeE
+00000f80: 7272 6f72 2822 496e 7075 7420 6d75 7374  rror("Input must
+00000f90: 2062 6520 6e70 2e6e 6461 7272 6179 206f   be np.ndarray o
+00000fa0: 7220 5049 4c2e 496d 6167 6522 290d 0a0d  r PIL.Image")...
+00000fb0: 0a0d 0a0d 0a64 6566 2070 6572 6365 6e74  .....def percent
+00000fc0: 6167 655f 6465 6e73 6974 7928 6d6f 6465  age_density(mode
+00000fd0: 6c2c 2069 6d61 6765 5f70 6174 6829 3a0d  l, image_path):.
+00000fe0: 0a20 2020 2022 2222 0d0a 2020 2020 436f  .    """..    Co
+00000ff0: 6d70 7574 6573 2074 6865 2070 6572 6365  mputes the perce
+00001000: 6e74 6167 6520 6f66 206d 616d 6d6f 6772  ntage of mammogr
+00001010: 616d 2064 656e 7369 7479 2069 6e20 616e  am density in an
+00001020: 2069 6e70 7574 2069 6d61 6765 2e0d 0a20   input image... 
+00001030: 2020 2041 7267 733a 0d0a 2020 2020 2020     Args:..      
+00001040: 2020 6d6f 6465 6c20 2873 7472 293a 2054    model (str): T
+00001050: 6865 206e 616d 6520 6f66 2074 6865 2070  he name of the p
+00001060: 7265 2d74 7261 696e 6564 206d 6f64 656c  re-trained model
+00001070: 2074 6f20 7573 652e 0d0a 2020 2020 2020   to use...      
+00001080: 2020 696d 6167 655f 7061 7468 2028 7374    image_path (st
+00001090: 7229 3a20 5468 6520 7061 7468 2074 6f20  r): The path to 
+000010a0: 7468 6520 696e 7075 7420 696d 6167 6520  the input image 
+000010b0: 6669 6c65 2e0d 0a20 2020 2052 6574 7572  file...    Retur
+000010c0: 6e73 3a0d 0a20 2020 2020 2020 2064 6963  ns:..        dic
+000010d0: 743a 2041 2064 6963 7469 6f6e 6172 7920  t: A dictionary 
+000010e0: 636f 6e74 6169 6e69 6e67 2074 6865 2072  containing the r
+000010f0: 6573 756c 7473 206f 6620 7468 6520 636f  esults of the co
+00001100: 6d70 7574 6174 696f 6e2e 2054 6865 2064  mputation. The d
+00001110: 6963 7469 6f6e 6172 790d 0a20 2020 2020  ictionary..     
+00001120: 2020 2068 6173 2074 6865 2066 6f6c 6c6f     has the follo
+00001130: 7769 6e67 206b 6579 733a 0d0a 2020 2020  wing keys:..    
+00001140: 2020 2020 2020 2020 2d20 6e6f 6e5f 6465          - non_de
+00001150: 6e73 655f 6172 6561 3a20 5468 6520 746f  nse_area: The to
+00001160: 7461 6c20 6e75 6d62 6572 206f 6620 7069  tal number of pi
+00001170: 7865 6c73 2069 6e20 7468 6520 696e 7075  xels in the inpu
+00001180: 7420 696d 6167 6520 7468 6174 2063 6f72  t image that cor
+00001190: 7265 7370 6f6e 7365 200d 0a20 2020 2020  response ..     
+000011a0: 2020 2020 2020 2074 6f20 6e6f 6e2d 6465         to non-de
+000011b0: 6e73 6520 7469 7373 7565 2e20 2869 2e65  nse tissue. (i.e
+000011c0: 2e2c 206e 6f6e 2d66 6962 726f 676c 616e  ., non-fibroglan
+000011d0: 6475 6c61 7229 0d0a 2020 2020 2020 2020  dular)..        
+000011e0: 2020 2020 2d20 6465 6e73 655f 6172 6561      - dense_area
+000011f0: 3a20 5468 6520 746f 7461 6c20 6e75 6d62  : The total numb
+00001200: 6572 206f 6620 7069 7865 6c73 2069 6e20  er of pixels in 
+00001210: 7468 6520 696e 7075 7420 696d 6167 6520  the input image 
+00001220: 7468 6174 2063 6f72 7265 7370 6f6e 7365  that corresponse
+00001230: 0d0a 2020 2020 2020 2020 2020 2020 746f  ..            to
+00001240: 2064 656e 7365 2074 6973 7375 652e 2028   dense tissue. (
+00001250: 692e 652e 2c20 6669 6272 6f67 6c61 6e64  i.e., fibrogland
+00001260: 756c 6172 290d 0a20 2020 2020 2020 2020  ular)..         
+00001270: 2020 202d 2070 6572 6365 6e74 6167 655f     - percentage_
+00001280: 6465 6e73 6974 793a 2054 6865 2070 6572  density: The per
+00001290: 6365 6e74 6167 6520 6f66 206d 616d 6d6f  centage of mammo
+000012a0: 6772 616d 2064 656e 7369 7479 2069 6e20  gram density in 
+000012b0: 7468 6520 696e 7075 7420 696d 6167 652e  the input image.
+000012c0: 0d0a 2020 2020 5261 6973 6573 3a0d 0a20  ..    Raises:.. 
+000012d0: 2020 2020 2020 2054 7970 6545 7272 6f72         TypeError
+000012e0: 3a20 4966 2060 6d6f 6465 6c60 2069 7320  : If `model` is 
+000012f0: 6e6f 7420 6120 7374 7269 6e67 206f 7220  not a string or 
+00001300: 6069 6d61 6765 5f70 6174 6860 2069 7320  `image_path` is 
+00001310: 6e6f 7420 6120 7374 7269 6e67 2e0d 0a20  not a string... 
+00001320: 2020 2020 2020 2056 616c 7565 4572 726f         ValueErro
+00001330: 723a 2049 6620 606d 6f64 656c 6020 6973  r: If `model` is
+00001340: 206e 6f74 2061 2076 616c 6964 2070 7265   not a valid pre
+00001350: 2d74 7261 696e 6564 206d 6f64 656c 206e  -trained model n
+00001360: 616d 6520 6f72 2060 696d 6167 655f 7061  ame or `image_pa
+00001370: 7468 600d 0a20 2020 2020 2020 2064 6f65  th`..        doe
+00001380: 7320 6e6f 7420 706f 696e 7420 746f 2061  s not point to a
+00001390: 2076 616c 6964 2069 6d61 6765 2066 696c   valid image fil
+000013a0: 652e 0d0a 2020 2020 2222 220d 0a0d 0a20  e...    """.... 
+000013b0: 2020 2023 204c 6f61 6420 7468 6520 7072     # Load the pr
+000013c0: 652d 7472 6169 6e65 6420 6d6f 6465 6c20  e-trained model 
+000013d0: 7765 6967 6874 730d 0a20 2020 2023 6d6f  weights..    #mo
+000013e0: 6465 6c20 3d20 6c6f 6164 5f6d 6f64 656c  del = load_model
+000013f0: 286d 6f64 656c 290d 0a0d 0a20 2020 2023  (model)....    #
+00001400: 204c 6f61 6420 7468 6520 696e 7075 7420   Load the input 
+00001410: 696d 6167 6520 616e 6420 636f 6e76 6572  image and conver
+00001420: 7420 6974 2074 6f20 6120 5079 546f 7263  t it to a PyTorc
+00001430: 6820 7465 6e73 6f72 0d0a 2020 2020 696d  h tensor..    im
+00001440: 6167 6520 3d20 496d 6167 652e 6f70 656e  age = Image.open
+00001450: 2869 6d61 6765 5f70 6174 6829 2e63 6f6e  (image_path).con
+00001460: 7665 7274 2827 5247 4227 290d 0a20 2020  vert('RGB')..   
+00001470: 2069 6d67 203d 2069 6d61 6765 5f74 656e   img = image_ten
+00001480: 736f 7228 696d 6167 6529 0d0a 0d0a 2020  sor(image)....  
+00001490: 2020 2320 436f 6d70 7574 6520 7468 6520    # Compute the 
+000014a0: 6d61 6d6d 6f67 7261 6d20 6465 6e73 6974  mammogram densit
+000014b0: 790d 0a20 2020 2072 6573 756c 7420 3d20  y..    result = 
+000014c0: 7b7d 0d0a 2020 2020 7072 6564 312c 2070  {}..    pred1, p
+000014d0: 7265 6432 203d 206d 6f64 656c 2e6d 6f64  red2 = model.mod
+000014e0: 756c 652e 7072 6564 6963 7428 696d 6729  ule.predict(img)
+000014f0: 0d0a 2020 2020 0d0a 2020 2020 7072 6564  ..    ..    pred
+00001500: 3120 3d20 7072 6564 315b 305d 2e63 7075  1 = pred1[0].cpu
+00001510: 2829 2e6e 756d 7079 2829 2e74 7261 6e73  ().numpy().trans
+00001520: 706f 7365 2831 2c20 322c 2030 290d 0a20  pose(1, 2, 0).. 
+00001530: 2020 2070 7265 6431 203d 2070 7265 6431     pred1 = pred1
+00001540: 5b3a 2c20 3a2c 2030 5d0d 0a0d 0a20 2020  [:, :, 0]....   
+00001550: 2070 7265 6432 203d 2070 7265 6432 5b30   pred2 = pred2[0
+00001560: 5d2e 6370 7528 292e 6e75 6d70 7928 292e  ].cpu().numpy().
+00001570: 7472 616e 7370 6f73 6528 312c 2032 2c20  transpose(1, 2, 
+00001580: 3029 0d0a 2020 2020 7072 6564 3220 3d20  0)..    pred2 = 
+00001590: 7072 6564 325b 3a2c 203a 2c20 305d 0d0a  pred2[:, :, 0]..
+000015a0: 0d0a 2020 2020 6272 6561 7374 5f61 7265  ..    breast_are
+000015b0: 6120 3d20 6e70 2e73 756d 286e 702e 6172  a = np.sum(np.ar
+000015c0: 7261 7928 7072 6564 3129 203d 3d20 3129  ray(pred1) == 1)
+000015d0: 0d0a 2020 2020 6465 6e73 655f 6172 6561  ..    dense_area
+000015e0: 203d 206e 702e 7375 6d28 6e70 2e61 7272   = np.sum(np.arr
+000015f0: 6179 2870 7265 6432 2920 3d3d 2031 290d  ay(pred2) == 1).
+00001600: 0a20 2020 2064 656e 7369 7479 203d 2028  .    density = (
+00001610: 6465 6e73 655f 6172 6561 202f 2062 7265  dense_area / bre
+00001620: 6173 745f 6172 6561 2920 2a20 3130 300d  ast_area) * 100.
+00001630: 0a20 2020 200d 0a20 2020 2023 2050 6f70  .    ..    # Pop
+00001640: 756c 6174 6520 7468 6520 7265 7375 6c74  ulate the result
+00001650: 2064 6963 7469 6f6e 6172 7920 7769 7468   dictionary with
+00001660: 2074 6865 2063 6f6d 7075 7465 6420 7661   the computed va
+00001670: 6c75 6573 0d0a 2020 2020 7265 7375 6c74  lues..    result
+00001680: 5b22 6e6f 6e5f 6465 6e73 655f 6172 6561  ["non_dense_area
+00001690: 225d 203d 2062 7265 6173 745f 6172 6561  "] = breast_area
+000016a0: 0d0a 2020 2020 7265 7375 6c74 5b22 6465  ..    result["de
+000016b0: 6e73 655f 6172 6561 225d 203d 2064 656e  nse_area"] = den
+000016c0: 7365 5f61 7265 610d 0a20 2020 2072 6573  se_area..    res
+000016d0: 756c 745b 2270 6572 6365 6e74 6167 655f  ult["percentage_
+000016e0: 6465 6e73 6974 7922 5d20 3d20 6465 6e73  density"] = dens
+000016f0: 6974 790d 0a20 2020 200d 0a20 2020 2072  ity..    ..    r
+00001700: 6574 7572 6e20 7265 7375 6c74 0d0a 0d0a  eturn result....
+00001710: 6465 6620 6361 6e6e 795f 6564 6765 7328  def canny_edges(
+00001720: 696d 6167 655f 6172 7261 7929 3a0d 0a20  image_array):.. 
+00001730: 2020 2022 2222 0d0a 2020 2020 4465 7465     """..    Dete
+00001740: 6374 2065 6467 6573 2075 7369 6e67 2074  ct edges using t
+00001750: 6865 2043 616e 6e79 2061 6c67 6f72 6974  he Canny algorit
+00001760: 686d 2e0d 0a20 2020 200d 0a20 2020 2050  hm...    ..    P
+00001770: 6172 616d 6574 6572 733a 0d0a 2020 2020  arameters:..    
+00001780: 696d 6167 655f 6172 7261 7920 286e 756d  image_array (num
+00001790: 7079 2e6e 6461 7272 6179 293a 2054 6865  py.ndarray): The
+000017a0: 2069 6e70 7574 2069 6d61 6765 2061 7272   input image arr
+000017b0: 6179 0d0a 2020 2020 0d0a 2020 2020 5265  ay..    ..    Re
+000017c0: 7475 726e 733a 0d0a 2020 2020 6564 6765  turns:..    edge
+000017d0: 7320 286e 756d 7079 2e6e 6461 7272 6179  s (numpy.ndarray
+000017e0: 293a 2041 2062 696e 6172 7920 6564 6765  ): A binary edge
+000017f0: 206d 6170 2077 6974 6820 6465 7465 6374   map with detect
+00001800: 6564 2065 6467 6573 206d 6172 6b65 6420  ed edges marked 
+00001810: 7769 7468 2031 2e0d 0a20 2020 200d 0a20  with 1...    .. 
+00001820: 2020 2052 6169 7365 733a 0d0a 2020 2020     Raises:..    
+00001830: 5479 7065 4572 726f 723a 2049 6620 7468  TypeError: If th
+00001840: 6520 696e 7075 7420 696d 6167 6520 6973  e input image is
+00001850: 206e 6f74 2061 206e 756d 7079 2061 7272   not a numpy arr
+00001860: 6179 2e0d 0a20 2020 2022 2222 0d0a 2020  ay...    """..  
+00001870: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
+00001880: 6e63 6528 696d 6167 655f 6172 7261 792c  nce(image_array,
+00001890: 206e 702e 6e64 6172 7261 7929 3a0d 0a20   np.ndarray):.. 
+000018a0: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
+000018b0: 6545 7272 6f72 2822 496e 7075 7420 696d  eError("Input im
+000018c0: 6167 6520 6d75 7374 2062 6520 6120 6e75  age must be a nu
+000018d0: 6d70 7920 6172 7261 792e 2229 0d0a 2020  mpy array.")..  
+000018e0: 2020 0d0a 2020 2020 2320 4465 7465 6374    ..    # Detect
+000018f0: 2065 6467 6573 2075 7369 6e67 2043 616e   edges using Can
+00001900: 6e79 2061 6c67 6f72 6974 686d 2077 6974  ny algorithm wit
+00001910: 6820 7369 676d 6120 7661 6c75 6520 6f66  h sigma value of
+00001920: 2033 2e0d 0a20 2020 2065 6467 6573 203d   3...    edges =
+00001930: 2066 6561 7475 7265 2e63 616e 6e79 2869   feature.canny(i
+00001940: 6d61 6765 5f61 7272 6179 2c20 7369 676d  mage_array, sigm
+00001950: 613d 3329 0d0a 2020 2020 0d0a 2020 2020  a=3)..    ..    
+00001960: 7265 7475 726e 2065 6467 6573 0d0a 0d0a  return edges....
+00001970: 2020 2020 0d0a 6465 6620 7669 7375 616c      ..def visual
+00001980: 697a 6528 6d6f 6465 6c2c 2069 6d61 6765  ize(model, image
+00001990: 5f70 6174 682c 6272 6561 7374 5f73 6567  _path,breast_seg
+000019a0: 6d65 6e74 6174 696f 6e3d 5472 7565 2c20  mentation=True, 
+000019b0: 6465 6e73 655f 7365 676d 656e 7461 7469  dense_segmentati
+000019c0: 6f6e 3d54 7275 6529 3a0d 0a20 2020 2022  on=True):..    "
+000019d0: 2222 0d0a 2020 2020 5468 6973 2066 756e  ""..    This fun
+000019e0: 6374 696f 6e20 6973 2075 7365 6420 746f  ction is used to
+000019f0: 2076 6973 7561 6c69 7a65 2074 6865 2073   visualize the s
+00001a00: 6567 6d65 6e74 6174 696f 6e20 7265 7375  egmentation resu
+00001a10: 6c74 7320 6f66 206d 616d 6d6f 6772 6170  lts of mammograp
+00001a20: 6879 2069 6d61 6765 7320 7573 696e 6720  hy images using 
+00001a30: 6120 6465 6570 206c 6561 726e 696e 6720  a deep learning 
+00001a40: 6d6f 6465 6c2e 0d0a 2020 2020 4172 6773  model...    Args
+00001a50: 3a0d 0a20 2020 202d 206d 6f64 656c 3a20  :..    - model: 
+00001a60: 5079 546f 7263 6820 6d6f 6465 6c20 7573  PyTorch model us
+00001a70: 6564 2066 6f72 2073 6567 6d65 6e74 6174  ed for segmentat
+00001a80: 696f 6e2e 0d0a 2020 2020 2d20 696d 6167  ion...    - imag
+00001a90: 655f 7061 7468 3a20 5061 7468 2074 6f20  e_path: Path to 
+00001aa0: 7468 6520 6d61 6d6d 6f67 7261 7068 7920  the mammography 
+00001ab0: 696d 6167 652e 0d0a 2020 2020 2d20 6272  image...    - br
+00001ac0: 6561 7374 5f73 6567 6d65 6e74 6174 696f  east_segmentatio
+00001ad0: 6e3a 2042 6f6f 6c65 616e 2069 6e64 6963  n: Boolean indic
+00001ae0: 6174 696e 6720 7768 6574 6865 7220 746f  ating whether to
+00001af0: 2064 6973 706c 6179 2074 6865 2062 7265   display the bre
+00001b00: 6173 7420 6172 6561 2063 6f6e 746f 7572  ast area contour
+00001b10: 206f 7220 6e6f 742e 0d0a 2020 2020 2d20   or not...    - 
+00001b20: 6465 6e73 655f 7365 676d 656e 7461 7469  dense_segmentati
+00001b30: 6f6e 3a20 426f 6f6c 6561 6e20 696e 6469  on: Boolean indi
+00001b40: 6361 7469 6e67 2077 6865 7468 6572 2074  cating whether t
+00001b50: 6f20 6469 7370 6c61 7920 7468 6520 6465  o display the de
+00001b60: 6e73 6520 7469 7373 7565 2073 6567 6d65  nse tissue segme
+00001b70: 6e74 6174 696f 6e20 6f72 206e 6f74 2e0d  ntation or not..
+00001b80: 0a20 2020 2052 6574 7572 6e73 3a0d 0a20  .    Returns:.. 
+00001b90: 2020 202d 204e 6f6e 650d 0a20 2020 2052     - None..    R
+00001ba0: 6169 7365 733a 0d0a 2020 2020 2d20 5479  aises:..    - Ty
+00001bb0: 7065 4572 726f 723a 2049 6620 6d6f 6465  peError: If mode
+00001bc0: 6c20 6973 206e 6f74 2061 2050 7954 6f72  l is not a PyTor
+00001bd0: 6368 206d 6f64 656c 206f 7220 6966 2069  ch model or if i
+00001be0: 6d61 6765 5f70 6174 6820 6973 206e 6f74  mage_path is not
+00001bf0: 2061 2073 7472 696e 672e 0d0a 2020 2020   a string...    
+00001c00: 2d20 5661 6c75 6545 7272 6f72 3a20 4966  - ValueError: If
+00001c10: 2062 7265 6173 745f 7365 676d 656e 7461   breast_segmenta
+00001c20: 7469 6f6e 2061 6e64 2064 656e 7365 5f73  tion and dense_s
+00001c30: 6567 6d65 6e74 6174 696f 6e20 6172 6520  egmentation are 
+00001c40: 626f 7468 2046 616c 7365 2e0d 0a20 2020  both False...   
+00001c50: 2022 2222 0d0a 2020 2020 0d0a 2020 2020   """..    ..    
+00001c60: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+00001c70: 6528 6d6f 6465 6c2c 2074 6f72 6368 2e6e  e(model, torch.n
+00001c80: 6e2e 4d6f 6475 6c65 293a 0d0a 2020 2020  n.Module):..    
+00001c90: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
+00001ca0: 726f 7228 224d 6f64 656c 206d 7573 7420  ror("Model must 
+00001cb0: 6265 2061 2050 7954 6f72 6368 206d 6f64  be a PyTorch mod
+00001cc0: 656c 2e22 290d 0a20 2020 2069 6620 6e6f  el.")..    if no
+00001cd0: 7420 6973 696e 7374 616e 6365 2869 6d61  t isinstance(ima
+00001ce0: 6765 5f70 6174 682c 2073 7472 293a 0d0a  ge_path, str):..
+00001cf0: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
+00001d00: 7065 4572 726f 7228 2249 6d61 6765 2070  peError("Image p
+00001d10: 6174 6820 6d75 7374 2062 6520 6120 7374  ath must be a st
+00001d20: 7269 6e67 2e22 290d 0a20 2020 2069 6620  ring.")..    if 
+00001d30: 6e6f 7420 6272 6561 7374 5f73 6567 6d65  not breast_segme
+00001d40: 6e74 6174 696f 6e20 616e 6420 6e6f 7420  ntation and not 
+00001d50: 6465 6e73 655f 7365 676d 656e 7461 7469  dense_segmentati
+00001d60: 6f6e 3a0d 0a20 2020 2020 2020 2072 6169  on:..        rai
+00001d70: 7365 2056 616c 7565 4572 726f 7228 2241  se ValueError("A
+00001d80: 7420 6c65 6173 7420 6f6e 6520 6f66 2062  t least one of b
+00001d90: 7265 6173 745f 7365 676d 656e 7461 7469  reast_segmentati
+00001da0: 6f6e 2061 6e64 2064 656e 7365 5f73 6567  on and dense_seg
+00001db0: 6d65 6e74 6174 696f 6e20 6d75 7374 2062  mentation must b
+00001dc0: 6520 5472 7565 2e22 290d 0a0d 0a20 2020  e True.")....   
+00001dd0: 2023 204c 6f61 6420 616e 6420 7072 6570   # Load and prep
+00001de0: 726f 6365 7373 2074 6865 2069 6d61 6765  rocess the image
+00001df0: 0d0a 2020 2020 696d 6167 6520 3d20 496d  ..    image = Im
+00001e00: 6167 652e 6f70 656e 2869 6d61 6765 5f70  age.open(image_p
+00001e10: 6174 6829 2e63 6f6e 7665 7274 2827 5247  ath).convert('RG
+00001e20: 4227 290d 0a20 2020 2069 6d67 203d 2069  B')..    img = i
+00001e30: 6d61 6765 5f74 656e 736f 7228 696d 6167  mage_tensor(imag
+00001e40: 6529 0d0a 0d0a 2020 2020 2320 4d61 6b65  e)....    # Make
+00001e50: 2070 7265 6469 6374 696f 6e73 2075 7369   predictions usi
+00001e60: 6e67 2074 6865 206d 6f64 656c 0d0a 2020  ng the model..  
+00001e70: 2020 7072 6564 312c 2070 7265 6432 203d    pred1, pred2 =
+00001e80: 206d 6f64 656c 2e6d 6f64 756c 652e 7072   model.module.pr
+00001e90: 6564 6963 7428 696d 6729 0d0a 0d0a 2020  edict(img)....  
+00001ea0: 2020 2320 436f 6e76 6572 7420 7072 6564    # Convert pred
+00001eb0: 6963 7469 6f6e 7320 746f 206e 756d 7079  ictions to numpy
+00001ec0: 2061 7272 6179 730d 0a20 2020 2069 6d67   arrays..    img
+00001ed0: 203d 2069 6d67 5b30 5d2e 6370 7528 292e   = img[0].cpu().
+00001ee0: 6e75 6d70 7928 292e 7472 616e 7370 6f73  numpy().transpos
+00001ef0: 6528 312c 2032 2c20 3029 0d0a 2020 2020  e(1, 2, 0)..    
+00001f00: 696d 6720 3d20 696d 675b 3a2c 203a 2c20  img = img[:, :, 
+00001f10: 305d 0d0a 0d0a 2020 2020 7072 6564 3120  0]....    pred1 
+00001f20: 3d20 7072 6564 315b 305d 2e63 7075 2829  = pred1[0].cpu()
+00001f30: 2e6e 756d 7079 2829 2e74 7261 6e73 706f  .numpy().transpo
+00001f40: 7365 2831 2c20 322c 2030 290d 0a20 2020  se(1, 2, 0)..   
+00001f50: 2070 7265 6431 203d 2070 7265 6431 5b3a   pred1 = pred1[:
+00001f60: 2c20 3a2c 2030 5d0d 0a0d 0a20 2020 2070  , :, 0]....    p
+00001f70: 7265 6432 203d 2070 7265 6432 5b30 5d2e  red2 = pred2[0].
+00001f80: 6370 7528 292e 6e75 6d70 7928 292e 7472  cpu().numpy().tr
+00001f90: 616e 7370 6f73 6528 312c 2032 2c20 3029  anspose(1, 2, 0)
+00001fa0: 0d0a 2020 2020 7072 6564 3220 3d20 7072  ..    pred2 = pr
+00001fb0: 6564 325b 3a2c 203a 2c20 305d 0d0a 0d0a  ed2[:, :, 0]....
+00001fc0: 2020 2020 2320 4765 6e65 7261 7465 2062      # Generate b
+00001fd0: 7265 6173 7420 6172 6561 2063 6f6e 746f  reast area conto
+00001fe0: 7572 2075 7369 6e67 2043 616e 6e79 2065  ur using Canny e
+00001ff0: 6467 6520 6465 7465 6374 696f 6e0d 0a20  dge detection.. 
+00002000: 2020 2062 7265 6173 745f 636f 6e74 6f75     breast_contou
+00002010: 7220 3d20 6361 6e6e 795f 6564 6765 7328  r = canny_edges(
+00002020: 7072 6564 3129 0d0a 0d0a 2020 2020 2320  pred1)....    # 
+00002030: 4469 7370 6c61 7920 7468 6520 7365 676d  Display the segm
+00002040: 656e 7461 7469 6f6e 2072 6573 756c 7473  entation results
+00002050: 0d0a 2020 2020 6966 2062 7265 6173 745f  ..    if breast_
+00002060: 7365 676d 656e 7461 7469 6f6e 2061 6e64  segmentation and
+00002070: 206e 6f74 2064 656e 7365 5f73 6567 6d65   not dense_segme
+00002080: 6e74 6174 696f 6e3a 0d0a 2020 2020 2020  ntation:..      
+00002090: 2020 706c 742e 7469 746c 6528 2742 7265    plt.title('Bre
+000020a0: 6173 7420 6172 6561 2063 6f6e 746f 7572  ast area contour
+000020b0: 2729 0d0a 2020 2020 2020 2020 706c 742e  ')..        plt.
+000020c0: 696d 7368 6f77 2869 6d67 2c20 636d 6170  imshow(img, cmap
+000020d0: 3d27 6772 6179 2729 0d0a 2020 2020 2020  ='gray')..      
+000020e0: 2020 706c 742e 696d 7368 6f77 286d 6173    plt.imshow(mas
+000020f0: 6b5f 746f 5f72 6762 6128 6272 6561 7374  k_to_rgba(breast
+00002100: 5f63 6f6e 746f 7572 2c20 636f 6c6f 723d  _contour, color=
+00002110: 2772 6564 2729 2c20 636d 6170 3d27 6772  'red'), cmap='gr
+00002120: 6179 2729 0d0a 2020 2020 2020 2020 706c  ay')..        pl
+00002130: 742e 6178 6973 2827 6f66 6627 290d 0a20  t.axis('off').. 
+00002140: 2020 2020 2020 2070 6c74 2e73 686f 7728         plt.show(
+00002150: 290d 0a0d 0a20 2020 2069 6620 6465 6e73  )....    if dens
+00002160: 655f 7365 676d 656e 7461 7469 6f6e 2061  e_segmentation a
+00002170: 6e64 206e 6f74 2062 7265 6173 745f 7365  nd not breast_se
+00002180: 676d 656e 7461 7469 6f6e 3a0d 0a20 2020  gmentation:..   
+00002190: 2020 2020 2070 6c74 2e74 6974 6c65 2827       plt.title('
+000021a0: 4465 6e73 6520 7469 7373 7565 7327 290d  Dense tissues').
+000021b0: 0a20 2020 2020 2020 2070 6c74 2e69 6d73  .        plt.ims
+000021c0: 686f 7728 696d 672c 2063 6d61 703d 2767  how(img, cmap='g
+000021d0: 7261 7927 290d 0a20 2020 2020 2020 2070  ray')..        p
+000021e0: 6c74 2e69 6d73 686f 7728 6d61 736b 5f74  lt.imshow(mask_t
+000021f0: 6f5f 7267 6261 2870 7265 6432 2c20 636f  o_rgba(pred2, co
+00002200: 6c6f 723d 2767 7265 656e 2729 2c20 636d  lor='green'), cm
+00002210: 6170 3d27 6772 6179 2729 0d0a 2020 2020  ap='gray')..    
+00002220: 2020 2020 706c 742e 6178 6973 2827 6f66      plt.axis('of
+00002230: 6627 290d 0a20 2020 2020 2020 2070 6c74  f')..        plt
+00002240: 2e73 686f 7728 290d 0a0d 0a20 2020 2069  .show()....    i
+00002250: 6620 6272 6561 7374 5f73 6567 6d65 6e74  f breast_segment
+00002260: 6174 696f 6e20 616e 6420 6465 6e73 655f  ation and dense_
+00002270: 7365 676d 656e 7461 7469 6f6e 3a0d 0a20  segmentation:.. 
+00002280: 2020 2020 2020 2066 6967 2c20 6178 6573         fig, axes
+00002290: 203d 2070 6c74 2e73 7562 706c 6f74 7328   = plt.subplots(
+000022a0: 312c 2032 2c20 6669 6773 697a 653d 2832  1, 2, figsize=(2
+000022b0: 302c 2031 3529 2c20 7371 7565 657a 653d  0, 15), squeeze=
+000022c0: 4661 6c73 6529 0d0a 2020 2020 0d0a 2020  False)..    ..  
+000022d0: 2020 2020 2020 6178 6573 5b30 2c20 305d        axes[0, 0]
+000022e0: 2e73 6574 5f74 6974 6c65 2827 496d 6167  .set_title('Imag
+000022f0: 6527 2c20 666f 6e74 7369 7a65 3d32 3529  e', fontsize=25)
+00002300: 0d0a 2020 2020 2020 2020 6178 6573 5b30  ..        axes[0
+00002310: 2c20 315d 2e73 6574 5f74 6974 6c65 2822  , 1].set_title("
+00002320: 4272 6561 7374 2061 6e64 2064 656e 7365  Breast and dense
+00002330: 2074 6973 7375 6520 7365 676d 656e 7461   tissue segmenta
+00002340: 7469 6f6e 222c 2066 6f6e 7473 697a 653d  tion", fontsize=
+00002350: 3235 290d 0a20 2020 2020 200d 0a20 2020  25)..      ..   
+00002360: 2020 2020 2061 7865 735b 302c 2030 5d2e       axes[0, 0].
+00002370: 696d 7368 6f77 2869 6d67 2c20 636d 6170  imshow(img, cmap
+00002380: 3d27 6772 6179 2729 0d0a 2020 2020 2020  ='gray')..      
+00002390: 2020 6178 6573 5b30 2c20 305d 2e73 6574    axes[0, 0].set
+000023a0: 5f61 7869 735f 6f66 6628 290d 0a0d 0a20  _axis_off().... 
+000023b0: 2020 2020 2020 2061 7865 735b 302c 2031         axes[0, 1
+000023c0: 5d2e 696d 7368 6f77 2869 6d67 2c20 636d  ].imshow(img, cm
+000023d0: 6170 3d27 6772 6179 2729 0d0a 2020 2020  ap='gray')..    
+000023e0: 2020 2020 6178 6573 5b30 2c20 315d 2e69      axes[0, 1].i
+000023f0: 6d73 686f 7728 6d61 736b 5f74 6f5f 7267  mshow(mask_to_rg
+00002400: 6261 2862 7265 6173 745f 636f 6e74 6f75  ba(breast_contou
+00002410: 722c 2063 6f6c 6f72 3d27 6772 6565 6e27  r, color='green'
+00002420: 292c 2063 6d61 703d 2767 7261 7927 290d  ), cmap='gray').
+00002430: 0a20 2020 2020 2020 2061 7865 735b 302c  .        axes[0,
+00002440: 2031 5d2e 696d 7368 6f77 286d 6173 6b5f   1].imshow(mask_
+00002450: 746f 5f72 6762 6128 7072 6564 322c 2063  to_rgba(pred2, c
+00002460: 6f6c 6f72 3d27 7265 6427 292c 2063 6d61  olor='red'), cma
+00002470: 703d 2767 7261 7927 2c20 616c 7068 613d  p='gray', alpha=
+00002480: 302e 3529 0d0a 2020 2020 2020 2020 6178  0.5)..        ax
+00002490: 6573 5b30 2c20 315d 2e73 6574 5f61 7869  es[0, 1].set_axi
+000024a0: 735f 6f66 6628 290d 0a0d 0a20 2020 2020  s_off()....     
+000024b0: 2020 2070 6c74 2e73 686f 7728 29            plt.show()
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/heads.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/base/__pycache__/heads.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/heads.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/base/__pycache__/heads.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/heads.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/base/__pycache__/heads.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/heads.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/base/__pycache__/heads.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:18 2023 UTC, .py size: 532 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -27,29 +27,29 @@
 000001a0: 6172 3264 da08 4964 656e 7469 7479 7204  ar2d..Identityr.
 000001b0: 0000 00da 0573 7570 6572 da08 5f5f 696e  .....super..__in
 000001c0: 6974 5f5f 2907 da04 7365 6c66 da0b 696e  it__)...self..in
 000001d0: 5f63 6861 6e6e 656c 73da 0c6f 7574 5f63  _channels..out_c
 000001e0: 6861 6e6e 656c 7372 0800 0000 da0a 6163  hannelsr......ac
 000001f0: 7469 7661 7469 6f6e da0a 7570 7361 6d70  tivation..upsamp
 00000200: 6c69 6e67 da06 636f 6e76 3264 a901 da09  ling..conv2d....
-00000210: 5f5f 636c 6173 735f 5fa9 00fa 5143 3a5c  __class__...QC:\
+00000210: 5f5f 636c 6173 735f 5fa9 00fa 4463 3a5c  __class__...Dc:\
 00000220: 5573 6572 735c 6d68 616e 616e 5c44 6f77  Users\mhanan\Dow
-00000230: 6e6c 6f61 6473 5c48 616e 616e 5c4d 616d  nloads\Hanan\Mam
-00000240: 6d6f 5079 5c6d 616d 6d6f 7079 5c73 6567  moPy\mammopy\seg
-00000250: 6d65 6e74 6174 696f 6e5f 6d6f 6465 6c73  mentation_models
-00000260: 5c62 6173 655c 6865 6164 732e 7079 7210  \base\heads.pyr.
-00000270: 0000 0007 0000 0073 0800 0000 0001 1601  .......s........
-00000280: 1c01 0801 7a19 5365 676d 656e 7461 7469  ....z.Segmentati
-00000290: 6f6e 4865 6164 2e5f 5f69 6e69 745f 5f29  onHead.__init__)
-000002a0: 0372 0600 0000 4e72 0200 0000 2905 da08  .r....Nr....)...
-000002b0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-000002c0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-000002d0: 5f5f 7210 0000 00da 0d5f 5f63 6c61 7373  __r......__class
-000002e0: 6365 6c6c 5f5f 7219 0000 0072 1900 0000  cell__r....r....
-000002f0: 7217 0000 0072 1a00 0000 7205 0000 0005  r....r....r.....
-00000300: 0000 0073 0200 0000 0802 7205 0000 0029  ...s......r....)
-00000310: 07da 0874 6f72 6368 2e6e 6e72 0b00 0000  ...torch.nnr....
-00000320: da07 6d6f 6475 6c65 7372 0300 0000 7204  ..modulesr....r.
-00000330: 0000 00da 0a53 6571 7565 6e74 6961 6c72  .....Sequentialr
-00000340: 0500 0000 7219 0000 0072 1900 0000 7219  ....r....r....r.
-00000350: 0000 0072 1a00 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000360: 653e 0100 0000 7304 0000 000c 0110 03    e>....s........
+00000230: 6e6c 6f61 6473 5c48 616e 616e 5c6d 675c  nloads\Hanan\mg\
+00000240: 7365 676d 656e 7461 7469 6f6e 5f6d 6f64  segmentation_mod
+00000250: 656c 735c 6261 7365 5c68 6561 6473 2e70  els\base\heads.p
+00000260: 7972 1000 0000 0700 0000 7308 0000 0000  yr........s.....
+00000270: 0116 011c 0108 017a 1953 6567 6d65 6e74  .......z.Segment
+00000280: 6174 696f 6e48 6561 642e 5f5f 696e 6974  ationHead.__init
+00000290: 5f5f 2903 7206 0000 004e 7202 0000 0029  __).r....Nr....)
+000002a0: 05da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+000002b0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+000002c0: 616d 655f 5f72 1000 0000 da0d 5f5f 636c  ame__r......__cl
+000002d0: 6173 7363 656c 6c5f 5f72 1900 0000 7219  asscell__r....r.
+000002e0: 0000 0072 1700 0000 721a 0000 0072 0500  ...r....r....r..
+000002f0: 0000 0500 0000 7302 0000 0008 0272 0500  ......s......r..
+00000300: 0000 2907 da08 746f 7263 682e 6e6e 720b  ..)...torch.nnr.
+00000310: 0000 00da 076d 6f64 756c 6573 7203 0000  .....modulesr...
+00000320: 0072 0400 0000 da0a 5365 7175 656e 7469  .r......Sequenti
+00000330: 616c 7205 0000 0072 1900 0000 7219 0000  alr....r....r...
+00000340: 0072 1900 0000 721a 0000 00da 083c 6d6f  .r....r......<mo
+00000350: 6475 6c65 3e01 0000 0073 0400 0000 0c01  dule>....s......
+00000360: 1003                                     ..
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/heads.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/base/__pycache__/heads.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/initialization.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/base/__pycache__/initialization.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/initialization.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/base/__pycache__/initialization.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/initialization.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/base/__pycache__/initialization.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/initialization.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/base/__pycache__/initialization.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:18 2023 UTC, .py size: 848 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,58 @@
-00000000: 550d 0d0a 0000 0000 5277 1164 5003 0000  U.......Rw.dP...
+00000000: 610d 0d0a 0000 0000 5277 1164 5003 0000  a.......Rw.dP...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 8400  d.l.m.Z...d.d...
 00000040: 5a02 6404 6405 8400 5a03 6401 5300 2906  Z.d.d...Z.d.S.).
 00000050: e900 0000 004e 6301 0000 0000 0000 0000  .....Nc.........
 00000060: 0000 0002 0000 0006 0000 0043 0000 0073  ...........C...s
 00000070: b000 0000 7c00 a000 a100 4400 5da2 7d01  ....|.....D.].}.
 00000080: 7401 7c01 7402 6a03 8302 7248 7402 6a04  t.|.t.j...rHt.j.
 00000090: 6a05 7c01 6a06 6401 6402 6403 8d03 0100  j.|.j.d.d.d.....
-000000a0: 7c01 6a07 6400 6b09 72aa 7402 6a04 a008  |.j.d.k.r.t.j...
+000000a0: 7c01 6a07 6400 7501 72aa 7402 6a04 a008  |.j.d.u.r.t.j...
 000000b0: 7c01 6a07 6404 a102 0100 7108 7401 7c01  |.j.d.....q.t.|.
 000000c0: 7402 6a09 8302 7276 7402 6a04 a008 7c01  t.j...rvt.j...|.
 000000d0: 6a06 6405 a102 0100 7402 6a04 a008 7c01  j.d.....t.j...|.
 000000e0: 6a07 6404 a102 0100 7108 7401 7c01 7402  j.d.....q.t.|.t.
 000000f0: 6a0a 8302 7208 7402 6a04 a00b 7c01 6a06  j...r.t.j...|.j.
-00000100: a101 0100 7c01 6a07 6400 6b09 7208 7402  ....|.j.d.k.r.t.
+00000100: a101 0100 7c01 6a07 6400 7501 7208 7402  ....|.j.d.u.r.t.
 00000110: 6a04 a008 7c01 6a07 6404 a102 0100 7108  j...|.j.d.....q.
 00000120: 6400 5300 2906 4eda 0666 616e 5f69 6eda  d.S.).N..fan_in.
 00000130: 0472 656c 7529 02da 046d 6f64 65da 0c6e  .relu)...mode..n
 00000140: 6f6e 6c69 6e65 6172 6974 7972 0100 0000  onlinearityr....
 00000150: e901 0000 0029 0cda 076d 6f64 756c 6573  .....)...modules
 00000160: da0a 6973 696e 7374 616e 6365 da02 6e6e  ..isinstance..nn
 00000170: da06 436f 6e76 3264 da04 696e 6974 da10  ..Conv2d..init..
 00000180: 6b61 696d 696e 675f 756e 6966 6f72 6d5f  kaiming_uniform_
 00000190: da06 7765 6967 6874 da04 6269 6173 da09  ..weight..bias..
 000001a0: 636f 6e73 7461 6e74 5fda 0b42 6174 6368  constant_..Batch
 000001b0: 4e6f 726d 3264 da06 4c69 6e65 6172 da0f  Norm2d..Linear..
 000001c0: 7861 7669 6572 5f75 6e69 666f 726d 5fa9  xavier_uniform_.
 000001d0: 02da 066d 6f64 756c 65da 016d a900 7216  ...module..m..r.
-000001e0: 0000 00fa 5a43 3a5c 5573 6572 735c 6d68  ....ZC:\Users\mh
-000001f0: 616e 616e 5c44 6f77 6e6c 6f61 6473 5c48  anan\Downloads\H
-00000200: 616e 616e 5c4d 616d 6d6f 5079 5c6d 616d  anan\MammoPy\mam
-00000210: 6d6f 7079 5c73 6567 6d65 6e74 6174 696f  mopy\segmentatio
-00000220: 6e5f 6d6f 6465 6c73 5c62 6173 655c 696e  n_models\base\in
-00000230: 6974 6961 6c69 7a61 7469 6f6e 2e70 79da  itialization.py.
-00000240: 1269 6e69 7469 616c 697a 655f 6465 636f  .initialize_deco
-00000250: 6465 7204 0000 0073 1800 0000 0001 0c02  der....s........
-00000260: 0c01 1401 0a01 1202 0c01 1001 1202 0c01  ................
-00000270: 0e01 0a01 7218 0000 0063 0100 0000 0000  ....r....c......
-00000280: 0000 0000 0000 0200 0000 0500 0000 4300  ..............C.
-00000290: 0000 734c 0000 007c 00a0 00a1 0044 005d  ..sL...|.....D.]
-000002a0: 3e7d 0174 017c 0174 026a 0374 026a 0466  >}.t.|.t.j.t.j.f
-000002b0: 0283 0272 0874 026a 05a0 067c 016a 07a1  ...r.t.j...|.j..
-000002c0: 0101 007c 016a 0864 006b 0972 0874 026a  ...|.j.d.k.r.t.j
-000002d0: 05a0 097c 016a 0864 01a1 0201 0071 0864  ...|.j.d.....q.d
-000002e0: 0053 0029 024e 7201 0000 0029 0a72 0700  .S.).Nr....).r..
-000002f0: 0000 7208 0000 0072 0900 0000 7211 0000  ..r....r....r...
-00000300: 0072 0a00 0000 720b 0000 0072 1200 0000  .r....r....r....
-00000310: 720d 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
-00000320: 1300 0000 7216 0000 0072 1600 0000 7217  ....r....r....r.
-00000330: 0000 00da 0f69 6e69 7469 616c 697a 655f  .....initialize_
-00000340: 6865 6164 1600 0000 730a 0000 0000 010c  head....s.......
-00000350: 0112 010e 010a 0172 1900 0000 2904 da08  .......r....)...
-00000360: 746f 7263 682e 6e6e 7209 0000 0072 1800  torch.nnr....r..
-00000370: 0000 7219 0000 0072 1600 0000 7216 0000  ..r....r....r...
-00000380: 0072 1600 0000 7217 0000 00da 083c 6d6f  .r....r......<mo
-00000390: 6475 6c65 3e01 0000 0073 0400 0000 0c03  dule>....s......
-000003a0: 0812                                     ..
+000001e0: 0000 00fa 5843 3a5c 5573 6572 735c 6d68  ....XC:\Users\mh
+000001f0: 616e 616e 5c44 6573 6b74 6f70 5c44 656e  anan\Desktop\Den
+00000200: 7369 7479 4170 705c 4465 6e73 6974 7941  sityApp\DensityA
+00000210: 7070 5c73 6567 6d65 6e74 6174 696f 6e5f  pp\segmentation_
+00000220: 6d6f 6465 6c73 5c62 6173 655c 696e 6974  models\base\init
+00000230: 6961 6c69 7a61 7469 6f6e 2e70 79da 1269  ialization.py..i
+00000240: 6e69 7469 616c 697a 655f 6465 636f 6465  nitialize_decode
+00000250: 7204 0000 0073 1800 0000 0001 0c02 0c01  r....s..........
+00000260: 1401 0a01 1202 0c01 1001 1202 0c01 0e01  ................
+00000270: 0a01 7218 0000 0063 0100 0000 0000 0000  ..r....c........
+00000280: 0000 0000 0200 0000 0500 0000 4300 0000  ............C...
+00000290: 734c 0000 007c 00a0 00a1 0044 005d 3e7d  sL...|.....D.]>}
+000002a0: 0174 017c 0174 026a 0374 026a 0466 0283  .t.|.t.j.t.j.f..
+000002b0: 0272 0874 026a 05a0 067c 016a 07a1 0101  .r.t.j...|.j....
+000002c0: 007c 016a 0864 0075 0172 0874 026a 05a0  .|.j.d.u.r.t.j..
+000002d0: 097c 016a 0864 01a1 0201 0071 0864 0053  .|.j.d.....q.d.S
+000002e0: 0029 024e 7201 0000 0029 0a72 0700 0000  .).Nr....).r....
+000002f0: 7208 0000 0072 0900 0000 7211 0000 0072  r....r....r....r
+00000300: 0a00 0000 720b 0000 0072 1200 0000 720d  ....r....r....r.
+00000310: 0000 0072 0e00 0000 720f 0000 0072 1300  ...r....r....r..
+00000320: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00000330: 00da 0f69 6e69 7469 616c 697a 655f 6865  ...initialize_he
+00000340: 6164 1600 0000 730a 0000 0000 010c 0112  ad....s.........
+00000350: 010e 010a 0172 1900 0000 2904 da08 746f  .....r....)...to
+00000360: 7263 682e 6e6e 7209 0000 0072 1800 0000  rch.nnr....r....
+00000370: 7219 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
+00000380: 1600 0000 7217 0000 00da 083c 6d6f 6475  ....r......<modu
+00000390: 6c65 3e01 0000 0073 0400 0000 0c03 0812  le>....s........
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/initialization.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/base/__pycache__/initialization.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Mar 15 07:44:18 2023 UTC, .py size: 848 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-00000000: 610d 0d0a 0000 0000 5277 1164 5003 0000  a.......Rw.dP...
+00000000: 550d 0d0a 0000 0000 5277 1164 5003 0000  U.......Rw.dP...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 8400  d.l.m.Z...d.d...
 00000040: 5a02 6404 6405 8400 5a03 6401 5300 2906  Z.d.d...Z.d.S.).
 00000050: e900 0000 004e 6301 0000 0000 0000 0000  .....Nc.........
 00000060: 0000 0002 0000 0006 0000 0043 0000 0073  ...........C...s
 00000070: b000 0000 7c00 a000 a100 4400 5da2 7d01  ....|.....D.].}.
 00000080: 7401 7c01 7402 6a03 8302 7248 7402 6a04  t.|.t.j...rHt.j.
 00000090: 6a05 7c01 6a06 6401 6402 6403 8d03 0100  j.|.j.d.d.d.....
-000000a0: 7c01 6a07 6400 7501 72aa 7402 6a04 a008  |.j.d.u.r.t.j...
+000000a0: 7c01 6a07 6400 6b09 72aa 7402 6a04 a008  |.j.d.k.r.t.j...
 000000b0: 7c01 6a07 6404 a102 0100 7108 7401 7c01  |.j.d.....q.t.|.
 000000c0: 7402 6a09 8302 7276 7402 6a04 a008 7c01  t.j...rvt.j...|.
 000000d0: 6a06 6405 a102 0100 7402 6a04 a008 7c01  j.d.....t.j...|.
 000000e0: 6a07 6404 a102 0100 7108 7401 7c01 7402  j.d.....q.t.|.t.
 000000f0: 6a0a 8302 7208 7402 6a04 a00b 7c01 6a06  j...r.t.j...|.j.
-00000100: a101 0100 7c01 6a07 6400 7501 7208 7402  ....|.j.d.u.r.t.
+00000100: a101 0100 7c01 6a07 6400 6b09 7208 7402  ....|.j.d.k.r.t.
 00000110: 6a04 a008 7c01 6a07 6404 a102 0100 7108  j...|.j.d.....q.
 00000120: 6400 5300 2906 4eda 0666 616e 5f69 6eda  d.S.).N..fan_in.
 00000130: 0472 656c 7529 02da 046d 6f64 65da 0c6e  .relu)...mode..n
 00000140: 6f6e 6c69 6e65 6172 6974 7972 0100 0000  onlinearityr....
 00000150: e901 0000 0029 0cda 076d 6f64 756c 6573  .....)...modules
 00000160: da0a 6973 696e 7374 616e 6365 da02 6e6e  ..isinstance..nn
 00000170: da06 436f 6e76 3264 da04 696e 6974 da10  ..Conv2d..init..
 00000180: 6b61 696d 696e 675f 756e 6966 6f72 6d5f  kaiming_uniform_
 00000190: da06 7765 6967 6874 da04 6269 6173 da09  ..weight..bias..
 000001a0: 636f 6e73 7461 6e74 5fda 0b42 6174 6368  constant_..Batch
 000001b0: 4e6f 726d 3264 da06 4c69 6e65 6172 da0f  Norm2d..Linear..
 000001c0: 7861 7669 6572 5f75 6e69 666f 726d 5fa9  xavier_uniform_.
 000001d0: 02da 066d 6f64 756c 65da 016d a900 7216  ...module..m..r.
-000001e0: 0000 00fa 5843 3a5c 5573 6572 735c 6d68  ....XC:\Users\mh
-000001f0: 616e 616e 5c44 6573 6b74 6f70 5c44 656e  anan\Desktop\Den
-00000200: 7369 7479 4170 705c 4465 6e73 6974 7941  sityApp\DensityA
-00000210: 7070 5c73 6567 6d65 6e74 6174 696f 6e5f  pp\segmentation_
-00000220: 6d6f 6465 6c73 5c62 6173 655c 696e 6974  models\base\init
-00000230: 6961 6c69 7a61 7469 6f6e 2e70 79da 1269  ialization.py..i
-00000240: 6e69 7469 616c 697a 655f 6465 636f 6465  nitialize_decode
-00000250: 7204 0000 0073 1800 0000 0001 0c02 0c01  r....s..........
-00000260: 1401 0a01 1202 0c01 1001 1202 0c01 0e01  ................
-00000270: 0a01 7218 0000 0063 0100 0000 0000 0000  ..r....c........
-00000280: 0000 0000 0200 0000 0500 0000 4300 0000  ............C...
-00000290: 734c 0000 007c 00a0 00a1 0044 005d 3e7d  sL...|.....D.]>}
-000002a0: 0174 017c 0174 026a 0374 026a 0466 0283  .t.|.t.j.t.j.f..
-000002b0: 0272 0874 026a 05a0 067c 016a 07a1 0101  .r.t.j...|.j....
-000002c0: 007c 016a 0864 0075 0172 0874 026a 05a0  .|.j.d.u.r.t.j..
-000002d0: 097c 016a 0864 01a1 0201 0071 0864 0053  .|.j.d.....q.d.S
-000002e0: 0029 024e 7201 0000 0029 0a72 0700 0000  .).Nr....).r....
-000002f0: 7208 0000 0072 0900 0000 7211 0000 0072  r....r....r....r
-00000300: 0a00 0000 720b 0000 0072 1200 0000 720d  ....r....r....r.
-00000310: 0000 0072 0e00 0000 720f 0000 0072 1300  ...r....r....r..
-00000320: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00000330: 00da 0f69 6e69 7469 616c 697a 655f 6865  ...initialize_he
-00000340: 6164 1600 0000 730a 0000 0000 010c 0112  ad....s.........
-00000350: 010e 010a 0172 1900 0000 2904 da08 746f  .....r....)...to
-00000360: 7263 682e 6e6e 7209 0000 0072 1800 0000  rch.nnr....r....
-00000370: 7219 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
-00000380: 1600 0000 7217 0000 00da 083c 6d6f 6475  ....r......<modu
-00000390: 6c65 3e01 0000 0073 0400 0000 0c03 0812  le>....s........
+000001e0: 0000 00fa 4d63 3a5c 5573 6572 735c 6d68  ....Mc:\Users\mh
+000001f0: 616e 616e 5c44 6f77 6e6c 6f61 6473 5c48  anan\Downloads\H
+00000200: 616e 616e 5c6d 675c 7365 676d 656e 7461  anan\mg\segmenta
+00000210: 7469 6f6e 5f6d 6f64 656c 735c 6261 7365  tion_models\base
+00000220: 5c69 6e69 7469 616c 697a 6174 696f 6e2e  \initialization.
+00000230: 7079 da12 696e 6974 6961 6c69 7a65 5f64  py..initialize_d
+00000240: 6563 6f64 6572 0400 0000 7318 0000 0000  ecoder....s.....
+00000250: 010c 020c 0114 010a 0112 020c 0110 0112  ................
+00000260: 020c 010e 010a 0172 1800 0000 6301 0000  .......r....c...
+00000270: 0000 0000 0000 0000 0002 0000 0005 0000  ................
+00000280: 0043 0000 0073 4c00 0000 7c00 a000 a100  .C...sL...|.....
+00000290: 4400 5d3e 7d01 7401 7c01 7402 6a03 7402  D.]>}.t.|.t.j.t.
+000002a0: 6a04 6602 8302 7208 7402 6a05 a006 7c01  j.f...r.t.j...|.
+000002b0: 6a07 a101 0100 7c01 6a08 6400 6b09 7208  j.....|.j.d.k.r.
+000002c0: 7402 6a05 a009 7c01 6a08 6401 a102 0100  t.j...|.j.d.....
+000002d0: 7108 6400 5300 2902 4e72 0100 0000 290a  q.d.S.).Nr....).
+000002e0: 7207 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
+000002f0: 1100 0000 720a 0000 0072 0b00 0000 7212  ....r....r....r.
+00000300: 0000 0072 0d00 0000 720e 0000 0072 0f00  ...r....r....r..
+00000310: 0000 7213 0000 0072 1600 0000 7216 0000  ..r....r....r...
+00000320: 0072 1700 0000 da0f 696e 6974 6961 6c69  .r......initiali
+00000330: 7a65 5f68 6561 6416 0000 0073 0a00 0000  ze_head....s....
+00000340: 0001 0c01 1201 0e01 0a01 7219 0000 0029  ..........r....)
+00000350: 04da 0874 6f72 6368 2e6e 6e72 0900 0000  ...torch.nnr....
+00000360: 7218 0000 0072 1900 0000 7216 0000 0072  r....r....r....r
+00000370: 1600 0000 7216 0000 0072 1700 0000 da08  ....r....r......
+00000380: 3c6d 6f64 756c 653e 0100 0000 7304 0000  <module>....s...
+00000390: 000c 0308 12                             .....
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/model.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/base/__pycache__/model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/model.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/base/__pycache__/model.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/model.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/base/__pycache__/model.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/model.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/base/__pycache__/model.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:18 2023 UTC, .py size: 1294 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -21,80 +21,80 @@
 00000140: 72da 0c6d 6173 6b5f 6465 636f 6465 725a  r..mask_decoderZ
 00000150: 0f69 6e69 7469 616c 697a 655f 6865 6164  .initialize_head
 00000160: da16 6d61 736b 5f73 6567 6d65 6e74 6174  ..mask_segmentat
 00000170: 696f 6e5f 6865 6164 da0f 636f 6e74 6f75  ion_head..contou
 00000180: 725f 6465 636f 6465 72da 1963 6f6e 746f  r_decoder..conto
 00000190: 7572 5f73 6567 6d65 6e74 6174 696f 6e5f  ur_segmentation_
 000001a0: 6865 6164 2901 da04 7365 6c66 a900 720b  head)...self..r.
-000001b0: 0000 00fa 5143 3a5c 5573 6572 735c 6d68  ....QC:\Users\mh
+000001b0: 0000 00fa 4463 3a5c 5573 6572 735c 6d68  ....Dc:\Users\mh
 000001c0: 616e 616e 5c44 6f77 6e6c 6f61 6473 5c48  anan\Downloads\H
-000001d0: 616e 616e 5c4d 616d 6d6f 5079 5c6d 616d  anan\MammoPy\mam
-000001e0: 6d6f 7079 5c73 6567 6d65 6e74 6174 696f  mopy\segmentatio
-000001f0: 6e5f 6d6f 6465 6c73 5c62 6173 655c 6d6f  n_models\base\mo
-00000200: 6465 6c2e 7079 da0a 696e 6974 6961 6c69  del.py..initiali
-00000210: 7a65 0700 0000 7308 0000 0000 010c 010c  ze....s.........
-00000220: 010c 017a 1c53 6567 6d65 6e74 6174 696f  ...z.Segmentatio
-00000230: 6e4d 6f64 656c 2e69 6e69 7469 616c 697a  nModel.initializ
-00000240: 6563 0200 0000 0000 0000 0000 0000 0700  ec..............
-00000250: 0000 0300 0000 4300 0000 733a 0000 007c  ......C...s:...|
-00000260: 00a0 007c 01a1 017d 027c 006a 017c 028e  ...|...}.|.j.|..
-00000270: 007d 037c 00a0 027c 03a1 017d 047c 006a  .}.|...|...}.|.j
-00000280: 037c 028e 007d 057c 00a0 047c 05a1 017d  .|...}.|...|...}
-00000290: 067c 047c 0666 0253 0029 017a 3f53 6571  .|.|.f.S.).z?Seq
-000002a0: 7565 6e74 6961 6c6c 7920 7061 7373 2060  uentially pass `
-000002b0: 7860 2074 726f 7567 6820 6d6f 6465 6c60  x` trough model`
-000002c0: 7320 656e 636f 6465 722c 2064 6563 6f64  s encoder, decod
-000002d0: 6572 2061 6e64 2068 6561 6473 2905 da07  er and heads)...
-000002e0: 656e 636f 6465 7272 0600 0000 7207 0000  encoderr....r...
-000002f0: 0072 0800 0000 7209 0000 0029 0772 0a00  .r....r....).r..
-00000300: 0000 da01 78da 0866 6561 7475 7265 735a  ....x..featuresZ
-00000310: 136d 6173 6b5f 6465 636f 6465 725f 6f75  .mask_decoder_ou
-00000320: 7470 7574 da05 6d61 736b 735a 1663 6f6e  tput..masksZ.con
-00000330: 746f 7572 5f64 6563 6f64 6572 5f6f 7574  tour_decoder_out
-00000340: 7075 74da 0863 6f6e 746f 7572 7372 0b00  put..contoursr..
-00000350: 0000 720b 0000 0072 0c00 0000 da07 666f  ..r....r......fo
-00000360: 7277 6172 640d 0000 0073 0c00 0000 0002  rward....s......
-00000370: 0a02 0a01 0a02 0a01 0a02 7a19 5365 676d  ..........z.Segm
-00000380: 656e 7461 7469 6f6e 4d6f 6465 6c2e 666f  entationModel.fo
-00000390: 7277 6172 6463 0200 0000 0000 0000 0000  rwardc..........
-000003a0: 0000 0200 0000 0900 0000 4300 0000 7330  ..........C...s0
-000003b0: 0000 007c 006a 0072 0e7c 00a0 01a1 0001  ...|.j.r.|......
-000003c0: 0074 02a0 03a1 008f 1001 007c 00a0 047c  .t.........|...|
-000003d0: 01a1 017d 0157 0035 0051 0052 0058 007c  ...}.W.5.Q.R.X.|
-000003e0: 0153 0029 0161 2a01 0000 496e 6665 7265  .S.).a*...Infere
-000003f0: 6e63 6520 6d65 7468 6f64 2e20 5377 6974  nce method. Swit
-00000400: 6368 206d 6f64 656c 2074 6f20 6065 7661  ch model to `eva
-00000410: 6c60 206d 6f64 652c 2063 616c 6c20 602e  l` mode, call `.
-00000420: 666f 7277 6172 6428 7829 6020 7769 7468  forward(x)` with
-00000430: 2060 746f 7263 682e 6e6f 5f67 7261 6428   `torch.no_grad(
-00000440: 2960 0a0a 2020 2020 2020 2020 4172 6773  )`..        Args
-00000450: 3a0a 2020 2020 2020 2020 2020 2020 783a  :.            x:
-00000460: 2034 4420 746f 7263 6820 7465 6e73 6f72   4D torch tensor
-00000470: 2077 6974 6820 7368 6170 6520 2862 6174   with shape (bat
-00000480: 6368 5f73 697a 652c 2063 6861 6e6e 656c  ch_size, channel
-00000490: 732c 2068 6569 6768 742c 2077 6964 7468  s, height, width
-000004a0: 290a 0a20 2020 2020 2020 2052 6574 7572  )..        Retur
-000004b0: 6e3a 0a20 2020 2020 2020 2020 2020 2070  n:.            p
-000004c0: 7265 6469 6374 696f 6e3a 2034 4420 746f  rediction: 4D to
-000004d0: 7263 6820 7465 6e73 6f72 2077 6974 6820  rch tensor with 
-000004e0: 7368 6170 6520 2862 6174 6368 5f73 697a  shape (batch_siz
-000004f0: 652c 2063 6c61 7373 6573 2c20 6865 6967  e, classes, heig
-00000500: 6874 2c20 7769 6474 6829 0a0a 2020 2020  ht, width)..    
-00000510: 2020 2020 2905 da08 7472 6169 6e69 6e67      )...training
-00000520: da04 6576 616c da05 746f 7263 68da 076e  ..eval..torch..n
-00000530: 6f5f 6772 6164 7213 0000 0029 0272 0a00  o_gradr....).r..
-00000540: 0000 720f 0000 0072 0b00 0000 720b 0000  ..r....r....r...
-00000550: 0072 0c00 0000 da07 7072 6564 6963 7419  .r......predict.
-00000560: 0000 0073 0a00 0000 000a 0601 0802 0a01  ...s............
-00000570: 1402 7a19 5365 676d 656e 7461 7469 6f6e  ..z.Segmentation
-00000580: 4d6f 6465 6c2e 7072 6564 6963 744e 2906  Model.predictN).
-00000590: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-000005a0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-000005b0: 6d65 5f5f 720d 0000 0072 1300 0000 7218  me__r....r....r.
-000005c0: 0000 0072 0b00 0000 720b 0000 0072 0b00  ...r....r....r..
-000005d0: 0000 720c 0000 0072 0400 0000 0500 0000  ..r....r........
-000005e0: 7306 0000 0008 0208 0608 0c72 0400 0000  s..........r....
-000005f0: 2907 7216 0000 00da 0072 0300 0000 7205  ).r......r....r.
-00000600: 0000 00da 026e 6eda 064d 6f64 756c 6572  .....nn..Moduler
-00000610: 0400 0000 720b 0000 0072 0b00 0000 720b  ....r....r....r.
-00000620: 0000 0072 0c00 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000630: 653e 0100 0000 7304 0000 0008 010c 03    e>....s........
+000001d0: 616e 616e 5c6d 675c 7365 676d 656e 7461  anan\mg\segmenta
+000001e0: 7469 6f6e 5f6d 6f64 656c 735c 6261 7365  tion_models\base
+000001f0: 5c6d 6f64 656c 2e70 79da 0a69 6e69 7469  \model.py..initi
+00000200: 616c 697a 6507 0000 0073 0800 0000 0001  alize....s......
+00000210: 0c01 0c01 0c01 7a1c 5365 676d 656e 7461  ......z.Segmenta
+00000220: 7469 6f6e 4d6f 6465 6c2e 696e 6974 6961  tionModel.initia
+00000230: 6c69 7a65 6302 0000 0000 0000 0000 0000  lizec...........
+00000240: 0007 0000 0003 0000 0043 0000 0073 3a00  .........C...s:.
+00000250: 0000 7c00 a000 7c01 a101 7d02 7c00 6a01  ..|...|...}.|.j.
+00000260: 7c02 8e00 7d03 7c00 a002 7c03 a101 7d04  |...}.|...|...}.
+00000270: 7c00 6a03 7c02 8e00 7d05 7c00 a004 7c05  |.j.|...}.|...|.
+00000280: a101 7d06 7c04 7c06 6602 5300 2901 7a3f  ..}.|.|.f.S.).z?
+00000290: 5365 7175 656e 7469 616c 6c79 2070 6173  Sequentially pas
+000002a0: 7320 6078 6020 7472 6f75 6768 206d 6f64  s `x` trough mod
+000002b0: 656c 6073 2065 6e63 6f64 6572 2c20 6465  el`s encoder, de
+000002c0: 636f 6465 7220 616e 6420 6865 6164 7329  coder and heads)
+000002d0: 05da 0765 6e63 6f64 6572 7206 0000 0072  ...encoderr....r
+000002e0: 0700 0000 7208 0000 0072 0900 0000 2907  ....r....r....).
+000002f0: 720a 0000 00da 0178 da08 6665 6174 7572  r......x..featur
+00000300: 6573 5a13 6d61 736b 5f64 6563 6f64 6572  esZ.mask_decoder
+00000310: 5f6f 7574 7075 74da 056d 6173 6b73 5a16  _output..masksZ.
+00000320: 636f 6e74 6f75 725f 6465 636f 6465 725f  contour_decoder_
+00000330: 6f75 7470 7574 da08 636f 6e74 6f75 7273  output..contours
+00000340: 720b 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
+00000350: 0766 6f72 7761 7264 0d00 0000 730c 0000  .forward....s...
+00000360: 0000 020a 020a 010a 020a 010a 027a 1953  .............z.S
+00000370: 6567 6d65 6e74 6174 696f 6e4d 6f64 656c  egmentationModel
+00000380: 2e66 6f72 7761 7264 6302 0000 0000 0000  .forwardc.......
+00000390: 0000 0000 0002 0000 0009 0000 0043 0000  .............C..
+000003a0: 0073 3000 0000 7c00 6a00 720e 7c00 a001  .s0...|.j.r.|...
+000003b0: a100 0100 7402 a003 a100 8f10 0100 7c00  ....t.........|.
+000003c0: a004 7c01 a101 7d01 5700 3500 5100 5200  ..|...}.W.5.Q.R.
+000003d0: 5800 7c01 5300 2901 612a 0100 0049 6e66  X.|.S.).a*...Inf
+000003e0: 6572 656e 6365 206d 6574 686f 642e 2053  erence method. S
+000003f0: 7769 7463 6820 6d6f 6465 6c20 746f 2060  witch model to `
+00000400: 6576 616c 6020 6d6f 6465 2c20 6361 6c6c  eval` mode, call
+00000410: 2060 2e66 6f72 7761 7264 2878 2960 2077   `.forward(x)` w
+00000420: 6974 6820 6074 6f72 6368 2e6e 6f5f 6772  ith `torch.no_gr
+00000430: 6164 2829 600a 0a20 2020 2020 2020 2041  ad()`..        A
+00000440: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00000450: 2078 3a20 3444 2074 6f72 6368 2074 656e   x: 4D torch ten
+00000460: 736f 7220 7769 7468 2073 6861 7065 2028  sor with shape (
+00000470: 6261 7463 685f 7369 7a65 2c20 6368 616e  batch_size, chan
+00000480: 6e65 6c73 2c20 6865 6967 6874 2c20 7769  nels, height, wi
+00000490: 6474 6829 0a0a 2020 2020 2020 2020 5265  dth)..        Re
+000004a0: 7475 726e 3a0a 2020 2020 2020 2020 2020  turn:.          
+000004b0: 2020 7072 6564 6963 7469 6f6e 3a20 3444    prediction: 4D
+000004c0: 2074 6f72 6368 2074 656e 736f 7220 7769   torch tensor wi
+000004d0: 7468 2073 6861 7065 2028 6261 7463 685f  th shape (batch_
+000004e0: 7369 7a65 2c20 636c 6173 7365 732c 2068  size, classes, h
+000004f0: 6569 6768 742c 2077 6964 7468 290a 0a20  eight, width).. 
+00000500: 2020 2020 2020 2029 05da 0874 7261 696e         )...train
+00000510: 696e 67da 0465 7661 6cda 0574 6f72 6368  ing..eval..torch
+00000520: da07 6e6f 5f67 7261 6472 1300 0000 2902  ..no_gradr....).
+00000530: 720a 0000 0072 0f00 0000 720b 0000 0072  r....r....r....r
+00000540: 0b00 0000 720c 0000 00da 0770 7265 6469  ....r......predi
+00000550: 6374 1900 0000 730a 0000 0000 0a06 0108  ct....s.........
+00000560: 020a 0114 027a 1953 6567 6d65 6e74 6174  .....z.Segmentat
+00000570: 696f 6e4d 6f64 656c 2e70 7265 6469 6374  ionModel.predict
+00000580: 4e29 06da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00000590: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+000005a0: 6c6e 616d 655f 5f72 0d00 0000 7213 0000  lname__r....r...
+000005b0: 0072 1800 0000 720b 0000 0072 0b00 0000  .r....r....r....
+000005c0: 720b 0000 0072 0c00 0000 7204 0000 0005  r....r....r.....
+000005d0: 0000 0073 0600 0000 0802 0806 080c 7204  ...s..........r.
+000005e0: 0000 0029 0772 1600 0000 da00 7203 0000  ...).r......r...
+000005f0: 0072 0500 0000 da02 6e6e da06 4d6f 6475  .r......nn..Modu
+00000600: 6c65 7204 0000 0072 0b00 0000 720b 0000  ler....r....r...
+00000610: 0072 0b00 0000 720c 0000 00da 083c 6d6f  .r....r......<mo
+00000620: 6475 6c65 3e01 0000 0073 0400 0000 0801  dule>....s......
+00000630: 0c03                                     ..
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/model.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/base/__pycache__/model.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/modules.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/base/__pycache__/modules.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/modules.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/base/__pycache__/modules.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/modules.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/base/__pycache__/modules.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/modules.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/base/__pycache__/modules.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:18 2023 UTC, .py size: 3561 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -52,198 +52,197 @@
 00000330: da08 5f5f 696e 6974 5f5f 290a da04 7365  ..__init__)...se
 00000340: 6c66 da0b 696e 5f63 6861 6e6e 656c 73da  lf..in_channels.
 00000350: 0c6f 7574 5f63 6861 6e6e 656c 73da 0b6b  .out_channels..k
 00000360: 6572 6e65 6c5f 7369 7a65 7207 0000 0072  ernel_sizer....r
 00000370: 0600 0000 da0d 7573 655f 6261 7463 686e  ......use_batchn
 00000380: 6f72 6dda 0463 6f6e 76da 0472 656c 75da  orm..conv..relu.
 00000390: 0262 6ea9 01da 095f 5f63 6c61 7373 5f5f  .bn....__class__
-000003a0: a900 fa53 433a 5c55 7365 7273 5c6d 6861  ...SC:\Users\mha
+000003a0: a900 fa46 633a 5c55 7365 7273 5c6d 6861  ...Fc:\Users\mha
 000003b0: 6e61 6e5c 446f 776e 6c6f 6164 735c 4861  nan\Downloads\Ha
-000003c0: 6e61 6e5c 4d61 6d6d 6f50 795c 6d61 6d6d  nan\MammoPy\mamm
-000003d0: 6f70 795c 7365 676d 656e 7461 7469 6f6e  opy\segmentation
-000003e0: 5f6d 6f64 656c 735c 6261 7365 5c6d 6f64  _models\base\mod
-000003f0: 756c 6573 2e70 7972 1300 0000 0b00 0000  ules.pyr........
-00000400: 7328 0000 0000 0a10 0102 0102 ff04 0504  s(..............
-00000410: 0102 0102 0102 0102 0102 0104 fa06 080c  ................
-00000420: 0208 010e 010a 020c 010c 0308 027a 1343  .............z.C
-00000430: 6f6e 7632 6452 654c 552e 5f5f 696e 6974  onv2dReLU.__init
-00000440: 5f5f 2903 7201 0000 0072 0400 0000 5429  __).r....r....T)
-00000450: 05da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00000460: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00000470: 616d 655f 5f72 1300 0000 da0d 5f5f 636c  ame__r......__cl
-00000480: 6173 7363 656c 6c5f 5f72 1e00 0000 721e  asscell__r....r.
-00000490: 0000 0072 1c00 0000 721f 0000 0072 0300  ...r....r....r..
-000004a0: 0000 0a00 0000 7308 0000 0008 0600 0100  ......s.........
-000004b0: 0100 f972 0300 0000 6300 0000 0000 0000  ...r....c.......
-000004c0: 0000 0000 0000 0000 0004 0000 0000 0000  ................
-000004d0: 0073 2600 0000 6500 5a01 6400 5a02 6406  .s&...e.Z.d.Z.d.
-000004e0: 8700 6601 6402 6403 8409 5a03 6404 6405  ..f.d.d...Z.d.d.
-000004f0: 8400 5a04 8700 0400 5a05 5300 2907 da0a  ..Z.....Z.S.)...
-00000500: 5343 5345 4d6f 6475 6c65 e910 0000 0063  SCSEModule.....c
-00000510: 0300 0000 0000 0000 0000 0000 0300 0000  ................
-00000520: 0a00 0000 0300 0000 736c 0000 0074 0083  ........sl...t..
-00000530: 00a0 01a1 0001 0074 02a0 0374 02a0 0464  .......t...t...d
-00000540: 01a1 0174 02a0 057c 017c 017c 021a 0064  ...t...|.|.|...d
-00000550: 01a1 0374 026a 0664 0264 038d 0174 02a0  ...t.j.d.d...t..
-00000560: 057c 017c 021a 007c 0164 01a1 0374 02a0  .|.|...|.d...t..
-00000570: 07a1 00a1 057c 005f 0874 02a0 0374 02a0  .....|._.t...t..
-00000580: 057c 0164 0164 01a1 0374 02a0 07a1 00a1  .|.d.d...t......
-00000590: 027c 005f 0964 0053 0029 044e 7204 0000  .|._.d.S.).Nr...
-000005a0: 0054 7209 0000 0029 0a72 1200 0000 7213  .Tr....).r....r.
-000005b0: 0000 0072 0d00 0000 da0a 5365 7175 656e  ...r......Sequen
-000005c0: 7469 616c da11 4164 6170 7469 7665 4176  tial..AdaptiveAv
-000005d0: 6750 6f6f 6c32 6472 0e00 0000 720f 0000  gPool2dr....r...
-000005e0: 00da 0753 6967 6d6f 6964 da03 6353 45da  ...Sigmoid..cSE.
-000005f0: 0373 5345 2903 7214 0000 0072 1500 0000  .sSE).r....r....
-00000600: da09 7265 6475 6374 696f 6e72 1c00 0000  ..reductionr....
-00000610: 721e 0000 0072 1f00 0000 7213 0000 0033  r....r....r....3
-00000620: 0000 0073 1200 0000 0001 0a01 0401 0801  ...s............
-00000630: 1001 0a01 1001 06fb 0607 7a13 5343 5345  ..........z.SCSE
-00000640: 4d6f 6475 6c65 2e5f 5f69 6e69 745f 5f63  Module.__init__c
-00000650: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000660: 0500 0000 4300 0000 731c 0000 007c 017c  ....C...s....|.|
-00000670: 00a0 007c 01a1 0114 007c 017c 00a0 017c  ...|.....|.|...|
-00000680: 01a1 0114 0017 0053 00a9 014e 2902 7229  .......S...N).r)
-00000690: 0000 0072 2a00 0000 a902 7214 0000 00da  ...r*.....r.....
-000006a0: 0178 721e 0000 0072 1e00 0000 721f 0000  .xr....r....r...
-000006b0: 00da 0766 6f72 7761 7264 3e00 0000 7302  ...forward>...s.
-000006c0: 0000 0000 017a 1253 4353 454d 6f64 756c  .....z.SCSEModul
-000006d0: 652e 666f 7277 6172 6429 0172 2500 0000  e.forward).r%...
-000006e0: a906 7220 0000 0072 2100 0000 7222 0000  ..r ...r!...r"..
-000006f0: 0072 1300 0000 722f 0000 0072 2300 0000  .r....r/...r#...
-00000700: 721e 0000 0072 1e00 0000 721c 0000 0072  r....r....r....r
-00000710: 1f00 0000 7224 0000 0032 0000 0073 0400  ....r$...2...s..
-00000720: 0000 0801 0e0b 7224 0000 0063 0000 0000  ......r$...c....
-00000730: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-00000740: 0000 0000 7326 0000 0065 005a 0164 005a  ....s&...e.Z.d.Z
-00000750: 0264 0687 0066 0164 0264 0384 095a 0364  .d...f.d.d...Z.d
-00000760: 0464 0584 005a 0487 0004 005a 0553 0029  .d...Z.....Z.S.)
-00000770: 07da 0641 7267 4d61 784e 6302 0000 0000  ...ArgMaxNc.....
-00000780: 0000 0000 0000 0002 0000 0002 0000 0003  ................
-00000790: 0000 0073 1400 0000 7400 8300 a001 a100  ...s....t.......
-000007a0: 0100 7c01 7c00 5f02 6400 5300 722c 0000  ..|.|._.d.S.r,..
-000007b0: 0029 0372 1200 0000 7213 0000 00da 0364  .).r....r......d
-000007c0: 696d 2902 7214 0000 0072 3200 0000 721c  im).r....r2...r.
-000007d0: 0000 0072 1e00 0000 721f 0000 0072 1300  ...r....r....r..
-000007e0: 0000 4400 0000 7304 0000 0000 010a 017a  ..D...s........z
-000007f0: 0f41 7267 4d61 782e 5f5f 696e 6974 5f5f  .ArgMax.__init__
-00000800: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000810: 0004 0000 0043 0000 0073 1000 0000 7400  .....C...s....t.
-00000820: 6a01 7c01 7c00 6a02 6401 8d02 5300 2902  j.|.|.j.d...S.).
-00000830: 4e29 0172 3200 0000 2903 da05 746f 7263  N).r2...)...torc
-00000840: 68da 0661 7267 6d61 7872 3200 0000 722d  h..argmaxr2...r-
-00000850: 0000 0072 1e00 0000 721e 0000 0072 1f00  ...r....r....r..
-00000860: 0000 722f 0000 0048 0000 0073 0200 0000  ..r/...H...s....
-00000870: 0001 7a0e 4172 674d 6178 2e66 6f72 7761  ..z.ArgMax.forwa
-00000880: 7264 2901 4e72 3000 0000 721e 0000 0072  rd).Nr0...r....r
-00000890: 1e00 0000 721c 0000 0072 1f00 0000 7231  ....r....r....r1
-000008a0: 0000 0042 0000 0073 0400 0000 0802 0e04  ...B...s........
-000008b0: 7231 0000 0063 0000 0000 0000 0000 0000  r1...c..........
-000008c0: 0000 0000 0000 0300 0000 0000 0000 7324  ..............s$
-000008d0: 0000 0065 005a 0164 005a 0287 0066 0164  ...e.Z.d.Z...f.d
-000008e0: 0164 0284 085a 0364 0364 0484 005a 0487  .d...Z.d.d...Z..
-000008f0: 0004 005a 0553 0029 05da 0a41 6374 6976  ...Z.S.)...Activ
-00000900: 6174 696f 6e63 0200 0000 0000 0000 0000  ationc..........
-00000910: 0000 0300 0000 0400 0000 0b00 0000 73ea  ..............s.
-00000920: 0000 0074 0083 00a0 01a1 0001 007c 0164  ...t.........|.d
-00000930: 006b 0873 1a7c 0164 016b 0272 2a74 026a  .k.s.|.d.k.r*t.j
-00000940: 0366 007c 028e 017c 005f 046e bc7c 0164  .f.|...|._.n.|.d
-00000950: 026b 0272 3e74 02a0 05a1 007c 005f 046e  .k.r>t.....|._.n
-00000960: a87c 0164 036b 0272 5e74 026a 0666 0064  .|.d.k.r^t.j.f.d
-00000970: 0464 0569 017c 0297 028e 017c 005f 046e  .d.i.|.....|._.n
-00000980: 887c 0164 066b 0272 7674 026a 0666 007c  .|.d.k.rvt.j.f.|
-00000990: 028e 017c 005f 046e 707c 0164 076b 0272  ...|._.np|.d.k.r
-000009a0: 8e74 026a 0766 007c 028e 017c 005f 046e  .t.j.f.|...|._.n
-000009b0: 587c 0164 086b 0272 a474 0866 007c 028e  X|.d.k.r.t.f.|..
-000009c0: 017c 005f 046e 427c 0164 096b 0272 c274  .|._.nB|.d.k.r.t
-000009d0: 0866 0064 0464 0569 017c 0297 028e 017c  .f.d.d.i.|.....|
-000009e0: 005f 046e 2474 097c 0183 0172 d87c 0166  ._.n$t.|...r.|.f
-000009f0: 007c 028e 017c 005f 046e 0e74 0a64 0aa0  .|...|._.n.t.d..
-00000a00: 0b7c 01a1 0183 0182 0164 0053 0029 0b4e  .|.......d.S.).N
-00000a10: da08 6964 656e 7469 7479 da07 7369 676d  ..identity..sigm
-00000a20: 6f69 645a 0973 6f66 746d 6178 3264 7232  oidZ.softmax2dr2
-00000a30: 0000 0072 0400 0000 da07 736f 6674 6d61  ...r......softma
-00000a40: 785a 0a6c 6f67 736f 6674 6d61 7872 3400  xZ.logsoftmaxr4.
-00000a50: 0000 5a08 6172 676d 6178 3264 7a45 4163  ..Z.argmax2dzEAc
-00000a60: 7469 7661 7469 6f6e 2073 686f 756c 6420  tivation should 
-00000a70: 6265 2063 616c 6c61 626c 652f 7369 676d  be callable/sigm
-00000a80: 6f69 642f 736f 6674 6d61 782f 6c6f 6773  oid/softmax/logs
-00000a90: 6f66 746d 6178 2f4e 6f6e 653b 2067 6f74  oftmax/None; got
-00000aa0: 207b 7d29 0c72 1200 0000 7213 0000 0072   {}).r....r....r
-00000ab0: 0d00 0000 7210 0000 0072 0b00 0000 7228  ....r....r....r(
-00000ac0: 0000 00da 0753 6f66 746d 6178 da0a 4c6f  .....Softmax..Lo
-00000ad0: 6753 6f66 746d 6178 7231 0000 00da 0863  gSoftmaxr1.....c
-00000ae0: 616c 6c61 626c 65da 0a56 616c 7565 4572  allable..ValueEr
-00000af0: 726f 72da 0666 6f72 6d61 74a9 0372 1400  ror..format..r..
-00000b00: 0000 da04 6e61 6d65 da06 7061 7261 6d73  ....name..params
-00000b10: 721c 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-00000b20: 1300 0000 4e00 0000 7324 0000 0000 020a  ....N...s$......
-00000b30: 0210 0110 0108 010c 0108 0118 0108 0110  ................
-00000b40: 0108 0110 0108 010e 0108 0116 0108 010e  ................
-00000b50: 027a 1341 6374 6976 6174 696f 6e2e 5f5f  .z.Activation.__
-00000b60: 696e 6974 5f5f 6302 0000 0000 0000 0000  init__c.........
-00000b70: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
-00000b80: 0a00 0000 7c00 a000 7c01 a101 5300 722c  ....|...|...S.r,
-00000b90: 0000 0029 0172 0b00 0000 722d 0000 0072  ...).r....r-...r
-00000ba0: 1e00 0000 721e 0000 0072 1f00 0000 722f  ....r....r....r/
-00000bb0: 0000 0065 0000 0073 0200 0000 0001 7a12  ...e...s......z.
-00000bc0: 4163 7469 7661 7469 6f6e 2e66 6f72 7761  Activation.forwa
-00000bd0: 7264 7230 0000 0072 1e00 0000 721e 0000  rdr0...r....r...
-00000be0: 0072 1c00 0000 721f 0000 0072 3500 0000  .r....r....r5...
-00000bf0: 4c00 0000 7304 0000 0008 020c 1772 3500  L...s........r5.
-00000c00: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000c10: 0000 0003 0000 0000 0000 0073 2400 0000  ...........s$...
-00000c20: 6500 5a01 6400 5a02 8700 6601 6401 6402  e.Z.d.Z...f.d.d.
-00000c30: 8408 5a03 6403 6404 8400 5a04 8700 0400  ..Z.d.d...Z.....
-00000c40: 5a05 5300 2905 da09 4174 7465 6e74 696f  Z.S.)...Attentio
-00000c50: 6e63 0200 0000 0000 0000 0000 0000 0300  nc..............
-00000c60: 0000 0400 0000 0b00 0000 734a 0000 0074  ..........sJ...t
-00000c70: 0083 00a0 01a1 0001 007c 0164 006b 0872  .........|.d.k.r
-00000c80: 2274 026a 0366 007c 028e 017c 005f 046e  "t.j.f.|...|._.n
-00000c90: 247c 0164 016b 0272 3874 0566 007c 028e  $|.d.k.r8t.f.|..
-00000ca0: 017c 005f 046e 0e74 0664 02a0 077c 01a1  .|._.n.t.d...|..
-00000cb0: 0183 0182 0164 0053 0029 034e 5a04 7363  .....d.S.).NZ.sc
-00000cc0: 7365 7a1f 4174 7465 6e74 696f 6e20 7b7d  sez.Attention {}
-00000cd0: 2069 7320 6e6f 7420 696d 706c 656d 656e   is not implemen
-00000ce0: 7465 6429 0872 1200 0000 7213 0000 0072  ted).r....r....r
-00000cf0: 0d00 0000 7210 0000 00da 0961 7474 656e  ....r......atten
-00000d00: 7469 6f6e 7224 0000 0072 3c00 0000 723d  tionr$...r<...r=
-00000d10: 0000 0072 3e00 0000 721c 0000 0072 1e00  ...r>...r....r..
-00000d20: 0000 721f 0000 0072 1300 0000 6b00 0000  ..r....r....k...
-00000d30: 730c 0000 0000 010a 0208 0110 0108 010e  s...............
-00000d40: 027a 1241 7474 656e 7469 6f6e 2e5f 5f69  .z.Attention.__i
-00000d50: 6e69 745f 5f63 0200 0000 0000 0000 0000  nit__c..........
-00000d60: 0000 0200 0000 0300 0000 4300 0000 730a  ..........C...s.
-00000d70: 0000 007c 00a0 007c 01a1 0153 0072 2c00  ...|...|...S.r,.
-00000d80: 0000 2901 7242 0000 0072 2d00 0000 721e  ..).rB...r-...r.
-00000d90: 0000 0072 1e00 0000 721f 0000 0072 2f00  ...r....r....r/.
-00000da0: 0000 7500 0000 7302 0000 0000 017a 1141  ..u...s......z.A
-00000db0: 7474 656e 7469 6f6e 2e66 6f72 7761 7264  ttention.forward
-00000dc0: 7230 0000 0072 1e00 0000 721e 0000 0072  r0...r....r....r
-00000dd0: 1c00 0000 721f 0000 0072 4100 0000 6900  ....r....rA...i.
-00000de0: 0000 7304 0000 0008 020c 0a72 4100 0000  ..s........rA...
-00000df0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000e00: 0002 0000 0040 0000 0073 1400 0000 6500  .....@...s....e.
-00000e10: 5a01 6400 5a02 6401 6402 8400 5a03 6403  Z.d.Z.d.d...Z.d.
-00000e20: 5300 2904 da07 466c 6174 7465 6e63 0200  S.)...Flattenc..
-00000e30: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00000e40: 0000 4300 0000 7312 0000 007c 01a0 007c  ..C...s....|...|
-00000e50: 016a 0164 0119 0064 02a1 0253 0029 034e  .j.d...d...S.).N
-00000e60: 7201 0000 00e9 ffff ffff 2902 da04 7669  r.........)...vi
-00000e70: 6577 da05 7368 6170 6572 2d00 0000 721e  ew..shaper-...r.
-00000e80: 0000 0072 1e00 0000 721f 0000 0072 2f00  ...r....r....r/.
-00000e90: 0000 7a00 0000 7302 0000 0000 017a 0f46  ..z...s......z.F
-00000ea0: 6c61 7474 656e 2e66 6f72 7761 7264 4e29  latten.forwardN)
-00000eb0: 0472 2000 0000 7221 0000 0072 2200 0000  .r ...r!...r"...
-00000ec0: 722f 0000 0072 1e00 0000 721e 0000 0072  r/...r....r....r
-00000ed0: 1e00 0000 721f 0000 0072 4300 0000 7900  ....r....rC...y.
-00000ee0: 0000 7302 0000 0008 0172 4300 0000 290e  ..s......rC...).
-00000ef0: 7233 0000 00da 0874 6f72 6368 2e6e 6e72  r3.....torch.nnr
-00000f00: 0d00 0000 5a0b 696e 706c 6163 655f 6162  ....Z.inplace_ab
-00000f10: 6e72 0200 0000 da0b 496d 706f 7274 4572  nr......ImportEr
-00000f20: 726f 7272 2600 0000 7203 0000 00da 064d  rorr&...r......M
-00000f30: 6f64 756c 6572 2400 0000 7231 0000 0072  oduler$...r1...r
-00000f40: 3500 0000 7241 0000 0072 4300 0000 721e  5...rA...rC...r.
-00000f50: 0000 0072 1e00 0000 721e 0000 0072 1f00  ...r....r....r..
-00000f60: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000f70: 7316 0000 0008 010c 0202 0110 010e 010a  s...............
-00000f80: 0312 2812 1012 0a12 1d12 10              ..(........
+000003c0: 6e61 6e5c 6d67 5c73 6567 6d65 6e74 6174  nan\mg\segmentat
+000003d0: 696f 6e5f 6d6f 6465 6c73 5c62 6173 655c  ion_models\base\
+000003e0: 6d6f 6475 6c65 732e 7079 7213 0000 000b  modules.pyr.....
+000003f0: 0000 0073 2800 0000 000a 1001 0201 02ff  ...s(...........
+00000400: 0405 0401 0201 0201 0201 0201 0201 04fa  ................
+00000410: 0608 0c02 0801 0e01 0a02 0c01 0c03 0802  ................
+00000420: 7a13 436f 6e76 3264 5265 4c55 2e5f 5f69  z.Conv2dReLU.__i
+00000430: 6e69 745f 5f29 0372 0100 0000 7204 0000  nit__).r....r...
+00000440: 0054 2905 da08 5f5f 6e61 6d65 5f5f da0a  .T)...__name__..
+00000450: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000460: 616c 6e61 6d65 5f5f 7213 0000 00da 0d5f  alname__r......_
+00000470: 5f63 6c61 7373 6365 6c6c 5f5f 721e 0000  _classcell__r...
+00000480: 0072 1e00 0000 721c 0000 0072 1f00 0000  .r....r....r....
+00000490: 7203 0000 000a 0000 0073 0800 0000 0806  r........s......
+000004a0: 0001 0001 00f9 7203 0000 0063 0000 0000  ......r....c....
+000004b0: 0000 0000 0000 0000 0000 0000 0400 0000  ................
+000004c0: 0000 0000 7326 0000 0065 005a 0164 005a  ....s&...e.Z.d.Z
+000004d0: 0264 0687 0066 0164 0264 0384 095a 0364  .d...f.d.d...Z.d
+000004e0: 0464 0584 005a 0487 0004 005a 0553 0029  .d...Z.....Z.S.)
+000004f0: 07da 0a53 4353 454d 6f64 756c 65e9 1000  ...SCSEModule...
+00000500: 0000 6303 0000 0000 0000 0000 0000 0003  ..c.............
+00000510: 0000 000a 0000 0003 0000 0073 6c00 0000  ...........sl...
+00000520: 7400 8300 a001 a100 0100 7402 a003 7402  t.........t...t.
+00000530: a004 6401 a101 7402 a005 7c01 7c01 7c02  ..d...t...|.|.|.
+00000540: 1a00 6401 a103 7402 6a06 6402 6403 8d01  ..d...t.j.d.d...
+00000550: 7402 a005 7c01 7c02 1a00 7c01 6401 a103  t...|.|...|.d...
+00000560: 7402 a007 a100 a105 7c00 5f08 7402 a003  t.......|._.t...
+00000570: 7402 a005 7c01 6401 6401 a103 7402 a007  t...|.d.d...t...
+00000580: a100 a102 7c00 5f09 6400 5300 2904 4e72  ....|._.d.S.).Nr
+00000590: 0400 0000 5472 0900 0000 290a 7212 0000  ....Tr....).r...
+000005a0: 0072 1300 0000 720d 0000 00da 0a53 6571  .r....r......Seq
+000005b0: 7565 6e74 6961 6cda 1141 6461 7074 6976  uential..Adaptiv
+000005c0: 6541 7667 506f 6f6c 3264 720e 0000 0072  eAvgPool2dr....r
+000005d0: 0f00 0000 da07 5369 676d 6f69 64da 0363  ......Sigmoid..c
+000005e0: 5345 da03 7353 4529 0372 1400 0000 7215  SE..sSE).r....r.
+000005f0: 0000 00da 0972 6564 7563 7469 6f6e 721c  .....reductionr.
+00000600: 0000 0072 1e00 0000 721f 0000 0072 1300  ...r....r....r..
+00000610: 0000 3300 0000 7312 0000 0000 010a 0104  ..3...s.........
+00000620: 0108 0110 010a 0110 0106 fb06 077a 1353  .............z.S
+00000630: 4353 454d 6f64 756c 652e 5f5f 696e 6974  CSEModule.__init
+00000640: 5f5f 6302 0000 0000 0000 0000 0000 0002  __c.............
+00000650: 0000 0005 0000 0043 0000 0073 1c00 0000  .......C...s....
+00000660: 7c01 7c00 a000 7c01 a101 1400 7c01 7c00  |.|...|.....|.|.
+00000670: a001 7c01 a101 1400 1700 5300 a901 4e29  ..|.......S...N)
+00000680: 0272 2900 0000 722a 0000 00a9 0272 1400  .r)...r*.....r..
+00000690: 0000 da01 7872 1e00 0000 721e 0000 0072  ....xr....r....r
+000006a0: 1f00 0000 da07 666f 7277 6172 643e 0000  ......forward>..
+000006b0: 0073 0200 0000 0001 7a12 5343 5345 4d6f  .s......z.SCSEMo
+000006c0: 6475 6c65 2e66 6f72 7761 7264 2901 7225  dule.forward).r%
+000006d0: 0000 00a9 0672 2000 0000 7221 0000 0072  .....r ...r!...r
+000006e0: 2200 0000 7213 0000 0072 2f00 0000 7223  "...r....r/...r#
+000006f0: 0000 0072 1e00 0000 721e 0000 0072 1c00  ...r....r....r..
+00000700: 0000 721f 0000 0072 2400 0000 3200 0000  ..r....r$...2...
+00000710: 7304 0000 0008 010e 0b72 2400 0000 6300  s........r$...c.
+00000720: 0000 0000 0000 0000 0000 0000 0000 0004  ................
+00000730: 0000 0000 0000 0073 2600 0000 6500 5a01  .......s&...e.Z.
+00000740: 6400 5a02 6406 8700 6601 6402 6403 8409  d.Z.d...f.d.d...
+00000750: 5a03 6404 6405 8400 5a04 8700 0400 5a05  Z.d.d...Z.....Z.
+00000760: 5300 2907 da06 4172 674d 6178 4e63 0200  S.)...ArgMaxNc..
+00000770: 0000 0000 0000 0000 0000 0200 0000 0200  ................
+00000780: 0000 0300 0000 7314 0000 0074 0083 00a0  ......s....t....
+00000790: 01a1 0001 007c 017c 005f 0264 0053 0072  .....|.|._.d.S.r
+000007a0: 2c00 0000 2903 7212 0000 0072 1300 0000  ,...).r....r....
+000007b0: da03 6469 6d29 0272 1400 0000 7232 0000  ..dim).r....r2..
+000007c0: 0072 1c00 0000 721e 0000 0072 1f00 0000  .r....r....r....
+000007d0: 7213 0000 0044 0000 0073 0400 0000 0001  r....D...s......
+000007e0: 0a01 7a0f 4172 674d 6178 2e5f 5f69 6e69  ..z.ArgMax.__ini
+000007f0: 745f 5f63 0200 0000 0000 0000 0000 0000  t__c............
+00000800: 0200 0000 0400 0000 4300 0000 7310 0000  ........C...s...
+00000810: 0074 006a 017c 017c 006a 0264 018d 0253  .t.j.|.|.j.d...S
+00000820: 0029 024e 2901 7232 0000 0029 03da 0574  .).N).r2...)...t
+00000830: 6f72 6368 da06 6172 676d 6178 7232 0000  orch..argmaxr2..
+00000840: 0072 2d00 0000 721e 0000 0072 1e00 0000  .r-...r....r....
+00000850: 721f 0000 0072 2f00 0000 4800 0000 7302  r....r/...H...s.
+00000860: 0000 0000 017a 0e41 7267 4d61 782e 666f  .....z.ArgMax.fo
+00000870: 7277 6172 6429 014e 7230 0000 0072 1e00  rward).Nr0...r..
+00000880: 0000 721e 0000 0072 1c00 0000 721f 0000  ..r....r....r...
+00000890: 0072 3100 0000 4200 0000 7304 0000 0008  .r1...B...s.....
+000008a0: 020e 0472 3100 0000 6300 0000 0000 0000  ...r1...c.......
+000008b0: 0000 0000 0000 0000 0003 0000 0000 0000  ................
+000008c0: 0073 2400 0000 6500 5a01 6400 5a02 8700  .s$...e.Z.d.Z...
+000008d0: 6601 6401 6402 8408 5a03 6403 6404 8400  f.d.d...Z.d.d...
+000008e0: 5a04 8700 0400 5a05 5300 2905 da0a 4163  Z.....Z.S.)...Ac
+000008f0: 7469 7661 7469 6f6e 6302 0000 0000 0000  tivationc.......
+00000900: 0000 0000 0003 0000 0004 0000 000b 0000  ................
+00000910: 0073 ea00 0000 7400 8300 a001 a100 0100  .s....t.........
+00000920: 7c01 6400 6b08 731a 7c01 6401 6b02 722a  |.d.k.s.|.d.k.r*
+00000930: 7402 6a03 6600 7c02 8e01 7c00 5f04 6ebc  t.j.f.|...|._.n.
+00000940: 7c01 6402 6b02 723e 7402 a005 a100 7c00  |.d.k.r>t.....|.
+00000950: 5f04 6ea8 7c01 6403 6b02 725e 7402 6a06  _.n.|.d.k.r^t.j.
+00000960: 6600 6404 6405 6901 7c02 9702 8e01 7c00  f.d.d.i.|.....|.
+00000970: 5f04 6e88 7c01 6406 6b02 7276 7402 6a06  _.n.|.d.k.rvt.j.
+00000980: 6600 7c02 8e01 7c00 5f04 6e70 7c01 6407  f.|...|._.np|.d.
+00000990: 6b02 728e 7402 6a07 6600 7c02 8e01 7c00  k.r.t.j.f.|...|.
+000009a0: 5f04 6e58 7c01 6408 6b02 72a4 7408 6600  _.nX|.d.k.r.t.f.
+000009b0: 7c02 8e01 7c00 5f04 6e42 7c01 6409 6b02  |...|._.nB|.d.k.
+000009c0: 72c2 7408 6600 6404 6405 6901 7c02 9702  r.t.f.d.d.i.|...
+000009d0: 8e01 7c00 5f04 6e24 7409 7c01 8301 72d8  ..|._.n$t.|...r.
+000009e0: 7c01 6600 7c02 8e01 7c00 5f04 6e0e 740a  |.f.|...|._.n.t.
+000009f0: 640a a00b 7c01 a101 8301 8201 6400 5300  d...|.......d.S.
+00000a00: 290b 4eda 0869 6465 6e74 6974 79da 0773  ).N..identity..s
+00000a10: 6967 6d6f 6964 5a09 736f 6674 6d61 7832  igmoidZ.softmax2
+00000a20: 6472 3200 0000 7204 0000 00da 0773 6f66  dr2...r......sof
+00000a30: 746d 6178 5a0a 6c6f 6773 6f66 746d 6178  tmaxZ.logsoftmax
+00000a40: 7234 0000 005a 0861 7267 6d61 7832 647a  r4...Z.argmax2dz
+00000a50: 4541 6374 6976 6174 696f 6e20 7368 6f75  EActivation shou
+00000a60: 6c64 2062 6520 6361 6c6c 6162 6c65 2f73  ld be callable/s
+00000a70: 6967 6d6f 6964 2f73 6f66 746d 6178 2f6c  igmoid/softmax/l
+00000a80: 6f67 736f 6674 6d61 782f 4e6f 6e65 3b20  ogsoftmax/None; 
+00000a90: 676f 7420 7b7d 290c 7212 0000 0072 1300  got {}).r....r..
+00000aa0: 0000 720d 0000 0072 1000 0000 720b 0000  ..r....r....r...
+00000ab0: 0072 2800 0000 da07 536f 6674 6d61 78da  .r(.....Softmax.
+00000ac0: 0a4c 6f67 536f 6674 6d61 7872 3100 0000  .LogSoftmaxr1...
+00000ad0: da08 6361 6c6c 6162 6c65 da0a 5661 6c75  ..callable..Valu
+00000ae0: 6545 7272 6f72 da06 666f 726d 6174 a903  eError..format..
+00000af0: 7214 0000 00da 046e 616d 65da 0670 6172  r......name..par
+00000b00: 616d 7372 1c00 0000 721e 0000 0072 1f00  amsr....r....r..
+00000b10: 0000 7213 0000 004e 0000 0073 2400 0000  ..r....N...s$...
+00000b20: 0002 0a02 1001 1001 0801 0c01 0801 1801  ................
+00000b30: 0801 1001 0801 1001 0801 0e01 0801 1601  ................
+00000b40: 0801 0e02 7a13 4163 7469 7661 7469 6f6e  ....z.Activation
+00000b50: 2e5f 5f69 6e69 745f 5f63 0200 0000 0000  .__init__c......
+00000b60: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+00000b70: 0000 730a 0000 007c 00a0 007c 01a1 0153  ..s....|...|...S
+00000b80: 0072 2c00 0000 2901 720b 0000 0072 2d00  .r,...).r....r-.
+00000b90: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
+00000ba0: 0072 2f00 0000 6500 0000 7302 0000 0000  .r/...e...s.....
+00000bb0: 017a 1241 6374 6976 6174 696f 6e2e 666f  .z.Activation.fo
+00000bc0: 7277 6172 6472 3000 0000 721e 0000 0072  rwardr0...r....r
+00000bd0: 1e00 0000 721c 0000 0072 1f00 0000 7235  ....r....r....r5
+00000be0: 0000 004c 0000 0073 0400 0000 0802 0c17  ...L...s........
+00000bf0: 7235 0000 0063 0000 0000 0000 0000 0000  r5...c..........
+00000c00: 0000 0000 0000 0300 0000 0000 0000 7324  ..............s$
+00000c10: 0000 0065 005a 0164 005a 0287 0066 0164  ...e.Z.d.Z...f.d
+00000c20: 0164 0284 085a 0364 0364 0484 005a 0487  .d...Z.d.d...Z..
+00000c30: 0004 005a 0553 0029 05da 0941 7474 656e  ...Z.S.)...Atten
+00000c40: 7469 6f6e 6302 0000 0000 0000 0000 0000  tionc...........
+00000c50: 0003 0000 0004 0000 000b 0000 0073 4a00  .............sJ.
+00000c60: 0000 7400 8300 a001 a100 0100 7c01 6400  ..t.........|.d.
+00000c70: 6b08 7222 7402 6a03 6600 7c02 8e01 7c00  k.r"t.j.f.|...|.
+00000c80: 5f04 6e24 7c01 6401 6b02 7238 7405 6600  _.n$|.d.k.r8t.f.
+00000c90: 7c02 8e01 7c00 5f04 6e0e 7406 6402 a007  |...|._.n.t.d...
+00000ca0: 7c01 a101 8301 8201 6400 5300 2903 4e5a  |.......d.S.).NZ
+00000cb0: 0473 6373 657a 1f41 7474 656e 7469 6f6e  .scsez.Attention
+00000cc0: 207b 7d20 6973 206e 6f74 2069 6d70 6c65   {} is not imple
+00000cd0: 6d65 6e74 6564 2908 7212 0000 0072 1300  mented).r....r..
+00000ce0: 0000 720d 0000 0072 1000 0000 da09 6174  ..r....r......at
+00000cf0: 7465 6e74 696f 6e72 2400 0000 723c 0000  tentionr$...r<..
+00000d00: 0072 3d00 0000 723e 0000 0072 1c00 0000  .r=...r>...r....
+00000d10: 721e 0000 0072 1f00 0000 7213 0000 006b  r....r....r....k
+00000d20: 0000 0073 0c00 0000 0001 0a02 0801 1001  ...s............
+00000d30: 0801 0e02 7a12 4174 7465 6e74 696f 6e2e  ....z.Attention.
+00000d40: 5f5f 696e 6974 5f5f 6302 0000 0000 0000  __init__c.......
+00000d50: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+00000d60: 0073 0a00 0000 7c00 a000 7c01 a101 5300  .s....|...|...S.
+00000d70: 722c 0000 0029 0172 4200 0000 722d 0000  r,...).rB...r-..
+00000d80: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
+00000d90: 722f 0000 0075 0000 0073 0200 0000 0001  r/...u...s......
+00000da0: 7a11 4174 7465 6e74 696f 6e2e 666f 7277  z.Attention.forw
+00000db0: 6172 6472 3000 0000 721e 0000 0072 1e00  ardr0...r....r..
+00000dc0: 0000 721c 0000 0072 1f00 0000 7241 0000  ..r....r....rA..
+00000dd0: 0069 0000 0073 0400 0000 0802 0c0a 7241  .i...s........rA
+00000de0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000df0: 0000 0000 0200 0000 4000 0000 7314 0000  ........@...s...
+00000e00: 0065 005a 0164 005a 0264 0164 0284 005a  .e.Z.d.Z.d.d...Z
+00000e10: 0364 0353 0029 04da 0746 6c61 7474 656e  .d.S.)...Flatten
+00000e20: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00000e30: 0004 0000 0043 0000 0073 1200 0000 7c01  .....C...s....|.
+00000e40: a000 7c01 6a01 6401 1900 6402 a102 5300  ..|.j.d...d...S.
+00000e50: 2903 4e72 0100 0000 e9ff ffff ff29 02da  ).Nr.........)..
+00000e60: 0476 6965 77da 0573 6861 7065 722d 0000  .view..shaper-..
+00000e70: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
+00000e80: 722f 0000 007a 0000 0073 0200 0000 0001  r/...z...s......
+00000e90: 7a0f 466c 6174 7465 6e2e 666f 7277 6172  z.Flatten.forwar
+00000ea0: 644e 2904 7220 0000 0072 2100 0000 7222  dN).r ...r!...r"
+00000eb0: 0000 0072 2f00 0000 721e 0000 0072 1e00  ...r/...r....r..
+00000ec0: 0000 721e 0000 0072 1f00 0000 7243 0000  ..r....r....rC..
+00000ed0: 0079 0000 0073 0200 0000 0801 7243 0000  .y...s......rC..
+00000ee0: 0029 0e72 3300 0000 da08 746f 7263 682e  .).r3.....torch.
+00000ef0: 6e6e 720d 0000 005a 0b69 6e70 6c61 6365  nnr....Z.inplace
+00000f00: 5f61 626e 7202 0000 00da 0b49 6d70 6f72  _abnr......Impor
+00000f10: 7445 7272 6f72 7226 0000 0072 0300 0000  tErrorr&...r....
+00000f20: da06 4d6f 6475 6c65 7224 0000 0072 3100  ..Moduler$...r1.
+00000f30: 0000 7235 0000 0072 4100 0000 7243 0000  ..r5...rA...rC..
+00000f40: 0072 1e00 0000 721e 0000 0072 1e00 0000  .r....r....r....
+00000f50: 721f 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000f60: 0000 0073 1600 0000 0801 0c02 0201 1001  ...s............
+00000f70: 0e01 0a03 1228 1210 120a 121d 1210       .....(........
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/base/__pycache__/modules.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/base/__pycache__/modules.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/base/heads.py` & `mammopy-0.0.9/segmentation_models/base/heads.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/base/initialization.py` & `mammopy-0.0.9/segmentation_models/base/initialization.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/base/model.py` & `mammopy-0.0.9/segmentation_models/base/model.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/base/modules.py` & `mammopy-0.0.9/segmentation_models/base/modules.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__init__.py` & `mammopy-0.0.9/segmentation_models/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/__init__.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/__init__.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/__init__.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/__init__.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/__init__.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:20 2023 UTC, .py size: 2341 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 5477 1164 2509 0000  U.......Tw.d%...
+00000000: 610d 0d0a 0000 0000 5477 1164 2509 0000  a.......Tw.d%...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4601 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 6d02 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d03 5a03 0100 6402 6403 6c04 6d05  ..m.Z...d.d.l.m.
 00000050: 5a05 0100 6402 6404 6c06 6d07 5a07 0100  Z...d.d.l.m.Z...
 00000060: 6402 6405 6c08 6d09 5a09 0100 6402 6406  d.d.l.m.Z...d.d.
 00000070: 6c0a 6d0b 5a0b 0100 6402 6407 6c0c 6d0d  l.m.Z...d.d.l.m.
@@ -36,104 +36,104 @@
 00000230: 6f62 696c 656e 6574 5f65 6e63 6f64 6572  obilenet_encoder
 00000240: 7329 01da 1178 6365 7074 696f 6e5f 656e  s)...xception_en
 00000250: 636f 6465 7273 2901 da1a 7469 6d6d 5f65  coders)...timm_e
 00000260: 6666 6963 6965 6e74 6e65 745f 656e 636f  fficientnet_enco
 00000270: 6465 7273 2901 da10 7072 6570 726f 6365  ders)...preproce
 00000280: 7373 5f69 6e70 7574 e903 0000 00e9 0500  ss_input........
 00000290: 0000 6304 0000 0000 0000 0000 0000 0008  ..c.............
-000002a0: 0000 0006 0000 0043 0000 0073 6800 0000  .......C...sh...
+000002a0: 0000 0006 0000 0043 0000 0073 6c00 0000  .......C...sl...
 000002b0: 7400 7c00 1900 6401 1900 7d04 7400 7c00  t.|...d...}.t.|.
 000002c0: 1900 6402 1900 7d05 7c05 6a01 7c02 6403  ..d...}.|.j.|.d.
-000002d0: 8d01 0100 7c04 6600 7c05 8e01 7d06 7c03  ....|.f.|...}.|.
-000002e0: 6400 6b09 725a 7400 7c00 1900 6404 1900  d.k.rZt.|...d...
-000002f0: 7c03 1900 7d07 7c06 a002 7403 a004 7c07  |...}.|...t...|.
-00000300: 6405 1900 a101 a101 0100 7c06 a005 7c01  d.........|...|.
-00000310: a101 0100 7c06 5300 2906 4eda 0765 6e63  ....|.S.).N..enc
-00000320: 6f64 6572 da06 7061 7261 6d73 2901 da05  oder..params)...
-00000330: 6465 7074 68da 1370 7265 7472 6169 6e65  depth..pretraine
-00000340: 645f 7365 7474 696e 6773 da03 7572 6c29  d_settings..url)
-00000350: 06da 0865 6e63 6f64 6572 73da 0675 7064  ...encoders..upd
-00000360: 6174 65da 0f6c 6f61 645f 7374 6174 655f  ate..load_state_
-00000370: 6469 6374 da09 6d6f 6465 6c5f 7a6f 6fda  dict..model_zoo.
-00000380: 086c 6f61 645f 7572 6c5a 0f73 6574 5f69  .load_urlZ.set_i
-00000390: 6e5f 6368 616e 6e65 6c73 2908 da04 6e61  n_channels)...na
-000003a0: 6d65 da0b 696e 5f63 6861 6e6e 656c 7372  me..in_channelsr
-000003b0: 1300 0000 da07 7765 6967 6874 73da 0745  ......weights..E
-000003c0: 6e63 6f64 6572 7212 0000 0072 1100 0000  ncoderr....r....
-000003d0: da08 7365 7474 696e 6773 a900 7220 0000  ..settings..r ..
-000003e0: 00fa 5843 3a5c 5573 6572 735c 6d68 616e  ..XC:\Users\mhan
-000003f0: 616e 5c44 6f77 6e6c 6f61 6473 5c48 616e  an\Downloads\Han
-00000400: 616e 5c4d 616d 6d6f 5079 5c6d 616d 6d6f  an\MammoPy\mammo
-00000410: 7079 5c73 6567 6d65 6e74 6174 696f 6e5f  py\segmentation_
-00000420: 6d6f 6465 6c73 5c65 6e63 6f64 6572 735c  models\encoders\
-00000430: 5f5f 696e 6974 5f5f 2e70 79da 0b67 6574  __init__.py..get
-00000440: 5f65 6e63 6f64 6572 2000 0000 7312 0000  _encoder ...s...
-00000450: 0000 010c 010c 010c 010a 0208 0110 0114  ................
-00000460: 020a 0272 2200 0000 6300 0000 0000 0000  ...r"...c.......
-00000470: 0000 0000 0000 0000 0003 0000 0043 0000  .............C..
-00000480: 0073 0c00 0000 7400 7401 a002 a100 8301  .s....t.t.......
-00000490: 5300 2901 4e29 03da 046c 6973 7472 1600  S.).N)...listr..
-000004a0: 0000 da04 6b65 7973 7220 0000 0072 2000  ....keysr ...r .
-000004b0: 0000 7220 0000 0072 2100 0000 da11 6765  ..r ...r!.....ge
-000004c0: 745f 656e 636f 6465 725f 6e61 6d65 732f  t_encoder_names/
-000004d0: 0000 0073 0200 0000 0001 7225 0000 00da  ...s......r%....
-000004e0: 0869 6d61 6765 6e65 7463 0200 0000 0000  .imagenetc......
-000004f0: 0000 0000 0000 0400 0000 0500 0000 4300  ..............C.
-00000500: 0000 737a 0000 0074 007c 0019 0064 0119  ..sz...t.|...d..
-00000510: 007d 027c 017c 02a0 01a1 006b 0772 2a74  .}.|.|.....k.r*t
-00000520: 0264 02a0 037c 02a0 01a1 00a1 0183 0182  .d...|..........
-00000530: 0169 007d 037c 027c 0119 00a0 0464 03a1  .i.}.|.|.....d..
-00000540: 017c 0364 033c 007c 027c 0119 00a0 0464  .|.d.<.|.|.....d
-00000550: 04a1 017c 0364 043c 007c 027c 0119 00a0  ...|.d.<.|.|....
-00000560: 0464 05a1 017c 0364 053c 007c 027c 0119  .d...|.d.<.|.|..
-00000570: 00a0 0464 06a1 017c 0364 063c 007c 0353  ...d...|.d.<.|.S
-00000580: 0029 074e 7214 0000 007a 1f41 7661 6c69  .).Nr....z.Avali
-00000590: 6162 6c65 2070 7265 7472 6169 6e65 6420  able pretrained 
-000005a0: 6f70 7469 6f6e 7320 7b7d 5a0b 696e 7075  options {}Z.inpu
-000005b0: 745f 7370 6163 655a 0b69 6e70 7574 5f72  t_spaceZ.input_r
-000005c0: 616e 6765 da04 6d65 616e da03 7374 6429  ange..mean..std)
-000005d0: 0572 1600 0000 7224 0000 00da 0a56 616c  .r....r$.....Val
-000005e0: 7565 4572 726f 72da 0666 6f72 6d61 74da  ueError..format.
-000005f0: 0367 6574 2904 da0c 656e 636f 6465 725f  .get)...encoder_
-00000600: 6e61 6d65 da0a 7072 6574 7261 696e 6564  name..pretrained
-00000610: 721f 0000 005a 1266 6f72 6d61 7474 6564  r....Z.formatted
-00000620: 5f73 6574 7469 6e67 7372 2000 0000 7220  _settingsr ...r 
-00000630: 0000 0072 2100 0000 da18 6765 745f 7072  ...r!.....get_pr
-00000640: 6570 726f 6365 7373 696e 675f 7061 7261  eprocessing_para
-00000650: 6d73 3300 0000 7312 0000 0000 010c 020c  ms3...s.........
-00000660: 0112 0204 0112 0112 0112 0112 0172 2e00  .............r..
-00000670: 0000 6302 0000 0000 0000 0000 0000 0003  ..c.............
-00000680: 0000 0004 0000 0043 0000 0073 1a00 0000  .......C...s....
-00000690: 7400 7c00 7c01 6401 8d02 7d02 7401 6a02  t.|.|.d...}.t.j.
-000006a0: 7403 6601 7c02 8e01 5300 2902 4e29 0172  t.f.|...S.).N).r
-000006b0: 2d00 0000 2904 722e 0000 00da 0966 756e  -...).r......fun
-000006c0: 6374 6f6f 6c73 da07 7061 7274 6961 6c72  ctools..partialr
-000006d0: 0e00 0000 2903 722c 0000 0072 2d00 0000  ....).r,...r-...
-000006e0: 7212 0000 0072 2000 0000 7220 0000 0072  r....r ...r ...r
-000006f0: 2100 0000 da14 6765 745f 7072 6570 726f  !.....get_prepro
-00000700: 6365 7373 696e 675f 666e 4100 0000 7304  cessing_fnA...s.
-00000710: 0000 0000 010c 0172 3100 0000 2903 720f  .......r1...).r.
-00000720: 0000 0072 1000 0000 4e29 0172 2600 0000  ...r....N).r&...
-00000730: 2901 7226 0000 0029 2272 2f00 0000 da15  ).r&...)"r/.....
-00000740: 746f 7263 682e 7574 696c 732e 6d6f 6465  torch.utils.mode
-00000750: 6c5f 7a6f 6fda 0575 7469 6c73 7219 0000  l_zoo..utilsr...
-00000760: 00da 0672 6573 6e65 7472 0300 0000 5a03  ...resnetr....Z.
-00000770: 6470 6e72 0400 0000 da03 7667 6772 0500  dpnr......vggr..
-00000780: 0000 5a05 7365 6e65 7472 0600 0000 da08  ..Z.senetr......
-00000790: 6465 6e73 656e 6574 7207 0000 005a 1169  densenetr....Z.i
-000007a0: 6e63 6570 7469 6f6e 7265 736e 6574 7632  nceptionresnetv2
-000007b0: 7208 0000 005a 0b69 6e63 6570 7469 6f6e  r....Z.inception
-000007c0: 7634 7209 0000 00da 0c65 6666 6963 6965  v4r......efficie
-000007d0: 6e74 6e65 7472 0a00 0000 da09 6d6f 6269  ntnetr......mobi
-000007e0: 6c65 6e65 7472 0b00 0000 5a08 7863 6570  lenetr....Z.xcep
-000007f0: 7469 6f6e 720c 0000 005a 1174 696d 6d5f  tionr....Z.timm_
-00000800: 6566 6669 6369 656e 746e 6574 720d 0000  efficientnetr...
-00000810: 005a 0e5f 7072 6570 726f 6365 7373 696e  .Z._preprocessin
-00000820: 6772 0e00 0000 7216 0000 0072 1700 0000  gr....r....r....
-00000830: 7222 0000 0072 2500 0000 722e 0000 0072  r"...r%...r....r
-00000840: 3100 0000 7220 0000 0072 2000 0000 7220  1...r ...r ...r 
-00000850: 0000 0072 2100 0000 da08 3c6d 6f64 756c  ...r!.....<modul
-00000860: 653e 0100 0000 733a 0000 0008 0112 020c  e>....s:........
-00000870: 010c 010c 010c 010c 010c 010c 010c 010c  ................
-00000880: 010c 010c 020c 0204 010a 010a 010a 010a  ................
-00000890: 010a 010a 010a 010a 010a 010a 010a 030a  ................
-000008a0: 0f08 040a 0e                             .....
+000002d0: 8d01 0100 7c04 6600 6900 7c05 a401 8e01  ....|.f.i.|.....
+000002e0: 7d06 7c03 6400 7501 725e 7400 7c00 1900  }.|.d.u.r^t.|...
+000002f0: 6404 1900 7c03 1900 7d07 7c06 a002 7403  d...|...}.|...t.
+00000300: a004 7c07 6405 1900 a101 a101 0100 7c06  ..|.d.........|.
+00000310: a005 7c01 a101 0100 7c06 5300 2906 4eda  ..|.....|.S.).N.
+00000320: 0765 6e63 6f64 6572 da06 7061 7261 6d73  .encoder..params
+00000330: 2901 da05 6465 7074 68da 1370 7265 7472  )...depth..pretr
+00000340: 6169 6e65 645f 7365 7474 696e 6773 da03  ained_settings..
+00000350: 7572 6c29 06da 0865 6e63 6f64 6572 73da  url)...encoders.
+00000360: 0675 7064 6174 65da 0f6c 6f61 645f 7374  .update..load_st
+00000370: 6174 655f 6469 6374 da09 6d6f 6465 6c5f  ate_dict..model_
+00000380: 7a6f 6fda 086c 6f61 645f 7572 6c5a 0f73  zoo..load_urlZ.s
+00000390: 6574 5f69 6e5f 6368 616e 6e65 6c73 2908  et_in_channels).
+000003a0: da04 6e61 6d65 da0b 696e 5f63 6861 6e6e  ..name..in_chann
+000003b0: 656c 7372 1300 0000 da07 7765 6967 6874  elsr......weight
+000003c0: 73da 0745 6e63 6f64 6572 7212 0000 0072  s..Encoderr....r
+000003d0: 1100 0000 da08 7365 7474 696e 6773 a900  ......settings..
+000003e0: 7220 0000 00fa 5643 3a5c 5573 6572 735c  r ....VC:\Users\
+000003f0: 6d68 616e 616e 5c44 6573 6b74 6f70 5c44  mhanan\Desktop\D
+00000400: 656e 7369 7479 4170 705c 4465 6e73 6974  ensityApp\Densit
+00000410: 7941 7070 5c73 6567 6d65 6e74 6174 696f  yApp\segmentatio
+00000420: 6e5f 6d6f 6465 6c73 5c65 6e63 6f64 6572  n_models\encoder
+00000430: 735c 5f5f 696e 6974 5f5f 2e70 79da 0b67  s\__init__.py..g
+00000440: 6574 5f65 6e63 6f64 6572 2000 0000 7312  et_encoder ...s.
+00000450: 0000 0000 010c 010c 010c 010e 0208 0110  ................
+00000460: 0114 020a 0272 2200 0000 6300 0000 0000  .....r"...c.....
+00000470: 0000 0000 0000 0000 0000 0003 0000 0043  ...............C
+00000480: 0000 0073 0c00 0000 7400 7401 a002 a100  ...s....t.t.....
+00000490: 8301 5300 2901 4e29 03da 046c 6973 7472  ..S.).N)...listr
+000004a0: 1600 0000 da04 6b65 7973 7220 0000 0072  ......keysr ...r
+000004b0: 2000 0000 7220 0000 0072 2100 0000 da11   ...r ...r!.....
+000004c0: 6765 745f 656e 636f 6465 725f 6e61 6d65  get_encoder_name
+000004d0: 732f 0000 0073 0200 0000 0001 7225 0000  s/...s......r%..
+000004e0: 00da 0869 6d61 6765 6e65 7463 0200 0000  ...imagenetc....
+000004f0: 0000 0000 0000 0000 0400 0000 0500 0000  ................
+00000500: 4300 0000 737a 0000 0074 007c 0019 0064  C...sz...t.|...d
+00000510: 0119 007d 027c 017c 02a0 01a1 0076 0172  ...}.|.|.....v.r
+00000520: 2a74 0264 02a0 037c 02a0 01a1 00a1 0183  *t.d...|........
+00000530: 0182 0169 007d 037c 027c 0119 00a0 0464  ...i.}.|.|.....d
+00000540: 03a1 017c 0364 033c 007c 027c 0119 00a0  ...|.d.<.|.|....
+00000550: 0464 04a1 017c 0364 043c 007c 027c 0119  .d...|.d.<.|.|..
+00000560: 00a0 0464 05a1 017c 0364 053c 007c 027c  ...d...|.d.<.|.|
+00000570: 0119 00a0 0464 06a1 017c 0364 063c 007c  .....d...|.d.<.|
+00000580: 0353 0029 074e 7214 0000 007a 1f41 7661  .S.).Nr....z.Ava
+00000590: 6c69 6162 6c65 2070 7265 7472 6169 6e65  liable pretraine
+000005a0: 6420 6f70 7469 6f6e 7320 7b7d 5a0b 696e  d options {}Z.in
+000005b0: 7075 745f 7370 6163 655a 0b69 6e70 7574  put_spaceZ.input
+000005c0: 5f72 616e 6765 da04 6d65 616e da03 7374  _range..mean..st
+000005d0: 6429 0572 1600 0000 7224 0000 00da 0a56  d).r....r$.....V
+000005e0: 616c 7565 4572 726f 72da 0666 6f72 6d61  alueError..forma
+000005f0: 74da 0367 6574 2904 da0c 656e 636f 6465  t..get)...encode
+00000600: 725f 6e61 6d65 da0a 7072 6574 7261 696e  r_name..pretrain
+00000610: 6564 721f 0000 005a 1266 6f72 6d61 7474  edr....Z.formatt
+00000620: 6564 5f73 6574 7469 6e67 7372 2000 0000  ed_settingsr ...
+00000630: 7220 0000 0072 2100 0000 da18 6765 745f  r ...r!.....get_
+00000640: 7072 6570 726f 6365 7373 696e 675f 7061  preprocessing_pa
+00000650: 7261 6d73 3300 0000 7312 0000 0000 010c  rams3...s.......
+00000660: 020c 0112 0204 0112 0112 0112 0112 0172  ...............r
+00000670: 2e00 0000 6302 0000 0000 0000 0000 0000  ....c...........
+00000680: 0003 0000 0004 0000 0043 0000 0073 1e00  .........C...s..
+00000690: 0000 7400 7c00 7c01 6401 8d02 7d02 7401  ..t.|.|.d...}.t.
+000006a0: 6a02 7403 6601 6900 7c02 a401 8e01 5300  j.t.f.i.|.....S.
+000006b0: 2902 4e29 0172 2d00 0000 2904 722e 0000  ).N).r-...).r...
+000006c0: 00da 0966 756e 6374 6f6f 6c73 da07 7061  ...functools..pa
+000006d0: 7274 6961 6c72 0e00 0000 2903 722c 0000  rtialr....).r,..
+000006e0: 0072 2d00 0000 7212 0000 0072 2000 0000  .r-...r....r ...
+000006f0: 7220 0000 0072 2100 0000 da14 6765 745f  r ...r!.....get_
+00000700: 7072 6570 726f 6365 7373 696e 675f 666e  preprocessing_fn
+00000710: 4100 0000 7304 0000 0000 010c 0172 3100  A...s........r1.
+00000720: 0000 2903 720f 0000 0072 1000 0000 4e29  ..).r....r....N)
+00000730: 0172 2600 0000 2901 7226 0000 0029 2272  .r&...).r&...)"r
+00000740: 2f00 0000 da15 746f 7263 682e 7574 696c  /.....torch.util
+00000750: 732e 6d6f 6465 6c5f 7a6f 6fda 0575 7469  s.model_zoo..uti
+00000760: 6c73 7219 0000 00da 0672 6573 6e65 7472  lsr......resnetr
+00000770: 0300 0000 5a03 6470 6e72 0400 0000 da03  ....Z.dpnr......
+00000780: 7667 6772 0500 0000 5a05 7365 6e65 7472  vggr....Z.senetr
+00000790: 0600 0000 da08 6465 6e73 656e 6574 7207  ......densenetr.
+000007a0: 0000 005a 1169 6e63 6570 7469 6f6e 7265  ...Z.inceptionre
+000007b0: 736e 6574 7632 7208 0000 005a 0b69 6e63  snetv2r....Z.inc
+000007c0: 6570 7469 6f6e 7634 7209 0000 00da 0c65  eptionv4r......e
+000007d0: 6666 6963 6965 6e74 6e65 7472 0a00 0000  fficientnetr....
+000007e0: da09 6d6f 6269 6c65 6e65 7472 0b00 0000  ..mobilenetr....
+000007f0: 5a08 7863 6570 7469 6f6e 720c 0000 005a  Z.xceptionr....Z
+00000800: 1174 696d 6d5f 6566 6669 6369 656e 746e  .timm_efficientn
+00000810: 6574 720d 0000 005a 0e5f 7072 6570 726f  etr....Z._prepro
+00000820: 6365 7373 696e 6772 0e00 0000 7216 0000  cessingr....r...
+00000830: 0072 1700 0000 7222 0000 0072 2500 0000  .r....r"...r%...
+00000840: 722e 0000 0072 3100 0000 7220 0000 0072  r....r1...r ...r
+00000850: 2000 0000 7220 0000 0072 2100 0000 da08   ...r ...r!.....
+00000860: 3c6d 6f64 756c 653e 0100 0000 733a 0000  <module>....s:..
+00000870: 0008 0112 020c 010c 010c 010c 010c 010c  ................
+00000880: 010c 010c 010c 010c 010c 020c 0204 010a  ................
+00000890: 010a 010a 010a 010a 010a 010a 010a 010a  ................
+000008a0: 010a 010a 030a 0f08 040a 0e              ...........
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/__init__.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Mar 15 07:44:20 2023 UTC, .py size: 2341 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 5477 1164 2509 0000  a.......Tw.d%...
+00000000: 550d 0d0a 0000 0000 5477 1164 2509 0000  U.......Tw.d%...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4601 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 6d02 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d03 5a03 0100 6402 6403 6c04 6d05  ..m.Z...d.d.l.m.
 00000050: 5a05 0100 6402 6404 6c06 6d07 5a07 0100  Z...d.d.l.m.Z...
 00000060: 6402 6405 6c08 6d09 5a09 0100 6402 6406  d.d.l.m.Z...d.d.
 00000070: 6c0a 6d0b 5a0b 0100 6402 6407 6c0c 6d0d  l.m.Z...d.d.l.m.
@@ -36,104 +36,103 @@
 00000230: 6f62 696c 656e 6574 5f65 6e63 6f64 6572  obilenet_encoder
 00000240: 7329 01da 1178 6365 7074 696f 6e5f 656e  s)...xception_en
 00000250: 636f 6465 7273 2901 da1a 7469 6d6d 5f65  coders)...timm_e
 00000260: 6666 6963 6965 6e74 6e65 745f 656e 636f  fficientnet_enco
 00000270: 6465 7273 2901 da10 7072 6570 726f 6365  ders)...preproce
 00000280: 7373 5f69 6e70 7574 e903 0000 00e9 0500  ss_input........
 00000290: 0000 6304 0000 0000 0000 0000 0000 0008  ..c.............
-000002a0: 0000 0006 0000 0043 0000 0073 6c00 0000  .......C...sl...
+000002a0: 0000 0006 0000 0043 0000 0073 6800 0000  .......C...sh...
 000002b0: 7400 7c00 1900 6401 1900 7d04 7400 7c00  t.|...d...}.t.|.
 000002c0: 1900 6402 1900 7d05 7c05 6a01 7c02 6403  ..d...}.|.j.|.d.
-000002d0: 8d01 0100 7c04 6600 6900 7c05 a401 8e01  ....|.f.i.|.....
-000002e0: 7d06 7c03 6400 7501 725e 7400 7c00 1900  }.|.d.u.r^t.|...
-000002f0: 6404 1900 7c03 1900 7d07 7c06 a002 7403  d...|...}.|...t.
-00000300: a004 7c07 6405 1900 a101 a101 0100 7c06  ..|.d.........|.
-00000310: a005 7c01 a101 0100 7c06 5300 2906 4eda  ..|.....|.S.).N.
-00000320: 0765 6e63 6f64 6572 da06 7061 7261 6d73  .encoder..params
-00000330: 2901 da05 6465 7074 68da 1370 7265 7472  )...depth..pretr
-00000340: 6169 6e65 645f 7365 7474 696e 6773 da03  ained_settings..
-00000350: 7572 6c29 06da 0865 6e63 6f64 6572 73da  url)...encoders.
-00000360: 0675 7064 6174 65da 0f6c 6f61 645f 7374  .update..load_st
-00000370: 6174 655f 6469 6374 da09 6d6f 6465 6c5f  ate_dict..model_
-00000380: 7a6f 6fda 086c 6f61 645f 7572 6c5a 0f73  zoo..load_urlZ.s
-00000390: 6574 5f69 6e5f 6368 616e 6e65 6c73 2908  et_in_channels).
-000003a0: da04 6e61 6d65 da0b 696e 5f63 6861 6e6e  ..name..in_chann
-000003b0: 656c 7372 1300 0000 da07 7765 6967 6874  elsr......weight
-000003c0: 73da 0745 6e63 6f64 6572 7212 0000 0072  s..Encoderr....r
-000003d0: 1100 0000 da08 7365 7474 696e 6773 a900  ......settings..
-000003e0: 7220 0000 00fa 5643 3a5c 5573 6572 735c  r ....VC:\Users\
-000003f0: 6d68 616e 616e 5c44 6573 6b74 6f70 5c44  mhanan\Desktop\D
-00000400: 656e 7369 7479 4170 705c 4465 6e73 6974  ensityApp\Densit
-00000410: 7941 7070 5c73 6567 6d65 6e74 6174 696f  yApp\segmentatio
-00000420: 6e5f 6d6f 6465 6c73 5c65 6e63 6f64 6572  n_models\encoder
-00000430: 735c 5f5f 696e 6974 5f5f 2e70 79da 0b67  s\__init__.py..g
-00000440: 6574 5f65 6e63 6f64 6572 2000 0000 7312  et_encoder ...s.
-00000450: 0000 0000 010c 010c 010c 010e 0208 0110  ................
-00000460: 0114 020a 0272 2200 0000 6300 0000 0000  .....r"...c.....
-00000470: 0000 0000 0000 0000 0000 0003 0000 0043  ...............C
-00000480: 0000 0073 0c00 0000 7400 7401 a002 a100  ...s....t.t.....
-00000490: 8301 5300 2901 4e29 03da 046c 6973 7472  ..S.).N)...listr
-000004a0: 1600 0000 da04 6b65 7973 7220 0000 0072  ......keysr ...r
-000004b0: 2000 0000 7220 0000 0072 2100 0000 da11   ...r ...r!.....
-000004c0: 6765 745f 656e 636f 6465 725f 6e61 6d65  get_encoder_name
-000004d0: 732f 0000 0073 0200 0000 0001 7225 0000  s/...s......r%..
-000004e0: 00da 0869 6d61 6765 6e65 7463 0200 0000  ...imagenetc....
-000004f0: 0000 0000 0000 0000 0400 0000 0500 0000  ................
-00000500: 4300 0000 737a 0000 0074 007c 0019 0064  C...sz...t.|...d
-00000510: 0119 007d 027c 017c 02a0 01a1 0076 0172  ...}.|.|.....v.r
-00000520: 2a74 0264 02a0 037c 02a0 01a1 00a1 0183  *t.d...|........
-00000530: 0182 0169 007d 037c 027c 0119 00a0 0464  ...i.}.|.|.....d
-00000540: 03a1 017c 0364 033c 007c 027c 0119 00a0  ...|.d.<.|.|....
-00000550: 0464 04a1 017c 0364 043c 007c 027c 0119  .d...|.d.<.|.|..
-00000560: 00a0 0464 05a1 017c 0364 053c 007c 027c  ...d...|.d.<.|.|
-00000570: 0119 00a0 0464 06a1 017c 0364 063c 007c  .....d...|.d.<.|
-00000580: 0353 0029 074e 7214 0000 007a 1f41 7661  .S.).Nr....z.Ava
-00000590: 6c69 6162 6c65 2070 7265 7472 6169 6e65  liable pretraine
-000005a0: 6420 6f70 7469 6f6e 7320 7b7d 5a0b 696e  d options {}Z.in
-000005b0: 7075 745f 7370 6163 655a 0b69 6e70 7574  put_spaceZ.input
-000005c0: 5f72 616e 6765 da04 6d65 616e da03 7374  _range..mean..st
-000005d0: 6429 0572 1600 0000 7224 0000 00da 0a56  d).r....r$.....V
-000005e0: 616c 7565 4572 726f 72da 0666 6f72 6d61  alueError..forma
-000005f0: 74da 0367 6574 2904 da0c 656e 636f 6465  t..get)...encode
-00000600: 725f 6e61 6d65 da0a 7072 6574 7261 696e  r_name..pretrain
-00000610: 6564 721f 0000 005a 1266 6f72 6d61 7474  edr....Z.formatt
-00000620: 6564 5f73 6574 7469 6e67 7372 2000 0000  ed_settingsr ...
-00000630: 7220 0000 0072 2100 0000 da18 6765 745f  r ...r!.....get_
-00000640: 7072 6570 726f 6365 7373 696e 675f 7061  preprocessing_pa
-00000650: 7261 6d73 3300 0000 7312 0000 0000 010c  rams3...s.......
-00000660: 020c 0112 0204 0112 0112 0112 0112 0172  ...............r
-00000670: 2e00 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00000680: 0003 0000 0004 0000 0043 0000 0073 1e00  .........C...s..
-00000690: 0000 7400 7c00 7c01 6401 8d02 7d02 7401  ..t.|.|.d...}.t.
-000006a0: 6a02 7403 6601 6900 7c02 a401 8e01 5300  j.t.f.i.|.....S.
-000006b0: 2902 4e29 0172 2d00 0000 2904 722e 0000  ).N).r-...).r...
-000006c0: 00da 0966 756e 6374 6f6f 6c73 da07 7061  ...functools..pa
-000006d0: 7274 6961 6c72 0e00 0000 2903 722c 0000  rtialr....).r,..
-000006e0: 0072 2d00 0000 7212 0000 0072 2000 0000  .r-...r....r ...
-000006f0: 7220 0000 0072 2100 0000 da14 6765 745f  r ...r!.....get_
-00000700: 7072 6570 726f 6365 7373 696e 675f 666e  preprocessing_fn
-00000710: 4100 0000 7304 0000 0000 010c 0172 3100  A...s........r1.
-00000720: 0000 2903 720f 0000 0072 1000 0000 4e29  ..).r....r....N)
-00000730: 0172 2600 0000 2901 7226 0000 0029 2272  .r&...).r&...)"r
-00000740: 2f00 0000 da15 746f 7263 682e 7574 696c  /.....torch.util
-00000750: 732e 6d6f 6465 6c5f 7a6f 6fda 0575 7469  s.model_zoo..uti
-00000760: 6c73 7219 0000 00da 0672 6573 6e65 7472  lsr......resnetr
-00000770: 0300 0000 5a03 6470 6e72 0400 0000 da03  ....Z.dpnr......
-00000780: 7667 6772 0500 0000 5a05 7365 6e65 7472  vggr....Z.senetr
-00000790: 0600 0000 da08 6465 6e73 656e 6574 7207  ......densenetr.
-000007a0: 0000 005a 1169 6e63 6570 7469 6f6e 7265  ...Z.inceptionre
-000007b0: 736e 6574 7632 7208 0000 005a 0b69 6e63  snetv2r....Z.inc
-000007c0: 6570 7469 6f6e 7634 7209 0000 00da 0c65  eptionv4r......e
-000007d0: 6666 6963 6965 6e74 6e65 7472 0a00 0000  fficientnetr....
-000007e0: da09 6d6f 6269 6c65 6e65 7472 0b00 0000  ..mobilenetr....
-000007f0: 5a08 7863 6570 7469 6f6e 720c 0000 005a  Z.xceptionr....Z
-00000800: 1174 696d 6d5f 6566 6669 6369 656e 746e  .timm_efficientn
-00000810: 6574 720d 0000 005a 0e5f 7072 6570 726f  etr....Z._prepro
-00000820: 6365 7373 696e 6772 0e00 0000 7216 0000  cessingr....r...
-00000830: 0072 1700 0000 7222 0000 0072 2500 0000  .r....r"...r%...
-00000840: 722e 0000 0072 3100 0000 7220 0000 0072  r....r1...r ...r
-00000850: 2000 0000 7220 0000 0072 2100 0000 da08   ...r ...r!.....
-00000860: 3c6d 6f64 756c 653e 0100 0000 733a 0000  <module>....s:..
-00000870: 0008 0112 020c 010c 010c 010c 010c 010c  ................
-00000880: 010c 010c 010c 010c 010c 020c 0204 010a  ................
-00000890: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-000008a0: 010a 010a 030a 0f08 040a 0e              ...........
+000002d0: 8d01 0100 7c04 6600 7c05 8e01 7d06 7c03  ....|.f.|...}.|.
+000002e0: 6400 6b09 725a 7400 7c00 1900 6404 1900  d.k.rZt.|...d...
+000002f0: 7c03 1900 7d07 7c06 a002 7403 a004 7c07  |...}.|...t...|.
+00000300: 6405 1900 a101 a101 0100 7c06 a005 7c01  d.........|...|.
+00000310: a101 0100 7c06 5300 2906 4eda 0765 6e63  ....|.S.).N..enc
+00000320: 6f64 6572 da06 7061 7261 6d73 2901 da05  oder..params)...
+00000330: 6465 7074 68da 1370 7265 7472 6169 6e65  depth..pretraine
+00000340: 645f 7365 7474 696e 6773 da03 7572 6c29  d_settings..url)
+00000350: 06da 0865 6e63 6f64 6572 73da 0675 7064  ...encoders..upd
+00000360: 6174 65da 0f6c 6f61 645f 7374 6174 655f  ate..load_state_
+00000370: 6469 6374 da09 6d6f 6465 6c5f 7a6f 6fda  dict..model_zoo.
+00000380: 086c 6f61 645f 7572 6c5a 0f73 6574 5f69  .load_urlZ.set_i
+00000390: 6e5f 6368 616e 6e65 6c73 2908 da04 6e61  n_channels)...na
+000003a0: 6d65 da0b 696e 5f63 6861 6e6e 656c 7372  me..in_channelsr
+000003b0: 1300 0000 da07 7765 6967 6874 73da 0745  ......weights..E
+000003c0: 6e63 6f64 6572 7212 0000 0072 1100 0000  ncoderr....r....
+000003d0: da08 7365 7474 696e 6773 a900 7220 0000  ..settings..r ..
+000003e0: 00fa 4b63 3a5c 5573 6572 735c 6d68 616e  ..Kc:\Users\mhan
+000003f0: 616e 5c44 6f77 6e6c 6f61 6473 5c48 616e  an\Downloads\Han
+00000400: 616e 5c6d 675c 7365 676d 656e 7461 7469  an\mg\segmentati
+00000410: 6f6e 5f6d 6f64 656c 735c 656e 636f 6465  on_models\encode
+00000420: 7273 5c5f 5f69 6e69 745f 5f2e 7079 da0b  rs\__init__.py..
+00000430: 6765 745f 656e 636f 6465 7220 0000 0073  get_encoder ...s
+00000440: 1200 0000 0001 0c01 0c01 0c01 0a02 0801  ................
+00000450: 1001 1402 0a02 7222 0000 0063 0000 0000  ......r"...c....
+00000460: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00000470: 4300 0000 730c 0000 0074 0074 01a0 02a1  C...s....t.t....
+00000480: 0083 0153 0029 014e 2903 da04 6c69 7374  ...S.).N)...list
+00000490: 7216 0000 00da 046b 6579 7372 2000 0000  r......keysr ...
+000004a0: 7220 0000 0072 2000 0000 7221 0000 00da  r ...r ...r!....
+000004b0: 1167 6574 5f65 6e63 6f64 6572 5f6e 616d  .get_encoder_nam
+000004c0: 6573 2f00 0000 7302 0000 0000 0172 2500  es/...s......r%.
+000004d0: 0000 da08 696d 6167 656e 6574 6302 0000  ....imagenetc...
+000004e0: 0000 0000 0000 0000 0004 0000 0005 0000  ................
+000004f0: 0043 0000 0073 7a00 0000 7400 7c00 1900  .C...sz...t.|...
+00000500: 6401 1900 7d02 7c01 7c02 a001 a100 6b07  d...}.|.|.....k.
+00000510: 722a 7402 6402 a003 7c02 a001 a100 a101  r*t.d...|.......
+00000520: 8301 8201 6900 7d03 7c02 7c01 1900 a004  ....i.}.|.|.....
+00000530: 6403 a101 7c03 6403 3c00 7c02 7c01 1900  d...|.d.<.|.|...
+00000540: a004 6404 a101 7c03 6404 3c00 7c02 7c01  ..d...|.d.<.|.|.
+00000550: 1900 a004 6405 a101 7c03 6405 3c00 7c02  ....d...|.d.<.|.
+00000560: 7c01 1900 a004 6406 a101 7c03 6406 3c00  |.....d...|.d.<.
+00000570: 7c03 5300 2907 4e72 1400 0000 7a1f 4176  |.S.).Nr....z.Av
+00000580: 616c 6961 626c 6520 7072 6574 7261 696e  aliable pretrain
+00000590: 6564 206f 7074 696f 6e73 207b 7d5a 0b69  ed options {}Z.i
+000005a0: 6e70 7574 5f73 7061 6365 5a0b 696e 7075  nput_spaceZ.inpu
+000005b0: 745f 7261 6e67 65da 046d 6561 6eda 0373  t_range..mean..s
+000005c0: 7464 2905 7216 0000 0072 2400 0000 da0a  td).r....r$.....
+000005d0: 5661 6c75 6545 7272 6f72 da06 666f 726d  ValueError..form
+000005e0: 6174 da03 6765 7429 04da 0c65 6e63 6f64  at..get)...encod
+000005f0: 6572 5f6e 616d 65da 0a70 7265 7472 6169  er_name..pretrai
+00000600: 6e65 6472 1f00 0000 5a12 666f 726d 6174  nedr....Z.format
+00000610: 7465 645f 7365 7474 696e 6773 7220 0000  ted_settingsr ..
+00000620: 0072 2000 0000 7221 0000 00da 1867 6574  .r ...r!.....get
+00000630: 5f70 7265 7072 6f63 6573 7369 6e67 5f70  _preprocessing_p
+00000640: 6172 616d 7333 0000 0073 1200 0000 0001  arams3...s......
+00000650: 0c02 0c01 1202 0401 1201 1201 1201 1201  ................
+00000660: 722e 0000 0063 0200 0000 0000 0000 0000  r....c..........
+00000670: 0000 0300 0000 0400 0000 4300 0000 731a  ..........C...s.
+00000680: 0000 0074 007c 007c 0164 018d 027d 0274  ...t.|.|.d...}.t
+00000690: 016a 0274 0366 017c 028e 0153 0029 024e  .j.t.f.|...S.).N
+000006a0: 2901 722d 0000 0029 0472 2e00 0000 da09  ).r-...).r......
+000006b0: 6675 6e63 746f 6f6c 73da 0770 6172 7469  functools..parti
+000006c0: 616c 720e 0000 0029 0372 2c00 0000 722d  alr....).r,...r-
+000006d0: 0000 0072 1200 0000 7220 0000 0072 2000  ...r....r ...r .
+000006e0: 0000 7221 0000 00da 1467 6574 5f70 7265  ..r!.....get_pre
+000006f0: 7072 6f63 6573 7369 6e67 5f66 6e41 0000  processing_fnA..
+00000700: 0073 0400 0000 0001 0c01 7231 0000 0029  .s........r1...)
+00000710: 0372 0f00 0000 7210 0000 004e 2901 7226  .r....r....N).r&
+00000720: 0000 0029 0172 2600 0000 2922 722f 0000  ...).r&...)"r/..
+00000730: 00da 1574 6f72 6368 2e75 7469 6c73 2e6d  ...torch.utils.m
+00000740: 6f64 656c 5f7a 6f6f da05 7574 696c 7372  odel_zoo..utilsr
+00000750: 1900 0000 da06 7265 736e 6574 7203 0000  ......resnetr...
+00000760: 005a 0364 706e 7204 0000 00da 0376 6767  .Z.dpnr......vgg
+00000770: 7205 0000 005a 0573 656e 6574 7206 0000  r....Z.senetr...
+00000780: 00da 0864 656e 7365 6e65 7472 0700 0000  ...densenetr....
+00000790: 5a11 696e 6365 7074 696f 6e72 6573 6e65  Z.inceptionresne
+000007a0: 7476 3272 0800 0000 5a0b 696e 6365 7074  tv2r....Z.incept
+000007b0: 696f 6e76 3472 0900 0000 da0c 6566 6669  ionv4r......effi
+000007c0: 6369 656e 746e 6574 720a 0000 00da 096d  cientnetr......m
+000007d0: 6f62 696c 656e 6574 720b 0000 005a 0878  obilenetr....Z.x
+000007e0: 6365 7074 696f 6e72 0c00 0000 5a11 7469  ceptionr....Z.ti
+000007f0: 6d6d 5f65 6666 6963 6965 6e74 6e65 7472  mm_efficientnetr
+00000800: 0d00 0000 5a0e 5f70 7265 7072 6f63 6573  ....Z._preproces
+00000810: 7369 6e67 720e 0000 0072 1600 0000 7217  singr....r....r.
+00000820: 0000 0072 2200 0000 7225 0000 0072 2e00  ...r"...r%...r..
+00000830: 0000 7231 0000 0072 2000 0000 7220 0000  ..r1...r ...r ..
+00000840: 0072 2000 0000 7221 0000 00da 083c 6d6f  .r ...r!.....<mo
+00000850: 6475 6c65 3e01 0000 0073 3a00 0000 0801  dule>....s:.....
+00000860: 1202 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00000870: 0c01 0c01 0c01 0c02 0c02 0401 0a01 0a01  ................
+00000880: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
+00000890: 0a03 0a0f 0804 0a0e                      ........
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_base.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/_base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_base.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/_base.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_base.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/_base.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_base.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/_base.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:20 2023 UTC, .py size: 1372 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -33,82 +33,81 @@
 00000200: 2063 6861 6e6e 656c 7320 6469 6d65 6e73   channels dimens
 00000210: 696f 6e73 2066 6f72 2065 6163 6820 7465  ions for each te
 00000220: 6e73 6f72 206f 6620 666f 7277 6172 6420  nsor of forward 
 00000230: 6f75 7470 7574 206f 6620 656e 636f 6465  output of encode
 00000240: 724e 7204 0000 0029 02da 0d5f 6f75 745f  rNr....)..._out_
 00000250: 6368 616e 6e65 6c73 da06 5f64 6570 7468  channels.._depth
 00000260: a901 da04 7365 6c66 a900 720b 0000 00fa  ....self..r.....
-00000270: 5543 3a5c 5573 6572 735c 6d68 616e 616e  UC:\Users\mhanan
+00000270: 4863 3a5c 5573 6572 735c 6d68 616e 616e  Hc:\Users\mhanan
 00000280: 5c44 6f77 6e6c 6f61 6473 5c48 616e 616e  \Downloads\Hanan
-00000290: 5c4d 616d 6d6f 5079 5c6d 616d 6d6f 7079  \MammoPy\mammopy
-000002a0: 5c73 6567 6d65 6e74 6174 696f 6e5f 6d6f  \segmentation_mo
-000002b0: 6465 6c73 5c65 6e63 6f64 6572 735c 5f62  dels\encoders\_b
-000002c0: 6173 652e 7079 da0c 6f75 745f 6368 616e  ase.py..out_chan
-000002d0: 6e65 6c73 0f00 0000 7302 0000 0000 037a  nels....s......z
-000002e0: 1945 6e63 6f64 6572 4d69 7869 6e2e 6f75  .EncoderMixin.ou
-000002f0: 745f 6368 616e 6e65 6c73 6302 0000 0000  t_channelsc.....
-00000300: 0000 0000 0000 0002 0000 0005 0000 0043  ...............C
-00000310: 0000 0073 5000 0000 7c01 6401 6b02 720c  ...sP...|.d.k.r.
-00000320: 6402 5300 7c01 7c00 5f00 7c00 6a01 6403  d.S.|.|._.|.j.d.
-00000330: 1900 6401 6b02 723e 7402 7c01 6701 7403  ..d.k.r>t.|.g.t.
-00000340: 7c00 6a01 8301 6404 6402 8502 1900 1700  |.j...d.d.......
-00000350: 8301 7c00 5f01 7404 6a05 7c00 7c01 6405  ..|._.t.j.|.|.d.
-00000360: 8d02 0100 6402 5300 2906 7a21 4368 616e  ....d.S.).z!Chan
-00000370: 6765 2066 6972 7374 2063 6f6e 766f 6c75  ge first convolu
-00000380: 7469 6f6e 2063 6865 6e6e 656c 73e9 0300  tion chennels...
-00000390: 0000 4e72 0100 0000 7204 0000 0029 02da  ..Nr....r....)..
-000003a0: 056d 6f64 656c da0b 696e 5f63 6861 6e6e  .model..in_chann
-000003b0: 656c 7329 06da 0c5f 696e 5f63 6861 6e6e  els)..._in_chann
-000003c0: 656c 7372 0700 0000 da05 7475 706c 65da  elsr......tuple.
-000003d0: 046c 6973 74da 0575 7469 6c73 5a10 7061  .list..utilsZ.pa
-000003e0: 7463 685f 6669 7273 745f 636f 6e76 2902  tch_first_conv).
-000003f0: 720a 0000 0072 1000 0000 720b 0000 0072  r....r....r....r
-00000400: 0b00 0000 720c 0000 00da 0f73 6574 5f69  ....r......set_i
-00000410: 6e5f 6368 616e 6e65 6c73 1400 0000 730c  n_channels....s.
-00000420: 0000 0000 0208 0104 0206 010e 011e 027a  ...............z
-00000430: 1c45 6e63 6f64 6572 4d69 7869 6e2e 7365  .EncoderMixin.se
-00000440: 745f 696e 5f63 6861 6e6e 656c 7363 0100  t_in_channelsc..
-00000450: 0000 0000 0000 0000 0000 0100 0000 0100  ................
-00000460: 0000 4300 0000 7308 0000 0074 0082 0164  ..C...s....t...d
-00000470: 0153 0029 027a 264d 6574 686f 6420 7368  .S.).z&Method sh
-00000480: 6f75 6c64 2062 6520 6f76 6572 7269 6464  ould be overridd
-00000490: 656e 2069 6e20 656e 636f 6465 724e 2901  en in encoderN).
-000004a0: da13 4e6f 7449 6d70 6c65 6d65 6e74 6564  ..NotImplemented
-000004b0: 4572 726f 7272 0900 0000 720b 0000 0072  Errorr....r....r
-000004c0: 0b00 0000 720c 0000 00da 0a67 6574 5f73  ....r......get_s
-000004d0: 7461 6765 731f 0000 0073 0200 0000 0002  tages....s......
-000004e0: 7a17 456e 636f 6465 724d 6978 696e 2e67  z.EncoderMixin.g
-000004f0: 6574 5f73 7461 6765 7363 0300 0000 0000  et_stagesc......
-00000500: 0000 0000 0000 0600 0000 0500 0000 4300  ..............C.
-00000510: 0000 7332 0000 007c 00a0 00a1 007d 0374  ..s2...|.....}.t
-00000520: 017c 017c 0283 0244 005d 1a5c 027d 047d  .|.|...D.].\.}.}
-00000530: 0574 026a 037c 037c 0419 007c 0564 018d  .t.j.|.|...|.d..
-00000540: 0201 0071 1264 0053 0029 024e 2902 da06  ...q.d.S.).N)...
-00000550: 6d6f 6475 6c65 da0d 6469 6c61 7469 6f6e  module..dilation
-00000560: 5f72 6174 6529 0472 1700 0000 da03 7a69  _rate).r......zi
-00000570: 7072 1400 0000 5a1d 7265 706c 6163 655f  pr....Z.replace_
-00000580: 7374 7269 6465 735f 7769 7468 5f64 696c  strides_with_dil
-00000590: 6174 696f 6e29 0672 0a00 0000 5a0a 7374  ation).r....Z.st
-000005a0: 6167 655f 6c69 7374 5a0d 6469 6c61 7469  age_listZ.dilati
-000005b0: 6f6e 5f6c 6973 74da 0673 7461 6765 735a  on_list..stagesZ
-000005c0: 0a73 7461 6765 5f69 6e64 7872 1900 0000  .stage_indxr....
-000005d0: 720b 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
-000005e0: 0c6d 616b 655f 6469 6c61 7465 6423 0000  .make_dilated#..
-000005f0: 0073 0c00 0000 0001 0801 1201 0401 0601  .s..............
-00000600: 02fe 7a19 456e 636f 6465 724d 6978 696e  ..z.EncoderMixin
-00000610: 2e6d 616b 655f 6469 6c61 7465 644e 2909  .make_dilatedN).
-00000620: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000630: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000640: 6d65 5f5f da07 5f5f 646f 635f 5fda 0870  me__..__doc__..p
-00000650: 726f 7065 7274 7972 0d00 0000 7215 0000  ropertyr....r...
-00000660: 0072 1700 0000 721c 0000 0072 0b00 0000  .r....r....r....
-00000670: 720b 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
-00000680: 0600 0000 0900 0000 730c 0000 0008 0104  ........s.......
-00000690: 0502 010a 0408 0b08 0472 0600 0000 290b  .........r....).
-000006a0: da05 746f 7263 68da 0874 6f72 6368 2e6e  ..torch..torch.n
-000006b0: 6eda 026e 6eda 0674 7970 696e 6772 0200  n..nn..typingr..
-000006c0: 0000 da0b 636f 6c6c 6563 7469 6f6e 7372  ....collectionsr
-000006d0: 0300 0000 da00 7205 0000 0072 1400 0000  ......r....r....
-000006e0: 7206 0000 0072 0b00 0000 720b 0000 0072  r....r....r....r
-000006f0: 0b00 0000 720c 0000 00da 083c 6d6f 6475  ....r......<modu
-00000700: 6c65 3e01 0000 0073 0a00 0000 0801 0c01  le>....s........
-00000710: 0c01 0c02 0c03                           ......
+00000290: 5c6d 675c 7365 676d 656e 7461 7469 6f6e  \mg\segmentation
+000002a0: 5f6d 6f64 656c 735c 656e 636f 6465 7273  _models\encoders
+000002b0: 5c5f 6261 7365 2e70 79da 0c6f 7574 5f63  \_base.py..out_c
+000002c0: 6861 6e6e 656c 730f 0000 0073 0200 0000  hannels....s....
+000002d0: 0003 7a19 456e 636f 6465 724d 6978 696e  ..z.EncoderMixin
+000002e0: 2e6f 7574 5f63 6861 6e6e 656c 7363 0200  .out_channelsc..
+000002f0: 0000 0000 0000 0000 0000 0200 0000 0500  ................
+00000300: 0000 4300 0000 7350 0000 007c 0164 016b  ..C...sP...|.d.k
+00000310: 0272 0c64 0253 007c 017c 005f 007c 006a  .r.d.S.|.|._.|.j
+00000320: 0164 0319 0064 016b 0272 3e74 027c 0167  .d...d.k.r>t.|.g
+00000330: 0174 037c 006a 0183 0164 0464 0285 0219  .t.|.j...d.d....
+00000340: 0017 0083 017c 005f 0174 046a 057c 007c  .....|._.t.j.|.|
+00000350: 0164 058d 0201 0064 0253 0029 067a 2143  .d.....d.S.).z!C
+00000360: 6861 6e67 6520 6669 7273 7420 636f 6e76  hange first conv
+00000370: 6f6c 7574 696f 6e20 6368 656e 6e65 6c73  olution chennels
+00000380: e903 0000 004e 7201 0000 0072 0400 0000  .....Nr....r....
+00000390: 2902 da05 6d6f 6465 6cda 0b69 6e5f 6368  )...model..in_ch
+000003a0: 616e 6e65 6c73 2906 da0c 5f69 6e5f 6368  annels)..._in_ch
+000003b0: 616e 6e65 6c73 7207 0000 00da 0574 7570  annelsr......tup
+000003c0: 6c65 da04 6c69 7374 da05 7574 696c 735a  le..list..utilsZ
+000003d0: 1070 6174 6368 5f66 6972 7374 5f63 6f6e  .patch_first_con
+000003e0: 7629 0272 0a00 0000 7210 0000 0072 0b00  v).r....r....r..
+000003f0: 0000 720b 0000 0072 0c00 0000 da0f 7365  ..r....r......se
+00000400: 745f 696e 5f63 6861 6e6e 656c 7314 0000  t_in_channels...
+00000410: 0073 0c00 0000 0002 0801 0402 0601 0e01  .s..............
+00000420: 1e02 7a1c 456e 636f 6465 724d 6978 696e  ..z.EncoderMixin
+00000430: 2e73 6574 5f69 6e5f 6368 616e 6e65 6c73  .set_in_channels
+00000440: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000450: 0001 0000 0043 0000 0073 0800 0000 7400  .....C...s....t.
+00000460: 8201 6401 5300 2902 7a26 4d65 7468 6f64  ..d.S.).z&Method
+00000470: 2073 686f 756c 6420 6265 206f 7665 7272   should be overr
+00000480: 6964 6465 6e20 696e 2065 6e63 6f64 6572  idden in encoder
+00000490: 4e29 01da 134e 6f74 496d 706c 656d 656e  N)...NotImplemen
+000004a0: 7465 6445 7272 6f72 7209 0000 0072 0b00  tedErrorr....r..
+000004b0: 0000 720b 0000 0072 0c00 0000 da0a 6765  ..r....r......ge
+000004c0: 745f 7374 6167 6573 1f00 0000 7302 0000  t_stages....s...
+000004d0: 0000 027a 1745 6e63 6f64 6572 4d69 7869  ...z.EncoderMixi
+000004e0: 6e2e 6765 745f 7374 6167 6573 6303 0000  n.get_stagesc...
+000004f0: 0000 0000 0000 0000 0006 0000 0005 0000  ................
+00000500: 0043 0000 0073 3200 0000 7c00 a000 a100  .C...s2...|.....
+00000510: 7d03 7401 7c01 7c02 8302 4400 5d1a 5c02  }.t.|.|...D.].\.
+00000520: 7d04 7d05 7402 6a03 7c03 7c04 1900 7c05  }.}.t.j.|.|...|.
+00000530: 6401 8d02 0100 7112 6400 5300 2902 4e29  d.....q.d.S.).N)
+00000540: 02da 066d 6f64 756c 65da 0d64 696c 6174  ...module..dilat
+00000550: 696f 6e5f 7261 7465 2904 7217 0000 00da  ion_rate).r.....
+00000560: 037a 6970 7214 0000 005a 1d72 6570 6c61  .zipr....Z.repla
+00000570: 6365 5f73 7472 6964 6573 5f77 6974 685f  ce_strides_with_
+00000580: 6469 6c61 7469 6f6e 2906 720a 0000 005a  dilation).r....Z
+00000590: 0a73 7461 6765 5f6c 6973 745a 0d64 696c  .stage_listZ.dil
+000005a0: 6174 696f 6e5f 6c69 7374 da06 7374 6167  ation_list..stag
+000005b0: 6573 5a0a 7374 6167 655f 696e 6478 7219  esZ.stage_indxr.
+000005c0: 0000 0072 0b00 0000 720b 0000 0072 0c00  ...r....r....r..
+000005d0: 0000 da0c 6d61 6b65 5f64 696c 6174 6564  ....make_dilated
+000005e0: 2300 0000 730c 0000 0000 0108 0112 0104  #...s...........
+000005f0: 0106 0102 fe7a 1945 6e63 6f64 6572 4d69  .....z.EncoderMi
+00000600: 7869 6e2e 6d61 6b65 5f64 696c 6174 6564  xin.make_dilated
+00000610: 4e29 09da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00000620: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000630: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
+00000640: da08 7072 6f70 6572 7479 720d 0000 0072  ..propertyr....r
+00000650: 1500 0000 7217 0000 0072 1c00 0000 720b  ....r....r....r.
+00000660: 0000 0072 0b00 0000 720b 0000 0072 0c00  ...r....r....r..
+00000670: 0000 7206 0000 0009 0000 0073 0c00 0000  ..r........s....
+00000680: 0801 0405 0201 0a04 080b 0804 7206 0000  ............r...
+00000690: 0029 0bda 0574 6f72 6368 da08 746f 7263  .)...torch..torc
+000006a0: 682e 6e6e da02 6e6e da06 7479 7069 6e67  h.nn..nn..typing
+000006b0: 7202 0000 00da 0b63 6f6c 6c65 6374 696f  r......collectio
+000006c0: 6e73 7203 0000 00da 0072 0500 0000 7214  nsr......r....r.
+000006d0: 0000 0072 0600 0000 720b 0000 0072 0b00  ...r....r....r..
+000006e0: 0000 720b 0000 0072 0c00 0000 da08 3c6d  ..r....r......<m
+000006f0: 6f64 756c 653e 0100 0000 730a 0000 0008  odule>....s.....
+00000700: 010c 010c 010c 020c 03                   .........
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_base.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/_base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/_preprocessing.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/_preprocessing.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/_preprocessing.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/_preprocessing.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:20 2023 UTC, .py size: 476 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 000000e0: 027c 007c 021b 007d 007c 0053 0029 064e  .|.|...}.|.S.).N
 000000f0: da03 4247 522e e9ff ffff ffe9 0100 0000  ..BGR...........
 00000100: 6700 0000 0000 e06f 4029 04da 0463 6f70  g......o@)...cop
 00000110: 79da 036d 6178 da02 6e70 da05 6172 7261  y..max..np..arra
 00000120: 7929 06da 0178 da04 6d65 616e da03 7374  y)...x..mean..st
 00000130: 64da 0b69 6e70 7574 5f73 7061 6365 da0b  d..input_space..
 00000140: 696e 7075 745f 7261 6e67 65da 066b 7761  input_range..kwa
-00000150: 7267 73a9 0072 1000 0000 fa5e 433a 5c55  rgs..r.....^C:\U
+00000150: 7267 73a9 0072 1000 0000 fa51 633a 5c55  rgs..r.....Qc:\U
 00000160: 7365 7273 5c6d 6861 6e61 6e5c 446f 776e  sers\mhanan\Down
-00000170: 6c6f 6164 735c 4861 6e61 6e5c 4d61 6d6d  loads\Hanan\Mamm
-00000180: 6f50 795c 6d61 6d6d 6f70 795c 7365 676d  oPy\mammopy\segm
-00000190: 656e 7461 7469 6f6e 5f6d 6f64 656c 735c  entation_models\
-000001a0: 656e 636f 6465 7273 5c5f 7072 6570 726f  encoders\_prepro
-000001b0: 6365 7373 696e 672e 7079 da10 7072 6570  cessing.py..prep
-000001c0: 726f 6365 7373 5f69 6e70 7574 0400 0000  rocess_input....
-000001d0: 7318 0000 0000 0408 0116 0208 0118 0108  s...............
-000001e0: 0208 010a 0108 0208 010a 0108 0272 1200  .............r..
-000001f0: 0000 2904 4e4e 7202 0000 004e 2903 da05  ..).NNr....N)...
-00000200: 6e75 6d70 7972 0800 0000 7212 0000 0072  numpyr....r....r
-00000210: 1000 0000 7210 0000 0072 1000 0000 7211  ....r....r....r.
-00000220: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000230: 0073 0a00 0000 0804 0000 0000 0000 00ff  .s..............
+00000170: 6c6f 6164 735c 4861 6e61 6e5c 6d67 5c73  loads\Hanan\mg\s
+00000180: 6567 6d65 6e74 6174 696f 6e5f 6d6f 6465  egmentation_mode
+00000190: 6c73 5c65 6e63 6f64 6572 735c 5f70 7265  ls\encoders\_pre
+000001a0: 7072 6f63 6573 7369 6e67 2e70 79da 1070  processing.py..p
+000001b0: 7265 7072 6f63 6573 735f 696e 7075 7404  reprocess_input.
+000001c0: 0000 0073 1800 0000 0004 0801 1602 0801  ...s............
+000001d0: 1801 0802 0801 0a01 0802 0801 0a01 0802  ................
+000001e0: 7212 0000 0029 044e 4e72 0200 0000 4e29  r....).NNr....N)
+000001f0: 03da 056e 756d 7079 7208 0000 0072 1200  ...numpyr....r..
+00000200: 0000 7210 0000 0072 1000 0000 7210 0000  ..r....r....r...
+00000210: 0072 1100 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000220: 0100 0000 730a 0000 0008 0400 0000 0000  ....s...........
+00000230: 0000 ff                                  ...
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_preprocessing.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/_preprocessing.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_utils.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_utils.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/_utils.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_utils.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/_utils.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_utils.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/_utils.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:20 2023 UTC, .py size: 1565 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-00000000: 550d 0d0a 0000 0000 5477 1164 1d06 0000  U.......Tw.d....
+00000000: 610d 0d0a 0000 0000 5477 1164 1d06 0000  a.......Tw.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6402 6403 8400 5a03 6404 6405 8400  ..d.d...Z.d.d...
 00000050: 5a04 6401 5300 2906 e900 0000 004e 6302  Z.d.S.)......Nc.
 00000060: 0000 0000 0000 0000 0000 0005 0000 0004  ................
-00000070: 0000 0043 0000 0073 ac00 0000 7c00 a000  ...C...s....|...
+00000070: 0000 0043 0000 0073 ae00 0000 7c00 a000  ...C...s....|...
 00000080: a100 4400 5d14 7d02 7401 7c02 7402 6a03  ..D.].}.t.|.t.j.
 00000090: 8302 7208 0100 711e 7108 7c01 7c02 5f04  ..r...q.q.|.|._.
 000000a0: 7c02 6a05 a006 a100 7d03 6401 7d04 7c01  |.j.....}.d.}.|.
 000000b0: 6402 6b02 724a 7c03 6a07 6402 6403 6404  d.k.rJ|.j.d.d.d.
-000000c0: 8d02 7d03 6e44 7c01 6405 6b02 726c 7c03  ..}.nD|.d.k.rl|.
+000000c0: 8d02 7d03 6e46 7c01 6405 6b02 726c 7c03  ..}.nF|.d.k.rl|.
 000000d0: 6406 6406 8502 6406 6405 8502 6602 1900  d.d...d.d...f...
-000000e0: 6407 1400 7d03 6e22 6403 7d04 7408 6a09  d...}.n"d.}.t.j.
-000000f0: 7c02 6a0a 7c02 6a04 7c02 6a0b 1a00 6602  |.j.|.j.|.j...f.
-00000100: 7c02 6a0c 9e02 8e00 7d03 7402 6a0d a00e  |.j.....}.t.j...
-00000110: 7c03 a101 7c02 5f05 7c04 72a8 7c02 a00f  |...|._.|.r.|...
-00000120: a100 0100 6406 5300 2908 7acc 4368 616e  ....d.S.).z.Chan
-00000130: 6765 2066 6972 7374 2063 6f6e 766f 6c75  ge first convolu
-00000140: 7469 6f6e 206c 6179 6572 2069 6e70 7574  tion layer input
-00000150: 2063 6861 6e6e 656c 732e 0a20 2020 2049   channels..    I
-00000160: 6e20 6361 7365 3a0a 2020 2020 2020 2020  n case:.        
-00000170: 696e 5f63 6861 6e6e 656c 7320 3d3d 2031  in_channels == 1
-00000180: 206f 7220 696e 5f63 6861 6e6e 656c 7320   or in_channels 
-00000190: 3d3d 2032 202d 3e20 7265 7573 6520 6f72  == 2 -> reuse or
-000001a0: 6967 696e 616c 2077 6569 6768 7473 0a20  iginal weights. 
-000001b0: 2020 2020 2020 2069 6e5f 6368 616e 6e65         in_channe
-000001c0: 6c73 203e 2033 202d 3e20 6d61 6b65 2072  ls > 3 -> make r
-000001d0: 616e 646f 6d20 6b61 696d 696e 6720 6e6f  andom kaiming no
-000001e0: 726d 616c 2069 6e69 7469 616c 697a 6174  rmal initializat
-000001f0: 696f 6e0a 2020 2020 46e9 0100 0000 5429  ion.    F.....T)
-00000200: 01da 076b 6565 7064 696d e902 0000 004e  ...keepdim.....N
-00000210: 6700 0000 0000 00f8 3f29 10da 076d 6f64  g.......?)...mod
-00000220: 756c 6573 da0a 6973 696e 7374 616e 6365  ules..isinstance
-00000230: da02 6e6e da06 436f 6e76 3264 da0b 696e  ..nn..Conv2d..in
-00000240: 5f63 6861 6e6e 656c 73da 0677 6569 6768  _channels..weigh
-00000250: 74da 0664 6574 6163 68da 0373 756d da05  t..detach..sum..
-00000260: 746f 7263 68da 0654 656e 736f 72da 0c6f  torch..Tensor..o
-00000270: 7574 5f63 6861 6e6e 656c 73da 0667 726f  ut_channels..gro
-00000280: 7570 73da 0b6b 6572 6e65 6c5f 7369 7a65  ups..kernel_size
-00000290: da09 7061 7261 6d65 7465 72da 0950 6172  ..parameter..Par
-000002a0: 616d 6574 6572 da10 7265 7365 745f 7061  ameter..reset_pa
-000002b0: 7261 6d65 7465 7273 2905 da05 6d6f 6465  rameters)...mode
-000002c0: 6c72 0900 0000 da06 6d6f 6475 6c65 720a  lr......moduler.
-000002d0: 0000 00da 0572 6573 6574 a900 7218 0000  .....reset..r...
-000002e0: 00fa 5643 3a5c 5573 6572 735c 6d68 616e  ..VC:\Users\mhan
-000002f0: 616e 5c44 6f77 6e6c 6f61 6473 5c48 616e  an\Downloads\Han
-00000300: 616e 5c4d 616d 6d6f 5079 5c6d 616d 6d6f  an\MammoPy\mammo
-00000310: 7079 5c73 6567 6d65 6e74 6174 696f 6e5f  py\segmentation_
+000000e0: 6407 1400 7d03 6e24 6403 7d04 7408 6a09  d...}.n$d.}.t.j.
+000000f0: 7c02 6a0a 7c02 6a04 7c02 6a0b 1a00 6702  |.j.|.j.|.j...g.
+00000100: 7c02 6a0c a201 5200 8e00 7d03 7402 6a0d  |.j...R...}.t.j.
+00000110: a00e 7c03 a101 7c02 5f05 7c04 72aa 7c02  ..|...|._.|.r.|.
+00000120: a00f a100 0100 6406 5300 2908 7acc 4368  ......d.S.).z.Ch
+00000130: 616e 6765 2066 6972 7374 2063 6f6e 766f  ange first convo
+00000140: 6c75 7469 6f6e 206c 6179 6572 2069 6e70  lution layer inp
+00000150: 7574 2063 6861 6e6e 656c 732e 0a20 2020  ut channels..   
+00000160: 2049 6e20 6361 7365 3a0a 2020 2020 2020   In case:.      
+00000170: 2020 696e 5f63 6861 6e6e 656c 7320 3d3d    in_channels ==
+00000180: 2031 206f 7220 696e 5f63 6861 6e6e 656c   1 or in_channel
+00000190: 7320 3d3d 2032 202d 3e20 7265 7573 6520  s == 2 -> reuse 
+000001a0: 6f72 6967 696e 616c 2077 6569 6768 7473  original weights
+000001b0: 0a20 2020 2020 2020 2069 6e5f 6368 616e  .        in_chan
+000001c0: 6e65 6c73 203e 2033 202d 3e20 6d61 6b65  nels > 3 -> make
+000001d0: 2072 616e 646f 6d20 6b61 696d 696e 6720   random kaiming 
+000001e0: 6e6f 726d 616c 2069 6e69 7469 616c 697a  normal initializ
+000001f0: 6174 696f 6e0a 2020 2020 46e9 0100 0000  ation.    F.....
+00000200: 5429 01da 076b 6565 7064 696d e902 0000  T)...keepdim....
+00000210: 004e 6700 0000 0000 00f8 3f29 10da 076d  .Ng.......?)...m
+00000220: 6f64 756c 6573 da0a 6973 696e 7374 616e  odules..isinstan
+00000230: 6365 da02 6e6e da06 436f 6e76 3264 da0b  ce..nn..Conv2d..
+00000240: 696e 5f63 6861 6e6e 656c 73da 0677 6569  in_channels..wei
+00000250: 6768 74da 0664 6574 6163 68da 0373 756d  ght..detach..sum
+00000260: da05 746f 7263 68da 0654 656e 736f 72da  ..torch..Tensor.
+00000270: 0c6f 7574 5f63 6861 6e6e 656c 73da 0667  .out_channels..g
+00000280: 726f 7570 73da 0b6b 6572 6e65 6c5f 7369  roups..kernel_si
+00000290: 7a65 da09 7061 7261 6d65 7465 72da 0950  ze..parameter..P
+000002a0: 6172 616d 6574 6572 da10 7265 7365 745f  arameter..reset_
+000002b0: 7061 7261 6d65 7465 7273 2905 da05 6d6f  parameters)...mo
+000002c0: 6465 6c72 0900 0000 da06 6d6f 6475 6c65  delr......module
+000002d0: 720a 0000 00da 0572 6573 6574 a900 7218  r......reset..r.
+000002e0: 0000 00fa 5443 3a5c 5573 6572 735c 6d68  ....TC:\Users\mh
+000002f0: 616e 616e 5c44 6573 6b74 6f70 5c44 656e  anan\Desktop\Den
+00000300: 7369 7479 4170 705c 4465 6e73 6974 7941  sityApp\DensityA
+00000310: 7070 5c73 6567 6d65 6e74 6174 696f 6e5f  pp\segmentation_
 00000320: 6d6f 6465 6c73 5c65 6e63 6f64 6572 735c  models\encoders\
 00000330: 5f75 7469 6c73 2e70 79da 1070 6174 6368  _utils.py..patch
 00000340: 5f66 6972 7374 5f63 6f6e 7605 0000 0073  _first_conv....s
 00000350: 2800 0000 0008 0c01 0c01 0603 0601 0a01  (...............
 00000360: 0402 0801 1001 0801 1a02 0401 0401 0401  ................
-00000370: 0afe 0203 04fd 0606 0e01 0401 721a 0000  ............r...
+00000370: 0afe 0203 04fd 0806 0e01 0401 721a 0000  ............r...
 00000380: 0063 0200 0000 0000 0000 0000 0000 0500  .c..............
 00000390: 0000 0400 0000 4300 0000 7366 0000 007c  ......C...sf...|
 000003a0: 00a0 00a1 0044 005d 587d 0274 017c 0274  .....D.]X}.t.|.t
 000003b0: 026a 0383 0272 0864 017c 025f 047c 017c  .j...r.d.|._.|.|
 000003c0: 0166 027c 025f 057c 026a 065c 027d 037d  .f.|._.|.j.\.}.}
 000003d0: 047c 0364 021a 007c 0114 007c 0364 021a  .|.d...|...|.d..
 000003e0: 007c 0114 0066 027c 025f 0774 087c 0264  .|...f.|._.t.|.d
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/_utils.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Mar 15 07:44:20 2023 UTC, .py size: 1565 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,87 +1,86 @@
-00000000: 610d 0d0a 0000 0000 5477 1164 1d06 0000  a.......Tw.d....
+00000000: 550d 0d0a 0000 0000 5477 1164 1d06 0000  U.......Tw.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6402 6403 8400 5a03 6404 6405 8400  ..d.d...Z.d.d...
 00000050: 5a04 6401 5300 2906 e900 0000 004e 6302  Z.d.S.)......Nc.
 00000060: 0000 0000 0000 0000 0000 0005 0000 0004  ................
-00000070: 0000 0043 0000 0073 ae00 0000 7c00 a000  ...C...s....|...
+00000070: 0000 0043 0000 0073 ac00 0000 7c00 a000  ...C...s....|...
 00000080: a100 4400 5d14 7d02 7401 7c02 7402 6a03  ..D.].}.t.|.t.j.
 00000090: 8302 7208 0100 711e 7108 7c01 7c02 5f04  ..r...q.q.|.|._.
 000000a0: 7c02 6a05 a006 a100 7d03 6401 7d04 7c01  |.j.....}.d.}.|.
 000000b0: 6402 6b02 724a 7c03 6a07 6402 6403 6404  d.k.rJ|.j.d.d.d.
-000000c0: 8d02 7d03 6e46 7c01 6405 6b02 726c 7c03  ..}.nF|.d.k.rl|.
+000000c0: 8d02 7d03 6e44 7c01 6405 6b02 726c 7c03  ..}.nD|.d.k.rl|.
 000000d0: 6406 6406 8502 6406 6405 8502 6602 1900  d.d...d.d...f...
-000000e0: 6407 1400 7d03 6e24 6403 7d04 7408 6a09  d...}.n$d.}.t.j.
-000000f0: 7c02 6a0a 7c02 6a04 7c02 6a0b 1a00 6702  |.j.|.j.|.j...g.
-00000100: 7c02 6a0c a201 5200 8e00 7d03 7402 6a0d  |.j...R...}.t.j.
-00000110: a00e 7c03 a101 7c02 5f05 7c04 72aa 7c02  ..|...|._.|.r.|.
-00000120: a00f a100 0100 6406 5300 2908 7acc 4368  ......d.S.).z.Ch
-00000130: 616e 6765 2066 6972 7374 2063 6f6e 766f  ange first convo
-00000140: 6c75 7469 6f6e 206c 6179 6572 2069 6e70  lution layer inp
-00000150: 7574 2063 6861 6e6e 656c 732e 0a20 2020  ut channels..   
-00000160: 2049 6e20 6361 7365 3a0a 2020 2020 2020   In case:.      
-00000170: 2020 696e 5f63 6861 6e6e 656c 7320 3d3d    in_channels ==
-00000180: 2031 206f 7220 696e 5f63 6861 6e6e 656c   1 or in_channel
-00000190: 7320 3d3d 2032 202d 3e20 7265 7573 6520  s == 2 -> reuse 
-000001a0: 6f72 6967 696e 616c 2077 6569 6768 7473  original weights
-000001b0: 0a20 2020 2020 2020 2069 6e5f 6368 616e  .        in_chan
-000001c0: 6e65 6c73 203e 2033 202d 3e20 6d61 6b65  nels > 3 -> make
-000001d0: 2072 616e 646f 6d20 6b61 696d 696e 6720   random kaiming 
-000001e0: 6e6f 726d 616c 2069 6e69 7469 616c 697a  normal initializ
-000001f0: 6174 696f 6e0a 2020 2020 46e9 0100 0000  ation.    F.....
-00000200: 5429 01da 076b 6565 7064 696d e902 0000  T)...keepdim....
-00000210: 004e 6700 0000 0000 00f8 3f29 10da 076d  .Ng.......?)...m
-00000220: 6f64 756c 6573 da0a 6973 696e 7374 616e  odules..isinstan
-00000230: 6365 da02 6e6e da06 436f 6e76 3264 da0b  ce..nn..Conv2d..
-00000240: 696e 5f63 6861 6e6e 656c 73da 0677 6569  in_channels..wei
-00000250: 6768 74da 0664 6574 6163 68da 0373 756d  ght..detach..sum
-00000260: da05 746f 7263 68da 0654 656e 736f 72da  ..torch..Tensor.
-00000270: 0c6f 7574 5f63 6861 6e6e 656c 73da 0667  .out_channels..g
-00000280: 726f 7570 73da 0b6b 6572 6e65 6c5f 7369  roups..kernel_si
-00000290: 7a65 da09 7061 7261 6d65 7465 72da 0950  ze..parameter..P
-000002a0: 6172 616d 6574 6572 da10 7265 7365 745f  arameter..reset_
-000002b0: 7061 7261 6d65 7465 7273 2905 da05 6d6f  parameters)...mo
-000002c0: 6465 6c72 0900 0000 da06 6d6f 6475 6c65  delr......module
-000002d0: 720a 0000 00da 0572 6573 6574 a900 7218  r......reset..r.
-000002e0: 0000 00fa 5443 3a5c 5573 6572 735c 6d68  ....TC:\Users\mh
-000002f0: 616e 616e 5c44 6573 6b74 6f70 5c44 656e  anan\Desktop\Den
-00000300: 7369 7479 4170 705c 4465 6e73 6974 7941  sityApp\DensityA
-00000310: 7070 5c73 6567 6d65 6e74 6174 696f 6e5f  pp\segmentation_
-00000320: 6d6f 6465 6c73 5c65 6e63 6f64 6572 735c  models\encoders\
-00000330: 5f75 7469 6c73 2e70 79da 1070 6174 6368  _utils.py..patch
-00000340: 5f66 6972 7374 5f63 6f6e 7605 0000 0073  _first_conv....s
-00000350: 2800 0000 0008 0c01 0c01 0603 0601 0a01  (...............
-00000360: 0402 0801 1001 0801 1a02 0401 0401 0401  ................
-00000370: 0afe 0203 04fd 0806 0e01 0401 721a 0000  ............r...
-00000380: 0063 0200 0000 0000 0000 0000 0000 0500  .c..............
-00000390: 0000 0400 0000 4300 0000 7366 0000 007c  ......C...sf...|
-000003a0: 00a0 00a1 0044 005d 587d 0274 017c 0274  .....D.]X}.t.|.t
-000003b0: 026a 0383 0272 0864 017c 025f 047c 017c  .j...r.d.|._.|.|
-000003c0: 0166 027c 025f 057c 026a 065c 027d 037d  .f.|._.|.j.\.}.}
-000003d0: 047c 0364 021a 007c 0114 007c 0364 021a  .|.d...|...|.d..
-000003e0: 007c 0114 0066 027c 025f 0774 087c 0264  .|...f.|._.t.|.d
-000003f0: 0383 0272 0874 02a0 09a1 007c 025f 0a71  ...r.t.....|._.q
-00000400: 0864 0453 0029 057a 3450 6174 6368 2043  .d.S.).z4Patch C
-00000410: 6f6e 7632 6420 6d6f 6475 6c65 7320 7265  onv2d modules re
-00000420: 706c 6163 696e 6720 7374 7269 6465 7320  placing strides 
-00000430: 7769 7468 2064 696c 6174 696f 6e29 0272  with dilation).r
-00000440: 0200 0000 7202 0000 0072 0400 0000 da0e  ....r....r......
-00000450: 7374 6174 6963 5f70 6164 6469 6e67 4e29  static_paddingN)
-00000460: 0b72 0500 0000 7206 0000 0072 0700 0000  .r....r....r....
-00000470: 7208 0000 00da 0673 7472 6964 65da 0864  r......stride..d
-00000480: 696c 6174 696f 6e72 1100 0000 da07 7061  ilationr......pa
-00000490: 6464 696e 67da 0768 6173 6174 7472 da08  dding..hasattr..
-000004a0: 4964 656e 7469 7479 721b 0000 0029 0572  Identityr....).r
-000004b0: 1600 0000 da0d 6469 6c61 7469 6f6e 5f72  ......dilation_r
-000004c0: 6174 65da 036d 6f64 da02 6b68 da02 6b77  ate..mod..kh..kw
-000004d0: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
-000004e0: 1d72 6570 6c61 6365 5f73 7472 6964 6573  .replace_strides
-000004f0: 5f77 6974 685f 6469 6c61 7469 6f6e 2700  _with_dilation'.
-00000500: 0000 7310 0000 0000 020c 010c 0106 010a  ..s.............
-00000510: 010a 011a 030a 0172 2500 0000 2905 720d  .......r%...).r.
-00000520: 0000 00da 0874 6f72 6368 2e6e 6e72 0700  .....torch.nnr..
-00000530: 0000 721a 0000 0072 2500 0000 7218 0000  ..r....r%...r...
-00000540: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00000550: da08 3c6d 6f64 756c 653e 0100 0000 7306  ..<module>....s.
-00000560: 0000 0008 010c 0308 22                   ........"
+000000e0: 6407 1400 7d03 6e22 6403 7d04 7408 6a09  d...}.n"d.}.t.j.
+000000f0: 7c02 6a0a 7c02 6a04 7c02 6a0b 1a00 6602  |.j.|.j.|.j...f.
+00000100: 7c02 6a0c 9e02 8e00 7d03 7402 6a0d a00e  |.j.....}.t.j...
+00000110: 7c03 a101 7c02 5f05 7c04 72a8 7c02 a00f  |...|._.|.r.|...
+00000120: a100 0100 6406 5300 2908 7acc 4368 616e  ....d.S.).z.Chan
+00000130: 6765 2066 6972 7374 2063 6f6e 766f 6c75  ge first convolu
+00000140: 7469 6f6e 206c 6179 6572 2069 6e70 7574  tion layer input
+00000150: 2063 6861 6e6e 656c 732e 0a20 2020 2049   channels..    I
+00000160: 6e20 6361 7365 3a0a 2020 2020 2020 2020  n case:.        
+00000170: 696e 5f63 6861 6e6e 656c 7320 3d3d 2031  in_channels == 1
+00000180: 206f 7220 696e 5f63 6861 6e6e 656c 7320   or in_channels 
+00000190: 3d3d 2032 202d 3e20 7265 7573 6520 6f72  == 2 -> reuse or
+000001a0: 6967 696e 616c 2077 6569 6768 7473 0a20  iginal weights. 
+000001b0: 2020 2020 2020 2069 6e5f 6368 616e 6e65         in_channe
+000001c0: 6c73 203e 2033 202d 3e20 6d61 6b65 2072  ls > 3 -> make r
+000001d0: 616e 646f 6d20 6b61 696d 696e 6720 6e6f  andom kaiming no
+000001e0: 726d 616c 2069 6e69 7469 616c 697a 6174  rmal initializat
+000001f0: 696f 6e0a 2020 2020 46e9 0100 0000 5429  ion.    F.....T)
+00000200: 01da 076b 6565 7064 696d e902 0000 004e  ...keepdim.....N
+00000210: 6700 0000 0000 00f8 3f29 10da 076d 6f64  g.......?)...mod
+00000220: 756c 6573 da0a 6973 696e 7374 616e 6365  ules..isinstance
+00000230: da02 6e6e da06 436f 6e76 3264 da0b 696e  ..nn..Conv2d..in
+00000240: 5f63 6861 6e6e 656c 73da 0677 6569 6768  _channels..weigh
+00000250: 74da 0664 6574 6163 68da 0373 756d da05  t..detach..sum..
+00000260: 746f 7263 68da 0654 656e 736f 72da 0c6f  torch..Tensor..o
+00000270: 7574 5f63 6861 6e6e 656c 73da 0667 726f  ut_channels..gro
+00000280: 7570 73da 0b6b 6572 6e65 6c5f 7369 7a65  ups..kernel_size
+00000290: da09 7061 7261 6d65 7465 72da 0950 6172  ..parameter..Par
+000002a0: 616d 6574 6572 da10 7265 7365 745f 7061  ameter..reset_pa
+000002b0: 7261 6d65 7465 7273 2905 da05 6d6f 6465  rameters)...mode
+000002c0: 6c72 0900 0000 da06 6d6f 6475 6c65 720a  lr......moduler.
+000002d0: 0000 00da 0572 6573 6574 a900 7218 0000  .....reset..r...
+000002e0: 00fa 4963 3a5c 5573 6572 735c 6d68 616e  ..Ic:\Users\mhan
+000002f0: 616e 5c44 6f77 6e6c 6f61 6473 5c48 616e  an\Downloads\Han
+00000300: 616e 5c6d 675c 7365 676d 656e 7461 7469  an\mg\segmentati
+00000310: 6f6e 5f6d 6f64 656c 735c 656e 636f 6465  on_models\encode
+00000320: 7273 5c5f 7574 696c 732e 7079 da10 7061  rs\_utils.py..pa
+00000330: 7463 685f 6669 7273 745f 636f 6e76 0500  tch_first_conv..
+00000340: 0000 7328 0000 0000 080c 010c 0106 0306  ..s(............
+00000350: 010a 0104 0208 0110 0108 011a 0204 0104  ................
+00000360: 0104 010a fe02 0304 fd06 060e 0104 0172  ...............r
+00000370: 1a00 0000 6302 0000 0000 0000 0000 0000  ....c...........
+00000380: 0005 0000 0004 0000 0043 0000 0073 6600  .........C...sf.
+00000390: 0000 7c00 a000 a100 4400 5d58 7d02 7401  ..|.....D.]X}.t.
+000003a0: 7c02 7402 6a03 8302 7208 6401 7c02 5f04  |.t.j...r.d.|._.
+000003b0: 7c01 7c01 6602 7c02 5f05 7c02 6a06 5c02  |.|.f.|._.|.j.\.
+000003c0: 7d03 7d04 7c03 6402 1a00 7c01 1400 7c03  }.}.|.d...|...|.
+000003d0: 6402 1a00 7c01 1400 6602 7c02 5f07 7408  d...|...f.|._.t.
+000003e0: 7c02 6403 8302 7208 7402 a009 a100 7c02  |.d...r.t.....|.
+000003f0: 5f0a 7108 6404 5300 2905 7a34 5061 7463  _.q.d.S.).z4Patc
+00000400: 6820 436f 6e76 3264 206d 6f64 756c 6573  h Conv2d modules
+00000410: 2072 6570 6c61 6369 6e67 2073 7472 6964   replacing strid
+00000420: 6573 2077 6974 6820 6469 6c61 7469 6f6e  es with dilation
+00000430: 2902 7202 0000 0072 0200 0000 7204 0000  ).r....r....r...
+00000440: 00da 0e73 7461 7469 635f 7061 6464 696e  ...static_paddin
+00000450: 674e 290b 7205 0000 0072 0600 0000 7207  gN).r....r....r.
+00000460: 0000 0072 0800 0000 da06 7374 7269 6465  ...r......stride
+00000470: da08 6469 6c61 7469 6f6e 7211 0000 00da  ..dilationr.....
+00000480: 0770 6164 6469 6e67 da07 6861 7361 7474  .padding..hasatt
+00000490: 72da 0849 6465 6e74 6974 7972 1b00 0000  r..Identityr....
+000004a0: 2905 7216 0000 00da 0d64 696c 6174 696f  ).r......dilatio
+000004b0: 6e5f 7261 7465 da03 6d6f 64da 026b 68da  n_rate..mod..kh.
+000004c0: 026b 7772 1800 0000 7218 0000 0072 1900  .kwr....r....r..
+000004d0: 0000 da1d 7265 706c 6163 655f 7374 7269  ....replace_stri
+000004e0: 6465 735f 7769 7468 5f64 696c 6174 696f  des_with_dilatio
+000004f0: 6e27 0000 0073 1000 0000 0002 0c01 0c01  n'...s..........
+00000500: 0601 0a01 0a01 1a03 0a01 7225 0000 0029  ..........r%...)
+00000510: 0572 0d00 0000 da08 746f 7263 682e 6e6e  .r......torch.nn
+00000520: 7207 0000 0072 1a00 0000 7225 0000 0072  r....r....r%...r
+00000530: 1800 0000 7218 0000 0072 1800 0000 7219  ....r....r....r.
+00000540: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000550: 0073 0600 0000 0801 0c03 0822            .s........."
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/densenet.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/densenet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/densenet.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/densenet.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/densenet.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/densenet.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/densenet.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/densenet.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:20 2023 UTC, .py size: 5317 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -107,196 +107,195 @@
 000006a0: 5769 7468 536b 6970 6302 0000 0000 0000  WithSkipc.......
 000006b0: 0000 0000 0002 0000 0002 0000 0003 0000  ................
 000006c0: 0073 1400 0000 7400 8300 a001 a100 0100  .s....t.........
 000006d0: 7c01 7c00 5f02 6400 5300 a901 4e29 03da  |.|._.d.S...N)..
 000006e0: 0573 7570 6572 da08 5f5f 696e 6974 5f5f  .super..__init__
 000006f0: da06 6d6f 6475 6c65 2902 da04 7365 6c66  ..module)...self
 00000700: 720a 0000 00a9 01da 095f 5f63 6c61 7373  r........__class
-00000710: 5f5f a900 fa58 433a 5c55 7365 7273 5c6d  __...XC:\Users\m
+00000710: 5f5f a900 fa4b 633a 5c55 7365 7273 5c6d  __...Kc:\Users\m
 00000720: 6861 6e61 6e5c 446f 776e 6c6f 6164 735c  hanan\Downloads\
-00000730: 4861 6e61 6e5c 4d61 6d6d 6f50 795c 6d61  Hanan\MammoPy\ma
-00000740: 6d6d 6f70 795c 7365 676d 656e 7461 7469  mmopy\segmentati
-00000750: 6f6e 5f6d 6f64 656c 735c 656e 636f 6465  on_models\encode
-00000760: 7273 5c64 656e 7365 6e65 742e 7079 7209  rs\densenet.pyr.
-00000770: 0000 0025 0000 0073 0400 0000 0001 0a01  ...%...s........
-00000780: 7a1b 5472 616e 7369 7469 6f6e 5769 7468  z.TransitionWith
-00000790: 536b 6970 2e5f 5f69 6e69 745f 5f63 0200  Skip.__init__c..
-000007a0: 0000 0000 0000 0000 0000 0400 0000 0400  ................
-000007b0: 0000 4300 0000 732c 0000 007c 006a 0044  ..C...s,...|.j.D
-000007c0: 005d 1c7d 027c 027c 0183 017d 0174 017c  .].}.|.|...}.t.|
-000007d0: 0274 026a 0383 0272 067c 017d 0371 067c  .t.j...r.|.}.q.|
-000007e0: 017c 0366 0253 0072 0700 0000 2904 720a  .|.f.S.r....).r.
-000007f0: 0000 00da 0a69 7369 6e73 7461 6e63 65da  .....isinstance.
-00000800: 026e 6eda 0452 654c 5529 0472 0b00 0000  .nn..ReLU).r....
-00000810: da01 7872 0a00 0000 da04 736b 6970 720e  ..xr......skipr.
-00000820: 0000 0072 0e00 0000 720f 0000 00da 0766  ...r....r......f
-00000830: 6f72 7761 7264 2900 0000 730a 0000 0000  orward)...s.....
-00000840: 010a 0108 010c 0106 017a 1a54 7261 6e73  .........z.Trans
-00000850: 6974 696f 6e57 6974 6853 6b69 702e 666f  itionWithSkip.fo
-00000860: 7277 6172 6429 06da 085f 5f6e 616d 655f  rward)...__name_
-00000870: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000880: 5f71 7561 6c6e 616d 655f 5f72 0900 0000  _qualname__r....
-00000890: 7215 0000 00da 0d5f 5f63 6c61 7373 6365  r......__classce
-000008a0: 6c6c 5f5f 720e 0000 0072 0e00 0000 720c  ll__r....r....r.
-000008b0: 0000 0072 0f00 0000 7206 0000 0023 0000  ...r....r....#..
-000008c0: 0073 0400 0000 0802 0c04 7206 0000 0063  .s........r....c
-000008d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000008e0: 0400 0000 0000 0000 7342 0000 0065 005a  ........sB...e.Z
-000008f0: 0164 005a 0264 0c87 0066 0164 0264 0384  .d.Z.d...f.d.d..
-00000900: 095a 0364 0464 0584 005a 0464 0664 0784  .Z.d.d...Z.d.d..
-00000910: 005a 0564 0864 0984 005a 0687 0066 0164  .Z.d.d...Z...f.d
-00000920: 0a64 0b84 085a 0787 0004 005a 0853 0029  .d...Z.....Z.S.)
-00000930: 0dda 0f44 656e 7365 4e65 7445 6e63 6f64  ...DenseNetEncod
-00000940: 6572 e905 0000 0063 0300 0000 0000 0000  er.....c........
-00000950: 0000 0000 0400 0000 0300 0000 0b00 0000  ................
-00000960: 7328 0000 0074 0083 006a 0166 007c 038e  s(...t...j.f.|..
-00000970: 0101 007c 017c 005f 027c 027c 005f 0364  ...|.|._.|.|._.d
-00000980: 017c 005f 047c 0060 0564 0053 0029 024e  .|._.|.`.d.S.).N
-00000990: e903 0000 0029 0672 0800 0000 7209 0000  .....).r....r...
-000009a0: 00da 0d5f 6f75 745f 6368 616e 6e65 6c73  ..._out_channels
-000009b0: da06 5f64 6570 7468 da0c 5f69 6e5f 6368  .._depth.._in_ch
-000009c0: 616e 6e65 6c73 da0a 636c 6173 7369 6669  annels..classifi
-000009d0: 6572 2904 720b 0000 00da 0c6f 7574 5f63  er).r......out_c
-000009e0: 6861 6e6e 656c 73da 0564 6570 7468 da06  hannels..depth..
-000009f0: 6b77 6172 6773 720c 0000 0072 0e00 0000  kwargsr....r....
-00000a00: 720f 0000 0072 0900 0000 3200 0000 730a  r....r....2...s.
-00000a10: 0000 0000 010e 0106 0106 0106 017a 1844  .............z.D
-00000a20: 656e 7365 4e65 7445 6e63 6f64 6572 2e5f  enseNetEncoder._
-00000a30: 5f69 6e69 745f 5f63 0300 0000 0000 0000  _init__c........
-00000a40: 0000 0000 0300 0000 0200 0000 4300 0000  ............C...
-00000a50: 730c 0000 0074 0064 0183 0182 0164 0053  s....t.d.....d.S
-00000a60: 0029 024e 7a58 4465 6e73 654e 6574 2065  .).NzXDenseNet e
-00000a70: 6e63 6f64 6572 7320 646f 206e 6f74 2073  ncoders do not s
-00000a80: 7570 706f 7274 2064 696c 6174 6564 206d  upport dilated m
-00000a90: 6f64 6520 6475 6520 746f 2070 6f6f 6c69  ode due to pooli
-00000aa0: 6e67 206f 7065 7261 7469 6f6e 2066 6f72  ng operation for
-00000ab0: 2064 6f77 6e73 616d 706c 696e 6721 2901   downsampling!).
-00000ac0: da0a 5661 6c75 6545 7272 6f72 2903 720b  ..ValueError).r.
-00000ad0: 0000 00da 0a73 7461 6765 5f6c 6973 74da  .....stage_list.
-00000ae0: 0d64 696c 6174 696f 6e5f 6c69 7374 720e  .dilation_listr.
-00000af0: 0000 0072 0e00 0000 720f 0000 00da 0c6d  ...r....r......m
-00000b00: 616b 655f 6469 6c61 7465 6439 0000 0073  ake_dilated9...s
-00000b10: 0200 0000 0001 7a1c 4465 6e73 654e 6574  ......z.DenseNet
-00000b20: 456e 636f 6465 722e 6d61 6b65 5f64 696c  Encoder.make_dil
-00000b30: 6174 6564 6301 0000 0000 0000 0000 0000  atedc...........
-00000b40: 0001 0000 0009 0000 0043 0000 0073 7c00  .........C...s|.
-00000b50: 0000 7400 a001 a100 7400 a002 7c00 6a03  ..t.....t...|.j.
-00000b60: 6a04 7c00 6a03 6a05 7c00 6a03 6a06 a103  j.|.j.j.|.j.j...
-00000b70: 7400 a002 7c00 6a03 6a07 7c00 6a03 6a08  t...|.j.j.|.j.j.
-00000b80: 7409 7c00 6a03 6a0a 8301 a103 7400 a002  t.|.j.j.....t...
-00000b90: 7c00 6a03 6a0b 7409 7c00 6a03 6a0c 8301  |.j.j.t.|.j.j...
-00000ba0: a102 7400 a002 7c00 6a03 6a0d 7409 7c00  ..t...|.j.j.t.|.
-00000bb0: 6a03 6a0e 8301 a102 7400 a002 7c00 6a03  j.j.....t...|.j.
-00000bc0: 6a0f 7c00 6a03 6a10 a102 6706 5300 7207  j.|.j.j...g.S.r.
-00000bd0: 0000 0029 1172 1100 0000 da08 4964 656e  ...).r......Iden
-00000be0: 7469 7479 da0a 5365 7175 656e 7469 616c  tity..Sequential
-00000bf0: da08 6665 6174 7572 6573 da05 636f 6e76  ..features..conv
-00000c00: 30da 056e 6f72 6d30 da05 7265 6c75 30da  0..norm0..relu0.
-00000c10: 0570 6f6f 6c30 5a0b 6465 6e73 6562 6c6f  .pool0Z.denseblo
-00000c20: 636b 3172 0600 0000 5a0b 7472 616e 7369  ck1r....Z.transi
-00000c30: 7469 6f6e 315a 0b64 656e 7365 626c 6f63  tion1Z.densebloc
-00000c40: 6b32 5a0b 7472 616e 7369 7469 6f6e 325a  k2Z.transition2Z
-00000c50: 0b64 656e 7365 626c 6f63 6b33 5a0b 7472  .denseblock3Z.tr
-00000c60: 616e 7369 7469 6f6e 335a 0b64 656e 7365  ansition3Z.dense
-00000c70: 626c 6f63 6b34 da05 6e6f 726d 3529 0172  block4..norm5).r
-00000c80: 0b00 0000 720e 0000 0072 0e00 0000 720f  ....r....r....r.
-00000c90: 0000 00da 0a67 6574 5f73 7461 6765 733d  .....get_stages=
-00000ca0: 0000 0073 1200 0000 0002 0601 1801 1001  ...s............
-00000cb0: 0aff 0202 1601 1601 12f9 7a1a 4465 6e73  ..........z.Dens
-00000cc0: 654e 6574 456e 636f 6465 722e 6765 745f  eNetEncoder.get_
-00000cd0: 7374 6167 6573 6302 0000 0000 0000 0000  stagesc.........
-00000ce0: 0000 0006 0000 0005 0000 0043 0000 0073  ...........C...s
-00000cf0: 5c00 0000 7c00 a000 a100 7d02 6700 7d03  \...|.....}.g.}.
-00000d00: 7401 7c00 6a02 6401 1700 8301 4400 5d3c  t.|.j.d.....D.]<
-00000d10: 7d04 7c02 7c04 1900 7c01 8301 7d01 7403  }.|.|...|...}.t.
-00000d20: 7c01 7404 7405 6602 8302 724c 7c01 5c02  |.t.t.f...rL|.\.
-00000d30: 7d01 7d05 7c03 a006 7c05 a101 0100 711a  }.}.|...|.....q.
-00000d40: 7c03 a006 7c01 a101 0100 711a 7c03 5300  |...|.....q.|.S.
-00000d50: 2902 4e72 0400 0000 2907 7230 0000 00da  ).Nr....).r0....
-00000d60: 0572 616e 6765 721e 0000 0072 1000 0000  .ranger....r....
-00000d70: da04 6c69 7374 da05 7475 706c 65da 0661  ..list..tuple..a
-00000d80: 7070 656e 6429 0672 0b00 0000 7213 0000  ppend).r....r...
-00000d90: 00da 0673 7461 6765 7372 2a00 0000 da01  ...stagesr*.....
-00000da0: 6972 1400 0000 720e 0000 0072 0e00 0000  ir....r....r....
-00000db0: 720f 0000 0072 1500 0000 4800 0000 7312  r....r....H...s.
-00000dc0: 0000 0000 0208 0204 0112 010c 010e 0108  ................
-00000dd0: 010c 020c 027a 1744 656e 7365 4e65 7445  .....z.DenseNetE
-00000de0: 6e63 6f64 6572 2e66 6f72 7761 7264 6302  ncoder.forwardc.
-00000df0: 0000 0000 0000 0000 0000 0006 0000 0005  ................
-00000e00: 0000 0003 0000 0073 7400 0000 7400 a001  .......st...t...
-00000e10: 6401 a101 7d02 7402 7c01 a003 a100 8301  d...}.t.|.......
-00000e20: 4400 5d38 7d03 7c02 a004 7c03 a101 7d04  D.]8}.|...|...}.
-00000e30: 7c04 7216 7c04 a005 6402 a101 7c04 a005  |.r.|...d...|...
-00000e40: 6403 a101 1700 7d05 7c01 7c03 1900 7c01  d.....}.|.|...|.
-00000e50: 7c05 3c00 7c01 7c03 3d00 7116 7c01 a006  |.<.|.|.=.q.|...
-00000e60: 6404 a101 0100 7c01 a006 6405 a101 0100  d.....|...d.....
-00000e70: 7407 8300 a008 7c01 a101 0100 6400 5300  t.....|.....d.S.
-00000e80: 2906 4e7a 5d5e 282e 2a64 656e 7365 6c61  ).Nz]^(.*densela
-00000e90: 7965 725c 642b 5c2e 283f 3a6e 6f72 6d7c  yer\d+\.(?:norm|
-00000ea0: 7265 6c75 7c63 6f6e 7629 295c 2e28 283f  relu|conv))\.((?
-00000eb0: 3a5b 3132 5d29 5c2e 283f 3a77 6569 6768  :[12])\.(?:weigh
-00000ec0: 747c 6269 6173 7c72 756e 6e69 6e67 5f6d  t|bias|running_m
-00000ed0: 6561 6e7c 7275 6e6e 696e 675f 7661 7229  ean|running_var)
-00000ee0: 2924 7204 0000 00e9 0200 0000 7a0f 636c  )$r.........z.cl
-00000ef0: 6173 7369 6669 6572 2e62 6961 737a 1163  assifier.biasz.c
-00000f00: 6c61 7373 6966 6965 722e 7765 6967 6874  lassifier.weight
-00000f10: 2909 da02 7265 da07 636f 6d70 696c 6572  )...re..compiler
-00000f20: 3200 0000 da04 6b65 7973 da05 6d61 7463  2.....keys..matc
-00000f30: 68da 0567 726f 7570 da03 706f 7072 0800  h..group..popr..
-00000f40: 0000 da0f 6c6f 6164 5f73 7461 7465 5f64  ....load_state_d
-00000f50: 6963 7429 0672 0b00 0000 da0a 7374 6174  ict).r......stat
-00000f60: 655f 6469 6374 da07 7061 7474 6572 6eda  e_dict..pattern.
-00000f70: 036b 6579 da03 7265 73da 076e 6577 5f6b  .key..res..new_k
-00000f80: 6579 720c 0000 0072 0e00 0000 720f 0000  eyr....r....r...
-00000f90: 0072 3e00 0000 5700 0000 7318 0000 0000  .r>...W...s.....
-00000fa0: 0104 0102 ff04 0310 010a 0104 0114 010c  ................
-00000fb0: 0108 030a 010a 027a 1f44 656e 7365 4e65  .......z.DenseNe
-00000fc0: 7445 6e63 6f64 6572 2e6c 6f61 645f 7374  tEncoder.load_st
-00000fd0: 6174 655f 6469 6374 2901 721b 0000 0029  ate_dict).r....)
-00000fe0: 0972 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
-00000ff0: 7209 0000 0072 2700 0000 7230 0000 0072  r....r'...r0...r
-00001000: 1500 0000 723e 0000 0072 1900 0000 720e  ....r>...r....r.
-00001010: 0000 0072 0e00 0000 720c 0000 0072 0f00  ...r....r....r..
-00001020: 0000 721a 0000 0031 0000 0073 0a00 0000  ..r....1...s....
-00001030: 0801 0e07 0804 080b 080f 721a 0000 00da  ..........r.....
-00001040: 0b64 656e 7365 6e65 7431 3231 2906 721c  .densenet121).r.
-00001050: 0000 00e9 4000 0000 e900 0100 00e9 0002  ....@...........
-00001060: 0000 e900 0400 0072 4800 0000 7245 0000  .......rH...rE..
-00001070: 00e9 2000 0000 2904 e906 0000 00e9 0c00  .. ...).........
-00001080: 0000 e918 0000 00e9 1000 0000 2904 7221  ............).r!
-00001090: 0000 00da 116e 756d 5f69 6e69 745f 6665  .....num_init_fe
-000010a0: 6174 7572 6573 da0b 6772 6f77 7468 5f72  atures..growth_r
-000010b0: 6174 65da 0c62 6c6f 636b 5f63 6f6e 6669  ate..block_confi
-000010c0: 6729 03da 0765 6e63 6f64 6572 7202 0000  g)...encoderr...
-000010d0: 00da 0670 6172 616d 73da 0b64 656e 7365  ...params..dense
-000010e0: 6e65 7431 3639 2906 721c 0000 0072 4500  net169).r....rE.
-000010f0: 0000 7246 0000 0072 4700 0000 6900 0500  ..rF...rG...i...
-00001100: 0069 8006 0000 2904 724a 0000 0072 4b00  .i....).rJ...rK.
-00001110: 0000 7249 0000 0072 4900 0000 da0b 6465  ..rI...rI.....de
-00001120: 6e73 656e 6574 3230 3129 0672 1c00 0000  nsenet201).r....
-00001130: 7245 0000 0072 4600 0000 7247 0000 0069  rE...rF...rG...i
-00001140: 0007 0000 6980 0700 0029 0472 4a00 0000  ....i....).rJ...
-00001150: 724b 0000 00e9 3000 0000 7249 0000 00da  rK....0...rI....
-00001160: 0b64 656e 7365 6e65 7431 3631 2906 721c  .densenet161).r.
-00001170: 0000 00e9 6000 0000 6980 0100 0069 0003  ....`...i....i..
-00001180: 0000 6940 0800 0069 a008 0000 7257 0000  ..i@...i....rW..
-00001190: 0072 5500 0000 2904 724a 0000 0072 4b00  .rU...).rJ...rK.
-000011a0: 0000 e924 0000 0072 4c00 0000 2904 7244  ...$...rL...).rD
-000011b0: 0000 0072 5300 0000 7254 0000 0072 5600  ...rS...rT...rV.
-000011c0: 0000 290e da07 5f5f 646f 635f 5f72 3800  ..)...__doc__r8.
-000011d0: 0000 da08 746f 7263 682e 6e6e 7211 0000  ....torch.nnr...
-000011e0: 005a 2a70 7265 7472 6169 6e65 646d 6f64  .Z*pretrainedmod
-000011f0: 656c 732e 6d6f 6465 6c73 2e74 6f72 6368  els.models.torch
-00001200: 7669 7369 6f6e 5f6d 6f64 656c 7372 0200  vision_modelsr..
-00001210: 0000 5a1b 746f 7263 6876 6973 696f 6e2e  ..Z.torchvision.
-00001220: 6d6f 6465 6c73 2e64 656e 7365 6e65 7472  models.densenetr
-00001230: 0300 0000 da05 5f62 6173 6572 0500 0000  ......_baser....
-00001240: da06 4d6f 6475 6c65 7206 0000 0072 1a00  ..Moduler....r..
-00001250: 0000 da11 6465 6e73 656e 6574 5f65 6e63  ....densenet_enc
-00001260: 6f64 6572 7372 0e00 0000 720e 0000 0072  odersr....r....r
-00001270: 0e00 0000 720f 0000 00da 083c 6d6f 6475  ....r......<modu
-00001280: 6c65 3e01 0000 0073 5000 0000 0419 0801  le>....sP.......
-00001290: 0c02 0c01 0c02 0c03 120e 123a 0201 0602  ...........:....
-000012a0: 0201 0201 0201 02fc 04fd 040b 0201 0602  ................
-000012b0: 0201 0201 0201 02fc 04fd 040b 0201 0602  ................
-000012c0: 0201 0201 0201 02fc 04fd 040b 0201 0602  ................
-000012d0: 0201 0201 0201 02fc 04fd 04e1            ............
+00000730: 4861 6e61 6e5c 6d67 5c73 6567 6d65 6e74  Hanan\mg\segment
+00000740: 6174 696f 6e5f 6d6f 6465 6c73 5c65 6e63  ation_models\enc
+00000750: 6f64 6572 735c 6465 6e73 656e 6574 2e70  oders\densenet.p
+00000760: 7972 0900 0000 2500 0000 7304 0000 0000  yr....%...s.....
+00000770: 010a 017a 1b54 7261 6e73 6974 696f 6e57  ...z.TransitionW
+00000780: 6974 6853 6b69 702e 5f5f 696e 6974 5f5f  ithSkip.__init__
+00000790: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
+000007a0: 0004 0000 0043 0000 0073 2c00 0000 7c00  .....C...s,...|.
+000007b0: 6a00 4400 5d1c 7d02 7c02 7c01 8301 7d01  j.D.].}.|.|...}.
+000007c0: 7401 7c02 7402 6a03 8302 7206 7c01 7d03  t.|.t.j...r.|.}.
+000007d0: 7106 7c01 7c03 6602 5300 7207 0000 0029  q.|.|.f.S.r....)
+000007e0: 0472 0a00 0000 da0a 6973 696e 7374 616e  .r......isinstan
+000007f0: 6365 da02 6e6e da04 5265 4c55 2904 720b  ce..nn..ReLU).r.
+00000800: 0000 00da 0178 720a 0000 00da 0473 6b69  .....xr......ski
+00000810: 7072 0e00 0000 720e 0000 0072 0f00 0000  pr....r....r....
+00000820: da07 666f 7277 6172 6429 0000 0073 0a00  ..forward)...s..
+00000830: 0000 0001 0a01 0801 0c01 0601 7a1a 5472  ............z.Tr
+00000840: 616e 7369 7469 6f6e 5769 7468 536b 6970  ansitionWithSkip
+00000850: 2e66 6f72 7761 7264 2906 da08 5f5f 6e61  .forward)...__na
+00000860: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000870: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7209  ..__qualname__r.
+00000880: 0000 0072 1500 0000 da0d 5f5f 636c 6173  ...r......__clas
+00000890: 7363 656c 6c5f 5f72 0e00 0000 720e 0000  scell__r....r...
+000008a0: 0072 0c00 0000 720f 0000 0072 0600 0000  .r....r....r....
+000008b0: 2300 0000 7304 0000 0008 020c 0472 0600  #...s........r..
+000008c0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000008d0: 0000 0004 0000 0000 0000 0073 4200 0000  ...........sB...
+000008e0: 6500 5a01 6400 5a02 640c 8700 6601 6402  e.Z.d.Z.d...f.d.
+000008f0: 6403 8409 5a03 6404 6405 8400 5a04 6406  d...Z.d.d...Z.d.
+00000900: 6407 8400 5a05 6408 6409 8400 5a06 8700  d...Z.d.d...Z...
+00000910: 6601 640a 640b 8408 5a07 8700 0400 5a08  f.d.d...Z.....Z.
+00000920: 5300 290d da0f 4465 6e73 654e 6574 456e  S.)...DenseNetEn
+00000930: 636f 6465 72e9 0500 0000 6303 0000 0000  coder.....c.....
+00000940: 0000 0000 0000 0004 0000 0003 0000 000b  ................
+00000950: 0000 0073 2800 0000 7400 8300 6a01 6600  ...s(...t...j.f.
+00000960: 7c03 8e01 0100 7c01 7c00 5f02 7c02 7c00  |.....|.|._.|.|.
+00000970: 5f03 6401 7c00 5f04 7c00 6005 6400 5300  _.d.|._.|.`.d.S.
+00000980: 2902 4ee9 0300 0000 2906 7208 0000 0072  ).N.....).r....r
+00000990: 0900 0000 da0d 5f6f 7574 5f63 6861 6e6e  ......_out_chann
+000009a0: 656c 73da 065f 6465 7074 68da 0c5f 696e  els.._depth.._in
+000009b0: 5f63 6861 6e6e 656c 73da 0a63 6c61 7373  _channels..class
+000009c0: 6966 6965 7229 0472 0b00 0000 da0c 6f75  ifier).r......ou
+000009d0: 745f 6368 616e 6e65 6c73 da05 6465 7074  t_channels..dept
+000009e0: 68da 066b 7761 7267 7372 0c00 0000 720e  h..kwargsr....r.
+000009f0: 0000 0072 0f00 0000 7209 0000 0032 0000  ...r....r....2..
+00000a00: 0073 0a00 0000 0001 0e01 0601 0601 0601  .s..............
+00000a10: 7a18 4465 6e73 654e 6574 456e 636f 6465  z.DenseNetEncode
+00000a20: 722e 5f5f 696e 6974 5f5f 6303 0000 0000  r.__init__c.....
+00000a30: 0000 0000 0000 0003 0000 0002 0000 0043  ...............C
+00000a40: 0000 0073 0c00 0000 7400 6401 8301 8201  ...s....t.d.....
+00000a50: 6400 5300 2902 4e7a 5844 656e 7365 4e65  d.S.).NzXDenseNe
+00000a60: 7420 656e 636f 6465 7273 2064 6f20 6e6f  t encoders do no
+00000a70: 7420 7375 7070 6f72 7420 6469 6c61 7465  t support dilate
+00000a80: 6420 6d6f 6465 2064 7565 2074 6f20 706f  d mode due to po
+00000a90: 6f6c 696e 6720 6f70 6572 6174 696f 6e20  oling operation 
+00000aa0: 666f 7220 646f 776e 7361 6d70 6c69 6e67  for downsampling
+00000ab0: 2129 01da 0a56 616c 7565 4572 726f 7229  !)...ValueError)
+00000ac0: 0372 0b00 0000 da0a 7374 6167 655f 6c69  .r......stage_li
+00000ad0: 7374 da0d 6469 6c61 7469 6f6e 5f6c 6973  st..dilation_lis
+00000ae0: 7472 0e00 0000 720e 0000 0072 0f00 0000  tr....r....r....
+00000af0: da0c 6d61 6b65 5f64 696c 6174 6564 3900  ..make_dilated9.
+00000b00: 0000 7302 0000 0000 017a 1c44 656e 7365  ..s......z.Dense
+00000b10: 4e65 7445 6e63 6f64 6572 2e6d 616b 655f  NetEncoder.make_
+00000b20: 6469 6c61 7465 6463 0100 0000 0000 0000  dilatedc........
+00000b30: 0000 0000 0100 0000 0900 0000 4300 0000  ............C...
+00000b40: 737c 0000 0074 00a0 01a1 0074 00a0 027c  s|...t.....t...|
+00000b50: 006a 036a 047c 006a 036a 057c 006a 036a  .j.j.|.j.j.|.j.j
+00000b60: 06a1 0374 00a0 027c 006a 036a 077c 006a  ...t...|.j.j.|.j
+00000b70: 036a 0874 097c 006a 036a 0a83 01a1 0374  .j.t.|.j.j.....t
+00000b80: 00a0 027c 006a 036a 0b74 097c 006a 036a  ...|.j.j.t.|.j.j
+00000b90: 0c83 01a1 0274 00a0 027c 006a 036a 0d74  .....t...|.j.j.t
+00000ba0: 097c 006a 036a 0e83 01a1 0274 00a0 027c  .|.j.j.....t...|
+00000bb0: 006a 036a 0f7c 006a 036a 10a1 0267 0653  .j.j.|.j.j...g.S
+00000bc0: 0072 0700 0000 2911 7211 0000 00da 0849  .r....).r......I
+00000bd0: 6465 6e74 6974 79da 0a53 6571 7565 6e74  dentity..Sequent
+00000be0: 6961 6cda 0866 6561 7475 7265 73da 0563  ial..features..c
+00000bf0: 6f6e 7630 da05 6e6f 726d 30da 0572 656c  onv0..norm0..rel
+00000c00: 7530 da05 706f 6f6c 305a 0b64 656e 7365  u0..pool0Z.dense
+00000c10: 626c 6f63 6b31 7206 0000 005a 0b74 7261  block1r....Z.tra
+00000c20: 6e73 6974 696f 6e31 5a0b 6465 6e73 6562  nsition1Z.denseb
+00000c30: 6c6f 636b 325a 0b74 7261 6e73 6974 696f  lock2Z.transitio
+00000c40: 6e32 5a0b 6465 6e73 6562 6c6f 636b 335a  n2Z.denseblock3Z
+00000c50: 0b74 7261 6e73 6974 696f 6e33 5a0b 6465  .transition3Z.de
+00000c60: 6e73 6562 6c6f 636b 34da 056e 6f72 6d35  nseblock4..norm5
+00000c70: 2901 720b 0000 0072 0e00 0000 720e 0000  ).r....r....r...
+00000c80: 0072 0f00 0000 da0a 6765 745f 7374 6167  .r......get_stag
+00000c90: 6573 3d00 0000 7312 0000 0000 0206 0118  es=...s.........
+00000ca0: 0110 010a ff02 0216 0116 0112 f97a 1a44  .............z.D
+00000cb0: 656e 7365 4e65 7445 6e63 6f64 6572 2e67  enseNetEncoder.g
+00000cc0: 6574 5f73 7461 6765 7363 0200 0000 0000  et_stagesc......
+00000cd0: 0000 0000 0000 0600 0000 0500 0000 4300  ..............C.
+00000ce0: 0000 735c 0000 007c 00a0 00a1 007d 0267  ..s\...|.....}.g
+00000cf0: 007d 0374 017c 006a 0264 0117 0083 0144  .}.t.|.j.d.....D
+00000d00: 005d 3c7d 047c 027c 0419 007c 0183 017d  .]<}.|.|...|...}
+00000d10: 0174 037c 0174 0474 0566 0283 0272 4c7c  .t.|.t.t.f...rL|
+00000d20: 015c 027d 017d 057c 03a0 067c 05a1 0101  .\.}.}.|...|....
+00000d30: 0071 1a7c 03a0 067c 01a1 0101 0071 1a7c  .q.|...|.....q.|
+00000d40: 0353 0029 024e 7204 0000 0029 0772 3000  .S.).Nr....).r0.
+00000d50: 0000 da05 7261 6e67 6572 1e00 0000 7210  ....ranger....r.
+00000d60: 0000 00da 046c 6973 74da 0574 7570 6c65  .....list..tuple
+00000d70: da06 6170 7065 6e64 2906 720b 0000 0072  ..append).r....r
+00000d80: 1300 0000 da06 7374 6167 6573 722a 0000  ......stagesr*..
+00000d90: 00da 0169 7214 0000 0072 0e00 0000 720e  ...ir....r....r.
+00000da0: 0000 0072 0f00 0000 7215 0000 0048 0000  ...r....r....H..
+00000db0: 0073 1200 0000 0002 0802 0401 1201 0c01  .s..............
+00000dc0: 0e01 0801 0c02 0c02 7a17 4465 6e73 654e  ........z.DenseN
+00000dd0: 6574 456e 636f 6465 722e 666f 7277 6172  etEncoder.forwar
+00000de0: 6463 0200 0000 0000 0000 0000 0000 0600  dc..............
+00000df0: 0000 0500 0000 0300 0000 7374 0000 0074  ..........st...t
+00000e00: 00a0 0164 01a1 017d 0274 027c 01a0 03a1  ...d...}.t.|....
+00000e10: 0083 0144 005d 387d 037c 02a0 047c 03a1  ...D.]8}.|...|..
+00000e20: 017d 047c 0472 167c 04a0 0564 02a1 017c  .}.|.r.|...d...|
+00000e30: 04a0 0564 03a1 0117 007d 057c 017c 0319  ...d.....}.|.|..
+00000e40: 007c 017c 053c 007c 017c 033d 0071 167c  .|.|.<.|.|.=.q.|
+00000e50: 01a0 0664 04a1 0101 007c 01a0 0664 05a1  ...d.....|...d..
+00000e60: 0101 0074 0783 00a0 087c 01a1 0101 0064  ...t.....|.....d
+00000e70: 0053 0029 064e 7a5d 5e28 2e2a 6465 6e73  .S.).Nz]^(.*dens
+00000e80: 656c 6179 6572 5c64 2b5c 2e28 3f3a 6e6f  elayer\d+\.(?:no
+00000e90: 726d 7c72 656c 757c 636f 6e76 2929 5c2e  rm|relu|conv))\.
+00000ea0: 2828 3f3a 5b31 325d 295c 2e28 3f3a 7765  ((?:[12])\.(?:we
+00000eb0: 6967 6874 7c62 6961 737c 7275 6e6e 696e  ight|bias|runnin
+00000ec0: 675f 6d65 616e 7c72 756e 6e69 6e67 5f76  g_mean|running_v
+00000ed0: 6172 2929 2472 0400 0000 e902 0000 007a  ar))$r.........z
+00000ee0: 0f63 6c61 7373 6966 6965 722e 6269 6173  .classifier.bias
+00000ef0: 7a11 636c 6173 7369 6669 6572 2e77 6569  z.classifier.wei
+00000f00: 6768 7429 09da 0272 65da 0763 6f6d 7069  ght)...re..compi
+00000f10: 6c65 7232 0000 00da 046b 6579 73da 056d  ler2.....keys..m
+00000f20: 6174 6368 da05 6772 6f75 70da 0370 6f70  atch..group..pop
+00000f30: 7208 0000 00da 0f6c 6f61 645f 7374 6174  r......load_stat
+00000f40: 655f 6469 6374 2906 720b 0000 00da 0a73  e_dict).r......s
+00000f50: 7461 7465 5f64 6963 74da 0770 6174 7465  tate_dict..patte
+00000f60: 726e da03 6b65 79da 0372 6573 da07 6e65  rn..key..res..ne
+00000f70: 775f 6b65 7972 0c00 0000 720e 0000 0072  w_keyr....r....r
+00000f80: 0f00 0000 723e 0000 0057 0000 0073 1800  ....r>...W...s..
+00000f90: 0000 0001 0401 02ff 0403 1001 0a01 0401  ................
+00000fa0: 1401 0c01 0803 0a01 0a02 7a1f 4465 6e73  ..........z.Dens
+00000fb0: 654e 6574 456e 636f 6465 722e 6c6f 6164  eNetEncoder.load
+00000fc0: 5f73 7461 7465 5f64 6963 7429 0172 1b00  _state_dict).r..
+00000fd0: 0000 2909 7216 0000 0072 1700 0000 7218  ..).r....r....r.
+00000fe0: 0000 0072 0900 0000 7227 0000 0072 3000  ...r....r'...r0.
+00000ff0: 0000 7215 0000 0072 3e00 0000 7219 0000  ..r....r>...r...
+00001000: 0072 0e00 0000 720e 0000 0072 0c00 0000  .r....r....r....
+00001010: 720f 0000 0072 1a00 0000 3100 0000 730a  r....r....1...s.
+00001020: 0000 0008 010e 0708 0408 0b08 0f72 1a00  .............r..
+00001030: 0000 da0b 6465 6e73 656e 6574 3132 3129  ....densenet121)
+00001040: 0672 1c00 0000 e940 0000 00e9 0001 0000  .r.....@........
+00001050: e900 0200 00e9 0004 0000 7248 0000 0072  ..........rH...r
+00001060: 4500 0000 e920 0000 0029 04e9 0600 0000  E.... ...)......
+00001070: e90c 0000 00e9 1800 0000 e910 0000 0029  ...............)
+00001080: 0472 2100 0000 da11 6e75 6d5f 696e 6974  .r!.....num_init
+00001090: 5f66 6561 7475 7265 73da 0b67 726f 7774  _features..growt
+000010a0: 685f 7261 7465 da0c 626c 6f63 6b5f 636f  h_rate..block_co
+000010b0: 6e66 6967 2903 da07 656e 636f 6465 7272  nfig)...encoderr
+000010c0: 0200 0000 da06 7061 7261 6d73 da0b 6465  ......params..de
+000010d0: 6e73 656e 6574 3136 3929 0672 1c00 0000  nsenet169).r....
+000010e0: 7245 0000 0072 4600 0000 7247 0000 0069  rE...rF...rG...i
+000010f0: 0005 0000 6980 0600 0029 0472 4a00 0000  ....i....).rJ...
+00001100: 724b 0000 0072 4900 0000 7249 0000 00da  rK...rI...rI....
+00001110: 0b64 656e 7365 6e65 7432 3031 2906 721c  .densenet201).r.
+00001120: 0000 0072 4500 0000 7246 0000 0072 4700  ...rE...rF...rG.
+00001130: 0000 6900 0700 0069 8007 0000 2904 724a  ..i....i....).rJ
+00001140: 0000 0072 4b00 0000 e930 0000 0072 4900  ...rK....0...rI.
+00001150: 0000 da0b 6465 6e73 656e 6574 3136 3129  ....densenet161)
+00001160: 0672 1c00 0000 e960 0000 0069 8001 0000  .r.....`...i....
+00001170: 6900 0300 0069 4008 0000 69a0 0800 0072  i....i@...i....r
+00001180: 5700 0000 7255 0000 0029 0472 4a00 0000  W...rU...).rJ...
+00001190: 724b 0000 00e9 2400 0000 724c 0000 0029  rK....$...rL...)
+000011a0: 0472 4400 0000 7253 0000 0072 5400 0000  .rD...rS...rT...
+000011b0: 7256 0000 0029 0eda 075f 5f64 6f63 5f5f  rV...)...__doc__
+000011c0: 7238 0000 00da 0874 6f72 6368 2e6e 6e72  r8.....torch.nnr
+000011d0: 1100 0000 5a2a 7072 6574 7261 696e 6564  ....Z*pretrained
+000011e0: 6d6f 6465 6c73 2e6d 6f64 656c 732e 746f  models.models.to
+000011f0: 7263 6876 6973 696f 6e5f 6d6f 6465 6c73  rchvision_models
+00001200: 7202 0000 005a 1b74 6f72 6368 7669 7369  r....Z.torchvisi
+00001210: 6f6e 2e6d 6f64 656c 732e 6465 6e73 656e  on.models.densen
+00001220: 6574 7203 0000 00da 055f 6261 7365 7205  etr......_baser.
+00001230: 0000 00da 064d 6f64 756c 6572 0600 0000  .....Moduler....
+00001240: 721a 0000 00da 1164 656e 7365 6e65 745f  r......densenet_
+00001250: 656e 636f 6465 7273 720e 0000 0072 0e00  encodersr....r..
+00001260: 0000 720e 0000 0072 0f00 0000 da08 3c6d  ..r....r......<m
+00001270: 6f64 756c 653e 0100 0000 7350 0000 0004  odule>....sP....
+00001280: 1908 010c 020c 010c 020c 0312 0e12 3a02  ..............:.
+00001290: 0106 0202 0102 0102 0102 fc04 fd04 0b02  ................
+000012a0: 0106 0202 0102 0102 0102 fc04 fd04 0b02  ................
+000012b0: 0106 0202 0102 0102 0102 fc04 fd04 0b02  ................
+000012c0: 0106 0202 0102 0102 0102 fc04 fd04 e1    ...............
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/densenet.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/densenet.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/dpn.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/dpn.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/dpn.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/dpn.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/dpn.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/dpn.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/dpn.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/dpn.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:20 2023 UTC, .py size: 6009 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -123,154 +123,153 @@
 000007a0: 6465 7074 68da 0d5f 6f75 745f 6368 616e  depth.._out_chan
 000007b0: 6e65 6c73 da0c 5f69 6e5f 6368 616e 6e65  nels.._in_channe
 000007c0: 6c73 da0b 6c61 7374 5f6c 696e 6561 7229  ls..last_linear)
 000007d0: 05da 0473 656c 66da 0a73 7461 6765 5f69  ...self..stage_i
 000007e0: 6478 73da 0c6f 7574 5f63 6861 6e6e 656c  dxs..out_channel
 000007f0: 73da 0564 6570 7468 da06 6b77 6172 6773  s..depth..kwargs
 00000800: a901 da09 5f5f 636c 6173 735f 5fa9 00fa  ....__class__...
-00000810: 5343 3a5c 5573 6572 735c 6d68 616e 616e  SC:\Users\mhanan
+00000810: 4663 3a5c 5573 6572 735c 6d68 616e 616e  Fc:\Users\mhanan
 00000820: 5c44 6f77 6e6c 6f61 6473 5c48 616e 616e  \Downloads\Hanan
-00000830: 5c4d 616d 6d6f 5079 5c6d 616d 6d6f 7079  \MammoPy\mammopy
-00000840: 5c73 6567 6d65 6e74 6174 696f 6e5f 6d6f  \segmentation_mo
-00000850: 6465 6c73 5c65 6e63 6f64 6572 735c 6470  dels\encoders\dp
-00000860: 6e2e 7079 720a 0000 0025 0000 0073 0c00  n.pyr....%...s..
-00000870: 0000 0001 0e01 0601 0601 0601 0602 7a14  ..............z.
-00000880: 4450 4e45 6e63 6f72 6465 722e 5f5f 696e  DPNEncorder.__in
-00000890: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
-000008a0: 0001 0000 0009 0000 0043 0000 0073 9800  .........C...s..
-000008b0: 0000 7400 a001 a100 7400 a002 7c00 6a03  ..t.....t...|.j.
-000008c0: 6401 1900 6a04 7c00 6a03 6401 1900 6a05  d...j.|.j.d...j.
-000008d0: 7c00 6a03 6401 1900 6a06 a103 7400 a002  |.j.d...j...t...
-000008e0: 7c00 6a03 6401 1900 6a07 7c00 6a03 6402  |.j.d...j.|.j.d.
-000008f0: 7c00 6a08 6401 1900 8502 1900 a102 7c00  |.j.d.........|.
-00000900: 6a03 7c00 6a08 6401 1900 7c00 6a08 6402  j.|.j.d...|.j.d.
-00000910: 1900 8502 1900 7c00 6a03 7c00 6a08 6402  ......|.j.|.j.d.
-00000920: 1900 7c00 6a08 6403 1900 8502 1900 7c00  ..|.j.d.......|.
-00000930: 6a03 7c00 6a08 6403 1900 7c00 6a08 6404  j.|.j.d...|.j.d.
-00000940: 1900 8502 1900 6706 5300 2905 4e72 0100  ......g.S.).Nr..
-00000950: 0000 7204 0000 00e9 0200 0000 7208 0000  ..r.........r...
-00000960: 0029 09da 026e 6eda 0849 6465 6e74 6974  .)...nn..Identit
-00000970: 79da 0a53 6571 7565 6e74 6961 6cda 0866  y..Sequential..f
-00000980: 6561 7475 7265 73da 0463 6f6e 76da 0262  eatures..conv..b
-00000990: 6eda 0361 6374 da04 706f 6f6c 720b 0000  n..act..poolr...
-000009a0: 0029 0172 1000 0000 7217 0000 0072 1700  .).r....r....r..
-000009b0: 0000 7218 0000 00da 0a67 6574 5f73 7461  ..r......get_sta
-000009c0: 6765 732e 0000 0073 0e00 0000 0002 0601  ges....s........
-000009d0: 2401 2201 1801 1801 18fa 7a16 4450 4e45  $.".......z.DPNE
-000009e0: 6e63 6f72 6465 722e 6765 745f 7374 6167  ncorder.get_stag
-000009f0: 6573 6302 0000 0000 0000 0000 0000 0005  esc.............
-00000a00: 0000 0008 0000 0043 0000 0073 6800 0000  .......C...sh...
-00000a10: 7c00 a000 a100 7d02 6700 7d03 7401 7c00  |.....}.g.}.t.|.
-00000a20: 6a02 6401 1700 8301 4400 5d48 7d04 7c02  j.d.....D.]H}.|.
-00000a30: 7c04 1900 7c01 8301 7d01 7403 7c01 7404  |...|...}.t.|.t.
-00000a40: 7405 6602 8302 7258 7c03 a006 7407 6a08  t.f...rX|...t.j.
-00000a50: 7409 6a0a 7c01 6401 6402 8d02 6403 6404  t.j.|.d.d...d.d.
-00000a60: 8d02 a101 0100 711a 7c03 a006 7c01 a101  ......q.|...|...
-00000a70: 0100 711a 7c03 5300 2905 4e72 0400 0000  ..q.|.S.).Nr....
-00000a80: 2901 da03 6469 6d54 2901 da07 696e 706c  )...dimT)...inpl
-00000a90: 6163 6529 0b72 2200 0000 da05 7261 6e67  ace).r".....rang
-00000aa0: 6572 0c00 0000 da0a 6973 696e 7374 616e  er......isinstan
-00000ab0: 6365 da04 6c69 7374 da05 7475 706c 65da  ce..list..tuple.
-00000ac0: 0661 7070 656e 64da 0146 da04 7265 6c75  .append..F..relu
-00000ad0: da05 746f 7263 68da 0363 6174 2905 7210  ..torch..cat).r.
-00000ae0: 0000 00da 0178 da06 7374 6167 6573 721d  .....x..stagesr.
-00000af0: 0000 00da 0169 7217 0000 0072 1700 0000  .....ir....r....
-00000b00: 7218 0000 00da 0766 6f72 7761 7264 3800  r......forward8.
-00000b10: 0000 7310 0000 0000 0208 0204 0112 010c  ..s.............
-00000b20: 010e 0120 020c 027a 1344 504e 456e 636f  ... ...z.DPNEnco
-00000b30: 7264 6572 2e66 6f72 7761 7264 6302 0000  rder.forwardc...
-00000b40: 0000 0000 0000 0000 0003 0000 0003 0000  ................
-00000b50: 000b 0000 0073 2800 0000 7c01 a000 6401  .....s(...|...d.
-00000b60: a101 0100 7c01 a000 6402 a101 0100 7401  ....|...d.....t.
-00000b70: 8300 6a02 7c01 6601 7c02 8e01 0100 6400  ..j.|.f.|.....d.
-00000b80: 5300 2903 4e7a 106c 6173 745f 6c69 6e65  S.).Nz.last_line
-00000b90: 6172 2e62 6961 737a 126c 6173 745f 6c69  ar.biasz.last_li
-00000ba0: 6e65 6172 2e77 6569 6768 7429 03da 0370  near.weight)...p
-00000bb0: 6f70 7209 0000 00da 0f6c 6f61 645f 7374  opr......load_st
-00000bc0: 6174 655f 6469 6374 2903 7210 0000 00da  ate_dict).r.....
-00000bd0: 0a73 7461 7465 5f64 6963 7472 1400 0000  .state_dictr....
-00000be0: 7215 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
-00000bf0: 3300 0000 4600 0000 7306 0000 0000 010a  3...F...s.......
-00000c00: 010a 017a 1b44 504e 456e 636f 7264 6572  ...z.DPNEncorder
-00000c10: 2e6c 6f61 645f 7374 6174 655f 6469 6374  .load_state_dict
-00000c20: 2901 7207 0000 0029 08da 085f 5f6e 616d  ).r....)...__nam
-00000c30: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000c40: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0a00  .__qualname__r..
-00000c50: 0000 7222 0000 0072 3100 0000 7233 0000  ..r"...r1...r3..
-00000c60: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
-00000c70: 7217 0000 0072 1700 0000 7215 0000 0072  r....r....r....r
-00000c80: 1800 0000 7206 0000 0024 0000 0073 0800  ....r....$...s..
-00000c90: 0000 0801 0e09 080a 080e 7206 0000 00da  ..........r.....
-00000ca0: 0564 706e 3638 2904 e904 0000 00e9 0800  .dpn68).........
-00000cb0: 0000 e914 0000 00e9 1800 0000 2906 7208  ............).r.
-00000cc0: 0000 00e9 0a00 0000 e990 0000 0069 4001  .............i@.
-00000cd0: 0000 e9c0 0200 00e9 4003 0000 e920 0000  ........@.... ..
-00000ce0: 0029 04e9 1000 0000 7242 0000 0072 4200  .)......rB...rB.
-00000cf0: 0000 e940 0000 00e9 8000 0000 2904 7208  ...@........).r.
-00000d00: 0000 0072 3a00 0000 e90c 0000 0072 0800  ...r:........r..
-00000d10: 0000 69e8 0300 0072 3e00 0000 5429 0a72  ..i....r>...T).r
-00000d20: 1100 0000 7212 0000 00da 0667 726f 7570  ....r......group
-00000d30: 73da 0769 6e63 5f73 6563 da03 6b5f 72da  s..inc_sec..k_r.
-00000d40: 056b 5f73 6563 da0b 6e75 6d5f 636c 6173  .k_sec..num_clas
-00000d50: 7365 73da 116e 756d 5f69 6e69 745f 6665  ses..num_init_fe
-00000d60: 6174 7572 6573 da05 736d 616c 6cda 0e74  atures..small..t
-00000d70: 6573 745f 7469 6d65 5f70 6f6f 6c29 03da  est_time_pool)..
-00000d80: 0765 6e63 6f64 6572 7203 0000 00da 0670  .encoderr......p
-00000d90: 6172 616d 73da 0664 706e 3638 6229 0b72  arams..dpn68b).r
-00000da0: 1100 0000 7212 0000 00da 0162 7247 0000  ....r......brG..
-00000db0: 0072 4800 0000 7249 0000 0072 4a00 0000  .rH...rI...rJ...
-00000dc0: 724b 0000 0072 4c00 0000 724d 0000 0072  rK...rL...rM...r
-00000dd0: 4e00 0000 da05 6470 6e39 3229 0472 3a00  N.....dpn92).r:.
-00000de0: 0000 723b 0000 00e9 1c00 0000 7242 0000  ..r;........rB..
-00000df0: 0029 0672 0800 0000 7244 0000 00e9 5001  .).r....rD....P.
-00000e00: 0000 7240 0000 0069 1006 0000 e980 0a00  ..r@...i........
-00000e10: 0029 0472 4300 0000 7242 0000 0072 3d00  .).rC...rB...r=.
-00000e20: 0000 7245 0000 00e9 6000 0000 2904 7208  ..rE....`...).r.
-00000e30: 0000 0072 3a00 0000 723c 0000 0072 0800  ...r:...r<...r..
-00000e40: 0000 7244 0000 0029 0972 1100 0000 7212  ..rD...).r....r.
-00000e50: 0000 0072 4700 0000 7248 0000 0072 4900  ...rG...rH...rI.
-00000e60: 0000 724a 0000 0072 4b00 0000 724c 0000  ..rJ...rK...rL..
-00000e70: 0072 4e00 0000 da05 6470 6e39 3829 0472  .rN.....dpn98).r
-00000e80: 3a00 0000 723e 0000 00e9 1e00 0000 e922  :...r>........."
-00000e90: 0000 0029 0672 0800 0000 7257 0000 0072  ...).r....rW...r
-00000ea0: 5500 0000 6900 0300 0069 c006 0000 7256  U...i....i....rV
-00000eb0: 0000 00e9 2800 0000 2904 7243 0000 0072  ....(...).rC...r
-00000ec0: 4200 0000 7242 0000 0072 4500 0000 e9a0  B...rB...rE.....
-00000ed0: 0000 0029 0472 0800 0000 e906 0000 0072  ...).r.........r
-00000ee0: 3c00 0000 7208 0000 00da 0664 706e 3130  <...r......dpn10
-00000ef0: 3729 0472 0700 0000 e90d 0000 00e9 2100  7).r..........!.
-00000f00: 0000 e925 0000 0029 0672 0800 0000 7245  ...%...).r....rE
-00000f10: 0000 0069 7801 0000 6980 0400 0069 8009  ...ix...i....i..
-00000f20: 0000 7256 0000 00e9 3200 0000 2904 723c  ..rV....2...).r<
-00000f30: 0000 0072 4400 0000 7244 0000 0072 4500  ...rD...rD...rE.
-00000f40: 0000 e9c8 0000 0029 0472 3a00 0000 723b  .......).r:...r;
-00000f50: 0000 0072 3c00 0000 7208 0000 00da 0664  ...r<...r......d
-00000f60: 706e 3133 3129 0472 0700 0000 725f 0000  pn131).r....r_..
-00000f70: 00e9 2900 0000 e92d 0000 0029 0672 0800  ..)....-...).r..
-00000f80: 0000 7245 0000 0069 6001 0000 7241 0000  ..rE...i`...rA..
-00000f90: 0069 c007 0000 7256 0000 0029 0472 3a00  .i....rV...).r:.
-00000fa0: 0000 723b 0000 0072 5400 0000 7208 0000  ..r;...rT...r...
-00000fb0: 0029 0672 3900 0000 7251 0000 0072 5300  .).r9...rQ...rS.
-00000fc0: 0000 7258 0000 0072 5e00 0000 7264 0000  ..rX...r^...rd..
-00000fd0: 0029 0eda 075f 5f64 6f63 5f5f 722c 0000  .)...__doc__r,..
-00000fe0: 00da 0874 6f72 6368 2e6e 6e72 1a00 0000  ...torch.nnr....
-00000ff0: 5a13 746f 7263 682e 6e6e 2e66 756e 6374  Z.torch.nn.funct
-00001000: 696f 6e61 6cda 0a66 756e 6374 696f 6e61  ional..functiona
-00001010: 6c72 2a00 0000 5a1b 7072 6574 7261 696e  lr*...Z.pretrain
-00001020: 6564 6d6f 6465 6c73 2e6d 6f64 656c 732e  edmodels.models.
-00001030: 6470 6e72 0200 0000 7203 0000 00da 055f  dpnr....r......_
-00001040: 6261 7365 7205 0000 0072 0600 0000 da0c  baser....r......
-00001050: 6470 6e5f 656e 636f 6465 7273 7217 0000  dpn_encodersr...
-00001060: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
-00001070: da08 3c6d 6f64 756c 653e 0100 0000 73b2  ..<module>....s.
-00001080: 0000 0004 1908 010c 0112 020c 010c 020c  ................
-00001090: 0312 2a02 0106 0202 0102 0102 0102 0102  ..*.............
-000010a0: 0102 0102 0102 0102 0102 f604 fd04 1102  ................
-000010b0: 0106 0202 0102 0102 0102 0102 0102 0102  ................
-000010c0: 0102 0102 0102 0102 f504 fd04 1202 0106  ................
-000010d0: 0202 0102 0102 0102 0102 0102 0102 0102  ................
-000010e0: 0102 f704 fd04 1002 0106 0202 0102 0102  ................
-000010f0: 0102 0102 0102 0102 0102 0102 f704 fd04  ................
-00001100: 1002 0106 0202 0102 0102 0102 0102 0102  ................
-00001110: 0102 0102 0102 f704 fd04 1002 0106 0202  ................
-00001120: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00001130: f704 fd04 b1                             .....
+00000830: 5c6d 675c 7365 676d 656e 7461 7469 6f6e  \mg\segmentation
+00000840: 5f6d 6f64 656c 735c 656e 636f 6465 7273  _models\encoders
+00000850: 5c64 706e 2e70 7972 0a00 0000 2500 0000  \dpn.pyr....%...
+00000860: 730c 0000 0000 010e 0106 0106 0106 0106  s...............
+00000870: 027a 1444 504e 456e 636f 7264 6572 2e5f  .z.DPNEncorder._
+00000880: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
+00000890: 0000 0000 0100 0000 0900 0000 4300 0000  ............C...
+000008a0: 7398 0000 0074 00a0 01a1 0074 00a0 027c  s....t.....t...|
+000008b0: 006a 0364 0119 006a 047c 006a 0364 0119  .j.d...j.|.j.d..
+000008c0: 006a 057c 006a 0364 0119 006a 06a1 0374  .j.|.j.d...j...t
+000008d0: 00a0 027c 006a 0364 0119 006a 077c 006a  ...|.j.d...j.|.j
+000008e0: 0364 027c 006a 0864 0119 0085 0219 00a1  .d.|.j.d........
+000008f0: 027c 006a 037c 006a 0864 0119 007c 006a  .|.j.|.j.d...|.j
+00000900: 0864 0219 0085 0219 007c 006a 037c 006a  .d.......|.j.|.j
+00000910: 0864 0219 007c 006a 0864 0319 0085 0219  .d...|.j.d......
+00000920: 007c 006a 037c 006a 0864 0319 007c 006a  .|.j.|.j.d...|.j
+00000930: 0864 0419 0085 0219 0067 0653 0029 054e  .d.......g.S.).N
+00000940: 7201 0000 0072 0400 0000 e902 0000 0072  r....r.........r
+00000950: 0800 0000 2909 da02 6e6e da08 4964 656e  ....)...nn..Iden
+00000960: 7469 7479 da0a 5365 7175 656e 7469 616c  tity..Sequential
+00000970: da08 6665 6174 7572 6573 da04 636f 6e76  ..features..conv
+00000980: da02 626e da03 6163 74da 0470 6f6f 6c72  ..bn..act..poolr
+00000990: 0b00 0000 2901 7210 0000 0072 1700 0000  ....).r....r....
+000009a0: 7217 0000 0072 1800 0000 da0a 6765 745f  r....r......get_
+000009b0: 7374 6167 6573 2e00 0000 730e 0000 0000  stages....s.....
+000009c0: 0206 0124 0122 0118 0118 0118 fa7a 1644  ...$.".......z.D
+000009d0: 504e 456e 636f 7264 6572 2e67 6574 5f73  PNEncorder.get_s
+000009e0: 7461 6765 7363 0200 0000 0000 0000 0000  tagesc..........
+000009f0: 0000 0500 0000 0800 0000 4300 0000 7368  ..........C...sh
+00000a00: 0000 007c 00a0 00a1 007d 0267 007d 0374  ...|.....}.g.}.t
+00000a10: 017c 006a 0264 0117 0083 0144 005d 487d  .|.j.d.....D.]H}
+00000a20: 047c 027c 0419 007c 0183 017d 0174 037c  .|.|...|...}.t.|
+00000a30: 0174 0474 0566 0283 0272 587c 03a0 0674  .t.t.f...rX|...t
+00000a40: 076a 0874 096a 0a7c 0164 0164 028d 0264  .j.t.j.|.d.d...d
+00000a50: 0364 048d 02a1 0101 0071 1a7c 03a0 067c  .d.......q.|...|
+00000a60: 01a1 0101 0071 1a7c 0353 0029 054e 7204  .....q.|.S.).Nr.
+00000a70: 0000 0029 01da 0364 696d 5429 01da 0769  ...)...dimT)...i
+00000a80: 6e70 6c61 6365 290b 7222 0000 00da 0572  nplace).r".....r
+00000a90: 616e 6765 720c 0000 00da 0a69 7369 6e73  anger......isins
+00000aa0: 7461 6e63 65da 046c 6973 74da 0574 7570  tance..list..tup
+00000ab0: 6c65 da06 6170 7065 6e64 da01 46da 0472  le..append..F..r
+00000ac0: 656c 75da 0574 6f72 6368 da03 6361 7429  elu..torch..cat)
+00000ad0: 0572 1000 0000 da01 78da 0673 7461 6765  .r......x..stage
+00000ae0: 7372 1d00 0000 da01 6972 1700 0000 7217  sr......ir....r.
+00000af0: 0000 0072 1800 0000 da07 666f 7277 6172  ...r......forwar
+00000b00: 6438 0000 0073 1000 0000 0002 0802 0401  d8...s..........
+00000b10: 1201 0c01 0e01 2002 0c02 7a13 4450 4e45  ...... ...z.DPNE
+00000b20: 6e63 6f72 6465 722e 666f 7277 6172 6463  ncorder.forwardc
+00000b30: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+00000b40: 0300 0000 0b00 0000 7328 0000 007c 01a0  ........s(...|..
+00000b50: 0064 01a1 0101 007c 01a0 0064 02a1 0101  .d.....|...d....
+00000b60: 0074 0183 006a 027c 0166 017c 028e 0101  .t...j.|.f.|....
+00000b70: 0064 0053 0029 034e 7a10 6c61 7374 5f6c  .d.S.).Nz.last_l
+00000b80: 696e 6561 722e 6269 6173 7a12 6c61 7374  inear.biasz.last
+00000b90: 5f6c 696e 6561 722e 7765 6967 6874 2903  _linear.weight).
+00000ba0: da03 706f 7072 0900 0000 da0f 6c6f 6164  ..popr......load
+00000bb0: 5f73 7461 7465 5f64 6963 7429 0372 1000  _state_dict).r..
+00000bc0: 0000 da0a 7374 6174 655f 6469 6374 7214  ....state_dictr.
+00000bd0: 0000 0072 1500 0000 7217 0000 0072 1800  ...r....r....r..
+00000be0: 0000 7233 0000 0046 0000 0073 0600 0000  ..r3...F...s....
+00000bf0: 0001 0a01 0a01 7a1b 4450 4e45 6e63 6f72  ......z.DPNEncor
+00000c00: 6465 722e 6c6f 6164 5f73 7461 7465 5f64  der.load_state_d
+00000c10: 6963 7429 0172 0700 0000 2908 da08 5f5f  ict).r....)...__
+00000c20: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00000c30: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00000c40: 720a 0000 0072 2200 0000 7231 0000 0072  r....r"...r1...r
+00000c50: 3300 0000 da0d 5f5f 636c 6173 7363 656c  3.....__classcel
+00000c60: 6c5f 5f72 1700 0000 7217 0000 0072 1500  l__r....r....r..
+00000c70: 0000 7218 0000 0072 0600 0000 2400 0000  ..r....r....$...
+00000c80: 7308 0000 0008 010e 0908 0a08 0e72 0600  s............r..
+00000c90: 0000 da05 6470 6e36 3829 04e9 0400 0000  ....dpn68)......
+00000ca0: e908 0000 00e9 1400 0000 e918 0000 0029  ...............)
+00000cb0: 0672 0800 0000 e90a 0000 00e9 9000 0000  .r..............
+00000cc0: 6940 0100 00e9 c002 0000 e940 0300 00e9  i@.........@....
+00000cd0: 2000 0000 2904 e910 0000 0072 4200 0000   ...)......rB...
+00000ce0: 7242 0000 00e9 4000 0000 e980 0000 0029  rB....@........)
+00000cf0: 0472 0800 0000 723a 0000 00e9 0c00 0000  .r....r:........
+00000d00: 7208 0000 0069 e803 0000 723e 0000 0054  r....i....r>...T
+00000d10: 290a 7211 0000 0072 1200 0000 da06 6772  ).r....r......gr
+00000d20: 6f75 7073 da07 696e 635f 7365 63da 036b  oups..inc_sec..k
+00000d30: 5f72 da05 6b5f 7365 63da 0b6e 756d 5f63  _r..k_sec..num_c
+00000d40: 6c61 7373 6573 da11 6e75 6d5f 696e 6974  lasses..num_init
+00000d50: 5f66 6561 7475 7265 73da 0573 6d61 6c6c  _features..small
+00000d60: da0e 7465 7374 5f74 696d 655f 706f 6f6c  ..test_time_pool
+00000d70: 2903 da07 656e 636f 6465 7272 0300 0000  )...encoderr....
+00000d80: da06 7061 7261 6d73 da06 6470 6e36 3862  ..params..dpn68b
+00000d90: 290b 7211 0000 0072 1200 0000 da01 6272  ).r....r......br
+00000da0: 4700 0000 7248 0000 0072 4900 0000 724a  G...rH...rI...rJ
+00000db0: 0000 0072 4b00 0000 724c 0000 0072 4d00  ...rK...rL...rM.
+00000dc0: 0000 724e 0000 00da 0564 706e 3932 2904  ..rN.....dpn92).
+00000dd0: 723a 0000 0072 3b00 0000 e91c 0000 0072  r:...r;........r
+00000de0: 4200 0000 2906 7208 0000 0072 4400 0000  B...).r....rD...
+00000df0: e950 0100 0072 4000 0000 6910 0600 00e9  .P...r@...i.....
+00000e00: 800a 0000 2904 7243 0000 0072 4200 0000  ....).rC...rB...
+00000e10: 723d 0000 0072 4500 0000 e960 0000 0029  r=...rE....`...)
+00000e20: 0472 0800 0000 723a 0000 0072 3c00 0000  .r....r:...r<...
+00000e30: 7208 0000 0072 4400 0000 2909 7211 0000  r....rD...).r...
+00000e40: 0072 1200 0000 7247 0000 0072 4800 0000  .r....rG...rH...
+00000e50: 7249 0000 0072 4a00 0000 724b 0000 0072  rI...rJ...rK...r
+00000e60: 4c00 0000 724e 0000 00da 0564 706e 3938  L...rN.....dpn98
+00000e70: 2904 723a 0000 0072 3e00 0000 e91e 0000  ).r:...r>.......
+00000e80: 00e9 2200 0000 2906 7208 0000 0072 5700  .."...).r....rW.
+00000e90: 0000 7255 0000 0069 0003 0000 69c0 0600  ..rU...i....i...
+00000ea0: 0072 5600 0000 e928 0000 0029 0472 4300  .rV....(...).rC.
+00000eb0: 0000 7242 0000 0072 4200 0000 7245 0000  ..rB...rB...rE..
+00000ec0: 00e9 a000 0000 2904 7208 0000 00e9 0600  ......).r.......
+00000ed0: 0000 723c 0000 0072 0800 0000 da06 6470  ..r<...r......dp
+00000ee0: 6e31 3037 2904 7207 0000 00e9 0d00 0000  n107).r.........
+00000ef0: e921 0000 00e9 2500 0000 2906 7208 0000  .!....%...).r...
+00000f00: 0072 4500 0000 6978 0100 0069 8004 0000  .rE...ix...i....
+00000f10: 6980 0900 0072 5600 0000 e932 0000 0029  i....rV....2...)
+00000f20: 0472 3c00 0000 7244 0000 0072 4400 0000  .r<...rD...rD...
+00000f30: 7245 0000 00e9 c800 0000 2904 723a 0000  rE........).r:..
+00000f40: 0072 3b00 0000 723c 0000 0072 0800 0000  .r;...r<...r....
+00000f50: da06 6470 6e31 3331 2904 7207 0000 0072  ..dpn131).r....r
+00000f60: 5f00 0000 e929 0000 00e9 2d00 0000 2906  _....)....-...).
+00000f70: 7208 0000 0072 4500 0000 6960 0100 0072  r....rE...i`...r
+00000f80: 4100 0000 69c0 0700 0072 5600 0000 2904  A...i....rV...).
+00000f90: 723a 0000 0072 3b00 0000 7254 0000 0072  r:...r;...rT...r
+00000fa0: 0800 0000 2906 7239 0000 0072 5100 0000  ....).r9...rQ...
+00000fb0: 7253 0000 0072 5800 0000 725e 0000 0072  rS...rX...r^...r
+00000fc0: 6400 0000 290e da07 5f5f 646f 635f 5f72  d...)...__doc__r
+00000fd0: 2c00 0000 da08 746f 7263 682e 6e6e 721a  ,.....torch.nnr.
+00000fe0: 0000 005a 1374 6f72 6368 2e6e 6e2e 6675  ...Z.torch.nn.fu
+00000ff0: 6e63 7469 6f6e 616c da0a 6675 6e63 7469  nctional..functi
+00001000: 6f6e 616c 722a 0000 005a 1b70 7265 7472  onalr*...Z.pretr
+00001010: 6169 6e65 646d 6f64 656c 732e 6d6f 6465  ainedmodels.mode
+00001020: 6c73 2e64 706e 7202 0000 0072 0300 0000  ls.dpnr....r....
+00001030: da05 5f62 6173 6572 0500 0000 7206 0000  .._baser....r...
+00001040: 00da 0c64 706e 5f65 6e63 6f64 6572 7372  ...dpn_encodersr
+00001050: 1700 0000 7217 0000 0072 1700 0000 7218  ....r....r....r.
+00001060: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00001070: 0073 b200 0000 0419 0801 0c01 1202 0c01  .s..............
+00001080: 0c02 0c03 122a 0201 0602 0201 0201 0201  .....*..........
+00001090: 0201 0201 0201 0201 0201 0201 02f6 04fd  ................
+000010a0: 0411 0201 0602 0201 0201 0201 0201 0201  ................
+000010b0: 0201 0201 0201 0201 0201 02f5 04fd 0412  ................
+000010c0: 0201 0602 0201 0201 0201 0201 0201 0201  ................
+000010d0: 0201 0201 02f7 04fd 0410 0201 0602 0201  ................
+000010e0: 0201 0201 0201 0201 0201 0201 0201 02f7  ................
+000010f0: 04fd 0410 0201 0602 0201 0201 0201 0201  ................
+00001100: 0201 0201 0201 0201 02f7 04fd 0410 0201  ................
+00001110: 0602 0201 0201 0201 0201 0201 0201 0201  ................
+00001120: 0201 02f7 04fd 04b1                      ........
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/dpn.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/dpn.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/efficientnet.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/efficientnet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/efficientnet.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/efficientnet.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/efficientnet.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/efficientnet.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/efficientnet.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/efficientnet.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:20 2023 UTC, .py size: 6470 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -126,166 +126,165 @@
 000007d0: da06 5f64 6570 7468 da0c 5f69 6e5f 6368  .._depth.._in_ch
 000007e0: 616e 6e65 6c73 5a03 5f66 6329 07da 0473  annelsZ._fc)...s
 000007f0: 656c 66da 0a73 7461 6765 5f69 6478 73da  elf..stage_idxs.
 00000800: 0c6f 7574 5f63 6861 6e6e 656c 73da 0a6d  .out_channels..m
 00000810: 6f64 656c 5f6e 616d 65da 0564 6570 7468  odel_name..depth
 00000820: 5a0b 626c 6f63 6b73 5f61 7267 735a 0d67  Z.blocks_argsZ.g
 00000830: 6c6f 6261 6c5f 7061 7261 6d73 a901 da09  lobal_params....
-00000840: 5f5f 636c 6173 735f 5fa9 00fa 5c43 3a5c  __class__...\C:\
+00000840: 5f5f 636c 6173 735f 5fa9 00fa 4f63 3a5c  __class__...Oc:\
 00000850: 5573 6572 735c 6d68 616e 616e 5c44 6f77  Users\mhanan\Dow
-00000860: 6e6c 6f61 6473 5c48 616e 616e 5c4d 616d  nloads\Hanan\Mam
-00000870: 6d6f 5079 5c6d 616d 6d6f 7079 5c73 6567  moPy\mammopy\seg
-00000880: 6d65 6e74 6174 696f 6e5f 6d6f 6465 6c73  mentation_models
-00000890: 5c65 6e63 6f64 6572 735c 6566 6669 6369  \encoders\effici
-000008a0: 656e 746e 6574 2e70 7972 0c00 0000 2100  entnet.pyr....!.
-000008b0: 0000 730e 0000 0000 0210 010e 0206 0106  ..s.............
-000008c0: 0106 0106 027a 1c45 6666 6963 6965 6e74  .....z.Efficient
-000008d0: 4e65 7445 6e63 6f64 6572 2e5f 5f69 6e69  NetEncoder.__ini
-000008e0: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
-000008f0: 0100 0000 0800 0000 4300 0000 7370 0000  ........C...sp..
-00000900: 0074 00a0 01a1 0074 00a0 027c 006a 037c  .t.....t...|.j.|
-00000910: 006a 047c 006a 05a1 037c 006a 0664 007c  .j.|.j...|.j.d.|
-00000920: 006a 0764 0119 0085 0219 007c 006a 067c  .j.d.......|.j.|
-00000930: 006a 0764 0119 007c 006a 0764 0219 0085  .j.d...|.j.d....
-00000940: 0219 007c 006a 067c 006a 0764 0219 007c  ...|.j.|.j.d...|
-00000950: 006a 0764 0319 0085 0219 007c 006a 067c  .j.d.......|.j.|
-00000960: 006a 0764 0319 0064 0085 0219 0067 0653  .j.d...d.....g.S
-00000970: 0029 044e 7201 0000 0072 0600 0000 e902  .).Nr....r......
-00000980: 0000 0029 08da 026e 6eda 0849 6465 6e74  ...)...nn..Ident
-00000990: 6974 79da 0a53 6571 7565 6e74 6961 6c5a  ity..SequentialZ
-000009a0: 0a5f 636f 6e76 5f73 7465 6d5a 045f 626e  ._conv_stemZ._bn
-000009b0: 305a 065f 7377 6973 68da 075f 626c 6f63  0Z._swish.._bloc
-000009c0: 6b73 720d 0000 0029 0172 1100 0000 7218  ksr....).r....r.
-000009d0: 0000 0072 1800 0000 7219 0000 00da 0a67  ...r....r......g
-000009e0: 6574 5f73 7461 6765 732d 0000 0073 0e00  et_stages-...s..
-000009f0: 0000 0002 0601 1201 1201 1801 1801 12fa  ................
-00000a00: 7a1e 4566 6669 6369 656e 744e 6574 456e  z.EfficientNetEn
-00000a10: 636f 6465 722e 6765 745f 7374 6167 6573  coder.get_stages
-00000a20: 6302 0000 0000 0000 0000 0000 0009 0000  c...............
-00000a30: 0005 0000 0043 0000 0073 8200 0000 7c00  .....C...s....|.
-00000a40: a000 a100 7d02 6401 7d03 7c00 6a01 6a02  ....}.d.}.|.j.j.
-00000a50: 7d04 6700 7d05 7403 7c00 6a04 6402 1700  }.g.}.t.|.j.d...
-00000a60: 8301 4400 5d56 7d06 7c06 6403 6b00 7240  ..D.]V}.|.d.k.r@
-00000a70: 7c02 7c06 1900 7c01 8301 7d01 6e32 7c02  |.|...|...}.n2|.
-00000a80: 7c06 1900 4400 5d28 7d07 7c04 7c03 1400  |...D.](}.|.|...
-00000a90: 7405 7c00 6a06 8301 1b00 7d08 7c03 6404  t.|.j.....}.|.d.
-00000aa0: 3700 7d03 7c07 7c01 7c08 8302 7d01 7148  7.}.|.|.|...}.qH
-00000ab0: 7c05 a007 7c01 a101 0100 7126 7c05 5300  |...|.....q&|.S.
-00000ac0: 2905 4e67 0000 0000 0000 0000 7206 0000  ).Ng........r...
-00000ad0: 0072 1a00 0000 6700 0000 0000 00f0 3f29  .r....g.......?)
-00000ae0: 0872 1f00 0000 5a0e 5f67 6c6f 6261 6c5f  .r....Z._global_
-00000af0: 7061 7261 6d73 da11 6472 6f70 5f63 6f6e  params..drop_con
-00000b00: 6e65 6374 5f72 6174 65da 0572 616e 6765  nect_rate..range
-00000b10: 720f 0000 00da 036c 656e 721e 0000 00da  r......lenr.....
-00000b20: 0661 7070 656e 6429 0972 1100 0000 da01  .append).r......
-00000b30: 78da 0673 7461 6765 735a 0c62 6c6f 636b  x..stagesZ.block
-00000b40: 5f6e 756d 6265 7272 2000 0000 da08 6665  _numberr .....fe
-00000b50: 6174 7572 6573 da01 69da 066d 6f64 756c  atures..i..modul
-00000b60: 655a 0c64 726f 705f 636f 6e6e 6563 7472  eZ.drop_connectr
-00000b70: 1800 0000 7218 0000 0072 1900 0000 da07  ....r....r......
-00000b80: 666f 7277 6172 6437 0000 0073 1a00 0000  forward7...s....
-00000b90: 0001 0802 0401 0802 0401 1203 0801 0e04  ................
-00000ba0: 0c01 1201 0801 0c02 0c02 7a1b 4566 6669  ..........z.Effi
-00000bb0: 6369 656e 744e 6574 456e 636f 6465 722e  cientNetEncoder.
-00000bc0: 666f 7277 6172 6463 0200 0000 0000 0000  forwardc........
-00000bd0: 0000 0000 0300 0000 0300 0000 0b00 0000  ................
-00000be0: 7328 0000 007c 01a0 0064 01a1 0101 007c  s(...|...d.....|
-00000bf0: 01a0 0064 02a1 0101 0074 0183 006a 027c  ...d.....t...j.|
-00000c00: 0166 017c 028e 0101 0064 0053 0029 034e  .f.|.....d.S.).N
-00000c10: 7a08 5f66 632e 6269 6173 7a0a 5f66 632e  z._fc.biasz._fc.
-00000c20: 7765 6967 6874 2903 da03 706f 7072 0b00  weight)...popr..
-00000c30: 0000 da0f 6c6f 6164 5f73 7461 7465 5f64  ....load_state_d
-00000c40: 6963 7429 0372 1100 0000 da0a 7374 6174  ict).r......stat
-00000c50: 655f 6469 6374 da06 6b77 6172 6773 7216  e_dict..kwargsr.
-00000c60: 0000 0072 1800 0000 7219 0000 0072 2b00  ...r....r....r+.
-00000c70: 0000 4f00 0000 7306 0000 0000 010a 010a  ..O...s.........
-00000c80: 017a 2345 6666 6963 6965 6e74 4e65 7445  .z#EfficientNetE
-00000c90: 6e63 6f64 6572 2e6c 6f61 645f 7374 6174  ncoder.load_stat
-00000ca0: 655f 6469 6374 2901 7209 0000 0029 08da  e_dict).r....)..
-00000cb0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000cc0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000cd0: 655f 5f72 0c00 0000 721f 0000 0072 2900  e__r....r....r).
-00000ce0: 0000 722b 0000 00da 0d5f 5f63 6c61 7373  ..r+.....__class
-00000cf0: 6365 6c6c 5f5f 7218 0000 0072 1800 0000  cell__r....r....
-00000d00: 7216 0000 0072 1900 0000 7208 0000 0020  r....r....r.... 
-00000d10: 0000 0073 0800 0000 0801 0e0c 080a 0818  ...s............
-00000d20: 7208 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00000d30: 0000 0200 0000 0700 0000 4300 0000 734e  ..........C...sN
-00000d40: 0000 0064 0164 0264 0367 0364 0464 0564  ...d.d.d.g.d.d.d
-00000d50: 0667 0374 007c 0019 0064 0764 0864 0967  .g.t.|...d.d.d.g
-00000d60: 0264 0a9c 0564 0b64 0b64 0b67 0364 0b64  .d...d.d.d.g.d.d
-00000d70: 0b64 0b67 0374 017c 0019 0064 0764 0864  .d.g.t.|...d.d.d
-00000d80: 0967 0264 0a9c 0564 0c9c 027d 017c 0153  .g.d...d...}.|.S
-00000d90: 0029 0d4e 670a d7a3 703d 0adf 3f67 c976  .).Ng...p=..?g.v
-00000da0: be9f 1a2f dd3f 6796 438b 6ce7 fbd9 3f67  .../.?g.C.l...?g
-00000db0: 1d5a 643b df4f cd3f 6779 e926 3108 accc  .Zd;.O.?gy.&1...
-00000dc0: 3f67 cdcc cccc cccc cc3f da03 5247 4272  ?g.......?..RGBr
-00000dd0: 0100 0000 7206 0000 0029 05da 046d 6561  ....r....)...mea
-00000de0: 6eda 0373 7464 da03 7572 6cda 0b69 6e70  n..std..url..inp
-00000df0: 7574 5f73 7061 6365 da0b 696e 7075 745f  ut_space..input_
-00000e00: 7261 6e67 6567 0000 0000 0000 e03f 2902  rangeg.......?).
-00000e10: da08 696d 6167 656e 6574 5a07 6164 7670  ..imagenetZ.advp
-00000e20: 726f 7029 0272 0300 0000 7204 0000 0029  rop).r....r....)
-00000e30: 02da 0765 6e63 6f64 6572 da13 7072 6574  ...encoder..pret
-00000e40: 7261 696e 6564 5f73 6574 7469 6e67 7372  rained_settingsr
-00000e50: 1800 0000 7218 0000 0072 1900 0000 da18  ....r....r......
-00000e60: 5f67 6574 5f70 7265 7472 6169 6e65 645f  _get_pretrained_
-00000e70: 7365 7474 696e 6773 5500 0000 731c 0000  settingsU...s...
-00000e80: 0000 0308 0108 0106 0102 0106 fb04 0808  ................
-00000e90: 0108 0106 0102 0106 fb04 f806 1072 3b00  .............r;.
-00000ea0: 0000 fa0f 6566 6669 6369 656e 746e 6574  ....efficientnet
-00000eb0: 2d62 3029 0672 0a00 0000 e920 0000 00e9  -b0).r..... ....
-00000ec0: 1800 0000 e928 0000 00e9 7000 0000 6940  .....(....p...i@
-00000ed0: 0100 0029 0472 0a00 0000 7209 0000 00e9  ...).r....r.....
-00000ee0: 0900 0000 e910 0000 0029 0372 1300 0000  .........).r....
-00000ef0: 7212 0000 0072 1400 0000 2903 7239 0000  r....r....).r9..
-00000f00: 0072 3a00 0000 da06 7061 7261 6d73 fa0f  .r:.....params..
-00000f10: 6566 6669 6369 656e 746e 6574 2d62 3129  efficientnet-b1)
-00000f20: 0472 0900 0000 e908 0000 0072 4200 0000  .r.........rB...
-00000f30: e917 0000 00fa 0f65 6666 6963 6965 6e74  .......efficient
-00000f40: 6e65 742d 6232 2906 720a 0000 0072 3d00  net-b2).r....r=.
-00000f50: 0000 723e 0000 00e9 3000 0000 e978 0000  ..r>....0....x..
-00000f60: 0069 6001 0000 fa0f 6566 6669 6369 656e  .i`.....efficien
-00000f70: 746e 6574 2d62 3329 0672 0a00 0000 723f  tnet-b3).r....r?
-00000f80: 0000 0072 3d00 0000 7248 0000 00e9 8800  ...r=...rH......
-00000f90: 0000 6980 0100 0029 0472 0900 0000 7245  ..i....).r....rE
-00000fa0: 0000 00e9 1200 0000 e91a 0000 00fa 0f65  ...............e
-00000fb0: 6666 6963 6965 6e74 6e65 742d 6234 2906  fficientnet-b4).
-00000fc0: 720a 0000 0072 4800 0000 723d 0000 00e9  r....rH...r=....
-00000fd0: 3800 0000 e9a0 0000 0069 c001 0000 2904  8........i....).
-00000fe0: e906 0000 00e9 0a00 0000 e916 0000 0072  ...............r
-00000ff0: 3d00 0000 fa0f 6566 6669 6369 656e 746e  =.....efficientn
-00001000: 6574 2d62 3529 0672 0a00 0000 7248 0000  et-b5).r....rH..
-00001010: 0072 3f00 0000 e940 0000 00e9 b000 0000  .r?....@........
-00001020: 6900 0200 0029 0472 4500 0000 e90d 0000  i....).rE.......
-00001030: 00e9 1b00 0000 e927 0000 00fa 0f65 6666  .......'.....eff
-00001040: 6963 6965 6e74 6e65 742d 6236 2906 720a  icientnet-b6).r.
-00001050: 0000 0072 4f00 0000 723f 0000 00e9 4800  ...rO...r?....H.
-00001060: 0000 e9c8 0000 0069 4002 0000 2904 7241  .......i@...).rA
-00001070: 0000 00e9 0f00 0000 e91f 0000 00e9 2d00  ..............-.
-00001080: 0000 fa0f 6566 6669 6369 656e 746e 6574  ....efficientnet
-00001090: 2d62 3729 0672 0a00 0000 7255 0000 0072  -b7).r....rU...r
-000010a0: 4800 0000 e950 0000 00e9 e000 0000 6980  H....P........i.
-000010b0: 0200 0029 04e9 0b00 0000 724c 0000 00e9  ...)......rL....
-000010c0: 2600 0000 e937 0000 0029 0872 3c00 0000  &....7...).r<...
-000010d0: 7244 0000 0072 4700 0000 724a 0000 0072  rD...rG...rJ...r
-000010e0: 4e00 0000 7254 0000 0072 5a00 0000 7260  N...rT...rZ...r`
-000010f0: 0000 0029 0eda 075f 5f64 6f63 5f5f da08  ...)...__doc__..
-00001100: 746f 7263 682e 6e6e 721b 0000 005a 1465  torch.nnr....Z.e
-00001110: 6666 6963 6965 6e74 6e65 745f 7079 746f  fficientnet_pyto
-00001120: 7263 6872 0200 0000 5a1a 6566 6669 6369  rchr....Z.effici
-00001130: 656e 746e 6574 5f70 7974 6f72 6368 2e75  entnet_pytorch.u
-00001140: 7469 6c73 7203 0000 0072 0400 0000 7205  tilsr....r....r.
-00001150: 0000 00da 055f 6261 7365 7207 0000 0072  ....._baser....r
-00001160: 0800 0000 723b 0000 00da 1665 6666 6963  ....r;.....effic
-00001170: 6965 6e74 5f6e 6574 5f65 6e63 6f64 6572  ient_net_encoder
-00001180: 7372 1800 0000 7218 0000 0072 1800 0000  sr....r....r....
-00001190: 7219 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-000011a0: 0000 0073 7e00 0000 0418 0c01 0c01 1402  ...s~...........
-000011b0: 0c03 1235 0816 0201 0602 0201 0201 02fd  ...5............
-000011c0: 04fd 040a 0201 0602 0201 0201 02fd 04fd  ................
-000011d0: 040a 0201 0602 0201 0201 02fd 04fd 040a  ................
-000011e0: 0201 0602 0201 0201 02fd 04fd 040a 0201  ................
-000011f0: 0602 0201 0201 02fd 04fd 040a 0201 0602  ................
-00001200: 0201 0201 02fd 04fd 040a 0201 0602 0201  ................
-00001210: 0201 02fd 04fd 040a 0201 0602 0201 0201  ................
-00001220: 02fd 04fd 04c0                           ......
+00000860: 6e6c 6f61 6473 5c48 616e 616e 5c6d 675c  nloads\Hanan\mg\
+00000870: 7365 676d 656e 7461 7469 6f6e 5f6d 6f64  segmentation_mod
+00000880: 656c 735c 656e 636f 6465 7273 5c65 6666  els\encoders\eff
+00000890: 6963 6965 6e74 6e65 742e 7079 720c 0000  icientnet.pyr...
+000008a0: 0021 0000 0073 0e00 0000 0002 1001 0e02  .!...s..........
+000008b0: 0601 0601 0601 0602 7a1c 4566 6669 6369  ........z.Effici
+000008c0: 656e 744e 6574 456e 636f 6465 722e 5f5f  entNetEncoder.__
+000008d0: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
+000008e0: 0000 0001 0000 0008 0000 0043 0000 0073  ...........C...s
+000008f0: 7000 0000 7400 a001 a100 7400 a002 7c00  p...t.....t...|.
+00000900: 6a03 7c00 6a04 7c00 6a05 a103 7c00 6a06  j.|.j.|.j...|.j.
+00000910: 6400 7c00 6a07 6401 1900 8502 1900 7c00  d.|.j.d.......|.
+00000920: 6a06 7c00 6a07 6401 1900 7c00 6a07 6402  j.|.j.d...|.j.d.
+00000930: 1900 8502 1900 7c00 6a06 7c00 6a07 6402  ......|.j.|.j.d.
+00000940: 1900 7c00 6a07 6403 1900 8502 1900 7c00  ..|.j.d.......|.
+00000950: 6a06 7c00 6a07 6403 1900 6400 8502 1900  j.|.j.d...d.....
+00000960: 6706 5300 2904 4e72 0100 0000 7206 0000  g.S.).Nr....r...
+00000970: 00e9 0200 0000 2908 da02 6e6e da08 4964  ......)...nn..Id
+00000980: 656e 7469 7479 da0a 5365 7175 656e 7469  entity..Sequenti
+00000990: 616c 5a0a 5f63 6f6e 765f 7374 656d 5a04  alZ._conv_stemZ.
+000009a0: 5f62 6e30 5a06 5f73 7769 7368 da07 5f62  _bn0Z._swish.._b
+000009b0: 6c6f 636b 7372 0d00 0000 2901 7211 0000  locksr....).r...
+000009c0: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+000009d0: da0a 6765 745f 7374 6167 6573 2d00 0000  ..get_stages-...
+000009e0: 730e 0000 0000 0206 0112 0112 0118 0118  s...............
+000009f0: 0112 fa7a 1e45 6666 6963 6965 6e74 4e65  ...z.EfficientNe
+00000a00: 7445 6e63 6f64 6572 2e67 6574 5f73 7461  tEncoder.get_sta
+00000a10: 6765 7363 0200 0000 0000 0000 0000 0000  gesc............
+00000a20: 0900 0000 0500 0000 4300 0000 7382 0000  ........C...s...
+00000a30: 007c 00a0 00a1 007d 0264 017d 037c 006a  .|.....}.d.}.|.j
+00000a40: 016a 027d 0467 007d 0574 037c 006a 0464  .j.}.g.}.t.|.j.d
+00000a50: 0217 0083 0144 005d 567d 067c 0664 036b  .....D.]V}.|.d.k
+00000a60: 0072 407c 027c 0619 007c 0183 017d 016e  .r@|.|...|...}.n
+00000a70: 327c 027c 0619 0044 005d 287d 077c 047c  2|.|...D.](}.|.|
+00000a80: 0314 0074 057c 006a 0683 011b 007d 087c  ...t.|.j.....}.|
+00000a90: 0364 0437 007d 037c 077c 017c 0883 027d  .d.7.}.|.|.|...}
+00000aa0: 0171 487c 05a0 077c 01a1 0101 0071 267c  .qH|...|.....q&|
+00000ab0: 0553 0029 054e 6700 0000 0000 0000 0072  .S.).Ng........r
+00000ac0: 0600 0000 721a 0000 0067 0000 0000 0000  ....r....g......
+00000ad0: f03f 2908 721f 0000 005a 0e5f 676c 6f62  .?).r....Z._glob
+00000ae0: 616c 5f70 6172 616d 73da 1164 726f 705f  al_params..drop_
+00000af0: 636f 6e6e 6563 745f 7261 7465 da05 7261  connect_rate..ra
+00000b00: 6e67 6572 0f00 0000 da03 6c65 6e72 1e00  nger......lenr..
+00000b10: 0000 da06 6170 7065 6e64 2909 7211 0000  ....append).r...
+00000b20: 00da 0178 da06 7374 6167 6573 5a0c 626c  ...x..stagesZ.bl
+00000b30: 6f63 6b5f 6e75 6d62 6572 7220 0000 00da  ock_numberr ....
+00000b40: 0866 6561 7475 7265 73da 0169 da06 6d6f  .features..i..mo
+00000b50: 6475 6c65 5a0c 6472 6f70 5f63 6f6e 6e65  duleZ.drop_conne
+00000b60: 6374 7218 0000 0072 1800 0000 7219 0000  ctr....r....r...
+00000b70: 00da 0766 6f72 7761 7264 3700 0000 731a  ...forward7...s.
+00000b80: 0000 0000 0108 0204 0108 0204 0112 0308  ................
+00000b90: 010e 040c 0112 0108 010c 020c 027a 1b45  .............z.E
+00000ba0: 6666 6963 6965 6e74 4e65 7445 6e63 6f64  fficientNetEncod
+00000bb0: 6572 2e66 6f72 7761 7264 6302 0000 0000  er.forwardc.....
+00000bc0: 0000 0000 0000 0003 0000 0003 0000 000b  ................
+00000bd0: 0000 0073 2800 0000 7c01 a000 6401 a101  ...s(...|...d...
+00000be0: 0100 7c01 a000 6402 a101 0100 7401 8300  ..|...d.....t...
+00000bf0: 6a02 7c01 6601 7c02 8e01 0100 6400 5300  j.|.f.|.....d.S.
+00000c00: 2903 4e7a 085f 6663 2e62 6961 737a 0a5f  ).Nz._fc.biasz._
+00000c10: 6663 2e77 6569 6768 7429 03da 0370 6f70  fc.weight)...pop
+00000c20: 720b 0000 00da 0f6c 6f61 645f 7374 6174  r......load_stat
+00000c30: 655f 6469 6374 2903 7211 0000 00da 0a73  e_dict).r......s
+00000c40: 7461 7465 5f64 6963 74da 066b 7761 7267  tate_dict..kwarg
+00000c50: 7372 1600 0000 7218 0000 0072 1900 0000  sr....r....r....
+00000c60: 722b 0000 004f 0000 0073 0600 0000 0001  r+...O...s......
+00000c70: 0a01 0a01 7a23 4566 6669 6369 656e 744e  ....z#EfficientN
+00000c80: 6574 456e 636f 6465 722e 6c6f 6164 5f73  etEncoder.load_s
+00000c90: 7461 7465 5f64 6963 7429 0172 0900 0000  tate_dict).r....
+00000ca0: 2908 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00000cb0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00000cc0: 6e61 6d65 5f5f 720c 0000 0072 1f00 0000  name__r....r....
+00000cd0: 7229 0000 0072 2b00 0000 da0d 5f5f 636c  r)...r+.....__cl
+00000ce0: 6173 7363 656c 6c5f 5f72 1800 0000 7218  asscell__r....r.
+00000cf0: 0000 0072 1600 0000 7219 0000 0072 0800  ...r....r....r..
+00000d00: 0000 2000 0000 7308 0000 0008 010e 0c08  .. ...s.........
+00000d10: 0a08 1872 0800 0000 6301 0000 0000 0000  ...r....c.......
+00000d20: 0000 0000 0002 0000 0007 0000 0043 0000  .............C..
+00000d30: 0073 4e00 0000 6401 6402 6403 6703 6404  .sN...d.d.d.g.d.
+00000d40: 6405 6406 6703 7400 7c00 1900 6407 6408  d.d.g.t.|...d.d.
+00000d50: 6409 6702 640a 9c05 640b 640b 640b 6703  d.g.d...d.d.d.g.
+00000d60: 640b 640b 640b 6703 7401 7c00 1900 6407  d.d.d.g.t.|...d.
+00000d70: 6408 6409 6702 640a 9c05 640c 9c02 7d01  d.d.g.d...d...}.
+00000d80: 7c01 5300 290d 4e67 0ad7 a370 3d0a df3f  |.S.).Ng...p=..?
+00000d90: 67c9 76be 9f1a 2fdd 3f67 9643 8b6c e7fb  g.v.../.?g.C.l..
+00000da0: d93f 671d 5a64 3bdf 4fcd 3f67 79e9 2631  .?g.Zd;.O.?gy.&1
+00000db0: 08ac cc3f 67cd cccc cccc cccc 3fda 0352  ...?g.......?..R
+00000dc0: 4742 7201 0000 0072 0600 0000 2905 da04  GBr....r....)...
+00000dd0: 6d65 616e da03 7374 64da 0375 726c da0b  mean..std..url..
+00000de0: 696e 7075 745f 7370 6163 65da 0b69 6e70  input_space..inp
+00000df0: 7574 5f72 616e 6765 6700 0000 0000 00e0  ut_rangeg.......
+00000e00: 3f29 02da 0869 6d61 6765 6e65 745a 0761  ?)...imagenetZ.a
+00000e10: 6476 7072 6f70 2902 7203 0000 0072 0400  dvprop).r....r..
+00000e20: 0000 2902 da07 656e 636f 6465 72da 1370  ..)...encoder..p
+00000e30: 7265 7472 6169 6e65 645f 7365 7474 696e  retrained_settin
+00000e40: 6773 7218 0000 0072 1800 0000 7219 0000  gsr....r....r...
+00000e50: 00da 185f 6765 745f 7072 6574 7261 696e  ..._get_pretrain
+00000e60: 6564 5f73 6574 7469 6e67 7355 0000 0073  ed_settingsU...s
+00000e70: 1c00 0000 0003 0801 0801 0601 0201 06fb  ................
+00000e80: 0408 0801 0801 0601 0201 06fb 04f8 0610  ................
+00000e90: 723b 0000 00fa 0f65 6666 6963 6965 6e74  r;.....efficient
+00000ea0: 6e65 742d 6230 2906 720a 0000 00e9 2000  net-b0).r..... .
+00000eb0: 0000 e918 0000 00e9 2800 0000 e970 0000  ........(....p..
+00000ec0: 0069 4001 0000 2904 720a 0000 0072 0900  .i@...).r....r..
+00000ed0: 0000 e909 0000 00e9 1000 0000 2903 7213  ............).r.
+00000ee0: 0000 0072 1200 0000 7214 0000 0029 0372  ...r....r....).r
+00000ef0: 3900 0000 723a 0000 00da 0670 6172 616d  9...r:.....param
+00000f00: 73fa 0f65 6666 6963 6965 6e74 6e65 742d  s..efficientnet-
+00000f10: 6231 2904 7209 0000 00e9 0800 0000 7242  b1).r.........rB
+00000f20: 0000 00e9 1700 0000 fa0f 6566 6669 6369  ..........effici
+00000f30: 656e 746e 6574 2d62 3229 0672 0a00 0000  entnet-b2).r....
+00000f40: 723d 0000 0072 3e00 0000 e930 0000 00e9  r=...r>....0....
+00000f50: 7800 0000 6960 0100 00fa 0f65 6666 6963  x...i`.....effic
+00000f60: 6965 6e74 6e65 742d 6233 2906 720a 0000  ientnet-b3).r...
+00000f70: 0072 3f00 0000 723d 0000 0072 4800 0000  .r?...r=...rH...
+00000f80: e988 0000 0069 8001 0000 2904 7209 0000  .....i....).r...
+00000f90: 0072 4500 0000 e912 0000 00e9 1a00 0000  .rE.............
+00000fa0: fa0f 6566 6669 6369 656e 746e 6574 2d62  ..efficientnet-b
+00000fb0: 3429 0672 0a00 0000 7248 0000 0072 3d00  4).r....rH...r=.
+00000fc0: 0000 e938 0000 00e9 a000 0000 69c0 0100  ...8........i...
+00000fd0: 0029 04e9 0600 0000 e90a 0000 00e9 1600  .)..............
+00000fe0: 0000 723d 0000 00fa 0f65 6666 6963 6965  ..r=.....efficie
+00000ff0: 6e74 6e65 742d 6235 2906 720a 0000 0072  ntnet-b5).r....r
+00001000: 4800 0000 723f 0000 00e9 4000 0000 e9b0  H...r?....@.....
+00001010: 0000 0069 0002 0000 2904 7245 0000 00e9  ...i....).rE....
+00001020: 0d00 0000 e91b 0000 00e9 2700 0000 fa0f  ..........'.....
+00001030: 6566 6669 6369 656e 746e 6574 2d62 3629  efficientnet-b6)
+00001040: 0672 0a00 0000 724f 0000 0072 3f00 0000  .r....rO...r?...
+00001050: e948 0000 00e9 c800 0000 6940 0200 0029  .H........i@...)
+00001060: 0472 4100 0000 e90f 0000 00e9 1f00 0000  .rA.............
+00001070: e92d 0000 00fa 0f65 6666 6963 6965 6e74  .-.....efficient
+00001080: 6e65 742d 6237 2906 720a 0000 0072 5500  net-b7).r....rU.
+00001090: 0000 7248 0000 00e9 5000 0000 e9e0 0000  ..rH....P.......
+000010a0: 0069 8002 0000 2904 e90b 0000 0072 4c00  .i....)......rL.
+000010b0: 0000 e926 0000 00e9 3700 0000 2908 723c  ...&....7...).r<
+000010c0: 0000 0072 4400 0000 7247 0000 0072 4a00  ...rD...rG...rJ.
+000010d0: 0000 724e 0000 0072 5400 0000 725a 0000  ..rN...rT...rZ..
+000010e0: 0072 6000 0000 290e da07 5f5f 646f 635f  .r`...)...__doc_
+000010f0: 5fda 0874 6f72 6368 2e6e 6e72 1b00 0000  _..torch.nnr....
+00001100: 5a14 6566 6669 6369 656e 746e 6574 5f70  Z.efficientnet_p
+00001110: 7974 6f72 6368 7202 0000 005a 1a65 6666  ytorchr....Z.eff
+00001120: 6963 6965 6e74 6e65 745f 7079 746f 7263  icientnet_pytorc
+00001130: 682e 7574 696c 7372 0300 0000 7204 0000  h.utilsr....r...
+00001140: 0072 0500 0000 da05 5f62 6173 6572 0700  .r......_baser..
+00001150: 0000 7208 0000 0072 3b00 0000 da16 6566  ..r....r;.....ef
+00001160: 6669 6369 656e 745f 6e65 745f 656e 636f  ficient_net_enco
+00001170: 6465 7273 7218 0000 0072 1800 0000 7218  dersr....r....r.
+00001180: 0000 0072 1900 0000 da08 3c6d 6f64 756c  ...r......<modul
+00001190: 653e 0100 0000 737e 0000 0004 180c 010c  e>....s~........
+000011a0: 0114 020c 0312 3508 1602 0106 0202 0102  ......5.........
+000011b0: 0102 fd04 fd04 0a02 0106 0202 0102 0102  ................
+000011c0: fd04 fd04 0a02 0106 0202 0102 0102 fd04  ................
+000011d0: fd04 0a02 0106 0202 0102 0102 fd04 fd04  ................
+000011e0: 0a02 0106 0202 0102 0102 fd04 fd04 0a02  ................
+000011f0: 0106 0202 0102 0102 fd04 fd04 0a02 0106  ................
+00001200: 0202 0102 0102 fd04 fd04 0a02 0106 0202  ................
+00001210: 0102 0102 fd04 fd04 c0                   .........
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/efficientnet.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/efficientnet.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:20 2023 UTC, .py size: 3551 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -120,117 +120,116 @@
 00000770: 7632 64da 0b6b 6572 6e65 6c5f 7369 7a65  v2d..kernel_size
 00000780: da07 7061 6464 696e 67da 094d 6178 506f  ..padding..MaxPo
 00000790: 6f6c 3264 da0a 6176 6770 6f6f 6c5f 3161  ol2d..avgpool_1a
 000007a0: da0b 6c61 7374 5f6c 696e 6561 7229 05da  ..last_linear)..
 000007b0: 0473 656c 66da 0c6f 7574 5f63 6861 6e6e  .self..out_chann
 000007c0: 656c 73da 0564 6570 7468 da06 6b77 6172  els..depth..kwar
 000007d0: 6773 da01 6da9 01da 095f 5f63 6c61 7373  gs..m....__class
-000007e0: 5f5f a900 fa61 433a 5c55 7365 7273 5c6d  __...aC:\Users\m
+000007e0: 5f5f a900 fa54 633a 5c55 7365 7273 5c6d  __...Tc:\Users\m
 000007f0: 6861 6e61 6e5c 446f 776e 6c6f 6164 735c  hanan\Downloads\
-00000800: 4861 6e61 6e5c 4d61 6d6d 6f50 795c 6d61  Hanan\MammoPy\ma
-00000810: 6d6d 6f70 795c 7365 676d 656e 7461 7469  mmopy\segmentati
-00000820: 6f6e 5f6d 6f64 656c 735c 656e 636f 6465  on_models\encode
-00000830: 7273 5c69 6e63 6570 7469 6f6e 7265 736e  rs\inceptionresn
-00000840: 6574 7632 2e70 7972 0a00 0000 2200 0000  etv2.pyr...."...
-00000850: 7318 0000 0000 010e 0206 0106 0106 030c  s...............
-00000860: 010c 010a 0106 010c 0108 0304 017a 2149  .............z!I
-00000870: 6e63 6570 7469 6f6e 5265 734e 6574 5632  nceptionResNetV2
-00000880: 456e 636f 6465 722e 5f5f 696e 6974 5f5f  Encoder.__init__
-00000890: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-000008a0: 0002 0000 0043 0000 0073 0c00 0000 7400  .....C...s....t.
-000008b0: 6401 8301 8201 6400 5300 2902 4e7a 6249  d.....d.S.).NzbI
-000008c0: 6e63 6570 7469 6f6e 5265 736e 6574 5632  nceptionResnetV2
-000008d0: 2065 6e63 6f64 6572 2064 6f65 7320 6e6f   encoder does no
-000008e0: 7420 7375 7070 6f72 7420 6469 6c61 7465  t support dilate
-000008f0: 6420 6d6f 6465 2064 7565 2074 6f20 706f  d mode due to po
-00000900: 6f6c 696e 6720 6f70 6572 6174 696f 6e20  oling operation 
-00000910: 666f 7220 646f 776e 7361 6d70 6c69 6e67  for downsampling
-00000920: 2129 01da 0a56 616c 7565 4572 726f 7229  !)...ValueError)
-00000930: 0372 1700 0000 da0a 7374 6167 655f 6c69  .r......stage_li
-00000940: 7374 da0d 6469 6c61 7469 6f6e 5f6c 6973  st..dilation_lis
-00000950: 7472 1e00 0000 721e 0000 0072 1f00 0000  tr....r....r....
-00000960: da0c 6d61 6b65 5f64 696c 6174 6564 3500  ..make_dilated5.
-00000970: 0000 7302 0000 0000 017a 2549 6e63 6570  ..s......z%Incep
-00000980: 7469 6f6e 5265 734e 6574 5632 456e 636f  tionResNetV2Enco
-00000990: 6465 722e 6d61 6b65 5f64 696c 6174 6564  der.make_dilated
-000009a0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000009b0: 000b 0000 0043 0000 0073 6400 0000 7400  .....C...sd...t.
-000009c0: a001 a100 7400 a002 7c00 6a03 7c00 6a04  ....t...|.j.|.j.
-000009d0: 7c00 6a05 a103 7400 a002 7c00 6a06 7c00  |.j...t...|.j.|.
-000009e0: 6a07 7c00 6a08 a103 7400 a002 7c00 6a09  j.|.j...t...|.j.
-000009f0: 7c00 6a0a 7c00 6a0b a103 7400 a002 7c00  |.j.|.j...t...|.
-00000a00: 6a0c 7c00 6a0d a102 7400 a002 7c00 6a0e  j.|.j...t...|.j.
-00000a10: 7c00 6a0f 7c00 6a10 7c00 6a11 a104 6706  |.j.|.j.|.j...g.
-00000a20: 5300 2901 4e29 1272 1000 0000 da08 4964  S.).N).r......Id
-00000a30: 656e 7469 7479 da0a 5365 7175 656e 7469  entity..Sequenti
-00000a40: 616c da09 636f 6e76 3264 5f31 61da 0963  al..conv2d_1a..c
-00000a50: 6f6e 7632 645f 3261 da09 636f 6e76 3264  onv2d_2a..conv2d
-00000a60: 5f32 62da 0a6d 6178 706f 6f6c 5f33 61da  _2b..maxpool_3a.
-00000a70: 0963 6f6e 7632 645f 3362 da09 636f 6e76  .conv2d_3b..conv
-00000a80: 3264 5f34 61da 0a6d 6178 706f 6f6c 5f35  2d_4a..maxpool_5
-00000a90: 61da 086d 6978 6564 5f35 62da 0672 6570  a..mixed_5b..rep
-00000aa0: 6561 74da 086d 6978 6564 5f36 61da 0872  eat..mixed_6a..r
-00000ab0: 6570 6561 745f 31da 086d 6978 6564 5f37  epeat_1..mixed_7
-00000ac0: 61da 0872 6570 6561 745f 32da 0662 6c6f  a..repeat_2..blo
-00000ad0: 636b 38da 0963 6f6e 7632 645f 3762 2901  ck8..conv2d_7b).
-00000ae0: 7217 0000 0072 1e00 0000 721e 0000 0072  r....r....r....r
-00000af0: 1f00 0000 da0a 6765 745f 7374 6167 6573  ......get_stages
-00000b00: 3900 0000 730e 0000 0000 0206 0112 0112  9...s...........
-00000b10: 0112 010e 0116 fa7a 2349 6e63 6570 7469  .......z#Incepti
-00000b20: 6f6e 5265 734e 6574 5632 456e 636f 6465  onResNetV2Encode
-00000b30: 722e 6765 745f 7374 6167 6573 6302 0000  r.get_stagesc...
-00000b40: 0000 0000 0000 0000 0005 0000 0004 0000  ................
-00000b50: 0043 0000 0073 3a00 0000 7c00 a000 a100  .C...s:...|.....
-00000b60: 7d02 6700 7d03 7401 7c00 6a02 6401 1700  }.g.}.t.|.j.d...
-00000b70: 8301 4400 5d1a 7d04 7c02 7c04 1900 7c01  ..D.].}.|.|...|.
-00000b80: 8301 7d01 7c03 a003 7c01 a101 0100 711a  ..}.|...|.....q.
-00000b90: 7c03 5300 2902 4e72 0400 0000 2904 7235  |.S.).Nr....).r5
-00000ba0: 0000 00da 0572 616e 6765 720c 0000 00da  .....ranger.....
-00000bb0: 0661 7070 656e 6429 0572 1700 0000 da01  .append).r......
-00000bc0: 78da 0673 7461 6765 73da 0866 6561 7475  x..stages..featu
-00000bd0: 7265 73da 0169 721e 0000 0072 1e00 0000  res..ir....r....
-00000be0: 721f 0000 00da 0766 6f72 7761 7264 4300  r......forwardC.
-00000bf0: 0000 730c 0000 0000 0208 0204 0112 010c  ..s.............
-00000c00: 010c 027a 2049 6e63 6570 7469 6f6e 5265  ...z InceptionRe
-00000c10: 734e 6574 5632 456e 636f 6465 722e 666f  sNetV2Encoder.fo
-00000c20: 7277 6172 6463 0200 0000 0000 0000 0000  rwardc..........
-00000c30: 0000 0300 0000 0300 0000 0b00 0000 7328  ..............s(
-00000c40: 0000 007c 01a0 0064 01a1 0101 007c 01a0  ...|...d.....|..
-00000c50: 0064 02a1 0101 0074 0183 006a 027c 0166  .d.....t...j.|.f
-00000c60: 017c 028e 0101 0064 0053 0029 034e 7a10  .|.....d.S.).Nz.
-00000c70: 6c61 7374 5f6c 696e 6561 722e 6269 6173  last_linear.bias
-00000c80: 7a12 6c61 7374 5f6c 696e 6561 722e 7765  z.last_linear.we
-00000c90: 6967 6874 2903 da03 706f 7072 0900 0000  ight)...popr....
-00000ca0: da0f 6c6f 6164 5f73 7461 7465 5f64 6963  ..load_state_dic
-00000cb0: 7429 0372 1700 0000 da0a 7374 6174 655f  t).r......state_
-00000cc0: 6469 6374 721a 0000 0072 1c00 0000 721e  dictr....r....r.
-00000cd0: 0000 0072 1f00 0000 723e 0000 004e 0000  ...r....r>...N..
-00000ce0: 0073 0600 0000 0001 0a01 0a01 7a28 496e  .s..........z(In
-00000cf0: 6365 7074 696f 6e52 6573 4e65 7456 3245  ceptionResNetV2E
-00000d00: 6e63 6f64 6572 2e6c 6f61 645f 7374 6174  ncoder.load_stat
-00000d10: 655f 6469 6374 2901 7207 0000 0029 09da  e_dict).r....)..
-00000d20: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000d30: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000d40: 655f 5f72 0a00 0000 7223 0000 0072 3500  e__r....r#...r5.
-00000d50: 0000 723c 0000 0072 3e00 0000 da0d 5f5f  ..r<...r>.....__
-00000d60: 636c 6173 7363 656c 6c5f 5f72 1e00 0000  classcell__r....
-00000d70: 721e 0000 0072 1c00 0000 721f 0000 0072  r....r....r....r
-00000d80: 0600 0000 2100 0000 730a 0000 0008 010e  ....!...s.......
-00000d90: 1308 0408 0a08 0b72 0600 0000 da11 696e  .......r......in
-00000da0: 6365 7074 696f 6e72 6573 6e65 7476 3229  ceptionresnetv2)
-00000db0: 0672 0800 0000 e940 0000 00e9 c000 0000  .r.....@........
-00000dc0: 6940 0100 0069 4004 0000 6900 0600 0069  i@...i@...i....i
-00000dd0: e803 0000 2902 7218 0000 00da 0b6e 756d  ....).r......num
-00000de0: 5f63 6c61 7373 6573 2903 da07 656e 636f  _classes)...enco
-00000df0: 6465 7272 0300 0000 da06 7061 7261 6d73  derr......params
-00000e00: 290a da07 5f5f 646f 635f 5fda 0874 6f72  )...__doc__..tor
-00000e10: 6368 2e6e 6e72 1000 0000 5a29 7072 6574  ch.nnr....Z)pret
-00000e20: 7261 696e 6564 6d6f 6465 6c73 2e6d 6f64  rainedmodels.mod
-00000e30: 656c 732e 696e 6365 7074 696f 6e72 6573  els.inceptionres
-00000e40: 6e65 7476 3272 0200 0000 7203 0000 00da  netv2r....r.....
-00000e50: 055f 6261 7365 7205 0000 0072 0600 0000  ._baser....r....
-00000e60: da1a 696e 6365 7074 696f 6e72 6573 6e65  ..inceptionresne
-00000e70: 7476 325f 656e 636f 6465 7273 721e 0000  tv2_encodersr...
-00000e80: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00000e90: da08 3c6d 6f64 756c 653e 0100 0000 7316  ..<module>....s.
-00000ea0: 0000 0004 190c 010c 010c 020c 0312 3402  ..............4.
-00000eb0: 0102 0106 0108 fd04 ff                   .........
+00000800: 4861 6e61 6e5c 6d67 5c73 6567 6d65 6e74  Hanan\mg\segment
+00000810: 6174 696f 6e5f 6d6f 6465 6c73 5c65 6e63  ation_models\enc
+00000820: 6f64 6572 735c 696e 6365 7074 696f 6e72  oders\inceptionr
+00000830: 6573 6e65 7476 322e 7079 720a 0000 0022  esnetv2.pyr...."
+00000840: 0000 0073 1800 0000 0001 0e02 0601 0601  ...s............
+00000850: 0603 0c01 0c01 0a01 0601 0c01 0803 0401  ................
+00000860: 7a21 496e 6365 7074 696f 6e52 6573 4e65  z!InceptionResNe
+00000870: 7456 3245 6e63 6f64 6572 2e5f 5f69 6e69  tV2Encoder.__ini
+00000880: 745f 5f63 0300 0000 0000 0000 0000 0000  t__c............
+00000890: 0300 0000 0200 0000 4300 0000 730c 0000  ........C...s...
+000008a0: 0074 0064 0183 0182 0164 0053 0029 024e  .t.d.....d.S.).N
+000008b0: 7a62 496e 6365 7074 696f 6e52 6573 6e65  zbInceptionResne
+000008c0: 7456 3220 656e 636f 6465 7220 646f 6573  tV2 encoder does
+000008d0: 206e 6f74 2073 7570 706f 7274 2064 696c   not support dil
+000008e0: 6174 6564 206d 6f64 6520 6475 6520 746f  ated mode due to
+000008f0: 2070 6f6f 6c69 6e67 206f 7065 7261 7469   pooling operati
+00000900: 6f6e 2066 6f72 2064 6f77 6e73 616d 706c  on for downsampl
+00000910: 696e 6721 2901 da0a 5661 6c75 6545 7272  ing!)...ValueErr
+00000920: 6f72 2903 7217 0000 00da 0a73 7461 6765  or).r......stage
+00000930: 5f6c 6973 74da 0d64 696c 6174 696f 6e5f  _list..dilation_
+00000940: 6c69 7374 721e 0000 0072 1e00 0000 721f  listr....r....r.
+00000950: 0000 00da 0c6d 616b 655f 6469 6c61 7465  .....make_dilate
+00000960: 6435 0000 0073 0200 0000 0001 7a25 496e  d5...s......z%In
+00000970: 6365 7074 696f 6e52 6573 4e65 7456 3245  ceptionResNetV2E
+00000980: 6e63 6f64 6572 2e6d 616b 655f 6469 6c61  ncoder.make_dila
+00000990: 7465 6463 0100 0000 0000 0000 0000 0000  tedc............
+000009a0: 0100 0000 0b00 0000 4300 0000 7364 0000  ........C...sd..
+000009b0: 0074 00a0 01a1 0074 00a0 027c 006a 037c  .t.....t...|.j.|
+000009c0: 006a 047c 006a 05a1 0374 00a0 027c 006a  .j.|.j...t...|.j
+000009d0: 067c 006a 077c 006a 08a1 0374 00a0 027c  .|.j.|.j...t...|
+000009e0: 006a 097c 006a 0a7c 006a 0ba1 0374 00a0  .j.|.j.|.j...t..
+000009f0: 027c 006a 0c7c 006a 0da1 0274 00a0 027c  .|.j.|.j...t...|
+00000a00: 006a 0e7c 006a 0f7c 006a 107c 006a 11a1  .j.|.j.|.j.|.j..
+00000a10: 0467 0653 0029 014e 2912 7210 0000 00da  .g.S.).N).r.....
+00000a20: 0849 6465 6e74 6974 79da 0a53 6571 7565  .Identity..Seque
+00000a30: 6e74 6961 6cda 0963 6f6e 7632 645f 3161  ntial..conv2d_1a
+00000a40: da09 636f 6e76 3264 5f32 61da 0963 6f6e  ..conv2d_2a..con
+00000a50: 7632 645f 3262 da0a 6d61 7870 6f6f 6c5f  v2d_2b..maxpool_
+00000a60: 3361 da09 636f 6e76 3264 5f33 62da 0963  3a..conv2d_3b..c
+00000a70: 6f6e 7632 645f 3461 da0a 6d61 7870 6f6f  onv2d_4a..maxpoo
+00000a80: 6c5f 3561 da08 6d69 7865 645f 3562 da06  l_5a..mixed_5b..
+00000a90: 7265 7065 6174 da08 6d69 7865 645f 3661  repeat..mixed_6a
+00000aa0: da08 7265 7065 6174 5f31 da08 6d69 7865  ..repeat_1..mixe
+00000ab0: 645f 3761 da08 7265 7065 6174 5f32 da06  d_7a..repeat_2..
+00000ac0: 626c 6f63 6b38 da09 636f 6e76 3264 5f37  block8..conv2d_7
+00000ad0: 6229 0172 1700 0000 721e 0000 0072 1e00  b).r....r....r..
+00000ae0: 0000 721f 0000 00da 0a67 6574 5f73 7461  ..r......get_sta
+00000af0: 6765 7339 0000 0073 0e00 0000 0002 0601  ges9...s........
+00000b00: 1201 1201 1201 0e01 16fa 7a23 496e 6365  ..........z#Ince
+00000b10: 7074 696f 6e52 6573 4e65 7456 3245 6e63  ptionResNetV2Enc
+00000b20: 6f64 6572 2e67 6574 5f73 7461 6765 7363  oder.get_stagesc
+00000b30: 0200 0000 0000 0000 0000 0000 0500 0000  ................
+00000b40: 0400 0000 4300 0000 733a 0000 007c 00a0  ....C...s:...|..
+00000b50: 00a1 007d 0267 007d 0374 017c 006a 0264  ...}.g.}.t.|.j.d
+00000b60: 0117 0083 0144 005d 1a7d 047c 027c 0419  .....D.].}.|.|..
+00000b70: 007c 0183 017d 017c 03a0 037c 01a1 0101  .|...}.|...|....
+00000b80: 0071 1a7c 0353 0029 024e 7204 0000 0029  .q.|.S.).Nr....)
+00000b90: 0472 3500 0000 da05 7261 6e67 6572 0c00  .r5.....ranger..
+00000ba0: 0000 da06 6170 7065 6e64 2905 7217 0000  ....append).r...
+00000bb0: 00da 0178 da06 7374 6167 6573 da08 6665  ...x..stages..fe
+00000bc0: 6174 7572 6573 da01 6972 1e00 0000 721e  atures..ir....r.
+00000bd0: 0000 0072 1f00 0000 da07 666f 7277 6172  ...r......forwar
+00000be0: 6443 0000 0073 0c00 0000 0002 0802 0401  dC...s..........
+00000bf0: 1201 0c01 0c02 7a20 496e 6365 7074 696f  ......z Inceptio
+00000c00: 6e52 6573 4e65 7456 3245 6e63 6f64 6572  nResNetV2Encoder
+00000c10: 2e66 6f72 7761 7264 6302 0000 0000 0000  .forwardc.......
+00000c20: 0000 0000 0003 0000 0003 0000 000b 0000  ................
+00000c30: 0073 2800 0000 7c01 a000 6401 a101 0100  .s(...|...d.....
+00000c40: 7c01 a000 6402 a101 0100 7401 8300 6a02  |...d.....t...j.
+00000c50: 7c01 6601 7c02 8e01 0100 6400 5300 2903  |.f.|.....d.S.).
+00000c60: 4e7a 106c 6173 745f 6c69 6e65 6172 2e62  Nz.last_linear.b
+00000c70: 6961 737a 126c 6173 745f 6c69 6e65 6172  iasz.last_linear
+00000c80: 2e77 6569 6768 7429 03da 0370 6f70 7209  .weight)...popr.
+00000c90: 0000 00da 0f6c 6f61 645f 7374 6174 655f  .....load_state_
+00000ca0: 6469 6374 2903 7217 0000 00da 0a73 7461  dict).r......sta
+00000cb0: 7465 5f64 6963 7472 1a00 0000 721c 0000  te_dictr....r...
+00000cc0: 0072 1e00 0000 721f 0000 0072 3e00 0000  .r....r....r>...
+00000cd0: 4e00 0000 7306 0000 0000 010a 010a 017a  N...s..........z
+00000ce0: 2849 6e63 6570 7469 6f6e 5265 734e 6574  (InceptionResNet
+00000cf0: 5632 456e 636f 6465 722e 6c6f 6164 5f73  V2Encoder.load_s
+00000d00: 7461 7465 5f64 6963 7429 0172 0700 0000  tate_dict).r....
+00000d10: 2909 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00000d20: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00000d30: 6e61 6d65 5f5f 720a 0000 0072 2300 0000  name__r....r#...
+00000d40: 7235 0000 0072 3c00 0000 723e 0000 00da  r5...r<...r>....
+00000d50: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 721e  .__classcell__r.
+00000d60: 0000 0072 1e00 0000 721c 0000 0072 1f00  ...r....r....r..
+00000d70: 0000 7206 0000 0021 0000 0073 0a00 0000  ..r....!...s....
+00000d80: 0801 0e13 0804 080a 080b 7206 0000 00da  ..........r.....
+00000d90: 1169 6e63 6570 7469 6f6e 7265 736e 6574  .inceptionresnet
+00000da0: 7632 2906 7208 0000 00e9 4000 0000 e9c0  v2).r.....@.....
+00000db0: 0000 0069 4001 0000 6940 0400 0069 0006  ...i@...i@...i..
+00000dc0: 0000 69e8 0300 0029 0272 1800 0000 da0b  ..i....).r......
+00000dd0: 6e75 6d5f 636c 6173 7365 7329 03da 0765  num_classes)...e
+00000de0: 6e63 6f64 6572 7203 0000 00da 0670 6172  ncoderr......par
+00000df0: 616d 7329 0ada 075f 5f64 6f63 5f5f da08  ams)...__doc__..
+00000e00: 746f 7263 682e 6e6e 7210 0000 005a 2970  torch.nnr....Z)p
+00000e10: 7265 7472 6169 6e65 646d 6f64 656c 732e  retrainedmodels.
+00000e20: 6d6f 6465 6c73 2e69 6e63 6570 7469 6f6e  models.inception
+00000e30: 7265 736e 6574 7632 7202 0000 0072 0300  resnetv2r....r..
+00000e40: 0000 da05 5f62 6173 6572 0500 0000 7206  ...._baser....r.
+00000e50: 0000 00da 1a69 6e63 6570 7469 6f6e 7265  .....inceptionre
+00000e60: 736e 6574 7632 5f65 6e63 6f64 6572 7372  snetv2_encodersr
+00000e70: 1e00 0000 721e 0000 0072 1e00 0000 721f  ....r....r....r.
+00000e80: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000e90: 0073 1600 0000 0419 0c01 0c01 0c02 0c03  .s..............
+00000ea0: 1234 0201 0201 0601 08fd 04ff            .4..........
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/inceptionresnetv2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/inceptionv4.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/inceptionv4.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/inceptionv4.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/inceptionv4.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:20 2023 UTC, .py size: 3544 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -121,109 +121,108 @@
 00000780: 6eda 0643 6f6e 7632 64da 0b6b 6572 6e65  n..Conv2d..kerne
 00000790: 6c5f 7369 7a65 da07 7061 6464 696e 67da  l_size..padding.
 000007a0: 094d 6178 506f 6f6c 3264 da0b 6c61 7374  .MaxPool2d..last
 000007b0: 5f6c 696e 6561 7229 06da 0473 656c 66da  _linear)...self.
 000007c0: 0a73 7461 6765 5f69 6478 73da 0c6f 7574  .stage_idxs..out
 000007d0: 5f63 6861 6e6e 656c 73da 0564 6570 7468  _channels..depth
 000007e0: da06 6b77 6172 6773 da01 6da9 01da 095f  ..kwargs..m...._
-000007f0: 5f63 6c61 7373 5f5f a900 fa5b 433a 5c55  _class__...[C:\U
+000007f0: 5f63 6c61 7373 5f5f a900 fa4e 633a 5c55  _class__...Nc:\U
 00000800: 7365 7273 5c6d 6861 6e61 6e5c 446f 776e  sers\mhanan\Down
-00000810: 6c6f 6164 735c 4861 6e61 6e5c 4d61 6d6d  loads\Hanan\Mamm
-00000820: 6f50 795c 6d61 6d6d 6f70 795c 7365 676d  oPy\mammopy\segm
-00000830: 656e 7461 7469 6f6e 5f6d 6f64 656c 735c  entation_models\
-00000840: 656e 636f 6465 7273 5c69 6e63 6570 7469  encoders\incepti
-00000850: 6f6e 7634 2e70 7972 0b00 0000 2200 0000  onv4.pyr...."...
-00000860: 7318 0000 0000 010e 0106 0106 0106 0106  s...............
-00000870: 030c 010c 010a 0106 010c 0108 037a 1b49  .............z.I
-00000880: 6e63 6570 7469 6f6e 5634 456e 636f 6465  nceptionV4Encode
-00000890: 722e 5f5f 696e 6974 5f5f 6303 0000 0000  r.__init__c.....
-000008a0: 0000 0000 0000 0003 0000 0002 0000 0043  ...............C
-000008b0: 0000 0073 0c00 0000 7400 6401 8301 8201  ...s....t.d.....
-000008c0: 6400 5300 2902 4e7a 5c49 6e63 6570 7469  d.S.).Nz\Incepti
-000008d0: 6f6e 5634 2065 6e63 6f64 6572 2064 6f65  onV4 encoder doe
-000008e0: 7320 6e6f 7420 7375 7070 6f72 7420 6469  s not support di
-000008f0: 6c61 7465 6420 6d6f 6465 2064 7565 2074  lated mode due t
-00000900: 6f20 706f 6f6c 696e 6720 6f70 6572 6174  o pooling operat
-00000910: 696f 6e20 666f 7220 646f 776e 7361 6d70  ion for downsamp
-00000920: 6c69 6e67 2129 01da 0a56 616c 7565 4572  ling!)...ValueEr
-00000930: 726f 7229 0372 1800 0000 da0a 7374 6167  ror).r......stag
-00000940: 655f 6c69 7374 da0d 6469 6c61 7469 6f6e  e_list..dilation
-00000950: 5f6c 6973 7472 2000 0000 7220 0000 0072  _listr ...r ...r
-00000960: 2100 0000 da0c 6d61 6b65 5f64 696c 6174  !.....make_dilat
-00000970: 6564 3400 0000 7302 0000 0000 017a 1f49  ed4...s......z.I
-00000980: 6e63 6570 7469 6f6e 5634 456e 636f 6465  nceptionV4Encode
-00000990: 722e 6d61 6b65 5f64 696c 6174 6564 6301  r.make_dilatedc.
-000009a0: 0000 0000 0000 0000 0000 0001 0000 0008  ................
-000009b0: 0000 0043 0000 0073 7600 0000 7400 a001  ...C...sv...t...
-000009c0: a100 7c00 6a02 6400 7c00 6a03 6401 1900  ..|.j.d.|.j.d...
-000009d0: 8502 1900 7c00 6a02 7c00 6a03 6401 1900  ....|.j.|.j.d...
-000009e0: 7c00 6a03 6402 1900 8502 1900 7c00 6a02  |.j.d.......|.j.
-000009f0: 7c00 6a03 6402 1900 7c00 6a03 6403 1900  |.j.d...|.j.d...
-00000a00: 8502 1900 7c00 6a02 7c00 6a03 6403 1900  ....|.j.|.j.d...
-00000a10: 7c00 6a03 6404 1900 8502 1900 7c00 6a02  |.j.d.......|.j.
-00000a20: 7c00 6a03 6404 1900 6400 8502 1900 6706  |.j.d...d.....g.
-00000a30: 5300 2905 4e72 0100 0000 7205 0000 00e9  S.).Nr....r.....
-00000a40: 0200 0000 7209 0000 0029 0472 1200 0000  ....r....).r....
-00000a50: da08 4964 656e 7469 7479 da08 6665 6174  ..Identity..feat
-00000a60: 7572 6573 720c 0000 0029 0172 1800 0000  uresr....).r....
-00000a70: 7220 0000 0072 2000 0000 7221 0000 00da  r ...r ...r!....
-00000a80: 0a67 6574 5f73 7461 6765 7338 0000 0073  .get_stages8...s
-00000a90: 0e00 0000 0002 0601 1201 1801 1801 1801  ................
-00000aa0: 12fa 7a1d 496e 6365 7074 696f 6e56 3445  ..z.InceptionV4E
-00000ab0: 6e63 6f64 6572 2e67 6574 5f73 7461 6765  ncoder.get_stage
-00000ac0: 7363 0200 0000 0000 0000 0000 0000 0500  sc..............
-00000ad0: 0000 0400 0000 4300 0000 733a 0000 007c  ......C...s:...|
-00000ae0: 00a0 00a1 007d 0267 007d 0374 017c 006a  .....}.g.}.t.|.j
-00000af0: 0264 0117 0083 0144 005d 1a7d 047c 027c  .d.....D.].}.|.|
-00000b00: 0419 007c 0183 017d 017c 03a0 037c 01a1  ...|...}.|...|..
-00000b10: 0101 0071 1a7c 0353 0029 024e 7205 0000  ...q.|.S.).Nr...
-00000b20: 0029 0472 2900 0000 da05 7261 6e67 6572  .).r).....ranger
-00000b30: 0e00 0000 da06 6170 7065 6e64 2905 7218  ......append).r.
-00000b40: 0000 00da 0178 da06 7374 6167 6573 7228  .....x..stagesr(
-00000b50: 0000 00da 0169 7220 0000 0072 2000 0000  .....ir ...r ...
-00000b60: 7221 0000 00da 0766 6f72 7761 7264 4200  r!.....forwardB.
-00000b70: 0000 730c 0000 0000 0208 0204 0112 010c  ..s.............
-00000b80: 010c 027a 1a49 6e63 6570 7469 6f6e 5634  ...z.InceptionV4
-00000b90: 456e 636f 6465 722e 666f 7277 6172 6463  Encoder.forwardc
-00000ba0: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-00000bb0: 0300 0000 0b00 0000 7328 0000 007c 01a0  ........s(...|..
-00000bc0: 0064 01a1 0101 007c 01a0 0064 02a1 0101  .d.....|...d....
-00000bd0: 0074 0183 006a 027c 0166 017c 028e 0101  .t...j.|.f.|....
-00000be0: 0064 0053 0029 034e 7a10 6c61 7374 5f6c  .d.S.).Nz.last_l
-00000bf0: 696e 6561 722e 6269 6173 7a12 6c61 7374  inear.biasz.last
-00000c00: 5f6c 696e 6561 722e 7765 6967 6874 2903  _linear.weight).
-00000c10: da03 706f 7072 0a00 0000 da0f 6c6f 6164  ..popr......load
-00000c20: 5f73 7461 7465 5f64 6963 7429 0372 1800  _state_dict).r..
-00000c30: 0000 da0a 7374 6174 655f 6469 6374 721c  ....state_dictr.
-00000c40: 0000 0072 1e00 0000 7220 0000 0072 2100  ...r....r ...r!.
-00000c50: 0000 7231 0000 004d 0000 0073 0600 0000  ..r1...M...s....
-00000c60: 0001 0a01 0a01 7a22 496e 6365 7074 696f  ......z"Inceptio
-00000c70: 6e56 3445 6e63 6f64 6572 2e6c 6f61 645f  nV4Encoder.load_
-00000c80: 7374 6174 655f 6469 6374 2901 7208 0000  state_dict).r...
-00000c90: 0029 09da 085f 5f6e 616d 655f 5fda 0a5f  .)...__name__.._
-00000ca0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00000cb0: 6c6e 616d 655f 5f72 0b00 0000 7225 0000  lname__r....r%..
-00000cc0: 0072 2900 0000 722f 0000 0072 3100 0000  .r)...r/...r1...
-00000cd0: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
-00000ce0: 2000 0000 7220 0000 0072 1e00 0000 7221   ...r ...r....r!
-00000cf0: 0000 0072 0700 0000 2100 0000 730a 0000  ...r....!...s...
-00000d00: 0008 010e 1208 0408 0a08 0b72 0700 0000  ...........r....
-00000d10: da0b 696e 6365 7074 696f 6e76 3429 0472  ..inceptionv4).r
-00000d20: 0900 0000 7208 0000 00e9 0900 0000 e90f  ....r...........
-00000d30: 0000 0029 0672 0900 0000 e940 0000 00e9  ...).r.....@....
-00000d40: c000 0000 6980 0100 0069 0004 0000 6900  ....i....i....i.
-00000d50: 0600 0069 e903 0000 2903 7219 0000 0072  ...i....).r....r
-00000d60: 1a00 0000 da0b 6e75 6d5f 636c 6173 7365  ......num_classe
-00000d70: 7329 03da 0765 6e63 6f64 6572 7204 0000  s)...encoderr...
-00000d80: 00da 0670 6172 616d 7329 0bda 075f 5f64  ...params)...__d
-00000d90: 6f63 5f5f da08 746f 7263 682e 6e6e 7212  oc__..torch.nnr.
-00000da0: 0000 005a 2370 7265 7472 6169 6e65 646d  ...Z#pretrainedm
-00000db0: 6f64 656c 732e 6d6f 6465 6c73 2e69 6e63  odels.models.inc
-00000dc0: 6570 7469 6f6e 7634 7202 0000 0072 0300  eptionv4r....r..
-00000dd0: 0000 7204 0000 00da 055f 6261 7365 7206  ..r......_baser.
-00000de0: 0000 0072 0700 0000 da14 696e 6365 7074  ...r......incept
-00000df0: 696f 6e76 345f 656e 636f 6465 7273 7220  ionv4_encodersr 
-00000e00: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
-00000e10: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000e20: 731c 0000 0004 190c 0110 010c 020c 0312  s...............
-00000e30: 3302 0102 0106 0202 0102 0102 fd04 fd04  3...............
-00000e40: ff                                       .
+00000810: 6c6f 6164 735c 4861 6e61 6e5c 6d67 5c73  loads\Hanan\mg\s
+00000820: 6567 6d65 6e74 6174 696f 6e5f 6d6f 6465  egmentation_mode
+00000830: 6c73 5c65 6e63 6f64 6572 735c 696e 6365  ls\encoders\ince
+00000840: 7074 696f 6e76 342e 7079 720b 0000 0022  ptionv4.pyr...."
+00000850: 0000 0073 1800 0000 0001 0e01 0601 0601  ...s............
+00000860: 0601 0603 0c01 0c01 0a01 0601 0c01 0803  ................
+00000870: 7a1b 496e 6365 7074 696f 6e56 3445 6e63  z.InceptionV4Enc
+00000880: 6f64 6572 2e5f 5f69 6e69 745f 5f63 0300  oder.__init__c..
+00000890: 0000 0000 0000 0000 0000 0300 0000 0200  ................
+000008a0: 0000 4300 0000 730c 0000 0074 0064 0183  ..C...s....t.d..
+000008b0: 0182 0164 0053 0029 024e 7a5c 496e 6365  ...d.S.).Nz\Ince
+000008c0: 7074 696f 6e56 3420 656e 636f 6465 7220  ptionV4 encoder 
+000008d0: 646f 6573 206e 6f74 2073 7570 706f 7274  does not support
+000008e0: 2064 696c 6174 6564 206d 6f64 6520 6475   dilated mode du
+000008f0: 6520 746f 2070 6f6f 6c69 6e67 206f 7065  e to pooling ope
+00000900: 7261 7469 6f6e 2066 6f72 2064 6f77 6e73  ration for downs
+00000910: 616d 706c 696e 6721 2901 da0a 5661 6c75  ampling!)...Valu
+00000920: 6545 7272 6f72 2903 7218 0000 00da 0a73  eError).r......s
+00000930: 7461 6765 5f6c 6973 74da 0d64 696c 6174  tage_list..dilat
+00000940: 696f 6e5f 6c69 7374 7220 0000 0072 2000  ion_listr ...r .
+00000950: 0000 7221 0000 00da 0c6d 616b 655f 6469  ..r!.....make_di
+00000960: 6c61 7465 6434 0000 0073 0200 0000 0001  lated4...s......
+00000970: 7a1f 496e 6365 7074 696f 6e56 3445 6e63  z.InceptionV4Enc
+00000980: 6f64 6572 2e6d 616b 655f 6469 6c61 7465  oder.make_dilate
+00000990: 6463 0100 0000 0000 0000 0000 0000 0100  dc..............
+000009a0: 0000 0800 0000 4300 0000 7376 0000 0074  ......C...sv...t
+000009b0: 00a0 01a1 007c 006a 0264 007c 006a 0364  .....|.j.d.|.j.d
+000009c0: 0119 0085 0219 007c 006a 027c 006a 0364  .......|.j.|.j.d
+000009d0: 0119 007c 006a 0364 0219 0085 0219 007c  ...|.j.d.......|
+000009e0: 006a 027c 006a 0364 0219 007c 006a 0364  .j.|.j.d...|.j.d
+000009f0: 0319 0085 0219 007c 006a 027c 006a 0364  .......|.j.|.j.d
+00000a00: 0319 007c 006a 0364 0419 0085 0219 007c  ...|.j.d.......|
+00000a10: 006a 027c 006a 0364 0419 0064 0085 0219  .j.|.j.d...d....
+00000a20: 0067 0653 0029 054e 7201 0000 0072 0500  .g.S.).Nr....r..
+00000a30: 0000 e902 0000 0072 0900 0000 2904 7212  .......r....).r.
+00000a40: 0000 00da 0849 6465 6e74 6974 79da 0866  .....Identity..f
+00000a50: 6561 7475 7265 7372 0c00 0000 2901 7218  eaturesr....).r.
+00000a60: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
+00000a70: 0000 da0a 6765 745f 7374 6167 6573 3800  ....get_stages8.
+00000a80: 0000 730e 0000 0000 0206 0112 0118 0118  ..s.............
+00000a90: 0118 0112 fa7a 1d49 6e63 6570 7469 6f6e  .....z.Inception
+00000aa0: 5634 456e 636f 6465 722e 6765 745f 7374  V4Encoder.get_st
+00000ab0: 6167 6573 6302 0000 0000 0000 0000 0000  agesc...........
+00000ac0: 0005 0000 0004 0000 0043 0000 0073 3a00  .........C...s:.
+00000ad0: 0000 7c00 a000 a100 7d02 6700 7d03 7401  ..|.....}.g.}.t.
+00000ae0: 7c00 6a02 6401 1700 8301 4400 5d1a 7d04  |.j.d.....D.].}.
+00000af0: 7c02 7c04 1900 7c01 8301 7d01 7c03 a003  |.|...|...}.|...
+00000b00: 7c01 a101 0100 711a 7c03 5300 2902 4e72  |.....q.|.S.).Nr
+00000b10: 0500 0000 2904 7229 0000 00da 0572 616e  ....).r).....ran
+00000b20: 6765 720e 0000 00da 0661 7070 656e 6429  ger......append)
+00000b30: 0572 1800 0000 da01 78da 0673 7461 6765  .r......x..stage
+00000b40: 7372 2800 0000 da01 6972 2000 0000 7220  sr(.....ir ...r 
+00000b50: 0000 0072 2100 0000 da07 666f 7277 6172  ...r!.....forwar
+00000b60: 6442 0000 0073 0c00 0000 0002 0802 0401  dB...s..........
+00000b70: 1201 0c01 0c02 7a1a 496e 6365 7074 696f  ......z.Inceptio
+00000b80: 6e56 3445 6e63 6f64 6572 2e66 6f72 7761  nV4Encoder.forwa
+00000b90: 7264 6302 0000 0000 0000 0000 0000 0003  rdc.............
+00000ba0: 0000 0003 0000 000b 0000 0073 2800 0000  ...........s(...
+00000bb0: 7c01 a000 6401 a101 0100 7c01 a000 6402  |...d.....|...d.
+00000bc0: a101 0100 7401 8300 6a02 7c01 6601 7c02  ....t...j.|.f.|.
+00000bd0: 8e01 0100 6400 5300 2903 4e7a 106c 6173  ....d.S.).Nz.las
+00000be0: 745f 6c69 6e65 6172 2e62 6961 737a 126c  t_linear.biasz.l
+00000bf0: 6173 745f 6c69 6e65 6172 2e77 6569 6768  ast_linear.weigh
+00000c00: 7429 03da 0370 6f70 720a 0000 00da 0f6c  t)...popr......l
+00000c10: 6f61 645f 7374 6174 655f 6469 6374 2903  oad_state_dict).
+00000c20: 7218 0000 00da 0a73 7461 7465 5f64 6963  r......state_dic
+00000c30: 7472 1c00 0000 721e 0000 0072 2000 0000  tr....r....r ...
+00000c40: 7221 0000 0072 3100 0000 4d00 0000 7306  r!...r1...M...s.
+00000c50: 0000 0000 010a 010a 017a 2249 6e63 6570  .........z"Incep
+00000c60: 7469 6f6e 5634 456e 636f 6465 722e 6c6f  tionV4Encoder.lo
+00000c70: 6164 5f73 7461 7465 5f64 6963 7429 0172  ad_state_dict).r
+00000c80: 0800 0000 2909 da08 5f5f 6e61 6d65 5f5f  ....)...__name__
+00000c90: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000ca0: 7175 616c 6e61 6d65 5f5f 720b 0000 0072  qualname__r....r
+00000cb0: 2500 0000 7229 0000 0072 2f00 0000 7231  %...r)...r/...r1
+00000cc0: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
+00000cd0: 5f5f 7220 0000 0072 2000 0000 721e 0000  __r ...r ...r...
+00000ce0: 0072 2100 0000 7207 0000 0021 0000 0073  .r!...r....!...s
+00000cf0: 0a00 0000 0801 0e12 0804 080a 080b 7207  ..............r.
+00000d00: 0000 00da 0b69 6e63 6570 7469 6f6e 7634  .....inceptionv4
+00000d10: 2904 7209 0000 0072 0800 0000 e909 0000  ).r....r........
+00000d20: 00e9 0f00 0000 2906 7209 0000 00e9 4000  ......).r.....@.
+00000d30: 0000 e9c0 0000 0069 8001 0000 6900 0400  .......i....i...
+00000d40: 0069 0006 0000 69e9 0300 0029 0372 1900  .i....i....).r..
+00000d50: 0000 721a 0000 00da 0b6e 756d 5f63 6c61  ..r......num_cla
+00000d60: 7373 6573 2903 da07 656e 636f 6465 7272  sses)...encoderr
+00000d70: 0400 0000 da06 7061 7261 6d73 290b da07  ......params)...
+00000d80: 5f5f 646f 635f 5fda 0874 6f72 6368 2e6e  __doc__..torch.n
+00000d90: 6e72 1200 0000 5a23 7072 6574 7261 696e  nr....Z#pretrain
+00000da0: 6564 6d6f 6465 6c73 2e6d 6f64 656c 732e  edmodels.models.
+00000db0: 696e 6365 7074 696f 6e76 3472 0200 0000  inceptionv4r....
+00000dc0: 7203 0000 0072 0400 0000 da05 5f62 6173  r....r......_bas
+00000dd0: 6572 0600 0000 7207 0000 00da 1469 6e63  er....r......inc
+00000de0: 6570 7469 6f6e 7634 5f65 6e63 6f64 6572  eptionv4_encoder
+00000df0: 7372 2000 0000 7220 0000 0072 2000 0000  sr ...r ...r ...
+00000e00: 7221 0000 00da 083c 6d6f 6475 6c65 3e01  r!.....<module>.
+00000e10: 0000 0073 1c00 0000 0419 0c01 1001 0c02  ...s............
+00000e20: 0c03 1233 0201 0201 0602 0201 0201 02fd  ...3............
+00000e30: 04fd 04ff                                ....
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/inceptionv4.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/inceptionv4.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/mobilenet.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/mobilenet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/mobilenet.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/mobilenet.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/mobilenet.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/mobilenet.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/mobilenet.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/mobilenet.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:20 2023 UTC, .py size: 2933 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -106,96 +106,96 @@
 00000690: 4ee9 0300 0000 2906 da05 7375 7065 72da  N.....)...super.
 000006a0: 085f 5f69 6e69 745f 5fda 065f 6465 7074  .__init__.._dept
 000006b0: 68da 0d5f 6f75 745f 6368 616e 6e65 6c73  h.._out_channels
 000006c0: da0c 5f69 6e5f 6368 616e 6e65 6c73 da0a  .._in_channels..
 000006d0: 636c 6173 7369 6669 6572 2904 da04 7365  classifier)...se
 000006e0: 6c66 da0c 6f75 745f 6368 616e 6e65 6c73  lf..out_channels
 000006f0: da05 6465 7074 68da 066b 7761 7267 73a9  ..depth..kwargs.
-00000700: 01da 095f 5f63 6c61 7373 5f5f a900 fa59  ...__class__...Y
-00000710: 433a 5c55 7365 7273 5c6d 6861 6e61 6e5c  C:\Users\mhanan\
+00000700: 01da 095f 5f63 6c61 7373 5f5f a900 fa4c  ...__class__...L
+00000710: 633a 5c55 7365 7273 5c6d 6861 6e61 6e5c  c:\Users\mhanan\
 00000720: 446f 776e 6c6f 6164 735c 4861 6e61 6e5c  Downloads\Hanan\
-00000730: 4d61 6d6d 6f50 795c 6d61 6d6d 6f70 795c  MammoPy\mammopy\
-00000740: 7365 676d 656e 7461 7469 6f6e 5f6d 6f64  segmentation_mod
-00000750: 656c 735c 656e 636f 6465 7273 5c6d 6f62  els\encoders\mob
-00000760: 696c 656e 6574 2e70 7972 0800 0000 2200  ilenet.pyr....".
-00000770: 0000 730a 0000 0000 010e 0106 0106 0106  ..s.............
-00000780: 017a 1b4d 6f62 696c 654e 6574 5632 456e  .z.MobileNetV2En
-00000790: 636f 6465 722e 5f5f 696e 6974 5f5f 6301  coder.__init__c.
-000007a0: 0000 0000 0000 0000 0000 0001 0000 0008  ................
-000007b0: 0000 0043 0000 0073 4600 0000 7400 a001  ...C...sF...t...
-000007c0: a100 7c00 6a02 6400 6401 8502 1900 7c00  ..|.j.d.d.....|.
-000007d0: 6a02 6401 6402 8502 1900 7c00 6a02 6402  j.d.d.....|.j.d.
-000007e0: 6403 8502 1900 7c00 6a02 6403 6404 8502  d.....|.j.d.d...
-000007f0: 1900 7c00 6a02 6404 6400 8502 1900 6706  ..|.j.d.d.....g.
-00000800: 5300 2905 4ee9 0200 0000 e904 0000 00e9  S.).N...........
-00000810: 0700 0000 e90e 0000 0029 03da 026e 6eda  .........)...nn.
-00000820: 0849 6465 6e74 6974 79da 0866 6561 7475  .Identity..featu
-00000830: 7265 7329 0172 0d00 0000 7213 0000 0072  res).r....r....r
-00000840: 1300 0000 7214 0000 00da 0a67 6574 5f73  ....r......get_s
-00000850: 7461 6765 7329 0000 0073 0e00 0000 0002  tages)...s......
-00000860: 0601 0c01 0c01 0c01 0c01 0cfa 7a1d 4d6f  ............z.Mo
-00000870: 6269 6c65 4e65 7456 3245 6e63 6f64 6572  bileNetV2Encoder
-00000880: 2e67 6574 5f73 7461 6765 7363 0200 0000  .get_stagesc....
-00000890: 0000 0000 0000 0000 0500 0000 0400 0000  ................
-000008a0: 4300 0000 733a 0000 007c 00a0 00a1 007d  C...s:...|.....}
-000008b0: 0267 007d 0374 017c 006a 0264 0117 0083  .g.}.t.|.j.d....
-000008c0: 0144 005d 1a7d 047c 027c 0419 007c 0183  .D.].}.|.|...|..
-000008d0: 017d 017c 03a0 037c 01a1 0101 0071 1a7c  .}.|...|.....q.|
-000008e0: 0353 0029 024e 7202 0000 0029 0472 1c00  .S.).Nr....).r..
-000008f0: 0000 da05 7261 6e67 6572 0900 0000 da06  ....ranger......
-00000900: 6170 7065 6e64 2905 720d 0000 00da 0178  append).r......x
-00000910: da06 7374 6167 6573 721b 0000 00da 0169  ..stagesr......i
-00000920: 7213 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
-00000930: 0766 6f72 7761 7264 3300 0000 730c 0000  .forward3...s...
-00000940: 0000 0108 0204 0112 010c 010c 027a 1a4d  .............z.M
-00000950: 6f62 696c 654e 6574 5632 456e 636f 6465  obileNetV2Encode
-00000960: 722e 666f 7277 6172 6463 0200 0000 0000  r.forwardc......
-00000970: 0000 0000 0000 0300 0000 0300 0000 0b00  ................
-00000980: 0000 7328 0000 007c 01a0 0064 01a1 0101  ..s(...|...d....
-00000990: 007c 01a0 0064 02a1 0101 0074 0183 006a  .|...d.....t...j
-000009a0: 027c 0166 017c 028e 0101 0064 0053 0029  .|.f.|.....d.S.)
-000009b0: 034e 7a11 636c 6173 7369 6669 6572 2e31  .Nz.classifier.1
-000009c0: 2e62 6961 737a 1363 6c61 7373 6966 6965  .biasz.classifie
-000009d0: 722e 312e 7765 6967 6874 2903 da03 706f  r.1.weight)...po
-000009e0: 7072 0700 0000 da0f 6c6f 6164 5f73 7461  pr......load_sta
-000009f0: 7465 5f64 6963 7429 0372 0d00 0000 da0a  te_dict).r......
-00000a00: 7374 6174 655f 6469 6374 7210 0000 0072  state_dictr....r
-00000a10: 1100 0000 7213 0000 0072 1400 0000 7224  ....r....r....r$
-00000a20: 0000 003d 0000 0073 0600 0000 0001 0a01  ...=...s........
-00000a30: 0a01 7a22 4d6f 6269 6c65 4e65 7456 3245  ..z"MobileNetV2E
-00000a40: 6e63 6f64 6572 2e6c 6f61 645f 7374 6174  ncoder.load_stat
-00000a50: 655f 6469 6374 2901 7205 0000 0029 08da  e_dict).r....)..
-00000a60: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000a70: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000a80: 655f 5f72 0800 0000 721c 0000 0072 2200  e__r....r....r".
-00000a90: 0000 7224 0000 00da 0d5f 5f63 6c61 7373  ..r$.....__class
-00000aa0: 6365 6c6c 5f5f 7213 0000 0072 1300 0000  cell__r....r....
-00000ab0: 7211 0000 0072 1400 0000 7204 0000 0020  r....r....r.... 
-00000ac0: 0000 0073 0800 0000 0802 0e07 080a 080a  ...s............
-00000ad0: 7204 0000 00da 0c6d 6f62 696c 656e 6574  r......mobilenet
-00000ae0: 5f76 32da 0869 6d61 6765 6e65 7467 0ad7  _v2..imagenetg..
-00000af0: a370 3d0a df3f 67c9 76be 9f1a 2fdd 3f67  .p=..?g.v.../.?g
-00000b00: 9643 8b6c e7fb d93f 671d 5a64 3bdf 4fcd  .C.l...?g.Zd;.O.
-00000b10: 3f67 79e9 2631 08ac cc3f 67cd cccc cccc  ?gy.&1...?g.....
-00000b20: cccc 3f7a 3d68 7474 7073 3a2f 2f64 6f77  ..?z=https://dow
-00000b30: 6e6c 6f61 642e 7079 746f 7263 682e 6f72  nload.pytorch.or
-00000b40: 672f 6d6f 6465 6c73 2f6d 6f62 696c 656e  g/models/mobilen
-00000b50: 6574 5f76 322d 6230 3335 3331 3034 2e70  et_v2-b0353104.p
-00000b60: 7468 da03 5247 4229 05da 046d 6561 6eda  th..RGB)...mean.
-00000b70: 0373 7464 da03 7572 6cda 0b69 6e70 7574  .std..url..input
-00000b80: 5f73 7061 6365 da0b 696e 7075 745f 7261  _space..input_ra
-00000b90: 6e67 6572 0e00 0000 2906 7206 0000 00e9  nger....).r.....
-00000ba0: 1000 0000 e918 0000 00e9 2000 0000 e960  .......... ....`
-00000bb0: 0000 0069 0005 0000 2903 da07 656e 636f  ...i....)...enco
-00000bc0: 6465 72da 1370 7265 7472 6169 6e65 645f  der..pretrained_
-00000bd0: 7365 7474 696e 6773 da06 7061 7261 6d73  settings..params
-00000be0: 290a da07 5f5f 646f 635f 5fda 0b74 6f72  )...__doc__..tor
-00000bf0: 6368 7669 7369 6f6e da08 746f 7263 682e  chvision..torch.
-00000c00: 6e6e 7219 0000 00da 055f 6261 7365 7203  nnr......_baser.
-00000c10: 0000 00da 066d 6f64 656c 73da 0b4d 6f62  .....models..Mob
-00000c20: 696c 654e 6574 5632 7204 0000 00da 126d  ileNetV2r......m
-00000c30: 6f62 696c 656e 6574 5f65 6e63 6f64 6572  obilenet_encoder
-00000c40: 7372 1300 0000 7213 0000 0072 1300 0000  sr....r....r....
-00000c50: 7214 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000c60: 0000 0073 2600 0000 0419 0801 0c02 0c03  ...s&...........
-00000c70: 1624 0201 0202 0201 0801 0801 0201 0201  .$..............
-00000c80: 06fb 04ff 020a 0200 02ff 02f5 04ff       ..............
+00000730: 6d67 5c73 6567 6d65 6e74 6174 696f 6e5f  mg\segmentation_
+00000740: 6d6f 6465 6c73 5c65 6e63 6f64 6572 735c  models\encoders\
+00000750: 6d6f 6269 6c65 6e65 742e 7079 7208 0000  mobilenet.pyr...
+00000760: 0022 0000 0073 0a00 0000 0001 0e01 0601  ."...s..........
+00000770: 0601 0601 7a1b 4d6f 6269 6c65 4e65 7456  ....z.MobileNetV
+00000780: 3245 6e63 6f64 6572 2e5f 5f69 6e69 745f  2Encoder.__init_
+00000790: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
+000007a0: 0000 0800 0000 4300 0000 7346 0000 0074  ......C...sF...t
+000007b0: 00a0 01a1 007c 006a 0264 0064 0185 0219  .....|.j.d.d....
+000007c0: 007c 006a 0264 0164 0285 0219 007c 006a  .|.j.d.d.....|.j
+000007d0: 0264 0264 0385 0219 007c 006a 0264 0364  .d.d.....|.j.d.d
+000007e0: 0485 0219 007c 006a 0264 0464 0085 0219  .....|.j.d.d....
+000007f0: 0067 0653 0029 054e e902 0000 00e9 0400  .g.S.).N........
+00000800: 0000 e907 0000 00e9 0e00 0000 2903 da02  ............)...
+00000810: 6e6e da08 4964 656e 7469 7479 da08 6665  nn..Identity..fe
+00000820: 6174 7572 6573 2901 720d 0000 0072 1300  atures).r....r..
+00000830: 0000 7213 0000 0072 1400 0000 da0a 6765  ..r....r......ge
+00000840: 745f 7374 6167 6573 2900 0000 730e 0000  t_stages)...s...
+00000850: 0000 0206 010c 010c 010c 010c 010c fa7a  ...............z
+00000860: 1d4d 6f62 696c 654e 6574 5632 456e 636f  .MobileNetV2Enco
+00000870: 6465 722e 6765 745f 7374 6167 6573 6302  der.get_stagesc.
+00000880: 0000 0000 0000 0000 0000 0005 0000 0004  ................
+00000890: 0000 0043 0000 0073 3a00 0000 7c00 a000  ...C...s:...|...
+000008a0: a100 7d02 6700 7d03 7401 7c00 6a02 6401  ..}.g.}.t.|.j.d.
+000008b0: 1700 8301 4400 5d1a 7d04 7c02 7c04 1900  ....D.].}.|.|...
+000008c0: 7c01 8301 7d01 7c03 a003 7c01 a101 0100  |...}.|...|.....
+000008d0: 711a 7c03 5300 2902 4e72 0200 0000 2904  q.|.S.).Nr....).
+000008e0: 721c 0000 00da 0572 616e 6765 7209 0000  r......ranger...
+000008f0: 00da 0661 7070 656e 6429 0572 0d00 0000  ...append).r....
+00000900: da01 78da 0673 7461 6765 7372 1b00 0000  ..x..stagesr....
+00000910: da01 6972 1300 0000 7213 0000 0072 1400  ..ir....r....r..
+00000920: 0000 da07 666f 7277 6172 6433 0000 0073  ....forward3...s
+00000930: 0c00 0000 0001 0802 0401 1201 0c01 0c02  ................
+00000940: 7a1a 4d6f 6269 6c65 4e65 7456 3245 6e63  z.MobileNetV2Enc
+00000950: 6f64 6572 2e66 6f72 7761 7264 6302 0000  oder.forwardc...
+00000960: 0000 0000 0000 0000 0003 0000 0003 0000  ................
+00000970: 000b 0000 0073 2800 0000 7c01 a000 6401  .....s(...|...d.
+00000980: a101 0100 7c01 a000 6402 a101 0100 7401  ....|...d.....t.
+00000990: 8300 6a02 7c01 6601 7c02 8e01 0100 6400  ..j.|.f.|.....d.
+000009a0: 5300 2903 4e7a 1163 6c61 7373 6966 6965  S.).Nz.classifie
+000009b0: 722e 312e 6269 6173 7a13 636c 6173 7369  r.1.biasz.classi
+000009c0: 6669 6572 2e31 2e77 6569 6768 7429 03da  fier.1.weight)..
+000009d0: 0370 6f70 7207 0000 00da 0f6c 6f61 645f  .popr......load_
+000009e0: 7374 6174 655f 6469 6374 2903 720d 0000  state_dict).r...
+000009f0: 00da 0a73 7461 7465 5f64 6963 7472 1000  ...state_dictr..
+00000a00: 0000 7211 0000 0072 1300 0000 7214 0000  ..r....r....r...
+00000a10: 0072 2400 0000 3d00 0000 7306 0000 0000  .r$...=...s.....
+00000a20: 010a 010a 017a 224d 6f62 696c 654e 6574  .....z"MobileNet
+00000a30: 5632 456e 636f 6465 722e 6c6f 6164 5f73  V2Encoder.load_s
+00000a40: 7461 7465 5f64 6963 7429 0172 0500 0000  tate_dict).r....
+00000a50: 2908 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00000a60: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00000a70: 6e61 6d65 5f5f 7208 0000 0072 1c00 0000  name__r....r....
+00000a80: 7222 0000 0072 2400 0000 da0d 5f5f 636c  r"...r$.....__cl
+00000a90: 6173 7363 656c 6c5f 5f72 1300 0000 7213  asscell__r....r.
+00000aa0: 0000 0072 1100 0000 7214 0000 0072 0400  ...r....r....r..
+00000ab0: 0000 2000 0000 7308 0000 0008 020e 0708  .. ...s.........
+00000ac0: 0a08 0a72 0400 0000 da0c 6d6f 6269 6c65  ...r......mobile
+00000ad0: 6e65 745f 7632 da08 696d 6167 656e 6574  net_v2..imagenet
+00000ae0: 670a d7a3 703d 0adf 3f67 c976 be9f 1a2f  g...p=..?g.v.../
+00000af0: dd3f 6796 438b 6ce7 fbd9 3f67 1d5a 643b  .?g.C.l...?g.Zd;
+00000b00: df4f cd3f 6779 e926 3108 accc 3f67 cdcc  .O.?gy.&1...?g..
+00000b10: cccc cccc cc3f 7a3d 6874 7470 733a 2f2f  .....?z=https://
+00000b20: 646f 776e 6c6f 6164 2e70 7974 6f72 6368  download.pytorch
+00000b30: 2e6f 7267 2f6d 6f64 656c 732f 6d6f 6269  .org/models/mobi
+00000b40: 6c65 6e65 745f 7632 2d62 3033 3533 3130  lenet_v2-b035310
+00000b50: 342e 7074 68da 0352 4742 2905 da04 6d65  4.pth..RGB)...me
+00000b60: 616e da03 7374 64da 0375 726c da0b 696e  an..std..url..in
+00000b70: 7075 745f 7370 6163 65da 0b69 6e70 7574  put_space..input
+00000b80: 5f72 616e 6765 720e 0000 0029 0672 0600  _ranger....).r..
+00000b90: 0000 e910 0000 00e9 1800 0000 e920 0000  ............. ..
+00000ba0: 00e9 6000 0000 6900 0500 0029 03da 0765  ..`...i....)...e
+00000bb0: 6e63 6f64 6572 da13 7072 6574 7261 696e  ncoder..pretrain
+00000bc0: 6564 5f73 6574 7469 6e67 73da 0670 6172  ed_settings..par
+00000bd0: 616d 7329 0ada 075f 5f64 6f63 5f5f da0b  ams)...__doc__..
+00000be0: 746f 7263 6876 6973 696f 6eda 0874 6f72  torchvision..tor
+00000bf0: 6368 2e6e 6e72 1900 0000 da05 5f62 6173  ch.nnr......_bas
+00000c00: 6572 0300 0000 da06 6d6f 6465 6c73 da0b  er......models..
+00000c10: 4d6f 6269 6c65 4e65 7456 3272 0400 0000  MobileNetV2r....
+00000c20: da12 6d6f 6269 6c65 6e65 745f 656e 636f  ..mobilenet_enco
+00000c30: 6465 7273 7213 0000 0072 1300 0000 7213  dersr....r....r.
+00000c40: 0000 0072 1400 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000c50: 653e 0100 0000 7326 0000 0004 1908 010c  e>....s&........
+00000c60: 020c 0316 2402 0102 0202 0108 0108 0102  ....$...........
+00000c70: 0102 0106 fb04 ff02 0a02 0002 ff02 f504  ................
+00000c80: ff                                       .
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/mobilenet.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/mobilenet.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/resnet.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/resnet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/resnet.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/resnet.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/resnet.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/resnet.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/resnet.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/resnet.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:20 2023 UTC, .py size: 9265 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -145,252 +145,251 @@
 00000900: 72da 085f 5f69 6e69 745f 5fda 065f 6465  r..__init__.._de
 00000910: 7074 685a 0d5f 6f75 745f 6368 616e 6e65  pthZ._out_channe
 00000920: 6c73 5a0c 5f69 6e5f 6368 616e 6e65 6c73  lsZ._in_channels
 00000930: da02 6663 da07 6176 6770 6f6f 6c29 04da  ..fc..avgpool)..
 00000940: 0473 656c 66da 0c6f 7574 5f63 6861 6e6e  .self..out_chann
 00000950: 656c 73da 0564 6570 7468 da06 6b77 6172  els..depth..kwar
 00000960: 6773 a901 da09 5f5f 636c 6173 735f 5fa9  gs....__class__.
-00000970: 00fa 5643 3a5c 5573 6572 735c 6d68 616e  ..VC:\Users\mhan
+00000970: 00fa 4963 3a5c 5573 6572 735c 6d68 616e  ..Ic:\Users\mhan
 00000980: 616e 5c44 6f77 6e6c 6f61 6473 5c48 616e  an\Downloads\Han
-00000990: 616e 5c4d 616d 6d6f 5079 5c6d 616d 6d6f  an\MammoPy\mammo
-000009a0: 7079 5c73 6567 6d65 6e74 6174 696f 6e5f  py\segmentation_
-000009b0: 6d6f 6465 6c73 5c65 6e63 6f64 6572 735c  models\encoders\
-000009c0: 7265 736e 6574 2e70 7972 0d00 0000 2600  resnet.pyr....&.
-000009d0: 0000 730c 0000 0000 010e 0106 0106 0106  ..s.............
-000009e0: 0204 017a 1652 6573 4e65 7445 6e63 6f64  ...z.ResNetEncod
-000009f0: 6572 2e5f 5f69 6e69 745f 5f63 0100 0000  er.__init__c....
-00000a00: 0000 0000 0000 0000 0100 0000 0600 0000  ................
-00000a10: 4300 0000 7336 0000 0074 00a0 01a1 0074  C...s6...t.....t
-00000a20: 00a0 027c 006a 037c 006a 047c 006a 05a1  ...|.j.|.j.|.j..
-00000a30: 0374 00a0 027c 006a 067c 006a 07a1 027c  .t...|.j.|.j...|
-00000a40: 006a 087c 006a 097c 006a 0a67 0653 0029  .j.|.j.|.j.g.S.)
-00000a50: 014e 290b da02 6e6e da08 4964 656e 7469  .N)...nn..Identi
-00000a60: 7479 da0a 5365 7175 656e 7469 616c da05  ty..Sequential..
-00000a70: 636f 6e76 31da 0362 6e31 da04 7265 6c75  conv1..bn1..relu
-00000a80: da07 6d61 7870 6f6f 6cda 066c 6179 6572  ..maxpool..layer
-00000a90: 31da 066c 6179 6572 32da 066c 6179 6572  1..layer2..layer
-00000aa0: 33da 066c 6179 6572 3429 0172 1100 0000  3..layer4).r....
-00000ab0: 7217 0000 0072 1700 0000 7218 0000 00da  r....r....r.....
-00000ac0: 0a67 6574 5f73 7461 6765 732f 0000 0073  .get_stages/...s
-00000ad0: 0e00 0000 0002 0601 1201 0e01 0401 0401  ................
-00000ae0: 04fa 7a18 5265 734e 6574 456e 636f 6465  ..z.ResNetEncode
-00000af0: 722e 6765 745f 7374 6167 6573 6302 0000  r.get_stagesc...
-00000b00: 0000 0000 0000 0000 0005 0000 0004 0000  ................
-00000b10: 0043 0000 0073 3a00 0000 7c00 a000 a100  .C...s:...|.....
-00000b20: 7d02 6700 7d03 7401 7c00 6a02 6401 1700  }.g.}.t.|.j.d...
-00000b30: 8301 4400 5d1a 7d04 7c02 7c04 1900 7c01  ..D.].}.|.|...|.
-00000b40: 8301 7d01 7c03 a003 7c01 a101 0100 711a  ..}.|...|.....q.
-00000b50: 7c03 5300 2902 4e72 0700 0000 2904 7224  |.S.).Nr....).r$
-00000b60: 0000 00da 0572 616e 6765 720e 0000 00da  .....ranger.....
-00000b70: 0661 7070 656e 6429 0572 1100 0000 da01  .append).r......
-00000b80: 785a 0673 7461 6765 73da 0866 6561 7475  xZ.stages..featu
-00000b90: 7265 73da 0169 7217 0000 0072 1700 0000  res..ir....r....
-00000ba0: 7218 0000 00da 0766 6f72 7761 7264 3900  r......forward9.
-00000bb0: 0000 730c 0000 0000 0108 0204 0112 010c  ..s.............
-00000bc0: 010c 027a 1552 6573 4e65 7445 6e63 6f64  ...z.ResNetEncod
-00000bd0: 6572 2e66 6f72 7761 7264 6302 0000 0000  er.forwardc.....
-00000be0: 0000 0000 0000 0003 0000 0003 0000 000b  ................
-00000bf0: 0000 0073 2800 0000 7c01 a000 6401 a101  ...s(...|...d...
-00000c00: 0100 7c01 a000 6402 a101 0100 7401 8300  ..|...d.....t...
-00000c10: 6a02 7c01 6601 7c02 8e01 0100 6400 5300  j.|.f.|.....d.S.
-00000c20: 2903 4e7a 0766 632e 6269 6173 7a09 6663  ).Nz.fc.biasz.fc
-00000c30: 2e77 6569 6768 7429 03da 0370 6f70 720c  .weight)...popr.
-00000c40: 0000 00da 0f6c 6f61 645f 7374 6174 655f  .....load_state_
-00000c50: 6469 6374 2903 7211 0000 00da 0a73 7461  dict).r......sta
-00000c60: 7465 5f64 6963 7472 1400 0000 7215 0000  te_dictr....r...
-00000c70: 0072 1700 0000 7218 0000 0072 2c00 0000  .r....r....r,...
-00000c80: 4300 0000 7306 0000 0000 010a 010a 017a  C...s..........z
-00000c90: 1d52 6573 4e65 7445 6e63 6f64 6572 2e6c  .ResNetEncoder.l
-00000ca0: 6f61 645f 7374 6174 655f 6469 6374 2901  oad_state_dict).
-00000cb0: 720a 0000 0029 08da 085f 5f6e 616d 655f  r....)...__name_
-00000cc0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000cd0: 5f71 7561 6c6e 616d 655f 5f72 0d00 0000  _qualname__r....
-00000ce0: 7224 0000 0072 2a00 0000 722c 0000 00da  r$...r*...r,....
-00000cf0: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7217  .__classcell__r.
-00000d00: 0000 0072 1700 0000 7215 0000 0072 1800  ...r....r....r..
-00000d10: 0000 7209 0000 0025 0000 0073 0800 0000  ..r....%...s....
-00000d20: 0801 0e09 080a 080a 7209 0000 007a 6468  ........r....zdh
-00000d30: 7474 7073 3a2f 2f64 6c2e 6662 6169 7075  ttps://dl.fbaipu
-00000d40: 626c 6963 6669 6c65 732e 636f 6d2f 7365  blicfiles.com/se
-00000d50: 6d69 7765 616b 7375 7065 7276 6973 696f  miweaksupervisio
-00000d60: 6e2f 6d6f 6465 6c5f 6669 6c65 732f 7365  n/model_files/se
-00000d70: 6d69 5f73 7570 6572 7669 7365 645f 7265  mi_supervised_re
-00000d80: 736e 6574 3138 2d64 3932 6630 3533 302e  snet18-d92f0530.
-00000d90: 7074 687a 6b68 7474 7073 3a2f 2f64 6c2e  pthzkhttps://dl.
-00000da0: 6662 6169 7075 626c 6963 6669 6c65 732e  fbaipublicfiles.
-00000db0: 636f 6d2f 7365 6d69 7765 616b 7375 7065  com/semiweaksupe
-00000dc0: 7276 6973 696f 6e2f 6d6f 6465 6c5f 6669  rvision/model_fi
-00000dd0: 6c65 732f 7365 6d69 5f77 6561 6b6c 795f  les/semi_weakly_
-00000de0: 7375 7065 7276 6973 6564 5f72 6573 6e65  supervised_resne
-00000df0: 7431 382d 3131 3866 3135 3536 2e70 7468  t18-118f1556.pth
-00000e00: 2902 da03 7373 6cda 0473 7773 6c7a 6468  )...ssl..swslzdh
-00000e10: 7474 7073 3a2f 2f64 6c2e 6662 6169 7075  ttps://dl.fbaipu
-00000e20: 626c 6963 6669 6c65 732e 636f 6d2f 7365  blicfiles.com/se
-00000e30: 6d69 7765 616b 7375 7065 7276 6973 696f  miweaksupervisio
-00000e40: 6e2f 6d6f 6465 6c5f 6669 6c65 732f 7365  n/model_files/se
-00000e50: 6d69 5f73 7570 6572 7669 7365 645f 7265  mi_supervised_re
-00000e60: 736e 6574 3530 2d30 3833 3839 3739 322e  snet50-08389792.
-00000e70: 7074 687a 6b68 7474 7073 3a2f 2f64 6c2e  pthzkhttps://dl.
-00000e80: 6662 6169 7075 626c 6963 6669 6c65 732e  fbaipublicfiles.
-00000e90: 636f 6d2f 7365 6d69 7765 616b 7375 7065  com/semiweaksupe
-00000ea0: 7276 6973 696f 6e2f 6d6f 6465 6c5f 6669  rvision/model_fi
-00000eb0: 6c65 732f 7365 6d69 5f77 6561 6b6c 795f  les/semi_weakly_
-00000ec0: 7375 7065 7276 6973 6564 5f72 6573 6e65  supervised_resne
-00000ed0: 7435 302d 3136 6131 3266 3162 2e70 7468  t50-16a12f1b.pth
-00000ee0: 7a40 6874 7470 733a 2f2f 646f 776e 6c6f  z@https://downlo
-00000ef0: 6164 2e70 7974 6f72 6368 2e6f 7267 2f6d  ad.pytorch.org/m
-00000f00: 6f64 656c 732f 7265 736e 6578 7435 305f  odels/resnext50_
-00000f10: 3332 7834 642d 3763 6466 3435 3837 2e70  32x4d-7cdf4587.p
-00000f20: 7468 7a6a 6874 7470 733a 2f2f 646c 2e66  thzjhttps://dl.f
-00000f30: 6261 6970 7562 6c69 6366 696c 6573 2e63  baipublicfiles.c
-00000f40: 6f6d 2f73 656d 6977 6561 6b73 7570 6572  om/semiweaksuper
-00000f50: 7669 7369 6f6e 2f6d 6f64 656c 5f66 696c  vision/model_fil
-00000f60: 6573 2f73 656d 695f 7375 7065 7276 6973  es/semi_supervis
-00000f70: 6564 5f72 6573 6e65 7874 3530 5f33 3278  ed_resnext50_32x
-00000f80: 342d 6464 6233 6535 3535 2e70 7468 7a71  4-ddb3e555.pthzq
-00000f90: 6874 7470 733a 2f2f 646c 2e66 6261 6970  https://dl.fbaip
-00000fa0: 7562 6c69 6366 696c 6573 2e63 6f6d 2f73  ublicfiles.com/s
-00000fb0: 656d 6977 6561 6b73 7570 6572 7669 7369  emiweaksupervisi
-00000fc0: 6f6e 2f6d 6f64 656c 5f66 696c 6573 2f73  on/model_files/s
-00000fd0: 656d 695f 7765 616b 6c79 5f73 7570 6572  emi_weakly_super
-00000fe0: 7669 7365 645f 7265 736e 6578 7435 305f  vised_resnext50_
-00000ff0: 3332 7834 2d37 3236 3739 6534 342e 7074  32x4-72679e44.pt
-00001000: 6829 03da 0869 6d61 6765 6e65 7472 3200  h)...imagenetr2.
-00001010: 0000 7233 0000 007a 6b68 7474 7073 3a2f  ..r3...zkhttps:/
-00001020: 2f64 6c2e 6662 6169 7075 626c 6963 6669  /dl.fbaipublicfi
-00001030: 6c65 732e 636f 6d2f 7365 6d69 7765 616b  les.com/semiweak
-00001040: 7375 7065 7276 6973 696f 6e2f 6d6f 6465  supervision/mode
-00001050: 6c5f 6669 6c65 732f 7365 6d69 5f73 7570  l_files/semi_sup
-00001060: 6572 7669 7365 645f 7265 736e 6578 7431  ervised_resnext1
-00001070: 3031 5f33 3278 342d 6463 3433 3537 3061  01_32x4-dc43570a
-00001080: 2e70 7468 7a72 6874 7470 733a 2f2f 646c  .pthzrhttps://dl
-00001090: 2e66 6261 6970 7562 6c69 6366 696c 6573  .fbaipublicfiles
-000010a0: 2e63 6f6d 2f73 656d 6977 6561 6b73 7570  .com/semiweaksup
-000010b0: 6572 7669 7369 6f6e 2f6d 6f64 656c 5f66  ervision/model_f
-000010c0: 696c 6573 2f73 656d 695f 7765 616b 6c79  iles/semi_weakly
-000010d0: 5f73 7570 6572 7669 7365 645f 7265 736e  _supervised_resn
-000010e0: 6578 7431 3031 5f33 3278 342d 3366 3837  ext101_32x4-3f87
-000010f0: 6534 3662 2e70 7468 7a41 6874 7470 733a  e46b.pthzAhttps:
-00001100: 2f2f 646f 776e 6c6f 6164 2e70 7974 6f72  //download.pytor
-00001110: 6368 2e6f 7267 2f6d 6f64 656c 732f 7265  ch.org/models/re
-00001120: 736e 6578 7431 3031 5f33 3278 3864 2d38  snext101_32x8d-8
-00001130: 6261 3536 6666 352e 7074 687a 4368 7474  ba56ff5.pthzChtt
-00001140: 7073 3a2f 2f64 6f77 6e6c 6f61 642e 7079  ps://download.py
-00001150: 746f 7263 682e 6f72 672f 6d6f 6465 6c73  torch.org/models
-00001160: 2f69 675f 7265 736e 6578 7431 3031 5f33  /ig_resnext101_3
-00001170: 3278 382d 6333 3833 3130 6535 2e70 7468  2x8-c38310e5.pth
-00001180: 7a6b 6874 7470 733a 2f2f 646c 2e66 6261  zkhttps://dl.fba
-00001190: 6970 7562 6c69 6366 696c 6573 2e63 6f6d  ipublicfiles.com
-000011a0: 2f73 656d 6977 6561 6b73 7570 6572 7669  /semiweaksupervi
-000011b0: 7369 6f6e 2f6d 6f64 656c 5f66 696c 6573  sion/model_files
-000011c0: 2f73 656d 695f 7375 7065 7276 6973 6564  /semi_supervised
-000011d0: 5f72 6573 6e65 7874 3130 315f 3332 7838  _resnext101_32x8
-000011e0: 2d32 6366 6532 6638 622e 7074 687a 7268  -2cfe2f8b.pthzrh
-000011f0: 7474 7073 3a2f 2f64 6c2e 6662 6169 7075  ttps://dl.fbaipu
-00001200: 626c 6963 6669 6c65 732e 636f 6d2f 7365  blicfiles.com/se
-00001210: 6d69 7765 616b 7375 7065 7276 6973 696f  miweaksupervisio
-00001220: 6e2f 6d6f 6465 6c5f 6669 6c65 732f 7365  n/model_files/se
-00001230: 6d69 5f77 6561 6b6c 795f 7375 7065 7276  mi_weakly_superv
-00001240: 6973 6564 5f72 6573 6e65 7874 3130 315f  ised_resnext101_
-00001250: 3332 7838 2d62 3437 3132 3930 342e 7074  32x8-b4712904.pt
-00001260: 6829 0472 3400 0000 da09 696e 7374 6167  h).r4.....instag
-00001270: 7261 6d72 3200 0000 7233 0000 007a 4468  ramr2...r3...zDh
-00001280: 7474 7073 3a2f 2f64 6f77 6e6c 6f61 642e  ttps://download.
-00001290: 7079 746f 7263 682e 6f72 672f 6d6f 6465  pytorch.org/mode
-000012a0: 6c73 2f69 675f 7265 736e 6578 7431 3031  ls/ig_resnext101
-000012b0: 5f33 3278 3136 2d63 3666 3739 3662 302e  _32x16-c6f796b0.
-000012c0: 7074 687a 6c68 7474 7073 3a2f 2f64 6c2e  pthzlhttps://dl.
-000012d0: 6662 6169 7075 626c 6963 6669 6c65 732e  fbaipublicfiles.
-000012e0: 636f 6d2f 7365 6d69 7765 616b 7375 7065  com/semiweaksupe
-000012f0: 7276 6973 696f 6e2f 6d6f 6465 6c5f 6669  rvision/model_fi
-00001300: 6c65 732f 7365 6d69 5f73 7570 6572 7669  les/semi_supervi
-00001310: 7365 645f 7265 736e 6578 7431 3031 5f33  sed_resnext101_3
-00001320: 3278 3136 2d31 3566 6666 6135 372e 7074  2x16-15fffa57.pt
-00001330: 687a 7368 7474 7073 3a2f 2f64 6c2e 6662  hzshttps://dl.fb
-00001340: 6169 7075 626c 6963 6669 6c65 732e 636f  aipublicfiles.co
-00001350: 6d2f 7365 6d69 7765 616b 7375 7065 7276  m/semiweaksuperv
-00001360: 6973 696f 6e2f 6d6f 6465 6c5f 6669 6c65  ision/model_file
-00001370: 732f 7365 6d69 5f77 6561 6b6c 795f 7375  s/semi_weakly_su
-00001380: 7065 7276 6973 6564 5f72 6573 6e65 7874  pervised_resnext
-00001390: 3130 315f 3332 7831 362d 6633 3535 3961  101_32x16-f3559a
-000013a0: 3963 2e70 7468 2903 7235 0000 0072 3200  9c.pth).r5...r2.
-000013b0: 0000 7233 0000 0072 3500 0000 7a44 6874  ..r3...r5...zDht
-000013c0: 7470 733a 2f2f 646f 776e 6c6f 6164 2e70  tps://download.p
-000013d0: 7974 6f72 6368 2e6f 7267 2f6d 6f64 656c  ytorch.org/model
-000013e0: 732f 6967 5f72 6573 6e65 7874 3130 315f  s/ig_resnext101_
-000013f0: 3332 7833 322d 6534 6239 3062 3030 2e70  32x32-e4b90b00.p
-00001400: 7468 7a44 6874 7470 733a 2f2f 646f 776e  thzDhttps://down
-00001410: 6c6f 6164 2e70 7974 6f72 6368 2e6f 7267  load.pytorch.org
-00001420: 2f6d 6f64 656c 732f 6967 5f72 6573 6e65  /models/ig_resne
-00001430: 7874 3130 315f 3332 7834 382d 3365 3431  xt101_32x48-3e41
-00001440: 6363 3861 2e70 7468 2908 da08 7265 736e  cc8a.pth)...resn
-00001450: 6574 3138 da08 7265 736e 6574 3530 da0f  et18..resnet50..
-00001460: 7265 736e 6578 7435 305f 3332 7834 64da  resnext50_32x4d.
-00001470: 1072 6573 6e65 7874 3130 315f 3332 7834  .resnext101_32x4
-00001480: 64da 1072 6573 6e65 7874 3130 315f 3332  d..resnext101_32
-00001490: 7838 64da 1172 6573 6e65 7874 3130 315f  x8d..resnext101_
-000014a0: 3332 7831 3664 da11 7265 736e 6578 7431  32x16d..resnext1
-000014b0: 3031 5f33 3278 3332 64da 1172 6573 6e65  01_32x32d..resne
-000014c0: 7874 3130 315f 3332 7834 3864 720b 0000  xt101_32x48dr...
-000014d0: 00e9 e000 0000 670a d7a3 703d 0adf 3f67  ......g...p=..?g
-000014e0: c976 be9f 1a2f dd3f 6796 438b 6ce7 fbd9  .v.../.?g.C.l...
-000014f0: 3f67 1d5a 643b df4f cd3f 6779 e926 3108  ?g.Zd;.O.?gy.&1.
-00001500: accc 3f67 cdcc cccc cccc cc3f 69e8 0300  ..?g.......?i...
-00001510: 0029 06da 0375 726c da0a 696e 7075 745f  .)...url..input_
-00001520: 7369 7a65 da0b 696e 7075 745f 7261 6e67  size..input_rang
-00001530: 65da 046d 6561 6eda 0373 7464 da0b 6e75  e..mean..std..nu
-00001540: 6d5f 636c 6173 7365 7372 3600 0000 2906  m_classesr6...).
-00001550: 720b 0000 00e9 4000 0000 7245 0000 00e9  r.....@...rE....
-00001560: 8000 0000 e900 0100 00e9 0002 0000 e902  ................
-00001570: 0000 0029 0372 1200 0000 da05 626c 6f63  ...).r......bloc
-00001580: 6bda 066c 6179 6572 7329 03da 0765 6e63  k..layers)...enc
-00001590: 6f64 6572 7206 0000 00da 0670 6172 616d  oderr......param
-000015a0: 73da 0872 6573 6e65 7433 34e9 0400 0000  s..resnet34.....
-000015b0: e906 0000 0072 3700 0000 2906 720b 0000  .....r7...).r...
-000015c0: 0072 4500 0000 7247 0000 0072 4800 0000  .rE...rG...rH...
-000015d0: 6900 0400 0069 0008 0000 da09 7265 736e  i....i......resn
-000015e0: 6574 3130 31e9 1700 0000 da09 7265 736e  et101.......resn
-000015f0: 6574 3135 32e9 0800 0000 e924 0000 0072  et152......$...r
-00001600: 3800 0000 e920 0000 0029 0572 1200 0000  8.... ...).r....
-00001610: 724a 0000 0072 4b00 0000 da06 6772 6f75  rJ...rK.....grou
-00001620: 7073 da0f 7769 6474 685f 7065 725f 6772  ps..width_per_gr
-00001630: 6f75 7072 3900 0000 723a 0000 0072 3b00  oupr9...r:...r;.
-00001640: 0000 e910 0000 0072 3c00 0000 723d 0000  .......r<...r=..
-00001650: 00e9 3000 0000 290b 7236 0000 0072 4e00  ..0...).r6...rN.
-00001660: 0000 7237 0000 0072 5100 0000 7253 0000  ..r7...rQ...rS..
-00001670: 0072 3800 0000 7239 0000 0072 3a00 0000  .r8...r9...r:...
-00001680: 723b 0000 0072 3c00 0000 723d 0000 0029  r;...r<...r=...)
-00001690: 15da 075f 5f64 6f63 5f5f da04 636f 7079  ...__doc__..copy
-000016a0: 7202 0000 00da 0874 6f72 6368 2e6e 6e72  r......torch.nnr
-000016b0: 1900 0000 5a19 746f 7263 6876 6973 696f  ....Z.torchvisio
-000016c0: 6e2e 6d6f 6465 6c73 2e72 6573 6e65 7472  n.models.resnetr
-000016d0: 0300 0000 7204 0000 0072 0500 0000 5a2a  ....r....r....Z*
-000016e0: 7072 6574 7261 696e 6564 6d6f 6465 6c73  pretrainedmodels
-000016f0: 2e6d 6f64 656c 732e 746f 7263 6876 6973  .models.torchvis
-00001700: 696f 6e5f 6d6f 6465 6c73 7206 0000 00da  ion_modelsr.....
-00001710: 055f 6261 7365 7208 0000 0072 0900 0000  ._baser....r....
-00001720: 5a0c 6e65 775f 7365 7474 696e 6773 da05  Z.new_settings..
-00001730: 6974 656d 735a 0a6d 6f64 656c 5f6e 616d  itemsZ.model_nam
-00001740: 65da 0773 6f75 7263 6573 5a0b 736f 7572  e..sourcesZ.sour
-00001750: 6365 5f6e 616d 65da 0a73 6f75 7263 655f  ce_name..source_
-00001760: 7572 6cda 0f72 6573 6e65 745f 656e 636f  url..resnet_enco
-00001770: 6465 7273 7217 0000 0072 1700 0000 7217  dersr....r....r.
-00001780: 0000 0072 1800 0000 da08 3c6d 6f64 756c  ...r......<modul
-00001790: 653e 0100 0000 7316 0100 0004 180c 020c  e>....s.........
-000017a0: 020c 010c 010c 010c 020c 0312 2602 0102  ............&...
-000017b0: fe04 0502 0102 fe04 0502 0102 0102 fd04  ................
-000017c0: 0602 0102 fe04 0502 0102 0102 0102 fc04  ................
-000017d0: 0702 0102 0102 fd04 0602 0002 ff02 0402  ................
-000017e0: 0002 ff02 e006 2508 0110 0108 0108 0210  ......%.........
-000017f0: 0202 0108 0106 0108 0108 0102 fa12 0c02  ................
-00001800: 0106 0202 0102 010a fd04 fd04 0a02 0106  ................
-00001810: 0202 0102 010a fd04 fd04 0a02 0106 0202  ................
-00001820: 0102 010a fd04 fd04 0a02 0106 0202 0102  ................
-00001830: 010a fd04 fd04 0a02 0106 0202 0102 010a  ................
-00001840: fd04 fd04 0a02 0106 0202 0102 010a 0102  ................
-00001850: 0102 fb04 fd04 0c02 0106 0202 0102 010a  ................
-00001860: 0102 0102 fb04 fd04 0c02 0106 0202 0102  ................
-00001870: 010a 0102 0102 fb04 fd04 0c02 0106 0202  ................
-00001880: 0102 010a 0102 0102 fb04 fd04 0c02 0106  ................
-00001890: 0202 0102 010a 0102 0102 fb04 fd04 0c02  ................
-000018a0: 0106 0202 0102 010a 0102 0102 fb04 fd04  ................
-000018b0: 9b                                       .
+00000990: 616e 5c6d 675c 7365 676d 656e 7461 7469  an\mg\segmentati
+000009a0: 6f6e 5f6d 6f64 656c 735c 656e 636f 6465  on_models\encode
+000009b0: 7273 5c72 6573 6e65 742e 7079 720d 0000  rs\resnet.pyr...
+000009c0: 0026 0000 0073 0c00 0000 0001 0e01 0601  .&...s..........
+000009d0: 0601 0602 0401 7a16 5265 734e 6574 456e  ......z.ResNetEn
+000009e0: 636f 6465 722e 5f5f 696e 6974 5f5f 6301  coder.__init__c.
+000009f0: 0000 0000 0000 0000 0000 0001 0000 0006  ................
+00000a00: 0000 0043 0000 0073 3600 0000 7400 a001  ...C...s6...t...
+00000a10: a100 7400 a002 7c00 6a03 7c00 6a04 7c00  ..t...|.j.|.j.|.
+00000a20: 6a05 a103 7400 a002 7c00 6a06 7c00 6a07  j...t...|.j.|.j.
+00000a30: a102 7c00 6a08 7c00 6a09 7c00 6a0a 6706  ..|.j.|.j.|.j.g.
+00000a40: 5300 2901 4e29 0bda 026e 6eda 0849 6465  S.).N)...nn..Ide
+00000a50: 6e74 6974 79da 0a53 6571 7565 6e74 6961  ntity..Sequentia
+00000a60: 6cda 0563 6f6e 7631 da03 626e 31da 0472  l..conv1..bn1..r
+00000a70: 656c 75da 076d 6178 706f 6f6c da06 6c61  elu..maxpool..la
+00000a80: 7965 7231 da06 6c61 7965 7232 da06 6c61  yer1..layer2..la
+00000a90: 7965 7233 da06 6c61 7965 7234 2901 7211  yer3..layer4).r.
+00000aa0: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00000ab0: 0000 da0a 6765 745f 7374 6167 6573 2f00  ....get_stages/.
+00000ac0: 0000 730e 0000 0000 0206 0112 010e 0104  ..s.............
+00000ad0: 0104 0104 fa7a 1852 6573 4e65 7445 6e63  .....z.ResNetEnc
+00000ae0: 6f64 6572 2e67 6574 5f73 7461 6765 7363  oder.get_stagesc
+00000af0: 0200 0000 0000 0000 0000 0000 0500 0000  ................
+00000b00: 0400 0000 4300 0000 733a 0000 007c 00a0  ....C...s:...|..
+00000b10: 00a1 007d 0267 007d 0374 017c 006a 0264  ...}.g.}.t.|.j.d
+00000b20: 0117 0083 0144 005d 1a7d 047c 027c 0419  .....D.].}.|.|..
+00000b30: 007c 0183 017d 017c 03a0 037c 01a1 0101  .|...}.|...|....
+00000b40: 0071 1a7c 0353 0029 024e 7207 0000 0029  .q.|.S.).Nr....)
+00000b50: 0472 2400 0000 da05 7261 6e67 6572 0e00  .r$.....ranger..
+00000b60: 0000 da06 6170 7065 6e64 2905 7211 0000  ....append).r...
+00000b70: 00da 0178 5a06 7374 6167 6573 da08 6665  ...xZ.stages..fe
+00000b80: 6174 7572 6573 da01 6972 1700 0000 7217  atures..ir....r.
+00000b90: 0000 0072 1800 0000 da07 666f 7277 6172  ...r......forwar
+00000ba0: 6439 0000 0073 0c00 0000 0001 0802 0401  d9...s..........
+00000bb0: 1201 0c01 0c02 7a15 5265 734e 6574 456e  ......z.ResNetEn
+00000bc0: 636f 6465 722e 666f 7277 6172 6463 0200  coder.forwardc..
+00000bd0: 0000 0000 0000 0000 0000 0300 0000 0300  ................
+00000be0: 0000 0b00 0000 7328 0000 007c 01a0 0064  ......s(...|...d
+00000bf0: 01a1 0101 007c 01a0 0064 02a1 0101 0074  .....|...d.....t
+00000c00: 0183 006a 027c 0166 017c 028e 0101 0064  ...j.|.f.|.....d
+00000c10: 0053 0029 034e 7a07 6663 2e62 6961 737a  .S.).Nz.fc.biasz
+00000c20: 0966 632e 7765 6967 6874 2903 da03 706f  .fc.weight)...po
+00000c30: 7072 0c00 0000 da0f 6c6f 6164 5f73 7461  pr......load_sta
+00000c40: 7465 5f64 6963 7429 0372 1100 0000 da0a  te_dict).r......
+00000c50: 7374 6174 655f 6469 6374 7214 0000 0072  state_dictr....r
+00000c60: 1500 0000 7217 0000 0072 1800 0000 722c  ....r....r....r,
+00000c70: 0000 0043 0000 0073 0600 0000 0001 0a01  ...C...s........
+00000c80: 0a01 7a1d 5265 734e 6574 456e 636f 6465  ..z.ResNetEncode
+00000c90: 722e 6c6f 6164 5f73 7461 7465 5f64 6963  r.load_state_dic
+00000ca0: 7429 0172 0a00 0000 2908 da08 5f5f 6e61  t).r....)...__na
+00000cb0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000cc0: da0c 5f5f 7175 616c 6e61 6d65 5f5f 720d  ..__qualname__r.
+00000cd0: 0000 0072 2400 0000 722a 0000 0072 2c00  ...r$...r*...r,.
+00000ce0: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
+00000cf0: 5f72 1700 0000 7217 0000 0072 1500 0000  _r....r....r....
+00000d00: 7218 0000 0072 0900 0000 2500 0000 7308  r....r....%...s.
+00000d10: 0000 0008 010e 0908 0a08 0a72 0900 0000  ...........r....
+00000d20: 7a64 6874 7470 733a 2f2f 646c 2e66 6261  zdhttps://dl.fba
+00000d30: 6970 7562 6c69 6366 696c 6573 2e63 6f6d  ipublicfiles.com
+00000d40: 2f73 656d 6977 6561 6b73 7570 6572 7669  /semiweaksupervi
+00000d50: 7369 6f6e 2f6d 6f64 656c 5f66 696c 6573  sion/model_files
+00000d60: 2f73 656d 695f 7375 7065 7276 6973 6564  /semi_supervised
+00000d70: 5f72 6573 6e65 7431 382d 6439 3266 3035  _resnet18-d92f05
+00000d80: 3330 2e70 7468 7a6b 6874 7470 733a 2f2f  30.pthzkhttps://
+00000d90: 646c 2e66 6261 6970 7562 6c69 6366 696c  dl.fbaipublicfil
+00000da0: 6573 2e63 6f6d 2f73 656d 6977 6561 6b73  es.com/semiweaks
+00000db0: 7570 6572 7669 7369 6f6e 2f6d 6f64 656c  upervision/model
+00000dc0: 5f66 696c 6573 2f73 656d 695f 7765 616b  _files/semi_weak
+00000dd0: 6c79 5f73 7570 6572 7669 7365 645f 7265  ly_supervised_re
+00000de0: 736e 6574 3138 2d31 3138 6631 3535 362e  snet18-118f1556.
+00000df0: 7074 6829 02da 0373 736c da04 7377 736c  pth)...ssl..swsl
+00000e00: 7a64 6874 7470 733a 2f2f 646c 2e66 6261  zdhttps://dl.fba
+00000e10: 6970 7562 6c69 6366 696c 6573 2e63 6f6d  ipublicfiles.com
+00000e20: 2f73 656d 6977 6561 6b73 7570 6572 7669  /semiweaksupervi
+00000e30: 7369 6f6e 2f6d 6f64 656c 5f66 696c 6573  sion/model_files
+00000e40: 2f73 656d 695f 7375 7065 7276 6973 6564  /semi_supervised
+00000e50: 5f72 6573 6e65 7435 302d 3038 3338 3937  _resnet50-083897
+00000e60: 3932 2e70 7468 7a6b 6874 7470 733a 2f2f  92.pthzkhttps://
+00000e70: 646c 2e66 6261 6970 7562 6c69 6366 696c  dl.fbaipublicfil
+00000e80: 6573 2e63 6f6d 2f73 656d 6977 6561 6b73  es.com/semiweaks
+00000e90: 7570 6572 7669 7369 6f6e 2f6d 6f64 656c  upervision/model
+00000ea0: 5f66 696c 6573 2f73 656d 695f 7765 616b  _files/semi_weak
+00000eb0: 6c79 5f73 7570 6572 7669 7365 645f 7265  ly_supervised_re
+00000ec0: 736e 6574 3530 2d31 3661 3132 6631 622e  snet50-16a12f1b.
+00000ed0: 7074 687a 4068 7474 7073 3a2f 2f64 6f77  pthz@https://dow
+00000ee0: 6e6c 6f61 642e 7079 746f 7263 682e 6f72  nload.pytorch.or
+00000ef0: 672f 6d6f 6465 6c73 2f72 6573 6e65 7874  g/models/resnext
+00000f00: 3530 5f33 3278 3464 2d37 6364 6634 3538  50_32x4d-7cdf458
+00000f10: 372e 7074 687a 6a68 7474 7073 3a2f 2f64  7.pthzjhttps://d
+00000f20: 6c2e 6662 6169 7075 626c 6963 6669 6c65  l.fbaipublicfile
+00000f30: 732e 636f 6d2f 7365 6d69 7765 616b 7375  s.com/semiweaksu
+00000f40: 7065 7276 6973 696f 6e2f 6d6f 6465 6c5f  pervision/model_
+00000f50: 6669 6c65 732f 7365 6d69 5f73 7570 6572  files/semi_super
+00000f60: 7669 7365 645f 7265 736e 6578 7435 305f  vised_resnext50_
+00000f70: 3332 7834 2d64 6462 3365 3535 352e 7074  32x4-ddb3e555.pt
+00000f80: 687a 7168 7474 7073 3a2f 2f64 6c2e 6662  hzqhttps://dl.fb
+00000f90: 6169 7075 626c 6963 6669 6c65 732e 636f  aipublicfiles.co
+00000fa0: 6d2f 7365 6d69 7765 616b 7375 7065 7276  m/semiweaksuperv
+00000fb0: 6973 696f 6e2f 6d6f 6465 6c5f 6669 6c65  ision/model_file
+00000fc0: 732f 7365 6d69 5f77 6561 6b6c 795f 7375  s/semi_weakly_su
+00000fd0: 7065 7276 6973 6564 5f72 6573 6e65 7874  pervised_resnext
+00000fe0: 3530 5f33 3278 342d 3732 3637 3965 3434  50_32x4-72679e44
+00000ff0: 2e70 7468 2903 da08 696d 6167 656e 6574  .pth)...imagenet
+00001000: 7232 0000 0072 3300 0000 7a6b 6874 7470  r2...r3...zkhttp
+00001010: 733a 2f2f 646c 2e66 6261 6970 7562 6c69  s://dl.fbaipubli
+00001020: 6366 696c 6573 2e63 6f6d 2f73 656d 6977  cfiles.com/semiw
+00001030: 6561 6b73 7570 6572 7669 7369 6f6e 2f6d  eaksupervision/m
+00001040: 6f64 656c 5f66 696c 6573 2f73 656d 695f  odel_files/semi_
+00001050: 7375 7065 7276 6973 6564 5f72 6573 6e65  supervised_resne
+00001060: 7874 3130 315f 3332 7834 2d64 6334 3335  xt101_32x4-dc435
+00001070: 3730 612e 7074 687a 7268 7474 7073 3a2f  70a.pthzrhttps:/
+00001080: 2f64 6c2e 6662 6169 7075 626c 6963 6669  /dl.fbaipublicfi
+00001090: 6c65 732e 636f 6d2f 7365 6d69 7765 616b  les.com/semiweak
+000010a0: 7375 7065 7276 6973 696f 6e2f 6d6f 6465  supervision/mode
+000010b0: 6c5f 6669 6c65 732f 7365 6d69 5f77 6561  l_files/semi_wea
+000010c0: 6b6c 795f 7375 7065 7276 6973 6564 5f72  kly_supervised_r
+000010d0: 6573 6e65 7874 3130 315f 3332 7834 2d33  esnext101_32x4-3
+000010e0: 6638 3765 3436 622e 7074 687a 4168 7474  f87e46b.pthzAhtt
+000010f0: 7073 3a2f 2f64 6f77 6e6c 6f61 642e 7079  ps://download.py
+00001100: 746f 7263 682e 6f72 672f 6d6f 6465 6c73  torch.org/models
+00001110: 2f72 6573 6e65 7874 3130 315f 3332 7838  /resnext101_32x8
+00001120: 642d 3862 6135 3666 6635 2e70 7468 7a43  d-8ba56ff5.pthzC
+00001130: 6874 7470 733a 2f2f 646f 776e 6c6f 6164  https://download
+00001140: 2e70 7974 6f72 6368 2e6f 7267 2f6d 6f64  .pytorch.org/mod
+00001150: 656c 732f 6967 5f72 6573 6e65 7874 3130  els/ig_resnext10
+00001160: 315f 3332 7838 2d63 3338 3331 3065 352e  1_32x8-c38310e5.
+00001170: 7074 687a 6b68 7474 7073 3a2f 2f64 6c2e  pthzkhttps://dl.
+00001180: 6662 6169 7075 626c 6963 6669 6c65 732e  fbaipublicfiles.
+00001190: 636f 6d2f 7365 6d69 7765 616b 7375 7065  com/semiweaksupe
+000011a0: 7276 6973 696f 6e2f 6d6f 6465 6c5f 6669  rvision/model_fi
+000011b0: 6c65 732f 7365 6d69 5f73 7570 6572 7669  les/semi_supervi
+000011c0: 7365 645f 7265 736e 6578 7431 3031 5f33  sed_resnext101_3
+000011d0: 3278 382d 3263 6665 3266 3862 2e70 7468  2x8-2cfe2f8b.pth
+000011e0: 7a72 6874 7470 733a 2f2f 646c 2e66 6261  zrhttps://dl.fba
+000011f0: 6970 7562 6c69 6366 696c 6573 2e63 6f6d  ipublicfiles.com
+00001200: 2f73 656d 6977 6561 6b73 7570 6572 7669  /semiweaksupervi
+00001210: 7369 6f6e 2f6d 6f64 656c 5f66 696c 6573  sion/model_files
+00001220: 2f73 656d 695f 7765 616b 6c79 5f73 7570  /semi_weakly_sup
+00001230: 6572 7669 7365 645f 7265 736e 6578 7431  ervised_resnext1
+00001240: 3031 5f33 3278 382d 6234 3731 3239 3034  01_32x8-b4712904
+00001250: 2e70 7468 2904 7234 0000 00da 0969 6e73  .pth).r4.....ins
+00001260: 7461 6772 616d 7232 0000 0072 3300 0000  tagramr2...r3...
+00001270: 7a44 6874 7470 733a 2f2f 646f 776e 6c6f  zDhttps://downlo
+00001280: 6164 2e70 7974 6f72 6368 2e6f 7267 2f6d  ad.pytorch.org/m
+00001290: 6f64 656c 732f 6967 5f72 6573 6e65 7874  odels/ig_resnext
+000012a0: 3130 315f 3332 7831 362d 6336 6637 3936  101_32x16-c6f796
+000012b0: 6230 2e70 7468 7a6c 6874 7470 733a 2f2f  b0.pthzlhttps://
+000012c0: 646c 2e66 6261 6970 7562 6c69 6366 696c  dl.fbaipublicfil
+000012d0: 6573 2e63 6f6d 2f73 656d 6977 6561 6b73  es.com/semiweaks
+000012e0: 7570 6572 7669 7369 6f6e 2f6d 6f64 656c  upervision/model
+000012f0: 5f66 696c 6573 2f73 656d 695f 7375 7065  _files/semi_supe
+00001300: 7276 6973 6564 5f72 6573 6e65 7874 3130  rvised_resnext10
+00001310: 315f 3332 7831 362d 3135 6666 6661 3537  1_32x16-15fffa57
+00001320: 2e70 7468 7a73 6874 7470 733a 2f2f 646c  .pthzshttps://dl
+00001330: 2e66 6261 6970 7562 6c69 6366 696c 6573  .fbaipublicfiles
+00001340: 2e63 6f6d 2f73 656d 6977 6561 6b73 7570  .com/semiweaksup
+00001350: 6572 7669 7369 6f6e 2f6d 6f64 656c 5f66  ervision/model_f
+00001360: 696c 6573 2f73 656d 695f 7765 616b 6c79  iles/semi_weakly
+00001370: 5f73 7570 6572 7669 7365 645f 7265 736e  _supervised_resn
+00001380: 6578 7431 3031 5f33 3278 3136 2d66 3335  ext101_32x16-f35
+00001390: 3539 6139 632e 7074 6829 0372 3500 0000  59a9c.pth).r5...
+000013a0: 7232 0000 0072 3300 0000 7235 0000 007a  r2...r3...r5...z
+000013b0: 4468 7474 7073 3a2f 2f64 6f77 6e6c 6f61  Dhttps://downloa
+000013c0: 642e 7079 746f 7263 682e 6f72 672f 6d6f  d.pytorch.org/mo
+000013d0: 6465 6c73 2f69 675f 7265 736e 6578 7431  dels/ig_resnext1
+000013e0: 3031 5f33 3278 3332 2d65 3462 3930 6230  01_32x32-e4b90b0
+000013f0: 302e 7074 687a 4468 7474 7073 3a2f 2f64  0.pthzDhttps://d
+00001400: 6f77 6e6c 6f61 642e 7079 746f 7263 682e  ownload.pytorch.
+00001410: 6f72 672f 6d6f 6465 6c73 2f69 675f 7265  org/models/ig_re
+00001420: 736e 6578 7431 3031 5f33 3278 3438 2d33  snext101_32x48-3
+00001430: 6534 3163 6338 612e 7074 6829 08da 0872  e41cc8a.pth)...r
+00001440: 6573 6e65 7431 38da 0872 6573 6e65 7435  esnet18..resnet5
+00001450: 30da 0f72 6573 6e65 7874 3530 5f33 3278  0..resnext50_32x
+00001460: 3464 da10 7265 736e 6578 7431 3031 5f33  4d..resnext101_3
+00001470: 3278 3464 da10 7265 736e 6578 7431 3031  2x4d..resnext101
+00001480: 5f33 3278 3864 da11 7265 736e 6578 7431  _32x8d..resnext1
+00001490: 3031 5f33 3278 3136 64da 1172 6573 6e65  01_32x16d..resne
+000014a0: 7874 3130 315f 3332 7833 3264 da11 7265  xt101_32x32d..re
+000014b0: 736e 6578 7431 3031 5f33 3278 3438 6472  snext101_32x48dr
+000014c0: 0b00 0000 e9e0 0000 0067 0ad7 a370 3d0a  .........g...p=.
+000014d0: df3f 67c9 76be 9f1a 2fdd 3f67 9643 8b6c  .?g.v.../.?g.C.l
+000014e0: e7fb d93f 671d 5a64 3bdf 4fcd 3f67 79e9  ...?g.Zd;.O.?gy.
+000014f0: 2631 08ac cc3f 67cd cccc cccc cccc 3f69  &1...?g.......?i
+00001500: e803 0000 2906 da03 7572 6cda 0a69 6e70  ....)...url..inp
+00001510: 7574 5f73 697a 65da 0b69 6e70 7574 5f72  ut_size..input_r
+00001520: 616e 6765 da04 6d65 616e da03 7374 64da  ange..mean..std.
+00001530: 0b6e 756d 5f63 6c61 7373 6573 7236 0000  .num_classesr6..
+00001540: 0029 0672 0b00 0000 e940 0000 0072 4500  .).r.....@...rE.
+00001550: 0000 e980 0000 00e9 0001 0000 e900 0200  ................
+00001560: 00e9 0200 0000 2903 7212 0000 00da 0562  ......).r......b
+00001570: 6c6f 636b da06 6c61 7965 7273 2903 da07  lock..layers)...
+00001580: 656e 636f 6465 7272 0600 0000 da06 7061  encoderr......pa
+00001590: 7261 6d73 da08 7265 736e 6574 3334 e904  rams..resnet34..
+000015a0: 0000 00e9 0600 0000 7237 0000 0029 0672  ........r7...).r
+000015b0: 0b00 0000 7245 0000 0072 4700 0000 7248  ....rE...rG...rH
+000015c0: 0000 0069 0004 0000 6900 0800 00da 0972  ...i....i......r
+000015d0: 6573 6e65 7431 3031 e917 0000 00da 0972  esnet101.......r
+000015e0: 6573 6e65 7431 3532 e908 0000 00e9 2400  esnet152......$.
+000015f0: 0000 7238 0000 00e9 2000 0000 2905 7212  ..r8.... ...).r.
+00001600: 0000 0072 4a00 0000 724b 0000 00da 0667  ...rJ...rK.....g
+00001610: 726f 7570 73da 0f77 6964 7468 5f70 6572  roups..width_per
+00001620: 5f67 726f 7570 7239 0000 0072 3a00 0000  _groupr9...r:...
+00001630: 723b 0000 00e9 1000 0000 723c 0000 0072  r;........r<...r
+00001640: 3d00 0000 e930 0000 0029 0b72 3600 0000  =....0...).r6...
+00001650: 724e 0000 0072 3700 0000 7251 0000 0072  rN...r7...rQ...r
+00001660: 5300 0000 7238 0000 0072 3900 0000 723a  S...r8...r9...r:
+00001670: 0000 0072 3b00 0000 723c 0000 0072 3d00  ...r;...r<...r=.
+00001680: 0000 2915 da07 5f5f 646f 635f 5fda 0463  ..)...__doc__..c
+00001690: 6f70 7972 0200 0000 da08 746f 7263 682e  opyr......torch.
+000016a0: 6e6e 7219 0000 005a 1974 6f72 6368 7669  nnr....Z.torchvi
+000016b0: 7369 6f6e 2e6d 6f64 656c 732e 7265 736e  sion.models.resn
+000016c0: 6574 7203 0000 0072 0400 0000 7205 0000  etr....r....r...
+000016d0: 005a 2a70 7265 7472 6169 6e65 646d 6f64  .Z*pretrainedmod
+000016e0: 656c 732e 6d6f 6465 6c73 2e74 6f72 6368  els.models.torch
+000016f0: 7669 7369 6f6e 5f6d 6f64 656c 7372 0600  vision_modelsr..
+00001700: 0000 da05 5f62 6173 6572 0800 0000 7209  ...._baser....r.
+00001710: 0000 005a 0c6e 6577 5f73 6574 7469 6e67  ...Z.new_setting
+00001720: 73da 0569 7465 6d73 5a0a 6d6f 6465 6c5f  s..itemsZ.model_
+00001730: 6e61 6d65 da07 736f 7572 6365 735a 0b73  name..sourcesZ.s
+00001740: 6f75 7263 655f 6e61 6d65 da0a 736f 7572  ource_name..sour
+00001750: 6365 5f75 726c da0f 7265 736e 6574 5f65  ce_url..resnet_e
+00001760: 6e63 6f64 6572 7372 1700 0000 7217 0000  ncodersr....r...
+00001770: 0072 1700 0000 7218 0000 00da 083c 6d6f  .r....r......<mo
+00001780: 6475 6c65 3e01 0000 0073 1601 0000 0418  dule>....s......
+00001790: 0c02 0c02 0c01 0c01 0c01 0c02 0c03 1226  ...............&
+000017a0: 0201 02fe 0405 0201 02fe 0405 0201 0201  ................
+000017b0: 02fd 0406 0201 02fe 0405 0201 0201 0201  ................
+000017c0: 02fc 0407 0201 0201 02fd 0406 0200 02ff  ................
+000017d0: 0204 0200 02ff 02e0 0625 0801 1001 0801  .........%......
+000017e0: 0802 1002 0201 0801 0601 0801 0801 02fa  ................
+000017f0: 120c 0201 0602 0201 0201 0afd 04fd 040a  ................
+00001800: 0201 0602 0201 0201 0afd 04fd 040a 0201  ................
+00001810: 0602 0201 0201 0afd 04fd 040a 0201 0602  ................
+00001820: 0201 0201 0afd 04fd 040a 0201 0602 0201  ................
+00001830: 0201 0afd 04fd 040a 0201 0602 0201 0201  ................
+00001840: 0a01 0201 02fb 04fd 040c 0201 0602 0201  ................
+00001850: 0201 0a01 0201 02fb 04fd 040c 0201 0602  ................
+00001860: 0201 0201 0a01 0201 02fb 04fd 040c 0201  ................
+00001870: 0602 0201 0201 0a01 0201 02fb 04fd 040c  ................
+00001880: 0201 0602 0201 0201 0a01 0201 02fb 04fd  ................
+00001890: 040c 0201 0602 0201 0201 0a01 0201 02fb  ................
+000018a0: 04fd 049b                                ....
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/resnet.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/resnet.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/senet.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/senet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/senet.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/senet.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/senet.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/senet.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/senet.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/senet.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:20 2023 UTC, .py size: 5849 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -127,116 +127,115 @@
 000007e0: da08 5f5f 696e 6974 5f5f da0d 5f6f 7574  ..__init__.._out
 000007f0: 5f63 6861 6e6e 656c 73da 065f 6465 7074  _channels.._dept
 00000800: 68da 0c5f 696e 5f63 6861 6e6e 656c 73da  h.._in_channels.
 00000810: 0b6c 6173 745f 6c69 6e65 6172 da08 6176  .last_linear..av
 00000820: 675f 706f 6f6c 2904 da04 7365 6c66 da0c  g_pool)...self..
 00000830: 6f75 745f 6368 616e 6e65 6c73 da05 6465  out_channels..de
 00000840: 7074 68da 066b 7761 7267 73a9 01da 095f  pth..kwargs...._
-00000850: 5f63 6c61 7373 5f5f a900 fa55 433a 5c55  _class__...UC:\U
+00000850: 5f63 6c61 7373 5f5f a900 fa48 633a 5c55  _class__...Hc:\U
 00000860: 7365 7273 5c6d 6861 6e61 6e5c 446f 776e  sers\mhanan\Down
-00000870: 6c6f 6164 735c 4861 6e61 6e5c 4d61 6d6d  loads\Hanan\Mamm
-00000880: 6f50 795c 6d61 6d6d 6f70 795c 7365 676d  oPy\mammopy\segm
-00000890: 656e 7461 7469 6f6e 5f6d 6f64 656c 735c  entation_models\
-000008a0: 656e 636f 6465 7273 5c73 656e 6574 2e70  encoders\senet.p
-000008b0: 7972 0d00 0000 2700 0000 730c 0000 0000  yr....'...s.....
-000008c0: 010e 0206 0106 0106 0204 017a 1553 454e  ...........z.SEN
-000008d0: 6574 456e 636f 6465 722e 5f5f 696e 6974  etEncoder.__init
-000008e0: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
-000008f0: 0000 0006 0000 0043 0000 0073 3400 0000  .......C...s4...
-00000900: 7400 a001 a100 7c00 6a02 6400 6401 8502  t.....|.j.d.d...
-00000910: 1900 7400 a003 7c00 6a02 6401 1900 7c00  ..t...|.j.d...|.
-00000920: 6a04 a102 7c00 6a05 7c00 6a06 7c00 6a07  j...|.j.|.j.|.j.
-00000930: 6706 5300 2902 4ee9 ffff ffff 2908 da02  g.S.).N.....)...
-00000940: 6e6e da08 4964 656e 7469 7479 da06 6c61  nn..Identity..la
-00000950: 7965 7230 da0a 5365 7175 656e 7469 616c  yer0..Sequential
-00000960: da06 6c61 7965 7231 da06 6c61 7965 7232  ..layer1..layer2
-00000970: da06 6c61 7965 7233 da06 6c61 7965 7234  ..layer3..layer4
-00000980: 2901 7213 0000 0072 1900 0000 7219 0000  ).r....r....r...
-00000990: 0072 1a00 0000 da0a 6765 745f 7374 6167  .r......get_stag
-000009a0: 6573 3100 0000 730e 0000 0000 0206 010c  es1...s.........
-000009b0: 0112 0104 0104 0104 fa7a 1753 454e 6574  .........z.SENet
-000009c0: 456e 636f 6465 722e 6765 745f 7374 6167  Encoder.get_stag
-000009d0: 6573 6302 0000 0000 0000 0000 0000 0005  esc.............
-000009e0: 0000 0004 0000 0043 0000 0073 3a00 0000  .......C...s:...
-000009f0: 7c00 a000 a100 7d02 6700 7d03 7401 7c00  |.....}.g.}.t.|.
-00000a00: 6a02 6401 1700 8301 4400 5d1a 7d04 7c02  j.d.....D.].}.|.
-00000a10: 7c04 1900 7c01 8301 7d01 7c03 a003 7c01  |...|...}.|...|.
-00000a20: a101 0100 711a 7c03 5300 2902 4e72 0700  ....q.|.S.).Nr..
-00000a30: 0000 2904 7224 0000 00da 0572 616e 6765  ..).r$.....range
-00000a40: 720f 0000 00da 0661 7070 656e 6429 0572  r......append).r
-00000a50: 1300 0000 da01 78da 0673 7461 6765 73da  ......x..stages.
-00000a60: 0866 6561 7475 7265 73da 0169 7219 0000  .features..ir...
-00000a70: 0072 1900 0000 721a 0000 00da 0766 6f72  .r....r......for
-00000a80: 7761 7264 3b00 0000 730c 0000 0000 0108  ward;...s.......
-00000a90: 0204 0112 010c 010c 027a 1453 454e 6574  .........z.SENet
-00000aa0: 456e 636f 6465 722e 666f 7277 6172 6463  Encoder.forwardc
-00000ab0: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-00000ac0: 0300 0000 0b00 0000 7328 0000 007c 01a0  ........s(...|..
-00000ad0: 0064 01a1 0101 007c 01a0 0064 02a1 0101  .d.....|...d....
-00000ae0: 0074 0183 006a 027c 0166 017c 028e 0101  .t...j.|.f.|....
-00000af0: 0064 0053 0029 034e 7a10 6c61 7374 5f6c  .d.S.).Nz.last_l
-00000b00: 696e 6561 722e 6269 6173 7a12 6c61 7374  inear.biasz.last
-00000b10: 5f6c 696e 6561 722e 7765 6967 6874 2903  _linear.weight).
-00000b20: da03 706f 7072 0c00 0000 da0f 6c6f 6164  ..popr......load
-00000b30: 5f73 7461 7465 5f64 6963 7429 0372 1300  _state_dict).r..
-00000b40: 0000 da0a 7374 6174 655f 6469 6374 7216  ....state_dictr.
-00000b50: 0000 0072 1700 0000 7219 0000 0072 1a00  ...r....r....r..
-00000b60: 0000 722d 0000 0045 0000 0073 0600 0000  ..r-...E...s....
-00000b70: 0001 0a01 0a01 7a1c 5345 4e65 7445 6e63  ......z.SENetEnc
-00000b80: 6f64 6572 2e6c 6f61 645f 7374 6174 655f  oder.load_state_
-00000b90: 6469 6374 2901 720a 0000 0029 08da 085f  dict).r....)..._
-00000ba0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000bb0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000bc0: 5f72 0d00 0000 7224 0000 0072 2b00 0000  _r....r$...r+...
-00000bd0: 722d 0000 00da 0d5f 5f63 6c61 7373 6365  r-.....__classce
-00000be0: 6c6c 5f5f 7219 0000 0072 1900 0000 7217  ll__r....r....r.
-00000bf0: 0000 0072 1a00 0000 7209 0000 0026 0000  ...r....r....&..
-00000c00: 0073 0800 0000 0801 0e0a 080a 080a 7209  .s............r.
-00000c10: 0000 00da 0873 656e 6574 3135 3429 0672  .....senet154).r
-00000c20: 0b00 0000 e980 0000 00e9 0001 0000 e900  ................
-00000c30: 0200 00e9 0004 0000 e900 0800 0067 9a99  .............g..
-00000c40: 9999 9999 c93f e940 0000 0072 0b00 0000  .....?.@...r....
-00000c50: e908 0000 00e9 2400 0000 69e8 0300 00e9  ......$...i.....
-00000c60: 1000 0000 2907 7214 0000 00da 0562 6c6f  ....).r......blo
-00000c70: 636b da09 6472 6f70 6f75 745f 70da 0667  ck..dropout_p..g
-00000c80: 726f 7570 73da 066c 6179 6572 73da 0b6e  roups..layers..n
-00000c90: 756d 5f63 6c61 7373 6573 da09 7265 6475  um_classes..redu
-00000ca0: 6374 696f 6e29 03da 0765 6e63 6f64 6572  ction)...encoder
-00000cb0: 7206 0000 00da 0670 6172 616d 73da 0b73  r......params..s
-00000cc0: 655f 7265 736e 6574 3530 2906 720b 0000  e_resnet50).r...
-00000cd0: 0072 3900 0000 7235 0000 0072 3600 0000  .r9...r5...r6...
-00000ce0: 7237 0000 0072 3800 0000 e904 0000 00e9  r7...r8.........
-00000cf0: 0600 0000 4629 0b72 1400 0000 723d 0000  ....F).r....r=..
-00000d00: 0072 4000 0000 da16 646f 776e 7361 6d70  .r@.....downsamp
-00000d10: 6c65 5f6b 6572 6e65 6c5f 7369 7a65 da12  le_kernel_size..
-00000d20: 646f 776e 7361 6d70 6c65 5f70 6164 6469  downsample_paddi
-00000d30: 6e67 723e 0000 0072 3f00 0000 da08 696e  ngr>...r?.....in
-00000d40: 706c 616e 6573 da09 696e 7075 745f 3378  planes..input_3x
-00000d50: 3372 4100 0000 7242 0000 00da 0c73 655f  3rA...rB.....se_
-00000d60: 7265 736e 6574 3130 31e9 1700 0000 da0c  resnet101.......
-00000d70: 7365 5f72 6573 6e65 7431 3532 da12 7365  se_resnet152..se
-00000d80: 5f72 6573 6e65 7874 3530 5f33 3278 3464  _resnext50_32x4d
-00000d90: e920 0000 00da 1373 655f 7265 736e 6578  . .....se_resnex
-00000da0: 7431 3031 5f33 3278 3464 2906 7233 0000  t101_32x4d).r3..
-00000db0: 0072 4500 0000 724c 0000 0072 4e00 0000  .rE...rL...rN...
-00000dc0: 724f 0000 0072 5100 0000 290d da07 5f5f  rO...rQ...)...__
-00000dd0: 646f 635f 5fda 0874 6f72 6368 2e6e 6e72  doc__..torch.nnr
-00000de0: 1c00 0000 5a1d 7072 6574 7261 696e 6564  ....Z.pretrained
-00000df0: 6d6f 6465 6c73 2e6d 6f64 656c 732e 7365  models.models.se
-00000e00: 6e65 7472 0200 0000 7203 0000 0072 0400  netr....r....r..
-00000e10: 0000 7205 0000 0072 0600 0000 da05 5f62  ..r....r......_b
-00000e20: 6173 6572 0800 0000 7209 0000 00da 0e73  aser....r......s
-00000e30: 656e 6574 5f65 6e63 6f64 6572 7372 1900  enet_encodersr..
-00000e40: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00000e50: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00000e60: b600 0000 0419 0c02 1c07 0c03 1227 0201  .............'..
-00000e70: 0602 0201 0201 0201 0201 0a01 0201 02f9  ................
-00000e80: 04fd 040e 0201 0602 0201 0201 0a01 0201  ................
-00000e90: 0201 0201 0201 0201 0201 0201 02f5 04fd  ................
-00000ea0: 0412 0201 0602 0201 0201 0a01 0201 0201  ................
-00000eb0: 0201 0201 0201 0201 0201 02f5 04fd 0412  ................
-00000ec0: 0201 0602 0201 0201 0a01 0201 0201 0201  ................
-00000ed0: 0201 0201 0201 0201 02f5 04fd 0412 0201  ................
-00000ee0: 0602 0201 0201 0a01 0201 0201 0201 0201  ................
-00000ef0: 0201 0201 0201 02f5 04fd 0412 0201 0602  ................
-00000f00: 0201 0201 0a01 0201 0201 0201 0201 0201  ................
-00000f10: 0201 0201 02f5 04fd 04ae                 ..........
+00000870: 6c6f 6164 735c 4861 6e61 6e5c 6d67 5c73  loads\Hanan\mg\s
+00000880: 6567 6d65 6e74 6174 696f 6e5f 6d6f 6465  egmentation_mode
+00000890: 6c73 5c65 6e63 6f64 6572 735c 7365 6e65  ls\encoders\sene
+000008a0: 742e 7079 720d 0000 0027 0000 0073 0c00  t.pyr....'...s..
+000008b0: 0000 0001 0e02 0601 0601 0602 0401 7a15  ..............z.
+000008c0: 5345 4e65 7445 6e63 6f64 6572 2e5f 5f69  SENetEncoder.__i
+000008d0: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
+000008e0: 0000 0100 0000 0600 0000 4300 0000 7334  ..........C...s4
+000008f0: 0000 0074 00a0 01a1 007c 006a 0264 0064  ...t.....|.j.d.d
+00000900: 0185 0219 0074 00a0 037c 006a 0264 0119  .....t...|.j.d..
+00000910: 007c 006a 04a1 027c 006a 057c 006a 067c  .|.j...|.j.|.j.|
+00000920: 006a 0767 0653 0029 024e e9ff ffff ff29  .j.g.S.).N.....)
+00000930: 08da 026e 6eda 0849 6465 6e74 6974 79da  ...nn..Identity.
+00000940: 066c 6179 6572 30da 0a53 6571 7565 6e74  .layer0..Sequent
+00000950: 6961 6cda 066c 6179 6572 31da 066c 6179  ial..layer1..lay
+00000960: 6572 32da 066c 6179 6572 33da 066c 6179  er2..layer3..lay
+00000970: 6572 3429 0172 1300 0000 7219 0000 0072  er4).r....r....r
+00000980: 1900 0000 721a 0000 00da 0a67 6574 5f73  ....r......get_s
+00000990: 7461 6765 7331 0000 0073 0e00 0000 0002  tages1...s......
+000009a0: 0601 0c01 1201 0401 0401 04fa 7a17 5345  ............z.SE
+000009b0: 4e65 7445 6e63 6f64 6572 2e67 6574 5f73  NetEncoder.get_s
+000009c0: 7461 6765 7363 0200 0000 0000 0000 0000  tagesc..........
+000009d0: 0000 0500 0000 0400 0000 4300 0000 733a  ..........C...s:
+000009e0: 0000 007c 00a0 00a1 007d 0267 007d 0374  ...|.....}.g.}.t
+000009f0: 017c 006a 0264 0117 0083 0144 005d 1a7d  .|.j.d.....D.].}
+00000a00: 047c 027c 0419 007c 0183 017d 017c 03a0  .|.|...|...}.|..
+00000a10: 037c 01a1 0101 0071 1a7c 0353 0029 024e  .|.....q.|.S.).N
+00000a20: 7207 0000 0029 0472 2400 0000 da05 7261  r....).r$.....ra
+00000a30: 6e67 6572 0f00 0000 da06 6170 7065 6e64  nger......append
+00000a40: 2905 7213 0000 00da 0178 da06 7374 6167  ).r......x..stag
+00000a50: 6573 da08 6665 6174 7572 6573 da01 6972  es..features..ir
+00000a60: 1900 0000 7219 0000 0072 1a00 0000 da07  ....r....r......
+00000a70: 666f 7277 6172 643b 0000 0073 0c00 0000  forward;...s....
+00000a80: 0001 0802 0401 1201 0c01 0c02 7a14 5345  ............z.SE
+00000a90: 4e65 7445 6e63 6f64 6572 2e66 6f72 7761  NetEncoder.forwa
+00000aa0: 7264 6302 0000 0000 0000 0000 0000 0003  rdc.............
+00000ab0: 0000 0003 0000 000b 0000 0073 2800 0000  ...........s(...
+00000ac0: 7c01 a000 6401 a101 0100 7c01 a000 6402  |...d.....|...d.
+00000ad0: a101 0100 7401 8300 6a02 7c01 6601 7c02  ....t...j.|.f.|.
+00000ae0: 8e01 0100 6400 5300 2903 4e7a 106c 6173  ....d.S.).Nz.las
+00000af0: 745f 6c69 6e65 6172 2e62 6961 737a 126c  t_linear.biasz.l
+00000b00: 6173 745f 6c69 6e65 6172 2e77 6569 6768  ast_linear.weigh
+00000b10: 7429 03da 0370 6f70 720c 0000 00da 0f6c  t)...popr......l
+00000b20: 6f61 645f 7374 6174 655f 6469 6374 2903  oad_state_dict).
+00000b30: 7213 0000 00da 0a73 7461 7465 5f64 6963  r......state_dic
+00000b40: 7472 1600 0000 7217 0000 0072 1900 0000  tr....r....r....
+00000b50: 721a 0000 0072 2d00 0000 4500 0000 7306  r....r-...E...s.
+00000b60: 0000 0000 010a 010a 017a 1c53 454e 6574  .........z.SENet
+00000b70: 456e 636f 6465 722e 6c6f 6164 5f73 7461  Encoder.load_sta
+00000b80: 7465 5f64 6963 7429 0172 0a00 0000 2908  te_dict).r....).
+00000b90: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000ba0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000bb0: 6d65 5f5f 720d 0000 0072 2400 0000 722b  me__r....r$...r+
+00000bc0: 0000 0072 2d00 0000 da0d 5f5f 636c 6173  ...r-.....__clas
+00000bd0: 7363 656c 6c5f 5f72 1900 0000 7219 0000  scell__r....r...
+00000be0: 0072 1700 0000 721a 0000 0072 0900 0000  .r....r....r....
+00000bf0: 2600 0000 7308 0000 0008 010e 0a08 0a08  &...s...........
+00000c00: 0a72 0900 0000 da08 7365 6e65 7431 3534  .r......senet154
+00000c10: 2906 720b 0000 00e9 8000 0000 e900 0100  ).r.............
+00000c20: 00e9 0002 0000 e900 0400 00e9 0008 0000  ................
+00000c30: 679a 9999 9999 99c9 3fe9 4000 0000 720b  g.......?.@...r.
+00000c40: 0000 00e9 0800 0000 e924 0000 0069 e803  .........$...i..
+00000c50: 0000 e910 0000 0029 0772 1400 0000 da05  .......).r......
+00000c60: 626c 6f63 6bda 0964 726f 706f 7574 5f70  block..dropout_p
+00000c70: da06 6772 6f75 7073 da06 6c61 7965 7273  ..groups..layers
+00000c80: da0b 6e75 6d5f 636c 6173 7365 73da 0972  ..num_classes..r
+00000c90: 6564 7563 7469 6f6e 2903 da07 656e 636f  eduction)...enco
+00000ca0: 6465 7272 0600 0000 da06 7061 7261 6d73  derr......params
+00000cb0: da0b 7365 5f72 6573 6e65 7435 3029 0672  ..se_resnet50).r
+00000cc0: 0b00 0000 7239 0000 0072 3500 0000 7236  ....r9...r5...r6
+00000cd0: 0000 0072 3700 0000 7238 0000 00e9 0400  ...r7...r8......
+00000ce0: 0000 e906 0000 0046 290b 7214 0000 0072  .......F).r....r
+00000cf0: 3d00 0000 7240 0000 00da 1664 6f77 6e73  =...r@.....downs
+00000d00: 616d 706c 655f 6b65 726e 656c 5f73 697a  ample_kernel_siz
+00000d10: 65da 1264 6f77 6e73 616d 706c 655f 7061  e..downsample_pa
+00000d20: 6464 696e 6772 3e00 0000 723f 0000 00da  ddingr>...r?....
+00000d30: 0869 6e70 6c61 6e65 73da 0969 6e70 7574  .inplanes..input
+00000d40: 5f33 7833 7241 0000 0072 4200 0000 da0c  _3x3rA...rB.....
+00000d50: 7365 5f72 6573 6e65 7431 3031 e917 0000  se_resnet101....
+00000d60: 00da 0c73 655f 7265 736e 6574 3135 32da  ...se_resnet152.
+00000d70: 1273 655f 7265 736e 6578 7435 305f 3332  .se_resnext50_32
+00000d80: 7834 64e9 2000 0000 da13 7365 5f72 6573  x4d. .....se_res
+00000d90: 6e65 7874 3130 315f 3332 7834 6429 0672  next101_32x4d).r
+00000da0: 3300 0000 7245 0000 0072 4c00 0000 724e  3...rE...rL...rN
+00000db0: 0000 0072 4f00 0000 7251 0000 0029 0dda  ...rO...rQ...)..
+00000dc0: 075f 5f64 6f63 5f5f da08 746f 7263 682e  .__doc__..torch.
+00000dd0: 6e6e 721c 0000 005a 1d70 7265 7472 6169  nnr....Z.pretrai
+00000de0: 6e65 646d 6f64 656c 732e 6d6f 6465 6c73  nedmodels.models
+00000df0: 2e73 656e 6574 7202 0000 0072 0300 0000  .senetr....r....
+00000e00: 7204 0000 0072 0500 0000 7206 0000 00da  r....r....r.....
+00000e10: 055f 6261 7365 7208 0000 0072 0900 0000  ._baser....r....
+00000e20: da0e 7365 6e65 745f 656e 636f 6465 7273  ..senet_encoders
+00000e30: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
+00000e40: 1a00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000e50: 0000 73b6 0000 0004 190c 021c 070c 0312  ..s.............
+00000e60: 2702 0106 0202 0102 0102 0102 010a 0102  '...............
+00000e70: 0102 f904 fd04 0e02 0106 0202 0102 010a  ................
+00000e80: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00000e90: f504 fd04 1202 0106 0202 0102 010a 0102  ................
+00000ea0: 0102 0102 0102 0102 0102 0102 0102 f504  ................
+00000eb0: fd04 1202 0106 0202 0102 010a 0102 0102  ................
+00000ec0: 0102 0102 0102 0102 0102 0102 f504 fd04  ................
+00000ed0: 1202 0106 0202 0102 010a 0102 0102 0102  ................
+00000ee0: 0102 0102 0102 0102 0102 f504 fd04 1202  ................
+00000ef0: 0106 0202 0102 010a 0102 0102 0102 0102  ................
+00000f00: 0102 0102 0102 0102 f504 fd04 ae         .............
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/senet.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/senet.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:20 2023 UTC, .py size: 9053 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -129,229 +129,228 @@
 00000800: 5f6c 6179 6572 5a0b 6e6f 726d 5f6b 7761  _layerZ.norm_kwa
 00000810: 7267 73da 0964 726f 705f 7261 7465 5a0e  rgs..drop_rateZ.
 00000820: 6472 6f70 5f70 6174 685f 7261 7465 2904  drop_path_rate).
 00000830: da04 6469 6374 7203 0000 0072 0400 0000  ..dictr....r....
 00000840: 7206 0000 0029 0472 0e00 0000 da10 6465  r....).r......de
 00000850: 7074 685f 6d75 6c74 6970 6c69 6572 5a08  pth_multiplierZ.
 00000860: 6172 6368 5f64 6566 5a0c 6d6f 6465 6c5f  arch_defZ.model_
-00000870: 6b77 6172 6773 a900 7212 0000 00fa 6143  kwargs..r.....aC
+00000870: 6b77 6172 6773 a900 7212 0000 00fa 5463  kwargs..r.....Tc
 00000880: 3a5c 5573 6572 735c 6d68 616e 616e 5c44  :\Users\mhanan\D
-00000890: 6f77 6e6c 6f61 6473 5c48 616e 616e 5c4d  ownloads\Hanan\M
-000008a0: 616d 6d6f 5079 5c6d 616d 6d6f 7079 5c73  ammoPy\mammopy\s
-000008b0: 6567 6d65 6e74 6174 696f 6e5f 6d6f 6465  egmentation_mode
-000008c0: 6c73 5c65 6e63 6f64 6572 735c 7469 6d6d  ls\encoders\timm
-000008d0: 5f65 6666 6963 6965 6e74 6e65 742e 7079  _efficientnet.py
-000008e0: da17 6765 745f 6566 6669 6369 656e 746e  ..get_efficientn
-000008f0: 6574 5f6b 7761 7267 730b 0000 0073 2600  et_kwargs....s&.
-00000900: 0000 0015 0401 0401 0401 0401 0401 0401  ................
-00000910: 04f9 0409 0201 0801 0c01 0201 0201 0201  ................
-00000920: 0201 0201 02f8 060a 7214 0000 0063 0000  ........r....c..
-00000930: 0000 0000 0000 0000 0000 0000 0000 0400  ................
-00000940: 0000 0000 0000 733a 0000 0065 005a 0164  ......s:...e.Z.d
-00000950: 005a 0264 0b87 0066 0164 0364 0484 095a  .Z.d...f.d.d...Z
-00000960: 0364 0564 0684 005a 0464 0764 0884 005a  .d.d...Z.d.d...Z
-00000970: 0587 0066 0164 0964 0a84 085a 0687 0004  ...f.d.d...Z....
-00000980: 005a 0753 0029 0cda 1345 6666 6963 6965  .Z.S.)...Efficie
-00000990: 6e74 4e65 7445 6e63 6f64 6572 e905 0000  ntNetEncoder....
-000009a0: 0072 0900 0000 6306 0000 0000 0000 0000  .r....c.........
-000009b0: 0000 0007 0000 0003 0000 0003 0000 0073  ...............s
-000009c0: 3800 0000 7400 7c04 7c05 8302 7d06 7401  8...t.|.|...}.t.
-000009d0: 8300 6a02 6600 7c06 8e01 0100 7c01 7c00  ..j.f.|.....|.|.
-000009e0: 5f03 7c02 7c00 5f04 7c03 7c00 5f05 6401  _.|.|._.|.|._.d.
-000009f0: 7c00 5f06 7c00 6007 6400 5300 2902 4ee9  |._.|.`.d.S.).N.
-00000a00: 0300 0000 2908 7214 0000 00da 0573 7570  ....).r......sup
-00000a10: 6572 da08 5f5f 696e 6974 5f5f da0b 5f73  er..__init__.._s
-00000a20: 7461 6765 5f69 6478 73da 0d5f 6f75 745f  tage_idxs.._out_
-00000a30: 6368 616e 6e65 6c73 da06 5f64 6570 7468  channels.._depth
-00000a40: da0c 5f69 6e5f 6368 616e 6e65 6c73 da0a  .._in_channels..
-00000a50: 636c 6173 7369 6669 6572 2907 da04 7365  classifier)...se
-00000a60: 6c66 da0a 7374 6167 655f 6964 7873 da0c  lf..stage_idxs..
-00000a70: 6f75 745f 6368 616e 6e65 6c73 da05 6465  out_channels..de
-00000a80: 7074 6872 0e00 0000 7211 0000 00da 066b  pthr....r......k
-00000a90: 7761 7267 73a9 01da 095f 5f63 6c61 7373  wargs....__class
-00000aa0: 5f5f 7212 0000 0072 1300 0000 7219 0000  __r....r....r...
-00000ab0: 0037 0000 0073 0e00 0000 0001 0a01 0e02  .7...s..........
-00000ac0: 0601 0601 0601 0602 7a1c 4566 6669 6369  ........z.Effici
-00000ad0: 656e 744e 6574 456e 636f 6465 722e 5f5f  entNetEncoder.__
-00000ae0: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
-00000af0: 0000 0001 0000 0008 0000 0043 0000 0073  ...........C...s
-00000b00: 7000 0000 7400 a001 a100 7400 a002 7c00  p...t.....t...|.
-00000b10: 6a03 7c00 6a04 7c00 6a05 a103 7c00 6a06  j.|.j.|.j...|.j.
-00000b20: 6400 7c00 6a07 6401 1900 8502 1900 7c00  d.|.j.d.......|.
-00000b30: 6a06 7c00 6a07 6401 1900 7c00 6a07 6402  j.|.j.d...|.j.d.
-00000b40: 1900 8502 1900 7c00 6a06 7c00 6a07 6402  ......|.j.|.j.d.
-00000b50: 1900 7c00 6a07 6403 1900 8502 1900 7c00  ..|.j.d.......|.
-00000b60: 6a06 7c00 6a07 6403 1900 6400 8502 1900  j.|.j.d...d.....
-00000b70: 6706 5300 2904 4e72 0100 0000 7207 0000  g.S.).Nr....r...
-00000b80: 00e9 0200 0000 2908 da02 6e6e da08 4964  ......)...nn..Id
-00000b90: 656e 7469 7479 da0a 5365 7175 656e 7469  entity..Sequenti
-00000ba0: 616c 5a09 636f 6e76 5f73 7465 6dda 0362  alZ.conv_stem..b
-00000bb0: 6e31 5a04 6163 7431 da06 626c 6f63 6b73  n1Z.act1..blocks
-00000bc0: 721a 0000 0029 0172 1f00 0000 7212 0000  r....).r....r...
-00000bd0: 0072 1200 0000 7213 0000 00da 0a67 6574  .r....r......get
-00000be0: 5f73 7461 6765 7342 0000 0073 0e00 0000  _stagesB...s....
-00000bf0: 0002 0601 1201 1201 1801 1801 12fa 7a1e  ..............z.
-00000c00: 4566 6669 6369 656e 744e 6574 456e 636f  EfficientNetEnco
-00000c10: 6465 722e 6765 745f 7374 6167 6573 6302  der.get_stagesc.
-00000c20: 0000 0000 0000 0000 0000 0005 0000 0004  ................
-00000c30: 0000 0043 0000 0073 3a00 0000 7c00 a000  ...C...s:...|...
-00000c40: a100 7d02 6700 7d03 7401 7c00 6a02 6401  ..}.g.}.t.|.j.d.
-00000c50: 1700 8301 4400 5d1a 7d04 7c02 7c04 1900  ....D.].}.|.|...
-00000c60: 7c01 8301 7d01 7c03 a003 7c01 a101 0100  |...}.|...|.....
-00000c70: 711a 7c03 5300 2902 4e72 0700 0000 2904  q.|.S.).Nr....).
-00000c80: 722c 0000 00da 0572 616e 6765 721c 0000  r,.....ranger...
-00000c90: 00da 0661 7070 656e 6429 0572 1f00 0000  ...append).r....
-00000ca0: da01 78da 0673 7461 6765 73da 0866 6561  ..x..stages..fea
-00000cb0: 7475 7265 73da 0169 7212 0000 0072 1200  tures..ir....r..
-00000cc0: 0000 7213 0000 00da 0766 6f72 7761 7264  ..r......forward
-00000cd0: 4c00 0000 730c 0000 0000 0108 0204 0112  L...s...........
-00000ce0: 010c 010c 027a 1b45 6666 6963 6965 6e74  .....z.Efficient
-00000cf0: 4e65 7445 6e63 6f64 6572 2e66 6f72 7761  NetEncoder.forwa
-00000d00: 7264 6302 0000 0000 0000 0000 0000 0003  rdc.............
-00000d10: 0000 0003 0000 000b 0000 0073 2800 0000  ...........s(...
-00000d20: 7c01 a000 6401 a101 0100 7c01 a000 6402  |...d.....|...d.
-00000d30: a101 0100 7401 8300 6a02 7c01 6601 7c02  ....t...j.|.f.|.
-00000d40: 8e01 0100 6400 5300 2903 4e7a 0f63 6c61  ....d.S.).Nz.cla
-00000d50: 7373 6966 6965 722e 6269 6173 7a11 636c  ssifier.biasz.cl
-00000d60: 6173 7369 6669 6572 2e77 6569 6768 7429  assifier.weight)
-00000d70: 03da 0370 6f70 7218 0000 00da 0f6c 6f61  ...popr......loa
-00000d80: 645f 7374 6174 655f 6469 6374 2903 721f  d_state_dict).r.
-00000d90: 0000 00da 0a73 7461 7465 5f64 6963 7472  .....state_dictr
-00000da0: 2300 0000 7224 0000 0072 1200 0000 7213  #...r$...r....r.
-00000db0: 0000 0072 3500 0000 5600 0000 7306 0000  ...r5...V...s...
-00000dc0: 0000 010a 010a 017a 2345 6666 6963 6965  .......z#Efficie
-00000dd0: 6e74 4e65 7445 6e63 6f64 6572 2e6c 6f61  ntNetEncoder.loa
-00000de0: 645f 7374 6174 655f 6469 6374 2903 7216  d_state_dict).r.
-00000df0: 0000 0072 0900 0000 7209 0000 0029 08da  ...r....r....)..
-00000e00: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000e10: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000e20: 655f 5f72 1900 0000 722c 0000 0072 3300  e__r....r,...r3.
-00000e30: 0000 7235 0000 00da 0d5f 5f63 6c61 7373  ..r5.....__class
-00000e40: 6365 6c6c 5f5f 7212 0000 0072 1200 0000  cell__r....r....
-00000e50: 7224 0000 0072 1300 0000 7215 0000 0035  r$...r....r....5
-00000e60: 0000 0073 0800 0000 0802 0e0b 080a 080a  ...s............
-00000e70: 7215 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00000e80: 0000 0100 0000 0600 0000 4300 0000 731c  ..........C...s.
-00000e90: 0000 007c 0064 0119 007c 0064 0219 007c  ...|.d...|.d...|
-00000ea0: 0064 0319 0064 0464 0564 069c 0553 0029  .d...d.d.d...S.)
-00000eb0: 074e da04 6d65 616e da03 7374 64da 0375  .N..mean..std..u
-00000ec0: 726c 2902 7201 0000 0072 0700 0000 da03  rl).r....r......
-00000ed0: 5247 4229 0572 3b00 0000 723c 0000 0072  RGB).r;...r<...r
-00000ee0: 3d00 0000 da0b 696e 7075 745f 7261 6e67  =.....input_rang
-00000ef0: 65da 0b69 6e70 7574 5f73 7061 6365 7212  e..input_spacer.
-00000f00: 0000 0029 01da 0873 6574 7469 6e67 7372  ...)...settingsr
-00000f10: 1200 0000 7212 0000 0072 1300 0000 da10  ....r....r......
-00000f20: 7072 6570 6172 655f 7365 7474 696e 6773  prepare_settings
-00000f30: 5c00 0000 730c 0000 0000 0206 0106 0106  \...s...........
-00000f40: 0102 0102 fb72 4200 0000 5a12 7466 5f65  .....rB...Z.tf_e
-00000f50: 6666 6963 6965 6e74 6e65 745f 6230 5a15  fficientnet_b0Z.
-00000f60: 7466 5f65 6666 6963 6965 6e74 6e65 745f  tf_efficientnet_
-00000f70: 6230 5f61 705a 1574 665f 6566 6669 6369  b0_apZ.tf_effici
-00000f80: 656e 746e 6574 5f62 305f 6e73 2903 da08  entnet_b0_ns)...
-00000f90: 696d 6167 656e 6574 da07 6164 7670 726f  imagenet..advpro
-00000fa0: 70fa 0d6e 6f69 7379 2d73 7475 6465 6e74  p..noisy-student
-00000fb0: 2906 7217 0000 0072 0b00 0000 e918 0000  ).r....r........
-00000fc0: 00e9 2800 0000 e970 0000 0069 4001 0000  ..(....p...i@...
-00000fd0: 2903 7226 0000 0072 1700 0000 7216 0000  ).r&...r....r...
-00000fe0: 0029 0472 2100 0000 7220 0000 0072 0e00  .).r!...r ...r..
-00000ff0: 0000 7211 0000 0029 03da 0765 6e63 6f64  ..r....)...encod
-00001000: 6572 da13 7072 6574 7261 696e 6564 5f73  er..pretrained_s
-00001010: 6574 7469 6e67 73da 0670 6172 616d 735a  ettings..paramsZ
-00001020: 1274 665f 6566 6669 6369 656e 746e 6574  .tf_efficientnet
-00001030: 5f62 315a 1574 665f 6566 6669 6369 656e  _b1Z.tf_efficien
-00001040: 746e 6574 5f62 315f 6170 5a15 7466 5f65  tnet_b1_apZ.tf_e
-00001050: 6666 6963 6965 6e74 6e65 745f 6231 5f6e  fficientnet_b1_n
-00001060: 7367 9a99 9999 9999 f13f 5a12 7466 5f65  sg.......?Z.tf_e
-00001070: 6666 6963 6965 6e74 6e65 745f 6232 5a15  fficientnet_b2Z.
-00001080: 7466 5f65 6666 6963 6965 6e74 6e65 745f  tf_efficientnet_
-00001090: 6232 5f61 705a 1574 665f 6566 6669 6369  b2_apZ.tf_effici
-000010a0: 656e 746e 6574 5f62 325f 6e73 2906 7217  entnet_b2_ns).r.
-000010b0: 0000 0072 0b00 0000 7246 0000 00e9 3000  ...r....rF....0.
-000010c0: 0000 e978 0000 0069 6001 0000 6733 3333  ...x...i`...g333
-000010d0: 3333 33f3 3f5a 1274 665f 6566 6669 6369  333.?Z.tf_effici
-000010e0: 656e 746e 6574 5f62 335a 1574 665f 6566  entnet_b3Z.tf_ef
-000010f0: 6669 6369 656e 746e 6574 5f62 335f 6170  ficientnet_b3_ap
-00001100: 5a15 7466 5f65 6666 6963 6965 6e74 6e65  Z.tf_efficientne
-00001110: 745f 6233 5f6e 7329 0672 1700 0000 7247  t_b3_ns).r....rG
-00001120: 0000 0072 0b00 0000 724c 0000 00e9 8800  ...r....rL......
-00001130: 0000 6980 0100 0067 6666 6666 6666 f63f  ..i....gffffff.?
-00001140: 5a12 7466 5f65 6666 6963 6965 6e74 6e65  Z.tf_efficientne
-00001150: 745f 6234 5a15 7466 5f65 6666 6963 6965  t_b4Z.tf_efficie
-00001160: 6e74 6e65 745f 6234 5f61 705a 1574 665f  ntnet_b4_apZ.tf_
-00001170: 6566 6669 6369 656e 746e 6574 5f62 345f  efficientnet_b4_
-00001180: 6e73 2906 7217 0000 0072 4c00 0000 720b  ns).r....rL...r.
-00001190: 0000 00e9 3800 0000 e9a0 0000 0069 c001  ....8........i..
-000011a0: 0000 67cd cccc cccc ccfc 3f5a 1274 665f  ..g.......?Z.tf_
-000011b0: 6566 6669 6369 656e 746e 6574 5f62 355a  efficientnet_b5Z
-000011c0: 1574 665f 6566 6669 6369 656e 746e 6574  .tf_efficientnet
-000011d0: 5f62 355f 6170 5a15 7466 5f65 6666 6963  _b5_apZ.tf_effic
-000011e0: 6965 6e74 6e65 745f 6235 5f6e 7329 0672  ientnet_b5_ns).r
-000011f0: 1700 0000 724c 0000 0072 4700 0000 e940  ....rL...rG....@
-00001200: 0000 00e9 b000 0000 6900 0200 0067 9a99  ........i....g..
-00001210: 9999 9999 f93f 679a 9999 9999 9901 405a  .....?g.......@Z
-00001220: 1274 665f 6566 6669 6369 656e 746e 6574  .tf_efficientnet
-00001230: 5f62 365a 1574 665f 6566 6669 6369 656e  _b6Z.tf_efficien
-00001240: 746e 6574 5f62 365f 6170 5a15 7466 5f65  tnet_b6_apZ.tf_e
-00001250: 6666 6963 6965 6e74 6e65 745f 6236 5f6e  fficientnet_b6_n
-00001260: 7329 0672 1700 0000 724f 0000 0072 4700  s).r....rO...rG.
-00001270: 0000 e948 0000 00e9 c800 0000 6940 0200  ...H........i@..
-00001280: 0067 cdcc cccc cccc 0440 5a12 7466 5f65  .g.......@Z.tf_e
-00001290: 6666 6963 6965 6e74 6e65 745f 6237 5a15  fficientnet_b7Z.
-000012a0: 7466 5f65 6666 6963 6965 6e74 6e65 745f  tf_efficientnet_
-000012b0: 6237 5f61 705a 1574 665f 6566 6669 6369  b7_apZ.tf_effici
-000012c0: 656e 746e 6574 5f62 375f 6e73 2906 7217  entnet_b7_ns).r.
-000012d0: 0000 0072 5100 0000 724c 0000 00e9 5000  ...rQ...rL....P.
-000012e0: 0000 e9e0 0000 0069 8002 0000 6700 0000  .......i....g...
-000012f0: 0000 0000 4067 cdcc cccc cccc 0840 5a12  ....@g.......@Z.
-00001300: 7466 5f65 6666 6963 6965 6e74 6e65 745f  tf_efficientnet_
-00001310: 6238 5a15 7466 5f65 6666 6963 6965 6e74  b8Z.tf_efficient
-00001320: 6e65 745f 6238 5f61 7029 0272 4300 0000  net_b8_ap).rC...
-00001330: 7244 0000 0029 0672 1700 0000 7253 0000  rD...).r....rS..
-00001340: 0072 4f00 0000 e958 0000 00e9 f800 0000  .rO....X........
-00001350: 69c0 0200 0067 cdcc cccc cccc 0c40 7245  i....g.......@rE
-00001360: 0000 005a 1574 665f 6566 6669 6369 656e  ...Z.tf_efficien
-00001370: 746e 6574 5f6c 325f 6e73 2906 7217 0000  tnet_l2_ns).r...
-00001380: 0072 4e00 0000 e968 0000 0072 5200 0000  .rN....h...rR...
-00001390: 69e0 0100 0069 6005 0000 6733 3333 3333  i....i`...g33333
-000013a0: 3311 4067 3333 3333 3333 1540 290a 7a14  3.@g333333.@).z.
-000013b0: 7469 6d6d 2d65 6666 6963 6965 6e74 6e65  timm-efficientne
-000013c0: 742d 6230 7a14 7469 6d6d 2d65 6666 6963  t-b0z.timm-effic
-000013d0: 6965 6e74 6e65 742d 6231 7a14 7469 6d6d  ientnet-b1z.timm
-000013e0: 2d65 6666 6963 6965 6e74 6e65 742d 6232  -efficientnet-b2
-000013f0: 7a14 7469 6d6d 2d65 6666 6963 6965 6e74  z.timm-efficient
-00001400: 6e65 742d 6233 7a14 7469 6d6d 2d65 6666  net-b3z.timm-eff
-00001410: 6963 6965 6e74 6e65 742d 6234 7a14 7469  icientnet-b4z.ti
-00001420: 6d6d 2d65 6666 6963 6965 6e74 6e65 742d  mm-efficientnet-
-00001430: 6235 7a14 7469 6d6d 2d65 6666 6963 6965  b5z.timm-efficie
-00001440: 6e74 6e65 742d 6236 7a14 7469 6d6d 2d65  ntnet-b6z.timm-e
-00001450: 6666 6963 6965 6e74 6e65 742d 6237 7a14  fficientnet-b7z.
-00001460: 7469 6d6d 2d65 6666 6963 6965 6e74 6e65  timm-efficientne
-00001470: 742d 6238 7a14 7469 6d6d 2d65 6666 6963  t-b8z.timm-effic
-00001480: 6965 6e74 6e65 742d 6c32 2902 7209 0000  ientnet-l2).r...
-00001490: 0072 0900 0000 2910 da05 746f 7263 68da  .r....)...torch.
-000014a0: 0874 6f72 6368 2e6e 6e72 2700 0000 5a18  .torch.nnr'...Z.
-000014b0: 7469 6d6d 2e6d 6f64 656c 732e 6566 6669  timm.models.effi
-000014c0: 6369 656e 746e 6574 7202 0000 0072 0300  cientnetr....r..
-000014d0: 0000 7204 0000 0072 0500 0000 5a1e 7469  ..r....r....Z.ti
-000014e0: 6d6d 2e6d 6f64 656c 732e 6c61 7965 7273  mm.models.layers
-000014f0: 2e61 6374 6976 6174 696f 6e73 7206 0000  .activationsr...
-00001500: 00da 055f 6261 7365 7208 0000 0072 1400  ..._baser....r..
-00001510: 0000 7215 0000 0072 4200 0000 da1a 7469  ..r....rB.....ti
-00001520: 6d6d 5f65 6666 6963 6965 6e74 6e65 745f  mm_efficientnet_
-00001530: 656e 636f 6465 7273 7212 0000 0072 1200  encodersr....r..
-00001540: 0000 7212 0000 0072 1300 0000 da08 3c6d  ..r....r......<m
-00001550: 6f64 756c 653e 0100 0000 73ec 0000 0008  odule>....s.....
-00001560: 010c 020c 0114 010c 020c 030a 2a12 2708  ............*.'.
-00001570: 0d02 020a 010a 010a fd04 0602 0102 0102  ................
-00001580: 0102 fc04 f904 1002 020a 010a 010a fd04  ................
-00001590: 0602 0102 0102 0102 fc04 f904 1002 020a  ................
-000015a0: 010a 010a fd04 0602 0102 0102 0102 fc04  ................
-000015b0: f904 1002 020a 010a 010a fd04 0602 0102  ................
-000015c0: 0102 0102 fc04 f904 1002 020a 010a 010a  ................
-000015d0: fd04 0602 0102 0102 0102 fc04 f904 1002  ................
-000015e0: 020a 010a 010a fd04 0602 0102 0102 0102  ................
-000015f0: fc04 f904 1002 020a 010a 010a fd04 0602  ................
-00001600: 0102 0102 0102 fc04 f904 1002 020a 010a  ................
-00001610: 010a fd04 0602 0102 0102 0102 fc04 f904  ................
-00001620: 1002 020a 010a fe04 0502 0102 0102 0102  ................
-00001630: fc04 fa04 0f02 0202 000a ff02 0402 0102  ................
-00001640: 0102 0102 fc04 fb04 8000 f8              ...........
+00000890: 6f77 6e6c 6f61 6473 5c48 616e 616e 5c6d  ownloads\Hanan\m
+000008a0: 675c 7365 676d 656e 7461 7469 6f6e 5f6d  g\segmentation_m
+000008b0: 6f64 656c 735c 656e 636f 6465 7273 5c74  odels\encoders\t
+000008c0: 696d 6d5f 6566 6669 6369 656e 746e 6574  imm_efficientnet
+000008d0: 2e70 79da 1767 6574 5f65 6666 6963 6965  .py..get_efficie
+000008e0: 6e74 6e65 745f 6b77 6172 6773 0b00 0000  ntnet_kwargs....
+000008f0: 7326 0000 0000 1504 0104 0104 0104 0104  s&..............
+00000900: 0104 0104 f904 0902 0108 010c 0102 0102  ................
+00000910: 0102 0102 0102 0102 f806 0a72 1400 0000  ...........r....
+00000920: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000930: 0004 0000 0000 0000 0073 3a00 0000 6500  .........s:...e.
+00000940: 5a01 6400 5a02 640b 8700 6601 6403 6404  Z.d.Z.d...f.d.d.
+00000950: 8409 5a03 6405 6406 8400 5a04 6407 6408  ..Z.d.d...Z.d.d.
+00000960: 8400 5a05 8700 6601 6409 640a 8408 5a06  ..Z...f.d.d...Z.
+00000970: 8700 0400 5a07 5300 290c da13 4566 6669  ....Z.S.)...Effi
+00000980: 6369 656e 744e 6574 456e 636f 6465 72e9  cientNetEncoder.
+00000990: 0500 0000 7209 0000 0063 0600 0000 0000  ....r....c......
+000009a0: 0000 0000 0000 0700 0000 0300 0000 0300  ................
+000009b0: 0000 7338 0000 0074 007c 047c 0583 027d  ..s8...t.|.|...}
+000009c0: 0674 0183 006a 0266 007c 068e 0101 007c  .t...j.f.|.....|
+000009d0: 017c 005f 037c 027c 005f 047c 037c 005f  .|._.|.|._.|.|._
+000009e0: 0564 017c 005f 067c 0060 0764 0053 0029  .d.|._.|.`.d.S.)
+000009f0: 024e e903 0000 0029 0872 1400 0000 da05  .N.....).r......
+00000a00: 7375 7065 72da 085f 5f69 6e69 745f 5fda  super..__init__.
+00000a10: 0b5f 7374 6167 655f 6964 7873 da0d 5f6f  ._stage_idxs.._o
+00000a20: 7574 5f63 6861 6e6e 656c 73da 065f 6465  ut_channels.._de
+00000a30: 7074 68da 0c5f 696e 5f63 6861 6e6e 656c  pth.._in_channel
+00000a40: 73da 0a63 6c61 7373 6966 6965 7229 07da  s..classifier)..
+00000a50: 0473 656c 66da 0a73 7461 6765 5f69 6478  .self..stage_idx
+00000a60: 73da 0c6f 7574 5f63 6861 6e6e 656c 73da  s..out_channels.
+00000a70: 0564 6570 7468 720e 0000 0072 1100 0000  .depthr....r....
+00000a80: da06 6b77 6172 6773 a901 da09 5f5f 636c  ..kwargs....__cl
+00000a90: 6173 735f 5f72 1200 0000 7213 0000 0072  ass__r....r....r
+00000aa0: 1900 0000 3700 0000 730e 0000 0000 010a  ....7...s.......
+00000ab0: 010e 0206 0106 0106 0106 027a 1c45 6666  ...........z.Eff
+00000ac0: 6963 6965 6e74 4e65 7445 6e63 6f64 6572  icientNetEncoder
+00000ad0: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
+00000ae0: 0000 0000 0000 0100 0000 0800 0000 4300  ..............C.
+00000af0: 0000 7370 0000 0074 00a0 01a1 0074 00a0  ..sp...t.....t..
+00000b00: 027c 006a 037c 006a 047c 006a 05a1 037c  .|.j.|.j.|.j...|
+00000b10: 006a 0664 007c 006a 0764 0119 0085 0219  .j.d.|.j.d......
+00000b20: 007c 006a 067c 006a 0764 0119 007c 006a  .|.j.|.j.d...|.j
+00000b30: 0764 0219 0085 0219 007c 006a 067c 006a  .d.......|.j.|.j
+00000b40: 0764 0219 007c 006a 0764 0319 0085 0219  .d...|.j.d......
+00000b50: 007c 006a 067c 006a 0764 0319 0064 0085  .|.j.|.j.d...d..
+00000b60: 0219 0067 0653 0029 044e 7201 0000 0072  ...g.S.).Nr....r
+00000b70: 0700 0000 e902 0000 0029 08da 026e 6eda  .........)...nn.
+00000b80: 0849 6465 6e74 6974 79da 0a53 6571 7565  .Identity..Seque
+00000b90: 6e74 6961 6c5a 0963 6f6e 765f 7374 656d  ntialZ.conv_stem
+00000ba0: da03 626e 315a 0461 6374 31da 0662 6c6f  ..bn1Z.act1..blo
+00000bb0: 636b 7372 1a00 0000 2901 721f 0000 0072  cksr....).r....r
+00000bc0: 1200 0000 7212 0000 0072 1300 0000 da0a  ....r....r......
+00000bd0: 6765 745f 7374 6167 6573 4200 0000 730e  get_stagesB...s.
+00000be0: 0000 0000 0206 0112 0112 0118 0118 0112  ................
+00000bf0: fa7a 1e45 6666 6963 6965 6e74 4e65 7445  .z.EfficientNetE
+00000c00: 6e63 6f64 6572 2e67 6574 5f73 7461 6765  ncoder.get_stage
+00000c10: 7363 0200 0000 0000 0000 0000 0000 0500  sc..............
+00000c20: 0000 0400 0000 4300 0000 733a 0000 007c  ......C...s:...|
+00000c30: 00a0 00a1 007d 0267 007d 0374 017c 006a  .....}.g.}.t.|.j
+00000c40: 0264 0117 0083 0144 005d 1a7d 047c 027c  .d.....D.].}.|.|
+00000c50: 0419 007c 0183 017d 017c 03a0 037c 01a1  ...|...}.|...|..
+00000c60: 0101 0071 1a7c 0353 0029 024e 7207 0000  ...q.|.S.).Nr...
+00000c70: 0029 0472 2c00 0000 da05 7261 6e67 6572  .).r,.....ranger
+00000c80: 1c00 0000 da06 6170 7065 6e64 2905 721f  ......append).r.
+00000c90: 0000 00da 0178 da06 7374 6167 6573 da08  .....x..stages..
+00000ca0: 6665 6174 7572 6573 da01 6972 1200 0000  features..ir....
+00000cb0: 7212 0000 0072 1300 0000 da07 666f 7277  r....r......forw
+00000cc0: 6172 644c 0000 0073 0c00 0000 0001 0802  ardL...s........
+00000cd0: 0401 1201 0c01 0c02 7a1b 4566 6669 6369  ........z.Effici
+00000ce0: 656e 744e 6574 456e 636f 6465 722e 666f  entNetEncoder.fo
+00000cf0: 7277 6172 6463 0200 0000 0000 0000 0000  rwardc..........
+00000d00: 0000 0300 0000 0300 0000 0b00 0000 7328  ..............s(
+00000d10: 0000 007c 01a0 0064 01a1 0101 007c 01a0  ...|...d.....|..
+00000d20: 0064 02a1 0101 0074 0183 006a 027c 0166  .d.....t...j.|.f
+00000d30: 017c 028e 0101 0064 0053 0029 034e 7a0f  .|.....d.S.).Nz.
+00000d40: 636c 6173 7369 6669 6572 2e62 6961 737a  classifier.biasz
+00000d50: 1163 6c61 7373 6966 6965 722e 7765 6967  .classifier.weig
+00000d60: 6874 2903 da03 706f 7072 1800 0000 da0f  ht)...popr......
+00000d70: 6c6f 6164 5f73 7461 7465 5f64 6963 7429  load_state_dict)
+00000d80: 0372 1f00 0000 da0a 7374 6174 655f 6469  .r......state_di
+00000d90: 6374 7223 0000 0072 2400 0000 7212 0000  ctr#...r$...r...
+00000da0: 0072 1300 0000 7235 0000 0056 0000 0073  .r....r5...V...s
+00000db0: 0600 0000 0001 0a01 0a01 7a23 4566 6669  ..........z#Effi
+00000dc0: 6369 656e 744e 6574 456e 636f 6465 722e  cientNetEncoder.
+00000dd0: 6c6f 6164 5f73 7461 7465 5f64 6963 7429  load_state_dict)
+00000de0: 0372 1600 0000 7209 0000 0072 0900 0000  .r....r....r....
+00000df0: 2908 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00000e00: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00000e10: 6e61 6d65 5f5f 7219 0000 0072 2c00 0000  name__r....r,...
+00000e20: 7233 0000 0072 3500 0000 da0d 5f5f 636c  r3...r5.....__cl
+00000e30: 6173 7363 656c 6c5f 5f72 1200 0000 7212  asscell__r....r.
+00000e40: 0000 0072 2400 0000 7213 0000 0072 1500  ...r$...r....r..
+00000e50: 0000 3500 0000 7308 0000 0008 020e 0b08  ..5...s.........
+00000e60: 0a08 0a72 1500 0000 6301 0000 0000 0000  ...r....c.......
+00000e70: 0000 0000 0001 0000 0006 0000 0043 0000  .............C..
+00000e80: 0073 1c00 0000 7c00 6401 1900 7c00 6402  .s....|.d...|.d.
+00000e90: 1900 7c00 6403 1900 6404 6405 6406 9c05  ..|.d...d.d.d...
+00000ea0: 5300 2907 4eda 046d 6561 6eda 0373 7464  S.).N..mean..std
+00000eb0: da03 7572 6c29 0272 0100 0000 7207 0000  ..url).r....r...
+00000ec0: 00da 0352 4742 2905 723b 0000 0072 3c00  ...RGB).r;...r<.
+00000ed0: 0000 723d 0000 00da 0b69 6e70 7574 5f72  ..r=.....input_r
+00000ee0: 616e 6765 da0b 696e 7075 745f 7370 6163  ange..input_spac
+00000ef0: 6572 1200 0000 2901 da08 7365 7474 696e  er....)...settin
+00000f00: 6773 7212 0000 0072 1200 0000 7213 0000  gsr....r....r...
+00000f10: 00da 1070 7265 7061 7265 5f73 6574 7469  ...prepare_setti
+00000f20: 6e67 735c 0000 0073 0c00 0000 0002 0601  ngs\...s........
+00000f30: 0601 0601 0201 02fb 7242 0000 005a 1274  ........rB...Z.t
+00000f40: 665f 6566 6669 6369 656e 746e 6574 5f62  f_efficientnet_b
+00000f50: 305a 1574 665f 6566 6669 6369 656e 746e  0Z.tf_efficientn
+00000f60: 6574 5f62 305f 6170 5a15 7466 5f65 6666  et_b0_apZ.tf_eff
+00000f70: 6963 6965 6e74 6e65 745f 6230 5f6e 7329  icientnet_b0_ns)
+00000f80: 03da 0869 6d61 6765 6e65 74da 0761 6476  ...imagenet..adv
+00000f90: 7072 6f70 fa0d 6e6f 6973 792d 7374 7564  prop..noisy-stud
+00000fa0: 656e 7429 0672 1700 0000 720b 0000 00e9  ent).r....r.....
+00000fb0: 1800 0000 e928 0000 00e9 7000 0000 6940  .....(....p...i@
+00000fc0: 0100 0029 0372 2600 0000 7217 0000 0072  ...).r&...r....r
+00000fd0: 1600 0000 2904 7221 0000 0072 2000 0000  ....).r!...r ...
+00000fe0: 720e 0000 0072 1100 0000 2903 da07 656e  r....r....)...en
+00000ff0: 636f 6465 72da 1370 7265 7472 6169 6e65  coder..pretraine
+00001000: 645f 7365 7474 696e 6773 da06 7061 7261  d_settings..para
+00001010: 6d73 5a12 7466 5f65 6666 6963 6965 6e74  msZ.tf_efficient
+00001020: 6e65 745f 6231 5a15 7466 5f65 6666 6963  net_b1Z.tf_effic
+00001030: 6965 6e74 6e65 745f 6231 5f61 705a 1574  ientnet_b1_apZ.t
+00001040: 665f 6566 6669 6369 656e 746e 6574 5f62  f_efficientnet_b
+00001050: 315f 6e73 679a 9999 9999 99f1 3f5a 1274  1_nsg.......?Z.t
+00001060: 665f 6566 6669 6369 656e 746e 6574 5f62  f_efficientnet_b
+00001070: 325a 1574 665f 6566 6669 6369 656e 746e  2Z.tf_efficientn
+00001080: 6574 5f62 325f 6170 5a15 7466 5f65 6666  et_b2_apZ.tf_eff
+00001090: 6963 6965 6e74 6e65 745f 6232 5f6e 7329  icientnet_b2_ns)
+000010a0: 0672 1700 0000 720b 0000 0072 4600 0000  .r....r....rF...
+000010b0: e930 0000 00e9 7800 0000 6960 0100 0067  .0....x...i`...g
+000010c0: 3333 3333 3333 f33f 5a12 7466 5f65 6666  333333.?Z.tf_eff
+000010d0: 6963 6965 6e74 6e65 745f 6233 5a15 7466  icientnet_b3Z.tf
+000010e0: 5f65 6666 6963 6965 6e74 6e65 745f 6233  _efficientnet_b3
+000010f0: 5f61 705a 1574 665f 6566 6669 6369 656e  _apZ.tf_efficien
+00001100: 746e 6574 5f62 335f 6e73 2906 7217 0000  tnet_b3_ns).r...
+00001110: 0072 4700 0000 720b 0000 0072 4c00 0000  .rG...r....rL...
+00001120: e988 0000 0069 8001 0000 6766 6666 6666  .....i....gfffff
+00001130: 66f6 3f5a 1274 665f 6566 6669 6369 656e  f.?Z.tf_efficien
+00001140: 746e 6574 5f62 345a 1574 665f 6566 6669  tnet_b4Z.tf_effi
+00001150: 6369 656e 746e 6574 5f62 345f 6170 5a15  cientnet_b4_apZ.
+00001160: 7466 5f65 6666 6963 6965 6e74 6e65 745f  tf_efficientnet_
+00001170: 6234 5f6e 7329 0672 1700 0000 724c 0000  b4_ns).r....rL..
+00001180: 0072 0b00 0000 e938 0000 00e9 a000 0000  .r.....8........
+00001190: 69c0 0100 0067 cdcc cccc cccc fc3f 5a12  i....g.......?Z.
+000011a0: 7466 5f65 6666 6963 6965 6e74 6e65 745f  tf_efficientnet_
+000011b0: 6235 5a15 7466 5f65 6666 6963 6965 6e74  b5Z.tf_efficient
+000011c0: 6e65 745f 6235 5f61 705a 1574 665f 6566  net_b5_apZ.tf_ef
+000011d0: 6669 6369 656e 746e 6574 5f62 355f 6e73  ficientnet_b5_ns
+000011e0: 2906 7217 0000 0072 4c00 0000 7247 0000  ).r....rL...rG..
+000011f0: 00e9 4000 0000 e9b0 0000 0069 0002 0000  ..@........i....
+00001200: 679a 9999 9999 99f9 3f67 9a99 9999 9999  g.......?g......
+00001210: 0140 5a12 7466 5f65 6666 6963 6965 6e74  .@Z.tf_efficient
+00001220: 6e65 745f 6236 5a15 7466 5f65 6666 6963  net_b6Z.tf_effic
+00001230: 6965 6e74 6e65 745f 6236 5f61 705a 1574  ientnet_b6_apZ.t
+00001240: 665f 6566 6669 6369 656e 746e 6574 5f62  f_efficientnet_b
+00001250: 365f 6e73 2906 7217 0000 0072 4f00 0000  6_ns).r....rO...
+00001260: 7247 0000 00e9 4800 0000 e9c8 0000 0069  rG....H........i
+00001270: 4002 0000 67cd cccc cccc cc04 405a 1274  @...g.......@Z.t
+00001280: 665f 6566 6669 6369 656e 746e 6574 5f62  f_efficientnet_b
+00001290: 375a 1574 665f 6566 6669 6369 656e 746e  7Z.tf_efficientn
+000012a0: 6574 5f62 375f 6170 5a15 7466 5f65 6666  et_b7_apZ.tf_eff
+000012b0: 6963 6965 6e74 6e65 745f 6237 5f6e 7329  icientnet_b7_ns)
+000012c0: 0672 1700 0000 7251 0000 0072 4c00 0000  .r....rQ...rL...
+000012d0: e950 0000 00e9 e000 0000 6980 0200 0067  .P........i....g
+000012e0: 0000 0000 0000 0040 67cd cccc cccc cc08  .......@g.......
+000012f0: 405a 1274 665f 6566 6669 6369 656e 746e  @Z.tf_efficientn
+00001300: 6574 5f62 385a 1574 665f 6566 6669 6369  et_b8Z.tf_effici
+00001310: 656e 746e 6574 5f62 385f 6170 2902 7243  entnet_b8_ap).rC
+00001320: 0000 0072 4400 0000 2906 7217 0000 0072  ...rD...).r....r
+00001330: 5300 0000 724f 0000 00e9 5800 0000 e9f8  S...rO....X.....
+00001340: 0000 0069 c002 0000 67cd cccc cccc cc0c  ...i....g.......
+00001350: 4072 4500 0000 5a15 7466 5f65 6666 6963  @rE...Z.tf_effic
+00001360: 6965 6e74 6e65 745f 6c32 5f6e 7329 0672  ientnet_l2_ns).r
+00001370: 1700 0000 724e 0000 00e9 6800 0000 7252  ....rN....h...rR
+00001380: 0000 0069 e001 0000 6960 0500 0067 3333  ...i....i`...g33
+00001390: 3333 3333 1140 6733 3333 3333 3315 4029  3333.@g333333.@)
+000013a0: 0a7a 1474 696d 6d2d 6566 6669 6369 656e  .z.timm-efficien
+000013b0: 746e 6574 2d62 307a 1474 696d 6d2d 6566  tnet-b0z.timm-ef
+000013c0: 6669 6369 656e 746e 6574 2d62 317a 1474  ficientnet-b1z.t
+000013d0: 696d 6d2d 6566 6669 6369 656e 746e 6574  imm-efficientnet
+000013e0: 2d62 327a 1474 696d 6d2d 6566 6669 6369  -b2z.timm-effici
+000013f0: 656e 746e 6574 2d62 337a 1474 696d 6d2d  entnet-b3z.timm-
+00001400: 6566 6669 6369 656e 746e 6574 2d62 347a  efficientnet-b4z
+00001410: 1474 696d 6d2d 6566 6669 6369 656e 746e  .timm-efficientn
+00001420: 6574 2d62 357a 1474 696d 6d2d 6566 6669  et-b5z.timm-effi
+00001430: 6369 656e 746e 6574 2d62 367a 1474 696d  cientnet-b6z.tim
+00001440: 6d2d 6566 6669 6369 656e 746e 6574 2d62  m-efficientnet-b
+00001450: 377a 1474 696d 6d2d 6566 6669 6369 656e  7z.timm-efficien
+00001460: 746e 6574 2d62 387a 1474 696d 6d2d 6566  tnet-b8z.timm-ef
+00001470: 6669 6369 656e 746e 6574 2d6c 3229 0272  ficientnet-l2).r
+00001480: 0900 0000 7209 0000 0029 10da 0574 6f72  ....r....)...tor
+00001490: 6368 da08 746f 7263 682e 6e6e 7227 0000  ch..torch.nnr'..
+000014a0: 005a 1874 696d 6d2e 6d6f 6465 6c73 2e65  .Z.timm.models.e
+000014b0: 6666 6963 6965 6e74 6e65 7472 0200 0000  fficientnetr....
+000014c0: 7203 0000 0072 0400 0000 7205 0000 005a  r....r....r....Z
+000014d0: 1e74 696d 6d2e 6d6f 6465 6c73 2e6c 6179  .timm.models.lay
+000014e0: 6572 732e 6163 7469 7661 7469 6f6e 7372  ers.activationsr
+000014f0: 0600 0000 da05 5f62 6173 6572 0800 0000  ......_baser....
+00001500: 7214 0000 0072 1500 0000 7242 0000 00da  r....r....rB....
+00001510: 1a74 696d 6d5f 6566 6669 6369 656e 746e  .timm_efficientn
+00001520: 6574 5f65 6e63 6f64 6572 7372 1200 0000  et_encodersr....
+00001530: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
+00001540: 083c 6d6f 6475 6c65 3e01 0000 0073 ec00  .<module>....s..
+00001550: 0000 0801 0c02 0c01 1401 0c02 0c03 0a2a  ...............*
+00001560: 1227 080d 0202 0a01 0a01 0afd 0406 0201  .'..............
+00001570: 0201 0201 02fc 04f9 0410 0202 0a01 0a01  ................
+00001580: 0afd 0406 0201 0201 0201 02fc 04f9 0410  ................
+00001590: 0202 0a01 0a01 0afd 0406 0201 0201 0201  ................
+000015a0: 02fc 04f9 0410 0202 0a01 0a01 0afd 0406  ................
+000015b0: 0201 0201 0201 02fc 04f9 0410 0202 0a01  ................
+000015c0: 0a01 0afd 0406 0201 0201 0201 02fc 04f9  ................
+000015d0: 0410 0202 0a01 0a01 0afd 0406 0201 0201  ................
+000015e0: 0201 02fc 04f9 0410 0202 0a01 0a01 0afd  ................
+000015f0: 0406 0201 0201 0201 02fc 04f9 0410 0202  ................
+00001600: 0a01 0a01 0afd 0406 0201 0201 0201 02fc  ................
+00001610: 04f9 0410 0202 0a01 0afe 0405 0201 0201  ................
+00001620: 0201 02fc 04fa 040f 0202 0200 0aff 0204  ................
+00001630: 0201 0201 0201 02fc 04fb 0480 00f8       ..............
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/timm_efficientnet.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/vgg.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/vgg.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/vgg.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/vgg.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/vgg.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/vgg.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/vgg.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/vgg.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:20 2023 UTC, .py size: 5637 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -135,120 +135,119 @@
 00000860: 5f5f 7203 0000 00da 0d5f 6f75 745f 6368  __r......_out_ch
 00000870: 616e 6e65 6c73 da06 5f64 6570 7468 da0c  annels.._depth..
 00000880: 5f69 6e5f 6368 616e 6e65 6c73 da0a 636c  _in_channels..cl
 00000890: 6173 7369 6669 6572 2906 da04 7365 6c66  assifier)...self
 000008a0: da0c 6f75 745f 6368 616e 6e65 6c73 da06  ..out_channels..
 000008b0: 636f 6e66 6967 7212 0000 00da 0564 6570  configr......dep
 000008c0: 7468 da06 6b77 6172 6773 a901 da09 5f5f  th..kwargs....__
-000008d0: 636c 6173 735f 5fa9 00fa 5343 3a5c 5573  class__...SC:\Us
+000008d0: 636c 6173 735f 5fa9 00fa 4663 3a5c 5573  class__...Fc:\Us
 000008e0: 6572 735c 6d68 616e 616e 5c44 6f77 6e6c  ers\mhanan\Downl
-000008f0: 6f61 6473 5c48 616e 616e 5c4d 616d 6d6f  oads\Hanan\Mammo
-00000900: 5079 5c6d 616d 6d6f 7079 5c73 6567 6d65  Py\mammopy\segme
-00000910: 6e74 6174 696f 6e5f 6d6f 6465 6c73 5c65  ntation_models\e
-00000920: 6e63 6f64 6572 735c 7667 672e 7079 7215  ncoders\vgg.pyr.
-00000930: 0000 002c 0000 0073 0a00 0000 0001 1801  ...,...s........
-00000940: 0601 0601 0601 7a13 5647 4745 6e63 6f64  ......z.VGGEncod
-00000950: 6572 2e5f 5f69 6e69 745f 5f63 0300 0000  er.__init__c....
-00000960: 0000 0000 0000 0000 0300 0000 0200 0000  ................
-00000970: 4300 0000 730c 0000 0074 0064 0183 0182  C...s....t.d....
-00000980: 0164 0053 0029 024e 7a58 2756 4747 2720  .d.S.).NzX'VGG' 
-00000990: 6d6f 6465 6c73 2064 6f20 6e6f 7420 7375  models do not su
-000009a0: 7070 6f72 7420 6469 6c61 7465 6420 6d6f  pport dilated mo
-000009b0: 6465 2064 7565 2074 6f20 4d61 7820 506f  de due to Max Po
-000009c0: 6f6c 696e 6720 6f70 6572 6174 696f 6e73  oling operations
-000009d0: 2066 6f72 2064 6f77 6e73 616d 706c 696e   for downsamplin
-000009e0: 6721 2901 da0a 5661 6c75 6545 7272 6f72  g!)...ValueError
-000009f0: 2903 721a 0000 00da 0a73 7461 6765 5f6c  ).r......stage_l
-00000a00: 6973 74da 0d64 696c 6174 696f 6e5f 6c69  ist..dilation_li
-00000a10: 7374 7221 0000 0072 2100 0000 7222 0000  str!...r!...r"..
-00000a20: 00da 0c6d 616b 655f 6469 6c61 7465 6433  ...make_dilated3
-00000a30: 0000 0073 0200 0000 0001 7a17 5647 4745  ...s......z.VGGE
-00000a40: 6e63 6f64 6572 2e6d 616b 655f 6469 6c61  ncoder.make_dila
-00000a50: 7465 6463 0100 0000 0000 0000 0000 0000  tedc............
-00000a60: 0400 0000 0500 0000 4300 0000 7352 0000  ........C...sR..
-00000a70: 0067 007d 0167 007d 027c 006a 0044 005d  .g.}.g.}.|.j.D.]
-00000a80: 2e7d 0374 017c 0374 026a 0383 0272 327c  .}.t.|.t.j...r2|
-00000a90: 01a0 0474 026a 057c 028e 00a1 0101 0067  ...t.j.|.......g
-00000aa0: 007d 027c 02a0 047c 03a1 0101 0071 0e7c  .}.|...|.....q.|
-00000ab0: 01a0 0474 026a 057c 028e 00a1 0101 007c  ...t.j.|.......|
-00000ac0: 0153 0029 014e 2906 da08 6665 6174 7572  .S.).N)...featur
-00000ad0: 6573 da0a 6973 696e 7374 616e 6365 da02  es..isinstance..
-00000ae0: 6e6e da09 4d61 7850 6f6f 6c32 64da 0661  nn..MaxPool2d..a
-00000af0: 7070 656e 64da 0a53 6571 7565 6e74 6961  ppend..Sequentia
-00000b00: 6c29 0472 1a00 0000 da06 7374 6167 6573  l).r......stages
-00000b10: 5a0d 7374 6167 655f 6d6f 6475 6c65 73da  Z.stage_modules.
-00000b20: 066d 6f64 756c 6572 2100 0000 7221 0000  .moduler!...r!..
-00000b30: 0072 2200 0000 da0a 6765 745f 7374 6167  .r".....get_stag
-00000b40: 6573 3700 0000 7312 0000 0000 0104 0104  es7...s.........
-00000b50: 010a 010c 0110 0104 010c 0110 017a 1556  .............z.V
-00000b60: 4747 456e 636f 6465 722e 6765 745f 7374  GGEncoder.get_st
-00000b70: 6167 6573 6302 0000 0000 0000 0000 0000  agesc...........
-00000b80: 0005 0000 0004 0000 0043 0000 0073 3a00  .........C...s:.
-00000b90: 0000 7c00 a000 a100 7d02 6700 7d03 7401  ..|.....}.g.}.t.
-00000ba0: 7c00 6a02 6401 1700 8301 4400 5d1a 7d04  |.j.d.....D.].}.
-00000bb0: 7c02 7c04 1900 7c01 8301 7d01 7c03 a003  |.|...|...}.|...
-00000bc0: 7c01 a101 0100 711a 7c03 5300 2902 4e72  |.....q.|.S.).Nr
-00000bd0: 0500 0000 2904 722f 0000 00da 0572 616e  ....).r/.....ran
-00000be0: 6765 7217 0000 0072 2b00 0000 2905 721a  ger....r+...).r.
-00000bf0: 0000 00da 0178 722d 0000 0072 2700 0000  .....xr-...r'...
-00000c00: da01 6972 2100 0000 7221 0000 0072 2200  ..ir!...r!...r".
-00000c10: 0000 da07 666f 7277 6172 6442 0000 0073  ....forwardB...s
-00000c20: 0c00 0000 0001 0802 0401 1201 0c01 0c02  ................
-00000c30: 7a12 5647 4745 6e63 6f64 6572 2e66 6f72  z.VGGEncoder.for
-00000c40: 7761 7264 6302 0000 0000 0000 0000 0000  wardc...........
-00000c50: 0005 0000 0004 0000 000b 0000 0073 3e00  .............s>.
-00000c60: 0000 7400 7c01 a001 a100 8301 7d03 7c03  ..t.|.......}.|.
-00000c70: 4400 5d18 7d04 7c04 a002 6401 a101 7210  D.].}.|...d...r.
-00000c80: 7c01 a003 7c04 a101 0100 7110 7404 8300  |...|.....q.t...
-00000c90: 6a05 7c01 6601 7c02 8e01 0100 6400 5300  j.|.f.|.....d.S.
-00000ca0: 2902 4e72 1900 0000 2906 da04 6c69 7374  ).Nr....)...list
-00000cb0: da04 6b65 7973 da0a 7374 6172 7473 7769  ..keys..startswi
-00000cc0: 7468 da03 706f 7072 1400 0000 da0f 6c6f  th..popr......lo
-00000cd0: 6164 5f73 7461 7465 5f64 6963 7429 0572  ad_state_dict).r
-00000ce0: 1a00 0000 da0a 7374 6174 655f 6469 6374  ......state_dict
-00000cf0: 721e 0000 0072 3500 0000 da01 6b72 1f00  r....r5.....kr..
-00000d00: 0000 7221 0000 0072 2200 0000 7238 0000  ..r!...r"...r8..
-00000d10: 004c 0000 0073 0a00 0000 0001 0c01 0801  .L...s..........
-00000d20: 0a01 0c01 7a1a 5647 4745 6e63 6f64 6572  ....z.VGGEncoder
-00000d30: 2e6c 6f61 645f 7374 6174 655f 6469 6374  .load_state_dict
-00000d40: 2902 4672 1100 0000 2909 da08 5f5f 6e61  ).Fr....)...__na
-00000d50: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000d60: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7215  ..__qualname__r.
-00000d70: 0000 0072 2600 0000 722f 0000 0072 3300  ...r&...r/...r3.
-00000d80: 0000 7238 0000 00da 0d5f 5f63 6c61 7373  ..r8.....__class
-00000d90: 6365 6c6c 5f5f 7221 0000 0072 2100 0000  cell__r!...r!...
-00000da0: 721f 0000 0072 2200 0000 7210 0000 002b  r....r"...r....+
-00000db0: 0000 0073 0a00 0000 0801 0e07 0804 080b  ...s............
-00000dc0: 080a 7210 0000 00da 0576 6767 3131 2906  ..r......vgg11).
-00000dd0: 7207 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
-00000de0: 0b00 0000 720b 0000 0072 0b00 0000 720c  ....r....r....r.
-00000df0: 0000 0046 2903 721b 0000 0072 1c00 0000  ...F).r....r....
-00000e00: 7212 0000 0029 03da 0765 6e63 6f64 6572  r....)...encoder
-00000e10: 7204 0000 00da 0670 6172 616d 73da 0876  r......params..v
-00000e20: 6767 3131 5f62 6e54 da05 7667 6731 3372  gg11_bnT..vgg13r
-00000e30: 0d00 0000 da08 7667 6731 335f 626e da05  ......vgg13_bn..
-00000e40: 7667 6731 3672 0e00 0000 da08 7667 6731  vgg16r......vgg1
-00000e50: 365f 626e da05 7667 6731 3972 0f00 0000  6_bn..vgg19r....
-00000e60: da08 7667 6731 395f 626e 2908 723f 0000  ..vgg19_bn).r?..
-00000e70: 0072 4200 0000 7243 0000 0072 4400 0000  .rB...rC...rD...
-00000e80: 7245 0000 0072 4600 0000 7247 0000 0072  rE...rF...rG...r
-00000e90: 4800 0000 290d da07 5f5f 646f 635f 5fda  H...)...__doc__.
-00000ea0: 0874 6f72 6368 2e6e 6e72 2900 0000 5a16  .torch.nnr)...Z.
-00000eb0: 746f 7263 6876 6973 696f 6e2e 6d6f 6465  torchvision.mode
-00000ec0: 6c73 2e76 6767 7202 0000 0072 0300 0000  ls.vggr....r....
-00000ed0: 5a2a 7072 6574 7261 696e 6564 6d6f 6465  Z*pretrainedmode
-00000ee0: 6c73 2e6d 6f64 656c 732e 746f 7263 6876  ls.models.torchv
-00000ef0: 6973 696f 6e5f 6d6f 6465 6c73 7204 0000  ision_modelsr...
-00000f00: 00da 055f 6261 7365 7206 0000 00da 0363  ..._baser......c
-00000f10: 6667 7210 0000 00da 0c76 6767 5f65 6e63  fgr......vgg_enc
-00000f20: 6f64 6572 7372 2100 0000 7221 0000 0072  odersr!...r!...r
-00000f30: 2100 0000 7222 0000 00da 083c 6d6f 6475  !...r".....<modu
-00000f40: 6c65 3e01 0000 0073 8800 0000 0419 0c01  le>....s........
-00000f50: 0c01 0c01 0c02 0c04 1c01 2001 2601 2cfc  .......... .&.,.
-00000f60: 0609 122b 0201 0602 0201 0601 02fd 04fd  ...+............
-00000f70: 040a 0201 0602 0201 0601 02fd 04fd 040a  ................
-00000f80: 0201 0602 0201 0601 02fd 04fd 040a 0201  ................
-00000f90: 0602 0201 0601 02fd 04fd 040a 0201 0602  ................
-00000fa0: 0201 0601 02fd 04fd 040a 0201 0602 0201  ................
-00000fb0: 0601 02fd 04fd 040a 0201 0602 0201 0601  ................
-00000fc0: 02fd 04fd 040a 0201 0602 0201 0601 02fd  ................
-00000fd0: 04fd 04c0                                ....
+000008f0: 6f61 6473 5c48 616e 616e 5c6d 675c 7365  oads\Hanan\mg\se
+00000900: 676d 656e 7461 7469 6f6e 5f6d 6f64 656c  gmentation_model
+00000910: 735c 656e 636f 6465 7273 5c76 6767 2e70  s\encoders\vgg.p
+00000920: 7972 1500 0000 2c00 0000 730a 0000 0000  yr....,...s.....
+00000930: 0118 0106 0106 0106 017a 1356 4747 456e  .........z.VGGEn
+00000940: 636f 6465 722e 5f5f 696e 6974 5f5f 6303  coder.__init__c.
+00000950: 0000 0000 0000 0000 0000 0003 0000 0002  ................
+00000960: 0000 0043 0000 0073 0c00 0000 7400 6401  ...C...s....t.d.
+00000970: 8301 8201 6400 5300 2902 4e7a 5827 5647  ....d.S.).NzX'VG
+00000980: 4727 206d 6f64 656c 7320 646f 206e 6f74  G' models do not
+00000990: 2073 7570 706f 7274 2064 696c 6174 6564   support dilated
+000009a0: 206d 6f64 6520 6475 6520 746f 204d 6178   mode due to Max
+000009b0: 2050 6f6f 6c69 6e67 206f 7065 7261 7469   Pooling operati
+000009c0: 6f6e 7320 666f 7220 646f 776e 7361 6d70  ons for downsamp
+000009d0: 6c69 6e67 2129 01da 0a56 616c 7565 4572  ling!)...ValueEr
+000009e0: 726f 7229 0372 1a00 0000 da0a 7374 6167  ror).r......stag
+000009f0: 655f 6c69 7374 da0d 6469 6c61 7469 6f6e  e_list..dilation
+00000a00: 5f6c 6973 7472 2100 0000 7221 0000 0072  _listr!...r!...r
+00000a10: 2200 0000 da0c 6d61 6b65 5f64 696c 6174  ".....make_dilat
+00000a20: 6564 3300 0000 7302 0000 0000 017a 1756  ed3...s......z.V
+00000a30: 4747 456e 636f 6465 722e 6d61 6b65 5f64  GGEncoder.make_d
+00000a40: 696c 6174 6564 6301 0000 0000 0000 0000  ilatedc.........
+00000a50: 0000 0004 0000 0005 0000 0043 0000 0073  ...........C...s
+00000a60: 5200 0000 6700 7d01 6700 7d02 7c00 6a00  R...g.}.g.}.|.j.
+00000a70: 4400 5d2e 7d03 7401 7c03 7402 6a03 8302  D.].}.t.|.t.j...
+00000a80: 7232 7c01 a004 7402 6a05 7c02 8e00 a101  r2|...t.j.|.....
+00000a90: 0100 6700 7d02 7c02 a004 7c03 a101 0100  ..g.}.|...|.....
+00000aa0: 710e 7c01 a004 7402 6a05 7c02 8e00 a101  q.|...t.j.|.....
+00000ab0: 0100 7c01 5300 2901 4e29 06da 0866 6561  ..|.S.).N)...fea
+00000ac0: 7475 7265 73da 0a69 7369 6e73 7461 6e63  tures..isinstanc
+00000ad0: 65da 026e 6eda 094d 6178 506f 6f6c 3264  e..nn..MaxPool2d
+00000ae0: da06 6170 7065 6e64 da0a 5365 7175 656e  ..append..Sequen
+00000af0: 7469 616c 2904 721a 0000 00da 0673 7461  tial).r......sta
+00000b00: 6765 735a 0d73 7461 6765 5f6d 6f64 756c  gesZ.stage_modul
+00000b10: 6573 da06 6d6f 6475 6c65 7221 0000 0072  es..moduler!...r
+00000b20: 2100 0000 7222 0000 00da 0a67 6574 5f73  !...r".....get_s
+00000b30: 7461 6765 7337 0000 0073 1200 0000 0001  tages7...s......
+00000b40: 0401 0401 0a01 0c01 1001 0401 0c01 1001  ................
+00000b50: 7a15 5647 4745 6e63 6f64 6572 2e67 6574  z.VGGEncoder.get
+00000b60: 5f73 7461 6765 7363 0200 0000 0000 0000  _stagesc........
+00000b70: 0000 0000 0500 0000 0400 0000 4300 0000  ............C...
+00000b80: 733a 0000 007c 00a0 00a1 007d 0267 007d  s:...|.....}.g.}
+00000b90: 0374 017c 006a 0264 0117 0083 0144 005d  .t.|.j.d.....D.]
+00000ba0: 1a7d 047c 027c 0419 007c 0183 017d 017c  .}.|.|...|...}.|
+00000bb0: 03a0 037c 01a1 0101 0071 1a7c 0353 0029  ...|.....q.|.S.)
+00000bc0: 024e 7205 0000 0029 0472 2f00 0000 da05  .Nr....).r/.....
+00000bd0: 7261 6e67 6572 1700 0000 722b 0000 0029  ranger....r+...)
+00000be0: 0572 1a00 0000 da01 7872 2d00 0000 7227  .r......xr-...r'
+00000bf0: 0000 00da 0169 7221 0000 0072 2100 0000  .....ir!...r!...
+00000c00: 7222 0000 00da 0766 6f72 7761 7264 4200  r".....forwardB.
+00000c10: 0000 730c 0000 0000 0108 0204 0112 010c  ..s.............
+00000c20: 010c 027a 1256 4747 456e 636f 6465 722e  ...z.VGGEncoder.
+00000c30: 666f 7277 6172 6463 0200 0000 0000 0000  forwardc........
+00000c40: 0000 0000 0500 0000 0400 0000 0b00 0000  ................
+00000c50: 733e 0000 0074 007c 01a0 01a1 0083 017d  s>...t.|.......}
+00000c60: 037c 0344 005d 187d 047c 04a0 0264 01a1  .|.D.].}.|...d..
+00000c70: 0172 107c 01a0 037c 04a1 0101 0071 1074  .r.|...|.....q.t
+00000c80: 0483 006a 057c 0166 017c 028e 0101 0064  ...j.|.f.|.....d
+00000c90: 0053 0029 024e 7219 0000 0029 06da 046c  .S.).Nr....)...l
+00000ca0: 6973 74da 046b 6579 73da 0a73 7461 7274  ist..keys..start
+00000cb0: 7377 6974 68da 0370 6f70 7214 0000 00da  swith..popr.....
+00000cc0: 0f6c 6f61 645f 7374 6174 655f 6469 6374  .load_state_dict
+00000cd0: 2905 721a 0000 00da 0a73 7461 7465 5f64  ).r......state_d
+00000ce0: 6963 7472 1e00 0000 7235 0000 00da 016b  ictr....r5.....k
+00000cf0: 721f 0000 0072 2100 0000 7222 0000 0072  r....r!...r"...r
+00000d00: 3800 0000 4c00 0000 730a 0000 0000 010c  8...L...s.......
+00000d10: 0108 010a 010c 017a 1a56 4747 456e 636f  .......z.VGGEnco
+00000d20: 6465 722e 6c6f 6164 5f73 7461 7465 5f64  der.load_state_d
+00000d30: 6963 7429 0246 7211 0000 0029 09da 085f  ict).Fr....)..._
+00000d40: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00000d50: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00000d60: 5f72 1500 0000 7226 0000 0072 2f00 0000  _r....r&...r/...
+00000d70: 7233 0000 0072 3800 0000 da0d 5f5f 636c  r3...r8.....__cl
+00000d80: 6173 7363 656c 6c5f 5f72 2100 0000 7221  asscell__r!...r!
+00000d90: 0000 0072 1f00 0000 7222 0000 0072 1000  ...r....r"...r..
+00000da0: 0000 2b00 0000 730a 0000 0008 010e 0708  ..+...s.........
+00000db0: 0408 0b08 0a72 1000 0000 da05 7667 6731  .....r......vgg1
+00000dc0: 3129 0672 0700 0000 7209 0000 0072 0a00  1).r....r....r..
+00000dd0: 0000 720b 0000 0072 0b00 0000 720b 0000  ..r....r....r...
+00000de0: 0072 0c00 0000 4629 0372 1b00 0000 721c  .r....F).r....r.
+00000df0: 0000 0072 1200 0000 2903 da07 656e 636f  ...r....)...enco
+00000e00: 6465 7272 0400 0000 da06 7061 7261 6d73  derr......params
+00000e10: da08 7667 6731 315f 626e 54da 0576 6767  ..vgg11_bnT..vgg
+00000e20: 3133 720d 0000 00da 0876 6767 3133 5f62  13r......vgg13_b
+00000e30: 6eda 0576 6767 3136 720e 0000 00da 0876  n..vgg16r......v
+00000e40: 6767 3136 5f62 6eda 0576 6767 3139 720f  gg16_bn..vgg19r.
+00000e50: 0000 00da 0876 6767 3139 5f62 6e29 0872  .....vgg19_bn).r
+00000e60: 3f00 0000 7242 0000 0072 4300 0000 7244  ?...rB...rC...rD
+00000e70: 0000 0072 4500 0000 7246 0000 0072 4700  ...rE...rF...rG.
+00000e80: 0000 7248 0000 0029 0dda 075f 5f64 6f63  ..rH...)...__doc
+00000e90: 5f5f da08 746f 7263 682e 6e6e 7229 0000  __..torch.nnr)..
+00000ea0: 005a 1674 6f72 6368 7669 7369 6f6e 2e6d  .Z.torchvision.m
+00000eb0: 6f64 656c 732e 7667 6772 0200 0000 7203  odels.vggr....r.
+00000ec0: 0000 005a 2a70 7265 7472 6169 6e65 646d  ...Z*pretrainedm
+00000ed0: 6f64 656c 732e 6d6f 6465 6c73 2e74 6f72  odels.models.tor
+00000ee0: 6368 7669 7369 6f6e 5f6d 6f64 656c 7372  chvision_modelsr
+00000ef0: 0400 0000 da05 5f62 6173 6572 0600 0000  ......_baser....
+00000f00: da03 6366 6772 1000 0000 da0c 7667 675f  ..cfgr......vgg_
+00000f10: 656e 636f 6465 7273 7221 0000 0072 2100  encodersr!...r!.
+00000f20: 0000 7221 0000 0072 2200 0000 da08 3c6d  ..r!...r".....<m
+00000f30: 6f64 756c 653e 0100 0000 7388 0000 0004  odule>....s.....
+00000f40: 190c 010c 010c 010c 020c 041c 0120 0126  ............. .&
+00000f50: 012c fc06 0912 2b02 0106 0202 0106 0102  .,....+.........
+00000f60: fd04 fd04 0a02 0106 0202 0106 0102 fd04  ................
+00000f70: fd04 0a02 0106 0202 0106 0102 fd04 fd04  ................
+00000f80: 0a02 0106 0202 0106 0102 fd04 fd04 0a02  ................
+00000f90: 0106 0202 0106 0102 fd04 fd04 0a02 0106  ................
+00000fa0: 0202 0106 0102 fd04 fd04 0a02 0106 0202  ................
+00000fb0: 0106 0102 fd04 fd04 0a02 0106 0202 0106  ................
+00000fc0: 0102 fd04 fd04 c0                        .......
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/vgg.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/vgg.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/xception.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/xception.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/xception.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/xception.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/xception.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/xception.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/xception.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/xception.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:20 2023 UTC, .py size: 1979 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -30,109 +30,109 @@
 000001d0: 696e 6974 5f5f da0d 5f6f 7574 5f63 6861  init__.._out_cha
 000001e0: 6e6e 656c 73da 065f 6465 7074 68da 0c5f  nnels.._depth.._
 000001f0: 696e 5f63 6861 6e6e 656c 73da 0563 6f6e  in_channels..con
 00000200: 7631 da07 7061 6464 696e 67da 0563 6f6e  v1..padding..con
 00000210: 7632 da02 6663 2905 da04 7365 6c66 da0c  v2..fc)...self..
 00000220: 6f75 745f 6368 616e 6e65 6c73 7208 0000  out_channelsr...
 00000230: 00da 0461 7267 73da 066b 7761 7267 73a9  ...args..kwargs.
-00000240: 01da 095f 5f63 6c61 7373 5f5f a900 fa58  ...__class__...X
-00000250: 433a 5c55 7365 7273 5c6d 6861 6e61 6e5c  C:\Users\mhanan\
+00000240: 01da 095f 5f63 6c61 7373 5f5f a900 fa4b  ...__class__...K
+00000250: 633a 5c55 7365 7273 5c6d 6861 6e61 6e5c  c:\Users\mhanan\
 00000260: 446f 776e 6c6f 6164 735c 4861 6e61 6e5c  Downloads\Hanan\
-00000270: 4d61 6d6d 6f50 795c 6d61 6d6d 6f70 795c  MammoPy\mammopy\
-00000280: 7365 676d 656e 7461 7469 6f6e 5f6d 6f64  segmentation_mod
-00000290: 656c 735c 656e 636f 6465 7273 5c78 6365  els\encoders\xce
-000002a0: 7074 696f 6e2e 7079 720b 0000 000c 0000  ption.pyr.......
-000002b0: 0073 0e00 0000 0001 0e02 0601 0601 0603  .s..............
-000002c0: 0801 0802 7a18 5863 6570 7469 6f6e 456e  ....z.XceptionEn
-000002d0: 636f 6465 722e 5f5f 696e 6974 5f5f 6303  coder.__init__c.
-000002e0: 0000 0000 0000 0000 0000 0003 0000 0002  ................
-000002f0: 0000 0043 0000 0073 0c00 0000 7400 6401  ...C...s....t.d.
-00000300: 8301 8201 6400 5300 2902 4e7a 5958 6365  ....d.S.).NzYXce
-00000310: 7074 696f 6e20 656e 636f 6465 7220 646f  ption encoder do
-00000320: 6573 206e 6f74 2073 7570 706f 7274 2064  es not support d
-00000330: 696c 6174 6564 206d 6f64 6520 6475 6520  ilated mode due 
-00000340: 746f 2070 6f6f 6c69 6e67 206f 7065 7261  to pooling opera
-00000350: 7469 6f6e 2066 6f72 2064 6f77 6e73 616d  tion for downsam
-00000360: 706c 696e 6721 2901 da0a 5661 6c75 6545  pling!)...ValueE
-00000370: 7272 6f72 2903 7213 0000 00da 0a73 7461  rror).r......sta
-00000380: 6765 5f6c 6973 74da 0d64 696c 6174 696f  ge_list..dilatio
-00000390: 6e5f 6c69 7374 7219 0000 0072 1900 0000  n_listr....r....
-000003a0: 721a 0000 00da 0c6d 616b 655f 6469 6c61  r......make_dila
-000003b0: 7465 6419 0000 0073 0200 0000 0001 7a1c  ted....s......z.
-000003c0: 5863 6570 7469 6f6e 456e 636f 6465 722e  XceptionEncoder.
-000003d0: 6d61 6b65 5f64 696c 6174 6564 6301 0000  make_dilatedc...
-000003e0: 0000 0000 0000 0000 0001 0000 000f 0000  ................
-000003f0: 0043 0000 0073 7800 0000 7400 a001 a100  .C...sx...t.....
-00000400: 7400 a002 7c00 6a03 7c00 6a04 7c00 6a05  t...|.j.|.j.|.j.
-00000410: 7c00 6a06 7c00 6a07 7c00 6a05 a106 7c00  |.j.|.j.|.j...|.
-00000420: 6a08 7c00 6a09 7400 a002 7c00 6a0a 7c00  j.|.j.t...|.j.|.
-00000430: 6a0b 7c00 6a0c 7c00 6a0d 7c00 6a0e 7c00  j.|.j.|.j.|.j.|.
-00000440: 6a0f 7c00 6a10 7c00 6a11 7c00 6a12 a109  j.|.j.|.j.|.j...
-00000450: 7400 a002 7c00 6a13 7c00 6a14 7c00 6a15  t...|.j.|.j.|.j.
-00000460: 7c00 6a05 7c00 6a16 7c00 6a17 a106 6706  |.j.|.j.|.j...g.
-00000470: 5300 2901 4e29 18da 026e 6eda 0849 6465  S.).N)...nn..Ide
-00000480: 6e74 6974 79da 0a53 6571 7565 6e74 6961  ntity..Sequentia
-00000490: 6c72 0f00 0000 da03 626e 31da 0472 656c  lr......bn1..rel
-000004a0: 7572 1100 0000 da03 626e 32da 0662 6c6f  ur......bn2..blo
-000004b0: 636b 31da 0662 6c6f 636b 32da 0662 6c6f  ck1..block2..blo
-000004c0: 636b 33da 0662 6c6f 636b 34da 0662 6c6f  ck3..block4..blo
-000004d0: 636b 35da 0662 6c6f 636b 36da 0662 6c6f  ck5..block6..blo
-000004e0: 636b 37da 0662 6c6f 636b 38da 0662 6c6f  ck7..block8..blo
-000004f0: 636b 39da 0762 6c6f 636b 3130 da07 626c  ck9..block10..bl
-00000500: 6f63 6b31 31da 0762 6c6f 636b 3132 da05  ock11..block12..
-00000510: 636f 6e76 33da 0362 6e33 da05 636f 6e76  conv3..bn3..conv
-00000520: 34da 0362 6e34 2901 7213 0000 0072 1900  4..bn4).r....r..
-00000530: 0000 7219 0000 0072 1a00 0000 da0a 6765  ..r....r......ge
-00000540: 745f 7374 6167 6573 1d00 0000 7318 0000  t_stages....s...
-00000550: 0000 0206 011e 0104 0104 0118 0104 0004  ................
-00000560: 0004 0004 ff02 021e f97a 1a58 6365 7074  .........z.Xcept
-00000570: 696f 6e45 6e63 6f64 6572 2e67 6574 5f73  ionEncoder.get_s
-00000580: 7461 6765 7363 0200 0000 0000 0000 0000  tagesc..........
-00000590: 0000 0500 0000 0400 0000 4300 0000 733a  ..........C...s:
-000005a0: 0000 007c 00a0 00a1 007d 0267 007d 0374  ...|.....}.g.}.t
-000005b0: 017c 006a 0264 0117 0083 0144 005d 1a7d  .|.j.d.....D.].}
-000005c0: 047c 027c 0419 007c 0183 017d 017c 03a0  .|.|...|...}.|..
-000005d0: 037c 01a1 0101 0071 1a7c 0353 0029 024e  .|.....q.|.S.).N
-000005e0: 7204 0000 0029 0472 3500 0000 da05 7261  r....).r5.....ra
-000005f0: 6e67 6572 0d00 0000 da06 6170 7065 6e64  nger......append
-00000600: 2905 7213 0000 00da 0178 da06 7374 6167  ).r......x..stag
-00000610: 6573 da08 6665 6174 7572 6573 da01 6972  es..features..ir
-00000620: 1900 0000 7219 0000 0072 1a00 0000 da07  ....r....r......
-00000630: 666f 7277 6172 6428 0000 0073 0c00 0000  forward(...s....
-00000640: 0001 0802 0401 1201 0c01 0c02 7a17 5863  ............z.Xc
-00000650: 6570 7469 6f6e 456e 636f 6465 722e 666f  eptionEncoder.fo
-00000660: 7277 6172 6463 0200 0000 0000 0000 0000  rwardc..........
-00000670: 0000 0200 0000 0300 0000 0300 0000 7324  ..............s$
-00000680: 0000 007c 01a0 0064 01a1 0101 007c 01a0  ...|...d.....|..
-00000690: 0064 02a1 0101 0074 0183 00a0 027c 01a1  .d.....t.....|..
-000006a0: 0101 0064 0053 0029 034e 7a07 6663 2e62  ...d.S.).Nz.fc.b
-000006b0: 6961 737a 0966 632e 7765 6967 6874 2903  iasz.fc.weight).
-000006c0: da03 706f 7072 0a00 0000 da0f 6c6f 6164  ..popr......load
-000006d0: 5f73 7461 7465 5f64 6963 7429 0272 1300  _state_dict).r..
-000006e0: 0000 da0a 7374 6174 655f 6469 6374 7217  ....state_dictr.
-000006f0: 0000 0072 1900 0000 721a 0000 0072 3e00  ...r....r....r>.
-00000700: 0000 3200 0000 7306 0000 0000 020a 010a  ..2...s.........
-00000710: 027a 1f58 6365 7074 696f 6e45 6e63 6f64  .z.XceptionEncod
-00000720: 6572 2e6c 6f61 645f 7374 6174 655f 6469  er.load_state_di
-00000730: 6374 2909 da08 5f5f 6e61 6d65 5f5f da0a  ct)...__name__..
-00000740: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00000750: 616c 6e61 6d65 5f5f 720b 0000 0072 1e00  alname__r....r..
-00000760: 0000 7235 0000 0072 3c00 0000 723e 0000  ..r5...r<...r>..
-00000770: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
-00000780: 7219 0000 0072 1900 0000 7217 0000 0072  r....r....r....r
-00000790: 1a00 0000 7206 0000 000a 0000 0073 0a00  ....r........s..
-000007a0: 0000 0802 120d 0804 080b 080a 7206 0000  ............r...
-000007b0: 00da 0878 6365 7074 696f 6e72 1400 0000  ...xceptionr....
-000007c0: 2906 7209 0000 00e9 4000 0000 e980 0000  ).r.....@.......
-000007d0: 00e9 0001 0000 69d8 0200 0069 0008 0000  ......i....i....
-000007e0: 2903 da07 656e 636f 6465 7272 0200 0000  )...encoderr....
-000007f0: da06 7061 7261 6d73 290a da02 7265 da08  ..params)...re..
-00000800: 746f 7263 682e 6e6e 721f 0000 005a 2070  torch.nnr....Z p
-00000810: 7265 7472 6169 6e65 646d 6f64 656c 732e  retrainedmodels.
-00000820: 6d6f 6465 6c73 2e78 6365 7074 696f 6e72  models.xceptionr
-00000830: 0200 0000 7203 0000 00da 055f 6261 7365  ....r......_base
-00000840: 7205 0000 0072 0600 0000 da11 7863 6570  r....r......xcep
-00000850: 7469 6f6e 5f65 6e63 6f64 6572 7372 1900  tion_encodersr..
-00000860: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00000870: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00000880: 1a00 0000 0801 0c02 0c01 0c02 0c03 1231  ...............1
-00000890: 0201 0201 0602 0200 02ff 02fd 04ff       ..............
+00000270: 6d67 5c73 6567 6d65 6e74 6174 696f 6e5f  mg\segmentation_
+00000280: 6d6f 6465 6c73 5c65 6e63 6f64 6572 735c  models\encoders\
+00000290: 7863 6570 7469 6f6e 2e70 7972 0b00 0000  xception.pyr....
+000002a0: 0c00 0000 730e 0000 0000 010e 0206 0106  ....s...........
+000002b0: 0106 0308 0108 027a 1858 6365 7074 696f  .......z.Xceptio
+000002c0: 6e45 6e63 6f64 6572 2e5f 5f69 6e69 745f  nEncoder.__init_
+000002d0: 5f63 0300 0000 0000 0000 0000 0000 0300  _c..............
+000002e0: 0000 0200 0000 4300 0000 730c 0000 0074  ......C...s....t
+000002f0: 0064 0183 0182 0164 0053 0029 024e 7a59  .d.....d.S.).NzY
+00000300: 5863 6570 7469 6f6e 2065 6e63 6f64 6572  Xception encoder
+00000310: 2064 6f65 7320 6e6f 7420 7375 7070 6f72   does not suppor
+00000320: 7420 6469 6c61 7465 6420 6d6f 6465 2064  t dilated mode d
+00000330: 7565 2074 6f20 706f 6f6c 696e 6720 6f70  ue to pooling op
+00000340: 6572 6174 696f 6e20 666f 7220 646f 776e  eration for down
+00000350: 7361 6d70 6c69 6e67 2129 01da 0a56 616c  sampling!)...Val
+00000360: 7565 4572 726f 7229 0372 1300 0000 da0a  ueError).r......
+00000370: 7374 6167 655f 6c69 7374 da0d 6469 6c61  stage_list..dila
+00000380: 7469 6f6e 5f6c 6973 7472 1900 0000 7219  tion_listr....r.
+00000390: 0000 0072 1a00 0000 da0c 6d61 6b65 5f64  ...r......make_d
+000003a0: 696c 6174 6564 1900 0000 7302 0000 0000  ilated....s.....
+000003b0: 017a 1c58 6365 7074 696f 6e45 6e63 6f64  .z.XceptionEncod
+000003c0: 6572 2e6d 616b 655f 6469 6c61 7465 6463  er.make_dilatedc
+000003d0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000003e0: 0f00 0000 4300 0000 7378 0000 0074 00a0  ....C...sx...t..
+000003f0: 01a1 0074 00a0 027c 006a 037c 006a 047c  ...t...|.j.|.j.|
+00000400: 006a 057c 006a 067c 006a 077c 006a 05a1  .j.|.j.|.j.|.j..
+00000410: 067c 006a 087c 006a 0974 00a0 027c 006a  .|.j.|.j.t...|.j
+00000420: 0a7c 006a 0b7c 006a 0c7c 006a 0d7c 006a  .|.j.|.j.|.j.|.j
+00000430: 0e7c 006a 0f7c 006a 107c 006a 117c 006a  .|.j.|.j.|.j.|.j
+00000440: 12a1 0974 00a0 027c 006a 137c 006a 147c  ...t...|.j.|.j.|
+00000450: 006a 157c 006a 057c 006a 167c 006a 17a1  .j.|.j.|.j.|.j..
+00000460: 0667 0653 0029 014e 2918 da02 6e6e da08  .g.S.).N)...nn..
+00000470: 4964 656e 7469 7479 da0a 5365 7175 656e  Identity..Sequen
+00000480: 7469 616c 720f 0000 00da 0362 6e31 da04  tialr......bn1..
+00000490: 7265 6c75 7211 0000 00da 0362 6e32 da06  relur......bn2..
+000004a0: 626c 6f63 6b31 da06 626c 6f63 6b32 da06  block1..block2..
+000004b0: 626c 6f63 6b33 da06 626c 6f63 6b34 da06  block3..block4..
+000004c0: 626c 6f63 6b35 da06 626c 6f63 6b36 da06  block5..block6..
+000004d0: 626c 6f63 6b37 da06 626c 6f63 6b38 da06  block7..block8..
+000004e0: 626c 6f63 6b39 da07 626c 6f63 6b31 30da  block9..block10.
+000004f0: 0762 6c6f 636b 3131 da07 626c 6f63 6b31  .block11..block1
+00000500: 32da 0563 6f6e 7633 da03 626e 33da 0563  2..conv3..bn3..c
+00000510: 6f6e 7634 da03 626e 3429 0172 1300 0000  onv4..bn4).r....
+00000520: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
+00000530: 0a67 6574 5f73 7461 6765 731d 0000 0073  .get_stages....s
+00000540: 1800 0000 0002 0601 1e01 0401 0401 1801  ................
+00000550: 0400 0400 0400 04ff 0202 1ef9 7a1a 5863  ............z.Xc
+00000560: 6570 7469 6f6e 456e 636f 6465 722e 6765  eptionEncoder.ge
+00000570: 745f 7374 6167 6573 6302 0000 0000 0000  t_stagesc.......
+00000580: 0000 0000 0005 0000 0004 0000 0043 0000  .............C..
+00000590: 0073 3a00 0000 7c00 a000 a100 7d02 6700  .s:...|.....}.g.
+000005a0: 7d03 7401 7c00 6a02 6401 1700 8301 4400  }.t.|.j.d.....D.
+000005b0: 5d1a 7d04 7c02 7c04 1900 7c01 8301 7d01  ].}.|.|...|...}.
+000005c0: 7c03 a003 7c01 a101 0100 711a 7c03 5300  |...|.....q.|.S.
+000005d0: 2902 4e72 0400 0000 2904 7235 0000 00da  ).Nr....).r5....
+000005e0: 0572 616e 6765 720d 0000 00da 0661 7070  .ranger......app
+000005f0: 656e 6429 0572 1300 0000 da01 78da 0673  end).r......x..s
+00000600: 7461 6765 73da 0866 6561 7475 7265 73da  tages..features.
+00000610: 0169 7219 0000 0072 1900 0000 721a 0000  .ir....r....r...
+00000620: 00da 0766 6f72 7761 7264 2800 0000 730c  ...forward(...s.
+00000630: 0000 0000 0108 0204 0112 010c 010c 027a  ...............z
+00000640: 1758 6365 7074 696f 6e45 6e63 6f64 6572  .XceptionEncoder
+00000650: 2e66 6f72 7761 7264 6302 0000 0000 0000  .forwardc.......
+00000660: 0000 0000 0002 0000 0003 0000 0003 0000  ................
+00000670: 0073 2400 0000 7c01 a000 6401 a101 0100  .s$...|...d.....
+00000680: 7c01 a000 6402 a101 0100 7401 8300 a002  |...d.....t.....
+00000690: 7c01 a101 0100 6400 5300 2903 4e7a 0766  |.....d.S.).Nz.f
+000006a0: 632e 6269 6173 7a09 6663 2e77 6569 6768  c.biasz.fc.weigh
+000006b0: 7429 03da 0370 6f70 720a 0000 00da 0f6c  t)...popr......l
+000006c0: 6f61 645f 7374 6174 655f 6469 6374 2902  oad_state_dict).
+000006d0: 7213 0000 00da 0a73 7461 7465 5f64 6963  r......state_dic
+000006e0: 7472 1700 0000 7219 0000 0072 1a00 0000  tr....r....r....
+000006f0: 723e 0000 0032 0000 0073 0600 0000 0002  r>...2...s......
+00000700: 0a01 0a02 7a1f 5863 6570 7469 6f6e 456e  ....z.XceptionEn
+00000710: 636f 6465 722e 6c6f 6164 5f73 7461 7465  coder.load_state
+00000720: 5f64 6963 7429 09da 085f 5f6e 616d 655f  _dict)...__name_
+00000730: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000740: 5f71 7561 6c6e 616d 655f 5f72 0b00 0000  _qualname__r....
+00000750: 721e 0000 0072 3500 0000 723c 0000 0072  r....r5...r<...r
+00000760: 3e00 0000 da0d 5f5f 636c 6173 7363 656c  >.....__classcel
+00000770: 6c5f 5f72 1900 0000 7219 0000 0072 1700  l__r....r....r..
+00000780: 0000 721a 0000 0072 0600 0000 0a00 0000  ..r....r........
+00000790: 730a 0000 0008 0212 0d08 0408 0b08 0a72  s..............r
+000007a0: 0600 0000 da08 7863 6570 7469 6f6e 7214  ......xceptionr.
+000007b0: 0000 0029 0672 0900 0000 e940 0000 00e9  ...).r.....@....
+000007c0: 8000 0000 e900 0100 0069 d802 0000 6900  .........i....i.
+000007d0: 0800 0029 03da 0765 6e63 6f64 6572 7202  ...)...encoderr.
+000007e0: 0000 00da 0670 6172 616d 7329 0ada 0272  .....params)...r
+000007f0: 65da 0874 6f72 6368 2e6e 6e72 1f00 0000  e..torch.nnr....
+00000800: 5a20 7072 6574 7261 696e 6564 6d6f 6465  Z pretrainedmode
+00000810: 6c73 2e6d 6f64 656c 732e 7863 6570 7469  ls.models.xcepti
+00000820: 6f6e 7202 0000 0072 0300 0000 da05 5f62  onr....r......_b
+00000830: 6173 6572 0500 0000 7206 0000 00da 1178  aser....r......x
+00000840: 6365 7074 696f 6e5f 656e 636f 6465 7273  ception_encoders
+00000850: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
+00000860: 1a00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000870: 0000 731a 0000 0008 010c 020c 010c 020c  ..s.............
+00000880: 0312 3102 0102 0106 0202 0002 ff02 fd04  ..1.............
+00000890: ff                                       .
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/__pycache__/xception.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/encoders/__pycache__/xception.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/_base.py` & `mammopy-0.0.9/segmentation_models/encoders/_base.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/_utils.py` & `mammopy-0.0.9/segmentation_models/encoders/_utils.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/densenet.py` & `mammopy-0.0.9/segmentation_models/encoders/densenet.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/dpn.py` & `mammopy-0.0.9/segmentation_models/encoders/dpn.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/efficientnet.py` & `mammopy-0.0.9/segmentation_models/encoders/efficientnet.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/inceptionresnetv2.py` & `mammopy-0.0.9/segmentation_models/encoders/inceptionresnetv2.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/inceptionv4.py` & `mammopy-0.0.9/segmentation_models/encoders/inceptionv4.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/mobilenet.py` & `mammopy-0.0.9/segmentation_models/encoders/mobilenet.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/resnet.py` & `mammopy-0.0.9/segmentation_models/encoders/resnet.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/senet.py` & `mammopy-0.0.9/segmentation_models/encoders/senet.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/timm_efficientnet.py` & `mammopy-0.0.9/segmentation_models/encoders/timm_efficientnet.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/vgg.py` & `mammopy-0.0.9/segmentation_models/encoders/vgg.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/encoders/xception.py` & `mammopy-0.0.9/segmentation_models/encoders/xception.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/decoder.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/unet/__pycache__/decoder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/decoder.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/unet/__pycache__/decoder.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/decoder.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/unet/__pycache__/decoder.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/decoder.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/unet/__pycache__/decoder.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:22 2023 UTC, .py size: 3862 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -33,160 +33,160 @@
 00000200: 6f6e da0a 6174 7465 6e74 696f 6e31 da05  on..attention1..
 00000210: 636f 6e76 32da 0a61 7474 656e 7469 6f6e  conv2..attention
 00000220: 3229 06da 0473 656c 6672 0b00 0000 da0d  2)...selfr......
 00000230: 736b 6970 5f63 6861 6e6e 656c 73da 0c6f  skip_channels..o
 00000240: 7574 5f63 6861 6e6e 656c 7372 0a00 0000  ut_channelsr....
 00000250: da0e 6174 7465 6e74 696f 6e5f 7479 7065  ..attention_type
 00000260: a901 da09 5f5f 636c 6173 735f 5fa9 00fa  ....__class__...
-00000270: 5343 3a5c 5573 6572 735c 6d68 616e 616e  SC:\Users\mhanan
+00000270: 4663 3a5c 5573 6572 735c 6d68 616e 616e  Fc:\Users\mhanan
 00000280: 5c44 6f77 6e6c 6f61 6473 5c48 616e 616e  \Downloads\Hanan
-00000290: 5c4d 616d 6d6f 5079 5c6d 616d 6d6f 7079  \MammoPy\mammopy
-000002a0: 5c73 6567 6d65 6e74 6174 696f 6e5f 6d6f  \segmentation_mo
-000002b0: 6465 6c73 5c75 6e65 745c 6465 636f 6465  dels\unet\decode
-000002c0: 722e 7079 720d 0000 0009 0000 0073 2200  r.pyr........s".
-000002d0: 0000 0008 0a01 0401 0601 0201 0201 0201  ................
-000002e0: 02fb 0807 1401 0401 0201 0201 0201 0201  ................
-000002f0: 02fb 0807 7a15 4465 636f 6465 7242 6c6f  ....z.DecoderBlo
-00000300: 636b 2e5f 5f69 6e69 745f 5f63 0300 0000  ck.__init__c....
-00000310: 0000 0000 0000 0000 0300 0000 0500 0000  ................
-00000320: 4300 0000 7356 0000 0074 006a 017c 0164  C...sV...t.j.|.d
-00000330: 0164 0264 038d 037d 017c 0264 006b 0972  .d.d...}.|.d.k.r
-00000340: 3474 026a 037c 017c 0267 0264 0464 058d  4t.j.|.|.g.d.d..
-00000350: 027d 017c 00a0 047c 01a1 017d 017c 00a0  .}.|...|...}.|..
-00000360: 057c 01a1 017d 017c 00a0 067c 01a1 017d  .|...}.|...|...}
-00000370: 017c 00a0 077c 01a1 017d 017c 0153 0029  .|...|...}.|.S.)
-00000380: 064e 7202 0000 00da 076e 6561 7265 7374  .Nr......nearest
-00000390: 2902 da0c 7363 616c 655f 6661 6374 6f72  )...scale_factor
-000003a0: da04 6d6f 6465 7206 0000 0029 01da 0364  ..moder....)...d
-000003b0: 696d 2908 da01 46da 0b69 6e74 6572 706f  im)...F..interpo
-000003c0: 6c61 7465 da05 746f 7263 68da 0363 6174  late..torch..cat
-000003d0: 7211 0000 0072 1000 0000 7212 0000 0072  r....r....r....r
-000003e0: 1300 0000 2903 7214 0000 00da 0178 da04  ....).r......x..
-000003f0: 736b 6970 721a 0000 0072 1a00 0000 721b  skipr....r....r.
-00000400: 0000 00da 0766 6f72 7761 7264 2300 0000  .....forward#...
-00000410: 7310 0000 0000 0110 0108 0112 010a 010a  s...............
-00000420: 010a 010a 017a 1444 6563 6f64 6572 426c  .....z.DecoderBl
-00000430: 6f63 6b2e 666f 7277 6172 6429 0254 4e29  ock.forward).TN)
-00000440: 014e a906 da08 5f5f 6e61 6d65 5f5f da0a  .N....__name__..
-00000450: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00000460: 616c 6e61 6d65 5f5f 720d 0000 0072 2600  alname__r....r&.
-00000470: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
-00000480: 5f72 1a00 0000 721a 0000 0072 1800 0000  _r....r....r....
-00000490: 721b 0000 0072 0400 0000 0800 0000 7308  r....r........s.
-000004a0: 0000 0008 0600 0100 fa0e 1a72 0400 0000  ...........r....
-000004b0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000004c0: 0004 0000 0000 0000 0073 1e00 0000 6500  .........s....e.
-000004d0: 5a01 6400 5a02 6404 8700 6601 6402 6403  Z.d.Z.d...f.d.d.
-000004e0: 8409 5a03 8700 0400 5a04 5300 2905 da0b  ..Z.....Z.S.)...
-000004f0: 4365 6e74 6572 426c 6f63 6b54 6304 0000  CenterBlockTc...
-00000500: 0000 0000 0000 0000 0006 0000 0007 0000  ................
-00000510: 0003 0000 0073 3a00 0000 7400 6a01 7c01  .....s:...t.j.|.
-00000520: 7c02 6401 6402 7c03 6403 8d05 7d04 7400  |.d.d.|.d...}.t.
-00000530: 6a01 7c02 7c02 6401 6402 7c03 6403 8d05  j.|.|.d.d.|.d...
-00000540: 7d05 7402 8300 a003 7c04 7c05 a102 0100  }.t.....|.|.....
-00000550: 6400 5300 2904 4e72 0500 0000 7206 0000  d.S.).Nr....r...
-00000560: 0072 0700 0000 2904 720e 0000 0072 0f00  .r....).r....r..
-00000570: 0000 720c 0000 0072 0d00 0000 2906 7214  ..r....r....).r.
-00000580: 0000 0072 0b00 0000 7216 0000 0072 0a00  ...r....r....r..
-00000590: 0000 7210 0000 0072 1200 0000 7218 0000  ..r....r....r...
-000005a0: 0072 1a00 0000 721b 0000 0072 0d00 0000  .r....r....r....
-000005b0: 2f00 0000 731e 0000 0000 0104 0102 0102  /...s...........
-000005c0: 0102 0102 0102 fb06 0704 0102 0102 0102  ................
-000005d0: 0102 0102 fb06 077a 1443 656e 7465 7242  .......z.CenterB
-000005e0: 6c6f 636b 2e5f 5f69 6e69 745f 5f29 0154  lock.__init__).T
-000005f0: 2905 7228 0000 0072 2900 0000 722a 0000  ).r(...r)...r*..
-00000600: 0072 0d00 0000 722b 0000 0072 1a00 0000  .r....r+...r....
-00000610: 721a 0000 0072 1800 0000 721b 0000 0072  r....r....r....r
-00000620: 2c00 0000 2e00 0000 7302 0000 0008 0172  ,.......s......r
-00000630: 2c00 0000 6300 0000 0000 0000 0000 0000  ,...c...........
-00000640: 0000 0000 0004 0000 0000 0000 0073 2600  .............s&.
-00000650: 0000 6500 5a01 6400 5a02 6409 8700 6601  ..e.Z.d.Z.d...f.
-00000660: 6405 6406 8409 5a03 6407 6408 8400 5a04  d.d...Z.d.d...Z.
-00000670: 8700 0400 5a05 5300 290a da0b 556e 6574  ....Z.S.)...Unet
-00000680: 4465 636f 6465 72e9 0500 0000 544e 4663  Decoder.....TNFc
-00000690: 0700 0000 0000 0000 0000 0000 0c00 0000  ................
-000006a0: 0600 0000 0300 0000 73d2 0000 0074 0083  ........s....t..
-000006b0: 00a0 01a1 0001 007c 0374 027c 0283 016b  .......|.t.|...k
-000006c0: 0372 2a74 0364 01a0 047c 0374 027c 0283  .r*t.d...|.t.|..
-000006d0: 01a1 0283 0182 017c 0164 0264 0085 0219  .......|.d.d....
-000006e0: 007d 017c 0164 0064 0064 0385 0319 007d  .}.|.d.d.d.....}
-000006f0: 017c 0164 0419 007d 077c 0767 0174 057c  .|.d...}.|.g.t.|
-00000700: 0264 0064 0385 0219 0083 0117 007d 0874  .d.d.........}.t
-00000710: 057c 0164 0264 0085 0219 0083 0164 0467  .|.d.d.......d.g
-00000720: 0117 007d 097c 027d 0a7c 0672 9274 067c  ...}.|.}.|.r.t.|
-00000730: 077c 077c 0464 058d 037c 005f 076e 0a74  .|.|.d...|._.n.t
-00000740: 08a0 09a1 007c 005f 0774 0a7c 047c 0564  .....|._.t.|.|.d
-00000750: 068d 0289 0087 0066 0164 0764 0884 0874  .......f.d.d...t
-00000760: 0b7c 087c 097c 0a83 0344 0083 017d 0b74  .|.|.|...D...}.t
-00000770: 08a0 0c7c 0ba1 017c 005f 0d64 0053 0029  ...|...|._.d.S.)
-00000780: 094e 7a44 4d6f 6465 6c20 6465 7074 6820  .NzDModel depth 
-00000790: 6973 207b 7d2c 2062 7574 2079 6f75 2070  is {}, but you p
-000007a0: 726f 7669 6465 2060 6465 636f 6465 725f  rovide `decoder_
-000007b0: 6368 616e 6e65 6c73 6020 666f 7220 7b7d  channels` for {}
-000007c0: 2062 6c6f 636b 732e 7206 0000 00e9 ffff   blocks.r.......
-000007d0: ffff 7201 0000 0029 0172 0a00 0000 2902  ..r....).r....).
-000007e0: 720a 0000 0072 1700 0000 6301 0000 0000  r....r....c.....
-000007f0: 0000 0000 0000 0004 0000 0006 0000 0013  ................
-00000800: 0000 0073 2200 0000 6700 7c00 5d1a 5c03  ...s"...g.|.].\.
-00000810: 7d01 7d02 7d03 7400 7c01 7c02 7c03 6603  }.}.}.t.|.|.|.f.
-00000820: 8800 8e01 9102 7104 5300 721a 0000 0029  ......q.S.r....)
-00000830: 0172 0400 0000 2904 da02 2e30 da05 696e  .r....)....0..in
-00000840: 5f63 685a 0773 6b69 705f 6368 da06 6f75  _chZ.skip_ch..ou
-00000850: 745f 6368 a901 da06 6b77 6172 6773 721a  t_ch....kwargsr.
-00000860: 0000 0072 1b00 0000 da0a 3c6c 6973 7463  ...r......<listc
-00000870: 6f6d 703e 6600 0000 7304 0000 0006 0208  omp>f...s.......
-00000880: ff7a 2855 6e65 7444 6563 6f64 6572 2e5f  .z(UnetDecoder._
-00000890: 5f69 6e69 745f 5f2e 3c6c 6f63 616c 733e  _init__.<locals>
-000008a0: 2e3c 6c69 7374 636f 6d70 3e29 0e72 0c00  .<listcomp>).r..
-000008b0: 0000 720d 0000 00da 036c 656e da0a 5661  ..r......len..Va
-000008c0: 6c75 6545 7272 6f72 da06 666f 726d 6174  lueError..format
-000008d0: da04 6c69 7374 722c 0000 00da 0663 656e  ..listr,.....cen
-000008e0: 7465 72da 026e 6eda 0849 6465 6e74 6974  ter..nn..Identit
-000008f0: 79da 0464 6963 74da 037a 6970 da0a 4d6f  y..dict..zip..Mo
-00000900: 6475 6c65 4c69 7374 da06 626c 6f63 6b73  duleList..blocks
-00000910: 290c 7214 0000 00da 1065 6e63 6f64 6572  ).r......encoder
-00000920: 5f63 6861 6e6e 656c 73da 1064 6563 6f64  _channels..decod
-00000930: 6572 5f63 6861 6e6e 656c 73da 086e 5f62  er_channels..n_b
-00000940: 6c6f 636b 7372 0a00 0000 7217 0000 0072  locksr....r....r
-00000950: 3a00 0000 5a0d 6865 6164 5f63 6861 6e6e  :...Z.head_chann
-00000960: 656c 7372 0b00 0000 7215 0000 0072 1600  elsr....r....r..
-00000970: 0000 7240 0000 0072 1800 0000 7233 0000  ..r@...r....r3..
-00000980: 0072 1b00 0000 720d 0000 0042 0000 0073  .r....r....B...s
-00000990: 3400 0000 0009 0a02 0c01 0201 0401 0200  4...............
-000009a0: 06ff 02ff 0406 0c01 0e03 0801 1601 1601  ................
-000009b0: 0402 0401 0201 0200 0200 02ff 0a04 0a03  ................
-000009c0: 0c01 0a02 0afe 0604 7a14 556e 6574 4465  ........z.UnetDe
-000009d0: 636f 6465 722e 5f5f 696e 6974 5f5f 6301  coder.__init__c.
-000009e0: 0000 0000 0000 0000 0000 0008 0000 0004  ................
-000009f0: 0000 0047 0000 0073 7200 0000 7c01 6401  ...G...sr...|.d.
-00000a00: 6400 8502 1900 7d01 7c01 6400 6400 6402  d.....}.|.d.d.d.
-00000a10: 8503 1900 7d01 7c01 6403 1900 7d02 7c01  ....}.|.d...}.|.
-00000a20: 6401 6400 8502 1900 7d03 7c00 a000 7c02  d.d.....}.|...|.
-00000a30: a101 7d04 7401 7c00 6a02 8301 4400 5d2a  ..}.t.|.j...D.]*
-00000a40: 5c02 7d05 7d06 7c05 7403 7c03 8301 6b00  \.}.}.|.t.|...k.
-00000a50: 725e 7c03 7c05 1900 6e02 6400 7d07 7c06  r^|.|...n.d.}.|.
-00000a60: 7c04 7c07 8302 7d04 7142 7c04 5300 2904  |.|...}.qB|.S.).
-00000a70: 4e72 0600 0000 722f 0000 0072 0100 0000  Nr....r/...r....
-00000a80: 2904 723a 0000 00da 0965 6e75 6d65 7261  ).r:.....enumera
-00000a90: 7465 7240 0000 0072 3600 0000 2908 7214  ter@...r6...).r.
-00000aa0: 0000 00da 0866 6561 7475 7265 73da 0468  .....features..h
-00000ab0: 6561 64da 0573 6b69 7073 7224 0000 00da  ead..skipsr$....
-00000ac0: 0169 5a0d 6465 636f 6465 725f 626c 6f63  .iZ.decoder_bloc
-00000ad0: 6b72 2500 0000 721a 0000 0072 1a00 0000  kr%...r....r....
-00000ae0: 721b 0000 0072 2600 0000 6c00 0000 7312  r....r&...l...s.
-00000af0: 0000 0000 020c 010e 0208 010c 020a 0112  ................
-00000b00: 0118 010c 027a 1355 6e65 7444 6563 6f64  .....z.UnetDecod
-00000b10: 6572 2e66 6f72 7761 7264 2904 722e 0000  er.forward).r...
-00000b20: 0054 4e46 7227 0000 0072 1a00 0000 721a  .TNFr'...r....r.
-00000b30: 0000 0072 1800 0000 721b 0000 0072 2d00  ...r....r....r-.
-00000b40: 0000 4100 0000 730c 0000 0008 0500 0100  ..A...s.........
-00000b50: 0100 0100 f90e 2a72 2d00 0000 290e 7222  ......*r-...).r"
-00000b60: 0000 00da 0874 6f72 6368 2e6e 6e72 3b00  .....torch.nnr;.
-00000b70: 0000 5a13 746f 7263 682e 6e6e 2e66 756e  ..Z.torch.nn.fun
-00000b80: 6374 696f 6e61 6cda 0a66 756e 6374 696f  ctional..functio
-00000b90: 6e61 6c72 2000 0000 da04 6261 7365 7203  nalr .....baser.
-00000ba0: 0000 0072 0e00 0000 da06 4d6f 6475 6c65  ...r......Module
-00000bb0: 7204 0000 00da 0a53 6571 7565 6e74 6961  r......Sequentia
-00000bc0: 6c72 2c00 0000 722d 0000 0072 1a00 0000  lr,...r-...r....
-00000bd0: 721a 0000 0072 1a00 0000 721b 0000 00da  r....r....r.....
-00000be0: 083c 6d6f 6475 6c65 3e01 0000 0073 0c00  .<module>....s..
-00000bf0: 0000 0801 0c01 1202 0c03 1226 1213       ...........&..
+00000290: 5c6d 675c 7365 676d 656e 7461 7469 6f6e  \mg\segmentation
+000002a0: 5f6d 6f64 656c 735c 756e 6574 5c64 6563  _models\unet\dec
+000002b0: 6f64 6572 2e70 7972 0d00 0000 0900 0000  oder.pyr........
+000002c0: 7322 0000 0000 080a 0104 0106 0102 0102  s"..............
+000002d0: 0102 0102 fb08 0714 0104 0102 0102 0102  ................
+000002e0: 0102 0102 fb08 077a 1544 6563 6f64 6572  .......z.Decoder
+000002f0: 426c 6f63 6b2e 5f5f 696e 6974 5f5f 6303  Block.__init__c.
+00000300: 0000 0000 0000 0000 0000 0003 0000 0005  ................
+00000310: 0000 0043 0000 0073 5600 0000 7400 6a01  ...C...sV...t.j.
+00000320: 7c01 6401 6402 6403 8d03 7d01 7c02 6400  |.d.d.d...}.|.d.
+00000330: 6b09 7234 7402 6a03 7c01 7c02 6702 6404  k.r4t.j.|.|.g.d.
+00000340: 6405 8d02 7d01 7c00 a004 7c01 a101 7d01  d...}.|...|...}.
+00000350: 7c00 a005 7c01 a101 7d01 7c00 a006 7c01  |...|...}.|...|.
+00000360: a101 7d01 7c00 a007 7c01 a101 7d01 7c01  ..}.|...|...}.|.
+00000370: 5300 2906 4e72 0200 0000 da07 6e65 6172  S.).Nr......near
+00000380: 6573 7429 02da 0c73 6361 6c65 5f66 6163  est)...scale_fac
+00000390: 746f 72da 046d 6f64 6572 0600 0000 2901  tor..moder....).
+000003a0: da03 6469 6d29 08da 0146 da0b 696e 7465  ..dim)...F..inte
+000003b0: 7270 6f6c 6174 65da 0574 6f72 6368 da03  rpolate..torch..
+000003c0: 6361 7472 1100 0000 7210 0000 0072 1200  catr....r....r..
+000003d0: 0000 7213 0000 0029 0372 1400 0000 da01  ..r....).r......
+000003e0: 78da 0473 6b69 7072 1a00 0000 721a 0000  x..skipr....r...
+000003f0: 0072 1b00 0000 da07 666f 7277 6172 6423  .r......forward#
+00000400: 0000 0073 1000 0000 0001 1001 0801 1201  ...s............
+00000410: 0a01 0a01 0a01 0a01 7a14 4465 636f 6465  ........z.Decode
+00000420: 7242 6c6f 636b 2e66 6f72 7761 7264 2902  rBlock.forward).
+00000430: 544e 2901 4ea9 06da 085f 5f6e 616d 655f  TN).N....__name_
+00000440: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000450: 5f71 7561 6c6e 616d 655f 5f72 0d00 0000  _qualname__r....
+00000460: 7226 0000 00da 0d5f 5f63 6c61 7373 6365  r&.....__classce
+00000470: 6c6c 5f5f 721a 0000 0072 1a00 0000 7218  ll__r....r....r.
+00000480: 0000 0072 1b00 0000 7204 0000 0008 0000  ...r....r.......
+00000490: 0073 0800 0000 0806 0001 00fa 0e1a 7204  .s............r.
+000004a0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000004b0: 0000 0000 0400 0000 0000 0000 731e 0000  ............s...
+000004c0: 0065 005a 0164 005a 0264 0487 0066 0164  .e.Z.d.Z.d...f.d
+000004d0: 0264 0384 095a 0387 0004 005a 0453 0029  .d...Z.....Z.S.)
+000004e0: 05da 0b43 656e 7465 7242 6c6f 636b 5463  ...CenterBlockTc
+000004f0: 0400 0000 0000 0000 0000 0000 0600 0000  ................
+00000500: 0700 0000 0300 0000 733a 0000 0074 006a  ........s:...t.j
+00000510: 017c 017c 0264 0164 027c 0364 038d 057d  .|.|.d.d.|.d...}
+00000520: 0474 006a 017c 027c 0264 0164 027c 0364  .t.j.|.|.d.d.|.d
+00000530: 038d 057d 0574 0283 00a0 037c 047c 05a1  ...}.t.....|.|..
+00000540: 0201 0064 0053 0029 044e 7205 0000 0072  ...d.S.).Nr....r
+00000550: 0600 0000 7207 0000 0029 0472 0e00 0000  ....r....).r....
+00000560: 720f 0000 0072 0c00 0000 720d 0000 0029  r....r....r....)
+00000570: 0672 1400 0000 720b 0000 0072 1600 0000  .r....r....r....
+00000580: 720a 0000 0072 1000 0000 7212 0000 0072  r....r....r....r
+00000590: 1800 0000 721a 0000 0072 1b00 0000 720d  ....r....r....r.
+000005a0: 0000 002f 0000 0073 1e00 0000 0001 0401  .../...s........
+000005b0: 0201 0201 0201 0201 02fb 0607 0401 0201  ................
+000005c0: 0201 0201 0201 02fb 0607 7a14 4365 6e74  ..........z.Cent
+000005d0: 6572 426c 6f63 6b2e 5f5f 696e 6974 5f5f  erBlock.__init__
+000005e0: 2901 5429 0572 2800 0000 7229 0000 0072  ).T).r(...r)...r
+000005f0: 2a00 0000 720d 0000 0072 2b00 0000 721a  *...r....r+...r.
+00000600: 0000 0072 1a00 0000 7218 0000 0072 1b00  ...r....r....r..
+00000610: 0000 722c 0000 002e 0000 0073 0200 0000  ..r,.......s....
+00000620: 0801 722c 0000 0063 0000 0000 0000 0000  ..r,...c........
+00000630: 0000 0000 0000 0000 0400 0000 0000 0000  ................
+00000640: 7326 0000 0065 005a 0164 005a 0264 0987  s&...e.Z.d.Z.d..
+00000650: 0066 0164 0564 0684 095a 0364 0764 0884  .f.d.d...Z.d.d..
+00000660: 005a 0487 0004 005a 0553 0029 0ada 0b55  .Z.....Z.S.)...U
+00000670: 6e65 7444 6563 6f64 6572 e905 0000 0054  netDecoder.....T
+00000680: 4e46 6307 0000 0000 0000 0000 0000 000c  NFc.............
+00000690: 0000 0006 0000 0003 0000 0073 d200 0000  ...........s....
+000006a0: 7400 8300 a001 a100 0100 7c03 7402 7c02  t.........|.t.|.
+000006b0: 8301 6b03 722a 7403 6401 a004 7c03 7402  ..k.r*t.d...|.t.
+000006c0: 7c02 8301 a102 8301 8201 7c01 6402 6400  |.........|.d.d.
+000006d0: 8502 1900 7d01 7c01 6400 6400 6403 8503  ....}.|.d.d.d...
+000006e0: 1900 7d01 7c01 6404 1900 7d07 7c07 6701  ..}.|.d...}.|.g.
+000006f0: 7405 7c02 6400 6403 8502 1900 8301 1700  t.|.d.d.........
+00000700: 7d08 7405 7c01 6402 6400 8502 1900 8301  }.t.|.d.d.......
+00000710: 6404 6701 1700 7d09 7c02 7d0a 7c06 7292  d.g...}.|.}.|.r.
+00000720: 7406 7c07 7c07 7c04 6405 8d03 7c00 5f07  t.|.|.|.d...|._.
+00000730: 6e0a 7408 a009 a100 7c00 5f07 740a 7c04  n.t.....|._.t.|.
+00000740: 7c05 6406 8d02 8900 8700 6601 6407 6408  |.d.......f.d.d.
+00000750: 8408 740b 7c08 7c09 7c0a 8303 4400 8301  ..t.|.|.|...D...
+00000760: 7d0b 7408 a00c 7c0b a101 7c00 5f0d 6400  }.t...|...|._.d.
+00000770: 5300 2909 4e7a 444d 6f64 656c 2064 6570  S.).NzDModel dep
+00000780: 7468 2069 7320 7b7d 2c20 6275 7420 796f  th is {}, but yo
+00000790: 7520 7072 6f76 6964 6520 6064 6563 6f64  u provide `decod
+000007a0: 6572 5f63 6861 6e6e 656c 7360 2066 6f72  er_channels` for
+000007b0: 207b 7d20 626c 6f63 6b73 2e72 0600 0000   {} blocks.r....
+000007c0: e9ff ffff ff72 0100 0000 2901 720a 0000  .....r....).r...
+000007d0: 0029 0272 0a00 0000 7217 0000 0063 0100  .).r....r....c..
+000007e0: 0000 0000 0000 0000 0000 0400 0000 0600  ................
+000007f0: 0000 1300 0000 7322 0000 0067 007c 005d  ......s"...g.|.]
+00000800: 1a5c 037d 017d 027d 0374 007c 017c 027c  .\.}.}.}.t.|.|.|
+00000810: 0366 0388 008e 0191 0271 0453 0072 1a00  .f.......q.S.r..
+00000820: 0000 2901 7204 0000 0029 04da 022e 30da  ..).r....)....0.
+00000830: 0569 6e5f 6368 5a07 736b 6970 5f63 68da  .in_chZ.skip_ch.
+00000840: 066f 7574 5f63 68a9 01da 066b 7761 7267  .out_ch....kwarg
+00000850: 7372 1a00 0000 721b 0000 00da 0a3c 6c69  sr....r......<li
+00000860: 7374 636f 6d70 3e66 0000 0073 0400 0000  stcomp>f...s....
+00000870: 0602 08ff 7a28 556e 6574 4465 636f 6465  ....z(UnetDecode
+00000880: 722e 5f5f 696e 6974 5f5f 2e3c 6c6f 6361  r.__init__.<loca
+00000890: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 290e  ls>.<listcomp>).
+000008a0: 720c 0000 0072 0d00 0000 da03 6c65 6eda  r....r......len.
+000008b0: 0a56 616c 7565 4572 726f 72da 0666 6f72  .ValueError..for
+000008c0: 6d61 74da 046c 6973 7472 2c00 0000 da06  mat..listr,.....
+000008d0: 6365 6e74 6572 da02 6e6e da08 4964 656e  center..nn..Iden
+000008e0: 7469 7479 da04 6469 6374 da03 7a69 70da  tity..dict..zip.
+000008f0: 0a4d 6f64 756c 654c 6973 74da 0662 6c6f  .ModuleList..blo
+00000900: 636b 7329 0c72 1400 0000 da10 656e 636f  cks).r......enco
+00000910: 6465 725f 6368 616e 6e65 6c73 da10 6465  der_channels..de
+00000920: 636f 6465 725f 6368 616e 6e65 6c73 da08  coder_channels..
+00000930: 6e5f 626c 6f63 6b73 720a 0000 0072 1700  n_blocksr....r..
+00000940: 0000 723a 0000 005a 0d68 6561 645f 6368  ..r:...Z.head_ch
+00000950: 616e 6e65 6c73 720b 0000 0072 1500 0000  annelsr....r....
+00000960: 7216 0000 0072 4000 0000 7218 0000 0072  r....r@...r....r
+00000970: 3300 0000 721b 0000 0072 0d00 0000 4200  3...r....r....B.
+00000980: 0000 7334 0000 0000 090a 020c 0102 0104  ..s4............
+00000990: 0102 0006 ff02 ff04 060c 010e 0308 0116  ................
+000009a0: 0116 0104 0204 0102 0102 0002 0002 ff0a  ................
+000009b0: 040a 030c 010a 020a fe06 047a 1455 6e65  ...........z.Une
+000009c0: 7444 6563 6f64 6572 2e5f 5f69 6e69 745f  tDecoder.__init_
+000009d0: 5f63 0100 0000 0000 0000 0000 0000 0800  _c..............
+000009e0: 0000 0400 0000 4700 0000 7372 0000 007c  ......G...sr...|
+000009f0: 0164 0164 0085 0219 007d 017c 0164 0064  .d.d.....}.|.d.d
+00000a00: 0064 0285 0319 007d 017c 0164 0319 007d  .d.....}.|.d...}
+00000a10: 027c 0164 0164 0085 0219 007d 037c 00a0  .|.d.d.....}.|..
+00000a20: 007c 02a1 017d 0474 017c 006a 0283 0144  .|...}.t.|.j...D
+00000a30: 005d 2a5c 027d 057d 067c 0574 037c 0383  .]*\.}.}.|.t.|..
+00000a40: 016b 0072 5e7c 037c 0519 006e 0264 007d  .k.r^|.|...n.d.}
+00000a50: 077c 067c 047c 0783 027d 0471 427c 0453  .|.|.|...}.qB|.S
+00000a60: 0029 044e 7206 0000 0072 2f00 0000 7201  .).Nr....r/...r.
+00000a70: 0000 0029 0472 3a00 0000 da09 656e 756d  ...).r:.....enum
+00000a80: 6572 6174 6572 4000 0000 7236 0000 0029  erater@...r6...)
+00000a90: 0872 1400 0000 da08 6665 6174 7572 6573  .r......features
+00000aa0: da04 6865 6164 da05 736b 6970 7372 2400  ..head..skipsr$.
+00000ab0: 0000 da01 695a 0d64 6563 6f64 6572 5f62  ....iZ.decoder_b
+00000ac0: 6c6f 636b 7225 0000 0072 1a00 0000 721a  lockr%...r....r.
+00000ad0: 0000 0072 1b00 0000 7226 0000 006c 0000  ...r....r&...l..
+00000ae0: 0073 1200 0000 0002 0c01 0e02 0801 0c02  .s..............
+00000af0: 0a01 1201 1801 0c02 7a13 556e 6574 4465  ........z.UnetDe
+00000b00: 636f 6465 722e 666f 7277 6172 6429 0472  coder.forward).r
+00000b10: 2e00 0000 544e 4672 2700 0000 721a 0000  ....TNFr'...r...
+00000b20: 0072 1a00 0000 7218 0000 0072 1b00 0000  .r....r....r....
+00000b30: 722d 0000 0041 0000 0073 0c00 0000 0805  r-...A...s......
+00000b40: 0001 0001 0001 00f9 0e2a 722d 0000 0029  .........*r-...)
+00000b50: 0e72 2200 0000 da08 746f 7263 682e 6e6e  .r".....torch.nn
+00000b60: 723b 0000 005a 1374 6f72 6368 2e6e 6e2e  r;...Z.torch.nn.
+00000b70: 6675 6e63 7469 6f6e 616c da0a 6675 6e63  functional..func
+00000b80: 7469 6f6e 616c 7220 0000 00da 0462 6173  tionalr .....bas
+00000b90: 6572 0300 0000 720e 0000 00da 064d 6f64  er....r......Mod
+00000ba0: 756c 6572 0400 0000 da0a 5365 7175 656e  uler......Sequen
+00000bb0: 7469 616c 722c 0000 0072 2d00 0000 721a  tialr,...r-...r.
+00000bc0: 0000 0072 1a00 0000 721a 0000 0072 1b00  ...r....r....r..
+00000bd0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000be0: 730c 0000 0008 010c 0112 020c 0312 2612  s.............&.
+00000bf0: 13                                       .
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/decoder.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/unet/__pycache__/decoder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/model.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/unet/__pycache__/model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/model.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/unet/__pycache__/model.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/model.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/unet/__pycache__/model.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/model.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/unet/__pycache__/model.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:22 2023 UTC, .py size: 4306 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -198,42 +198,41 @@
 00000c50: 6f75 725f 7365 676d 656e 7461 7469 6f6e  our_segmentation
 00000c60: 5f68 6561 64da 0666 6f72 6d61 74da 046e  _head..format..n
 00000c70: 616d 65da 0a69 6e69 7469 616c 697a 6529  ame..initialize)
 00000c80: 0bda 0473 656c 6672 1600 0000 7217 0000  ...selfr....r...
 00000c90: 0072 1800 0000 7219 0000 0072 1a00 0000  .r....r....r....
 00000ca0: 721b 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
 00000cb0: 1e00 0000 721f 0000 00a9 01da 095f 5f63  ....r........__c
-00000cc0: 6c61 7373 5f5f a900 fa51 433a 5c55 7365  lass__...QC:\Use
+00000cc0: 6c61 7373 5f5f a900 fa44 633a 5c55 7365  lass__...Dc:\Use
 00000cd0: 7273 5c6d 6861 6e61 6e5c 446f 776e 6c6f  rs\mhanan\Downlo
-00000ce0: 6164 735c 4861 6e61 6e5c 4d61 6d6d 6f50  ads\Hanan\MammoP
-00000cf0: 795c 6d61 6d6d 6f70 795c 7365 676d 656e  y\mammopy\segmen
-00000d00: 7461 7469 6f6e 5f6d 6f64 656c 735c 756e  tation_models\un
-00000d10: 6574 5c6d 6f64 656c 2e70 7972 2900 0000  et\model.pyr)...
-00000d20: 2c00 0000 734a 0000 0000 0d0a 0202 0102  ,...sJ..........
-00000d30: 0102 0102 0102 fc08 0702 0106 0102 0102  ................
-00000d40: 0102 0110 0102 fa08 0902 0106 0102 0102  ................
-00000d50: 0102 fc08 0702 0106 0102 0102 0102 0110  ................
-00000d60: 0102 fa08 0902 0106 0102 0102 0102 fc08  ................
-00000d70: 090c 017a 0d55 6e65 742e 5f5f 696e 6974  ...z.Unet.__init
-00000d80: 5f5f 290a 720c 0000 0072 0d00 0000 720e  __).r....r....r.
-00000d90: 0000 0054 720f 0000 004e 7215 0000 0072  ...Tr....Nr....r
-00000da0: 0500 0000 4e4e 290e da08 5f5f 6e61 6d65  ....NN)...__name
-00000db0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00000dc0: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
-00000dd0: 646f 635f 5fda 0373 7472 da03 696e 74da  doc__..str..int.
-00000de0: 0462 6f6f 6c72 0400 0000 7202 0000 0072  .boolr....r....r
-00000df0: 0300 0000 da08 6361 6c6c 6162 6c65 da04  ......callable..
-00000e00: 6469 6374 7229 0000 00da 0d5f 5f63 6c61  dictr).....__cla
-00000e10: 7373 6365 6c6c 5f5f 7232 0000 0072 3200  sscell__r2...r2.
-00000e20: 0000 7230 0000 0072 3300 0000 720b 0000  ..r0...r3...r...
-00000e30: 0008 0000 0073 2e00 0000 0801 0425 0001  .....s.......%..
-00000e40: 0001 0001 0001 0001 0001 0001 0001 0001  ................
-00000e50: 00f5 0202 0201 0201 0201 0201 0601 0601  ................
-00000e60: 0201 0201 0e01 06f5 720b 0000 004e 290c  ........r....N).
-00000e70: da06 7479 7069 6e67 7202 0000 0072 0300  ..typingr....r..
-00000e80: 0000 7204 0000 00da 0764 6563 6f64 6572  ..r......decoder
-00000e90: 7206 0000 00da 0865 6e63 6f64 6572 7372  r......encodersr
-00000ea0: 0800 0000 da04 6261 7365 7209 0000 0072  ......baser....r
-00000eb0: 0a00 0000 720b 0000 0072 3200 0000 7232  ....r....r2...r2
-00000ec0: 0000 0072 3200 0000 7233 0000 00da 083c  ...r2...r3.....<
-00000ed0: 6d6f 6475 6c65 3e01 0000 0073 0a00 0000  module>....s....
-00000ee0: 1401 0c01 0c01 0c01 0c03                 ..........
+00000ce0: 6164 735c 4861 6e61 6e5c 6d67 5c73 6567  ads\Hanan\mg\seg
+00000cf0: 6d65 6e74 6174 696f 6e5f 6d6f 6465 6c73  mentation_models
+00000d00: 5c75 6e65 745c 6d6f 6465 6c2e 7079 7229  \unet\model.pyr)
+00000d10: 0000 002c 0000 0073 4a00 0000 000d 0a02  ...,...sJ.......
+00000d20: 0201 0201 0201 0201 02fc 0807 0201 0601  ................
+00000d30: 0201 0201 0201 1001 02fa 0809 0201 0601  ................
+00000d40: 0201 0201 02fc 0807 0201 0601 0201 0201  ................
+00000d50: 0201 1001 02fa 0809 0201 0601 0201 0201  ................
+00000d60: 02fc 0809 0c01 7a0d 556e 6574 2e5f 5f69  ......z.Unet.__i
+00000d70: 6e69 745f 5f29 0a72 0c00 0000 720d 0000  nit__).r....r...
+00000d80: 0072 0e00 0000 5472 0f00 0000 4e72 1500  .r....Tr....Nr..
+00000d90: 0000 7205 0000 004e 4e29 0eda 085f 5f6e  ..r....NN)...__n
+00000da0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00000db0: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
+00000dc0: 075f 5f64 6f63 5f5f da03 7374 72da 0369  .__doc__..str..i
+00000dd0: 6e74 da04 626f 6f6c 7204 0000 0072 0200  nt..boolr....r..
+00000de0: 0000 7203 0000 00da 0863 616c 6c61 626c  ..r......callabl
+00000df0: 65da 0464 6963 7472 2900 0000 da0d 5f5f  e..dictr).....__
+00000e00: 636c 6173 7363 656c 6c5f 5f72 3200 0000  classcell__r2...
+00000e10: 7232 0000 0072 3000 0000 7233 0000 0072  r2...r0...r3...r
+00000e20: 0b00 0000 0800 0000 732e 0000 0008 0104  ........s.......
+00000e30: 2500 0100 0100 0100 0100 0100 0100 0100  %...............
+00000e40: 0100 0100 f502 0202 0102 0102 0102 0106  ................
+00000e50: 0106 0102 0102 010e 0106 f572 0b00 0000  ...........r....
+00000e60: 4e29 0cda 0674 7970 696e 6772 0200 0000  N)...typingr....
+00000e70: 7203 0000 0072 0400 0000 da07 6465 636f  r....r......deco
+00000e80: 6465 7272 0600 0000 da08 656e 636f 6465  derr......encode
+00000e90: 7273 7208 0000 00da 0462 6173 6572 0900  rsr......baser..
+00000ea0: 0000 720a 0000 0072 0b00 0000 7232 0000  ..r....r....r2..
+00000eb0: 0072 3200 0000 7232 0000 0072 3300 0000  .r2...r2...r3...
+00000ec0: da08 3c6d 6f64 756c 653e 0100 0000 730a  ..<module>....s.
+00000ed0: 0000 0014 010c 010c 010c 010c 03         .............
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/unet/__pycache__/model.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/unet/__pycache__/model.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/unet/decoder.py` & `mammopy-0.0.9/segmentation_models/unet/decoder.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/unet/model.py` & `mammopy-0.0.9/segmentation_models/unet/model.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/base.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/base.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/base.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/base.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/base.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/base.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/base.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:22 2023 UTC, .py size: 2513 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -31,196 +31,195 @@
 000001e0: da08 4964 656e 7469 7479 da0a 6163 7469  ..Identity..acti
 000001f0: 7661 7469 6f6e da05 746f 7263 6872 0400  vation..torchr..
 00000200: 0000 da09 6675 6e63 746f 6f6c 73da 0770  ....functools..p
 00000210: 6172 7469 616c da07 736f 6674 6d61 78da  artial..softmax.
 00000220: 0863 616c 6c61 626c 65da 0a56 616c 7565  .callable..Value
 00000230: 4572 726f 7229 02da 0473 656c 6672 0c00  Error)...selfr..
 00000240: 0000 a901 da09 5f5f 636c 6173 735f 5fa9  ......__class__.
-00000250: 00fa 5143 3a5c 5573 6572 735c 6d68 616e  ..QC:\Users\mhan
+00000250: 00fa 4463 3a5c 5573 6572 735c 6d68 616e  ..Dc:\Users\mhan
 00000260: 616e 5c44 6f77 6e6c 6f61 6473 5c48 616e  an\Downloads\Han
-00000270: 616e 5c4d 616d 6d6f 5079 5c6d 616d 6d6f  an\MammoPy\mammo
-00000280: 7079 5c73 6567 6d65 6e74 6174 696f 6e5f  py\segmentation_
-00000290: 6d6f 6465 6c73 5c75 7469 6c73 5c62 6173  models\utils\bas
-000002a0: 652e 7079 7209 0000 0008 0000 0073 1400  e.pyr........s..
-000002b0: 0000 0001 0a01 1001 0c01 0801 0a01 0801  ................
-000002c0: 1401 0801 0802 7a13 4163 7469 7661 7469  ......z.Activati
-000002d0: 6f6e 2e5f 5f69 6e69 745f 5f63 0200 0000  on.__init__c....
-000002e0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-000002f0: 4300 0000 730a 0000 007c 00a0 007c 01a1  C...s....|...|..
-00000300: 0153 00a9 014e 2901 720c 0000 0029 0272  .S...N).r....).r
-00000310: 1300 0000 da01 7872 1600 0000 7216 0000  ......xr....r...
-00000320: 0072 1700 0000 da07 666f 7277 6172 6415  .r......forward.
-00000330: 0000 0073 0200 0000 0001 7a12 4163 7469  ...s......z.Acti
-00000340: 7661 7469 6f6e 2e66 6f72 7761 7264 2906  vation.forward).
-00000350: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000360: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000370: 6d65 5f5f 7209 0000 0072 1a00 0000 da0d  me__r....r......
-00000380: 5f5f 636c 6173 7363 656c 6c5f 5f72 1600  __classcell__r..
-00000390: 0000 7216 0000 0072 1400 0000 7217 0000  ..r....r....r...
-000003a0: 0072 0200 0000 0700 0000 7304 0000 0008  .r........s.....
-000003b0: 010c 0d72 0200 0000 6300 0000 0000 0000  ...r....c.......
-000003c0: 0000 0000 0000 0000 0004 0000 0000 0000  ................
-000003d0: 0073 2a00 0000 6500 5a01 6400 5a02 6406  .s*...e.Z.d.Z.d.
-000003e0: 8700 6601 6402 6403 8409 5a03 6504 6404  ..f.d.d...Z.e.d.
-000003f0: 6405 8400 8301 5a00 8700 0400 5a05 5300  d.....Z.....Z.S.
-00000400: 2907 da0a 4261 7365 4f62 6a65 6374 4e63  )...BaseObjectNc
-00000410: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000420: 0200 0000 0300 0000 7314 0000 0074 0083  ........s....t..
-00000430: 00a0 01a1 0001 007c 017c 005f 0264 0053  .......|.|._.d.S
-00000440: 0072 1800 0000 2903 7208 0000 0072 0900  .r....).r....r..
-00000450: 0000 da05 5f6e 616d 6529 0272 1300 0000  ...._name).r....
-00000460: da04 6e61 6d65 7214 0000 0072 1600 0000  ..namer....r....
-00000470: 7217 0000 0072 0900 0000 1a00 0000 7304  r....r........s.
-00000480: 0000 0000 010a 017a 1342 6173 654f 626a  .......z.BaseObj
-00000490: 6563 742e 5f5f 696e 6974 5f5f 6301 0000  ect.__init__c...
-000004a0: 0000 0000 0000 0000 0003 0000 0005 0000  ................
-000004b0: 0043 0000 0073 3c00 0000 7c00 6a00 6400  .C...s<...|.j.d.
-000004c0: 6b08 7232 7c00 6a01 6a02 7d01 7403 a004  k.r2|.j.j.}.t...
-000004d0: 6401 6402 7c01 a103 7d02 7403 a004 6403  d.d.|...}.t...d.
-000004e0: 6402 7c02 a103 a005 a100 5300 7c00 6a00  d.|.......S.|.j.
-000004f0: 5300 6400 5300 2904 4e7a 1028 2e29 285b  S.d.S.).Nz.(.)([
-00000500: 412d 5a5d 5b61 2d7a 5d2b 297a 055c 315f  A-Z][a-z]+)z.\1_
-00000510: 5c32 7a11 285b 612d 7a30 2d39 5d29 285b  \2z.([a-z0-9])([
-00000520: 412d 5a5d 2929 0672 2000 0000 7215 0000  A-Z])).r ...r...
-00000530: 0072 1b00 0000 da02 7265 da03 7375 62da  .r......re..sub.
-00000540: 056c 6f77 6572 2903 7213 0000 0072 2100  .lower).r....r!.
-00000550: 0000 da02 7331 7216 0000 0072 1600 0000  ....s1r....r....
-00000560: 7217 0000 0072 1b00 0000 1e00 0000 730a  r....r........s.
-00000570: 0000 0000 020a 0108 010e 0112 027a 1342  .............z.B
-00000580: 6173 654f 626a 6563 742e 5f5f 6e61 6d65  aseObject.__name
-00000590: 5f5f 2901 4e29 0672 1b00 0000 721c 0000  __).N).r....r...
-000005a0: 0072 1d00 0000 7209 0000 00da 0870 726f  .r....r......pro
-000005b0: 7065 7274 7972 1e00 0000 7216 0000 0072  pertyr....r....r
-000005c0: 1600 0000 7214 0000 0072 1700 0000 721f  ....r....r....r.
-000005d0: 0000 0018 0000 0073 0600 0000 0802 0e04  .......s........
-000005e0: 0201 721f 0000 0063 0000 0000 0000 0000  ..r....c........
-000005f0: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
-00000600: 730c 0000 0065 005a 0164 005a 0264 0153  s....e.Z.d.Z.d.S
-00000610: 0029 02da 064d 6574 7269 634e 2903 721b  .)...MetricN).r.
-00000620: 0000 0072 1c00 0000 721d 0000 0072 1600  ...r....r....r..
-00000630: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00000640: 0072 2700 0000 2800 0000 7302 0000 0008  .r'...(...s.....
-00000650: 0172 2700 0000 6300 0000 0000 0000 0000  .r'...c.........
-00000660: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
-00000670: 2c00 0000 6500 5a01 6400 5a02 6401 6402  ,...e.Z.d.Z.d.d.
-00000680: 8400 5a03 6403 6404 8400 5a04 6405 6406  ..Z.d.d...Z.d.d.
-00000690: 8400 5a05 6407 6408 8400 5a06 6409 5300  ..Z.d.d...Z.d.S.
-000006a0: 290a da04 4c6f 7373 6302 0000 0000 0000  )...Lossc.......
-000006b0: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
-000006c0: 0073 2000 0000 7400 7c01 7401 8302 7214  .s ...t.|.t...r.
-000006d0: 7402 7c00 7c01 8302 5300 7403 6401 8301  t.|.|...S.t.d...
-000006e0: 8201 6400 5300 2902 4e7a 2a4c 6f73 7320  ..d.S.).Nz*Loss 
-000006f0: 7368 6f75 6c64 2062 6520 696e 6865 7269  should be inheri
-00000700: 7465 6420 6672 6f6d 2060 4c6f 7373 6020  ted from `Loss` 
-00000710: 636c 6173 7329 04da 0a69 7369 6e73 7461  class)...isinsta
-00000720: 6e63 6572 2800 0000 da0b 5375 6d4f 664c  ncer(.....SumOfL
-00000730: 6f73 7365 7372 1200 0000 a902 7213 0000  ossesr......r...
-00000740: 00da 056f 7468 6572 7216 0000 0072 1600  ...otherr....r..
-00000750: 0000 7217 0000 00da 075f 5f61 6464 5f5f  ..r......__add__
-00000760: 2e00 0000 7306 0000 0000 010a 010a 027a  ....s..........z
-00000770: 0c4c 6f73 732e 5f5f 6164 645f 5f63 0200  .Loss.__add__c..
-00000780: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00000790: 0000 4300 0000 730a 0000 007c 00a0 007c  ..C...s....|...|
-000007a0: 01a1 0153 0072 1800 0000 2901 722d 0000  ...S.r....).r-..
-000007b0: 0072 2b00 0000 7216 0000 0072 1600 0000  .r+...r....r....
-000007c0: 7217 0000 00da 085f 5f72 6164 645f 5f34  r......__radd__4
-000007d0: 0000 0073 0200 0000 0001 7a0d 4c6f 7373  ...s......z.Loss
-000007e0: 2e5f 5f72 6164 645f 5f63 0200 0000 0000  .__radd__c......
-000007f0: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-00000800: 0000 7324 0000 0074 007c 0174 0174 0266  ..s$...t.|.t.t.f
-00000810: 0283 0272 1874 037c 007c 0183 0253 0074  ...r.t.|.|...S.t
-00000820: 0464 0183 0182 0164 0053 0029 024e 7a2e  .d.....d.S.).Nz.
-00000830: 4c6f 7373 2073 686f 756c 6420 6265 2069  Loss should be i
-00000840: 6e68 6572 6974 6564 2066 726f 6d20 6042  nherited from `B
-00000850: 6173 654c 6f73 7360 2063 6c61 7373 2905  aseLoss` class).
-00000860: 7229 0000 00da 0369 6e74 da05 666c 6f61  r).....int..floa
-00000870: 74da 0e4d 756c 7469 706c 6965 644c 6f73  t..MultipliedLos
-00000880: 7372 1200 0000 2902 7213 0000 00da 0576  sr....).r......v
-00000890: 616c 7565 7216 0000 0072 1600 0000 7217  aluer....r....r.
-000008a0: 0000 00da 075f 5f6d 756c 5f5f 3700 0000  .....__mul__7...
-000008b0: 7306 0000 0000 010e 010a 027a 0c4c 6f73  s..........z.Los
-000008c0: 732e 5f5f 6d75 6c5f 5f63 0200 0000 0000  s.__mul__c......
-000008d0: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
-000008e0: 0000 730a 0000 007c 00a0 007c 01a1 0153  ..s....|...|...S
-000008f0: 0072 1800 0000 2901 7233 0000 0072 2b00  .r....).r3...r+.
-00000900: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00000910: 00da 085f 5f72 6d75 6c5f 5f3d 0000 0073  ...__rmul__=...s
-00000920: 0200 0000 0001 7a0d 4c6f 7373 2e5f 5f72  ......z.Loss.__r
-00000930: 6d75 6c5f 5f4e 2907 721b 0000 0072 1c00  mul__N).r....r..
-00000940: 0000 721d 0000 0072 2d00 0000 722e 0000  ..r....r-...r...
-00000950: 0072 3300 0000 7234 0000 0072 1600 0000  .r3...r4...r....
-00000960: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-00000970: 2800 0000 2c00 0000 7308 0000 0008 0208  (...,...s.......
-00000980: 0608 0308 0672 2800 0000 6300 0000 0000  .....r(...c.....
-00000990: 0000 0000 0000 0000 0000 0003 0000 0000  ................
-000009a0: 0000 0073 2400 0000 6500 5a01 6400 5a02  ...s$...e.Z.d.Z.
-000009b0: 8700 6601 6401 6402 8408 5a03 6403 6404  ..f.d.d...Z.d.d.
-000009c0: 8400 5a04 8700 0400 5a05 5300 2905 722a  ..Z.....Z.S.).r*
-000009d0: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
-000009e0: 0400 0000 0400 0000 0300 0000 732e 0000  ............s...
-000009f0: 0064 01a0 007c 016a 017c 026a 01a1 027d  .d...|.j.|.j...}
-00000a00: 0374 0283 006a 037c 0364 028d 0101 007c  .t...j.|.d.....|
-00000a10: 017c 005f 047c 027c 005f 0564 0053 0029  .|._.|.|._.d.S.)
-00000a20: 034e 7a07 7b7d 202b 207b 7da9 0172 2100  .Nz.{} + {}..r!.
-00000a30: 0000 2906 da06 666f 726d 6174 721b 0000  ..)...formatr...
-00000a40: 0072 0800 0000 7209 0000 00da 026c 31da  .r....r......l1.
-00000a50: 026c 3229 0472 1300 0000 7237 0000 0072  .l2).r....r7...r
-00000a60: 3800 0000 7221 0000 0072 1400 0000 7216  8...r!...r....r.
-00000a70: 0000 0072 1700 0000 7209 0000 0043 0000  ...r....r....C..
-00000a80: 0073 0800 0000 0001 1001 0e01 0601 7a14  .s............z.
-00000a90: 5375 6d4f 664c 6f73 7365 732e 5f5f 696e  SumOfLosses.__in
-00000aa0: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
-00000ab0: 0002 0000 0003 0000 0047 0000 0073 1800  .........G...s..
-00000ac0: 0000 7c00 6a00 6a01 7c01 8e00 7c00 6a02  ..|.j.j.|...|.j.
-00000ad0: 6a01 7c01 8e00 1700 5300 7218 0000 0029  j.|.....S.r....)
-00000ae0: 0372 3700 0000 721a 0000 0072 3800 0000  .r7...r....r8...
-00000af0: a902 7213 0000 00da 0669 6e70 7574 7372  ..r......inputsr
-00000b00: 1600 0000 7216 0000 0072 1700 0000 da08  ....r....r......
-00000b10: 5f5f 6361 6c6c 5f5f 4900 0000 7302 0000  __call__I...s...
-00000b20: 0000 017a 1453 756d 4f66 4c6f 7373 6573  ...z.SumOfLosses
-00000b30: 2e5f 5f63 616c 6c5f 5fa9 0672 1b00 0000  .__call__..r....
-00000b40: 721c 0000 0072 1d00 0000 7209 0000 0072  r....r....r....r
-00000b50: 3b00 0000 721e 0000 0072 1600 0000 7216  ;...r....r....r.
-00000b60: 0000 0072 1400 0000 7217 0000 0072 2a00  ...r....r....r*.
-00000b70: 0000 4100 0000 7304 0000 0008 020c 0672  ..A...s........r
-00000b80: 2a00 0000 6300 0000 0000 0000 0000 0000  *...c...........
-00000b90: 0000 0000 0003 0000 0000 0000 0073 2400  .............s$.
-00000ba0: 0000 6500 5a01 6400 5a02 8700 6601 6401  ..e.Z.d.Z...f.d.
-00000bb0: 6402 8408 5a03 6403 6404 8400 5a04 8700  d...Z.d.d...Z...
-00000bc0: 0400 5a05 5300 2905 7231 0000 0063 0300  ..Z.S.).r1...c..
-00000bd0: 0000 0000 0000 0000 0000 0400 0000 0400  ................
-00000be0: 0000 0300 0000 7350 0000 0074 007c 016a  ......sP...t.|.j
-00000bf0: 01a0 0264 01a1 0183 0164 026b 0472 2464  ...d.....d.k.r$d
-00000c00: 03a0 037c 027c 016a 01a1 027d 036e 0e64  ...|.|.j...}.n.d
-00000c10: 04a0 037c 027c 016a 01a1 027d 0374 0483  ...|.|.j...}.t..
-00000c20: 006a 057c 0364 058d 0101 007c 017c 005f  .j.|.d.....|.|._
-00000c30: 067c 027c 005f 0764 0053 0029 064e fa01  .|.|._.d.S.).N..
-00000c40: 2b72 0600 0000 7a09 7b7d 202a 2028 7b7d  +r....z.{} * ({}
-00000c50: 297a 077b 7d20 2a20 7b7d 7235 0000 0029  )z.{} * {}r5...)
-00000c60: 08da 036c 656e 721b 0000 00da 0573 706c  ...lenr......spl
-00000c70: 6974 7236 0000 0072 0800 0000 7209 0000  itr6...r....r...
-00000c80: 00da 046c 6f73 73da 0a6d 756c 7469 706c  ...loss..multipl
-00000c90: 6965 7229 0472 1300 0000 7240 0000 0072  ier).r....r@...r
-00000ca0: 4100 0000 7221 0000 0072 1400 0000 7216  A...r!...r....r.
-00000cb0: 0000 0072 1700 0000 7209 0000 004f 0000  ...r....r....O..
-00000cc0: 0073 0c00 0000 0003 1401 1002 0e01 0e01  .s..............
-00000cd0: 0601 7a17 4d75 6c74 6970 6c69 6564 4c6f  ..z.MultipliedLo
-00000ce0: 7373 2e5f 5f69 6e69 745f 5f63 0100 0000  ss.__init__c....
-00000cf0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00000d00: 4700 0000 7312 0000 007c 006a 007c 006a  G...s....|.j.|.j
-00000d10: 016a 027c 018e 0014 0053 0072 1800 0000  .j.|.....S.r....
-00000d20: 2903 7241 0000 0072 4000 0000 721a 0000  ).rA...r@...r...
-00000d30: 0072 3900 0000 7216 0000 0072 1600 0000  .r9...r....r....
-00000d40: 7217 0000 0072 3b00 0000 5a00 0000 7302  r....r;...Z...s.
-00000d50: 0000 0000 017a 174d 756c 7469 706c 6965  .....z.Multiplie
-00000d60: 644c 6f73 732e 5f5f 6361 6c6c 5f5f 723c  dLoss.__call__r<
-00000d70: 0000 0072 1600 0000 7216 0000 0072 1400  ...r....r....r..
-00000d80: 0000 7217 0000 0072 3100 0000 4d00 0000  ..r....r1...M...
-00000d90: 7304 0000 0008 020c 0b72 3100 0000 290c  s........r1...).
-00000da0: 7222 0000 0072 0e00 0000 720d 0000 00da  r"...r....r.....
-00000db0: 0874 6f72 6368 2e6e 6e72 0a00 0000 da06  .torch.nnr......
-00000dc0: 4d6f 6475 6c65 7202 0000 0072 1f00 0000  Moduler....r....
-00000dd0: 7227 0000 0072 2800 0000 722a 0000 0072  r'...r(...r*...r
-00000de0: 3100 0000 7216 0000 0072 1600 0000 7216  1...r....r....r.
-00000df0: 0000 0072 1700 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000e00: 653e 0100 0000 7312 0000 0008 0108 0108  e>....s.........
-00000e10: 010c 0312 1112 1010 0410 1510 0c         .............
+00000270: 616e 5c6d 675c 7365 676d 656e 7461 7469  an\mg\segmentati
+00000280: 6f6e 5f6d 6f64 656c 735c 7574 696c 735c  on_models\utils\
+00000290: 6261 7365 2e70 7972 0900 0000 0800 0000  base.pyr........
+000002a0: 7314 0000 0000 010a 0110 010c 0108 010a  s...............
+000002b0: 0108 0114 0108 0108 027a 1341 6374 6976  .........z.Activ
+000002c0: 6174 696f 6e2e 5f5f 696e 6974 5f5f 6302  ation.__init__c.
+000002d0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+000002e0: 0000 0043 0000 0073 0a00 0000 7c00 a000  ...C...s....|...
+000002f0: 7c01 a101 5300 a901 4e29 0172 0c00 0000  |...S...N).r....
+00000300: 2902 7213 0000 00da 0178 7216 0000 0072  ).r......xr....r
+00000310: 1600 0000 7217 0000 00da 0766 6f72 7761  ....r......forwa
+00000320: 7264 1500 0000 7302 0000 0000 017a 1241  rd....s......z.A
+00000330: 6374 6976 6174 696f 6e2e 666f 7277 6172  ctivation.forwar
+00000340: 6429 06da 085f 5f6e 616d 655f 5fda 0a5f  d)...__name__.._
+00000350: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000360: 6c6e 616d 655f 5f72 0900 0000 721a 0000  lname__r....r...
+00000370: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
+00000380: 7216 0000 0072 1600 0000 7214 0000 0072  r....r....r....r
+00000390: 1700 0000 7202 0000 0007 0000 0073 0400  ....r........s..
+000003a0: 0000 0801 0c0d 7202 0000 0063 0000 0000  ......r....c....
+000003b0: 0000 0000 0000 0000 0000 0000 0400 0000  ................
+000003c0: 0000 0000 732a 0000 0065 005a 0164 005a  ....s*...e.Z.d.Z
+000003d0: 0264 0687 0066 0164 0264 0384 095a 0365  .d...f.d.d...Z.e
+000003e0: 0464 0464 0584 0083 015a 0087 0004 005a  .d.d.....Z.....Z
+000003f0: 0553 0029 07da 0a42 6173 654f 626a 6563  .S.)...BaseObjec
+00000400: 744e 6302 0000 0000 0000 0000 0000 0002  tNc.............
+00000410: 0000 0002 0000 0003 0000 0073 1400 0000  ...........s....
+00000420: 7400 8300 a001 a100 0100 7c01 7c00 5f02  t.........|.|._.
+00000430: 6400 5300 7218 0000 0029 0372 0800 0000  d.S.r....).r....
+00000440: 7209 0000 00da 055f 6e61 6d65 2902 7213  r......_name).r.
+00000450: 0000 00da 046e 616d 6572 1400 0000 7216  .....namer....r.
+00000460: 0000 0072 1700 0000 7209 0000 001a 0000  ...r....r.......
+00000470: 0073 0400 0000 0001 0a01 7a13 4261 7365  .s........z.Base
+00000480: 4f62 6a65 6374 2e5f 5f69 6e69 745f 5f63  Object.__init__c
+00000490: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+000004a0: 0500 0000 4300 0000 733c 0000 007c 006a  ....C...s<...|.j
+000004b0: 0064 006b 0872 327c 006a 016a 027d 0174  .d.k.r2|.j.j.}.t
+000004c0: 03a0 0464 0164 027c 01a1 037d 0274 03a0  ...d.d.|...}.t..
+000004d0: 0464 0364 027c 02a1 03a0 05a1 0053 007c  .d.d.|.......S.|
+000004e0: 006a 0053 0064 0053 0029 044e 7a10 282e  .j.S.d.S.).Nz.(.
+000004f0: 2928 5b41 2d5a 5d5b 612d 7a5d 2b29 7a05  )([A-Z][a-z]+)z.
+00000500: 5c31 5f5c 327a 1128 5b61 2d7a 302d 395d  \1_\2z.([a-z0-9]
+00000510: 2928 5b41 2d5a 5d29 2906 7220 0000 0072  )([A-Z])).r ...r
+00000520: 1500 0000 721b 0000 00da 0272 65da 0373  ....r......re..s
+00000530: 7562 da05 6c6f 7765 7229 0372 1300 0000  ub..lower).r....
+00000540: 7221 0000 00da 0273 3172 1600 0000 7216  r!.....s1r....r.
+00000550: 0000 0072 1700 0000 721b 0000 001e 0000  ...r....r.......
+00000560: 0073 0a00 0000 0002 0a01 0801 0e01 1202  .s..............
+00000570: 7a13 4261 7365 4f62 6a65 6374 2e5f 5f6e  z.BaseObject.__n
+00000580: 616d 655f 5f29 014e 2906 721b 0000 0072  ame__).N).r....r
+00000590: 1c00 0000 721d 0000 0072 0900 0000 da08  ....r....r......
+000005a0: 7072 6f70 6572 7479 721e 0000 0072 1600  propertyr....r..
+000005b0: 0000 7216 0000 0072 1400 0000 7217 0000  ..r....r....r...
+000005c0: 0072 1f00 0000 1800 0000 7306 0000 0008  .r........s.....
+000005d0: 020e 0402 0172 1f00 0000 6300 0000 0000  .....r....c.....
+000005e0: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
+000005f0: 0000 0073 0c00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00000600: 6401 5300 2902 da06 4d65 7472 6963 4e29  d.S.)...MetricN)
+00000610: 0372 1b00 0000 721c 0000 0072 1d00 0000  .r....r....r....
+00000620: 7216 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
+00000630: 1700 0000 7227 0000 0028 0000 0073 0200  ....r'...(...s..
+00000640: 0000 0801 7227 0000 0063 0000 0000 0000  ....r'...c......
+00000650: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
+00000660: 0000 732c 0000 0065 005a 0164 005a 0264  ..s,...e.Z.d.Z.d
+00000670: 0164 0284 005a 0364 0364 0484 005a 0464  .d...Z.d.d...Z.d
+00000680: 0564 0684 005a 0564 0764 0884 005a 0664  .d...Z.d.d...Z.d
+00000690: 0953 0029 0ada 044c 6f73 7363 0200 0000  .S.)...Lossc....
+000006a0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+000006b0: 4300 0000 7320 0000 0074 007c 0174 0183  C...s ...t.|.t..
+000006c0: 0272 1474 027c 007c 0183 0253 0074 0364  .r.t.|.|...S.t.d
+000006d0: 0183 0182 0164 0053 0029 024e 7a2a 4c6f  .....d.S.).Nz*Lo
+000006e0: 7373 2073 686f 756c 6420 6265 2069 6e68  ss should be inh
+000006f0: 6572 6974 6564 2066 726f 6d20 604c 6f73  erited from `Los
+00000700: 7360 2063 6c61 7373 2904 da0a 6973 696e  s` class)...isin
+00000710: 7374 616e 6365 7228 0000 00da 0b53 756d  stancer(.....Sum
+00000720: 4f66 4c6f 7373 6573 7212 0000 00a9 0272  OfLossesr......r
+00000730: 1300 0000 da05 6f74 6865 7272 1600 0000  ......otherr....
+00000740: 7216 0000 0072 1700 0000 da07 5f5f 6164  r....r......__ad
+00000750: 645f 5f2e 0000 0073 0600 0000 0001 0a01  d__....s........
+00000760: 0a02 7a0c 4c6f 7373 2e5f 5f61 6464 5f5f  ..z.Loss.__add__
+00000770: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00000780: 0003 0000 0043 0000 0073 0a00 0000 7c00  .....C...s....|.
+00000790: a000 7c01 a101 5300 7218 0000 0029 0172  ..|...S.r....).r
+000007a0: 2d00 0000 722b 0000 0072 1600 0000 7216  -...r+...r....r.
+000007b0: 0000 0072 1700 0000 da08 5f5f 7261 6464  ...r......__radd
+000007c0: 5f5f 3400 0000 7302 0000 0000 017a 0d4c  __4...s......z.L
+000007d0: 6f73 732e 5f5f 7261 6464 5f5f 6302 0000  oss.__radd__c...
+000007e0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+000007f0: 0043 0000 0073 2400 0000 7400 7c01 7401  .C...s$...t.|.t.
+00000800: 7402 6602 8302 7218 7403 7c00 7c01 8302  t.f...r.t.|.|...
+00000810: 5300 7404 6401 8301 8201 6400 5300 2902  S.t.d.....d.S.).
+00000820: 4e7a 2e4c 6f73 7320 7368 6f75 6c64 2062  Nz.Loss should b
+00000830: 6520 696e 6865 7269 7465 6420 6672 6f6d  e inherited from
+00000840: 2060 4261 7365 4c6f 7373 6020 636c 6173   `BaseLoss` clas
+00000850: 7329 0572 2900 0000 da03 696e 74da 0566  s).r).....int..f
+00000860: 6c6f 6174 da0e 4d75 6c74 6970 6c69 6564  loat..Multiplied
+00000870: 4c6f 7373 7212 0000 0029 0272 1300 0000  Lossr....).r....
+00000880: da05 7661 6c75 6572 1600 0000 7216 0000  ..valuer....r...
+00000890: 0072 1700 0000 da07 5f5f 6d75 6c5f 5f37  .r......__mul__7
+000008a0: 0000 0073 0600 0000 0001 0e01 0a02 7a0c  ...s..........z.
+000008b0: 4c6f 7373 2e5f 5f6d 756c 5f5f 6302 0000  Loss.__mul__c...
+000008c0: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+000008d0: 0043 0000 0073 0a00 0000 7c00 a000 7c01  .C...s....|...|.
+000008e0: a101 5300 7218 0000 0029 0172 3300 0000  ..S.r....).r3...
+000008f0: 722b 0000 0072 1600 0000 7216 0000 0072  r+...r....r....r
+00000900: 1700 0000 da08 5f5f 726d 756c 5f5f 3d00  ......__rmul__=.
+00000910: 0000 7302 0000 0000 017a 0d4c 6f73 732e  ..s......z.Loss.
+00000920: 5f5f 726d 756c 5f5f 4e29 0772 1b00 0000  __rmul__N).r....
+00000930: 721c 0000 0072 1d00 0000 722d 0000 0072  r....r....r-...r
+00000940: 2e00 0000 7233 0000 0072 3400 0000 7216  ....r3...r4...r.
+00000950: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+00000960: 0000 7228 0000 002c 0000 0073 0800 0000  ..r(...,...s....
+00000970: 0802 0806 0803 0806 7228 0000 0063 0000  ........r(...c..
+00000980: 0000 0000 0000 0000 0000 0000 0000 0300  ................
+00000990: 0000 0000 0000 7324 0000 0065 005a 0164  ......s$...e.Z.d
+000009a0: 005a 0287 0066 0164 0164 0284 085a 0364  .Z...f.d.d...Z.d
+000009b0: 0364 0484 005a 0487 0004 005a 0553 0029  .d...Z.....Z.S.)
+000009c0: 0572 2a00 0000 6303 0000 0000 0000 0000  .r*...c.........
+000009d0: 0000 0004 0000 0004 0000 0003 0000 0073  ...............s
+000009e0: 2e00 0000 6401 a000 7c01 6a01 7c02 6a01  ....d...|.j.|.j.
+000009f0: a102 7d03 7402 8300 6a03 7c03 6402 8d01  ..}.t...j.|.d...
+00000a00: 0100 7c01 7c00 5f04 7c02 7c00 5f05 6400  ..|.|._.|.|._.d.
+00000a10: 5300 2903 4e7a 077b 7d20 2b20 7b7d a901  S.).Nz.{} + {}..
+00000a20: 7221 0000 0029 06da 0666 6f72 6d61 7472  r!...)...formatr
+00000a30: 1b00 0000 7208 0000 0072 0900 0000 da02  ....r....r......
+00000a40: 6c31 da02 6c32 2904 7213 0000 0072 3700  l1..l2).r....r7.
+00000a50: 0000 7238 0000 0072 2100 0000 7214 0000  ..r8...r!...r...
+00000a60: 0072 1600 0000 7217 0000 0072 0900 0000  .r....r....r....
+00000a70: 4300 0000 7308 0000 0000 0110 010e 0106  C...s...........
+00000a80: 017a 1453 756d 4f66 4c6f 7373 6573 2e5f  .z.SumOfLosses._
+00000a90: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
+00000aa0: 0000 0000 0200 0000 0300 0000 4700 0000  ............G...
+00000ab0: 7318 0000 007c 006a 006a 017c 018e 007c  s....|.j.j.|...|
+00000ac0: 006a 026a 017c 018e 0017 0053 0072 1800  .j.j.|.....S.r..
+00000ad0: 0000 2903 7237 0000 0072 1a00 0000 7238  ..).r7...r....r8
+00000ae0: 0000 00a9 0272 1300 0000 da06 696e 7075  .....r......inpu
+00000af0: 7473 7216 0000 0072 1600 0000 7217 0000  tsr....r....r...
+00000b00: 00da 085f 5f63 616c 6c5f 5f49 0000 0073  ...__call__I...s
+00000b10: 0200 0000 0001 7a14 5375 6d4f 664c 6f73  ......z.SumOfLos
+00000b20: 7365 732e 5f5f 6361 6c6c 5f5f a906 721b  ses.__call__..r.
+00000b30: 0000 0072 1c00 0000 721d 0000 0072 0900  ...r....r....r..
+00000b40: 0000 723b 0000 0072 1e00 0000 7216 0000  ..r;...r....r...
+00000b50: 0072 1600 0000 7214 0000 0072 1700 0000  .r....r....r....
+00000b60: 722a 0000 0041 0000 0073 0400 0000 0802  r*...A...s......
+00000b70: 0c06 722a 0000 0063 0000 0000 0000 0000  ..r*...c........
+00000b80: 0000 0000 0000 0000 0300 0000 0000 0000  ................
+00000b90: 7324 0000 0065 005a 0164 005a 0287 0066  s$...e.Z.d.Z...f
+00000ba0: 0164 0164 0284 085a 0364 0364 0484 005a  .d.d...Z.d.d...Z
+00000bb0: 0487 0004 005a 0553 0029 0572 3100 0000  .....Z.S.).r1...
+00000bc0: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
+00000bd0: 0004 0000 0003 0000 0073 5000 0000 7400  .........sP...t.
+00000be0: 7c01 6a01 a002 6401 a101 8301 6402 6b04  |.j...d.....d.k.
+00000bf0: 7224 6403 a003 7c02 7c01 6a01 a102 7d03  r$d...|.|.j...}.
+00000c00: 6e0e 6404 a003 7c02 7c01 6a01 a102 7d03  n.d...|.|.j...}.
+00000c10: 7404 8300 6a05 7c03 6405 8d01 0100 7c01  t...j.|.d.....|.
+00000c20: 7c00 5f06 7c02 7c00 5f07 6400 5300 2906  |._.|.|._.d.S.).
+00000c30: 4efa 012b 7206 0000 007a 097b 7d20 2a20  N..+r....z.{} * 
+00000c40: 287b 7d29 7a07 7b7d 202a 207b 7d72 3500  ({})z.{} * {}r5.
+00000c50: 0000 2908 da03 6c65 6e72 1b00 0000 da05  ..)...lenr......
+00000c60: 7370 6c69 7472 3600 0000 7208 0000 0072  splitr6...r....r
+00000c70: 0900 0000 da04 6c6f 7373 da0a 6d75 6c74  ......loss..mult
+00000c80: 6970 6c69 6572 2904 7213 0000 0072 4000  iplier).r....r@.
+00000c90: 0000 7241 0000 0072 2100 0000 7214 0000  ..rA...r!...r...
+00000ca0: 0072 1600 0000 7217 0000 0072 0900 0000  .r....r....r....
+00000cb0: 4f00 0000 730c 0000 0000 0314 0110 020e  O...s...........
+00000cc0: 010e 0106 017a 174d 756c 7469 706c 6965  .....z.Multiplie
+00000cd0: 644c 6f73 732e 5f5f 696e 6974 5f5f 6301  dLoss.__init__c.
+00000ce0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00000cf0: 0000 0047 0000 0073 1200 0000 7c00 6a00  ...G...s....|.j.
+00000d00: 7c00 6a01 6a02 7c01 8e00 1400 5300 7218  |.j.j.|.....S.r.
+00000d10: 0000 0029 0372 4100 0000 7240 0000 0072  ...).rA...r@...r
+00000d20: 1a00 0000 7239 0000 0072 1600 0000 7216  ....r9...r....r.
+00000d30: 0000 0072 1700 0000 723b 0000 005a 0000  ...r....r;...Z..
+00000d40: 0073 0200 0000 0001 7a17 4d75 6c74 6970  .s......z.Multip
+00000d50: 6c69 6564 4c6f 7373 2e5f 5f63 616c 6c5f  liedLoss.__call_
+00000d60: 5f72 3c00 0000 7216 0000 0072 1600 0000  _r<...r....r....
+00000d70: 7214 0000 0072 1700 0000 7231 0000 004d  r....r....r1...M
+00000d80: 0000 0073 0400 0000 0802 0c0b 7231 0000  ...s........r1..
+00000d90: 0029 0c72 2200 0000 720e 0000 0072 0d00  .).r"...r....r..
+00000da0: 0000 da08 746f 7263 682e 6e6e 720a 0000  ....torch.nnr...
+00000db0: 00da 064d 6f64 756c 6572 0200 0000 721f  ...Moduler....r.
+00000dc0: 0000 0072 2700 0000 7228 0000 0072 2a00  ...r'...r(...r*.
+00000dd0: 0000 7231 0000 0072 1600 0000 7216 0000  ..r1...r....r...
+00000de0: 0072 1600 0000 7217 0000 00da 083c 6d6f  .r....r......<mo
+00000df0: 6475 6c65 3e01 0000 0073 1200 0000 0801  dule>....s......
+00000e00: 0801 0801 0c03 1211 1210 1004 1015 100c  ................
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/base.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/functional.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/functional.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/functional.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/functional.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/functional.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/functional.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/functional.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/functional.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:22 2023 UTC, .py size: 5051 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -18,276 +18,275 @@
 00000110: 0189 0087 0066 0164 0564 0284 087c 0144  .....f.d.d...|.D
 00000120: 0083 017d 017c 0153 0064 0053 0029 064e  ...}.|.S.d.S.).N
 00000130: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
 00000140: 0004 0000 0013 0000 0073 1800 0000 6700  .........s....g.
 00000150: 7c00 5d10 7d01 7c01 8800 6b07 7204 7c01  |.].}.|...k.r.|.
 00000160: 9102 7104 5300 a900 7204 0000 0029 02da  ..q.S...r....)..
 00000170: 022e 30da 0763 6861 6e6e 656c 7202 0000  ..0..channelr...
-00000180: 0072 0400 0000 fa57 433a 5c55 7365 7273  .r.....WC:\Users
+00000180: 0072 0400 0000 fa4a 633a 5c55 7365 7273  .r.....Jc:\Users
 00000190: 5c6d 6861 6e61 6e5c 446f 776e 6c6f 6164  \mhanan\Download
-000001a0: 735c 4861 6e61 6e5c 4d61 6d6d 6f50 795c  s\Hanan\MammoPy\
-000001b0: 6d61 6d6d 6f70 795c 7365 676d 656e 7461  mammopy\segmenta
-000001c0: 7469 6f6e 5f6d 6f64 656c 735c 7574 696c  tion_models\util
-000001d0: 735c 6675 6e63 7469 6f6e 616c 2e70 79da  s\functional.py.
-000001e0: 0a3c 6c69 7374 636f 6d70 3e08 0000 0073  .<listcomp>....s
-000001f0: 0600 0000 0600 0200 0800 7a22 5f74 616b  ..........z"_tak
-00000200: 655f 6368 616e 6e65 6c73 2e3c 6c6f 6361  e_channels.<loca
-00000210: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7201  ls>.<listcomp>r.
-00000220: 0000 00e9 0100 0000 6301 0000 0000 0000  ........c.......
-00000230: 0000 0000 0002 0000 0008 0000 0013 0000  ................
-00000240: 0073 2a00 0000 6700 7c00 5d22 7d01 7400  .s*...g.|.]"}.t.
-00000250: 6a01 7c01 6400 7400 a002 8800 a101 a003  j.|.d.t.........
-00000260: 7c01 6a04 a101 6401 8d03 9102 7104 5300  |.j...d.....q.S.
-00000270: 2902 7209 0000 0029 02da 0364 696d da05  ).r....)...dim..
-00000280: 696e 6465 7829 05da 0574 6f72 6368 da0c  index)...torch..
-00000290: 696e 6465 785f 7365 6c65 6374 da06 7465  index_select..te
-000002a0: 6e73 6f72 da02 746f da06 6465 7669 6365  nsor..to..device
-000002b0: 2902 7205 0000 00da 0178 2901 da08 6368  ).r......x)...ch
-000002c0: 616e 6e65 6c73 7204 0000 0072 0700 0000  annelsr....r....
-000002d0: 7208 0000 0009 0000 0073 0400 0000 0600  r........s......
-000002e0: 0200 2902 da05 7261 6e67 65da 0573 6861  ..)...range..sha
-000002f0: 7065 2902 7203 0000 00da 0278 7372 0400  pe).r......xsr..
-00000300: 0000 2902 7212 0000 0072 0300 0000 7207  ..).r....r....r.
-00000310: 0000 00da 0e5f 7461 6b65 5f63 6861 6e6e  ....._take_chann
-00000320: 656c 7304 0000 0073 0a00 0000 0001 0801  els....s........
-00000330: 0402 2001 1201 7216 0000 0063 0200 0000  .. ...r....c....
-00000340: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00000350: 4300 0000 7320 0000 007c 0164 006b 0972  C...s ...|.d.k.r
-00000360: 187c 007c 016b 04a0 007c 006a 01a1 0153  .|.|.k...|.j...S
-00000370: 007c 0053 0064 0053 0029 014e 2902 da04  .|.S.d.S.).N)...
-00000380: 7479 7065 da05 6474 7970 6529 0272 1100  type..dtype).r..
-00000390: 0000 da09 7468 7265 7368 6f6c 6472 0400  ....thresholdr..
-000003a0: 0000 7204 0000 0072 0700 0000 da0a 5f74  ..r....r......_t
-000003b0: 6872 6573 686f 6c64 0d00 0000 7306 0000  hreshold....s...
-000003c0: 0000 0108 0110 0272 1a00 0000 e748 afbc  .......r.....H..
-000003d0: 9af2 d77a 3e63 0500 0000 0000 0000 0000  ...z>c..........
-000003e0: 0000 0700 0000 0500 0000 4300 0000 7354  ..........C...sT
-000003f0: 0000 0074 007c 007c 0364 018d 027d 0074  ...t.|.|.d...}.t
-00000400: 017c 007c 017c 0464 028d 035c 027d 007d  .|.|.|.d...\.}.}
-00000410: 0174 02a0 037c 017c 0014 00a1 017d 0574  .t...|.|.....}.t
-00000420: 02a0 037c 01a1 0174 02a0 037c 00a1 0117  ...|...t...|....
-00000430: 007c 0518 007c 0217 007d 067c 057c 0217  .|...|...}.|.|..
-00000440: 007c 061b 0053 0029 0361 4a01 0000 4361  .|...S.).aJ...Ca
-00000450: 6c63 756c 6174 6520 496e 7465 7273 6563  lculate Intersec
-00000460: 7469 6f6e 206f 7665 7220 556e 696f 6e20  tion over Union 
-00000470: 6265 7477 6565 6e20 6772 6f75 6e64 2074  between ground t
-00000480: 7275 7468 2061 6e64 2070 7265 6469 6374  ruth and predict
-00000490: 696f 6e0a 2020 2020 4172 6773 3a0a 2020  ion.    Args:.  
-000004a0: 2020 2020 2020 7072 2028 746f 7263 682e        pr (torch.
-000004b0: 5465 6e73 6f72 293a 2070 7265 6469 6374  Tensor): predict
-000004c0: 6564 2074 656e 736f 720a 2020 2020 2020  ed tensor.      
-000004d0: 2020 6774 2028 746f 7263 682e 5465 6e73    gt (torch.Tens
-000004e0: 6f72 293a 2020 6772 6f75 6e64 2074 7275  or):  ground tru
-000004f0: 7468 2074 656e 736f 720a 2020 2020 2020  th tensor.      
-00000500: 2020 6570 7320 2866 6c6f 6174 293a 2065    eps (float): e
-00000510: 7073 696c 6f6e 2074 6f20 6176 6f69 6420  psilon to avoid 
-00000520: 7a65 726f 2064 6976 6973 696f 6e0a 2020  zero division.  
-00000530: 2020 2020 2020 7468 7265 7368 6f6c 643a        threshold:
-00000540: 2074 6872 6573 686f 6c64 2066 6f72 206f   threshold for o
-00000550: 7574 7075 7473 2062 696e 6172 697a 6174  utputs binarizat
-00000560: 696f 6e0a 2020 2020 5265 7475 726e 733a  ion.    Returns:
-00000570: 0a20 2020 2020 2020 2066 6c6f 6174 3a20  .        float: 
-00000580: 496f 5520 284a 6163 6361 7264 2920 7363  IoU (Jaccard) sc
-00000590: 6f72 650a 2020 2020 a901 7219 0000 0072  ore.    ..r....r
-000005a0: 0200 0000 a904 721a 0000 0072 1600 0000  ......r....r....
-000005b0: 720c 0000 00da 0373 756d 2907 da02 7072  r......sum)...pr
-000005c0: da02 6774 da03 6570 7372 1900 0000 7203  ..gt..epsr....r.
-000005d0: 0000 00da 0c69 6e74 6572 7365 6374 696f  .....intersectio
-000005e0: 6eda 0575 6e69 6f6e 7204 0000 0072 0400  n..unionr....r..
-000005f0: 0000 7207 0000 00da 0369 6f75 1400 0000  ..r......iou....
-00000600: 730a 0000 0000 0b0c 0112 020e 011c 0172  s..............r
-00000610: 2400 0000 e733 3333 3333 33d3 3fe7 6666  $....333333.?.ff
-00000620: 6666 6666 e63f 6307 0000 0000 0000 0000  ffff.?c.........
-00000630: 0000 000b 0000 0005 0000 0043 0000 0073  ...........C...s
-00000640: 6c00 0000 7400 7c00 7c05 6401 8d02 7d00  l...t.|.|.d...}.
-00000650: 7401 7c00 7c01 7c06 6402 8d03 5c02 7d00  t.|.|.|.d...\.}.
-00000660: 7d01 7402 a003 7c01 7c00 1400 a101 7d07  }.t...|.|.....}.
-00000670: 7402 a003 7c00 a101 7c07 1800 7d08 7402  t...|...|...}.t.
-00000680: a003 7c01 a101 7c07 1800 7d09 7c07 7c04  ..|...|...}.|.|.
-00000690: 1700 7c07 7c02 7c08 1400 1700 7c03 7c09  ..|.|.|.....|.|.
-000006a0: 1400 1700 7c04 1700 1b00 7d0a 7c0a 5300  ....|.....}.|.S.
-000006b0: 2903 7a3b 4361 6c63 7574 6174 6520 5476  ).z;Calcutate Tv
-000006c0: 6572 736b 7920 7363 6f72 6520 6265 7477  ersky score betw
-000006d0: 6565 6e20 6772 6f75 6e64 2074 7275 7468  een ground truth
-000006e0: 2061 6e64 2070 7265 6469 6374 696f 6e72   and predictionr
-000006f0: 1c00 0000 7202 0000 0072 1d00 0000 290b  ....r....r....).
-00000700: 721f 0000 0072 2000 0000 da05 616c 7068  r....r .....alph
-00000710: 61da 0462 6574 6172 2100 0000 7219 0000  a..betar!...r...
-00000720: 0072 0300 0000 da02 7470 da02 6670 da02  .r......tp..fp..
-00000730: 666e da05 7363 6f72 6572 0400 0000 7204  fn..scorer....r.
-00000740: 0000 0072 0700 0000 da0d 7476 6572 736b  ...r......tversk
-00000750: 795f 7363 6f72 6529 0000 0073 0e00 0000  y_score)...s....
-00000760: 0003 0c01 1202 0e01 0e01 0e02 2002 722d  ............ .r-
-00000770: 0000 0072 0900 0000 6306 0000 0000 0000  ...r....c.......
-00000780: 0000 0000 000a 0000 0005 0000 0043 0000  .............C..
-00000790: 0073 8400 0000 7400 7c00 7c04 6401 8d02  .s....t.|.|.d...
-000007a0: 7d00 7401 7c00 7c01 7c05 6402 8d03 5c02  }.t.|.|.|.d...\.
-000007b0: 7d00 7d01 7402 a003 7c01 7c00 1400 a101  }.}.t...|.|.....
-000007c0: 7d06 7402 a003 7c00 a101 7c06 1800 7d07  }.t...|...|...}.
-000007d0: 7402 a003 7c01 a101 7c06 1800 7d08 6403  t...|...|...}.d.
-000007e0: 7c02 6404 1300 1700 7c06 1400 7c03 1700  |.d.....|...|...
-000007f0: 6403 7c02 6404 1300 1700 7c06 1400 7c02  d.|.d.....|...|.
-00000800: 6404 1300 7c08 1400 1700 7c07 1700 7c03  d...|.....|...|.
-00000810: 1700 1b00 7d09 7c09 5300 2905 6156 0100  ....}.|.S.).aV..
-00000820: 0043 616c 6375 6c61 7465 2046 2d73 636f  .Calculate F-sco
-00000830: 7265 2062 6574 7765 656e 2067 726f 756e  re between groun
-00000840: 6420 7472 7574 6820 616e 6420 7072 6564  d truth and pred
-00000850: 6963 7469 6f6e 0a20 2020 2041 7267 733a  iction.    Args:
-00000860: 0a20 2020 2020 2020 2070 7220 2874 6f72  .        pr (tor
-00000870: 6368 2e54 656e 736f 7229 3a20 7072 6564  ch.Tensor): pred
-00000880: 6963 7465 6420 7465 6e73 6f72 0a20 2020  icted tensor.   
-00000890: 2020 2020 2067 7420 2874 6f72 6368 2e54       gt (torch.T
-000008a0: 656e 736f 7229 3a20 2067 726f 756e 6420  ensor):  ground 
-000008b0: 7472 7574 6820 7465 6e73 6f72 0a20 2020  truth tensor.   
-000008c0: 2020 2020 2062 6574 6120 2866 6c6f 6174       beta (float
-000008d0: 293a 2070 6f73 6974 6976 6520 636f 6e73  ): positive cons
-000008e0: 7461 6e74 0a20 2020 2020 2020 2065 7073  tant.        eps
-000008f0: 2028 666c 6f61 7429 3a20 6570 7369 6c6f   (float): epsilo
-00000900: 6e20 746f 2061 766f 6964 207a 6572 6f20  n to avoid zero 
-00000910: 6469 7669 7369 6f6e 0a20 2020 2020 2020  division.       
-00000920: 2074 6872 6573 686f 6c64 3a20 7468 7265   threshold: thre
-00000930: 7368 6f6c 6420 666f 7220 6f75 7470 7574  shold for output
-00000940: 7320 6269 6e61 7269 7a61 7469 6f6e 0a20  s binarization. 
-00000950: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00000960: 2020 2020 666c 6f61 743a 2046 2073 636f      float: F sco
-00000970: 7265 0a20 2020 2072 1c00 0000 7202 0000  re.    r....r...
-00000980: 0072 0900 0000 e902 0000 0072 1d00 0000  .r.........r....
-00000990: 290a 721f 0000 0072 2000 0000 7228 0000  ).r....r ...r(..
-000009a0: 0072 2100 0000 7219 0000 0072 0300 0000  .r!...r....r....
-000009b0: 7229 0000 0072 2a00 0000 722b 0000 0072  r)...r*...r+...r
-000009c0: 2c00 0000 7204 0000 0072 0400 0000 7207  ,...r....r....r.
-000009d0: 0000 00da 0766 5f73 636f 7265 3900 0000  .....f_score9...
-000009e0: 7312 0000 0000 0c0c 0112 020e 010e 010e  s...............
-000009f0: 0212 0122 ff04 0372 2f00 0000 e700 0000  ..."...r/.......
-00000a00: 0000 00e0 3f63 0400 0000 0000 0000 0000  ....?c..........
-00000a10: 0000 0600 0000 0500 0000 4300 0000 734a  ..........C...sJ
-00000a20: 0000 0074 007c 007c 0264 018d 027d 0074  ...t.|.|.d...}.t
-00000a30: 017c 007c 017c 0364 028d 035c 027d 007d  .|.|.|.d...\.}.}
-00000a40: 0174 026a 037c 017c 006b 027c 006a 0464  .t.j.|.|.k.|.j.d
-00000a50: 038d 027d 047c 047c 01a0 0564 04a1 016a  ...}.|.|...d...j
-00000a60: 0664 0519 001b 007d 057c 0553 0029 0661  .d.....}.|.S.).a
-00000a70: 3d01 0000 4361 6c63 756c 6174 6520 6163  =...Calculate ac
-00000a80: 6375 7261 6379 2073 636f 7265 2062 6574  curacy score bet
-00000a90: 7765 656e 2067 726f 756e 6420 7472 7574  ween ground trut
-00000aa0: 6820 616e 6420 7072 6564 6963 7469 6f6e  h and prediction
-00000ab0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-00000ac0: 2020 2070 7220 2874 6f72 6368 2e54 656e     pr (torch.Ten
-00000ad0: 736f 7229 3a20 7072 6564 6963 7465 6420  sor): predicted 
-00000ae0: 7465 6e73 6f72 0a20 2020 2020 2020 2067  tensor.        g
-00000af0: 7420 2874 6f72 6368 2e54 656e 736f 7229  t (torch.Tensor)
-00000b00: 3a20 2067 726f 756e 6420 7472 7574 6820  :  ground truth 
-00000b10: 7465 6e73 6f72 0a20 2020 2020 2020 2065  tensor.        e
-00000b20: 7073 2028 666c 6f61 7429 3a20 6570 7369  ps (float): epsi
-00000b30: 6c6f 6e20 746f 2061 766f 6964 207a 6572  lon to avoid zer
-00000b40: 6f20 6469 7669 7369 6f6e 0a20 2020 2020  o division.     
-00000b50: 2020 2074 6872 6573 686f 6c64 3a20 7468     threshold: th
-00000b60: 7265 7368 6f6c 6420 666f 7220 6f75 7470  reshold for outp
-00000b70: 7574 7320 6269 6e61 7269 7a61 7469 6f6e  uts binarization
-00000b80: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
-00000b90: 2020 2020 2020 666c 6f61 743a 2070 7265        float: pre
-00000ba0: 6369 7369 6f6e 2073 636f 7265 0a20 2020  cision score.   
-00000bb0: 2072 1c00 0000 7202 0000 0029 0172 1800   r....r....).r..
-00000bc0: 0000 e9ff ffff ff72 0100 0000 2907 721a  .......r....).r.
-00000bd0: 0000 0072 1600 0000 720c 0000 0072 1e00  ...r....r....r..
-00000be0: 0000 7218 0000 00da 0476 6965 7772 1400  ..r......viewr..
-00000bf0: 0000 2906 721f 0000 0072 2000 0000 7219  ..).r....r ...r.
-00000c00: 0000 0072 0300 0000 7229 0000 0072 2c00  ...r....r)...r,.
-00000c10: 0000 7204 0000 0072 0400 0000 7207 0000  ..r....r....r...
-00000c20: 00da 0861 6363 7572 6163 7952 0000 0073  ...accuracyR...s
-00000c30: 0a00 0000 000a 0c01 1202 1401 1401 7233  ..............r3
-00000c40: 0000 0063 0500 0000 0000 0000 0000 0000  ...c............
-00000c50: 0800 0000 0500 0000 4300 0000 7352 0000  ........C...sR..
-00000c60: 0074 007c 007c 0364 018d 027d 0074 017c  .t.|.|.d...}.t.|
-00000c70: 007c 017c 0464 028d 035c 027d 007d 0174  .|.|.d...\.}.}.t
-00000c80: 02a0 037c 017c 0014 00a1 017d 0574 02a0  ...|.|.....}.t..
-00000c90: 037c 00a1 017c 0518 007d 067c 057c 0217  .|...|...}.|.|..
-00000ca0: 007c 057c 0617 007c 0217 001b 007d 077c  .|.|...|.....}.|
-00000cb0: 0753 0029 0361 3e01 0000 4361 6c63 756c  .S.).a>...Calcul
-00000cc0: 6174 6520 7072 6563 6973 696f 6e20 7363  ate precision sc
-00000cd0: 6f72 6520 6265 7477 6565 6e20 6772 6f75  ore between grou
-00000ce0: 6e64 2074 7275 7468 2061 6e64 2070 7265  nd truth and pre
-00000cf0: 6469 6374 696f 6e0a 2020 2020 4172 6773  diction.    Args
-00000d00: 3a0a 2020 2020 2020 2020 7072 2028 746f  :.        pr (to
-00000d10: 7263 682e 5465 6e73 6f72 293a 2070 7265  rch.Tensor): pre
-00000d20: 6469 6374 6564 2074 656e 736f 720a 2020  dicted tensor.  
-00000d30: 2020 2020 2020 6774 2028 746f 7263 682e        gt (torch.
-00000d40: 5465 6e73 6f72 293a 2020 6772 6f75 6e64  Tensor):  ground
-00000d50: 2074 7275 7468 2074 656e 736f 720a 2020   truth tensor.  
-00000d60: 2020 2020 2020 6570 7320 2866 6c6f 6174        eps (float
-00000d70: 293a 2065 7073 696c 6f6e 2074 6f20 6176  ): epsilon to av
-00000d80: 6f69 6420 7a65 726f 2064 6976 6973 696f  oid zero divisio
-00000d90: 6e0a 2020 2020 2020 2020 7468 7265 7368  n.        thresh
-00000da0: 6f6c 643a 2074 6872 6573 686f 6c64 2066  old: threshold f
-00000db0: 6f72 206f 7574 7075 7473 2062 696e 6172  or outputs binar
-00000dc0: 697a 6174 696f 6e0a 2020 2020 5265 7475  ization.    Retu
-00000dd0: 726e 733a 0a20 2020 2020 2020 2066 6c6f  rns:.        flo
-00000de0: 6174 3a20 7072 6563 6973 696f 6e20 7363  at: precision sc
-00000df0: 6f72 650a 2020 2020 721c 0000 0072 0200  ore.    r....r..
-00000e00: 0000 721d 0000 0029 0872 1f00 0000 7220  ..r....).r....r 
-00000e10: 0000 0072 2100 0000 7219 0000 0072 0300  ...r!...r....r..
-00000e20: 0000 7229 0000 0072 2a00 0000 722c 0000  ..r)...r*...r,..
-00000e30: 0072 0400 0000 7204 0000 0072 0700 0000  .r....r....r....
-00000e40: da09 7072 6563 6973 696f 6e64 0000 0073  ..precisiond...s
-00000e50: 0c00 0000 000b 0c01 1202 0e01 0e02 1402  ................
-00000e60: 7234 0000 0063 0500 0000 0000 0000 0000  r4...c..........
-00000e70: 0000 0800 0000 0500 0000 4300 0000 7352  ..........C...sR
-00000e80: 0000 0074 007c 007c 0364 018d 027d 0074  ...t.|.|.d...}.t
-00000e90: 017c 007c 017c 0464 028d 035c 027d 007d  .|.|.|.d...\.}.}
-00000ea0: 0174 02a0 037c 017c 0014 00a1 017d 0574  .t...|.|.....}.t
-00000eb0: 02a0 037c 01a1 017c 0518 007d 067c 057c  ...|...|...}.|.|
-00000ec0: 0217 007c 057c 0617 007c 0217 001b 007d  ...|.|...|.....}
-00000ed0: 077c 0753 00a9 0361 5601 0000 4361 6c63  .|.S...aV...Calc
-00000ee0: 756c 6174 6520 5265 6361 6c6c 2062 6574  ulate Recall bet
-00000ef0: 7765 656e 2067 726f 756e 6420 7472 7574  ween ground trut
-00000f00: 6820 616e 6420 7072 6564 6963 7469 6f6e  h and prediction
-00000f10: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-00000f20: 2020 2070 7220 2874 6f72 6368 2e54 656e     pr (torch.Ten
-00000f30: 736f 7229 3a20 4120 6c69 7374 206f 6620  sor): A list of 
-00000f40: 7072 6564 6963 7465 6420 656c 656d 656e  predicted elemen
-00000f50: 7473 0a20 2020 2020 2020 2067 7420 2874  ts.        gt (t
-00000f60: 6f72 6368 2e54 656e 736f 7229 3a20 2041  orch.Tensor):  A
-00000f70: 206c 6973 7420 6f66 2065 6c65 6d65 6e74   list of element
-00000f80: 7320 7468 6174 2061 7265 2074 6f20 6265  s that are to be
-00000f90: 2070 7265 6469 6374 6564 0a20 2020 2020   predicted.     
-00000fa0: 2020 2065 7073 2028 666c 6f61 7429 3a20     eps (float): 
-00000fb0: 6570 7369 6c6f 6e20 746f 2061 766f 6964  epsilon to avoid
-00000fc0: 207a 6572 6f20 6469 7669 7369 6f6e 0a20   zero division. 
-00000fd0: 2020 2020 2020 2074 6872 6573 686f 6c64         threshold
-00000fe0: 3a20 7468 7265 7368 6f6c 6420 666f 7220  : threshold for 
-00000ff0: 6f75 7470 7574 7320 6269 6e61 7269 7a61  outputs binariza
-00001000: 7469 6f6e 0a20 2020 2052 6574 7572 6e73  tion.    Returns
-00001010: 3a0a 2020 2020 2020 2020 666c 6f61 743a  :.        float:
-00001020: 2072 6563 616c 6c20 7363 6f72 650a 2020   recall score.  
-00001030: 2020 721c 0000 0072 0200 0000 721d 0000    r....r....r...
-00001040: 0029 0872 1f00 0000 7220 0000 0072 2100  .).r....r ...r!.
-00001050: 0000 7219 0000 0072 0300 0000 7229 0000  ..r....r....r)..
-00001060: 0072 2b00 0000 722c 0000 0072 0400 0000  .r+...r,...r....
-00001070: 7204 0000 0072 0700 0000 da06 7265 6361  r....r......reca
-00001080: 6c6c 7a00 0000 730c 0000 0000 0b0c 0112  llz...s.........
-00001090: 020e 010e 0214 0272 3600 0000 6304 0000  .......r6...c...
-000010a0: 0000 0000 0000 0000 0004 0000 0005 0000  ................
-000010b0: 0043 0000 0073 2a00 0000 7400 7c00 7c02  .C...s*...t.|.|.
-000010c0: 6401 8d02 7d00 7401 7c00 7c01 7c03 6402  d...}.t.|.|.|.d.
-000010d0: 8d03 5c02 7d00 7d01 7402 a003 7c01 7c00  ..\.}.}.t...|.|.
-000010e0: a102 5300 7235 0000 0029 0472 1a00 0000  ..S.r5...).r....
-000010f0: 7216 0000 00da 0246 32da 2062 696e 6172  r......F2. binar
-00001100: 795f 6372 6f73 735f 656e 7472 6f70 795f  y_cross_entropy_
-00001110: 7769 7468 5f6c 6f67 6974 7329 0472 1f00  with_logits).r..
-00001120: 0000 7220 0000 0072 1900 0000 7203 0000  ..r ...r....r...
-00001130: 0072 0400 0000 7204 0000 0072 0700 0000  .r....r....r....
-00001140: 7238 0000 0090 0000 0073 0600 0000 000b  r8.......s......
-00001150: 0c01 1202 7238 0000 0029 014e 2903 721b  ....r8...).N).r.
-00001160: 0000 004e 4e29 0572 2500 0000 7226 0000  ...NN).r%...r&..
-00001170: 0072 1b00 0000 4e4e 2904 7209 0000 0072  .r....NN).r....r
-00001180: 1b00 0000 4e4e 2902 7230 0000 004e 2903  ....NN).r0...N).
-00001190: 721b 0000 004e 4e29 0372 1b00 0000 4e4e  r....NN).r....NN
-000011a0: 2902 4e4e 290f 720c 0000 005a 1374 6f72  ).NN).r....Z.tor
-000011b0: 6368 2e6e 6e2e 6675 6e63 7469 6f6e 616c  ch.nn.functional
-000011c0: da02 6e6e da0a 6675 6e63 7469 6f6e 616c  ..nn..functional
-000011d0: 7237 0000 0072 1600 0000 721a 0000 0072  r7...r....r....r
-000011e0: 2400 0000 da07 6a61 6363 6172 6472 2d00  $.....jaccardr-.
-000011f0: 0000 722f 0000 0072 3300 0000 7234 0000  ..r/...r3...r4..
-00001200: 0072 3600 0000 7238 0000 0072 0400 0000  .r6...r8...r....
-00001210: 7204 0000 0072 0400 0000 7207 0000 00da  r....r....r.....
-00001220: 083c 6d6f 6475 6c65 3e01 0000 0073 1600  .<module>....s..
-00001230: 0000 0801 1202 0e09 0a07 0a13 0402 0a10  ................
-00001240: 0a19 0a12 0a16 0a16                      ........
+000001a0: 735c 4861 6e61 6e5c 6d67 5c73 6567 6d65  s\Hanan\mg\segme
+000001b0: 6e74 6174 696f 6e5f 6d6f 6465 6c73 5c75  ntation_models\u
+000001c0: 7469 6c73 5c66 756e 6374 696f 6e61 6c2e  tils\functional.
+000001d0: 7079 da0a 3c6c 6973 7463 6f6d 703e 0800  py..<listcomp>..
+000001e0: 0000 7306 0000 0006 0002 0008 007a 225f  ..s..........z"_
+000001f0: 7461 6b65 5f63 6861 6e6e 656c 732e 3c6c  take_channels.<l
+00000200: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00000210: 3e72 0100 0000 e901 0000 0063 0100 0000  >r.........c....
+00000220: 0000 0000 0000 0000 0200 0000 0800 0000  ................
+00000230: 1300 0000 732a 0000 0067 007c 005d 227d  ....s*...g.|.]"}
+00000240: 0174 006a 017c 0164 0074 00a0 0288 00a1  .t.j.|.d.t......
+00000250: 01a0 037c 016a 04a1 0164 018d 0391 0271  ...|.j...d.....q
+00000260: 0453 0029 0272 0900 0000 2902 da03 6469  .S.).r....)...di
+00000270: 6dda 0569 6e64 6578 2905 da05 746f 7263  m..index)...torc
+00000280: 68da 0c69 6e64 6578 5f73 656c 6563 74da  h..index_select.
+00000290: 0674 656e 736f 72da 0274 6fda 0664 6576  .tensor..to..dev
+000002a0: 6963 6529 0272 0500 0000 da01 7829 01da  ice).r......x)..
+000002b0: 0863 6861 6e6e 656c 7372 0400 0000 7207  .channelsr....r.
+000002c0: 0000 0072 0800 0000 0900 0000 7304 0000  ...r........s...
+000002d0: 0006 0002 0029 02da 0572 616e 6765 da05  .....)...range..
+000002e0: 7368 6170 6529 0272 0300 0000 da02 7873  shape).r......xs
+000002f0: 7204 0000 0029 0272 1200 0000 7203 0000  r....).r....r...
+00000300: 0072 0700 0000 da0e 5f74 616b 655f 6368  .r......_take_ch
+00000310: 616e 6e65 6c73 0400 0000 730a 0000 0000  annels....s.....
+00000320: 0108 0104 0220 0112 0172 1600 0000 6302  ..... ...r....c.
+00000330: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00000340: 0000 0043 0000 0073 2000 0000 7c01 6400  ...C...s ...|.d.
+00000350: 6b09 7218 7c00 7c01 6b04 a000 7c00 6a01  k.r.|.|.k...|.j.
+00000360: a101 5300 7c00 5300 6400 5300 2901 4e29  ..S.|.S.d.S.).N)
+00000370: 02da 0474 7970 65da 0564 7479 7065 2902  ...type..dtype).
+00000380: 7211 0000 00da 0974 6872 6573 686f 6c64  r......threshold
+00000390: 7204 0000 0072 0400 0000 7207 0000 00da  r....r....r.....
+000003a0: 0a5f 7468 7265 7368 6f6c 640d 0000 0073  ._threshold....s
+000003b0: 0600 0000 0001 0801 1002 721a 0000 00e7  ..........r.....
+000003c0: 48af bc9a f2d7 7a3e 6305 0000 0000 0000  H.....z>c.......
+000003d0: 0000 0000 0007 0000 0005 0000 0043 0000  .............C..
+000003e0: 0073 5400 0000 7400 7c00 7c03 6401 8d02  .sT...t.|.|.d...
+000003f0: 7d00 7401 7c00 7c01 7c04 6402 8d03 5c02  }.t.|.|.|.d...\.
+00000400: 7d00 7d01 7402 a003 7c01 7c00 1400 a101  }.}.t...|.|.....
+00000410: 7d05 7402 a003 7c01 a101 7402 a003 7c00  }.t...|...t...|.
+00000420: a101 1700 7c05 1800 7c02 1700 7d06 7c05  ....|...|...}.|.
+00000430: 7c02 1700 7c06 1b00 5300 2903 614a 0100  |...|...S.).aJ..
+00000440: 0043 616c 6375 6c61 7465 2049 6e74 6572  .Calculate Inter
+00000450: 7365 6374 696f 6e20 6f76 6572 2055 6e69  section over Uni
+00000460: 6f6e 2062 6574 7765 656e 2067 726f 756e  on between groun
+00000470: 6420 7472 7574 6820 616e 6420 7072 6564  d truth and pred
+00000480: 6963 7469 6f6e 0a20 2020 2041 7267 733a  iction.    Args:
+00000490: 0a20 2020 2020 2020 2070 7220 2874 6f72  .        pr (tor
+000004a0: 6368 2e54 656e 736f 7229 3a20 7072 6564  ch.Tensor): pred
+000004b0: 6963 7465 6420 7465 6e73 6f72 0a20 2020  icted tensor.   
+000004c0: 2020 2020 2067 7420 2874 6f72 6368 2e54       gt (torch.T
+000004d0: 656e 736f 7229 3a20 2067 726f 756e 6420  ensor):  ground 
+000004e0: 7472 7574 6820 7465 6e73 6f72 0a20 2020  truth tensor.   
+000004f0: 2020 2020 2065 7073 2028 666c 6f61 7429       eps (float)
+00000500: 3a20 6570 7369 6c6f 6e20 746f 2061 766f  : epsilon to avo
+00000510: 6964 207a 6572 6f20 6469 7669 7369 6f6e  id zero division
+00000520: 0a20 2020 2020 2020 2074 6872 6573 686f  .        thresho
+00000530: 6c64 3a20 7468 7265 7368 6f6c 6420 666f  ld: threshold fo
+00000540: 7220 6f75 7470 7574 7320 6269 6e61 7269  r outputs binari
+00000550: 7a61 7469 6f6e 0a20 2020 2052 6574 7572  zation.    Retur
+00000560: 6e73 3a0a 2020 2020 2020 2020 666c 6f61  ns:.        floa
+00000570: 743a 2049 6f55 2028 4a61 6363 6172 6429  t: IoU (Jaccard)
+00000580: 2073 636f 7265 0a20 2020 20a9 0172 1900   score.    ..r..
+00000590: 0000 7202 0000 00a9 0472 1a00 0000 7216  ..r......r....r.
+000005a0: 0000 0072 0c00 0000 da03 7375 6d29 07da  ...r......sum)..
+000005b0: 0270 72da 0267 74da 0365 7073 7219 0000  .pr..gt..epsr...
+000005c0: 0072 0300 0000 da0c 696e 7465 7273 6563  .r......intersec
+000005d0: 7469 6f6e da05 756e 696f 6e72 0400 0000  tion..unionr....
+000005e0: 7204 0000 0072 0700 0000 da03 696f 7514  r....r......iou.
+000005f0: 0000 0073 0a00 0000 000b 0c01 1202 0e01  ...s............
+00000600: 1c01 7224 0000 00e7 3333 3333 3333 d33f  ..r$....333333.?
+00000610: e766 6666 6666 66e6 3f63 0700 0000 0000  .ffffff.?c......
+00000620: 0000 0000 0000 0b00 0000 0500 0000 4300  ..............C.
+00000630: 0000 736c 0000 0074 007c 007c 0564 018d  ..sl...t.|.|.d..
+00000640: 027d 0074 017c 007c 017c 0664 028d 035c  .}.t.|.|.|.d...\
+00000650: 027d 007d 0174 02a0 037c 017c 0014 00a1  .}.}.t...|.|....
+00000660: 017d 0774 02a0 037c 00a1 017c 0718 007d  .}.t...|...|...}
+00000670: 0874 02a0 037c 01a1 017c 0718 007d 097c  .t...|...|...}.|
+00000680: 077c 0417 007c 077c 027c 0814 0017 007c  .|...|.|.|.....|
+00000690: 037c 0914 0017 007c 0417 001b 007d 0a7c  .|.....|.....}.|
+000006a0: 0a53 0029 037a 3b43 616c 6375 7461 7465  .S.).z;Calcutate
+000006b0: 2054 7665 7273 6b79 2073 636f 7265 2062   Tversky score b
+000006c0: 6574 7765 656e 2067 726f 756e 6420 7472  etween ground tr
+000006d0: 7574 6820 616e 6420 7072 6564 6963 7469  uth and predicti
+000006e0: 6f6e 721c 0000 0072 0200 0000 721d 0000  onr....r....r...
+000006f0: 0029 0b72 1f00 0000 7220 0000 00da 0561  .).r....r .....a
+00000700: 6c70 6861 da04 6265 7461 7221 0000 0072  lpha..betar!...r
+00000710: 1900 0000 7203 0000 00da 0274 70da 0266  ....r......tp..f
+00000720: 70da 0266 6eda 0573 636f 7265 7204 0000  p..fn..scorer...
+00000730: 0072 0400 0000 7207 0000 00da 0d74 7665  .r....r......tve
+00000740: 7273 6b79 5f73 636f 7265 2900 0000 730e  rsky_score)...s.
+00000750: 0000 0000 030c 0112 020e 010e 010e 0220  ............... 
+00000760: 0272 2d00 0000 7209 0000 0063 0600 0000  .r-...r....c....
+00000770: 0000 0000 0000 0000 0a00 0000 0500 0000  ................
+00000780: 4300 0000 7384 0000 0074 007c 007c 0464  C...s....t.|.|.d
+00000790: 018d 027d 0074 017c 007c 017c 0564 028d  ...}.t.|.|.|.d..
+000007a0: 035c 027d 007d 0174 02a0 037c 017c 0014  .\.}.}.t...|.|..
+000007b0: 00a1 017d 0674 02a0 037c 00a1 017c 0618  ...}.t...|...|..
+000007c0: 007d 0774 02a0 037c 01a1 017c 0618 007d  .}.t...|...|...}
+000007d0: 0864 037c 0264 0413 0017 007c 0614 007c  .d.|.d.....|...|
+000007e0: 0317 0064 037c 0264 0413 0017 007c 0614  ...d.|.d.....|..
+000007f0: 007c 0264 0413 007c 0814 0017 007c 0717  .|.d...|.....|..
+00000800: 007c 0317 001b 007d 097c 0953 0029 0561  .|.....}.|.S.).a
+00000810: 5601 0000 4361 6c63 756c 6174 6520 462d  V...Calculate F-
+00000820: 7363 6f72 6520 6265 7477 6565 6e20 6772  score between gr
+00000830: 6f75 6e64 2074 7275 7468 2061 6e64 2070  ound truth and p
+00000840: 7265 6469 6374 696f 6e0a 2020 2020 4172  rediction.    Ar
+00000850: 6773 3a0a 2020 2020 2020 2020 7072 2028  gs:.        pr (
+00000860: 746f 7263 682e 5465 6e73 6f72 293a 2070  torch.Tensor): p
+00000870: 7265 6469 6374 6564 2074 656e 736f 720a  redicted tensor.
+00000880: 2020 2020 2020 2020 6774 2028 746f 7263          gt (torc
+00000890: 682e 5465 6e73 6f72 293a 2020 6772 6f75  h.Tensor):  grou
+000008a0: 6e64 2074 7275 7468 2074 656e 736f 720a  nd truth tensor.
+000008b0: 2020 2020 2020 2020 6265 7461 2028 666c          beta (fl
+000008c0: 6f61 7429 3a20 706f 7369 7469 7665 2063  oat): positive c
+000008d0: 6f6e 7374 616e 740a 2020 2020 2020 2020  onstant.        
+000008e0: 6570 7320 2866 6c6f 6174 293a 2065 7073  eps (float): eps
+000008f0: 696c 6f6e 2074 6f20 6176 6f69 6420 7a65  ilon to avoid ze
+00000900: 726f 2064 6976 6973 696f 6e0a 2020 2020  ro division.    
+00000910: 2020 2020 7468 7265 7368 6f6c 643a 2074      threshold: t
+00000920: 6872 6573 686f 6c64 2066 6f72 206f 7574  hreshold for out
+00000930: 7075 7473 2062 696e 6172 697a 6174 696f  puts binarizatio
+00000940: 6e0a 2020 2020 5265 7475 726e 733a 0a20  n.    Returns:. 
+00000950: 2020 2020 2020 2066 6c6f 6174 3a20 4620         float: F 
+00000960: 7363 6f72 650a 2020 2020 721c 0000 0072  score.    r....r
+00000970: 0200 0000 7209 0000 00e9 0200 0000 721d  ....r.........r.
+00000980: 0000 0029 0a72 1f00 0000 7220 0000 0072  ...).r....r ...r
+00000990: 2800 0000 7221 0000 0072 1900 0000 7203  (...r!...r....r.
+000009a0: 0000 0072 2900 0000 722a 0000 0072 2b00  ...r)...r*...r+.
+000009b0: 0000 722c 0000 0072 0400 0000 7204 0000  ..r,...r....r...
+000009c0: 0072 0700 0000 da07 665f 7363 6f72 6539  .r......f_score9
+000009d0: 0000 0073 1200 0000 000c 0c01 1202 0e01  ...s............
+000009e0: 0e01 0e02 1201 22ff 0403 722f 0000 00e7  ......"...r/....
+000009f0: 0000 0000 0000 e03f 6304 0000 0000 0000  .......?c.......
+00000a00: 0000 0000 0006 0000 0005 0000 0043 0000  .............C..
+00000a10: 0073 4a00 0000 7400 7c00 7c02 6401 8d02  .sJ...t.|.|.d...
+00000a20: 7d00 7401 7c00 7c01 7c03 6402 8d03 5c02  }.t.|.|.|.d...\.
+00000a30: 7d00 7d01 7402 6a03 7c01 7c00 6b02 7c00  }.}.t.j.|.|.k.|.
+00000a40: 6a04 6403 8d02 7d04 7c04 7c01 a005 6404  j.d...}.|.|...d.
+00000a50: a101 6a06 6405 1900 1b00 7d05 7c05 5300  ..j.d.....}.|.S.
+00000a60: 2906 613d 0100 0043 616c 6375 6c61 7465  ).a=...Calculate
+00000a70: 2061 6363 7572 6163 7920 7363 6f72 6520   accuracy score 
+00000a80: 6265 7477 6565 6e20 6772 6f75 6e64 2074  between ground t
+00000a90: 7275 7468 2061 6e64 2070 7265 6469 6374  ruth and predict
+00000aa0: 696f 6e0a 2020 2020 4172 6773 3a0a 2020  ion.    Args:.  
+00000ab0: 2020 2020 2020 7072 2028 746f 7263 682e        pr (torch.
+00000ac0: 5465 6e73 6f72 293a 2070 7265 6469 6374  Tensor): predict
+00000ad0: 6564 2074 656e 736f 720a 2020 2020 2020  ed tensor.      
+00000ae0: 2020 6774 2028 746f 7263 682e 5465 6e73    gt (torch.Tens
+00000af0: 6f72 293a 2020 6772 6f75 6e64 2074 7275  or):  ground tru
+00000b00: 7468 2074 656e 736f 720a 2020 2020 2020  th tensor.      
+00000b10: 2020 6570 7320 2866 6c6f 6174 293a 2065    eps (float): e
+00000b20: 7073 696c 6f6e 2074 6f20 6176 6f69 6420  psilon to avoid 
+00000b30: 7a65 726f 2064 6976 6973 696f 6e0a 2020  zero division.  
+00000b40: 2020 2020 2020 7468 7265 7368 6f6c 643a        threshold:
+00000b50: 2074 6872 6573 686f 6c64 2066 6f72 206f   threshold for o
+00000b60: 7574 7075 7473 2062 696e 6172 697a 6174  utputs binarizat
+00000b70: 696f 6e0a 2020 2020 5265 7475 726e 733a  ion.    Returns:
+00000b80: 0a20 2020 2020 2020 2066 6c6f 6174 3a20  .        float: 
+00000b90: 7072 6563 6973 696f 6e20 7363 6f72 650a  precision score.
+00000ba0: 2020 2020 721c 0000 0072 0200 0000 2901      r....r....).
+00000bb0: 7218 0000 00e9 ffff ffff 7201 0000 0029  r.........r....)
+00000bc0: 0772 1a00 0000 7216 0000 0072 0c00 0000  .r....r....r....
+00000bd0: 721e 0000 0072 1800 0000 da04 7669 6577  r....r......view
+00000be0: 7214 0000 0029 0672 1f00 0000 7220 0000  r....).r....r ..
+00000bf0: 0072 1900 0000 7203 0000 0072 2900 0000  .r....r....r)...
+00000c00: 722c 0000 0072 0400 0000 7204 0000 0072  r,...r....r....r
+00000c10: 0700 0000 da08 6163 6375 7261 6379 5200  ......accuracyR.
+00000c20: 0000 730a 0000 0000 0a0c 0112 0214 0114  ..s.............
+00000c30: 0172 3300 0000 6305 0000 0000 0000 0000  .r3...c.........
+00000c40: 0000 0008 0000 0005 0000 0043 0000 0073  ...........C...s
+00000c50: 5200 0000 7400 7c00 7c03 6401 8d02 7d00  R...t.|.|.d...}.
+00000c60: 7401 7c00 7c01 7c04 6402 8d03 5c02 7d00  t.|.|.|.d...\.}.
+00000c70: 7d01 7402 a003 7c01 7c00 1400 a101 7d05  }.t...|.|.....}.
+00000c80: 7402 a003 7c00 a101 7c05 1800 7d06 7c05  t...|...|...}.|.
+00000c90: 7c02 1700 7c05 7c06 1700 7c02 1700 1b00  |...|.|...|.....
+00000ca0: 7d07 7c07 5300 2903 613e 0100 0043 616c  }.|.S.).a>...Cal
+00000cb0: 6375 6c61 7465 2070 7265 6369 7369 6f6e  culate precision
+00000cc0: 2073 636f 7265 2062 6574 7765 656e 2067   score between g
+00000cd0: 726f 756e 6420 7472 7574 6820 616e 6420  round truth and 
+00000ce0: 7072 6564 6963 7469 6f6e 0a20 2020 2041  prediction.    A
+00000cf0: 7267 733a 0a20 2020 2020 2020 2070 7220  rgs:.        pr 
+00000d00: 2874 6f72 6368 2e54 656e 736f 7229 3a20  (torch.Tensor): 
+00000d10: 7072 6564 6963 7465 6420 7465 6e73 6f72  predicted tensor
+00000d20: 0a20 2020 2020 2020 2067 7420 2874 6f72  .        gt (tor
+00000d30: 6368 2e54 656e 736f 7229 3a20 2067 726f  ch.Tensor):  gro
+00000d40: 756e 6420 7472 7574 6820 7465 6e73 6f72  und truth tensor
+00000d50: 0a20 2020 2020 2020 2065 7073 2028 666c  .        eps (fl
+00000d60: 6f61 7429 3a20 6570 7369 6c6f 6e20 746f  oat): epsilon to
+00000d70: 2061 766f 6964 207a 6572 6f20 6469 7669   avoid zero divi
+00000d80: 7369 6f6e 0a20 2020 2020 2020 2074 6872  sion.        thr
+00000d90: 6573 686f 6c64 3a20 7468 7265 7368 6f6c  eshold: threshol
+00000da0: 6420 666f 7220 6f75 7470 7574 7320 6269  d for outputs bi
+00000db0: 6e61 7269 7a61 7469 6f6e 0a20 2020 2052  narization.    R
+00000dc0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00000dd0: 666c 6f61 743a 2070 7265 6369 7369 6f6e  float: precision
+00000de0: 2073 636f 7265 0a20 2020 2072 1c00 0000   score.    r....
+00000df0: 7202 0000 0072 1d00 0000 2908 721f 0000  r....r....).r...
+00000e00: 0072 2000 0000 7221 0000 0072 1900 0000  .r ...r!...r....
+00000e10: 7203 0000 0072 2900 0000 722a 0000 0072  r....r)...r*...r
+00000e20: 2c00 0000 7204 0000 0072 0400 0000 7207  ,...r....r....r.
+00000e30: 0000 00da 0970 7265 6369 7369 6f6e 6400  .....precisiond.
+00000e40: 0000 730c 0000 0000 0b0c 0112 020e 010e  ..s.............
+00000e50: 0214 0272 3400 0000 6305 0000 0000 0000  ...r4...c.......
+00000e60: 0000 0000 0008 0000 0005 0000 0043 0000  .............C..
+00000e70: 0073 5200 0000 7400 7c00 7c03 6401 8d02  .sR...t.|.|.d...
+00000e80: 7d00 7401 7c00 7c01 7c04 6402 8d03 5c02  }.t.|.|.|.d...\.
+00000e90: 7d00 7d01 7402 a003 7c01 7c00 1400 a101  }.}.t...|.|.....
+00000ea0: 7d05 7402 a003 7c01 a101 7c05 1800 7d06  }.t...|...|...}.
+00000eb0: 7c05 7c02 1700 7c05 7c06 1700 7c02 1700  |.|...|.|...|...
+00000ec0: 1b00 7d07 7c07 5300 a903 6156 0100 0043  ..}.|.S...aV...C
+00000ed0: 616c 6375 6c61 7465 2052 6563 616c 6c20  alculate Recall 
+00000ee0: 6265 7477 6565 6e20 6772 6f75 6e64 2074  between ground t
+00000ef0: 7275 7468 2061 6e64 2070 7265 6469 6374  ruth and predict
+00000f00: 696f 6e0a 2020 2020 4172 6773 3a0a 2020  ion.    Args:.  
+00000f10: 2020 2020 2020 7072 2028 746f 7263 682e        pr (torch.
+00000f20: 5465 6e73 6f72 293a 2041 206c 6973 7420  Tensor): A list 
+00000f30: 6f66 2070 7265 6469 6374 6564 2065 6c65  of predicted ele
+00000f40: 6d65 6e74 730a 2020 2020 2020 2020 6774  ments.        gt
+00000f50: 2028 746f 7263 682e 5465 6e73 6f72 293a   (torch.Tensor):
+00000f60: 2020 4120 6c69 7374 206f 6620 656c 656d    A list of elem
+00000f70: 656e 7473 2074 6861 7420 6172 6520 746f  ents that are to
+00000f80: 2062 6520 7072 6564 6963 7465 640a 2020   be predicted.  
+00000f90: 2020 2020 2020 6570 7320 2866 6c6f 6174        eps (float
+00000fa0: 293a 2065 7073 696c 6f6e 2074 6f20 6176  ): epsilon to av
+00000fb0: 6f69 6420 7a65 726f 2064 6976 6973 696f  oid zero divisio
+00000fc0: 6e0a 2020 2020 2020 2020 7468 7265 7368  n.        thresh
+00000fd0: 6f6c 643a 2074 6872 6573 686f 6c64 2066  old: threshold f
+00000fe0: 6f72 206f 7574 7075 7473 2062 696e 6172  or outputs binar
+00000ff0: 697a 6174 696f 6e0a 2020 2020 5265 7475  ization.    Retu
+00001000: 726e 733a 0a20 2020 2020 2020 2066 6c6f  rns:.        flo
+00001010: 6174 3a20 7265 6361 6c6c 2073 636f 7265  at: recall score
+00001020: 0a20 2020 2072 1c00 0000 7202 0000 0072  .    r....r....r
+00001030: 1d00 0000 2908 721f 0000 0072 2000 0000  ....).r....r ...
+00001040: 7221 0000 0072 1900 0000 7203 0000 0072  r!...r....r....r
+00001050: 2900 0000 722b 0000 0072 2c00 0000 7204  )...r+...r,...r.
+00001060: 0000 0072 0400 0000 7207 0000 00da 0672  ...r....r......r
+00001070: 6563 616c 6c7a 0000 0073 0c00 0000 000b  ecallz...s......
+00001080: 0c01 1202 0e01 0e02 1402 7236 0000 0063  ..........r6...c
+00001090: 0400 0000 0000 0000 0000 0000 0400 0000  ................
+000010a0: 0500 0000 4300 0000 732a 0000 0074 007c  ....C...s*...t.|
+000010b0: 007c 0264 018d 027d 0074 017c 007c 017c  .|.d...}.t.|.|.|
+000010c0: 0364 028d 035c 027d 007d 0174 02a0 037c  .d...\.}.}.t...|
+000010d0: 017c 00a1 0253 0072 3500 0000 2904 721a  .|...S.r5...).r.
+000010e0: 0000 0072 1600 0000 da02 4632 da20 6269  ...r......F2. bi
+000010f0: 6e61 7279 5f63 726f 7373 5f65 6e74 726f  nary_cross_entro
+00001100: 7079 5f77 6974 685f 6c6f 6769 7473 2904  py_with_logits).
+00001110: 721f 0000 0072 2000 0000 7219 0000 0072  r....r ...r....r
+00001120: 0300 0000 7204 0000 0072 0400 0000 7207  ....r....r....r.
+00001130: 0000 0072 3800 0000 9000 0000 7306 0000  ...r8.......s...
+00001140: 0000 0b0c 0112 0272 3800 0000 2901 4e29  .......r8...).N)
+00001150: 0372 1b00 0000 4e4e 2905 7225 0000 0072  .r....NN).r%...r
+00001160: 2600 0000 721b 0000 004e 4e29 0472 0900  &...r....NN).r..
+00001170: 0000 721b 0000 004e 4e29 0272 3000 0000  ..r....NN).r0...
+00001180: 4e29 0372 1b00 0000 4e4e 2903 721b 0000  N).r....NN).r...
+00001190: 004e 4e29 024e 4e29 0f72 0c00 0000 5a13  .NN).NN).r....Z.
+000011a0: 746f 7263 682e 6e6e 2e66 756e 6374 696f  torch.nn.functio
+000011b0: 6e61 6cda 026e 6eda 0a66 756e 6374 696f  nal..nn..functio
+000011c0: 6e61 6c72 3700 0000 7216 0000 0072 1a00  nalr7...r....r..
+000011d0: 0000 7224 0000 00da 076a 6163 6361 7264  ..r$.....jaccard
+000011e0: 722d 0000 0072 2f00 0000 7233 0000 0072  r-...r/...r3...r
+000011f0: 3400 0000 7236 0000 0072 3800 0000 7204  4...r6...r8...r.
+00001200: 0000 0072 0400 0000 7204 0000 0072 0700  ...r....r....r..
+00001210: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00001220: 7316 0000 0008 0112 020e 090a 070a 1304  s...............
+00001230: 020a 100a 190a 120a 160a 16              ...........
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/functional.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/functional.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/losses.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/losses.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/losses.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/losses.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/losses.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/losses.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/losses.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/losses.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:22 2023 UTC, .py size: 3475 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -33,231 +33,230 @@
 00000200: 7c03 7c00 5f05 6400 5300 a901 4e29 06da  |.|._.d.S...N)..
 00000210: 0573 7570 6572 da08 5f5f 696e 6974 5f5f  .super..__init__
 00000220: da03 6570 7372 0500 0000 da0a 6163 7469  ..epsr......acti
 00000230: 7661 7469 6f6e da0f 6967 6e6f 7265 5f63  vation..ignore_c
 00000240: 6861 6e6e 656c 7329 05da 0473 656c 6672  hannels)...selfr
 00000250: 0b00 0000 720c 0000 0072 0d00 0000 da06  ....r....r......
 00000260: 6b77 6172 6773 a901 da09 5f5f 636c 6173  kwargs....__clas
-00000270: 735f 5fa9 00fa 5343 3a5c 5573 6572 735c  s__...SC:\Users\
+00000270: 735f 5fa9 00fa 4663 3a5c 5573 6572 735c  s__...Fc:\Users\
 00000280: 6d68 616e 616e 5c44 6f77 6e6c 6f61 6473  mhanan\Downloads
-00000290: 5c48 616e 616e 5c4d 616d 6d6f 5079 5c6d  \Hanan\MammoPy\m
-000002a0: 616d 6d6f 7079 5c73 6567 6d65 6e74 6174  ammopy\segmentat
-000002b0: 696f 6e5f 6d6f 6465 6c73 5c75 7469 6c73  ion_models\utils
-000002c0: 5c6c 6f73 7365 732e 7079 720a 0000 000a  \losses.pyr.....
-000002d0: 0000 0073 0800 0000 0001 0e01 0601 0a01  ...s............
-000002e0: 7a14 4a61 6363 6172 644c 6f73 732e 5f5f  z.JaccardLoss.__
-000002f0: 696e 6974 5f5f 6303 0000 0000 0000 0000  init__c.........
-00000300: 0000 0003 0000 0008 0000 0043 0000 0073  ...........C...s
-00000310: 2600 0000 7c00 a000 7c01 a101 7d01 6401  &...|...|...}.d.
-00000320: 7401 6a02 7c01 7c02 7c00 6a03 6400 7c00  t.j.|.|.|.j.d.|.
-00000330: 6a04 6402 8d05 1800 5300 2903 4e72 0200  j.d.....S.).Nr..
-00000340: 0000 2903 720b 0000 00da 0974 6872 6573  ..).r......thres
-00000350: 686f 6c64 720d 0000 0029 0572 0c00 0000  holdr....).r....
-00000360: da01 46da 076a 6163 6361 7264 720b 0000  ..F..jaccardr...
-00000370: 0072 0d00 0000 a903 720e 0000 00da 0479  .r......r......y
-00000380: 5f70 72da 0479 5f67 7472 1200 0000 7212  _pr..y_gtr....r.
-00000390: 0000 0072 1300 0000 da07 666f 7277 6172  ...r......forwar
-000003a0: 6410 0000 0073 1000 0000 0001 0a01 0601  d....s..........
-000003b0: 0200 0201 0401 0201 04fc 7a13 4a61 6363  ..........z.Jacc
-000003c0: 6172 644c 6f73 732e 666f 7277 6172 6429  ardLoss.forward)
-000003d0: 0372 0700 0000 4e4e a906 da08 5f5f 6e61  .r....NN....__na
-000003e0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-000003f0: da0c 5f5f 7175 616c 6e61 6d65 5f5f 720a  ..__qualname__r.
-00000400: 0000 0072 1a00 0000 da0d 5f5f 636c 6173  ...r......__clas
-00000410: 7363 656c 6c5f 5f72 1200 0000 7212 0000  scell__r....r...
-00000420: 0072 1000 0000 7213 0000 0072 0600 0000  .r....r....r....
-00000430: 0800 0000 7304 0000 0008 020e 0672 0600  ....s........r..
-00000440: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000450: 0000 0004 0000 0000 0000 0073 2600 0000  ...........s&...
-00000460: 6500 5a01 6400 5a02 6407 8700 6601 6403  e.Z.d.Z.d...f.d.
-00000470: 6404 8409 5a03 6405 6406 8400 5a04 8700  d...Z.d.d...Z...
-00000480: 0400 5a05 5300 2908 da08 4469 6365 4c6f  ..Z.S.)...DiceLo
-00000490: 7373 7207 0000 004e 6305 0000 0000 0000  ssr....Nc.......
-000004a0: 0000 0000 0006 0000 0003 0000 000b 0000  ................
-000004b0: 0073 2e00 0000 7400 8300 6a01 6600 7c05  .s....t...j.f.|.
-000004c0: 8e01 0100 7c01 7c00 5f02 7c02 7c00 5f03  ....|.|._.|.|._.
-000004d0: 7404 7c03 8301 7c00 5f05 7c04 7c00 5f06  t.|...|._.|.|._.
-000004e0: 6400 5300 7208 0000 0029 0772 0900 0000  d.S.r....).r....
-000004f0: 720a 0000 0072 0b00 0000 da04 6265 7461  r....r......beta
-00000500: 7205 0000 0072 0c00 0000 720d 0000 0029  r....r....r....)
-00000510: 0672 0e00 0000 720b 0000 0072 2100 0000  .r....r....r!...
-00000520: 720c 0000 0072 0d00 0000 720f 0000 0072  r....r....r....r
-00000530: 1000 0000 7212 0000 0072 1300 0000 720a  ....r....r....r.
-00000540: 0000 001c 0000 0073 0a00 0000 0001 0e01  .......s........
-00000550: 0601 0601 0a01 7a11 4469 6365 4c6f 7373  ......z.DiceLoss
-00000560: 2e5f 5f69 6e69 745f 5f63 0300 0000 0000  .__init__c......
-00000570: 0000 0000 0000 0300 0000 0900 0000 4300  ..............C.
-00000580: 0000 732a 0000 007c 00a0 007c 01a1 017d  ..s*...|...|...}
-00000590: 0164 0174 016a 027c 017c 027c 006a 037c  .d.t.j.|.|.|.j.|
-000005a0: 006a 0464 007c 006a 0564 028d 0618 0053  .j.d.|.j.d.....S
-000005b0: 0029 034e 7202 0000 0029 0472 2100 0000  .).Nr....).r!...
-000005c0: 720b 0000 0072 1400 0000 720d 0000 0029  r....r....r....)
-000005d0: 0672 0c00 0000 7215 0000 005a 0766 5f73  .r....r....Z.f_s
-000005e0: 636f 7265 7221 0000 0072 0b00 0000 720d  corer!...r....r.
-000005f0: 0000 0072 1700 0000 7212 0000 0072 1200  ...r....r....r..
-00000600: 0000 7213 0000 0072 1a00 0000 2300 0000  ..r....r....#...
-00000610: 7312 0000 0000 010a 0106 0102 0002 0104  s...............
-00000620: 0104 0102 0104 fb7a 1044 6963 654c 6f73  .......z.DiceLos
-00000630: 732e 666f 7277 6172 6429 0472 0700 0000  s.forward).r....
-00000640: 7207 0000 004e 4e72 1b00 0000 7212 0000  r....NNr....r...
-00000650: 0072 1200 0000 7210 0000 0072 1300 0000  .r....r....r....
-00000660: 7220 0000 001a 0000 0073 0400 0000 0802  r .......s......
-00000670: 0e07 7220 0000 0063 0000 0000 0000 0000  ..r ...c........
-00000680: 0000 0000 0000 0000 0500 0000 0000 0000  ................
-00000690: 7326 0000 0065 005a 0164 005a 0264 0987  s&...e.Z.d.Z.d..
-000006a0: 0066 0164 0564 0684 095a 0364 0764 0884  .f.d.d...Z.d.d..
-000006b0: 005a 0487 0004 005a 0553 0029 0ada 0b54  .Z.....Z.S.)...T
-000006c0: 7665 7273 6b79 4c6f 7373 e733 3333 3333  verskyLoss.33333
-000006d0: 33d3 3f72 0700 0000 e766 6666 6666 66e6  3.?r.....ffffff.
-000006e0: 3f4e 6306 0000 0000 0000 0000 0000 0007  ?Nc.............
-000006f0: 0000 0003 0000 000b 0000 0073 3400 0000  ...........s4...
-00000700: 7400 8300 6a01 6600 7c06 8e01 0100 7c02  t...j.f.|.....|.
-00000710: 7c00 5f02 7c01 7c00 5f03 7c03 7c00 5f04  |._.|.|._.|.|._.
-00000720: 7405 7c04 8301 7c00 5f06 7c05 7c00 5f07  t.|...|._.|.|._.
-00000730: 6400 5300 7208 0000 0029 0872 0900 0000  d.S.r....).r....
-00000740: 720a 0000 0072 0b00 0000 da05 616c 7068  r....r......alph
-00000750: 6172 2100 0000 7205 0000 0072 0c00 0000  ar!...r....r....
-00000760: 720d 0000 0029 0772 0e00 0000 7225 0000  r....).r....r%..
-00000770: 0072 0b00 0000 7221 0000 0072 0c00 0000  .r....r!...r....
-00000780: 720d 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-00000790: 1200 0000 7213 0000 0072 0a00 0000 2f00  ....r....r..../.
-000007a0: 0000 730c 0000 0000 010e 0106 0106 0106  ..s.............
-000007b0: 010a 017a 1454 7665 7273 6b79 4c6f 7373  ...z.TverskyLoss
-000007c0: 2e5f 5f69 6e69 745f 5f63 0300 0000 0000  .__init__c......
-000007d0: 0000 0000 0000 0300 0000 0a00 0000 4300  ..............C.
-000007e0: 0000 732e 0000 007c 00a0 007c 01a1 017d  ..s....|...|...}
-000007f0: 0164 0174 016a 027c 017c 027c 006a 037c  .d.t.j.|.|.|.j.|
-00000800: 006a 047c 006a 0564 007c 006a 0664 028d  .j.|.j.d.|.j.d..
-00000810: 0718 0053 00a9 034e 7202 0000 0029 0572  ...S...Nr....).r
-00000820: 2500 0000 7221 0000 0072 0b00 0000 7214  %...r!...r....r.
-00000830: 0000 0072 0d00 0000 2907 720c 0000 0072  ...r....).r....r
-00000840: 1500 0000 da0d 7476 6572 736b 795f 7363  ......tversky_sc
-00000850: 6f72 6572 2500 0000 7221 0000 0072 0b00  orer%...r!...r..
-00000860: 0000 720d 0000 0072 1700 0000 7212 0000  ..r....r....r...
-00000870: 0072 1200 0000 7213 0000 0072 1a00 0000  .r....r....r....
-00000880: 3700 0000 7314 0000 0000 010a 0106 0102  7...s...........
-00000890: 0002 0104 0104 0104 0102 0104 fa7a 1354  .............z.T
-000008a0: 7665 7273 6b79 4c6f 7373 2e66 6f72 7761  verskyLoss.forwa
-000008b0: 7264 2905 7223 0000 0072 0700 0000 7224  rd).r#...r....r$
-000008c0: 0000 004e 4e72 1b00 0000 7212 0000 0072  ...NNr....r....r
-000008d0: 1200 0000 7210 0000 0072 1300 0000 7222  ....r....r....r"
-000008e0: 0000 002d 0000 0073 0400 0000 0802 0e08  ...-...s........
-000008f0: 7222 0000 0063 0000 0000 0000 0000 0000  r"...c..........
-00000900: 0000 0000 0000 0600 0000 0000 0000 7326  ..............s&
-00000910: 0000 0065 005a 0164 005a 0264 0a87 0066  ...e.Z.d.Z.d...f
-00000920: 0164 0664 0784 095a 0364 0864 0984 005a  .d.d...Z.d.d...Z
-00000930: 0487 0004 005a 0553 0029 0bda 1046 6f63  .....Z.S.)...Foc
-00000940: 616c 5476 6572 736b 794c 6f73 7372 2300  alTverskyLossr#.
-00000950: 0000 7207 0000 0072 2400 0000 e700 0000  ..r....r$.......
-00000960: 0000 00e8 3f4e 6307 0000 0000 0000 0000  ....?Nc.........
-00000970: 0000 0008 0000 0003 0000 000b 0000 0073  ...............s
-00000980: 3a00 0000 7400 8300 6a01 6600 7c07 8e01  :...t...j.f.|...
-00000990: 0100 7c02 7c00 5f02 7c01 7c00 5f03 7c03  ..|.|._.|.|._.|.
-000009a0: 7c00 5f04 7c04 7c00 5f05 7406 7c05 8301  |._.|.|._.t.|...
-000009b0: 7c00 5f07 7c06 7c00 5f08 6400 5300 7208  |._.|.|._.d.S.r.
-000009c0: 0000 0029 0972 0900 0000 720a 0000 0072  ...).r....r....r
-000009d0: 0b00 0000 7225 0000 0072 2100 0000 da05  ....r%...r!.....
-000009e0: 6761 6d6d 6172 0500 0000 720c 0000 0072  gammar....r....r
-000009f0: 0d00 0000 2908 720e 0000 0072 2500 0000  ....).r....r%...
-00000a00: 720b 0000 0072 2100 0000 722a 0000 0072  r....r!...r*...r
-00000a10: 0c00 0000 720d 0000 0072 0f00 0000 7210  ....r....r....r.
-00000a20: 0000 0072 1200 0000 7213 0000 0072 0a00  ...r....r....r..
-00000a30: 0000 4400 0000 730e 0000 0000 010e 0106  ..D...s.........
-00000a40: 0106 0106 0106 010a 017a 1946 6f63 616c  .........z.Focal
-00000a50: 5476 6572 736b 794c 6f73 732e 5f5f 696e  TverskyLoss.__in
-00000a60: 6974 5f5f 6303 0000 0000 0000 0000 0000  it__c...........
-00000a70: 0004 0000 000a 0000 0043 0000 0073 3c00  .........C...s<.
-00000a80: 0000 7c00 a000 7c01 a101 7d01 6401 7401  ..|...|...}.d.t.
-00000a90: 6a02 7c01 7c02 7c00 6a03 7c00 6a04 7c00  j.|.|.|.j.|.j.|.
-00000aa0: 6a05 6400 7c00 6a06 6402 8d07 1800 7d03  j.d.|.j.d.....}.
-00000ab0: 7407 a008 7c03 7c00 6a09 a102 5300 7226  t...|.|.j...S.r&
-00000ac0: 0000 0029 0a72 0c00 0000 7215 0000 0072  ...).r....r....r
-00000ad0: 2700 0000 7225 0000 0072 2100 0000 720b  '...r%...r!...r.
-00000ae0: 0000 0072 0d00 0000 da05 746f 7263 68da  ...r......torch.
-00000af0: 0370 6f77 722a 0000 0029 0472 0e00 0000  .powr*...).r....
-00000b00: 7218 0000 0072 1900 0000 5a0c 7476 6572  r....r....Z.tver
-00000b10: 736b 795f 6c6f 7373 7212 0000 0072 1200  sky_lossr....r..
-00000b20: 0000 7213 0000 0072 1a00 0000 4d00 0000  ..r....r....M...
-00000b30: 7316 0000 0000 010a 0106 0102 0002 0104  s...............
-00000b40: 0104 0104 0102 0104 fa08 097a 1846 6f63  ...........z.Foc
-00000b50: 616c 5476 6572 736b 794c 6f73 732e 666f  alTverskyLoss.fo
-00000b60: 7277 6172 6429 0672 2300 0000 7207 0000  rward).r#...r...
-00000b70: 0072 2400 0000 7229 0000 004e 4e72 1b00  .r$...r)...NNr..
-00000b80: 0000 7212 0000 0072 1200 0000 7210 0000  ..r....r....r...
-00000b90: 0072 1300 0000 7228 0000 0042 0000 0073  .r....r(...B...s
-00000ba0: 0400 0000 0802 0e09 7228 0000 0063 0000  ........r(...c..
-00000bb0: 0000 0000 0000 0000 0000 0000 0000 0100  ................
-00000bc0: 0000 4000 0000 730c 0000 0065 005a 0164  ..@...s....e.Z.d
-00000bd0: 005a 0264 0153 0029 02da 064c 314c 6f73  .Z.d.S.)...L1Los
-00000be0: 734e a903 721c 0000 0072 1d00 0000 721e  sN..r....r....r.
-00000bf0: 0000 0072 1200 0000 7212 0000 0072 1200  ...r....r....r..
-00000c00: 0000 7213 0000 0072 2d00 0000 5b00 0000  ..r....r-...[...
-00000c10: 7302 0000 0008 0172 2d00 0000 6300 0000  s......r-...c...
-00000c20: 0000 0000 0000 0000 0000 0000 0001 0000  ................
-00000c30: 0040 0000 0073 0c00 0000 6500 5a01 6400  .@...s....e.Z.d.
-00000c40: 5a02 6401 5300 2902 da07 4d53 454c 6f73  Z.d.S.)...MSELos
-00000c50: 734e 722e 0000 0072 1200 0000 7212 0000  sNr....r....r...
-00000c60: 0072 1200 0000 7213 0000 0072 2f00 0000  .r....r....r/...
-00000c70: 5f00 0000 7302 0000 0008 0172 2f00 0000  _...s......r/...
-00000c80: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000c90: 0001 0000 0040 0000 0073 0c00 0000 6500  .....@...s....e.
-00000ca0: 5a01 6400 5a02 6401 5300 2902 da10 4372  Z.d.Z.d.S.)...Cr
-00000cb0: 6f73 7345 6e74 726f 7079 4c6f 7373 4e72  ossEntropyLossNr
-00000cc0: 2e00 0000 7212 0000 0072 1200 0000 7212  ....r....r....r.
-00000cd0: 0000 0072 1300 0000 7230 0000 0063 0000  ...r....r0...c..
-00000ce0: 0073 0200 0000 0801 7230 0000 0063 0000  .s......r0...c..
-00000cf0: 0000 0000 0000 0000 0000 0000 0000 0100  ................
-00000d00: 0000 4000 0000 730c 0000 0065 005a 0164  ..@...s....e.Z.d
-00000d10: 005a 0264 0153 0029 02da 074e 4c4c 4c6f  .Z.d.S.)...NLLLo
-00000d20: 7373 4e72 2e00 0000 7212 0000 0072 1200  ssNr....r....r..
-00000d30: 0000 7212 0000 0072 1300 0000 7231 0000  ..r....r....r1..
-00000d40: 0067 0000 0073 0200 0000 0801 7231 0000  .g...s......r1..
-00000d50: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000d60: 0000 0100 0000 4000 0000 730c 0000 0065  ......@...s....e
-00000d70: 005a 0164 005a 0264 0153 0029 02da 0742  .Z.d.Z.d.S.)...B
-00000d80: 4345 4c6f 7373 4e72 2e00 0000 7212 0000  CELossNr....r...
-00000d90: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
-00000da0: 7232 0000 006b 0000 0073 0200 0000 0801  r2...k...s......
-00000db0: 7232 0000 0063 0000 0000 0000 0000 0000  r2...c..........
-00000dc0: 0000 0000 0000 0400 0000 0000 0000 7326  ..............s&
-00000dd0: 0000 0065 005a 0164 005a 0264 0687 0066  ...e.Z.d.Z.d...f
-00000de0: 0164 0264 0384 095a 0364 0464 0584 005a  .d.d...Z.d.d...Z
-00000df0: 0487 0004 005a 0553 0029 07da 1142 4345  .....Z.S.)...BCE
-00000e00: 5769 7468 4c6f 6769 7473 4c6f 7373 4e63  WithLogitsLossNc
-00000e10: 0300 0000 0000 0000 0000 0000 0400 0000  ................
-00000e20: 0300 0000 0b00 0000 7322 0000 0074 0083  ........s"...t..
-00000e30: 006a 0166 007c 038e 0101 0074 027c 0183  .j.f.|.....t.|..
-00000e40: 017c 005f 037c 027c 005f 0464 0053 0072  .|._.|.|._.d.S.r
-00000e50: 0800 0000 2905 7209 0000 0072 0a00 0000  ....).r....r....
-00000e60: 7205 0000 0072 0c00 0000 720d 0000 0029  r....r....r....)
-00000e70: 0472 0e00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-00000e80: 720f 0000 0072 1000 0000 7212 0000 0072  r....r....r....r
-00000e90: 1300 0000 720a 0000 0070 0000 0073 0600  ....r....p...s..
-00000ea0: 0000 0001 0e02 0a01 7a1a 4243 4557 6974  ........z.BCEWit
-00000eb0: 684c 6f67 6974 734c 6f73 732e 5f5f 696e  hLogitsLoss.__in
-00000ec0: 6974 5f5f 6303 0000 0000 0000 0000 0000  it__c...........
-00000ed0: 0003 0000 0006 0000 0043 0000 0073 1e00  .........C...s..
-00000ee0: 0000 7c00 a000 7c01 a101 7d01 7401 6a02  ..|...|...}.t.j.
-00000ef0: 7c01 7c02 6400 7c00 6a03 6401 8d04 5300  |.|.d.|.j.d...S.
-00000f00: 2902 4e29 0272 1400 0000 720d 0000 0029  ).N).r....r....)
-00000f10: 0472 0c00 0000 7215 0000 00da 2062 696e  .r....r..... bin
-00000f20: 6172 795f 6372 6f73 735f 656e 7472 6f70  ary_cross_entrop
-00000f30: 795f 7769 7468 5f6c 6f67 6974 7372 0d00  y_with_logitsr..
-00000f40: 0000 7217 0000 0072 1200 0000 7212 0000  ..r....r....r...
-00000f50: 0072 1300 0000 721a 0000 0076 0000 0073  .r....r....v...s
-00000f60: 0e00 0000 0001 0a01 0401 0200 0201 0201  ................
-00000f70: 04fd 7a19 4243 4557 6974 684c 6f67 6974  ..z.BCEWithLogit
-00000f80: 734c 6f73 732e 666f 7277 6172 6429 024e  sLoss.forward).N
-00000f90: 4e72 1b00 0000 7212 0000 0072 1200 0000  Nr....r....r....
-00000fa0: 7210 0000 0072 1300 0000 7233 0000 006f  r....r....r3...o
-00000fb0: 0000 0073 0400 0000 0801 0e06 7233 0000  ...s........r3..
-00000fc0: 0029 13da 0874 6f72 6368 2e6e 6eda 026e  .)...torch.nn..n
-00000fd0: 6e72 2b00 0000 da00 7203 0000 0072 0400  nr+.....r....r..
-00000fe0: 0000 7215 0000 0072 0500 0000 5a04 4c6f  ..r....r....Z.Lo
-00000ff0: 7373 7206 0000 0072 2000 0000 7222 0000  ssr....r ...r"..
-00001000: 0072 2800 0000 722d 0000 0072 2f00 0000  .r(...r-...r/...
-00001010: 7230 0000 0072 3100 0000 7232 0000 0072  r0...r1...r2...r
-00001020: 3300 0000 7212 0000 0072 1200 0000 7212  3...r....r....r.
-00001030: 0000 0072 1300 0000 da08 3c6d 6f64 756c  ...r......<modul
-00001040: 653e 0100 0000 731c 0000 000c 0108 010c  e>....s.........
-00001050: 010c 010c 0312 1212 1312 1512 1916 0416  ................
-00001060: 0416 0416 0416 04                        .......
+00000290: 5c48 616e 616e 5c6d 675c 7365 676d 656e  \Hanan\mg\segmen
+000002a0: 7461 7469 6f6e 5f6d 6f64 656c 735c 7574  tation_models\ut
+000002b0: 696c 735c 6c6f 7373 6573 2e70 7972 0a00  ils\losses.pyr..
+000002c0: 0000 0a00 0000 7308 0000 0000 010e 0106  ......s.........
+000002d0: 010a 017a 144a 6163 6361 7264 4c6f 7373  ...z.JaccardLoss
+000002e0: 2e5f 5f69 6e69 745f 5f63 0300 0000 0000  .__init__c......
+000002f0: 0000 0000 0000 0300 0000 0800 0000 4300  ..............C.
+00000300: 0000 7326 0000 007c 00a0 007c 01a1 017d  ..s&...|...|...}
+00000310: 0164 0174 016a 027c 017c 027c 006a 0364  .d.t.j.|.|.|.j.d
+00000320: 007c 006a 0464 028d 0518 0053 0029 034e  .|.j.d.....S.).N
+00000330: 7202 0000 0029 0372 0b00 0000 da09 7468  r....).r......th
+00000340: 7265 7368 6f6c 6472 0d00 0000 2905 720c  resholdr....).r.
+00000350: 0000 00da 0146 da07 6a61 6363 6172 6472  .....F..jaccardr
+00000360: 0b00 0000 720d 0000 00a9 0372 0e00 0000  ....r......r....
+00000370: da04 795f 7072 da04 795f 6774 7212 0000  ..y_pr..y_gtr...
+00000380: 0072 1200 0000 7213 0000 00da 0766 6f72  .r....r......for
+00000390: 7761 7264 1000 0000 7310 0000 0000 010a  ward....s.......
+000003a0: 0106 0102 0002 0104 0102 0104 fc7a 134a  .............z.J
+000003b0: 6163 6361 7264 4c6f 7373 2e66 6f72 7761  accardLoss.forwa
+000003c0: 7264 2903 7207 0000 004e 4ea9 06da 085f  rd).r....NN...._
+000003d0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+000003e0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+000003f0: 5f72 0a00 0000 721a 0000 00da 0d5f 5f63  _r....r......__c
+00000400: 6c61 7373 6365 6c6c 5f5f 7212 0000 0072  lasscell__r....r
+00000410: 1200 0000 7210 0000 0072 1300 0000 7206  ....r....r....r.
+00000420: 0000 0008 0000 0073 0400 0000 0802 0e06  .......s........
+00000430: 7206 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00000440: 0000 0000 0000 0400 0000 0000 0000 7326  ..............s&
+00000450: 0000 0065 005a 0164 005a 0264 0787 0066  ...e.Z.d.Z.d...f
+00000460: 0164 0364 0484 095a 0364 0564 0684 005a  .d.d...Z.d.d...Z
+00000470: 0487 0004 005a 0553 0029 08da 0844 6963  .....Z.S.)...Dic
+00000480: 654c 6f73 7372 0700 0000 4e63 0500 0000  eLossr....Nc....
+00000490: 0000 0000 0000 0000 0600 0000 0300 0000  ................
+000004a0: 0b00 0000 732e 0000 0074 0083 006a 0166  ....s....t...j.f
+000004b0: 007c 058e 0101 007c 017c 005f 027c 027c  .|.....|.|._.|.|
+000004c0: 005f 0374 047c 0383 017c 005f 057c 047c  ._.t.|...|._.|.|
+000004d0: 005f 0664 0053 0072 0800 0000 2907 7209  ._.d.S.r....).r.
+000004e0: 0000 0072 0a00 0000 720b 0000 00da 0462  ...r....r......b
+000004f0: 6574 6172 0500 0000 720c 0000 0072 0d00  etar....r....r..
+00000500: 0000 2906 720e 0000 0072 0b00 0000 7221  ..).r....r....r!
+00000510: 0000 0072 0c00 0000 720d 0000 0072 0f00  ...r....r....r..
+00000520: 0000 7210 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00000530: 0072 0a00 0000 1c00 0000 730a 0000 0000  .r........s.....
+00000540: 010e 0106 0106 010a 017a 1144 6963 654c  .........z.DiceL
+00000550: 6f73 732e 5f5f 696e 6974 5f5f 6303 0000  oss.__init__c...
+00000560: 0000 0000 0000 0000 0003 0000 0009 0000  ................
+00000570: 0043 0000 0073 2a00 0000 7c00 a000 7c01  .C...s*...|...|.
+00000580: a101 7d01 6401 7401 6a02 7c01 7c02 7c00  ..}.d.t.j.|.|.|.
+00000590: 6a03 7c00 6a04 6400 7c00 6a05 6402 8d06  j.|.j.d.|.j.d...
+000005a0: 1800 5300 2903 4e72 0200 0000 2904 7221  ..S.).Nr....).r!
+000005b0: 0000 0072 0b00 0000 7214 0000 0072 0d00  ...r....r....r..
+000005c0: 0000 2906 720c 0000 0072 1500 0000 5a07  ..).r....r....Z.
+000005d0: 665f 7363 6f72 6572 2100 0000 720b 0000  f_scorer!...r...
+000005e0: 0072 0d00 0000 7217 0000 0072 1200 0000  .r....r....r....
+000005f0: 7212 0000 0072 1300 0000 721a 0000 0023  r....r....r....#
+00000600: 0000 0073 1200 0000 0001 0a01 0601 0200  ...s............
+00000610: 0201 0401 0401 0201 04fb 7a10 4469 6365  ..........z.Dice
+00000620: 4c6f 7373 2e66 6f72 7761 7264 2904 7207  Loss.forward).r.
+00000630: 0000 0072 0700 0000 4e4e 721b 0000 0072  ...r....NNr....r
+00000640: 1200 0000 7212 0000 0072 1000 0000 7213  ....r....r....r.
+00000650: 0000 0072 2000 0000 1a00 0000 7304 0000  ...r .......s...
+00000660: 0008 020e 0772 2000 0000 6300 0000 0000  .....r ...c.....
+00000670: 0000 0000 0000 0000 0000 0005 0000 0000  ................
+00000680: 0000 0073 2600 0000 6500 5a01 6400 5a02  ...s&...e.Z.d.Z.
+00000690: 6409 8700 6601 6405 6406 8409 5a03 6407  d...f.d.d...Z.d.
+000006a0: 6408 8400 5a04 8700 0400 5a05 5300 290a  d...Z.....Z.S.).
+000006b0: da0b 5476 6572 736b 794c 6f73 73e7 3333  ..TverskyLoss.33
+000006c0: 3333 3333 d33f 7207 0000 00e7 6666 6666  3333.?r.....ffff
+000006d0: 6666 e63f 4e63 0600 0000 0000 0000 0000  ff.?Nc..........
+000006e0: 0000 0700 0000 0300 0000 0b00 0000 7334  ..............s4
+000006f0: 0000 0074 0083 006a 0166 007c 068e 0101  ...t...j.f.|....
+00000700: 007c 027c 005f 027c 017c 005f 037c 037c  .|.|._.|.|._.|.|
+00000710: 005f 0474 057c 0483 017c 005f 067c 057c  ._.t.|...|._.|.|
+00000720: 005f 0764 0053 0072 0800 0000 2908 7209  ._.d.S.r....).r.
+00000730: 0000 0072 0a00 0000 720b 0000 00da 0561  ...r....r......a
+00000740: 6c70 6861 7221 0000 0072 0500 0000 720c  lphar!...r....r.
+00000750: 0000 0072 0d00 0000 2907 720e 0000 0072  ...r....).r....r
+00000760: 2500 0000 720b 0000 0072 2100 0000 720c  %...r....r!...r.
+00000770: 0000 0072 0d00 0000 720f 0000 0072 1000  ...r....r....r..
+00000780: 0000 7212 0000 0072 1300 0000 720a 0000  ..r....r....r...
+00000790: 002f 0000 0073 0c00 0000 0001 0e01 0601  ./...s..........
+000007a0: 0601 0601 0a01 7a14 5476 6572 736b 794c  ......z.TverskyL
+000007b0: 6f73 732e 5f5f 696e 6974 5f5f 6303 0000  oss.__init__c...
+000007c0: 0000 0000 0000 0000 0003 0000 000a 0000  ................
+000007d0: 0043 0000 0073 2e00 0000 7c00 a000 7c01  .C...s....|...|.
+000007e0: a101 7d01 6401 7401 6a02 7c01 7c02 7c00  ..}.d.t.j.|.|.|.
+000007f0: 6a03 7c00 6a04 7c00 6a05 6400 7c00 6a06  j.|.j.|.j.d.|.j.
+00000800: 6402 8d07 1800 5300 a903 4e72 0200 0000  d.....S...Nr....
+00000810: 2905 7225 0000 0072 2100 0000 720b 0000  ).r%...r!...r...
+00000820: 0072 1400 0000 720d 0000 0029 0772 0c00  .r....r....).r..
+00000830: 0000 7215 0000 00da 0d74 7665 7273 6b79  ..r......tversky
+00000840: 5f73 636f 7265 7225 0000 0072 2100 0000  _scorer%...r!...
+00000850: 720b 0000 0072 0d00 0000 7217 0000 0072  r....r....r....r
+00000860: 1200 0000 7212 0000 0072 1300 0000 721a  ....r....r....r.
+00000870: 0000 0037 0000 0073 1400 0000 0001 0a01  ...7...s........
+00000880: 0601 0200 0201 0401 0401 0401 0201 04fa  ................
+00000890: 7a13 5476 6572 736b 794c 6f73 732e 666f  z.TverskyLoss.fo
+000008a0: 7277 6172 6429 0572 2300 0000 7207 0000  rward).r#...r...
+000008b0: 0072 2400 0000 4e4e 721b 0000 0072 1200  .r$...NNr....r..
+000008c0: 0000 7212 0000 0072 1000 0000 7213 0000  ..r....r....r...
+000008d0: 0072 2200 0000 2d00 0000 7304 0000 0008  .r"...-...s.....
+000008e0: 020e 0872 2200 0000 6300 0000 0000 0000  ...r"...c.......
+000008f0: 0000 0000 0000 0000 0006 0000 0000 0000  ................
+00000900: 0073 2600 0000 6500 5a01 6400 5a02 640a  .s&...e.Z.d.Z.d.
+00000910: 8700 6601 6406 6407 8409 5a03 6408 6409  ..f.d.d...Z.d.d.
+00000920: 8400 5a04 8700 0400 5a05 5300 290b da10  ..Z.....Z.S.)...
+00000930: 466f 6361 6c54 7665 7273 6b79 4c6f 7373  FocalTverskyLoss
+00000940: 7223 0000 0072 0700 0000 7224 0000 00e7  r#...r....r$....
+00000950: 0000 0000 0000 e83f 4e63 0700 0000 0000  .......?Nc......
+00000960: 0000 0000 0000 0800 0000 0300 0000 0b00  ................
+00000970: 0000 733a 0000 0074 0083 006a 0166 007c  ..s:...t...j.f.|
+00000980: 078e 0101 007c 027c 005f 027c 017c 005f  .....|.|._.|.|._
+00000990: 037c 037c 005f 047c 047c 005f 0574 067c  .|.|._.|.|._.t.|
+000009a0: 0583 017c 005f 077c 067c 005f 0864 0053  ...|._.|.|._.d.S
+000009b0: 0072 0800 0000 2909 7209 0000 0072 0a00  .r....).r....r..
+000009c0: 0000 720b 0000 0072 2500 0000 7221 0000  ..r....r%...r!..
+000009d0: 00da 0567 616d 6d61 7205 0000 0072 0c00  ...gammar....r..
+000009e0: 0000 720d 0000 0029 0872 0e00 0000 7225  ..r....).r....r%
+000009f0: 0000 0072 0b00 0000 7221 0000 0072 2a00  ...r....r!...r*.
+00000a00: 0000 720c 0000 0072 0d00 0000 720f 0000  ..r....r....r...
+00000a10: 0072 1000 0000 7212 0000 0072 1300 0000  .r....r....r....
+00000a20: 720a 0000 0044 0000 0073 0e00 0000 0001  r....D...s......
+00000a30: 0e01 0601 0601 0601 0601 0a01 7a19 466f  ............z.Fo
+00000a40: 6361 6c54 7665 7273 6b79 4c6f 7373 2e5f  calTverskyLoss._
+00000a50: 5f69 6e69 745f 5f63 0300 0000 0000 0000  _init__c........
+00000a60: 0000 0000 0400 0000 0a00 0000 4300 0000  ............C...
+00000a70: 733c 0000 007c 00a0 007c 01a1 017d 0164  s<...|...|...}.d
+00000a80: 0174 016a 027c 017c 027c 006a 037c 006a  .t.j.|.|.|.j.|.j
+00000a90: 047c 006a 0564 007c 006a 0664 028d 0718  .|.j.d.|.j.d....
+00000aa0: 007d 0374 07a0 087c 037c 006a 09a1 0253  .}.t...|.|.j...S
+00000ab0: 0072 2600 0000 290a 720c 0000 0072 1500  .r&...).r....r..
+00000ac0: 0000 7227 0000 0072 2500 0000 7221 0000  ..r'...r%...r!..
+00000ad0: 0072 0b00 0000 720d 0000 00da 0574 6f72  .r....r......tor
+00000ae0: 6368 da03 706f 7772 2a00 0000 2904 720e  ch..powr*...).r.
+00000af0: 0000 0072 1800 0000 7219 0000 005a 0c74  ...r....r....Z.t
+00000b00: 7665 7273 6b79 5f6c 6f73 7372 1200 0000  versky_lossr....
+00000b10: 7212 0000 0072 1300 0000 721a 0000 004d  r....r....r....M
+00000b20: 0000 0073 1600 0000 0001 0a01 0601 0200  ...s............
+00000b30: 0201 0401 0401 0401 0201 04fa 0809 7a18  ..............z.
+00000b40: 466f 6361 6c54 7665 7273 6b79 4c6f 7373  FocalTverskyLoss
+00000b50: 2e66 6f72 7761 7264 2906 7223 0000 0072  .forward).r#...r
+00000b60: 0700 0000 7224 0000 0072 2900 0000 4e4e  ....r$...r)...NN
+00000b70: 721b 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+00000b80: 1000 0000 7213 0000 0072 2800 0000 4200  ....r....r(...B.
+00000b90: 0000 7304 0000 0008 020e 0972 2800 0000  ..s........r(...
+00000ba0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000bb0: 0001 0000 0040 0000 0073 0c00 0000 6500  .....@...s....e.
+00000bc0: 5a01 6400 5a02 6401 5300 2902 da06 4c31  Z.d.Z.d.S.)...L1
+00000bd0: 4c6f 7373 4ea9 0372 1c00 0000 721d 0000  LossN..r....r...
+00000be0: 0072 1e00 0000 7212 0000 0072 1200 0000  .r....r....r....
+00000bf0: 7212 0000 0072 1300 0000 722d 0000 005b  r....r....r-...[
+00000c00: 0000 0073 0200 0000 0801 722d 0000 0063  ...s......r-...c
+00000c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000c20: 0100 0000 4000 0000 730c 0000 0065 005a  ....@...s....e.Z
+00000c30: 0164 005a 0264 0153 0029 02da 074d 5345  .d.Z.d.S.)...MSE
+00000c40: 4c6f 7373 4e72 2e00 0000 7212 0000 0072  LossNr....r....r
+00000c50: 1200 0000 7212 0000 0072 1300 0000 722f  ....r....r....r/
+00000c60: 0000 005f 0000 0073 0200 0000 0801 722f  ..._...s......r/
+00000c70: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000c80: 0000 0000 0100 0000 4000 0000 730c 0000  ........@...s...
+00000c90: 0065 005a 0164 005a 0264 0153 0029 02da  .e.Z.d.Z.d.S.)..
+00000ca0: 1043 726f 7373 456e 7472 6f70 794c 6f73  .CrossEntropyLos
+00000cb0: 734e 722e 0000 0072 1200 0000 7212 0000  sNr....r....r...
+00000cc0: 0072 1200 0000 7213 0000 0072 3000 0000  .r....r....r0...
+00000cd0: 6300 0000 7302 0000 0008 0172 3000 0000  c...s......r0...
+00000ce0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000cf0: 0001 0000 0040 0000 0073 0c00 0000 6500  .....@...s....e.
+00000d00: 5a01 6400 5a02 6401 5300 2902 da07 4e4c  Z.d.Z.d.S.)...NL
+00000d10: 4c4c 6f73 734e 722e 0000 0072 1200 0000  LLossNr....r....
+00000d20: 7212 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+00000d30: 3100 0000 6700 0000 7302 0000 0008 0172  1...g...s......r
+00000d40: 3100 0000 6300 0000 0000 0000 0000 0000  1...c...........
+00000d50: 0000 0000 0001 0000 0040 0000 0073 0c00  .........@...s..
+00000d60: 0000 6500 5a01 6400 5a02 6401 5300 2902  ..e.Z.d.Z.d.S.).
+00000d70: da07 4243 454c 6f73 734e 722e 0000 0072  ..BCELossNr....r
+00000d80: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
+00000d90: 0000 0072 3200 0000 6b00 0000 7302 0000  ...r2...k...s...
+00000da0: 0008 0172 3200 0000 6300 0000 0000 0000  ...r2...c.......
+00000db0: 0000 0000 0000 0000 0004 0000 0000 0000  ................
+00000dc0: 0073 2600 0000 6500 5a01 6400 5a02 6406  .s&...e.Z.d.Z.d.
+00000dd0: 8700 6601 6402 6403 8409 5a03 6404 6405  ..f.d.d...Z.d.d.
+00000de0: 8400 5a04 8700 0400 5a05 5300 2907 da11  ..Z.....Z.S.)...
+00000df0: 4243 4557 6974 684c 6f67 6974 734c 6f73  BCEWithLogitsLos
+00000e00: 734e 6303 0000 0000 0000 0000 0000 0004  sNc.............
+00000e10: 0000 0003 0000 000b 0000 0073 2200 0000  ...........s"...
+00000e20: 7400 8300 6a01 6600 7c03 8e01 0100 7402  t...j.f.|.....t.
+00000e30: 7c01 8301 7c00 5f03 7c02 7c00 5f04 6400  |...|._.|.|._.d.
+00000e40: 5300 7208 0000 0029 0572 0900 0000 720a  S.r....).r....r.
+00000e50: 0000 0072 0500 0000 720c 0000 0072 0d00  ...r....r....r..
+00000e60: 0000 2904 720e 0000 0072 0c00 0000 720d  ..).r....r....r.
+00000e70: 0000 0072 0f00 0000 7210 0000 0072 1200  ...r....r....r..
+00000e80: 0000 7213 0000 0072 0a00 0000 7000 0000  ..r....r....p...
+00000e90: 7306 0000 0000 010e 020a 017a 1a42 4345  s..........z.BCE
+00000ea0: 5769 7468 4c6f 6769 7473 4c6f 7373 2e5f  WithLogitsLoss._
+00000eb0: 5f69 6e69 745f 5f63 0300 0000 0000 0000  _init__c........
+00000ec0: 0000 0000 0300 0000 0600 0000 4300 0000  ............C...
+00000ed0: 731e 0000 007c 00a0 007c 01a1 017d 0174  s....|...|...}.t
+00000ee0: 016a 027c 017c 0264 007c 006a 0364 018d  .j.|.|.d.|.j.d..
+00000ef0: 0453 0029 024e 2902 7214 0000 0072 0d00  .S.).N).r....r..
+00000f00: 0000 2904 720c 0000 0072 1500 0000 da20  ..).r....r..... 
+00000f10: 6269 6e61 7279 5f63 726f 7373 5f65 6e74  binary_cross_ent
+00000f20: 726f 7079 5f77 6974 685f 6c6f 6769 7473  ropy_with_logits
+00000f30: 720d 0000 0072 1700 0000 7212 0000 0072  r....r....r....r
+00000f40: 1200 0000 7213 0000 0072 1a00 0000 7600  ....r....r....v.
+00000f50: 0000 730e 0000 0000 010a 0104 0102 0002  ..s.............
+00000f60: 0102 0104 fd7a 1942 4345 5769 7468 4c6f  .....z.BCEWithLo
+00000f70: 6769 7473 4c6f 7373 2e66 6f72 7761 7264  gitsLoss.forward
+00000f80: 2902 4e4e 721b 0000 0072 1200 0000 7212  ).NNr....r....r.
+00000f90: 0000 0072 1000 0000 7213 0000 0072 3300  ...r....r....r3.
+00000fa0: 0000 6f00 0000 7304 0000 0008 010e 0672  ..o...s........r
+00000fb0: 3300 0000 2913 da08 746f 7263 682e 6e6e  3...)...torch.nn
+00000fc0: da02 6e6e 722b 0000 00da 0072 0300 0000  ..nnr+.....r....
+00000fd0: 7204 0000 0072 1500 0000 7205 0000 005a  r....r....r....Z
+00000fe0: 044c 6f73 7372 0600 0000 7220 0000 0072  .Lossr....r ...r
+00000ff0: 2200 0000 7228 0000 0072 2d00 0000 722f  "...r(...r-...r/
+00001000: 0000 0072 3000 0000 7231 0000 0072 3200  ...r0...r1...r2.
+00001010: 0000 7233 0000 0072 1200 0000 7212 0000  ..r3...r....r...
+00001020: 0072 1200 0000 7213 0000 00da 083c 6d6f  .r....r......<mo
+00001030: 6475 6c65 3e01 0000 0073 1c00 0000 0c01  dule>....s......
+00001040: 0801 0c01 0c01 0c03 1212 1213 1215 1219  ................
+00001050: 1604 1604 1604 1604 1604                 ..........
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/losses.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/losses.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/meter.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/meter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/meter.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/meter.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/meter.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/meter.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/meter.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/meter.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:22 2023 UTC, .py size: 1719 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -22,122 +22,121 @@
 00000150: 746f 2066 6f6c 6c6f 772e 0a20 2020 2063  to follow..    c
 00000160: 0100 0000 0000 0000 0000 0000 0100 0000  ................
 00000170: 0100 0000 4300 0000 7304 0000 0064 0153  ....C...s....d.S
 00000180: 0029 027a 2552 6573 6574 7320 7468 6520  .).z%Resets the 
 00000190: 6d65 7465 7220 746f 2064 6566 6175 6c74  meter to default
 000001a0: 2073 6574 7469 6e67 732e 4ea9 00a9 01da   settings.N.....
 000001b0: 0473 656c 6672 0300 0000 7203 0000 00fa  .selfr....r.....
-000001c0: 5243 3a5c 5573 6572 735c 6d68 616e 616e  RC:\Users\mhanan
+000001c0: 4563 3a5c 5573 6572 735c 6d68 616e 616e  Ec:\Users\mhanan
 000001d0: 5c44 6f77 6e6c 6f61 6473 5c48 616e 616e  \Downloads\Hanan
-000001e0: 5c4d 616d 6d6f 5079 5c6d 616d 6d6f 7079  \MammoPy\mammopy
-000001f0: 5c73 6567 6d65 6e74 6174 696f 6e5f 6d6f  \segmentation_mo
-00000200: 6465 6c73 5c75 7469 6c73 5c6d 6574 6572  dels\utils\meter
-00000210: 2e70 79da 0572 6573 6574 0900 0000 7302  .py..reset....s.
-00000220: 0000 0000 027a 0b4d 6574 6572 2e72 6573  .....z.Meter.res
-00000230: 6574 6302 0000 0000 0000 0000 0000 0002  etc.............
-00000240: 0000 0001 0000 0043 0000 0073 0400 0000  .......C...s....
-00000250: 6401 5300 2902 7a5f 4c6f 6720 6120 6e65  d.S.).z_Log a ne
-00000260: 7720 7661 6c75 6520 746f 2074 6865 206d  w value to the m
-00000270: 6574 6572 0a20 2020 2020 2020 2041 7267  eter.        Arg
-00000280: 733a 0a20 2020 2020 2020 2020 2020 2076  s:.            v
-00000290: 616c 7565 3a20 4e65 7874 2072 6573 7475  alue: Next restu
-000002a0: 6c74 2074 6f20 696e 636c 7564 652e 0a20  lt to include.. 
-000002b0: 2020 2020 2020 204e 7203 0000 0029 0272         Nr....).r
-000002c0: 0500 0000 da05 7661 6c75 6572 0300 0000  ......valuer....
-000002d0: 7203 0000 0072 0600 0000 da03 6164 640d  r....r......add.
-000002e0: 0000 0073 0200 0000 0005 7a09 4d65 7465  ...s......z.Mete
-000002f0: 722e 6164 6463 0100 0000 0000 0000 0000  r.addc..........
-00000300: 0000 0100 0000 0100 0000 4300 0000 7304  ..........C...s.
-00000310: 0000 0064 0153 0029 027a 3047 6574 2074  ...d.S.).z0Get t
-00000320: 6865 2076 616c 7565 206f 6620 7468 6520  he value of the 
-00000330: 6d65 7465 7220 696e 2074 6865 2063 7572  meter in the cur
-00000340: 7265 6e74 2073 7461 7465 2e4e 7203 0000  rent state.Nr...
-00000350: 0072 0400 0000 7203 0000 0072 0300 0000  .r....r....r....
-00000360: 7206 0000 0072 0800 0000 1400 0000 7302  r....r........s.
-00000370: 0000 0000 027a 0b4d 6574 6572 2e76 616c  .....z.Meter.val
-00000380: 7565 4e29 07da 085f 5f6e 616d 655f 5fda  ueN)...__name__.
-00000390: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-000003a0: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
-000003b0: 5f5f 7207 0000 0072 0900 0000 7208 0000  __r....r....r...
-000003c0: 0072 0300 0000 7203 0000 0072 0300 0000  .r....r....r....
-000003d0: 7206 0000 0072 0200 0000 0400 0000 7308  r....r........s.
-000003e0: 0000 0008 0104 0408 0408 0772 0200 0000  ...........r....
-000003f0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000400: 0003 0000 0000 0000 0073 3600 0000 6500  .........s6...e.
-00000410: 5a01 6400 5a02 8700 6601 6401 6402 8408  Z.d.Z...f.d.d...
-00000420: 5a03 640a 6404 6405 8401 5a04 6406 6407  Z.d.d.d...Z.d.d.
-00000430: 8400 5a05 6408 6409 8400 5a06 8700 0400  ..Z.d.d...Z.....
-00000440: 5a07 5300 290b da11 4176 6572 6167 6556  Z.S.)...AverageV
-00000450: 616c 7565 4d65 7465 7263 0100 0000 0000  alueMeterc......
-00000460: 0000 0000 0000 0100 0000 0300 0000 0300  ................
-00000470: 0000 7320 0000 0074 0074 017c 0083 02a0  ..s ...t.t.|....
-00000480: 02a1 0001 007c 00a0 03a1 0001 0064 017c  .....|.......d.|
-00000490: 005f 0464 0053 0029 024e 7201 0000 0029  ._.d.S.).Nr....)
-000004a0: 05da 0573 7570 6572 720e 0000 00da 085f  ...superr......_
-000004b0: 5f69 6e69 745f 5f72 0700 0000 da03 7661  _init__r......va
-000004c0: 6c72 0400 0000 a901 da09 5f5f 636c 6173  lr........__clas
-000004d0: 735f 5f72 0300 0000 7206 0000 0072 1000  s__r....r....r..
-000004e0: 0000 1a00 0000 7306 0000 0000 010e 0108  ......s.........
-000004f0: 017a 1a41 7665 7261 6765 5661 6c75 654d  .z.AverageValueM
-00000500: 6574 6572 2e5f 5f69 6e69 745f 5fe9 0100  eter.__init__...
-00000510: 0000 6303 0000 0000 0000 0000 0000 0003  ..c.............
-00000520: 0000 0005 0000 0043 0000 0073 e200 0000  .......C...s....
-00000530: 7c01 7c00 5f00 7c00 0400 6a01 7c01 3700  |.|._.|...j.|.7.
-00000540: 0200 5f01 7c00 0400 6a02 7c01 7c01 1400  .._.|...j.|.|...
-00000550: 3700 0200 5f02 7c00 0400 6a03 7c02 3700  7..._.|...j.|.7.
-00000560: 0200 5f03 7c00 6a03 6401 6b02 7252 7404  .._.|.j.d.k.rRt.
-00000570: 6a05 7404 6a05 0200 7c00 5f06 7c00 5f07  j.t.j...|._.|._.
-00000580: 6e8c 7c00 6a03 6402 6b02 7280 6403 7c00  n.|.j.d.k.r.d.|.
-00000590: 6a01 1700 7c00 5f06 7404 6a08 7c00 5f07  j...|._.t.j.|._.
-000005a0: 7c00 6a06 7c00 5f09 6403 7c00 5f0a 6e5e  |.j.|._.d.|._.n^
-000005b0: 7c00 6a09 7c01 7c02 7c00 6a09 1400 1800  |.j.|.|.|.j.....
-000005c0: 740b 7c00 6a03 8301 1b00 1700 7c00 5f06  t.|.j.......|._.
-000005d0: 7c00 0400 6a0a 7c01 7c00 6a09 1800 7c01  |...j.|.|.j...|.
-000005e0: 7c00 6a06 1800 1400 3700 0200 5f0a 7c00  |.j.....7..._.|.
-000005f0: 6a06 7c00 5f09 7404 a00c 7c00 6a0a 7c00  j.|._.t...|.j.|.
-00000600: 6a03 6404 1800 1b00 a101 7c00 5f07 6400  j.d.......|._.d.
-00000610: 5300 2905 4e72 0100 0000 7214 0000 00e7  S.).Nr....r.....
-00000620: 0000 0000 0000 0000 6700 0000 0000 00f0  ........g.......
-00000630: 3f29 0d72 1100 0000 da03 7375 6dda 0376  ?).r......sum..v
-00000640: 6172 da01 6eda 026e 70da 036e 616e da04  ar..n..np..nan..
-00000650: 6d65 616e da03 7374 64da 0369 6e66 da08  mean..std..inf..
-00000660: 6d65 616e 5f6f 6c64 da03 6d5f 73da 0566  mean_old..m_s..f
-00000670: 6c6f 6174 da04 7371 7274 2903 7205 0000  loat..sqrt).r...
-00000680: 0072 0800 0000 7218 0000 0072 0300 0000  .r....r....r....
-00000690: 7203 0000 0072 0600 0000 7209 0000 001f  r....r....r.....
-000006a0: 0000 0073 1e00 0000 0001 0601 0e01 1201  ...s............
-000006b0: 0e02 0a01 1401 0a01 0c01 0801 0801 0802  ................
-000006c0: 2001 1e01 0801 7a15 4176 6572 6167 6556   .....z.AverageV
-000006d0: 616c 7565 4d65 7465 722e 6164 6463 0100  alueMeter.addc..
-000006e0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-000006f0: 0000 4300 0000 730c 0000 007c 006a 007c  ..C...s....|.j.|
-00000700: 006a 0166 0253 0029 014e 2902 721b 0000  .j.f.S.).N).r...
-00000710: 0072 1c00 0000 7204 0000 0072 0300 0000  .r....r....r....
-00000720: 7203 0000 0072 0600 0000 7208 0000 0032  r....r....r....2
-00000730: 0000 0073 0200 0000 0001 7a17 4176 6572  ...s......z.Aver
-00000740: 6167 6556 616c 7565 4d65 7465 722e 7661  ageValueMeter.va
-00000750: 6c75 6563 0100 0000 0000 0000 0000 0000  luec............
-00000760: 0100 0000 0200 0000 4300 0000 7338 0000  ........C...s8..
-00000770: 0064 017c 005f 0064 027c 005f 0164 027c  .d.|._.d.|._.d.|
-00000780: 005f 0264 027c 005f 0374 046a 057c 005f  ._.d.|._.t.j.|._
-00000790: 0664 027c 005f 0764 027c 005f 0874 046a  .d.|._.d.|._.t.j
-000007a0: 057c 005f 0964 0053 0029 034e 7201 0000  .|._.d.S.).Nr...
-000007b0: 0072 1500 0000 290a 7218 0000 0072 1600  .r....).r....r..
-000007c0: 0000 7217 0000 0072 1100 0000 7219 0000  ..r....r....r...
-000007d0: 0072 1a00 0000 721b 0000 0072 1e00 0000  .r....r....r....
-000007e0: 721f 0000 0072 1c00 0000 7204 0000 0072  r....r....r....r
-000007f0: 0300 0000 7203 0000 0072 0600 0000 7207  ....r....r....r.
-00000800: 0000 0035 0000 0073 1000 0000 0001 0601  ...5...s........
-00000810: 0601 0601 0601 0801 0601 0601 7a17 4176  ............z.Av
-00000820: 6572 6167 6556 616c 7565 4d65 7465 722e  erageValueMeter.
-00000830: 7265 7365 7429 0172 1400 0000 2908 720a  reset).r....).r.
-00000840: 0000 0072 0b00 0000 720c 0000 0072 1000  ...r....r....r..
-00000850: 0000 7209 0000 0072 0800 0000 7207 0000  ..r....r....r...
-00000860: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
-00000870: 7203 0000 0072 0300 0000 7212 0000 0072  r....r....r....r
-00000880: 0600 0000 720e 0000 0019 0000 0073 0800  ....r........s..
-00000890: 0000 0801 0c05 0a13 0803 720e 0000 0029  ..........r....)
-000008a0: 05da 056e 756d 7079 7219 0000 00da 066f  ...numpyr......o
-000008b0: 626a 6563 7472 0200 0000 720e 0000 0072  bjectr....r....r
-000008c0: 0300 0000 7203 0000 0072 0300 0000 7206  ....r....r....r.
-000008d0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-000008e0: 0073 0400 0000 0803 1015                 .s........
+000001e0: 5c6d 675c 7365 676d 656e 7461 7469 6f6e  \mg\segmentation
+000001f0: 5f6d 6f64 656c 735c 7574 696c 735c 6d65  _models\utils\me
+00000200: 7465 722e 7079 da05 7265 7365 7409 0000  ter.py..reset...
+00000210: 0073 0200 0000 0002 7a0b 4d65 7465 722e  .s......z.Meter.
+00000220: 7265 7365 7463 0200 0000 0000 0000 0000  resetc..........
+00000230: 0000 0200 0000 0100 0000 4300 0000 7304  ..........C...s.
+00000240: 0000 0064 0153 0029 027a 5f4c 6f67 2061  ...d.S.).z_Log a
+00000250: 206e 6577 2076 616c 7565 2074 6f20 7468   new value to th
+00000260: 6520 6d65 7465 720a 2020 2020 2020 2020  e meter.        
+00000270: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+00000280: 2020 7661 6c75 653a 204e 6578 7420 7265    value: Next re
+00000290: 7374 756c 7420 746f 2069 6e63 6c75 6465  stult to include
+000002a0: 2e0a 2020 2020 2020 2020 4e72 0300 0000  ..        Nr....
+000002b0: 2902 7205 0000 00da 0576 616c 7565 7203  ).r......valuer.
+000002c0: 0000 0072 0300 0000 7206 0000 00da 0361  ...r....r......a
+000002d0: 6464 0d00 0000 7302 0000 0000 057a 094d  dd....s......z.M
+000002e0: 6574 6572 2e61 6464 6301 0000 0000 0000  eter.addc.......
+000002f0: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
+00000300: 0073 0400 0000 6401 5300 2902 7a30 4765  .s....d.S.).z0Ge
+00000310: 7420 7468 6520 7661 6c75 6520 6f66 2074  t the value of t
+00000320: 6865 206d 6574 6572 2069 6e20 7468 6520  he meter in the 
+00000330: 6375 7272 656e 7420 7374 6174 652e 4e72  current state.Nr
+00000340: 0300 0000 7204 0000 0072 0300 0000 7203  ....r....r....r.
+00000350: 0000 0072 0600 0000 7208 0000 0014 0000  ...r....r.......
+00000360: 0073 0200 0000 0002 7a0b 4d65 7465 722e  .s......z.Meter.
+00000370: 7661 6c75 654e 2907 da08 5f5f 6e61 6d65  valueN)...__name
+00000380: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000390: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
+000003a0: 646f 635f 5f72 0700 0000 7209 0000 0072  doc__r....r....r
+000003b0: 0800 0000 7203 0000 0072 0300 0000 7203  ....r....r....r.
+000003c0: 0000 0072 0600 0000 7202 0000 0004 0000  ...r....r.......
+000003d0: 0073 0800 0000 0801 0404 0804 0807 7202  .s............r.
+000003e0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000003f0: 0000 0000 0300 0000 0000 0000 7336 0000  ............s6..
+00000400: 0065 005a 0164 005a 0287 0066 0164 0164  .e.Z.d.Z...f.d.d
+00000410: 0284 085a 0364 0a64 0464 0584 015a 0464  ...Z.d.d.d...Z.d
+00000420: 0664 0784 005a 0564 0864 0984 005a 0687  .d...Z.d.d...Z..
+00000430: 0004 005a 0753 0029 0bda 1141 7665 7261  ...Z.S.)...Avera
+00000440: 6765 5661 6c75 654d 6574 6572 6301 0000  geValueMeterc...
+00000450: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+00000460: 0003 0000 0073 2000 0000 7400 7401 7c00  .....s ...t.t.|.
+00000470: 8302 a002 a100 0100 7c00 a003 a100 0100  ........|.......
+00000480: 6401 7c00 5f04 6400 5300 2902 4e72 0100  d.|._.d.S.).Nr..
+00000490: 0000 2905 da05 7375 7065 7272 0e00 0000  ..)...superr....
+000004a0: da08 5f5f 696e 6974 5f5f 7207 0000 00da  ..__init__r.....
+000004b0: 0376 616c 7204 0000 00a9 01da 095f 5f63  .valr........__c
+000004c0: 6c61 7373 5f5f 7203 0000 0072 0600 0000  lass__r....r....
+000004d0: 7210 0000 001a 0000 0073 0600 0000 0001  r........s......
+000004e0: 0e01 0801 7a1a 4176 6572 6167 6556 616c  ....z.AverageVal
+000004f0: 7565 4d65 7465 722e 5f5f 696e 6974 5f5f  ueMeter.__init__
+00000500: e901 0000 0063 0300 0000 0000 0000 0000  .....c..........
+00000510: 0000 0300 0000 0500 0000 4300 0000 73e2  ..........C...s.
+00000520: 0000 007c 017c 005f 007c 0004 006a 017c  ...|.|._.|...j.|
+00000530: 0137 0002 005f 017c 0004 006a 027c 017c  .7..._.|...j.|.|
+00000540: 0114 0037 0002 005f 027c 0004 006a 037c  ...7..._.|...j.|
+00000550: 0237 0002 005f 037c 006a 0364 016b 0272  .7..._.|.j.d.k.r
+00000560: 5274 046a 0574 046a 0502 007c 005f 067c  Rt.j.t.j...|._.|
+00000570: 005f 076e 8c7c 006a 0364 026b 0272 8064  ._.n.|.j.d.k.r.d
+00000580: 037c 006a 0117 007c 005f 0674 046a 087c  .|.j...|._.t.j.|
+00000590: 005f 077c 006a 067c 005f 0964 037c 005f  ._.|.j.|._.d.|._
+000005a0: 0a6e 5e7c 006a 097c 017c 027c 006a 0914  .n^|.j.|.|.|.j..
+000005b0: 0018 0074 0b7c 006a 0383 011b 0017 007c  ...t.|.j.......|
+000005c0: 005f 067c 0004 006a 0a7c 017c 006a 0918  ._.|...j.|.|.j..
+000005d0: 007c 017c 006a 0618 0014 0037 0002 005f  .|.|.j.....7..._
+000005e0: 0a7c 006a 067c 005f 0974 04a0 0c7c 006a  .|.j.|._.t...|.j
+000005f0: 0a7c 006a 0364 0418 001b 00a1 017c 005f  .|.j.d.......|._
+00000600: 0764 0053 0029 054e 7201 0000 0072 1400  .d.S.).Nr....r..
+00000610: 0000 e700 0000 0000 0000 0067 0000 0000  ...........g....
+00000620: 0000 f03f 290d 7211 0000 00da 0373 756d  ...?).r......sum
+00000630: da03 7661 72da 016e da02 6e70 da03 6e61  ..var..n..np..na
+00000640: 6eda 046d 6561 6eda 0373 7464 da03 696e  n..mean..std..in
+00000650: 66da 086d 6561 6e5f 6f6c 64da 036d 5f73  f..mean_old..m_s
+00000660: da05 666c 6f61 74da 0473 7172 7429 0372  ..float..sqrt).r
+00000670: 0500 0000 7208 0000 0072 1800 0000 7203  ....r....r....r.
+00000680: 0000 0072 0300 0000 7206 0000 0072 0900  ...r....r....r..
+00000690: 0000 1f00 0000 731e 0000 0000 0106 010e  ......s.........
+000006a0: 0112 010e 020a 0114 010a 010c 0108 0108  ................
+000006b0: 0108 0220 011e 0108 017a 1541 7665 7261  ... .....z.Avera
+000006c0: 6765 5661 6c75 654d 6574 6572 2e61 6464  geValueMeter.add
+000006d0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000006e0: 0002 0000 0043 0000 0073 0c00 0000 7c00  .....C...s....|.
+000006f0: 6a00 7c00 6a01 6602 5300 2901 4e29 0272  j.|.j.f.S.).N).r
+00000700: 1b00 0000 721c 0000 0072 0400 0000 7203  ....r....r....r.
+00000710: 0000 0072 0300 0000 7206 0000 0072 0800  ...r....r....r..
+00000720: 0000 3200 0000 7302 0000 0000 017a 1741  ..2...s......z.A
+00000730: 7665 7261 6765 5661 6c75 654d 6574 6572  verageValueMeter
+00000740: 2e76 616c 7565 6301 0000 0000 0000 0000  .valuec.........
+00000750: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
+00000760: 3800 0000 6401 7c00 5f00 6402 7c00 5f01  8...d.|._.d.|._.
+00000770: 6402 7c00 5f02 6402 7c00 5f03 7404 6a05  d.|._.d.|._.t.j.
+00000780: 7c00 5f06 6402 7c00 5f07 6402 7c00 5f08  |._.d.|._.d.|._.
+00000790: 7404 6a05 7c00 5f09 6400 5300 2903 4e72  t.j.|._.d.S.).Nr
+000007a0: 0100 0000 7215 0000 0029 0a72 1800 0000  ....r....).r....
+000007b0: 7216 0000 0072 1700 0000 7211 0000 0072  r....r....r....r
+000007c0: 1900 0000 721a 0000 0072 1b00 0000 721e  ....r....r....r.
+000007d0: 0000 0072 1f00 0000 721c 0000 0072 0400  ...r....r....r..
+000007e0: 0000 7203 0000 0072 0300 0000 7206 0000  ..r....r....r...
+000007f0: 0072 0700 0000 3500 0000 7310 0000 0000  .r....5...s.....
+00000800: 0106 0106 0106 0106 0108 0106 0106 017a  ...............z
+00000810: 1741 7665 7261 6765 5661 6c75 654d 6574  .AverageValueMet
+00000820: 6572 2e72 6573 6574 2901 7214 0000 0029  er.reset).r....)
+00000830: 0872 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
+00000840: 7210 0000 0072 0900 0000 7208 0000 0072  r....r....r....r
+00000850: 0700 0000 da0d 5f5f 636c 6173 7363 656c  ......__classcel
+00000860: 6c5f 5f72 0300 0000 7203 0000 0072 1200  l__r....r....r..
+00000870: 0000 7206 0000 0072 0e00 0000 1900 0000  ..r....r........
+00000880: 7308 0000 0008 010c 050a 1308 0372 0e00  s............r..
+00000890: 0000 2905 da05 6e75 6d70 7972 1900 0000  ..)...numpyr....
+000008a0: da06 6f62 6a65 6374 7202 0000 0072 0e00  ..objectr....r..
+000008b0: 0000 7203 0000 0072 0300 0000 7203 0000  ..r....r....r...
+000008c0: 0072 0600 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+000008d0: 0100 0000 7304 0000 0008 0310 15         ....s........
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/meter.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/meter.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/metrics.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/metrics.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/metrics.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/metrics.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/metrics.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/metrics.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/metrics.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/metrics.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:22 2023 UTC, .py size: 3026 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -27,170 +27,169 @@
 000001a0: da08 5f5f 696e 6974 5f5f da03 6570 73da  ..__init__..eps.
 000001b0: 0974 6872 6573 686f 6c64 7204 0000 00da  .thresholdr.....
 000001c0: 0a61 6374 6976 6174 696f 6eda 0f69 676e  .activation..ign
 000001d0: 6f72 655f 6368 616e 6e65 6c73 a906 da04  ore_channels....
 000001e0: 7365 6c66 720c 0000 0072 0d00 0000 720e  selfr....r....r.
 000001f0: 0000 0072 0f00 0000 da06 6b77 6172 6773  ...r......kwargs
 00000200: a901 da09 5f5f 636c 6173 735f 5fa9 00fa  ....__class__...
-00000210: 5443 3a5c 5573 6572 735c 6d68 616e 616e  TC:\Users\mhanan
+00000210: 4763 3a5c 5573 6572 735c 6d68 616e 616e  Gc:\Users\mhanan
 00000220: 5c44 6f77 6e6c 6f61 6473 5c48 616e 616e  \Downloads\Hanan
-00000230: 5c4d 616d 6d6f 5079 5c6d 616d 6d6f 7079  \MammoPy\mammopy
-00000240: 5c73 6567 6d65 6e74 6174 696f 6e5f 6d6f  \segmentation_mo
-00000250: 6465 6c73 5c75 7469 6c73 5c6d 6574 7269  dels\utils\metri
-00000260: 6373 2e70 7972 0b00 0000 0900 0000 730a  cs.pyr........s.
-00000270: 0000 0000 010e 0106 0106 010a 017a 0c49  .............z.I
-00000280: 6f55 2e5f 5f69 6e69 745f 5f63 0300 0000  oU.__init__c....
-00000290: 0000 0000 0000 0000 0300 0000 0700 0000  ................
-000002a0: 4300 0000 7324 0000 007c 00a0 007c 01a1  C...s$...|...|..
-000002b0: 017d 0174 016a 027c 017c 027c 006a 037c  .}.t.j.|.|.|.j.|
-000002c0: 006a 047c 006a 0564 018d 0553 00a9 024e  .j.|.j.d...S...N
-000002d0: 2903 720c 0000 0072 0d00 0000 720f 0000  ).r....r....r...
-000002e0: 0029 0672 0e00 0000 da01 46da 0369 6f75  .).r......F..iou
-000002f0: 720c 0000 0072 0d00 0000 720f 0000 00a9  r....r....r.....
-00000300: 0372 1100 0000 da04 795f 7072 da04 795f  .r......y_pr..y_
-00000310: 6774 7215 0000 0072 1500 0000 7216 0000  gtr....r....r...
-00000320: 00da 0766 6f72 7761 7264 1000 0000 7310  ...forward....s.
-00000330: 0000 0000 010a 0104 0102 0002 0104 0104  ................
-00000340: 0104 fc7a 0b49 6f55 2e66 6f72 7761 7264  ...z.IoU.forward
-00000350: 2904 7206 0000 0072 0700 0000 4e4e a906  ).r....r....NN..
-00000360: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000370: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000380: 6d65 5f5f 720b 0000 0072 1d00 0000 da0d  me__r....r......
-00000390: 5f5f 636c 6173 7363 656c 6c5f 5f72 1500  __classcell__r..
-000003a0: 0000 7215 0000 0072 1300 0000 7216 0000  ..r....r....r...
-000003b0: 0072 0500 0000 0600 0000 7306 0000 0008  .r........s.....
-000003c0: 0104 020e 0772 0500 0000 6300 0000 0000  .....r....c.....
-000003d0: 0000 0000 0000 0000 0000 0005 0000 0000  ................
-000003e0: 0000 0073 2600 0000 6500 5a01 6400 5a02  ...s&...e.Z.d.Z.
-000003f0: 6409 8700 6601 6405 6406 8409 5a03 6407  d...f.d.d...Z.d.
-00000400: 6408 8400 5a04 8700 0400 5a05 5300 290a  d...Z.....Z.S.).
-00000410: da06 4673 636f 7265 7201 0000 0072 0600  ..Fscorer....r..
-00000420: 0000 7207 0000 004e 6306 0000 0000 0000  ..r....Nc.......
-00000430: 0000 0000 0007 0000 0003 0000 000b 0000  ................
-00000440: 0073 3400 0000 7400 8300 6a01 6600 7c06  .s4...t...j.f.|.
-00000450: 8e01 0100 7c02 7c00 5f02 7c01 7c00 5f03  ....|.|._.|.|._.
-00000460: 7c03 7c00 5f04 7405 7c04 8301 7c00 5f06  |.|._.t.|...|._.
-00000470: 7c05 7c00 5f07 6400 5300 7208 0000 0029  |.|._.d.S.r....)
-00000480: 0872 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
-00000490: da04 6265 7461 720d 0000 0072 0400 0000  ..betar....r....
-000004a0: 720e 0000 0072 0f00 0000 2907 7211 0000  r....r....).r...
-000004b0: 0072 2400 0000 720c 0000 0072 0d00 0000  .r$...r....r....
-000004c0: 720e 0000 0072 0f00 0000 7212 0000 0072  r....r....r....r
-000004d0: 1300 0000 7215 0000 0072 1600 0000 720b  ....r....r....r.
-000004e0: 0000 001c 0000 0073 0c00 0000 0001 0e01  .......s........
-000004f0: 0601 0601 0601 0a01 7a0f 4673 636f 7265  ........z.Fscore
-00000500: 2e5f 5f69 6e69 745f 5f63 0300 0000 0000  .__init__c......
-00000510: 0000 0000 0000 0300 0000 0800 0000 4300  ..............C.
-00000520: 0000 7328 0000 007c 00a0 007c 01a1 017d  ..s(...|...|...}
-00000530: 0174 016a 027c 017c 027c 006a 037c 006a  .t.j.|.|.|.j.|.j
-00000540: 047c 006a 057c 006a 0664 018d 0653 0029  .|.j.|.j.d...S.)
-00000550: 024e 2904 720c 0000 0072 2400 0000 720d  .N).r....r$...r.
-00000560: 0000 0072 0f00 0000 2907 720e 0000 0072  ...r....).r....r
-00000570: 1800 0000 da07 665f 7363 6f72 6572 0c00  ......f_scorer..
-00000580: 0000 7224 0000 0072 0d00 0000 720f 0000  ..r$...r....r...
-00000590: 0072 1a00 0000 7215 0000 0072 1500 0000  .r....r....r....
-000005a0: 7216 0000 0072 1d00 0000 2400 0000 7312  r....r....$...s.
-000005b0: 0000 0000 010a 0104 0102 0002 0104 0104  ................
-000005c0: 0104 0104 fb7a 0e46 7363 6f72 652e 666f  .....z.Fscore.fo
-000005d0: 7277 6172 6429 0572 0100 0000 7206 0000  rward).r....r...
-000005e0: 0072 0700 0000 4e4e 721e 0000 0072 1500  .r....NNr....r..
-000005f0: 0000 7215 0000 0072 1300 0000 7216 0000  ..r....r....r...
-00000600: 0072 2300 0000 1a00 0000 7304 0000 0008  .r#.......s.....
-00000610: 020e 0872 2300 0000 6300 0000 0000 0000  ...r#...c.......
-00000620: 0000 0000 0000 0000 0004 0000 0000 0000  ................
-00000630: 0073 2600 0000 6500 5a01 6400 5a02 6407  .s&...e.Z.d.Z.d.
-00000640: 8700 6601 6403 6404 8409 5a03 6405 6406  ..f.d.d...Z.d.d.
-00000650: 8400 5a04 8700 0400 5a05 5300 2908 da08  ..Z.....Z.S.)...
-00000660: 4163 6375 7261 6379 7207 0000 004e 6304  Accuracyr....Nc.
-00000670: 0000 0000 0000 0000 0000 0005 0000 0003  ................
-00000680: 0000 000b 0000 0073 2800 0000 7400 8300  .......s(...t...
-00000690: 6a01 6600 7c04 8e01 0100 7c01 7c00 5f02  j.f.|.....|.|._.
-000006a0: 7403 7c02 8301 7c00 5f04 7c03 7c00 5f05  t.|...|._.|.|._.
-000006b0: 6400 5300 7208 0000 0029 0672 0a00 0000  d.S.r....).r....
-000006c0: 720b 0000 0072 0d00 0000 7204 0000 0072  r....r....r....r
-000006d0: 0e00 0000 720f 0000 0029 0572 1100 0000  ....r....).r....
-000006e0: 720d 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
-000006f0: 1200 0000 7213 0000 0072 1500 0000 7216  ....r....r....r.
-00000700: 0000 0072 0b00 0000 3100 0000 7308 0000  ...r....1...s...
-00000710: 0000 010e 0106 010a 017a 1141 6363 7572  .........z.Accur
-00000720: 6163 792e 5f5f 696e 6974 5f5f 6303 0000  acy.__init__c...
-00000730: 0000 0000 0000 0000 0003 0000 0006 0000  ................
-00000740: 0043 0000 0073 2000 0000 7c00 a000 7c01  .C...s ...|...|.
-00000750: a101 7d01 7401 6a02 7c01 7c02 7c00 6a03  ..}.t.j.|.|.|.j.
-00000760: 7c00 6a04 6401 8d04 5300 2902 4e29 0272  |.j.d...S.).N).r
-00000770: 0d00 0000 720f 0000 0029 0572 0e00 0000  ....r....).r....
-00000780: 7218 0000 00da 0861 6363 7572 6163 7972  r......accuracyr
-00000790: 0d00 0000 720f 0000 0072 1a00 0000 7215  ....r....r....r.
-000007a0: 0000 0072 1500 0000 7216 0000 0072 1d00  ...r....r....r..
-000007b0: 0000 3700 0000 730e 0000 0000 010a 0104  ..7...s.........
-000007c0: 0102 0002 0104 0104 fd7a 1041 6363 7572  .........z.Accur
-000007d0: 6163 792e 666f 7277 6172 6429 0372 0700  acy.forward).r..
-000007e0: 0000 4e4e 721e 0000 0072 1500 0000 7215  ..NNr....r....r.
-000007f0: 0000 0072 1300 0000 7216 0000 0072 2600  ...r....r....r&.
-00000800: 0000 2f00 0000 7304 0000 0008 020e 0672  ../...s........r
-00000810: 2600 0000 6300 0000 0000 0000 0000 0000  &...c...........
-00000820: 0000 0000 0004 0000 0000 0000 0073 2600  .............s&.
-00000830: 0000 6500 5a01 6400 5a02 6408 8700 6601  ..e.Z.d.Z.d...f.
-00000840: 6404 6405 8409 5a03 6406 6407 8400 5a04  d.d...Z.d.d...Z.
-00000850: 8700 0400 5a05 5300 2909 da06 5265 6361  ....Z.S.)...Reca
-00000860: 6c6c 7206 0000 0072 0700 0000 4e63 0500  llr....r....Nc..
-00000870: 0000 0000 0000 0000 0000 0600 0000 0300  ................
-00000880: 0000 0b00 0000 732e 0000 0074 0083 006a  ......s....t...j
-00000890: 0166 007c 058e 0101 007c 017c 005f 027c  .f.|.....|.|._.|
-000008a0: 027c 005f 0374 047c 0383 017c 005f 057c  .|._.t.|...|._.|
-000008b0: 047c 005f 0664 0053 0072 0800 0000 7209  .|._.d.S.r....r.
-000008c0: 0000 0072 1000 0000 7213 0000 0072 1500  ...r....r....r..
-000008d0: 0000 7216 0000 0072 0b00 0000 4200 0000  ..r....r....B...
-000008e0: 730a 0000 0000 010e 0106 0106 010a 017a  s..............z
-000008f0: 0f52 6563 616c 6c2e 5f5f 696e 6974 5f5f  .Recall.__init__
-00000900: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-00000910: 0007 0000 0043 0000 0073 2400 0000 7c00  .....C...s$...|.
-00000920: a000 7c01 a101 7d01 7401 6a02 7c01 7c02  ..|...}.t.j.|.|.
-00000930: 7c00 6a03 7c00 6a04 7c00 6a05 6401 8d05  |.j.|.j.|.j.d...
-00000940: 5300 7217 0000 0029 0672 0e00 0000 7218  S.r....).r....r.
-00000950: 0000 00da 0672 6563 616c 6c72 0c00 0000  .....recallr....
-00000960: 720d 0000 0072 0f00 0000 721a 0000 0072  r....r....r....r
-00000970: 1500 0000 7215 0000 0072 1600 0000 721d  ....r....r....r.
-00000980: 0000 0049 0000 0073 1000 0000 0001 0a01  ...I...s........
-00000990: 0401 0200 0201 0401 0401 04fc 7a0e 5265  ............z.Re
-000009a0: 6361 6c6c 2e66 6f72 7761 7264 2904 7206  call.forward).r.
-000009b0: 0000 0072 0700 0000 4e4e 721e 0000 0072  ...r....NNr....r
-000009c0: 1500 0000 7215 0000 0072 1300 0000 7216  ....r....r....r.
-000009d0: 0000 0072 2800 0000 4000 0000 7304 0000  ...r(...@...s...
-000009e0: 0008 020e 0772 2800 0000 6300 0000 0000  .....r(...c.....
-000009f0: 0000 0000 0000 0000 0000 0004 0000 0000  ................
-00000a00: 0000 0073 2600 0000 6500 5a01 6400 5a02  ...s&...e.Z.d.Z.
-00000a10: 6408 8700 6601 6404 6405 8409 5a03 6406  d...f.d.d...Z.d.
-00000a20: 6407 8400 5a04 8700 0400 5a05 5300 2909  d...Z.....Z.S.).
-00000a30: da09 5072 6563 6973 696f 6e72 0600 0000  ..Precisionr....
-00000a40: 7207 0000 004e 6305 0000 0000 0000 0000  r....Nc.........
-00000a50: 0000 0006 0000 0003 0000 000b 0000 0073  ...............s
-00000a60: 2e00 0000 7400 8300 6a01 6600 7c05 8e01  ....t...j.f.|...
-00000a70: 0100 7c01 7c00 5f02 7c02 7c00 5f03 7404  ..|.|._.|.|._.t.
-00000a80: 7c03 8301 7c00 5f05 7c04 7c00 5f06 6400  |...|._.|.|._.d.
-00000a90: 5300 7208 0000 0072 0900 0000 7210 0000  S.r....r....r...
-00000aa0: 0072 1300 0000 7215 0000 0072 1600 0000  .r....r....r....
-00000ab0: 720b 0000 0055 0000 0073 0a00 0000 0001  r....U...s......
-00000ac0: 0e01 0601 0601 0a01 7a12 5072 6563 6973  ........z.Precis
-00000ad0: 696f 6e2e 5f5f 696e 6974 5f5f 6303 0000  ion.__init__c...
-00000ae0: 0000 0000 0000 0000 0003 0000 0007 0000  ................
-00000af0: 0043 0000 0073 2400 0000 7c00 a000 7c01  .C...s$...|...|.
-00000b00: a101 7d01 7401 6a02 7c01 7c02 7c00 6a03  ..}.t.j.|.|.|.j.
-00000b10: 7c00 6a04 7c00 6a05 6401 8d05 5300 7217  |.j.|.j.d...S.r.
-00000b20: 0000 0029 0672 0e00 0000 7218 0000 00da  ...).r....r.....
-00000b30: 0970 7265 6369 7369 6f6e 720c 0000 0072  .precisionr....r
-00000b40: 0d00 0000 720f 0000 0072 1a00 0000 7215  ....r....r....r.
-00000b50: 0000 0072 1500 0000 7216 0000 0072 1d00  ...r....r....r..
-00000b60: 0000 5c00 0000 7310 0000 0000 010a 0104  ..\...s.........
-00000b70: 0102 0002 0104 0104 0104 fc7a 1150 7265  ...........z.Pre
-00000b80: 6369 7369 6f6e 2e66 6f72 7761 7264 2904  cision.forward).
-00000b90: 7206 0000 0072 0700 0000 4e4e 721e 0000  r....r....NNr...
-00000ba0: 0072 1500 0000 7215 0000 0072 1300 0000  .r....r....r....
-00000bb0: 7216 0000 0072 2a00 0000 5300 0000 7304  r....r*...S...s.
-00000bc0: 0000 0008 020e 0772 2a00 0000 4e29 0bda  .......r*...N)..
-00000bd0: 0072 0200 0000 7203 0000 0072 1800 0000  .r....r....r....
-00000be0: 7204 0000 00da 064d 6574 7269 6372 0500  r......Metricr..
-00000bf0: 0000 7223 0000 0072 2600 0000 7228 0000  ..r#...r&...r(..
-00000c00: 0072 2a00 0000 7215 0000 0072 1500 0000  .r*...r....r....
-00000c10: 7215 0000 0072 1600 0000 da08 3c6d 6f64  r....r......<mod
-00000c20: 756c 653e 0100 0000 730e 0000 000c 010c  ule>....s.......
-00000c30: 010c 0312 1412 1512 1112 13              ...........
+00000230: 5c6d 675c 7365 676d 656e 7461 7469 6f6e  \mg\segmentation
+00000240: 5f6d 6f64 656c 735c 7574 696c 735c 6d65  _models\utils\me
+00000250: 7472 6963 732e 7079 720b 0000 0009 0000  trics.pyr.......
+00000260: 0073 0a00 0000 0001 0e01 0601 0601 0a01  .s..............
+00000270: 7a0c 496f 552e 5f5f 696e 6974 5f5f 6303  z.IoU.__init__c.
+00000280: 0000 0000 0000 0000 0000 0003 0000 0007  ................
+00000290: 0000 0043 0000 0073 2400 0000 7c00 a000  ...C...s$...|...
+000002a0: 7c01 a101 7d01 7401 6a02 7c01 7c02 7c00  |...}.t.j.|.|.|.
+000002b0: 6a03 7c00 6a04 7c00 6a05 6401 8d05 5300  j.|.j.|.j.d...S.
+000002c0: a902 4e29 0372 0c00 0000 720d 0000 0072  ..N).r....r....r
+000002d0: 0f00 0000 2906 720e 0000 00da 0146 da03  ....).r......F..
+000002e0: 696f 7572 0c00 0000 720d 0000 0072 0f00  iour....r....r..
+000002f0: 0000 a903 7211 0000 00da 0479 5f70 72da  ....r......y_pr.
+00000300: 0479 5f67 7472 1500 0000 7215 0000 0072  .y_gtr....r....r
+00000310: 1600 0000 da07 666f 7277 6172 6410 0000  ......forward...
+00000320: 0073 1000 0000 0001 0a01 0401 0200 0201  .s..............
+00000330: 0401 0401 04fc 7a0b 496f 552e 666f 7277  ......z.IoU.forw
+00000340: 6172 6429 0472 0600 0000 7207 0000 004e  ard).r....r....N
+00000350: 4ea9 06da 085f 5f6e 616d 655f 5fda 0a5f  N....__name__.._
+00000360: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000370: 6c6e 616d 655f 5f72 0b00 0000 721d 0000  lname__r....r...
+00000380: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
+00000390: 7215 0000 0072 1500 0000 7213 0000 0072  r....r....r....r
+000003a0: 1600 0000 7205 0000 0006 0000 0073 0600  ....r........s..
+000003b0: 0000 0801 0402 0e07 7205 0000 0063 0000  ........r....c..
+000003c0: 0000 0000 0000 0000 0000 0000 0000 0500  ................
+000003d0: 0000 0000 0000 7326 0000 0065 005a 0164  ......s&...e.Z.d
+000003e0: 005a 0264 0987 0066 0164 0564 0684 095a  .Z.d...f.d.d...Z
+000003f0: 0364 0764 0884 005a 0487 0004 005a 0553  .d.d...Z.....Z.S
+00000400: 0029 0ada 0646 7363 6f72 6572 0100 0000  .)...Fscorer....
+00000410: 7206 0000 0072 0700 0000 4e63 0600 0000  r....r....Nc....
+00000420: 0000 0000 0000 0000 0700 0000 0300 0000  ................
+00000430: 0b00 0000 7334 0000 0074 0083 006a 0166  ....s4...t...j.f
+00000440: 007c 068e 0101 007c 027c 005f 027c 017c  .|.....|.|._.|.|
+00000450: 005f 037c 037c 005f 0474 057c 0483 017c  ._.|.|._.t.|...|
+00000460: 005f 067c 057c 005f 0764 0053 0072 0800  ._.|.|._.d.S.r..
+00000470: 0000 2908 720a 0000 0072 0b00 0000 720c  ..).r....r....r.
+00000480: 0000 00da 0462 6574 6172 0d00 0000 7204  .....betar....r.
+00000490: 0000 0072 0e00 0000 720f 0000 0029 0772  ...r....r....).r
+000004a0: 1100 0000 7224 0000 0072 0c00 0000 720d  ....r$...r....r.
+000004b0: 0000 0072 0e00 0000 720f 0000 0072 1200  ...r....r....r..
+000004c0: 0000 7213 0000 0072 1500 0000 7216 0000  ..r....r....r...
+000004d0: 0072 0b00 0000 1c00 0000 730c 0000 0000  .r........s.....
+000004e0: 010e 0106 0106 0106 010a 017a 0f46 7363  ...........z.Fsc
+000004f0: 6f72 652e 5f5f 696e 6974 5f5f 6303 0000  ore.__init__c...
+00000500: 0000 0000 0000 0000 0003 0000 0008 0000  ................
+00000510: 0043 0000 0073 2800 0000 7c00 a000 7c01  .C...s(...|...|.
+00000520: a101 7d01 7401 6a02 7c01 7c02 7c00 6a03  ..}.t.j.|.|.|.j.
+00000530: 7c00 6a04 7c00 6a05 7c00 6a06 6401 8d06  |.j.|.j.|.j.d...
+00000540: 5300 2902 4e29 0472 0c00 0000 7224 0000  S.).N).r....r$..
+00000550: 0072 0d00 0000 720f 0000 0029 0772 0e00  .r....r....).r..
+00000560: 0000 7218 0000 00da 0766 5f73 636f 7265  ..r......f_score
+00000570: 720c 0000 0072 2400 0000 720d 0000 0072  r....r$...r....r
+00000580: 0f00 0000 721a 0000 0072 1500 0000 7215  ....r....r....r.
+00000590: 0000 0072 1600 0000 721d 0000 0024 0000  ...r....r....$..
+000005a0: 0073 1200 0000 0001 0a01 0401 0200 0201  .s..............
+000005b0: 0401 0401 0401 04fb 7a0e 4673 636f 7265  ........z.Fscore
+000005c0: 2e66 6f72 7761 7264 2905 7201 0000 0072  .forward).r....r
+000005d0: 0600 0000 7207 0000 004e 4e72 1e00 0000  ....r....NNr....
+000005e0: 7215 0000 0072 1500 0000 7213 0000 0072  r....r....r....r
+000005f0: 1600 0000 7223 0000 001a 0000 0073 0400  ....r#.......s..
+00000600: 0000 0802 0e08 7223 0000 0063 0000 0000  ......r#...c....
+00000610: 0000 0000 0000 0000 0000 0000 0400 0000  ................
+00000620: 0000 0000 7326 0000 0065 005a 0164 005a  ....s&...e.Z.d.Z
+00000630: 0264 0787 0066 0164 0364 0484 095a 0364  .d...f.d.d...Z.d
+00000640: 0564 0684 005a 0487 0004 005a 0553 0029  .d...Z.....Z.S.)
+00000650: 08da 0841 6363 7572 6163 7972 0700 0000  ...Accuracyr....
+00000660: 4e63 0400 0000 0000 0000 0000 0000 0500  Nc..............
+00000670: 0000 0300 0000 0b00 0000 7328 0000 0074  ..........s(...t
+00000680: 0083 006a 0166 007c 048e 0101 007c 017c  ...j.f.|.....|.|
+00000690: 005f 0274 037c 0283 017c 005f 047c 037c  ._.t.|...|._.|.|
+000006a0: 005f 0564 0053 0072 0800 0000 2906 720a  ._.d.S.r....).r.
+000006b0: 0000 0072 0b00 0000 720d 0000 0072 0400  ...r....r....r..
+000006c0: 0000 720e 0000 0072 0f00 0000 2905 7211  ..r....r....).r.
+000006d0: 0000 0072 0d00 0000 720e 0000 0072 0f00  ...r....r....r..
+000006e0: 0000 7212 0000 0072 1300 0000 7215 0000  ..r....r....r...
+000006f0: 0072 1600 0000 720b 0000 0031 0000 0073  .r....r....1...s
+00000700: 0800 0000 0001 0e01 0601 0a01 7a11 4163  ............z.Ac
+00000710: 6375 7261 6379 2e5f 5f69 6e69 745f 5f63  curacy.__init__c
+00000720: 0300 0000 0000 0000 0000 0000 0300 0000  ................
+00000730: 0600 0000 4300 0000 7320 0000 007c 00a0  ....C...s ...|..
+00000740: 007c 01a1 017d 0174 016a 027c 017c 027c  .|...}.t.j.|.|.|
+00000750: 006a 037c 006a 0464 018d 0453 0029 024e  .j.|.j.d...S.).N
+00000760: 2902 720d 0000 0072 0f00 0000 2905 720e  ).r....r....).r.
+00000770: 0000 0072 1800 0000 da08 6163 6375 7261  ...r......accura
+00000780: 6379 720d 0000 0072 0f00 0000 721a 0000  cyr....r....r...
+00000790: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
+000007a0: 721d 0000 0037 0000 0073 0e00 0000 0001  r....7...s......
+000007b0: 0a01 0401 0200 0201 0401 04fd 7a10 4163  ............z.Ac
+000007c0: 6375 7261 6379 2e66 6f72 7761 7264 2903  curacy.forward).
+000007d0: 7207 0000 004e 4e72 1e00 0000 7215 0000  r....NNr....r...
+000007e0: 0072 1500 0000 7213 0000 0072 1600 0000  .r....r....r....
+000007f0: 7226 0000 002f 0000 0073 0400 0000 0802  r&.../...s......
+00000800: 0e06 7226 0000 0063 0000 0000 0000 0000  ..r&...c........
+00000810: 0000 0000 0000 0000 0400 0000 0000 0000  ................
+00000820: 7326 0000 0065 005a 0164 005a 0264 0887  s&...e.Z.d.Z.d..
+00000830: 0066 0164 0464 0584 095a 0364 0664 0784  .f.d.d...Z.d.d..
+00000840: 005a 0487 0004 005a 0553 0029 09da 0652  .Z.....Z.S.)...R
+00000850: 6563 616c 6c72 0600 0000 7207 0000 004e  ecallr....r....N
+00000860: 6305 0000 0000 0000 0000 0000 0006 0000  c...............
+00000870: 0003 0000 000b 0000 0073 2e00 0000 7400  .........s....t.
+00000880: 8300 6a01 6600 7c05 8e01 0100 7c01 7c00  ..j.f.|.....|.|.
+00000890: 5f02 7c02 7c00 5f03 7404 7c03 8301 7c00  _.|.|._.t.|...|.
+000008a0: 5f05 7c04 7c00 5f06 6400 5300 7208 0000  _.|.|._.d.S.r...
+000008b0: 0072 0900 0000 7210 0000 0072 1300 0000  .r....r....r....
+000008c0: 7215 0000 0072 1600 0000 720b 0000 0042  r....r....r....B
+000008d0: 0000 0073 0a00 0000 0001 0e01 0601 0601  ...s............
+000008e0: 0a01 7a0f 5265 6361 6c6c 2e5f 5f69 6e69  ..z.Recall.__ini
+000008f0: 745f 5f63 0300 0000 0000 0000 0000 0000  t__c............
+00000900: 0300 0000 0700 0000 4300 0000 7324 0000  ........C...s$..
+00000910: 007c 00a0 007c 01a1 017d 0174 016a 027c  .|...|...}.t.j.|
+00000920: 017c 027c 006a 037c 006a 047c 006a 0564  .|.|.j.|.j.|.j.d
+00000930: 018d 0553 0072 1700 0000 2906 720e 0000  ...S.r....).r...
+00000940: 0072 1800 0000 da06 7265 6361 6c6c 720c  .r......recallr.
+00000950: 0000 0072 0d00 0000 720f 0000 0072 1a00  ...r....r....r..
+00000960: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
+00000970: 0072 1d00 0000 4900 0000 7310 0000 0000  .r....I...s.....
+00000980: 010a 0104 0102 0002 0104 0104 0104 fc7a  ...............z
+00000990: 0e52 6563 616c 6c2e 666f 7277 6172 6429  .Recall.forward)
+000009a0: 0472 0600 0000 7207 0000 004e 4e72 1e00  .r....r....NNr..
+000009b0: 0000 7215 0000 0072 1500 0000 7213 0000  ..r....r....r...
+000009c0: 0072 1600 0000 7228 0000 0040 0000 0073  .r....r(...@...s
+000009d0: 0400 0000 0802 0e07 7228 0000 0063 0000  ........r(...c..
+000009e0: 0000 0000 0000 0000 0000 0000 0000 0400  ................
+000009f0: 0000 0000 0000 7326 0000 0065 005a 0164  ......s&...e.Z.d
+00000a00: 005a 0264 0887 0066 0164 0464 0584 095a  .Z.d...f.d.d...Z
+00000a10: 0364 0664 0784 005a 0487 0004 005a 0553  .d.d...Z.....Z.S
+00000a20: 0029 09da 0950 7265 6369 7369 6f6e 7206  .)...Precisionr.
+00000a30: 0000 0072 0700 0000 4e63 0500 0000 0000  ...r....Nc......
+00000a40: 0000 0000 0000 0600 0000 0300 0000 0b00  ................
+00000a50: 0000 732e 0000 0074 0083 006a 0166 007c  ..s....t...j.f.|
+00000a60: 058e 0101 007c 017c 005f 027c 027c 005f  .....|.|._.|.|._
+00000a70: 0374 047c 0383 017c 005f 057c 047c 005f  .t.|...|._.|.|._
+00000a80: 0664 0053 0072 0800 0000 7209 0000 0072  .d.S.r....r....r
+00000a90: 1000 0000 7213 0000 0072 1500 0000 7216  ....r....r....r.
+00000aa0: 0000 0072 0b00 0000 5500 0000 730a 0000  ...r....U...s...
+00000ab0: 0000 010e 0106 0106 010a 017a 1250 7265  ...........z.Pre
+00000ac0: 6369 7369 6f6e 2e5f 5f69 6e69 745f 5f63  cision.__init__c
+00000ad0: 0300 0000 0000 0000 0000 0000 0300 0000  ................
+00000ae0: 0700 0000 4300 0000 7324 0000 007c 00a0  ....C...s$...|..
+00000af0: 007c 01a1 017d 0174 016a 027c 017c 027c  .|...}.t.j.|.|.|
+00000b00: 006a 037c 006a 047c 006a 0564 018d 0553  .j.|.j.|.j.d...S
+00000b10: 0072 1700 0000 2906 720e 0000 0072 1800  .r....).r....r..
+00000b20: 0000 da09 7072 6563 6973 696f 6e72 0c00  ....precisionr..
+00000b30: 0000 720d 0000 0072 0f00 0000 721a 0000  ..r....r....r...
+00000b40: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
+00000b50: 721d 0000 005c 0000 0073 1000 0000 0001  r....\...s......
+00000b60: 0a01 0401 0200 0201 0401 0401 04fc 7a11  ..............z.
+00000b70: 5072 6563 6973 696f 6e2e 666f 7277 6172  Precision.forwar
+00000b80: 6429 0472 0600 0000 7207 0000 004e 4e72  d).r....r....NNr
+00000b90: 1e00 0000 7215 0000 0072 1500 0000 7213  ....r....r....r.
+00000ba0: 0000 0072 1600 0000 722a 0000 0053 0000  ...r....r*...S..
+00000bb0: 0073 0400 0000 0802 0e07 722a 0000 004e  .s........r*...N
+00000bc0: 290b da00 7202 0000 0072 0300 0000 7218  )...r....r....r.
+00000bd0: 0000 0072 0400 0000 da06 4d65 7472 6963  ...r......Metric
+00000be0: 7205 0000 0072 2300 0000 7226 0000 0072  r....r#...r&...r
+00000bf0: 2800 0000 722a 0000 0072 1500 0000 7215  (...r*...r....r.
+00000c00: 0000 0072 1500 0000 7216 0000 00da 083c  ...r....r......<
+00000c10: 6d6f 6475 6c65 3e01 0000 0073 0e00 0000  module>....s....
+00000c20: 0c01 0c01 0c03 1214 1215 1211 1213       ..............
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/metrics.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/metrics.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/train.cpython-310.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/train.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/train.cpython-36.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/train.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/train.cpython-37.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/train.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/train.cpython-38.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/train.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Mar 15 07:44:22 2023 UTC, .py size: 6382 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -26,348 +26,347 @@
 00000190: a101 7c00 5f08 6400 5300 a901 4e29 09da  ..|._.d.S...N)..
 000001a0: 0573 7570 6572 7205 0000 00da 085f 5f69  .superr......__i
 000001b0: 6e69 745f 5fda 0874 6173 6b5f 6e75 6dda  nit__..task_num.
 000001c0: 026e 6eda 0950 6172 616d 6574 6572 da05  .nn..Parameter..
 000001d0: 746f 7263 68da 057a 6572 6f73 da08 6c6f  torch..zeros..lo
 000001e0: 675f 7661 7273 2902 da04 7365 6c66 7209  g_vars)...selfr.
 000001f0: 0000 00a9 01da 095f 5f63 6c61 7373 5f5f  .......__class__
-00000200: a900 fa52 433a 5c55 7365 7273 5c6d 6861  ...RC:\Users\mha
+00000200: a900 fa45 633a 5c55 7365 7273 5c6d 6861  ...Ec:\Users\mha
 00000210: 6e61 6e5c 446f 776e 6c6f 6164 735c 4861  nan\Downloads\Ha
-00000220: 6e61 6e5c 4d61 6d6d 6f50 795c 6d61 6d6d  nan\MammoPy\mamm
-00000230: 6f70 795c 7365 676d 656e 7461 7469 6f6e  opy\segmentation
-00000240: 5f6d 6f64 656c 735c 7574 696c 735c 7472  _models\utils\tr
-00000250: 6169 6e2e 7079 7208 0000 000a 0000 0073  ain.pyr........s
-00000260: 0600 0000 0001 0e01 0601 7a15 5765 6967  ..........z.Weig
-00000270: 6874 6564 4c6f 7373 2e5f 5f69 6e69 745f  htedLoss.__init_
-00000280: 5f63 0300 0000 0000 0000 0000 0000 0500  _c..............
-00000290: 0000 0400 0000 4300 0000 7350 0000 0074  ......C...sP...t
-000002a0: 00a0 017c 006a 0264 0119 000b 00a1 017d  ...|.j.d.......}
-000002b0: 037c 037c 0114 007c 006a 0264 0119 0017  .|.|...|.j.d....
-000002c0: 007d 0174 00a0 017c 006a 0264 0219 000b  .}.t...|.j.d....
-000002d0: 00a1 017d 047c 047c 0214 007c 006a 0264  ...}.|.|...|.j.d
-000002e0: 0219 0017 007d 027c 017c 0217 0053 0029  .....}.|.|...S.)
-000002f0: 034e 7201 0000 0072 0300 0000 2903 720c  .Nr....r....).r.
-00000300: 0000 00da 0365 7870 720e 0000 0029 0572  .....expr....).r
-00000310: 0f00 0000 da06 6c6f 7373 5f31 da06 6c6f  ......loss_1..lo
-00000320: 7373 5f32 5a0b 7072 6563 6973 696f 6e5f  ss_2Z.precision_
-00000330: 315a 0b70 7265 6369 7369 6f6e 5f32 7212  1Z.precision_2r.
-00000340: 0000 0072 1200 0000 7213 0000 00da 0766  ...r....r......f
-00000350: 6f72 7761 7264 0f00 0000 730a 0000 0000  orward....s.....
-00000360: 0112 0112 0212 0112 027a 1457 6569 6768  .........z.Weigh
-00000370: 7465 644c 6f73 732e 666f 7277 6172 64a9  tedLoss.forward.
-00000380: 06da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00000390: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-000003a0: 616d 655f 5f72 0800 0000 7217 0000 00da  ame__r....r.....
-000003b0: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7212  .__classcell__r.
-000003c0: 0000 0072 1200 0000 7210 0000 0072 1300  ...r....r....r..
-000003d0: 0000 7205 0000 0009 0000 0073 0400 0000  ..r........s....
-000003e0: 0801 0c05 7205 0000 0063 0000 0000 0000  ....r....c......
-000003f0: 0000 0000 0000 0000 0000 0300 0000 0000  ................
-00000400: 0000 7324 0000 0065 005a 0164 005a 0287  ..s$...e.Z.d.Z..
-00000410: 0066 0164 0164 0284 085a 0364 0364 0484  .f.d.d...Z.d.d..
-00000420: 005a 0487 0004 005a 0553 0029 05da 0d4d  .Z.....Z.S.)...M
-00000430: 756c 7469 5461 736b 4c6f 7373 6301 0000  ultiTaskLossc...
-00000440: 0000 0000 0000 0000 0001 0000 0005 0000  ................
-00000450: 0003 0000 0073 3600 0000 7400 7401 7c00  .....s6...t.t.|.
-00000460: 8302 a002 a100 0100 7403 a004 7405 a006  ........t...t...
-00000470: 6401 a101 a101 7c00 5f07 7403 a004 7405  d.....|._.t...t.
-00000480: a006 6401 a101 a101 7c00 5f08 6400 5300  ..d.....|._.d.S.
-00000490: 2902 4e72 0300 0000 2909 7207 0000 0072  ).Nr....).r....r
-000004a0: 1d00 0000 7208 0000 0072 0a00 0000 720b  ....r....r....r.
-000004b0: 0000 0072 0c00 0000 720d 0000 00da 0773  ...r....r......s
-000004c0: 6967 6d61 5f31 da07 7369 676d 615f 32a9  igma_1..sigma_2.
-000004d0: 0172 0f00 0000 7210 0000 0072 1200 0000  .r....r....r....
-000004e0: 7213 0000 0072 0800 0000 1a00 0000 7306  r....r........s.
-000004f0: 0000 0000 010e 0212 017a 164d 756c 7469  .........z.Multi
-00000500: 5461 736b 4c6f 7373 2e5f 5f69 6e69 745f  TaskLoss.__init_
-00000510: 5f63 0300 0000 0000 0000 0000 0000 0600  _c..............
-00000520: 0000 0300 0000 4300 0000 7340 0000 0074  ......C...s@...t
-00000530: 00a0 017c 01a1 017c 006a 0264 0113 001b  ...|...|.j.d....
-00000540: 007c 006a 0217 007d 0374 00a0 017c 02a1  .|.j...}.t...|..
-00000550: 017c 006a 0364 0113 001b 007c 006a 0317  .|.j.d.....|.j..
-00000560: 007d 047c 037c 0417 007d 057c 0553 0029  .}.|.|...}.|.S.)
-00000570: 024e e902 0000 0029 0472 0c00 0000 da06  .N.....).r......
-00000580: 5465 6e73 6f72 721e 0000 0072 1f00 0000  Tensorr....r....
-00000590: 2906 720f 0000 0072 1500 0000 7216 0000  ).r....r....r...
-000005a0: 00da 026c 31da 026c 32da 046c 6f73 7372  ...l1..l2..lossr
-000005b0: 1200 0000 7212 0000 0072 1300 0000 7217  ....r....r....r.
-000005c0: 0000 0021 0000 0073 0800 0000 0003 1a01  ...!...s........
-000005d0: 1a01 0801 7a15 4d75 6c74 6954 6173 6b4c  ....z.MultiTaskL
-000005e0: 6f73 732e 666f 7277 6172 6472 1800 0000  oss.forwardr....
-000005f0: 7212 0000 0072 1200 0000 7210 0000 0072  r....r....r....r
-00000600: 1300 0000 721d 0000 0019 0000 0073 0400  ....r........s..
-00000610: 0000 0801 0c07 721d 0000 0072 2100 0000  ......r....r!...
-00000620: 2901 7209 0000 0063 0000 0000 0000 0000  ).r....c........
-00000630: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-00000640: 733e 0000 0065 005a 0164 005a 0264 1064  s>...e.Z.d.Z.d.d
-00000650: 0364 0484 015a 0364 0564 0684 005a 0464  .d...Z.d.d...Z.d
-00000660: 0764 0884 005a 0564 0964 0a84 005a 0664  .d...Z.d.d...Z.d
-00000670: 0b64 0c84 005a 0764 0d64 0e84 005a 0864  .d...Z.d.d...Z.d
-00000680: 0f53 0029 11da 0545 706f 6368 da03 6370  .S.)...Epoch..cp
-00000690: 7554 6307 0000 0000 0000 0000 0000 0007  uTc.............
-000006a0: 0000 0002 0000 0043 0000 0073 3000 0000  .......C...s0...
-000006b0: 7c01 7c00 5f00 7c02 7c00 5f01 7c03 7c00  |.|._.|.|._.|.|.
-000006c0: 5f02 7c04 7c00 5f03 7c06 7c00 5f04 7c05  _.|.|._.|.|._.|.
-000006d0: 7c00 5f05 7c00 a006 a100 0100 6400 5300  |._.|.......d.S.
-000006e0: 7206 0000 0029 07da 056d 6f64 656c 7225  r....)...modelr%
-000006f0: 0000 00da 076d 6574 7269 6373 da0a 7374  .....metrics..st
-00000700: 6167 655f 6e61 6d65 da07 7665 7262 6f73  age_name..verbos
-00000710: 65da 0664 6576 6963 65da 0a5f 746f 5f64  e..device.._to_d
-00000720: 6576 6963 6529 0772 0f00 0000 7228 0000  evice).r....r(..
-00000730: 0072 2500 0000 7229 0000 0072 2a00 0000  .r%...r)...r*...
-00000740: 722c 0000 0072 2b00 0000 7212 0000 0072  r,...r+...r....r
-00000750: 1200 0000 7213 0000 0072 0800 0000 2e00  ....r....r......
-00000760: 0000 730e 0000 0000 0106 0106 0106 0106  ..s.............
-00000770: 0106 0106 027a 0e45 706f 6368 2e5f 5f69  .....z.Epoch.__i
-00000780: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
-00000790: 0000 0200 0000 0400 0000 4300 0000 7338  ..........C...s8
-000007a0: 0000 007c 006a 00a0 017c 006a 02a1 0101  ...|.j...|.j....
-000007b0: 007c 006a 03a0 017c 006a 02a1 0101 007c  .|.j...|.j.....|
-000007c0: 006a 0444 005d 107d 017c 01a0 017c 006a  .j.D.].}.|...|.j
-000007d0: 02a1 0101 0071 2264 0053 0072 0600 0000  .....q"d.S.r....
-000007e0: 2905 7228 0000 00da 0274 6f72 2c00 0000  ).r(.....tor,...
-000007f0: 7225 0000 0072 2900 0000 2902 720f 0000  r%...r)...).r...
-00000800: 00da 066d 6574 7269 6372 1200 0000 7212  ...metricr....r.
-00000810: 0000 0072 1300 0000 722d 0000 0038 0000  ...r....r-...8..
-00000820: 0073 0800 0000 0001 0e01 0e01 0a01 7a10  .s............z.
-00000830: 4570 6f63 682e 5f74 6f5f 6465 7669 6365  Epoch._to_device
-00000840: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
-00000850: 0003 0000 0043 0000 0073 2000 0000 6401  .....C...s ...d.
-00000860: 6402 8400 7c01 a000 a100 4400 8301 7d02  d...|.....D...}.
-00000870: 6403 a001 7c02 a101 7d03 7c03 5300 2904  d...|...}.|.S.).
-00000880: 4e63 0100 0000 0000 0000 0000 0000 0300  Nc..............
-00000890: 0000 0600 0000 5300 0000 731c 0000 0067  ......S...s....g
-000008a0: 007c 005d 145c 027d 017d 0264 00a0 007c  .|.].\.}.}.d...|
-000008b0: 017c 02a1 0291 0271 0453 0029 017a 0a7b  .|.....q.S.).z.{
-000008c0: 7d20 2d20 7b3a 2e34 7d29 01da 0666 6f72  } - {:.4})...for
-000008d0: 6d61 74a9 03da 022e 30da 016b da01 7672  mat.....0..k..vr
-000008e0: 1200 0000 7212 0000 0072 1300 0000 da0a  ....r....r......
-000008f0: 3c6c 6973 7463 6f6d 703e 3f00 0000 7304  <listcomp>?...s.
-00000900: 0000 0006 0006 007a 2645 706f 6368 2e5f  .......z&Epoch._
-00000910: 666f 726d 6174 5f6c 6f67 732e 3c6c 6f63  format_logs.<loc
-00000920: 616c 733e 2e3c 6c69 7374 636f 6d70 3e7a  als>.<listcomp>z
-00000930: 022c 2029 02da 0569 7465 6d73 da04 6a6f  ., )...items..jo
-00000940: 696e 2904 720f 0000 00da 046c 6f67 735a  in).r......logsZ
-00000950: 0873 7472 5f6c 6f67 73da 0173 7212 0000  .str_logs..sr...
-00000960: 0072 1200 0000 7213 0000 00da 0c5f 666f  .r....r......_fo
-00000970: 726d 6174 5f6c 6f67 733e 0000 0073 0600  rmat_logs>...s..
-00000980: 0000 0001 1201 0a01 7a12 4570 6f63 682e  ........z.Epoch.
-00000990: 5f66 6f72 6d61 745f 6c6f 6773 6303 0000  _format_logsc...
-000009a0: 0000 0000 0000 0000 0003 0000 0001 0000  ................
-000009b0: 0043 0000 0073 0800 0000 7400 8201 6400  .C...s....t...d.
-000009c0: 5300 7206 0000 0029 01da 134e 6f74 496d  S.r....)...NotIm
-000009d0: 706c 656d 656e 7465 6445 7272 6f72 2903  plementedError).
-000009e0: 720f 0000 00da 0178 da01 7972 1200 0000  r......x..yr....
-000009f0: 7212 0000 0072 1300 0000 da0c 6261 7463  r....r......batc
-00000a00: 685f 7570 6461 7465 4300 0000 7302 0000  h_updateC...s...
-00000a10: 0000 017a 1245 706f 6368 2e62 6174 6368  ...z.Epoch.batch
-00000a20: 5f75 7064 6174 6563 0100 0000 0000 0000  _updatec........
-00000a30: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-00000a40: 7304 0000 0064 0053 0072 0600 0000 7212  s....d.S.r....r.
-00000a50: 0000 0072 2000 0000 7212 0000 0072 1200  ...r ...r....r..
-00000a60: 0000 7213 0000 00da 0e6f 6e5f 6570 6f63  ..r......on_epoc
-00000a70: 685f 7374 6172 7446 0000 0073 0200 0000  h_startF...s....
-00000a80: 0001 7a14 4570 6f63 682e 6f6e 5f65 706f  ..z.Epoch.on_epo
-00000a90: 6368 5f73 7461 7274 6302 0000 0000 0000  ch_startc.......
-00000aa0: 0000 0000 001c 0000 0009 0000 0043 0000  .............C..
-00000ab0: 0073 e401 0000 7c00 a000 a100 0100 6900  .s....|.......i.
-00000ac0: 7d02 7401 8300 7d03 7401 8300 7d04 7401  }.t...}.t...}.t.
-00000ad0: 8300 7d05 6401 6402 8400 7c00 6a02 4400  ..}.d.d...|.j.D.
-00000ae0: 8301 7d06 7403 7c01 7c00 6a04 7405 6a06  ..}.t.|.|.j.t.j.
-00000af0: 7c00 6a07 0c00 6403 8d04 9001 8f92 7d07  |.j...d.......}.
-00000b00: 7c07 4400 9001 5d84 5c03 7d08 7d09 7d0a  |.D...].\.}.}.}.
-00000b10: 7c08 a008 7c00 6a09 a101 7c09 a008 7c00  |...|.j...|...|.
-00000b20: 6a09 a101 7c0a a008 7c00 6a09 a101 0300  j...|...|.j.....
-00000b30: 0200 7d08 7d09 7d0a 7c00 a00a 7c08 7c09  ..}.}.}.|...|.|.
-00000b40: 7c0a a103 5c05 7d0b 7d0c 7d0d 7d0e 7d0f  |...\.}.}.}.}.}.
-00000b50: 7c0b a00b a100 a00c a100 a00d a100 7d10  |.............}.
-00000b60: 7c0c a00b a100 a00c a100 a00d a100 7d11  |.............}.
-00000b70: 7c0d a00b a100 a00c a100 a00d a100 7d12  |.............}.
-00000b80: 7c03 a00e 7c10 a101 0100 7c04 a00e 7c11  |...|.....|...|.
-00000b90: a101 0100 7c05 a00e 7c12 a101 0100 7c00  ....|...|.....|.
-00000ba0: 6a0f 6a10 7411 6404 8301 1700 7c03 6a12  j.j.t.d.....|.j.
-00000bb0: 6901 7d13 7c00 6a0f 6a10 7411 6405 8301  i.}.|.j.j.t.d...
-00000bc0: 1700 7c04 6a12 6901 7d14 7c00 6a0f 6a10  ..|.j.i.}.|.j.j.
-00000bd0: 7411 6406 8301 1700 7c05 6a12 6901 7d15  t.d.....|.j.i.}.
-00000be0: 7c02 a013 7c13 a101 0100 7c02 a013 7c14  |...|.....|...|.
-00000bf0: a101 0100 7c02 a013 7c15 a101 0100 7c00  ....|...|.....|.
-00000c00: 6a02 4400 5d4e 7d16 7c16 7c0e 7c09 8302  j.D.]N}.|.|.|...
-00000c10: a00b a100 a00c a100 a00d a100 7d17 7c16  ............}.|.
-00000c20: 7c0f 7c0a 8302 a00b a100 a00c a100 a00d  |.|.............
-00000c30: a100 7d18 7c17 7c18 1700 6407 1b00 7d19  ..}.|.|...d...}.
-00000c40: 7c06 7c16 6a10 1900 a00e 7c19 a101 0100  |.|.j.....|.....
-00000c50: 9001 714e 6408 6402 8400 7c06 a014 a100  ..qNd.d...|.....
-00000c60: 4400 8301 7d1a 7c02 a013 7c1a a101 0100  D...}.|...|.....
-00000c70: 7c00 6a07 724e 7c00 a015 7c02 a101 7d1b  |.j.rN|...|...}.
-00000c80: 7c07 a016 7c1b a101 0100 714e 5700 3500  |...|.....qNW.5.
-00000c90: 5100 5200 5800 7c02 5300 2909 4e63 0100  Q.R.X.|.S.).Nc..
-00000ca0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00000cb0: 0000 5300 0000 7316 0000 0069 007c 005d  ..S...s....i.|.]
-00000cc0: 0e7d 017c 016a 0074 0183 0093 0271 0453  .}.|.j.t.....q.S
-00000cd0: 0072 1200 0000 2902 7219 0000 0072 0400  .r....).r....r..
-00000ce0: 0000 2902 7232 0000 0072 2f00 0000 7212  ..).r2...r/...r.
-00000cf0: 0000 0072 1200 0000 7213 0000 00da 0a3c  ...r....r......<
-00000d00: 6469 6374 636f 6d70 3e51 0000 0073 0600  dictcomp>Q...s..
-00000d10: 0000 0600 0200 0400 7a1d 4570 6f63 682e  ........z.Epoch.
-00000d20: 7275 6e2e 3c6c 6f63 616c 733e 2e3c 6469  run.<locals>.<di
-00000d30: 6374 636f 6d70 3e29 03da 0464 6573 63da  ctcomp>)...desc.
-00000d40: 0466 696c 65da 0764 6973 6162 6c65 5a07  .file..disableZ.
-00000d50: 5f62 7265 6173 745a 065f 6465 6e73 655a  _breastZ._denseZ
-00000d60: 095f 7765 6967 6874 6564 7221 0000 0063  ._weightedr!...c
-00000d70: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00000d80: 0400 0000 5300 0000 7318 0000 0069 007c  ....S...s....i.|
-00000d90: 005d 105c 027d 017d 027c 017c 026a 0093  .].\.}.}.|.|.j..
-00000da0: 0271 0453 0072 1200 0000 2901 da04 6d65  .q.S.r....)...me
-00000db0: 616e 7231 0000 0072 1200 0000 7212 0000  anr1...r....r...
-00000dc0: 0072 1300 0000 7240 0000 0074 0000 0073  .r....r@...t...s
-00000dd0: 0600 0000 0600 0600 0200 2917 723f 0000  ..........).r?..
-00000de0: 0072 0400 0000 7229 0000 0072 0200 0000  .r....r)...r....
-00000df0: 722a 0000 00da 0373 7973 da06 7374 646f  r*.....sys..stdo
-00000e00: 7574 722b 0000 0072 2e00 0000 722c 0000  utr+...r....r,..
-00000e10: 0072 3e00 0000 7227 0000 00da 0664 6574  .r>...r'.....det
-00000e20: 6163 68da 056e 756d 7079 da03 6164 6472  ach..numpy..addr
-00000e30: 2500 0000 7219 0000 00da 0373 7472 7244  %...r......strrD
-00000e40: 0000 00da 0675 7064 6174 6572 3600 0000  .....updater6...
-00000e50: 723a 0000 00da 0f73 6574 5f70 6f73 7466  r:.....set_postf
-00000e60: 6978 5f73 7472 291c 720f 0000 00da 0a64  ix_str).r......d
-00000e70: 6174 616c 6f61 6465 7272 3800 0000 5a0b  ataloaderr8...Z.
-00000e80: 6c6f 7373 315f 6d65 7465 725a 0b6c 6f73  loss1_meterZ.los
-00000e90: 7332 5f6d 6574 6572 5a0a 6c6f 7373 5f6d  s2_meterZ.loss_m
-00000ea0: 6574 6572 5a0e 6d65 7472 6963 735f 6d65  eterZ.metrics_me
-00000eb0: 7465 7273 da08 6974 6572 6174 6f72 723c  ters..iteratorr<
-00000ec0: 0000 0072 3d00 0000 da01 7ada 056c 6f73  ...r=.....z..los
-00000ed0: 7331 da05 6c6f 7373 32da 0d77 6569 6768  s1..loss2..weigh
-00000ee0: 7465 645f 6c6f 7373 5a06 795f 7072 6564  ted_lossZ.y_pred
-00000ef0: 5a06 7a5f 7072 6564 5a0b 6c6f 7373 315f  Z.z_predZ.loss1_
-00000f00: 7661 6c75 655a 0b6c 6f73 7332 5f76 616c  valueZ.loss2_val
-00000f10: 7565 5a0a 6c6f 7373 5f76 616c 7565 5a0a  ueZ.loss_valueZ.
-00000f20: 6c6f 7373 315f 6c6f 6773 5a0a 6c6f 7373  loss1_logsZ.loss
-00000f30: 325f 6c6f 6773 5a09 6c6f 7373 5f6c 6f67  2_logsZ.loss_log
-00000f40: 735a 096d 6574 7269 635f 666e 5a0d 6d65  sZ.metric_fnZ.me
-00000f50: 7472 6963 5f76 616c 7565 315a 0d6d 6574  tric_value1Z.met
-00000f60: 7269 635f 7661 6c75 6532 da0c 6d65 7472  ric_value2..metr
-00000f70: 6963 5f76 616c 7565 5a0c 6d65 7472 6963  ic_valueZ.metric
-00000f80: 735f 6c6f 6773 7239 0000 0072 1200 0000  s_logsr9...r....
-00000f90: 7212 0000 0072 1300 0000 da03 7275 6e49  r....r......runI
-00000fa0: 0000 0073 4200 0000 0002 0802 0401 0601  ...sB...........
-00000fb0: 0601 0601 1003 1c01 1001 2801 1803 1001  ..........(.....
-00000fc0: 1001 1002 0a01 0a01 0a02 1601 1601 1602  ................
-00000fd0: 0a01 0a01 0a03 0a01 1601 1602 0c02 1403  ................
-00000fe0: 1203 0a02 0601 0a01 1602 7a09 4570 6f63  ..........z.Epoc
-00000ff0: 682e 7275 6e4e 2902 7227 0000 0054 2909  h.runN).r'...T).
-00001000: 7219 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
-00001010: 0800 0000 722d 0000 0072 3a00 0000 723e  ....r-...r:...r>
-00001020: 0000 0072 3f00 0000 7254 0000 0072 1200  ...r?...rT...r..
-00001030: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00001040: 0072 2600 0000 2c00 0000 730c 0000 0008  .r&...,...s.....
-00001050: 020a 0a08 0608 0508 0308 0372 2600 0000  ...........r&...
-00001060: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00001070: 0004 0000 0000 0000 0073 2e00 0000 6500  .........s....e.
-00001080: 5a01 6400 5a02 6409 8700 6601 6403 6404  Z.d.Z.d...f.d.d.
-00001090: 8409 5a03 6405 6406 8400 5a04 6407 6408  ..Z.d.d...Z.d.d.
-000010a0: 8400 5a05 8700 0400 5a06 5300 290a da0a  ..Z.....Z.S.)...
-000010b0: 5472 6169 6e45 706f 6368 da04 6375 6461  TrainEpoch..cuda
-000010c0: 5463 0800 0000 0000 0000 0000 0000 0800  Tc..............
-000010d0: 0000 0800 0000 0300 0000 7328 0000 0074  ..........s(...t
-000010e0: 0083 006a 017c 017c 027c 0364 017c 067c  ...j.|.|.|.d.|.|
-000010f0: 0764 028d 0601 007c 047c 005f 027c 057c  .d.....|.|._.|.|
-00001100: 005f 0364 0053 0029 034e da05 7472 6169  ._.d.S.).N..trai
-00001110: 6ea9 0672 2800 0000 7225 0000 0072 2900  n..r(...r%...r).
-00001120: 0000 722a 0000 0072 2c00 0000 722b 0000  ..r*...r,...r+..
-00001130: 0029 0472 0700 0000 7208 0000 00da 096f  .).r....r......o
-00001140: 7074 696d 697a 6572 da0c 6c72 5f73 6368  ptimizer..lr_sch
-00001150: 6564 756c 6172 2908 720f 0000 0072 2800  edular).r....r(.
-00001160: 0000 7225 0000 0072 2900 0000 7259 0000  ..r%...r)...rY..
-00001170: 0072 5a00 0000 722c 0000 0072 2b00 0000  .rZ...r,...r+...
-00001180: 7210 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-00001190: 0800 0000 8200 0000 7314 0000 0000 0106  ........s.......
-000011a0: 0102 0102 0102 0102 0102 0102 fa06 0806  ................
-000011b0: 017a 1354 7261 696e 4570 6f63 682e 5f5f  .z.TrainEpoch.__
-000011c0: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
-000011d0: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
-000011e0: 0e00 0000 7c00 6a00 a001 a100 0100 6400  ....|.j.......d.
-000011f0: 5300 7206 0000 0029 0272 2800 0000 7257  S.r....).r(...rW
-00001200: 0000 0072 2000 0000 7212 0000 0072 1200  ...r ...r....r..
-00001210: 0000 7213 0000 0072 3f00 0000 9000 0000  ..r....r?.......
-00001220: 7302 0000 0000 017a 1954 7261 696e 4570  s......z.TrainEp
-00001230: 6f63 682e 6f6e 5f65 706f 6368 5f73 7461  och.on_epoch_sta
-00001240: 7274 6304 0000 0000 0000 0000 0000 0009  rtc.............
-00001250: 0000 0005 0000 0043 0000 0073 6200 0000  .......C...sb...
-00001260: 7c00 6a00 a001 a100 0100 7c00 6a02 a003  |.j.......|.j...
-00001270: 7c01 a101 5c02 7d04 7d05 7c00 a004 7c04  |...\.}.}.|...|.
-00001280: 7c02 a102 7d06 7c00 a004 7c05 7c03 a102  |...}.|...|.|...
-00001290: 7d07 6401 7c06 1400 6401 7c07 1400 1700  }.d.|...d.|.....
-000012a0: 7d08 7c08 a005 a100 0100 7c00 6a00 a006  }.|.......|.j...
-000012b0: a100 0100 7c06 7c07 7c08 7c04 7c05 6605  ....|.|.|.|.|.f.
-000012c0: 5300 a902 4e67 0000 0000 0000 e03f 2907  S...Ng.......?).
-000012d0: 7259 0000 00da 097a 6572 6f5f 6772 6164  rY.....zero_grad
-000012e0: 7228 0000 0072 1700 0000 7225 0000 00da  r(...r....r%....
-000012f0: 0862 6163 6b77 6172 64da 0473 7465 70a9  .backward..step.
-00001300: 0972 0f00 0000 723c 0000 0072 3d00 0000  .r....r<...r=...
-00001310: 724f 0000 005a 0b70 7265 6469 6374 696f  rO...Z.predictio
-00001320: 6e31 5a0b 7072 6564 6963 7469 6f6e 3272  n1Z.prediction2r
-00001330: 5000 0000 7251 0000 0072 5200 0000 7212  P...rQ...rR...r.
-00001340: 0000 0072 1200 0000 7213 0000 0072 3e00  ...r....r....r>.
-00001350: 0000 9300 0000 7310 0000 0000 010a 0110  ......s.........
-00001360: 010c 010c 0410 0508 010a 027a 1754 7261  ...........z.Tra
-00001370: 696e 4570 6f63 682e 6261 7463 685f 7570  inEpoch.batch_up
-00001380: 6461 7465 2902 7256 0000 0054 a907 7219  date).rV...T..r.
-00001390: 0000 0072 1a00 0000 721b 0000 0072 0800  ...r....r....r..
-000013a0: 0000 723f 0000 0072 3e00 0000 721c 0000  ..r?...r>...r...
-000013b0: 0072 1200 0000 7212 0000 0072 1000 0000  .r....r....r....
-000013c0: 7213 0000 0072 5500 0000 8000 0000 7306  r....rU.......s.
-000013d0: 0000 0008 020e 0e08 0372 5500 0000 6300  .........rU...c.
-000013e0: 0000 0000 0000 0000 0000 0000 0000 0004  ................
-000013f0: 0000 0000 0000 0073 2e00 0000 6500 5a01  .......s....e.Z.
-00001400: 6400 5a02 6409 8700 6601 6403 6404 8409  d.Z.d...f.d.d...
-00001410: 5a03 6405 6406 8400 5a04 6407 6408 8400  Z.d.d...Z.d.d...
-00001420: 5a05 8700 0400 5a06 5300 290a da0a 5661  Z.....Z.S.)...Va
-00001430: 6c69 6445 706f 6368 7256 0000 0054 6306  lidEpochrV...Tc.
-00001440: 0000 0000 0000 0000 0000 0006 0000 0008  ................
-00001450: 0000 0003 0000 0073 1c00 0000 7400 8300  .......s....t...
-00001460: 6a01 7c01 7c02 7c03 6401 7c04 7c05 6402  j.|.|.|.d.|.|.d.
-00001470: 8d06 0100 6400 5300 2903 4eda 0576 616c  ....d.S.).N..val
-00001480: 6964 7258 0000 0029 0272 0700 0000 7208  idrX...).r....r.
-00001490: 0000 0029 0672 0f00 0000 7228 0000 0072  ...).r....r(...r
-000014a0: 2500 0000 7229 0000 0072 2c00 0000 722b  %...r)...r,...r+
-000014b0: 0000 0072 1000 0000 7212 0000 0072 1300  ...r....r....r..
-000014c0: 0000 7208 0000 00a8 0000 0073 1000 0000  ..r........s....
-000014d0: 0001 0601 0201 0201 0201 0201 0201 02fa  ................
-000014e0: 7a13 5661 6c69 6445 706f 6368 2e5f 5f69  z.ValidEpoch.__i
-000014f0: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
-00001500: 0000 0100 0000 0200 0000 4300 0000 730e  ..........C...s.
-00001510: 0000 007c 006a 00a0 01a1 0001 0064 0053  ...|.j.......d.S
-00001520: 0072 0600 0000 2902 7228 0000 00da 0465  .r....).r(.....e
-00001530: 7661 6c72 2000 0000 7212 0000 0072 1200  valr ...r....r..
-00001540: 0000 7213 0000 0072 3f00 0000 b200 0000  ..r....r?.......
-00001550: 7302 0000 0000 017a 1956 616c 6964 4570  s......z.ValidEp
-00001560: 6f63 682e 6f6e 5f65 706f 6368 5f73 7461  och.on_epoch_sta
-00001570: 7274 6304 0000 0000 0000 0000 0000 0009  rtc.............
-00001580: 0000 0009 0000 0043 0000 0073 5a00 0000  .......C...sZ...
-00001590: 7400 a001 a100 8f3e 0100 7c00 6a02 a003  t......>..|.j...
-000015a0: 7c01 a101 5c02 7d04 7d05 7c00 a004 7c04  |...\.}.}.|...|.
-000015b0: 7c02 a102 7d06 7c00 a004 7c05 7c03 a102  |...}.|...|.|...
-000015c0: 7d07 6401 7c06 1400 6401 7c07 1400 1700  }.d.|...d.|.....
-000015d0: 7d08 5700 3500 5100 5200 5800 7c06 7c07  }.W.5.Q.R.X.|.|.
-000015e0: 7c08 7c04 7c05 6605 5300 725b 0000 0029  |.|.|.f.S.r[...)
-000015f0: 0572 0c00 0000 da07 6e6f 5f67 7261 6472  .r......no_gradr
-00001600: 2800 0000 7217 0000 0072 2500 0000 725f  (...r....r%...r_
-00001610: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
-00001620: 0000 723e 0000 00b5 0000 0073 0c00 0000  ..r>.......s....
-00001630: 0001 0a01 1001 0c01 0c04 1a04 7a17 5661  ............z.Va
-00001640: 6c69 6445 706f 6368 2e62 6174 6368 5f75  lidEpoch.batch_u
-00001650: 7064 6174 6529 0272 5600 0000 5472 6000  pdate).rV...Tr`.
-00001660: 0000 7212 0000 0072 1200 0000 7210 0000  ..r....r....r...
-00001670: 0072 1300 0000 7261 0000 00a6 0000 0073  .r....ra.......s
-00001680: 0600 0000 0802 0e0a 0803 7261 0000 0029  ..........ra...)
-00001690: 1272 4500 0000 720c 0000 005a 0b74 6f72  .rE...r....Z.tor
-000016a0: 6368 2e6f 7074 696d da05 6f70 7469 6dda  ch.optim..optim.
-000016b0: 0874 6f72 6368 2e6e 6e72 0a00 0000 7248  .torch.nnr....rH
-000016c0: 0000 00da 026e 7072 0200 0000 5a05 6d65  .....npr....Z.me
-000016d0: 7465 7272 0400 0000 da06 4d6f 6475 6c65  terr......Module
-000016e0: 7205 0000 0072 1d00 0000 5a0e 6d75 6c74  r....r....Z.mult
-000016f0: 6974 6173 6b5f 6c6f 7373 7226 0000 0072  itask_lossr&...r
-00001700: 5500 0000 7261 0000 0072 1200 0000 7212  U...ra...r....r.
-00001710: 0000 0072 1200 0000 7213 0000 00da 083c  ...r....r......<
-00001720: 6d6f 6475 6c65 3e01 0000 0073 1800 0000  module>....s....
-00001730: 0801 0801 0c01 0c01 0801 0c01 0c02 1210  ................
-00001740: 1211 0a02 0e54 1026                      .....T.&
+00000220: 6e61 6e5c 6d67 5c73 6567 6d65 6e74 6174  nan\mg\segmentat
+00000230: 696f 6e5f 6d6f 6465 6c73 5c75 7469 6c73  ion_models\utils
+00000240: 5c74 7261 696e 2e70 7972 0800 0000 0a00  \train.pyr......
+00000250: 0000 7306 0000 0000 010e 0106 017a 1557  ..s..........z.W
+00000260: 6569 6768 7465 644c 6f73 732e 5f5f 696e  eightedLoss.__in
+00000270: 6974 5f5f 6303 0000 0000 0000 0000 0000  it__c...........
+00000280: 0005 0000 0004 0000 0043 0000 0073 5000  .........C...sP.
+00000290: 0000 7400 a001 7c00 6a02 6401 1900 0b00  ..t...|.j.d.....
+000002a0: a101 7d03 7c03 7c01 1400 7c00 6a02 6401  ..}.|.|...|.j.d.
+000002b0: 1900 1700 7d01 7400 a001 7c00 6a02 6402  ....}.t...|.j.d.
+000002c0: 1900 0b00 a101 7d04 7c04 7c02 1400 7c00  ......}.|.|...|.
+000002d0: 6a02 6402 1900 1700 7d02 7c01 7c02 1700  j.d.....}.|.|...
+000002e0: 5300 2903 4e72 0100 0000 7203 0000 0029  S.).Nr....r....)
+000002f0: 0372 0c00 0000 da03 6578 7072 0e00 0000  .r......expr....
+00000300: 2905 720f 0000 00da 066c 6f73 735f 31da  ).r......loss_1.
+00000310: 066c 6f73 735f 325a 0b70 7265 6369 7369  .loss_2Z.precisi
+00000320: 6f6e 5f31 5a0b 7072 6563 6973 696f 6e5f  on_1Z.precision_
+00000330: 3272 1200 0000 7212 0000 0072 1300 0000  2r....r....r....
+00000340: da07 666f 7277 6172 640f 0000 0073 0a00  ..forward....s..
+00000350: 0000 0001 1201 1202 1201 1202 7a14 5765  ............z.We
+00000360: 6967 6874 6564 4c6f 7373 2e66 6f72 7761  ightedLoss.forwa
+00000370: 7264 a906 da08 5f5f 6e61 6d65 5f5f da0a  rd....__name__..
+00000380: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000390: 616c 6e61 6d65 5f5f 7208 0000 0072 1700  alname__r....r..
+000003a0: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
+000003b0: 5f72 1200 0000 7212 0000 0072 1000 0000  _r....r....r....
+000003c0: 7213 0000 0072 0500 0000 0900 0000 7304  r....r........s.
+000003d0: 0000 0008 010c 0572 0500 0000 6300 0000  .......r....c...
+000003e0: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+000003f0: 0000 0000 0073 2400 0000 6500 5a01 6400  .....s$...e.Z.d.
+00000400: 5a02 8700 6601 6401 6402 8408 5a03 6403  Z...f.d.d...Z.d.
+00000410: 6404 8400 5a04 8700 0400 5a05 5300 2905  d...Z.....Z.S.).
+00000420: da0d 4d75 6c74 6954 6173 6b4c 6f73 7363  ..MultiTaskLossc
+00000430: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000440: 0500 0000 0300 0000 7336 0000 0074 0074  ........s6...t.t
+00000450: 017c 0083 02a0 02a1 0001 0074 03a0 0474  .|.........t...t
+00000460: 05a0 0664 01a1 01a1 017c 005f 0774 03a0  ...d.....|._.t..
+00000470: 0474 05a0 0664 01a1 01a1 017c 005f 0864  .t...d.....|._.d
+00000480: 0053 0029 024e 7203 0000 0029 0972 0700  .S.).Nr....).r..
+00000490: 0000 721d 0000 0072 0800 0000 720a 0000  ..r....r....r...
+000004a0: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+000004b0: da07 7369 676d 615f 31da 0773 6967 6d61  ..sigma_1..sigma
+000004c0: 5f32 a901 720f 0000 0072 1000 0000 7212  _2..r....r....r.
+000004d0: 0000 0072 1300 0000 7208 0000 001a 0000  ...r....r.......
+000004e0: 0073 0600 0000 0001 0e02 1201 7a16 4d75  .s..........z.Mu
+000004f0: 6c74 6954 6173 6b4c 6f73 732e 5f5f 696e  ltiTaskLoss.__in
+00000500: 6974 5f5f 6303 0000 0000 0000 0000 0000  it__c...........
+00000510: 0006 0000 0003 0000 0043 0000 0073 4000  .........C...s@.
+00000520: 0000 7400 a001 7c01 a101 7c00 6a02 6401  ..t...|...|.j.d.
+00000530: 1300 1b00 7c00 6a02 1700 7d03 7400 a001  ....|.j...}.t...
+00000540: 7c02 a101 7c00 6a03 6401 1300 1b00 7c00  |...|.j.d.....|.
+00000550: 6a03 1700 7d04 7c03 7c04 1700 7d05 7c05  j...}.|.|...}.|.
+00000560: 5300 2902 4ee9 0200 0000 2904 720c 0000  S.).N.....).r...
+00000570: 00da 0654 656e 736f 7272 1e00 0000 721f  ...Tensorr....r.
+00000580: 0000 0029 0672 0f00 0000 7215 0000 0072  ...).r....r....r
+00000590: 1600 0000 da02 6c31 da02 6c32 da04 6c6f  ......l1..l2..lo
+000005a0: 7373 7212 0000 0072 1200 0000 7213 0000  ssr....r....r...
+000005b0: 0072 1700 0000 2100 0000 7308 0000 0000  .r....!...s.....
+000005c0: 031a 011a 0108 017a 154d 756c 7469 5461  .......z.MultiTa
+000005d0: 736b 4c6f 7373 2e66 6f72 7761 7264 7218  skLoss.forwardr.
+000005e0: 0000 0072 1200 0000 7212 0000 0072 1000  ...r....r....r..
+000005f0: 0000 7213 0000 0072 1d00 0000 1900 0000  ..r....r........
+00000600: 7304 0000 0008 010c 0772 1d00 0000 7221  s........r....r!
+00000610: 0000 0029 0172 0900 0000 6300 0000 0000  ...).r....c.....
+00000620: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+00000630: 0000 0073 3e00 0000 6500 5a01 6400 5a02  ...s>...e.Z.d.Z.
+00000640: 6410 6403 6404 8401 5a03 6405 6406 8400  d.d.d...Z.d.d...
+00000650: 5a04 6407 6408 8400 5a05 6409 640a 8400  Z.d.d...Z.d.d...
+00000660: 5a06 640b 640c 8400 5a07 640d 640e 8400  Z.d.d...Z.d.d...
+00000670: 5a08 640f 5300 2911 da05 4570 6f63 68da  Z.d.S.)...Epoch.
+00000680: 0363 7075 5463 0700 0000 0000 0000 0000  .cpuTc..........
+00000690: 0000 0700 0000 0200 0000 4300 0000 7330  ..........C...s0
+000006a0: 0000 007c 017c 005f 007c 027c 005f 017c  ...|.|._.|.|._.|
+000006b0: 037c 005f 027c 047c 005f 037c 067c 005f  .|._.|.|._.|.|._
+000006c0: 047c 057c 005f 057c 00a0 06a1 0001 0064  .|.|._.|.......d
+000006d0: 0053 0072 0600 0000 2907 da05 6d6f 6465  .S.r....)...mode
+000006e0: 6c72 2500 0000 da07 6d65 7472 6963 73da  lr%.....metrics.
+000006f0: 0a73 7461 6765 5f6e 616d 65da 0776 6572  .stage_name..ver
+00000700: 626f 7365 da06 6465 7669 6365 da0a 5f74  bose..device.._t
+00000710: 6f5f 6465 7669 6365 2907 720f 0000 0072  o_device).r....r
+00000720: 2800 0000 7225 0000 0072 2900 0000 722a  (...r%...r)...r*
+00000730: 0000 0072 2c00 0000 722b 0000 0072 1200  ...r,...r+...r..
+00000740: 0000 7212 0000 0072 1300 0000 7208 0000  ..r....r....r...
+00000750: 002e 0000 0073 0e00 0000 0001 0601 0601  .....s..........
+00000760: 0601 0601 0601 0602 7a0e 4570 6f63 682e  ........z.Epoch.
+00000770: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
+00000780: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+00000790: 0073 3800 0000 7c00 6a00 a001 7c00 6a02  .s8...|.j...|.j.
+000007a0: a101 0100 7c00 6a03 a001 7c00 6a02 a101  ....|.j...|.j...
+000007b0: 0100 7c00 6a04 4400 5d10 7d01 7c01 a001  ..|.j.D.].}.|...
+000007c0: 7c00 6a02 a101 0100 7122 6400 5300 7206  |.j.....q"d.S.r.
+000007d0: 0000 0029 0572 2800 0000 da02 746f 722c  ...).r(.....tor,
+000007e0: 0000 0072 2500 0000 7229 0000 0029 0272  ...r%...r)...).r
+000007f0: 0f00 0000 da06 6d65 7472 6963 7212 0000  ......metricr...
+00000800: 0072 1200 0000 7213 0000 0072 2d00 0000  .r....r....r-...
+00000810: 3800 0000 7308 0000 0000 010e 010e 010a  8...s...........
+00000820: 017a 1045 706f 6368 2e5f 746f 5f64 6576  .z.Epoch._to_dev
+00000830: 6963 6563 0200 0000 0000 0000 0000 0000  icec............
+00000840: 0400 0000 0300 0000 4300 0000 7320 0000  ........C...s ..
+00000850: 0064 0164 0284 007c 01a0 00a1 0044 0083  .d.d...|.....D..
+00000860: 017d 0264 03a0 017c 02a1 017d 037c 0353  .}.d...|...}.|.S
+00000870: 0029 044e 6301 0000 0000 0000 0000 0000  .).Nc...........
+00000880: 0003 0000 0006 0000 0053 0000 0073 1c00  .........S...s..
+00000890: 0000 6700 7c00 5d14 5c02 7d01 7d02 6400  ..g.|.].\.}.}.d.
+000008a0: a000 7c01 7c02 a102 9102 7104 5300 2901  ..|.|.....q.S.).
+000008b0: 7a0a 7b7d 202d 207b 3a2e 347d 2901 da06  z.{} - {:.4})...
+000008c0: 666f 726d 6174 a903 da02 2e30 da01 6bda  format.....0..k.
+000008d0: 0176 7212 0000 0072 1200 0000 7213 0000  .vr....r....r...
+000008e0: 00da 0a3c 6c69 7374 636f 6d70 3e3f 0000  ...<listcomp>?..
+000008f0: 0073 0400 0000 0600 0600 7a26 4570 6f63  .s........z&Epoc
+00000900: 682e 5f66 6f72 6d61 745f 6c6f 6773 2e3c  h._format_logs.<
+00000910: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00000920: 703e 7a02 2c20 2902 da05 6974 656d 73da  p>z., )...items.
+00000930: 046a 6f69 6e29 0472 0f00 0000 da04 6c6f  .join).r......lo
+00000940: 6773 5a08 7374 725f 6c6f 6773 da01 7372  gsZ.str_logs..sr
+00000950: 1200 0000 7212 0000 0072 1300 0000 da0c  ....r....r......
+00000960: 5f66 6f72 6d61 745f 6c6f 6773 3e00 0000  _format_logs>...
+00000970: 7306 0000 0000 0112 010a 017a 1245 706f  s..........z.Epo
+00000980: 6368 2e5f 666f 726d 6174 5f6c 6f67 7363  ch._format_logsc
+00000990: 0300 0000 0000 0000 0000 0000 0300 0000  ................
+000009a0: 0100 0000 4300 0000 7308 0000 0074 0082  ....C...s....t..
+000009b0: 0164 0053 0072 0600 0000 2901 da13 4e6f  .d.S.r....)...No
+000009c0: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
+000009d0: 7229 0372 0f00 0000 da01 78da 0179 7212  r).r......x..yr.
+000009e0: 0000 0072 1200 0000 7213 0000 00da 0c62  ...r....r......b
+000009f0: 6174 6368 5f75 7064 6174 6543 0000 0073  atch_updateC...s
+00000a00: 0200 0000 0001 7a12 4570 6f63 682e 6261  ......z.Epoch.ba
+00000a10: 7463 685f 7570 6461 7465 6301 0000 0000  tch_updatec.....
+00000a20: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
+00000a30: 0000 0073 0400 0000 6400 5300 7206 0000  ...s....d.S.r...
+00000a40: 0072 1200 0000 7220 0000 0072 1200 0000  .r....r ...r....
+00000a50: 7212 0000 0072 1300 0000 da0e 6f6e 5f65  r....r......on_e
+00000a60: 706f 6368 5f73 7461 7274 4600 0000 7302  poch_startF...s.
+00000a70: 0000 0000 017a 1445 706f 6368 2e6f 6e5f  .....z.Epoch.on_
+00000a80: 6570 6f63 685f 7374 6172 7463 0200 0000  epoch_startc....
+00000a90: 0000 0000 0000 0000 1c00 0000 0900 0000  ................
+00000aa0: 4300 0000 73e4 0100 007c 00a0 00a1 0001  C...s....|......
+00000ab0: 0069 007d 0274 0183 007d 0374 0183 007d  .i.}.t...}.t...}
+00000ac0: 0474 0183 007d 0564 0164 0284 007c 006a  .t...}.d.d...|.j
+00000ad0: 0244 0083 017d 0674 037c 017c 006a 0474  .D...}.t.|.|.j.t
+00000ae0: 056a 067c 006a 070c 0064 038d 0490 018f  .j.|.j...d......
+00000af0: 927d 077c 0744 0090 015d 845c 037d 087d  .}.|.D...].\.}.}
+00000b00: 097d 0a7c 08a0 087c 006a 09a1 017c 09a0  .}.|...|.j...|..
+00000b10: 087c 006a 09a1 017c 0aa0 087c 006a 09a1  .|.j...|...|.j..
+00000b20: 0103 0002 007d 087d 097d 0a7c 00a0 0a7c  .....}.}.}.|...|
+00000b30: 087c 097c 0aa1 035c 057d 0b7d 0c7d 0d7d  .|.|...\.}.}.}.}
+00000b40: 0e7d 0f7c 0ba0 0ba1 00a0 0ca1 00a0 0da1  .}.|............
+00000b50: 007d 107c 0ca0 0ba1 00a0 0ca1 00a0 0da1  .}.|............
+00000b60: 007d 117c 0da0 0ba1 00a0 0ca1 00a0 0da1  .}.|............
+00000b70: 007d 127c 03a0 0e7c 10a1 0101 007c 04a0  .}.|...|.....|..
+00000b80: 0e7c 11a1 0101 007c 05a0 0e7c 12a1 0101  .|.....|...|....
+00000b90: 007c 006a 0f6a 1074 1164 0483 0117 007c  .|.j.j.t.d.....|
+00000ba0: 036a 1269 017d 137c 006a 0f6a 1074 1164  .j.i.}.|.j.j.t.d
+00000bb0: 0583 0117 007c 046a 1269 017d 147c 006a  .....|.j.i.}.|.j
+00000bc0: 0f6a 1074 1164 0683 0117 007c 056a 1269  .j.t.d.....|.j.i
+00000bd0: 017d 157c 02a0 137c 13a1 0101 007c 02a0  .}.|...|.....|..
+00000be0: 137c 14a1 0101 007c 02a0 137c 15a1 0101  .|.....|...|....
+00000bf0: 007c 006a 0244 005d 4e7d 167c 167c 0e7c  .|.j.D.]N}.|.|.|
+00000c00: 0983 02a0 0ba1 00a0 0ca1 00a0 0da1 007d  ...............}
+00000c10: 177c 167c 0f7c 0a83 02a0 0ba1 00a0 0ca1  .|.|.|..........
+00000c20: 00a0 0da1 007d 187c 177c 1817 0064 071b  .....}.|.|...d..
+00000c30: 007d 197c 067c 166a 1019 00a0 0e7c 19a1  .}.|.|.j.....|..
+00000c40: 0101 0090 0171 4e64 0864 0284 007c 06a0  .....qNd.d...|..
+00000c50: 14a1 0044 0083 017d 1a7c 02a0 137c 1aa1  ...D...}.|...|..
+00000c60: 0101 007c 006a 0772 4e7c 00a0 157c 02a1  ...|.j.rN|...|..
+00000c70: 017d 1b7c 07a0 167c 1ba1 0101 0071 4e57  .}.|...|.....qNW
+00000c80: 0035 0051 0052 0058 007c 0253 0029 094e  .5.Q.R.X.|.S.).N
+00000c90: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000ca0: 0004 0000 0053 0000 0073 1600 0000 6900  .....S...s....i.
+00000cb0: 7c00 5d0e 7d01 7c01 6a00 7401 8300 9302  |.].}.|.j.t.....
+00000cc0: 7104 5300 7212 0000 0029 0272 1900 0000  q.S.r....).r....
+00000cd0: 7204 0000 0029 0272 3200 0000 722f 0000  r....).r2...r/..
+00000ce0: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
+00000cf0: da0a 3c64 6963 7463 6f6d 703e 5100 0000  ..<dictcomp>Q...
+00000d00: 7306 0000 0006 0002 0004 007a 1d45 706f  s..........z.Epo
+00000d10: 6368 2e72 756e 2e3c 6c6f 6361 6c73 3e2e  ch.run.<locals>.
+00000d20: 3c64 6963 7463 6f6d 703e 2903 da04 6465  <dictcomp>)...de
+00000d30: 7363 da04 6669 6c65 da07 6469 7361 626c  sc..file..disabl
+00000d40: 655a 075f 6272 6561 7374 5a06 5f64 656e  eZ._breastZ._den
+00000d50: 7365 5a09 5f77 6569 6768 7465 6472 2100  seZ._weightedr!.
+00000d60: 0000 6301 0000 0000 0000 0000 0000 0003  ..c.............
+00000d70: 0000 0004 0000 0053 0000 0073 1800 0000  .......S...s....
+00000d80: 6900 7c00 5d10 5c02 7d01 7d02 7c01 7c02  i.|.].\.}.}.|.|.
+00000d90: 6a00 9302 7104 5300 7212 0000 0029 01da  j...q.S.r....)..
+00000da0: 046d 6561 6e72 3100 0000 7212 0000 0072  .meanr1...r....r
+00000db0: 1200 0000 7213 0000 0072 4000 0000 7400  ....r....r@...t.
+00000dc0: 0000 7306 0000 0006 0006 0002 0029 1772  ..s..........).r
+00000dd0: 3f00 0000 7204 0000 0072 2900 0000 7202  ?...r....r)...r.
+00000de0: 0000 0072 2a00 0000 da03 7379 73da 0673  ...r*.....sys..s
+00000df0: 7464 6f75 7472 2b00 0000 722e 0000 0072  tdoutr+...r....r
+00000e00: 2c00 0000 723e 0000 0072 2700 0000 da06  ,...r>...r'.....
+00000e10: 6465 7461 6368 da05 6e75 6d70 79da 0361  detach..numpy..a
+00000e20: 6464 7225 0000 0072 1900 0000 da03 7374  ddr%...r......st
+00000e30: 7272 4400 0000 da06 7570 6461 7465 7236  rrD.....updater6
+00000e40: 0000 0072 3a00 0000 da0f 7365 745f 706f  ...r:.....set_po
+00000e50: 7374 6669 785f 7374 7229 1c72 0f00 0000  stfix_str).r....
+00000e60: da0a 6461 7461 6c6f 6164 6572 7238 0000  ..dataloaderr8..
+00000e70: 005a 0b6c 6f73 7331 5f6d 6574 6572 5a0b  .Z.loss1_meterZ.
+00000e80: 6c6f 7373 325f 6d65 7465 725a 0a6c 6f73  loss2_meterZ.los
+00000e90: 735f 6d65 7465 725a 0e6d 6574 7269 6373  s_meterZ.metrics
+00000ea0: 5f6d 6574 6572 73da 0869 7465 7261 746f  _meters..iterato
+00000eb0: 7272 3c00 0000 723d 0000 00da 017a da05  rr<...r=.....z..
+00000ec0: 6c6f 7373 31da 056c 6f73 7332 da0d 7765  loss1..loss2..we
+00000ed0: 6967 6874 6564 5f6c 6f73 735a 0679 5f70  ighted_lossZ.y_p
+00000ee0: 7265 645a 067a 5f70 7265 645a 0b6c 6f73  redZ.z_predZ.los
+00000ef0: 7331 5f76 616c 7565 5a0b 6c6f 7373 325f  s1_valueZ.loss2_
+00000f00: 7661 6c75 655a 0a6c 6f73 735f 7661 6c75  valueZ.loss_valu
+00000f10: 655a 0a6c 6f73 7331 5f6c 6f67 735a 0a6c  eZ.loss1_logsZ.l
+00000f20: 6f73 7332 5f6c 6f67 735a 096c 6f73 735f  oss2_logsZ.loss_
+00000f30: 6c6f 6773 5a09 6d65 7472 6963 5f66 6e5a  logsZ.metric_fnZ
+00000f40: 0d6d 6574 7269 635f 7661 6c75 6531 5a0d  .metric_value1Z.
+00000f50: 6d65 7472 6963 5f76 616c 7565 32da 0c6d  metric_value2..m
+00000f60: 6574 7269 635f 7661 6c75 655a 0c6d 6574  etric_valueZ.met
+00000f70: 7269 6373 5f6c 6f67 7372 3900 0000 7212  rics_logsr9...r.
+00000f80: 0000 0072 1200 0000 7213 0000 00da 0372  ...r....r......r
+00000f90: 756e 4900 0000 7342 0000 0000 0208 0204  unI...sB........
+00000fa0: 0106 0106 0106 0110 031c 0110 0128 0118  .............(..
+00000fb0: 0310 0110 0110 020a 010a 010a 0216 0116  ................
+00000fc0: 0116 020a 010a 010a 030a 0116 0116 020c  ................
+00000fd0: 0214 0312 030a 0206 010a 0116 027a 0945  .............z.E
+00000fe0: 706f 6368 2e72 756e 4e29 0272 2700 0000  poch.runN).r'...
+00000ff0: 5429 0972 1900 0000 721a 0000 0072 1b00  T).r....r....r..
+00001000: 0000 7208 0000 0072 2d00 0000 723a 0000  ..r....r-...r:..
+00001010: 0072 3e00 0000 723f 0000 0072 5400 0000  .r>...r?...rT...
+00001020: 7212 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+00001030: 1300 0000 7226 0000 002c 0000 0073 0c00  ....r&...,...s..
+00001040: 0000 0802 0a0a 0806 0805 0803 0803 7226  ..............r&
+00001050: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00001060: 0000 0000 0400 0000 0000 0000 732e 0000  ............s...
+00001070: 0065 005a 0164 005a 0264 0987 0066 0164  .e.Z.d.Z.d...f.d
+00001080: 0364 0484 095a 0364 0564 0684 005a 0464  .d...Z.d.d...Z.d
+00001090: 0764 0884 005a 0587 0004 005a 0653 0029  .d...Z.....Z.S.)
+000010a0: 0ada 0a54 7261 696e 4570 6f63 68da 0463  ...TrainEpoch..c
+000010b0: 7564 6154 6308 0000 0000 0000 0000 0000  udaTc...........
+000010c0: 0008 0000 0008 0000 0003 0000 0073 2800  .............s(.
+000010d0: 0000 7400 8300 6a01 7c01 7c02 7c03 6401  ..t...j.|.|.|.d.
+000010e0: 7c06 7c07 6402 8d06 0100 7c04 7c00 5f02  |.|.d.....|.|._.
+000010f0: 7c05 7c00 5f03 6400 5300 2903 4eda 0574  |.|._.d.S.).N..t
+00001100: 7261 696e a906 7228 0000 0072 2500 0000  rain..r(...r%...
+00001110: 7229 0000 0072 2a00 0000 722c 0000 0072  r)...r*...r,...r
+00001120: 2b00 0000 2904 7207 0000 0072 0800 0000  +...).r....r....
+00001130: da09 6f70 7469 6d69 7a65 72da 0c6c 725f  ..optimizer..lr_
+00001140: 7363 6865 6475 6c61 7229 0872 0f00 0000  schedular).r....
+00001150: 7228 0000 0072 2500 0000 7229 0000 0072  r(...r%...r)...r
+00001160: 5900 0000 725a 0000 0072 2c00 0000 722b  Y...rZ...r,...r+
+00001170: 0000 0072 1000 0000 7212 0000 0072 1300  ...r....r....r..
+00001180: 0000 7208 0000 0082 0000 0073 1400 0000  ..r........s....
+00001190: 0001 0601 0201 0201 0201 0201 0201 02fa  ................
+000011a0: 0608 0601 7a13 5472 6169 6e45 706f 6368  ....z.TrainEpoch
+000011b0: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
+000011c0: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
+000011d0: 0000 730e 0000 007c 006a 00a0 01a1 0001  ..s....|.j......
+000011e0: 0064 0053 0072 0600 0000 2902 7228 0000  .d.S.r....).r(..
+000011f0: 0072 5700 0000 7220 0000 0072 1200 0000  .rW...r ...r....
+00001200: 7212 0000 0072 1300 0000 723f 0000 0090  r....r....r?....
+00001210: 0000 0073 0200 0000 0001 7a19 5472 6169  ...s......z.Trai
+00001220: 6e45 706f 6368 2e6f 6e5f 6570 6f63 685f  nEpoch.on_epoch_
+00001230: 7374 6172 7463 0400 0000 0000 0000 0000  startc..........
+00001240: 0000 0900 0000 0500 0000 4300 0000 7362  ..........C...sb
+00001250: 0000 007c 006a 00a0 01a1 0001 007c 006a  ...|.j.......|.j
+00001260: 02a0 037c 01a1 015c 027d 047d 057c 00a0  ...|...\.}.}.|..
+00001270: 047c 047c 02a1 027d 067c 00a0 047c 057c  .|.|...}.|...|.|
+00001280: 03a1 027d 0764 017c 0614 0064 017c 0714  ...}.d.|...d.|..
+00001290: 0017 007d 087c 08a0 05a1 0001 007c 006a  ...}.|.......|.j
+000012a0: 00a0 06a1 0001 007c 067c 077c 087c 047c  .......|.|.|.|.|
+000012b0: 0566 0553 00a9 024e 6700 0000 0000 00e0  .f.S...Ng.......
+000012c0: 3f29 0772 5900 0000 da09 7a65 726f 5f67  ?).rY.....zero_g
+000012d0: 7261 6472 2800 0000 7217 0000 0072 2500  radr(...r....r%.
+000012e0: 0000 da08 6261 636b 7761 7264 da04 7374  ....backward..st
+000012f0: 6570 a909 720f 0000 0072 3c00 0000 723d  ep..r....r<...r=
+00001300: 0000 0072 4f00 0000 5a0b 7072 6564 6963  ...rO...Z.predic
+00001310: 7469 6f6e 315a 0b70 7265 6469 6374 696f  tion1Z.predictio
+00001320: 6e32 7250 0000 0072 5100 0000 7252 0000  n2rP...rQ...rR..
+00001330: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
+00001340: 723e 0000 0093 0000 0073 1000 0000 0001  r>.......s......
+00001350: 0a01 1001 0c01 0c04 1005 0801 0a02 7a17  ..............z.
+00001360: 5472 6169 6e45 706f 6368 2e62 6174 6368  TrainEpoch.batch
+00001370: 5f75 7064 6174 6529 0272 5600 0000 54a9  _update).rV...T.
+00001380: 0772 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00001390: 7208 0000 0072 3f00 0000 723e 0000 0072  r....r?...r>...r
+000013a0: 1c00 0000 7212 0000 0072 1200 0000 7210  ....r....r....r.
+000013b0: 0000 0072 1300 0000 7255 0000 0080 0000  ...r....rU......
+000013c0: 0073 0600 0000 0802 0e0e 0803 7255 0000  .s..........rU..
+000013d0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+000013e0: 0000 0400 0000 0000 0000 732e 0000 0065  ..........s....e
+000013f0: 005a 0164 005a 0264 0987 0066 0164 0364  .Z.d.Z.d...f.d.d
+00001400: 0484 095a 0364 0564 0684 005a 0464 0764  ...Z.d.d...Z.d.d
+00001410: 0884 005a 0587 0004 005a 0653 0029 0ada  ...Z.....Z.S.)..
+00001420: 0a56 616c 6964 4570 6f63 6872 5600 0000  .ValidEpochrV...
+00001430: 5463 0600 0000 0000 0000 0000 0000 0600  Tc..............
+00001440: 0000 0800 0000 0300 0000 731c 0000 0074  ..........s....t
+00001450: 0083 006a 017c 017c 027c 0364 017c 047c  ...j.|.|.|.d.|.|
+00001460: 0564 028d 0601 0064 0053 0029 034e da05  .d.....d.S.).N..
+00001470: 7661 6c69 6472 5800 0000 2902 7207 0000  validrX...).r...
+00001480: 0072 0800 0000 2906 720f 0000 0072 2800  .r....).r....r(.
+00001490: 0000 7225 0000 0072 2900 0000 722c 0000  ..r%...r)...r,..
+000014a0: 0072 2b00 0000 7210 0000 0072 1200 0000  .r+...r....r....
+000014b0: 7213 0000 0072 0800 0000 a800 0000 7310  r....r........s.
+000014c0: 0000 0000 0106 0102 0102 0102 0102 0102  ................
+000014d0: 0102 fa7a 1356 616c 6964 4570 6f63 682e  ...z.ValidEpoch.
+000014e0: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
+000014f0: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
+00001500: 0073 0e00 0000 7c00 6a00 a001 a100 0100  .s....|.j.......
+00001510: 6400 5300 7206 0000 0029 0272 2800 0000  d.S.r....).r(...
+00001520: da04 6576 616c 7220 0000 0072 1200 0000  ..evalr ...r....
+00001530: 7212 0000 0072 1300 0000 723f 0000 00b2  r....r....r?....
+00001540: 0000 0073 0200 0000 0001 7a19 5661 6c69  ...s......z.Vali
+00001550: 6445 706f 6368 2e6f 6e5f 6570 6f63 685f  dEpoch.on_epoch_
+00001560: 7374 6172 7463 0400 0000 0000 0000 0000  startc..........
+00001570: 0000 0900 0000 0900 0000 4300 0000 735a  ..........C...sZ
+00001580: 0000 0074 00a0 01a1 008f 3e01 007c 006a  ...t......>..|.j
+00001590: 02a0 037c 01a1 015c 027d 047d 057c 00a0  ...|...\.}.}.|..
+000015a0: 047c 047c 02a1 027d 067c 00a0 047c 057c  .|.|...}.|...|.|
+000015b0: 03a1 027d 0764 017c 0614 0064 017c 0714  ...}.d.|...d.|..
+000015c0: 0017 007d 0857 0035 0051 0052 0058 007c  ...}.W.5.Q.R.X.|
+000015d0: 067c 077c 087c 047c 0566 0553 0072 5b00  .|.|.|.|.f.S.r[.
+000015e0: 0000 2905 720c 0000 00da 076e 6f5f 6772  ..).r......no_gr
+000015f0: 6164 7228 0000 0072 1700 0000 7225 0000  adr(...r....r%..
+00001600: 0072 5f00 0000 7212 0000 0072 1200 0000  .r_...r....r....
+00001610: 7213 0000 0072 3e00 0000 b500 0000 730c  r....r>.......s.
+00001620: 0000 0000 010a 0110 010c 010c 041a 047a  ...............z
+00001630: 1756 616c 6964 4570 6f63 682e 6261 7463  .ValidEpoch.batc
+00001640: 685f 7570 6461 7465 2902 7256 0000 0054  h_update).rV...T
+00001650: 7260 0000 0072 1200 0000 7212 0000 0072  r`...r....r....r
+00001660: 1000 0000 7213 0000 0072 6100 0000 a600  ....r....ra.....
+00001670: 0000 7306 0000 0008 020e 0a08 0372 6100  ..s..........ra.
+00001680: 0000 2912 7245 0000 0072 0c00 0000 5a0b  ..).rE...r....Z.
+00001690: 746f 7263 682e 6f70 7469 6dda 056f 7074  torch.optim..opt
+000016a0: 696d da08 746f 7263 682e 6e6e 720a 0000  im..torch.nnr...
+000016b0: 0072 4800 0000 da02 6e70 7202 0000 005a  .rH.....npr....Z
+000016c0: 056d 6574 6572 7204 0000 00da 064d 6f64  .meterr......Mod
+000016d0: 756c 6572 0500 0000 721d 0000 005a 0e6d  uler....r....Z.m
+000016e0: 756c 7469 7461 736b 5f6c 6f73 7372 2600  ultitask_lossr&.
+000016f0: 0000 7255 0000 0072 6100 0000 7212 0000  ..rU...ra...r...
+00001700: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
+00001710: da08 3c6d 6f64 756c 653e 0100 0000 7318  ..<module>....s.
+00001720: 0000 0008 0108 010c 010c 0108 010c 010c  ................
+00001730: 0212 1012 110a 020e 5410 26              ........T.&
```

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/__pycache__/train.cpython-39.pyc` & `mammopy-0.0.9/segmentation_models/utils/__pycache__/train.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/base.py` & `mammopy-0.0.9/segmentation_models/utils/base.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/functional.py` & `mammopy-0.0.9/segmentation_models/utils/functional.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/losses.py` & `mammopy-0.0.9/segmentation_models/utils/losses.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/meter.py` & `mammopy-0.0.9/segmentation_models/utils/meter.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/metrics.py` & `mammopy-0.0.9/segmentation_models/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/mammopy/segmentation_models/utils/train.py` & `mammopy-0.0.9/segmentation_models/utils/train.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/README.md` & `mammopy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.8/PKG-INFO` & `mammopy-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mammopy
-Version: 0.0.8
+Version: 0.0.9
 Summary: A unified solution for mammogram image analysis and interpretation
 Author: UEF Cancer
 Author-email: uef.cancergroup@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

