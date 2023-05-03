# Comparing `tmp/messageflux-0.2.3.tar.gz` & `tmp/messageflux-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "messageflux-0.2.3.tar", last modified: Tue May  2 17:06:37 2023, max compression
+gzip compressed data, was "messageflux-0.2.4.tar", last modified: Wed May  3 16:01:10 2023, max compression
```

## Comparing `messageflux-0.2.3.tar` & `messageflux-0.2.4.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:37.641652 messageflux-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-02 17:06:27.000000 messageflux-0.2.3/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-02 17:06:27.000000 messageflux-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-02 17:06:27.000000 messageflux-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-05-02 17:06:37.641652 messageflux-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-05-02 17:06:27.000000 messageflux-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 17:06:28.000000 messageflux-0.2.3/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:37.633652 messageflux-0.2.3/_custom_build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:27.000000 messageflux-0.2.3/_custom_build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-02 17:06:27.000000 messageflux-0.2.3/_custom_build/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-02 17:06:27.000000 messageflux-0.2.3/_custom_build/make_all_extra_requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:37.633652 messageflux-0.2.3/messageflux/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/base_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/fastmessage_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:37.633652 messageflux-0.2.3/messageflux/iodevices/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:37.637652 messageflux-0.2.3/messageflux/iodevices/base/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/base/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/base/input_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/base/input_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/base/output_devices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:37.637652 messageflux-0.2.3/messageflux/iodevices/collection_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/collection_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/collection_device_wrapper/collection_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/collection_device_wrapper/collection_output_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:37.637652 messageflux-0.2.3/messageflux/iodevices/failover_output_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/failover_output_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:37.637652 messageflux-0.2.3/messageflux/iodevices/file_system/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/file_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/file_system/file_system_device_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24466 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/file_system/file_system_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/file_system/file_system_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/file_system/file_system_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:37.637652 messageflux-0.2.3/messageflux/iodevices/in_memory_device/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/in_memory_device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/in_memory_device/in_memory_device_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:37.637652 messageflux-0.2.3/messageflux/iodevices/message_store_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/message_store_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/message_store_device_wrapper/message_store_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:37.637652 messageflux-0.2.3/messageflux/iodevices/objectstorage/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/objectstorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/objectstorage/s3_message_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:37.637652 messageflux-0.2.3/messageflux/iodevices/objectstorage/s3api/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/objectstorage/s3api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/objectstorage/s3api/s3bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/objectstorage/s3api/s3client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:37.637652 messageflux-0.2.3/messageflux/iodevices/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/rabbitmq/fs_poison_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14045 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16736 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:37.637652 messageflux-0.2.3/messageflux/iodevices/round_robin_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/round_robin_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:37.641652 messageflux-0.2.3/messageflux/iodevices/short_circuit_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/short_circuit_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/short_circuit_device_wrapper/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:37.641652 messageflux-0.2.3/messageflux/iodevices/transformer_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/transformer_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:37.641652 messageflux-0.2.3/messageflux/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/logging/LogType.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/logging/bulk_rotating_device_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/logging/bulk_rotating_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/logging/bulk_rotating_handler_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/logging/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/message_handling_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/metadata_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:37.641652 messageflux-0.2.3/messageflux/multiprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/multiprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/multiprocessing/multiprocessrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/multiprocessing/singleprocesshandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/pipeline_service.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/server_loop_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:37.641652 messageflux-0.2.3/messageflux/service_addons/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/service_addons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/service_addons/loop_health_addon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:37.641652 messageflux-0.2.3/messageflux/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-02 17:06:27.000000 messageflux-0.2.3/messageflux/utils/filesystem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:37.633652 messageflux-0.2.3/messageflux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-05-02 17:06:37.000000 messageflux-0.2.3/messageflux.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-02 17:06:37.000000 messageflux-0.2.3/messageflux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:06:37.000000 messageflux-0.2.3/messageflux.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-02 17:06:37.000000 messageflux-0.2.3/messageflux.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 17:06:37.000000 messageflux-0.2.3/messageflux.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-02 17:06:27.000000 messageflux-0.2.3/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-02 17:06:27.000000 messageflux-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-02 17:06:27.000000 messageflux-0.2.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-02 17:06:37.000000 messageflux-0.2.3/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-02 17:06:27.000000 messageflux-0.2.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 17:06:27.000000 messageflux-0.2.3/requirements-fastmessage.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-02 17:06:27.000000 messageflux-0.2.3/requirements-objectstorage.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-02 17:06:27.000000 messageflux-0.2.3/requirements-rabbitmq.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:06:27.000000 messageflux-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 17:06:37.641652 messageflux-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:01:10.845889 messageflux-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-03 16:00:59.000000 messageflux-0.2.4/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 16:00:59.000000 messageflux-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-03 16:00:59.000000 messageflux-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-05-03 16:01:10.845889 messageflux-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-05-03 16:00:59.000000 messageflux-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 16:01:00.000000 messageflux-0.2.4/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:01:10.837890 messageflux-0.2.4/_custom_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 16:00:59.000000 messageflux-0.2.4/_custom_build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-03 16:00:59.000000 messageflux-0.2.4/_custom_build/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-03 16:00:59.000000 messageflux-0.2.4/_custom_build/make_all_extra_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:01:10.837890 messageflux-0.2.4/messageflux/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/base_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/fastmessage_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:01:10.837890 messageflux-0.2.4/messageflux/iodevices/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:01:10.837890 messageflux-0.2.4/messageflux/iodevices/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/base/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/base/input_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/base/input_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/base/output_devices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:01:10.837890 messageflux-0.2.4/messageflux/iodevices/collection_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/collection_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/collection_device_wrapper/collection_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/collection_device_wrapper/collection_output_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:01:10.837890 messageflux-0.2.4/messageflux/iodevices/failover_output_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/failover_output_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:01:10.841889 messageflux-0.2.4/messageflux/iodevices/file_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/file_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/file_system/file_system_device_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24466 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/file_system/file_system_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/file_system/file_system_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/file_system/file_system_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:01:10.841889 messageflux-0.2.4/messageflux/iodevices/in_memory_device/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/in_memory_device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/in_memory_device/in_memory_device_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:01:10.841889 messageflux-0.2.4/messageflux/iodevices/message_store_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/message_store_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/message_store_device_wrapper/message_store_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:01:10.841889 messageflux-0.2.4/messageflux/iodevices/objectstorage/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/objectstorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/objectstorage/s3_message_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:01:10.841889 messageflux-0.2.4/messageflux/iodevices/objectstorage/s3api/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/objectstorage/s3api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/objectstorage/s3api/s3bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/objectstorage/s3api/s3client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:01:10.841889 messageflux-0.2.4/messageflux/iodevices/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/rabbitmq/fs_poison_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14045 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16736 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:01:10.841889 messageflux-0.2.4/messageflux/iodevices/round_robin_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/round_robin_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:01:10.841889 messageflux-0.2.4/messageflux/iodevices/short_circuit_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/short_circuit_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/short_circuit_device_wrapper/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:01:10.841889 messageflux-0.2.4/messageflux/iodevices/transformer_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/transformer_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:01:10.845889 messageflux-0.2.4/messageflux/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/logging/LogType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/logging/bulk_rotating_device_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/logging/bulk_rotating_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/logging/bulk_rotating_handler_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/logging/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/message_handling_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/metadata_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:01:10.845889 messageflux-0.2.4/messageflux/multiprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/multiprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/multiprocessing/multiprocessrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/multiprocessing/singleprocesshandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/pipeline_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/server_loop_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:01:10.845889 messageflux-0.2.4/messageflux/service_addons/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/service_addons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/service_addons/loop_health_addon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:01:10.845889 messageflux-0.2.4/messageflux/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-03 16:00:59.000000 messageflux-0.2.4/messageflux/utils/filesystem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:01:10.837890 messageflux-0.2.4/messageflux.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-05-03 16:01:10.000000 messageflux-0.2.4/messageflux.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-03 16:01:10.000000 messageflux-0.2.4/messageflux.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 16:01:10.000000 messageflux-0.2.4/messageflux.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-03 16:01:10.000000 messageflux-0.2.4/messageflux.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 16:01:10.000000 messageflux-0.2.4/messageflux.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-03 16:00:59.000000 messageflux-0.2.4/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-03 16:00:59.000000 messageflux-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-03 16:00:59.000000 messageflux-0.2.4/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-03 16:01:10.000000 messageflux-0.2.4/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-03 16:00:59.000000 messageflux-0.2.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 16:00:59.000000 messageflux-0.2.4/requirements-fastmessage.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-03 16:00:59.000000 messageflux-0.2.4/requirements-objectstorage.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-03 16:00:59.000000 messageflux-0.2.4/requirements-rabbitmq.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 16:00:59.000000 messageflux-0.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 16:01:10.845889 messageflux-0.2.4/setup.cfg
```

### Comparing `messageflux-0.2.3/LICENSE` & `messageflux-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/PKG-INFO` & `messageflux-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messageflux
-Version: 0.2.3
+Version: 0.2.4
 Author-email: Aviv Salem <avivsalem@gmail.com>
 Maintainer-email: Aviv Salem <avivsalem@gmail.com>, Nir Schulman <narsssx@gmail.com>, Rafael Zilberman <Zilberman.rafi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Avivsalem/MessageFlux/
 Project-URL: Documentation, https://messageflux.readthedocs.io/
 Platform: win32
 Platform: linux
