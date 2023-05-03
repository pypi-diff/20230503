# Comparing `tmp/hahomematic-2023.4.5.tar.gz` & `tmp/hahomematic-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2023.4.5.tar", last modified: Fri Apr 28 18:27:42 2023, max compression
+gzip compressed data, was "hahomematic-2023.5.0.tar", last modified: Wed May  3 05:22:29 2023, max compression
```

## Comparing `hahomematic-2023.4.5.tar` & `hahomematic-2023.5.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:27:42.516555 hahomematic-2023.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-28 18:27:42.516555 hahomematic-2023.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:27:42.508555 hahomematic-2023.4.5/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/backport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:27:42.512555 hahomematic-2023.4.5/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)    17167 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)    24401 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/caches/visibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    49209 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/central_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    44779 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/json_rpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:27:42.512555 hahomematic-2023.4.5/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:27:42.512555 hahomematic-2023.4.5/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)    28032 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    36970 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19415 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19910 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:27:42.512555 hahomematic-2023.4.5/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:27:42.516555 hahomematic-2023.4.5/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:27:42.516555 hahomematic-2023.4.5/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/xml_rpc_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:27:42.512555 hahomematic-2023.4.5/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-28 18:27:41.000000 hahomematic-2023.4.5/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-28 18:27:42.000000 hahomematic-2023.4.5/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 18:27:41.000000 hahomematic-2023.4.5/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 18:27:40.000000 hahomematic-2023.4.5/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-28 18:27:42.000000 hahomematic-2023.4.5/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 18:27:42.000000 hahomematic-2023.4.5/hahomematic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-28 18:27:42.516555 hahomematic-2023.4.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:22:29.052802 hahomematic-2023.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-03 05:22:29.052802 hahomematic-2023.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:22:29.044802 hahomematic-2023.5.0/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/backport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:22:29.044802 hahomematic-2023.5.0/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17167 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24401 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/caches/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49209 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/central_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44779 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/json_rpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:22:29.048802 hahomematic-2023.5.0/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:22:29.048802 hahomematic-2023.5.0/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27916 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33824 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19415 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19910 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:22:29.048802 hahomematic-2023.5.0/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:22:29.048802 hahomematic-2023.5.0/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:22:29.052802 hahomematic-2023.5.0/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/xml_rpc_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/hahomematic/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:22:29.044802 hahomematic-2023.5.0/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-03 05:22:28.000000 hahomematic-2023.5.0/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-03 05:22:29.000000 hahomematic-2023.5.0/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 05:22:28.000000 hahomematic-2023.5.0/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 05:22:27.000000 hahomematic-2023.5.0/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-03 05:22:28.000000 hahomematic-2023.5.0/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 05:22:28.000000 hahomematic-2023.5.0/hahomematic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-03 05:21:52.000000 hahomematic-2023.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-03 05:22:29.052802 hahomematic-2023.5.0/setup.cfg
```

### Comparing `hahomematic-2023.4.5/LICENSE` & `hahomematic-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/PKG-INFO` & `hahomematic-2023.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.4.5
+Version: 2023.5.0
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.4.5/README.md` & `hahomematic-2023.5.0/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/__init__.py` & `hahomematic-2023.5.0/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/backport.py` & `hahomematic-2023.5.0/hahomematic/backport.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/caches/dynamic.py` & `hahomematic-2023.5.0/hahomematic/caches/dynamic.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/caches/persistent.py` & `hahomematic-2023.5.0/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/caches/visibility.py` & `hahomematic-2023.5.0/hahomematic/caches/visibility.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/central_unit.py` & `hahomematic-2023.5.0/hahomematic/central_unit.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/client.py` & `hahomematic-2023.5.0/hahomematic/client.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/const.py` & `hahomematic-2023.5.0/hahomematic/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/decorators.py` & `hahomematic-2023.5.0/hahomematic/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/exceptions.py` & `hahomematic-2023.5.0/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/exporter.py` & `hahomematic-2023.5.0/hahomematic/exporter.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/hmcli.py` & `hahomematic-2023.5.0/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/json_rpc_client.py` & `hahomematic-2023.5.0/hahomematic/json_rpc_client.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/__init__.py` & `hahomematic-2023.5.0/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/custom/__init__.py` & `hahomematic-2023.5.0/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/custom/climate.py` & `hahomematic-2023.5.0/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/custom/const.py` & `hahomematic-2023.5.0/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/custom/cover.py` & `hahomematic-2023.5.0/hahomematic/platforms/custom/cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/custom/definition.py` & `hahomematic-2023.5.0/hahomematic/platforms/custom/definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,16 +232,14 @@
         HmEntityDefinition.IP_RGBW_LIGHT: {
             ED_DEVICE_GROUP: {
                 ED_PRIMARY_CHANNEL: 1,
                 ED_SECONDARY_CHANNELS: (2, 3, 4),
                 ED_REPEATABLE_FIELDS: {
                     FIELD_DIRECTION: "ACTIVITY_STATE",
                     FIELD_COLOR_TEMPERATURE: "COLOR_TEMPERATURE",
-                    FIELD_ON_TIME_UNIT: "DURATION_UNIT",
-                    FIELD_ON_TIME_VALUE: "DURATION_VALUE",
                     FIELD_EFFECT: "EFFECT",
                     FIELD_HUE: "HUE",
                     FIELD_LEVEL: "LEVEL",
                     FIELD_RAMP_TIME_TO_OFF_UNIT: "RAMP_TIME_TO_OFF_UNIT",
                     FIELD_RAMP_TIME_TO_OFF_VALUE: "RAMP_TIME_TO_OFF_VALUE",
                     FIELD_RAMP_TIME_UNIT: "RAMP_TIME_UNIT",
                     FIELD_RAMP_TIME_VALUE: "RAMP_TIME_VALUE",
```

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/custom/entity.py` & `hahomematic-2023.5.0/hahomematic/platforms/custom/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/custom/light.py` & `hahomematic-2023.5.0/hahomematic/platforms/custom/light.py`

 * *Files 3% similar despite different names*

```diff
@@ -399,42 +399,32 @@
 
 
 class CeIpRGBWLight(BaseHmLight):
     """Class for HomematicIP HmIP-RGBW light entities."""
 
     def _init_entity_fields(self) -> None:
         """Init the entity fields."""
-        OnTimeMixin.__init__(self)
+        super()._init_entity_fields()
         self._e_activity_state: HmSelect = self._get_entity(
             field_name=FIELD_DIRECTION, entity_type=HmSelect
         )
         self._e_color_temperature_kelvin: HmInteger = self._get_entity(
             field_name=FIELD_COLOR_TEMPERATURE, entity_type=HmInteger
         )
-        self._e_on_time_value: HmAction = self._get_entity(
-            field_name=FIELD_ON_TIME_VALUE, entity_type=HmAction
-        )
-        self._e_on_time_unit: HmAction = self._get_entity(
-            field_name=FIELD_ON_TIME_UNIT, entity_type=HmAction
-        )
         self._e_device_operation_mode: HmSelect = self._get_entity(
             field_name=FIELD_DEVICE_OPERATION_MODE, entity_type=HmSelect
         )
         self._e_effect: HmAction = self._get_entity(field_name=FIELD_EFFECT, entity_type=HmAction)
         self._e_hue: HmInteger = self._get_entity(field_name=FIELD_HUE, entity_type=HmInteger)
-        self._e_level: HmFloat = self._get_entity(field_name=FIELD_LEVEL, entity_type=HmFloat)
         self._e_ramp_time_to_off_unit: HmAction = self._get_entity(
             field_name=FIELD_RAMP_TIME_TO_OFF_UNIT, entity_type=HmAction
         )
         self._e_ramp_time_to_off_value: HmAction = self._get_entity(
             field_name=FIELD_RAMP_TIME_TO_OFF_VALUE, entity_type=HmAction
         )
-        self._e_ramp_time_value: HmAction = self._get_entity(
-            field_name=FIELD_RAMP_TIME_VALUE, entity_type=HmAction
-        )
         self._e_ramp_time_unit: HmAction = self._get_entity(
             field_name=FIELD_RAMP_TIME_UNIT, entity_type=HmAction
         )
         self._e_saturation: HmFloat = self._get_entity(
             field_name=FIELD_SATURATION, entity_type=HmFloat
         )
 
@@ -459,19 +449,14 @@
     def hs_color(self) -> tuple[float, float] | None:
         """Return the hue and saturation color value [float, float]."""
         if self._e_hue.value is not None and self._e_saturation.value is not None:
             return self._e_hue.value, self._e_saturation.value * 100
         return None
 
     @config_property
-    def supports_brightness(self) -> bool:
-        """Flag if light supports brightness."""
-        return True
-
-    @config_property
     def supports_color_temperature(self) -> bool:
         """Flag if light supports color temperature."""
         return self._e_device_operation_mode.value == _DOM_TUNABLE_WHITE
 
     @config_property
     def supports_effects(self) -> bool:
         """Flag if light supports effects."""
@@ -484,75 +469,41 @@
 
     @config_property
     def supports_transition(self) -> bool:
         """Flag if light supports transition."""
         return True
 
     @value_property
-    def effect(self) -> str | None:
-        """Return the current effect."""
-        return None
-
-    @value_property
     def effect_list(self) -> list[str] | None:
         """Return the list of supported effects."""
         return list(self._e_effect.value_list or ())
 
     @bind_collector
     async def turn_on(
         self,
         collector: CallParameterCollector | None = None,
         **kwargs: Any,
     ) -> None:
         """Turn the light on."""
         if not self.is_state_change(on=True, **kwargs):
             return
-        if ramp_time := kwargs.get(_HM_ARG_RAMP_TIME):
-            await self._set_ramp_time_on_value(ramp_time=float(ramp_time), collector=collector)
-        if (on_time := kwargs.get(HM_ARG_ON_TIME)) or (on_time := self.get_on_time_and_cleanup()):
-            await self._set_on_time_value(on_time=on_time, collector=collector)
         if (hs_color := kwargs.get(_HM_ARG_HS_COLOR)) is not None:
             hue, ksaturation = hs_color
             saturation = ksaturation / 100
             await self._e_hue.send_value(value=int(hue), collector=collector)
             await self._e_saturation.send_value(value=saturation, collector=collector)
         if color_temp := kwargs.get(_HM_ARG_COLOR_TEMP):
             color_temp_kelvin = math.floor(1000000 / color_temp)
             await self._e_color_temperature_kelvin.send_value(
                 value=color_temp_kelvin, collector=collector
             )
         if self.supports_effects and (effect := kwargs.get(_HM_ARG_EFFECT)) is not None:
             await self._e_effect.send_value(value=effect, collector=collector)
 
-        brightness = kwargs.get(_HM_ARG_BRIGHTNESS, self.brightness)
-        if not brightness:
-            brightness = 255
-        level = brightness / 255.0
-        await self._e_level.send_value(value=level, collector=collector)
-
-    @bind_collector
-    async def turn_off(
-        self, collector: CallParameterCollector | None = None, **kwargs: Any
-    ) -> None:
-        """Turn the light off."""
-        if not self.is_state_change(off=True, **kwargs):
-            return
-        if ramp_time := kwargs.get(_HM_ARG_RAMP_TIME):
-            await self._set_ramp_time_off_value(ramp_time=float(ramp_time), collector=collector)
-
-        await self._e_level.send_value(value=HM_DIMMER_OFF, collector=collector)
-
-    @bind_collector
-    async def _set_on_time_value(
-        self, on_time: float, collector: CallParameterCollector | None = None
-    ) -> None:
-        """Set the on time value in seconds."""
-        on_time, on_time_unit = _recalc_unit_timer(time=on_time)
-        await self._e_on_time_unit.send_value(value=on_time_unit, collector=collector)
-        await self._e_on_time_value.send_value(value=float(on_time), collector=collector)
+        await super().turn_on(collector=collector, **kwargs)
 
     async def _set_ramp_time_on_value(
         self, ramp_time: float, collector: CallParameterCollector | None = None
     ) -> None:
         """Set the ramp time value in seconds."""
         ramp_time, ramp_time_unit = _recalc_unit_timer(time=ramp_time)
         await self._e_ramp_time_unit.send_value(value=ramp_time_unit, collector=collector)
@@ -564,36 +515,14 @@
         """Set the ramp time value in seconds."""
         ramp_time, ramp_time_unit = _recalc_unit_timer(time=ramp_time)
         await self._e_ramp_time_to_off_unit.send_value(value=ramp_time_unit, collector=collector)
         await self._e_ramp_time_to_off_value.send_value(
             value=float(ramp_time), collector=collector
         )
 
-    def is_state_change(self, **kwargs: Any) -> bool:
-        """Check if the state changes due to kwargs."""
-        if kwargs.get(HM_ARG_ON) is not None and self.is_on is not True and len(kwargs) == 1:
-            return True
-        if kwargs.get(HM_ARG_OFF) is not None and self.is_on is not False and len(kwargs) == 1:
-            return True
-        if (
-            brightness := kwargs.get(_HM_ARG_BRIGHTNESS)
-        ) is not None and brightness != self.brightness:
-            return True
-        if (hs_color := kwargs.get(_HM_ARG_HS_COLOR)) is not None and hs_color != self.hs_color:
-            return True
-        if (
-            color_temp := kwargs.get(_HM_ARG_COLOR_TEMP)
-        ) is not None and color_temp != self.color_temp:
-            return True
-        if kwargs.get(_HM_ARG_RAMP_TIME) is not None:
-            return True
-        if kwargs.get(HM_ARG_ON_TIME) is not None:
-            return True
-        return super().is_state_change(**kwargs)
-
 
 class CeIpFixedColorLight(BaseHmLight):
     """Class for HomematicIP HmIP-BSL, HmIPW-WRC6 light entities."""
 
     _color_switcher: dict[str, tuple[float, float]] = {
         "WHITE": (0.0, 0.0),
         "RED": (0.0, 100.0),
```

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/custom/lock.py` & `hahomematic-2023.5.0/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/custom/siren.py` & `hahomematic-2023.5.0/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/custom/support.py` & `hahomematic-2023.5.0/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/custom/switch.py` & `hahomematic-2023.5.0/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/device.py` & `hahomematic-2023.5.0/hahomematic/platforms/device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/entity.py` & `hahomematic-2023.5.0/hahomematic/platforms/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/event.py` & `hahomematic-2023.5.0/hahomematic/platforms/event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/generic/__init__.py` & `hahomematic-2023.5.0/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/generic/action.py` & `hahomematic-2023.5.0/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2023.5.0/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/generic/button.py` & `hahomematic-2023.5.0/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/generic/entity.py` & `hahomematic-2023.5.0/hahomematic/platforms/generic/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/generic/number.py` & `hahomematic-2023.5.0/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/generic/select.py` & `hahomematic-2023.5.0/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/generic/sensor.py` & `hahomematic-2023.5.0/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/generic/switch.py` & `hahomematic-2023.5.0/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/hub/__init__.py` & `hahomematic-2023.5.0/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2023.5.0/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/hub/button.py` & `hahomematic-2023.5.0/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/hub/entity.py` & `hahomematic-2023.5.0/hahomematic/platforms/hub/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/hub/number.py` & `hahomematic-2023.5.0/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/hub/select.py` & `hahomematic-2023.5.0/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/hub/sensor.py` & `hahomematic-2023.5.0/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/hub/text.py` & `hahomematic-2023.5.0/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/platforms/support.py` & `hahomematic-2023.5.0/hahomematic/platforms/support.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     def set_on_time(self, on_time: float) -> None:
         """Set the on_time."""
         self._on_time = on_time
         self._on_time_updated = datetime.now()
 
     def get_on_time_and_cleanup(self) -> float | None:
         """Return the on_time and cleanup afterwards."""
-        if self._on_time is None:
+        if not hasattr(self, "_on_time") or self._on_time is None:
             return None
         # save values
         on_time = self._on_time
         on_time_updated = self._on_time_updated
         # cleanup values
         self._on_time = None
         self._on_time_updated = INIT_DATETIME
```

### Comparing `hahomematic-2023.4.5/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2023.5.0/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2023.5.0/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2023.5.0/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/support.py` & `hahomematic-2023.5.0/hahomematic/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/xml_rpc_proxy.py` & `hahomematic-2023.5.0/hahomematic/xml_rpc_proxy.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic/xml_rpc_server.py` & `hahomematic-2023.5.0/hahomematic/xml_rpc_server.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/hahomematic.egg-info/PKG-INFO` & `hahomematic-2023.5.0/hahomematic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.4.5
+Version: 2023.5.0
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.4.5/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2023.5.0/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.5/pyproject.toml` & `hahomematic-2023.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2023.4.5"
+version     = "2023.5.0"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
```

