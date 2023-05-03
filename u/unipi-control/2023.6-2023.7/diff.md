# Comparing `tmp/unipi-control-2023.6.tar.gz` & `tmp/unipi-control-2023.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unipi-control-2023.6.tar", last modified: Sun Mar 19 20:57:30 2023, max compression
+gzip compressed data, was "unipi-control-2023.7.tar", last modified: Wed May  3 19:06:21 2023, max compression
```

## Comparing `unipi-control-2023.6.tar` & `unipi-control-2023.7.tar`

### file list

```diff
@@ -1,59 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:57:30.542946 unipi-control-2023.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-19 20:57:20.000000 unipi-control-2023.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-19 20:57:20.000000 unipi-control-2023.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17517 2023-03-19 20:57:30.542946 unipi-control-2023.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16769 2023-03-19 20:57:20.000000 unipi-control-2023.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-03-19 20:57:20.000000 unipi-control-2023.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-03-19 20:57:30.542946 unipi-control-2023.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 20:57:20.000000 unipi-control-2023.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:57:30.538946 unipi-control-2023.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:57:30.538946 unipi-control-2023.6/src/unipi_control/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:57:30.538946 unipi-control-2023.6/src/unipi_control/config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:57:30.538946 unipi-control-2023.6/src/unipi_control/config/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:57:30.538946 unipi-control-2023.6/src/unipi_control/config/etc/systemd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:57:30.538946 unipi-control-2023.6/src/unipi_control/config/etc/systemd/system/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/config/etc/systemd/system/unipi-control.service
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:57:30.542946 unipi-control-2023.6/src/unipi_control/config/etc/unipi/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/config/etc/unipi/control.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/config/etc/unipi/control.yaml.example
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:57:30.538946 unipi-control-2023.6/src/unipi_control/config/etc/unipi/hardware/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:57:30.542946 unipi-control-2023.6/src/unipi_control/config/etc/unipi/hardware/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/config/etc/unipi/hardware/extensions/Eastron_SDM120M.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/config/etc/unipi/hardware/extensions/xS11.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:57:30.542946 unipi-control-2023.6/src/unipi_control/config/etc/unipi/hardware/neuron/
--rwxr-xr-x   0 runner    (1001) docker     (123)      796 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/config/etc/unipi/hardware/neuron/L203.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:57:30.542946 unipi-control-2023.6/src/unipi_control/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/extensions/eastron.py
--rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:57:30.542946 unipi-control-2023.6/src/unipi_control/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21972 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/integrations/covers.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/modbus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2163 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/model_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:57:30.542946 unipi-control-2023.6/src/unipi_control/mqtt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/mqtt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:57:30.542946 unipi-control-2023.6/src/unipi_control/mqtt/discovery/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/mqtt/discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/mqtt/discovery/binary_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/mqtt/discovery/covers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/mqtt/discovery/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/mqtt/discovery/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/mqtt/discovery/switches.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/mqtt/features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:57:30.542946 unipi-control-2023.6/src/unipi_control/mqtt/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/mqtt/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/mqtt/integrations/covers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/neuron.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6362 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/unipi_control.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-19 20:57:20.000000 unipi-control-2023.6/src/unipi_control/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:57:30.538946 unipi-control-2023.6/src/unipi_control.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17517 2023-03-19 20:57:30.000000 unipi-control-2023.6/src/unipi_control.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-03-19 20:57:30.000000 unipi-control-2023.6/src/unipi_control.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 20:57:30.000000 unipi-control-2023.6/src/unipi_control.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-19 20:57:30.000000 unipi-control-2023.6/src/unipi_control.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-19 20:57:30.000000 unipi-control-2023.6/src/unipi_control.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-19 20:57:30.000000 unipi-control-2023.6/src/unipi_control.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:06:21.977882 unipi-control-2023.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 19:06:12.000000 unipi-control-2023.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-03 19:06:12.000000 unipi-control-2023.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19230 2023-05-03 19:06:21.977882 unipi-control-2023.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18196 2023-05-03 19:06:12.000000 unipi-control-2023.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:06:21.965882 unipi-control-2023.7/extras/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:06:21.965882 unipi-control-2023.7/extras/homeassistant/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:06:21.965882 unipi-control-2023.7/extras/homeassistant/blueprints/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:06:21.965882 unipi-control-2023.7/extras/homeassistant/blueprints/automation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:06:21.965882 unipi-control-2023.7/extras/homeassistant/blueprints/automation/cover/
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-03 19:06:12.000000 unipi-control-2023.7/extras/homeassistant/blueprints/automation/cover/control.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1686 2023-05-03 19:06:12.000000 unipi-control-2023.7/extras/homeassistant/blueprints/automation/cover/simple_cover_control.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-03 19:06:12.000000 unipi-control-2023.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-03 19:06:12.000000 unipi-control-2023.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-03 19:06:21.977882 unipi-control-2023.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-03 19:06:12.000000 unipi-control-2023.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:06:21.965882 unipi-control-2023.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:06:21.969882 unipi-control-2023.7/src/unipi_control/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16790 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:06:21.973882 unipi-control-2023.7/src/unipi_control/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/extensions/eastron.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16982 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:06:21.977882 unipi-control-2023.7/src/unipi_control/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21956 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/integrations/covers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/modbus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:06:21.977882 unipi-control-2023.7/src/unipi_control/mqtt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/mqtt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:06:21.977882 unipi-control-2023.7/src/unipi_control/mqtt/discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/mqtt/discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/mqtt/discovery/binary_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/mqtt/discovery/covers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/mqtt/discovery/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/mqtt/discovery/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/mqtt/discovery/switches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/mqtt/features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:06:21.977882 unipi-control-2023.7/src/unipi_control/mqtt/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/mqtt/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/mqtt/integrations/covers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/neuron.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:06:21.977882 unipi-control-2023.7/src/unipi_control/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/tools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2758 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/tools/config_backup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4611 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/tools/config_converter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2100 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/tools/model_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6724 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/unipi_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-03 19:06:12.000000 unipi-control-2023.7/src/unipi_control/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:06:21.973882 unipi-control-2023.7/src/unipi_control.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19230 2023-05-03 19:06:21.000000 unipi-control-2023.7/src/unipi_control.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-03 19:06:21.000000 unipi-control-2023.7/src/unipi_control.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:06:21.000000 unipi-control-2023.7/src/unipi_control.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-03 19:06:21.000000 unipi-control-2023.7/src/unipi_control.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-03 19:06:21.000000 unipi-control-2023.7/src/unipi_control.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 19:06:21.000000 unipi-control-2023.7/src/unipi_control.egg-info/top_level.txt
```

### Comparing `unipi-control-2023.6/PKG-INFO` & `unipi-control-2023.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,77 +1,112 @@
-Metadata-Version: 2.1
-Name: unipi-control
-Version: 2023.6
-Summary: Control Unipi I/O directly with MQTT commands and without Evok.
-Home-page: https://github.com/mh-superbox/unipi-control
-Author: Michael Hacker
-Author-email: mh@superbox.one
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![license-url](https://img.shields.io/npm/l/make-coverage-badge.svg)](https://opensource.org/licenses/MIT)
-![coverage-badge](https://raw.githubusercontent.com/mh-superbox/unipi-control/main/coverage.svg)
+[![license-url](https://img.shields.io/badge/license-Apache%202-yellowgreen)](https://opensource.org/license/apache-2-0/)
+![coverage-badge](https://raw.githubusercontent.com/superbox-dev/unipi-control/main/coverage.svg)
 ![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)
 ![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)
 ![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
+![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
+
+# Unipi Control
+
+Control Unipi I/O directly with MQTT commands and without [Evok](https://github.com/UniPiTechnology/evok). Unipi Control use Modbus for fast access to the I/O and provide MQTT topics for reading and writing the circuits. Optionally you can enable the Home Assistant MQTT discovery for binary sensors, sensors, switches and covers.
 
 ### Support me if you like this project 😀
 
 I want to extend the code to support Unipi extensions modules.
 The necessary hardware is also required for this.
 
-[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/mhacker)
-
-# Unipi Control
+[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/F2F0KXO6D)
 
-Control Unipi I/O directly with MQTT commands and without [Evok](https://github.com/UniPiTechnology/evok). Unipi Control use Modbus for fast access to the I/O and provide MQTT topics for reading and writing the circuits. Optionally you can enable the Home Assistant MQTT discovery for binary sensors, sensors, switches and covers.
+[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/superbox_dev)
 
 ## Supported hardware
 
-* Unipi Neuron L203
+* Tested:
+  * Unipi Neuron
+    * L203
+* Untested:
+  * Unipi Neuron
+    * S103
+    * S103-G
+    * M103
+    * M203
+    * M523
+    * L523
+    * L533
+  * Unipi Patron
+    * Patron S107
+    * Patron S117
+    * Patron S167
+    * Patron M207
+    * Patron M267
+    * Patron M527
+    * Patron M567
+    * Patron S207
+    * Patron L207
+    * Patron L527
 * External Modbus RTU devices
   * [Eastron SDM120M](https://www.eastroneurope.com/products/view/sdm120modbus)
 
+If you tried an untested Unipi device then please let me know the result to update this page.
+
 If you have an Unipi device, that is not supported, then contact me.
 
 ## Getting Started
 
+### Recommended installation (Only for Unipi Neuron)
+
+Use the [Unipi Control OS](https://github.com/superbox-dev/unipi-control-os).
+
+### Alternative installation (Debian based systems)
+
 **Requirements:**
 
-* Unipi Neuron Kernel Module and Unipi tools
-  * Use the officially APT mirror (https://repo.unipi.technology/debian/) from Unipi Technology
-  * Or compile it
-    * https://github.com/UniPiTechnology/unipi-kernel
-    * https://github.com/UniPiTechnology/unipi-tools
-* Python 3.8
+* Unipi Neuron Kernel Module and Unipi tools (Use the officially APT mirror (https://repo.unipi.technology/debian/) from Unipi Technology)
+* Python >= 3.8
 
 Install **Unipi Control** with `pip`.
 
 ```shell
 $ python -m venv /opt/.venv
 $ /opt/.venv/bin/pip install unipi-control
 ```
 
-Copy the [config files](src/unipi_control/config/etc) to your `/etc` directory and start the systemd service:
+Copy the [config files](opkg/data/local/etc/unipi) to your `/etc/unipi` directory and
+create the systemd service `/etc/systemd/system/unipi-control.service` with following content:
+
+```
+[Unit]
+Description=Unipi Control
+After=multi-user.target
+
+[Service]
+Type=simple
+ExecStart=/opt/.venv/bin/unipi-control --log systemd
+Environment=PYTHONUNBUFFERED=1
+
+[Install]
+WantedBy=multi-user.target
+```
+
+Enable and start the systemd service:
 
 ```shell
+$ systemctl --system daemon-reload
 $ systemctl enable unipi-control.service
 $ systemctl start unipi-control.service
 ```
 
+## Arguments
+
+| Argument   | Description                                                           |
+|------------|-----------------------------------------------------------------------|
+| `--config` | path to the configuration (default: /etc/unipi)                       |
+| `-v`       | verbose mode: multiple -v options increase the verbosity (maximum: 4) |
+
+
 ## Configuration
 
 You can set the client settings in the `/etc/unipi/control.yaml`.
 
 ### Device
 
 | Key    | Value                                                                                                                                                               |
@@ -281,17 +316,22 @@
 ## Development
 
 For development, you must clone the git repository and install **Unipi Control** with `pipenv`.
 
 ```shell
 $ git clone https://github.com/mh-superbox/unipi-control.git
 $ cd unipi-control
-~/unipi-control$ pipenv install --deploy --dev 
-~/unipi-control$ pipenv run pip install -e .
+~/unipi-control$ make install-dev
+```
+
+Copy the [config files](opkg/data/local/etc/unipi) to your `/etc/unipi` directory
+and activate your virtualenv with:
+
+```shell
+~/unipi-control$ source .venv/bin/activate
 ```
 
-Copy the config files to your `/etc` directory.
-Now you can start unipi-control with `pipenv run unipi-control`.
+Now you can start unipi-control with `unipi-control`.
 
 ## Extras
 
 I have written a Home Assistant blueprint automation to control covers with binary sensors. Take a look in the [extras](extras) directory.
```

### Comparing `unipi-control-2023.6/README.md` & `unipi-control-2023.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,137 @@
-[![license-url](https://img.shields.io/npm/l/make-coverage-badge.svg)](https://opensource.org/licenses/MIT)
-![coverage-badge](https://raw.githubusercontent.com/mh-superbox/unipi-control/main/coverage.svg)
+Metadata-Version: 2.1
+Name: unipi-control
+Version: 2023.7
+Summary: Control Unipi I/O directly with MQTT commands.
+Home-page: https://github.com/superbox-dev/unipi-control
+Author: Michael Hacker
+Author-email: mh@superbox.one
+License: Apache-2.0 license
+Project-URL: Source Code, https://github.com/superbox-dev/unipi-control
+Project-URL: Bug Reports, https://github.com/superbox-dev/unipi-control/issues
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Topic :: System :: Networking
+Classifier: Topic :: Utilities
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![license-url](https://img.shields.io/badge/license-Apache%202-yellowgreen)](https://opensource.org/license/apache-2-0/)
+![coverage-badge](https://raw.githubusercontent.com/superbox-dev/unipi-control/main/coverage.svg)
 ![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)
 ![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)
 ![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
+![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
+
+# Unipi Control
+
+Control Unipi I/O directly with MQTT commands and without [Evok](https://github.com/UniPiTechnology/evok). Unipi Control use Modbus for fast access to the I/O and provide MQTT topics for reading and writing the circuits. Optionally you can enable the Home Assistant MQTT discovery for binary sensors, sensors, switches and covers.
 
 ### Support me if you like this project 😀
 
 I want to extend the code to support Unipi extensions modules.
 The necessary hardware is also required for this.
 
-[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/mhacker)
-
-# Unipi Control
+[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/F2F0KXO6D)
 
-Control Unipi I/O directly with MQTT commands and without [Evok](https://github.com/UniPiTechnology/evok). Unipi Control use Modbus for fast access to the I/O and provide MQTT topics for reading and writing the circuits. Optionally you can enable the Home Assistant MQTT discovery for binary sensors, sensors, switches and covers.
+[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/superbox_dev)
 
 ## Supported hardware
 
-* Unipi Neuron L203
+* Tested:
+  * Unipi Neuron
+    * L203
+* Untested:
+  * Unipi Neuron
+    * S103
+    * S103-G
+    * M103
+    * M203
+    * M523
+    * L523
+    * L533
+  * Unipi Patron
+    * Patron S107
+    * Patron S117
+    * Patron S167
+    * Patron M207
+    * Patron M267
+    * Patron M527
+    * Patron M567
+    * Patron S207
+    * Patron L207
+    * Patron L527
 * External Modbus RTU devices
   * [Eastron SDM120M](https://www.eastroneurope.com/products/view/sdm120modbus)
 
+If you tried an untested Unipi device then please let me know the result to update this page.
+
 If you have an Unipi device, that is not supported, then contact me.
 
 ## Getting Started
 
+### Recommended installation (Only for Unipi Neuron)
+
+Use the [Unipi Control OS](https://github.com/superbox-dev/unipi-control-os).
+
+### Alternative installation (Debian based systems)
+
 **Requirements:**
 
-* Unipi Neuron Kernel Module and Unipi tools
-  * Use the officially APT mirror (https://repo.unipi.technology/debian/) from Unipi Technology
-  * Or compile it
-    * https://github.com/UniPiTechnology/unipi-kernel
-    * https://github.com/UniPiTechnology/unipi-tools
-* Python 3.8
+* Unipi Neuron Kernel Module and Unipi tools (Use the officially APT mirror (https://repo.unipi.technology/debian/) from Unipi Technology)
+* Python >= 3.8
 
 Install **Unipi Control** with `pip`.
 
 ```shell
 $ python -m venv /opt/.venv
 $ /opt/.venv/bin/pip install unipi-control
 ```
 
-Copy the [config files](src/unipi_control/config/etc) to your `/etc` directory and start the systemd service:
+Copy the [config files](opkg/data/local/etc/unipi) to your `/etc/unipi` directory and
+create the systemd service `/etc/systemd/system/unipi-control.service` with following content:
+
+```
+[Unit]
+Description=Unipi Control
+After=multi-user.target
+
+[Service]
+Type=simple
+ExecStart=/opt/.venv/bin/unipi-control --log systemd
+Environment=PYTHONUNBUFFERED=1
+
+[Install]
+WantedBy=multi-user.target
+```
+
+Enable and start the systemd service:
 
 ```shell
+$ systemctl --system daemon-reload
 $ systemctl enable unipi-control.service
 $ systemctl start unipi-control.service
 ```
 
+## Arguments
+
+| Argument   | Description                                                           |
+|------------|-----------------------------------------------------------------------|
+| `--config` | path to the configuration (default: /etc/unipi)                       |
+| `-v`       | verbose mode: multiple -v options increase the verbosity (maximum: 4) |
+
+
 ## Configuration
 
 You can set the client settings in the `/etc/unipi/control.yaml`.
 
 ### Device
 
 | Key    | Value                                                                                                                                                               |
@@ -261,17 +341,22 @@
 ## Development
 
 For development, you must clone the git repository and install **Unipi Control** with `pipenv`.
 
 ```shell
 $ git clone https://github.com/mh-superbox/unipi-control.git
 $ cd unipi-control
-~/unipi-control$ pipenv install --deploy --dev 
-~/unipi-control$ pipenv run pip install -e .
+~/unipi-control$ make install-dev
+```
+
+Copy the [config files](opkg/data/local/etc/unipi) to your `/etc/unipi` directory
+and activate your virtualenv with:
+
+```shell
+~/unipi-control$ source .venv/bin/activate
 ```
 
-Copy the config files to your `/etc` directory.
-Now you can start unipi-control with `pipenv run unipi-control`.
+Now you can start unipi-control with `unipi-control`.
 
 ## Extras
 
 I have written a Home Assistant blueprint automation to control covers with binary sensors. Take a look in the [extras](extras) directory.
```

### Comparing `unipi-control-2023.6/pyproject.toml` & `unipi-control-2023.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ignore_missing_imports = true
 
 [tool.pylint.master]
 # C0114: missing-module-docstring
 # C0115: missing-class-docstring
 # C0116: missing-function-docstring
 # C0301: line-too-long
-# C0411: rong-import-order
+# C0411: wrong-import-order
 # E0401: import-error
 # R0801: duplicate-code
 # R1732: consider-using-with
 # R6003: consider-alternative-union-syntax (python 3.8 compatibility)
 # W6001: deprecated-typing-alias (python 3.8 compatibility)
 disable = ["C0114", "C0115", "C0116", "C0301", "C0411", "E0401", "R0801", "R1732", "R6003", "W6001"]
 notes = ["FIXME"]
```

### Comparing `unipi-control-2023.6/setup.cfg` & `unipi-control-2023.7/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 [bdist_wheel]
 universal = 0
 
 [metadata]
 name = unipi-control
 version = attr: unipi_control.__version__
-description = Control Unipi I/O directly with MQTT commands and without Evok.
+description = Control Unipi I/O directly with MQTT commands.
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/mh-superbox/unipi-control
+url = https://github.com/superbox-dev/unipi-control
 author = Michael Hacker
 author_email = mh@superbox.one
-license = MIT
+license = Apache-2.0 license
 license_files = 
 	LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
-	License :: OSI Approved :: MIT License
+	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3 :: Only
 	Operating System :: POSIX :: Linux
+	Topic :: System :: Networking
+	Topic :: Utilities
+project_urls = 
+	Source Code = https://github.com/superbox-dev/unipi-control
+	Bug Reports = https://github.com/superbox-dev/unipi-control/issues
 
 [options]
 package_dir = 
 	= src
 packages = find:
 include_package_data = True
 python_requires = >=3.8
-install_requires = 
-	pymodbus[serial]~=3.2.0
-	superbox-utils[mqtt]~=2023.3
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	unipi-control = unipi_control.unipi_control:main
-	unipi-model-info = unipi_control.model_info:main
+	unipi-config-backup = unipi_control.tools.config_backup:main
+	unipi-config-converter = unipi_control.tools.config_converter:main
+	unipi-model-info = unipi_control.tools.model_info:main
 
 [flake8]
 max-line-length = 120
 noqa-require-code = True
 docstring-convention = numpy
 ignore = 
 	D100,
```

### Comparing `unipi-control-2023.6/src/unipi_control/config.py` & `unipi-control-2023.7/src/unipi_control/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 from superbox_utils.config.exception import ConfigException
 from superbox_utils.config.loader import ConfigLoaderMixin
 from superbox_utils.config.loader import Validation
 from superbox_utils.hass.config import HomeAssistantConfig
 from superbox_utils.logging.config import LoggingConfig
 from superbox_utils.mqtt.config import MqttConfig
 from superbox_utils.yaml.loader import yaml_loader_safe
-from unipi_control.log import LOG_NAME
 
-logger: logging.Logger = logging.getLogger(LOG_NAME)
+logger: logging.Logger = logging.getLogger()
 
+DEFAULT_CONFIG_PATH: Final[Path] = Path("/etc/unipi")
 DEVICE_CLASSES: Final[List[str]] = ["blind", "roller_shutter", "garage_door"]
 
 MODBUS_BAUD_RATES: Final[List[int]] = [2400, 4800, 9600, 19200, 38400, 57600, 115200]
 MODBUS_PARITY: Final[List[str]] = ["E", "O", "N"]
 
 
 class LogPrefix:
@@ -195,23 +195,22 @@
             )
 
         return value
 
 
 @dataclass
 class Config(ConfigLoaderMixin):
-    device_info: DeviceInfo = field(default=DeviceInfo())
+    device_info: DeviceInfo = field(default_factory=DeviceInfo)
     mqtt: MqttConfig = field(default_factory=MqttConfig)
     modbus: ModbusConfig = field(default_factory=ModbusConfig)
     homeassistant: HomeAssistantConfig = field(default_factory=HomeAssistantConfig)
     features: dict = field(init=False, default_factory=dict)
     covers: list = field(init=False, default_factory=list)
     logging: LoggingConfig = field(default_factory=LoggingConfig)
-    config_base_path: Path = field(default=Path("/etc/unipi"))
-    systemd_path: Path = field(default=Path("/etc/systemd/system"))
+    config_base_path: Path = field(default=DEFAULT_CONFIG_PATH)
     temp_path: Path = field(default=Path(gettempdir()) / "unipi")
     sys_bus: Path = field(default=Path("/sys/bus/i2c/devices"))
 
     @cached_property
     def hardware_path(self) -> Path:
         """Return hardware path to neuron devices and extensions."""
         return self.config_base_path / "hardware"
@@ -280,14 +279,21 @@
 
         for cover in self.covers:
             if cover.object_id in object_ids:
                 raise ConfigException(f"{LogPrefix.COVER} Duplicate ID '{cover.object_id}' found in 'covers'!")
 
             object_ids.append(cover.object_id)
 
+    @staticmethod
+    def _validate_config_base_path(value: Path, _field: dataclasses.Field) -> Path:
+        if not value.is_dir() or not value.exists():
+            raise ConfigException(f"{LogPrefix.DEVICEINFO} Config path '{value}' is invalid!")
+
+        return value
+
 
 @dataclass
 class HardwareInfo:
     sys_bus: Path
     name: str = field(default="unknown")
     model: str = field(default="unknown", init=False)
     version: str = field(default="unknown", init=False)
@@ -405,17 +411,15 @@
                     )
                 )
             except TypeError as error:
                 raise ConfigException(f"{LogPrefix.CONFIG} Definition is invalid: {definition_file}") from error
 
             logger.debug("%s Definition loaded: %s", LogPrefix.CONFIG, definition_file)
         else:
-            raise ConfigException(
-                f'No valid YAML definition for active Neuron device! Device name is {self.data["neuron"].model}'
-            )
+            raise ConfigException("No valid YAML definition found for this device!")
 
     def _read_extension_definitions(self) -> None:
         try:
             for definition_file in Path(f"{self.config.hardware_path}/extensions").glob("*.yaml"):
                 yaml_content: dict = yaml_loader_safe(definition_file)
 
                 try:
```

### Comparing `unipi-control-2023.6/src/unipi_control/extensions/eastron.py` & `unipi-control-2023.7/src/unipi_control/extensions/eastron.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import asyncio
 from typing import Optional
 
-from pymodbus.register_read_message import ReadHoldingRegistersResponse
+from pymodbus.pdu import ModbusResponse
 
 from unipi_control.config import HardwareDefinition
-from unipi_control.config import LogPrefix
-from unipi_control.config import logger
 from unipi_control.features import EastronMeter
+from unipi_control.modbus import check_modbus_call
 
 
 class EastronSDM120M:
     def __init__(self, neuron, definition: HardwareDefinition) -> None:
         """Initialize Eastron SDM120M electricity meter.
 
         Attributes
@@ -35,34 +34,42 @@
     def _parse_feature(self, modbus_feature: dict) -> None:
         feature_type: str = modbus_feature["feature_type"].lower()
 
         if func := getattr(self, f"_parse_feature_{feature_type}", None):
             func(modbus_feature)
 
     async def _get_sw_version(self) -> Optional[str]:
-        await asyncio.sleep(4e-3)
-
-        sw_version: Optional[str] = None
+        sw_version: str = "Unknown"
 
         data: dict = {
             "address": 64514,
             "count": 2,
             "slave": self.definition.unit,
         }
 
-        try:
-            response: ReadHoldingRegistersResponse = await self.neuron.modbus_client.serial.read_holding_registers(
-                **data
+        retry: bool = True
+        retry_reconnect: int = 0
+        retry_limit: int = 5
+
+        while retry:
+            retry_reconnect += 1
+
+            response: Optional[ModbusResponse] = await check_modbus_call(
+                self.neuron.modbus_client.serial.read_holding_registers, data
             )
 
-            if not response.isError():
-                meter_code: str = f"{format(response.registers[0], '0x')}{format(response.registers[1], '0x')}"
+            if response:
+                meter_code: str = f"{format(getattr(response, 'registers')[0], '0x')}{format(getattr(response, 'registers')[1], '0x')}"
                 sw_version = f"{meter_code[:3]}.{meter_code[3:]}"
-        except asyncio.exceptions.TimeoutError:
-            logger.error("%s Timeout on: %s", LogPrefix.MODBUS, data)
+                retry = False
+
+            if retry_reconnect == retry_limit:
+                retry = False
+
+            await asyncio.sleep(1)
 
         return sw_version
 
     def parse_features(self) -> None:
         """Parse features from hardware definition."""
         for modbus_feature in self.definition.modbus_features:
             self._parse_feature(modbus_feature)
```

### Comparing `unipi-control-2023.6/src/unipi_control/features.py` & `unipi-control-2023.7/src/unipi_control/features.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,26 @@
 from typing import Any
 from typing import Dict
 from typing import Final
 from typing import List
 from typing import Optional
 from typing import Union
 
-from pymodbus.bit_write_message import WriteSingleCoilResponse
 from pymodbus.constants import Endian
 from pymodbus.payload import BinaryPayloadDecoder
+from pymodbus.pdu import ModbusResponse
 
 from superbox_utils.text.text import slugify
 from unipi_control.config import Config
 from unipi_control.config import ConfigException
 from unipi_control.config import FeatureConfig
 from unipi_control.config import HardwareDefinition
 from unipi_control.config import LogPrefix
 from unipi_control.modbus import ModbusClient
+from unipi_control.modbus import check_modbus_call
 
 
 class FeatureState:
     ON: str = "ON"
     OFF: str = "OFF"
 
 
@@ -262,66 +263,87 @@
         """Return software version from the Unipi Neuron."""
         return self.neuron.boards[self.major_group - 1].firmware
 
 
 class Relay(NeuronFeature):
     """Class for the relay feature from the Unipi Neuron."""
 
-    async def set_state(self, value: bool) -> WriteSingleCoilResponse:
+    async def set_state(self, value: bool) -> Optional[ModbusResponse]:
         """Set state for relay feature.
 
         Parameters
         ----------
         value: bool
 
         Returns
         -------
-        WriteSingleCoilResponse
+        ModbusResponse
         """
-        return await self.modbus_client.tcp.write_coil(address=self.val_coil, value=value, slave=0)
+        return await check_modbus_call(
+            self.modbus_client.tcp.write_coil,
+            data={
+                "address": self.val_coil,
+                "value": value,
+                "slave": 0,
+            },
+        )
 
 
 class DigitalOutput(NeuronFeature):
     """Class for the digital output feature from the Unipi Neuron."""
 
-    async def set_state(self, value: bool) -> WriteSingleCoilResponse:
+    async def set_state(self, value: bool) -> Optional[ModbusResponse]:
         """Set state for digital output feature.
 
         Parameters
         ----------
         value: bool
 
         Returns
         -------
-        WriteSingleCoilResponse
+        ModbusResponse
         """
-        return await self.modbus_client.tcp.write_coil(address=self.val_coil, value=value, slave=0)
+        return await check_modbus_call(
+            self.modbus_client.tcp.write_coil,
+            data={
+                "address": self.val_coil,
+                "value": value,
+                "slave": 0,
+            },
+        )
 
 
 class DigitalInput(NeuronFeature):
     """Class for the digital input feature from the Unipi Neuron."""
 
     pass  # pylint: disable=unnecessary-pass
 
 
 class Led(NeuronFeature):
     """Class for the LED feature from the Unipi Neuron."""
 
-    async def set_state(self, value: bool) -> WriteSingleCoilResponse:
+    async def set_state(self, value: bool) -> Optional[ModbusResponse]:
         """Set state for LED feature.
 
         Parameters
         ----------
         value: bool
 
         Returns
         -------
-        WriteSingleCoilResponse
+        ModbusResponse
         """
-        return await self.modbus_client.tcp.write_coil(address=self.val_coil, value=value, slave=0)
+        return await check_modbus_call(
+            self.modbus_client.tcp.write_coil,
+            data={
+                "address": self.val_coil,
+                "value": value,
+                "slave": 0,
+            },
+        )
 
 
 class MeterFeature(BaseFeature):
     def __init__(self, neuron, definition: HardwareDefinition, **kwargs) -> None:
         super().__init__(neuron, definition, kwargs["feature_type"])
 
         self._base_friendly_name: str = kwargs["friendly_name"]
```

### Comparing `unipi-control-2023.6/src/unipi_control/integrations/covers.py` & `unipi-control-2023.7/src/unipi_control/integrations/covers.py`

 * *Files 2% similar despite different names*

```diff
@@ -413,18 +413,18 @@
             if self.position is not None and self.position >= 100:
                 return None
 
         if self.calibrate_mode is True and not calibrate:
             return None
 
         self._update_position()
-        response: ModbusResponse = await self.cover_down_feature.set_state(False)
+        response: Optional[ModbusResponse] = await self.cover_down_feature.set_state(False)
         self._stop_timer()
 
-        if not response.isError():
+        if response:
             await self.cover_up_feature.set_state(True)
 
             self._device_state = CoverDeviceState.OPEN
             self.state = CoverState.OPENING
             self._start_timer = time.monotonic()
 
             if self.settings.set_position is True:
@@ -478,18 +478,18 @@
             if self.position <= 0:
                 return None
 
         if self.calibrate_mode is True:
             return None
 
         self._update_position()
-        response: ModbusResponse = await self.cover_up_feature.set_state(False)
+        response: Optional[ModbusResponse] = await self.cover_up_feature.set_state(False)
         self._stop_timer()
 
-        if not response.isError():
+        if response:
             await self.cover_down_feature.set_state(True)
 
             self._device_state = CoverDeviceState.CLOSE
             self.state = CoverState.CLOSING
             self._start_timer = time.monotonic()
 
             if self.settings.set_position is True:
@@ -550,18 +550,18 @@
             return None
 
         if self.tilt == 100:
             return None
 
         if self.tilt_change_time:
             self._update_position()
-            response: ModbusResponse = await self.cover_down_feature.set_state(False)
+            response: Optional[ModbusResponse] = await self.cover_down_feature.set_state(False)
             self._stop_timer()
 
-            if not response.isError():
+            if response:
                 await self.cover_up_feature.set_state(True)
 
                 self._device_state = CoverDeviceState.OPEN
                 self.state = CoverState.OPENING
                 self._start_timer = time.monotonic()
 
                 cover_run_time = (tilt - self.tilt) * self.tilt_change_time / 100
@@ -577,18 +577,18 @@
         cover_run_time: Optional[float] = None
 
         if not self.tilt:
             return None
 
         if self.tilt_change_time:
             self._update_position()
-            response: ModbusResponse = await self.cover_up_feature.set_state(False)
+            response: Optional[ModbusResponse] = await self.cover_up_feature.set_state(False)
             self._stop_timer()
 
-            if not response.isError():
+            if response:
                 await self.cover_down_feature.set_state(True)
 
                 self._device_state = CoverDeviceState.CLOSE
                 self.state = CoverState.CLOSING
                 self._start_timer = time.monotonic()
 
                 cover_run_time = (self.tilt - tilt) * self.tilt_change_time / 100
```

### Comparing `unipi-control-2023.6/src/unipi_control/modbus.py` & `unipi-control-2023.7/src/unipi_control/modbus.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,55 @@
 import asyncio
+from typing import Callable
 from typing import Dict
 from typing import List
 from typing import NamedTuple
 from typing import Optional
 
 from pymodbus.client import AsyncModbusSerialClient
 from pymodbus.client import AsyncModbusTcpClient
-from pymodbus.exceptions import ModbusIOException
-from pymodbus.pdu import ExceptionResponse
-from pymodbus.register_read_message import ReadInputRegistersResponse
+from pymodbus.exceptions import ModbusException
+from pymodbus.pdu import ModbusResponse
 
 from unipi_control.config import HardwareData
 from unipi_control.config import HardwareDefinition
 from unipi_control.config import LogPrefix
 from unipi_control.config import logger
 
 
+async def check_modbus_call(callback: Callable, data: dict) -> Optional[ModbusResponse]:
+    """Check modbus read/write call has errors and log the errors.
+
+    Parameters
+    ----------
+    callback: Callable
+        modbus callback function e.g. read_input_registers()
+    data: dict
+        Arguments pass to the callback function
+
+    Returns
+    -------
+    ModbusResponse: optional
+        Return modbus response if no errors found else None.
+    """
+    response: Optional[ModbusResponse] = None
+
+    try:
+        response = await callback(**data)
+
+        if response and response.isError():
+            response = None
+    except ModbusException as error:
+        logger.error("%s %s", LogPrefix.MODBUS, error)
+    except asyncio.exceptions.TimeoutError:
+        logger.error("%s Timeout on: %s", LogPrefix.MODBUS, data)
+
+    return response
+
+
 class ModbusClient(NamedTuple):
     tcp: AsyncModbusTcpClient
     serial: AsyncModbusSerialClient
 
 
 class ModbusCacheData:
     """Class that scan modbus register blocks and cache the response.
@@ -38,39 +68,40 @@
 
         self.data: Dict[int, Dict[int, int]] = {}
 
     async def _save_response(self, scan_type: str, modbus_register_block: dict, definition: HardwareDefinition) -> None:
         data: dict = {
             "address": modbus_register_block["start_reg"],
             "count": modbus_register_block["count"],
-            "slave": definition.unit,
+            "slave": modbus_register_block.get("slave", definition.unit),
         }
 
-        response: Optional[ReadInputRegistersResponse] = None
+        response: Optional[ModbusResponse] = None
 
-        try:
-            if scan_type == "tcp":
-                response = await self.modbus_client.tcp.read_input_registers(**data)
-            elif scan_type == "serial":
-                response = await self.modbus_client.serial.read_input_registers(**data)
-
-            if response:
-                if not isinstance(response, (ModbusIOException, ExceptionResponse)):
-                    for index in range(data["count"]):
-                        self.data[definition.unit][data["address"] + index] = response.registers[index]
-        except asyncio.exceptions.TimeoutError:
-            logger.error("%s [%s] Timeout on: %s", LogPrefix.MODBUS, scan_type.upper(), data)
+        if scan_type == "tcp":
+            response = await check_modbus_call(self.modbus_client.tcp.read_input_registers, data)
+        elif scan_type == "serial":
+            response = await check_modbus_call(self.modbus_client.serial.read_input_registers, data)
+
+        if registers := getattr(response, "registers", None):
+            for index in range(data["count"]):
+                self.data[definition.unit][
+                    data["address"] + index
+                ] = registers[  # pylint: disable=unsubscriptable-object
+                    index
+                ]
 
     async def scan(self, scan_type: str, hardware_types: List[str]) -> None:
         """Read modbus register blocks and cache the response."""
         for definition in self.hardware.get_definition_by_hardware_types(hardware_types):
             if not self.data.get(definition.unit):
                 self.data[definition.unit] = {}
 
-            await asyncio.sleep(8e-3)
+            if scan_type == "serial":
+                await asyncio.sleep(1)
 
             for modbus_register_block in definition.modbus_register_blocks:
                 await self._save_response(scan_type, modbus_register_block, definition)
 
     def get_register(self, address: int, index: int, unit: int) -> list:
         """Get the responses from the cached modbus register blocks.
```

### Comparing `unipi-control-2023.6/src/unipi_control/model_info.py` & `unipi-control-2023.7/src/unipi_control/tools/model_info.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 import struct
 from pathlib import Path
 
 
 def main() -> None:
     """Tiny script to detect the Unipi Neuron model."""
     unipi_1: Path = Path("/sys/bus/i2c/devices/1-0050/eeprom")
@@ -55,11 +54,7 @@
             version = f"{ee_bytes[99]}.{ee_bytes[98]}"
             serial = struct.unpack("i", ee_bytes[100:104])[0]
 
     print(f"Name: {name}")
     print(f"Model: {model}")
     print(f"Version: {version}")
     print(f"Serial: {serial}")
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `unipi-control-2023.6/src/unipi_control/mqtt/discovery/binary_sensors.py` & `unipi-control-2023.7/src/unipi_control/mqtt/discovery/binary_sensors.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2023.6/src/unipi_control/mqtt/discovery/covers.py` & `unipi-control-2023.7/src/unipi_control/mqtt/discovery/covers.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2023.6/src/unipi_control/mqtt/discovery/mixin.py` & `unipi-control-2023.7/src/unipi_control/mqtt/discovery/mixin.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2023.6/src/unipi_control/mqtt/discovery/sensors.py` & `unipi-control-2023.7/src/unipi_control/mqtt/discovery/sensors.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2023.6/src/unipi_control/mqtt/discovery/switches.py` & `unipi-control-2023.7/src/unipi_control/mqtt/discovery/switches.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2023.6/src/unipi_control/mqtt/features.py` & `unipi-control-2023.7/src/unipi_control/mqtt/features.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,25 +89,24 @@
             logger.info(LOG_MQTT_SUBSCRIBE, topic, value)
 
 
 class MeterFeaturesMqttPlugin(BaseFeaturesMqttPlugin):
     """Provide features control as MQTT commands."""
 
     publish_feature_types: List[str] = ["METER"]
-    scan_interval: float = 50e-1
+    scan_interval: float = 25e-3
 
     async def init_tasks(self, tasks: Set[Task]) -> None:
         """Initialize MQTT tasks for publish MQTT topics.
 
         Parameters
         ----------
         tasks: set
             A set of all MQTT tasks.
         """
-        # TODO create task by unit
         task: Task[Any] = asyncio.create_task(
             self._publish(
                 scan_type="serial",
                 hardware_types=[HardwareType.EXTENSION],
                 feature_types=self.publish_feature_types,
                 sleep=self.scan_interval,
             )
```

### Comparing `unipi-control-2023.6/src/unipi_control/mqtt/integrations/covers.py` & `unipi-control-2023.7/src/unipi_control/mqtt/integrations/covers.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2023.6/src/unipi_control/neuron.py` & `unipi-control-2023.7/src/unipi_control/neuron.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-import importlib
 from typing import List
-
-from pymodbus.register_read_message import ReadInputRegistersResponse
+from typing import Optional
 
 from unipi_control.config import Config
 from unipi_control.config import HardwareData
 from unipi_control.config import HardwareDefinition
 from unipi_control.config import HardwareType
 from unipi_control.config import LogPrefix
 from unipi_control.config import logger
 from unipi_control.features import DigitalInput
 from unipi_control.features import DigitalOutput
 from unipi_control.features import FeatureMap
 from unipi_control.features import Led
 from unipi_control.features import Relay
 from unipi_control.modbus import ModbusCacheData
 from unipi_control.modbus import ModbusClient
+from unipi_control.modbus import check_modbus_call
+from unipi_control.extensions.eastron import EastronSDM120M
+
+from pymodbus.pdu import ModbusResponse
 
 
 class Board:
     """Class to parse board features and register it to the ``FeatureMap``."""
 
     def __init__(self, neuron, versions: list, major_group: int) -> None:
         """Initialize board.
@@ -136,32 +138,36 @@
         await self.read_extensions()
 
     async def read_boards(self) -> None:
         """Scan Modbus TCP and initialize Unipi Neuron board."""
         logger.info("%s Reading SPI boards", LogPrefix.MODBUS)
 
         for index in (1, 2, 3):
-            response: ReadInputRegistersResponse = await self.modbus_client.tcp.read_input_registers(
-                address=1000, count=1, slave=index
+            response: Optional[ModbusResponse] = await check_modbus_call(
+                self.modbus_client.tcp.read_input_registers,
+                data={
+                    "address": 1000,
+                    "count": 1,
+                    "slave": index,
+                },
             )
 
-            if response.isError():
-                logger.info("%s No board on SPI %s", LogPrefix.MODBUS, index)
-            else:
-                board = Board(neuron=self, versions=response.registers, major_group=index)
+            if response:
+                board = Board(neuron=self, versions=getattr(response, "registers"), major_group=index)
                 board.parse_features()
 
                 self.boards.append(board)
+            else:
+                logger.info("%s No board on SPI %s", LogPrefix.MODBUS, index)
 
         await self.modbus_cache_data.scan("tcp", hardware_types=[HardwareType.NEURON])
 
     async def read_extensions(self) -> None:
         """Scan Modbus RTU and initialize extension classes."""
         logger.info("%s Reading extensions", LogPrefix.MODBUS)
 
         for definition in self.hardware["definitions"][1:]:
-            await getattr(
-                importlib.import_module(f"unipi_control.extensions.{definition.manufacturer.lower()}"),
-                f"{definition.manufacturer}{definition.model}",
-            )(neuron=self, definition=definition).init()
+            if definition.manufacturer.lower() == "eastron":
+                if definition.model == "SDM120M":
+                    await EastronSDM120M(neuron=self, definition=definition).init()
 
         await self.modbus_cache_data.scan("serial", hardware_types=[HardwareType.EXTENSION])
```

### Comparing `unipi-control-2023.6/src/unipi_control/unipi_control.py` & `unipi-control-2023.7/src/unipi_control/unipi_control.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 import argparse
 import asyncio
-import sys
 import uuid
 from asyncio import Task
 from contextlib import AsyncExitStack
 from pathlib import Path
-from typing import Final
 from typing import Optional
 from typing import Set
 
+import sys
 from asyncio_mqtt import Client
 from pymodbus.client import AsyncModbusSerialClient
 from pymodbus.client import AsyncModbusTcpClient
+
 from superbox_utils.argparse import init_argparse
 from superbox_utils.config.exception import ConfigException
 from superbox_utils.core.exception import UnexpectedException
 from superbox_utils.mqtt.connect import mqtt_connect
 from superbox_utils.text.text import slugify
-
 from unipi_control.config import Config
+from unipi_control.config import DEFAULT_CONFIG_PATH
 from unipi_control.config import LogPrefix
 from unipi_control.config import logger
 from unipi_control.integrations.covers import CoverMap
-from unipi_control.log import LOG_NAME
 from unipi_control.modbus import ModbusClient
 from unipi_control.mqtt.discovery.binary_sensors import HassBinarySensorsMqttPlugin
 from unipi_control.mqtt.discovery.covers import HassCoversMqttPlugin
 from unipi_control.mqtt.discovery.sensors import HassSensorsMqttPlugin
 from unipi_control.mqtt.discovery.switches import HassSwitchesMqttPlugin
 from unipi_control.mqtt.features import MeterFeaturesMqttPlugin
 from unipi_control.mqtt.features import NeuronFeaturesMqttPlugin
@@ -39,16 +38,14 @@
     """Control Unipi I/O directly with MQTT commands.
 
     Unipi Control use Modbus for fast access to the I/O and provide MQTT
     topics for reading and writing the circuits. Optionally you can enable
     the Home Assistant MQTT discovery for binary sensors, sensors, switches and covers.
     """
 
-    NAME: Final[str] = "unipi-control"
-
     def __init__(self, config: Config, modbus_client: ModbusClient) -> None:
         self.config: Config = config
         self.modbus_client: ModbusClient = modbus_client
         self.neuron: Neuron = Neuron(config=config, modbus_client=modbus_client)
 
     async def _init_tasks(self, stack: AsyncExitStack, mqtt_client: Client) -> None:
         tasks: Set[Task] = set()
@@ -129,48 +126,62 @@
         Arguments as list.
 
     Returns
     -------
     Argparse namespace
     """
     parser: argparse.ArgumentParser = init_argparse(description="Control Unipi I/O with MQTT commands")
+    parser.add_argument(
+        "-c",
+        "--config",
+        action="store",
+        default=DEFAULT_CONFIG_PATH,
+        help=f"path to the configuration (default: {DEFAULT_CONFIG_PATH})",
+    )
     parser.add_argument("--version", action="version", version=f"%(prog)s {__version__}")
 
     return parser.parse_args(args)
 
 
 def main() -> None:
-    """Entrypoint for Unipi Control script."""
+    """Entrypoint for Unipi Control."""
     unipi_control: Optional[UnipiControl] = None
 
     try:
         args: argparse.Namespace = parse_args(sys.argv[1:])
 
-        config: Config = Config()
-        config.logging.init(LOG_NAME, log=args.log, log_path=Path("/var/log"), verbose=args.verbose)
+        config: Config = Config(config_base_path=Path(args.config))
+        config.logging.init(log=args.log, verbose=args.verbose)
 
         unipi_control = UnipiControl(
             config=config,
             modbus_client=ModbusClient(
-                tcp=AsyncModbusTcpClient(host="localhost"),
+                tcp=AsyncModbusTcpClient(
+                    host="localhost",
+                    timeout=0.5,
+                    retries=3,
+                    retry_on_empty=True,
+                ),
                 serial=AsyncModbusSerialClient(
                     port="/dev/extcomm/0/0",
                     baudrate=config.modbus.baud_rate,
                     parity=config.modbus.parity,
-                    timeout=30,
+                    timeout=1,
+                    retries=3,
+                    retry_on_empty=True,
                 ),
             ),
         )
 
         asyncio.run(unipi_control.run())
     except ConfigException as error:
-        logger.error("%s %s", LogPrefix.CONFIG, error)
+        logger.critical("%s %s", LogPrefix.CONFIG, error)
         sys.exit(1)
     except UnexpectedException as error:
-        logger.error(error)
+        logger.critical(error)
         sys.exit(1)
     except KeyboardInterrupt:
         pass
     except asyncio.CancelledError:
         pass
     finally:
         if unipi_control:
```

### Comparing `unipi-control-2023.6/src/unipi_control.egg-info/PKG-INFO` & `unipi-control-2023.7/src/unipi_control.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,137 @@
 Metadata-Version: 2.1
 Name: unipi-control
-Version: 2023.6
-Summary: Control Unipi I/O directly with MQTT commands and without Evok.
-Home-page: https://github.com/mh-superbox/unipi-control
+Version: 2023.7
+Summary: Control Unipi I/O directly with MQTT commands.
+Home-page: https://github.com/superbox-dev/unipi-control
 Author: Michael Hacker
 Author-email: mh@superbox.one
-License: MIT
+License: Apache-2.0 license
+Project-URL: Source Code, https://github.com/superbox-dev/unipi-control
+Project-URL: Bug Reports, https://github.com/superbox-dev/unipi-control/issues
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Topic :: System :: Networking
+Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![license-url](https://img.shields.io/npm/l/make-coverage-badge.svg)](https://opensource.org/licenses/MIT)
-![coverage-badge](https://raw.githubusercontent.com/mh-superbox/unipi-control/main/coverage.svg)
+[![license-url](https://img.shields.io/badge/license-Apache%202-yellowgreen)](https://opensource.org/license/apache-2-0/)
+![coverage-badge](https://raw.githubusercontent.com/superbox-dev/unipi-control/main/coverage.svg)
 ![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)
 ![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)
 ![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
+![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
+
+# Unipi Control
+
+Control Unipi I/O directly with MQTT commands and without [Evok](https://github.com/UniPiTechnology/evok). Unipi Control use Modbus for fast access to the I/O and provide MQTT topics for reading and writing the circuits. Optionally you can enable the Home Assistant MQTT discovery for binary sensors, sensors, switches and covers.
 
 ### Support me if you like this project 😀
 
 I want to extend the code to support Unipi extensions modules.
 The necessary hardware is also required for this.
 
-[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/mhacker)
-
-# Unipi Control
+[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/F2F0KXO6D)
 
-Control Unipi I/O directly with MQTT commands and without [Evok](https://github.com/UniPiTechnology/evok). Unipi Control use Modbus for fast access to the I/O and provide MQTT topics for reading and writing the circuits. Optionally you can enable the Home Assistant MQTT discovery for binary sensors, sensors, switches and covers.
+[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/superbox_dev)
 
 ## Supported hardware
 
-* Unipi Neuron L203
+* Tested:
+  * Unipi Neuron
+    * L203
+* Untested:
+  * Unipi Neuron
+    * S103
+    * S103-G
+    * M103
+    * M203
+    * M523
+    * L523
+    * L533
+  * Unipi Patron
+    * Patron S107
+    * Patron S117
+    * Patron S167
+    * Patron M207
+    * Patron M267
+    * Patron M527
+    * Patron M567
+    * Patron S207
+    * Patron L207
+    * Patron L527
 * External Modbus RTU devices
   * [Eastron SDM120M](https://www.eastroneurope.com/products/view/sdm120modbus)
 
+If you tried an untested Unipi device then please let me know the result to update this page.
+
 If you have an Unipi device, that is not supported, then contact me.
 
 ## Getting Started
 
+### Recommended installation (Only for Unipi Neuron)
+
+Use the [Unipi Control OS](https://github.com/superbox-dev/unipi-control-os).
+
+### Alternative installation (Debian based systems)
+
 **Requirements:**
 
-* Unipi Neuron Kernel Module and Unipi tools
-  * Use the officially APT mirror (https://repo.unipi.technology/debian/) from Unipi Technology
-  * Or compile it
-    * https://github.com/UniPiTechnology/unipi-kernel
-    * https://github.com/UniPiTechnology/unipi-tools
-* Python 3.8
+* Unipi Neuron Kernel Module and Unipi tools (Use the officially APT mirror (https://repo.unipi.technology/debian/) from Unipi Technology)
+* Python >= 3.8
 
 Install **Unipi Control** with `pip`.
 
 ```shell
 $ python -m venv /opt/.venv
 $ /opt/.venv/bin/pip install unipi-control
 ```
 
-Copy the [config files](src/unipi_control/config/etc) to your `/etc` directory and start the systemd service:
+Copy the [config files](opkg/data/local/etc/unipi) to your `/etc/unipi` directory and
+create the systemd service `/etc/systemd/system/unipi-control.service` with following content:
+
+```
+[Unit]
+Description=Unipi Control
+After=multi-user.target
+
+[Service]
+Type=simple
+ExecStart=/opt/.venv/bin/unipi-control --log systemd
+Environment=PYTHONUNBUFFERED=1
+
+[Install]
+WantedBy=multi-user.target
+```
+
+Enable and start the systemd service:
 
 ```shell
+$ systemctl --system daemon-reload
 $ systemctl enable unipi-control.service
 $ systemctl start unipi-control.service
 ```
 
+## Arguments
+
+| Argument   | Description                                                           |
+|------------|-----------------------------------------------------------------------|
+| `--config` | path to the configuration (default: /etc/unipi)                       |
+| `-v`       | verbose mode: multiple -v options increase the verbosity (maximum: 4) |
+
+
 ## Configuration
 
 You can set the client settings in the `/etc/unipi/control.yaml`.
 
 ### Device
 
 | Key    | Value                                                                                                                                                               |
@@ -281,17 +341,22 @@
 ## Development
 
 For development, you must clone the git repository and install **Unipi Control** with `pipenv`.
 
 ```shell
 $ git clone https://github.com/mh-superbox/unipi-control.git
 $ cd unipi-control
-~/unipi-control$ pipenv install --deploy --dev 
-~/unipi-control$ pipenv run pip install -e .
+~/unipi-control$ make install-dev
+```
+
+Copy the [config files](opkg/data/local/etc/unipi) to your `/etc/unipi` directory
+and activate your virtualenv with:
+
+```shell
+~/unipi-control$ source .venv/bin/activate
 ```
 
-Copy the config files to your `/etc` directory.
-Now you can start unipi-control with `pipenv run unipi-control`.
+Now you can start unipi-control with `unipi-control`.
 
 ## Extras
 
 I have written a Home Assistant blueprint automation to control covers with binary sensors. Take a look in the [extras](extras) directory.
```

### Comparing `unipi-control-2023.6/src/unipi_control.egg-info/SOURCES.txt` & `unipi-control-2023.7/src/unipi_control.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
+requirements.txt
 setup.cfg
 setup.py
+extras/homeassistant/blueprints/automation/cover/control.yaml
+extras/homeassistant/blueprints/automation/cover/simple_cover_control.yaml
 src/unipi_control/__init__.py
 src/unipi_control/config.py
 src/unipi_control/features.py
 src/unipi_control/log.py
 src/unipi_control/modbus.py
-src/unipi_control/model_info.py
 src/unipi_control/neuron.py
 src/unipi_control/unipi_control.py
 src/unipi_control/version.py
 src/unipi_control.egg-info/PKG-INFO
 src/unipi_control.egg-info/SOURCES.txt
 src/unipi_control.egg-info/dependency_links.txt
 src/unipi_control.egg-info/entry_points.txt
 src/unipi_control.egg-info/requires.txt
 src/unipi_control.egg-info/top_level.txt
-src/unipi_control/config/etc/systemd/system/unipi-control.service
-src/unipi_control/config/etc/unipi/control.yaml
-src/unipi_control/config/etc/unipi/control.yaml.example
-src/unipi_control/config/etc/unipi/hardware/extensions/Eastron_SDM120M.yaml
-src/unipi_control/config/etc/unipi/hardware/extensions/xS11.yaml
-src/unipi_control/config/etc/unipi/hardware/neuron/L203.yaml
 src/unipi_control/extensions/__init__.py
 src/unipi_control/extensions/eastron.py
 src/unipi_control/integrations/__init__.py
 src/unipi_control/integrations/covers.py
 src/unipi_control/mqtt/__init__.py
 src/unipi_control/mqtt/features.py
 src/unipi_control/mqtt/discovery/__init__.py
 src/unipi_control/mqtt/discovery/binary_sensors.py
 src/unipi_control/mqtt/discovery/covers.py
 src/unipi_control/mqtt/discovery/mixin.py
 src/unipi_control/mqtt/discovery/sensors.py
 src/unipi_control/mqtt/discovery/switches.py
 src/unipi_control/mqtt/integrations/__init__.py
-src/unipi_control/mqtt/integrations/covers.py
+src/unipi_control/mqtt/integrations/covers.py
+src/unipi_control/tools/__init__.py
+src/unipi_control/tools/config_backup.py
+src/unipi_control/tools/config_converter.py
+src/unipi_control/tools/model_info.py
```