```

### Comparing `messageflux-0.2.3/README.md` & `messageflux-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/_custom_build/make_all_extra_requirements.py` & `messageflux-0.2.4/_custom_build/make_all_extra_requirements.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/base_service.py` & `messageflux-0.2.4/messageflux/base_service.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/fastmessage_handler.py` & `messageflux-0.2.4/messageflux/fastmessage_handler.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/base/__init__.py` & `messageflux-0.2.4/messageflux/iodevices/base/__init__.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/base/common.py` & `messageflux-0.2.4/messageflux/iodevices/base/common.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/base/input_devices.py` & `messageflux-0.2.4/messageflux/iodevices/base/input_devices.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/base/input_transaction.py` & `messageflux-0.2.4/messageflux/iodevices/base/input_transaction.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/base/output_devices.py` & `messageflux-0.2.4/messageflux/iodevices/base/output_devices.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/collection_device_wrapper/collection_input_device.py` & `messageflux-0.2.4/messageflux/iodevices/collection_device_wrapper/collection_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/collection_device_wrapper/collection_output_device.py` & `messageflux-0.2.4/messageflux/iodevices/collection_device_wrapper/collection_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py` & `messageflux-0.2.4/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/file_system/__init__.py` & `messageflux-0.2.4/messageflux/iodevices/file_system/__init__.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/file_system/file_system_device_manager_base.py` & `messageflux-0.2.4/messageflux/iodevices/file_system/file_system_device_manager_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/file_system/file_system_input_device.py` & `messageflux-0.2.4/messageflux/iodevices/file_system/file_system_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/file_system/file_system_output_device.py` & `messageflux-0.2.4/messageflux/iodevices/file_system/file_system_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/file_system/file_system_serializer.py` & `messageflux-0.2.4/messageflux/iodevices/file_system/file_system_serializer.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/in_memory_device/in_memory_device_manager.py` & `messageflux-0.2.4/messageflux/iodevices/in_memory_device/in_memory_device_manager.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py` & `messageflux-0.2.4/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/message_store_device_wrapper/message_store_base.py` & `messageflux-0.2.4/messageflux/iodevices/message_store_device_wrapper/message_store_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py` & `messageflux-0.2.4/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py` & `messageflux-0.2.4/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py` & `messageflux-0.2.4/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/objectstorage/s3_message_store.py` & `messageflux-0.2.4/messageflux/iodevices/objectstorage/s3_message_store.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/objectstorage/s3api/s3bucket.py` & `messageflux-0.2.4/messageflux/iodevices/objectstorage/s3api/s3bucket.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/objectstorage/s3api/s3client.py` & `messageflux-0.2.4/messageflux/iodevices/objectstorage/s3api/s3client.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/rabbitmq/fs_poison_counter.py` & `messageflux-0.2.4/messageflux/iodevices/rabbitmq/fs_poison_counter.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py` & `messageflux-0.2.4/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py` & `messageflux-0.2.4/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py` & `messageflux-0.2.4/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py` & `messageflux-0.2.4/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py` & `messageflux-0.2.4/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/short_circuit_device_wrapper/common.py` & `messageflux-0.2.4/messageflux/iodevices/short_circuit_device_wrapper/common.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py` & `messageflux-0.2.4/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py` & `messageflux-0.2.4/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py` & `messageflux-0.2.4/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py` & `messageflux-0.2.4/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py` & `messageflux-0.2.4/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/logging/bulk_rotating_device_handler.py` & `messageflux-0.2.4/messageflux/logging/bulk_rotating_device_handler.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/logging/bulk_rotating_file_handler.py` & `messageflux-0.2.4/messageflux/logging/bulk_rotating_file_handler.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/logging/bulk_rotating_handler_base.py` & `messageflux-0.2.4/messageflux/logging/bulk_rotating_handler_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/message_handling_service.py` & `messageflux-0.2.4/messageflux/message_handling_service.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/multiprocessing/multiprocessrunner.py` & `messageflux-0.2.4/messageflux/multiprocessing/multiprocessrunner.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/multiprocessing/singleprocesshandler.py` & `messageflux-0.2.4/messageflux/multiprocessing/singleprocesshandler.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/pipeline_service.py` & `messageflux-0.2.4/messageflux/pipeline_service.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/server_loop_service.py` & `messageflux-0.2.4/messageflux/server_loop_service.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/service_addons/loop_health_addon.py` & `messageflux-0.2.4/messageflux/service_addons/loop_health_addon.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/utils/__init__.py` & `messageflux-0.2.4/messageflux/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/utils/context.py` & `messageflux-0.2.4/messageflux/utils/context.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux/utils/filesystem.py` & `messageflux-0.2.4/messageflux/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/messageflux.egg-info/PKG-INFO` & `messageflux-0.2.4/messageflux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messageflux
-Version: 0.2.3
+Version: 0.2.4
 Author-email: Aviv Salem <avivsalem@gmail.com>
 Maintainer-email: Aviv Salem <avivsalem@gmail.com>, Nir Schulman <narsssx@gmail.com>, Rafael Zilberman <Zilberman.rafi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Avivsalem/MessageFlux/
 Project-URL: Documentation, https://messageflux.readthedocs.io/
 Platform: win32
 Platform: linux
```

### Comparing `messageflux-0.2.3/messageflux.egg-info/SOURCES.txt` & `messageflux-0.2.4/messageflux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `messageflux-0.2.3/pyproject.toml` & `messageflux-0.2.4/pyproject.toml`

 * *Files identical despite different names*

