# Comparing `tmp/python_ember_mug-0.7.0b6.tar.gz` & `tmp/python_ember_mug-0.7.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_ember_mug-0.7.0b6.tar", max compression
+gzip compressed data, was "python_ember_mug-0.7.0b7.tar", max compression
```

## Comparing `python_ember_mug-0.7.0b6.tar` & `python_ember_mug-0.7.0b7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/LICENSE
--rw-r--r--   0        0        0     5282 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/README.md
--rwxr-xr-x   0        0        0      189 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/ember_mug/__init__.py
--rw-r--r--   0        0        0      106 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/ember_mug/__main__.py
--rw-r--r--   0        0        0      296 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/ember_mug/cli/__init__.py
--rw-r--r--   0        0        0     8933 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/ember_mug/cli/commands.py
--rw-r--r--   0        0        0     2910 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/ember_mug/cli/helpers.py
--rw-r--r--   0        0        0     5436 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/ember_mug/consts.py
--rw-r--r--   0        0        0     8946 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/ember_mug/data.py
--rw-r--r--   0        0        0      605 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/ember_mug/formatting.py
--rw-r--r--   0        0        0    18898 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/ember_mug/mug.py
--rw-r--r--   0        0        0     2212 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/ember_mug/scanner.py
--rw-r--r--   0        0        0     3528 2023-04-29 16:10:28.941926 python_ember_mug-0.7.0b6/ember_mug/utils.py
--rw-r--r--   0        0        0     2896 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/pyproject.toml
--rw-r--r--   0        0        0       46 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/tests/cli/__init__.py
--rw-r--r--   0        0        0     7846 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/tests/cli/test_commands.py
--rw-r--r--   0        0        0     2663 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/tests/cli/test_helpers.py
--rw-r--r--   0        0        0     1199 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/tests/conftest.py
--rw-r--r--   0        0        0    19254 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/tests/test_connection.py
--rw-r--r--   0        0        0     1115 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/tests/test_consts.py
--rw-r--r--   0        0        0     2395 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/tests/test_data.py
--rw-r--r--   0        0        0      534 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/tests/test_formatting.py
--rw-r--r--   0        0        0     3428 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/tests/test_mug_data.py
--rw-r--r--   0        0        0     2012 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/tests/test_scanner.py
--rw-r--r--   0        0        0     2289 2023-04-29 16:10:28.945926 python_ember_mug-0.7.0b6/tests/test_utils.py
--rw-r--r--   0        0        0     6490 1970-01-01 00:00:00.000000 python_ember_mug-0.7.0b6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-03 00:16:50.110255 python_ember_mug-0.7.0b7/LICENSE
+-rw-r--r--   0        0        0     5282 2023-05-03 00:16:50.110255 python_ember_mug-0.7.0b7/README.md
+-rwxr-xr-x   0        0        0      189 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/ember_mug/__init__.py
+-rw-r--r--   0        0        0      106 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/ember_mug/__main__.py
+-rw-r--r--   0        0        0      296 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/ember_mug/cli/__init__.py
+-rw-r--r--   0        0        0     8933 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/ember_mug/cli/commands.py
+-rw-r--r--   0        0        0     2910 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/ember_mug/cli/helpers.py
+-rw-r--r--   0        0        0     5436 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/ember_mug/consts.py
+-rw-r--r--   0        0        0     8946 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/ember_mug/data.py
+-rw-r--r--   0        0        0      605 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/ember_mug/formatting.py
+-rw-r--r--   0        0        0    19423 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/ember_mug/mug.py
+-rw-r--r--   0        0        0     2212 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/ember_mug/scanner.py
+-rw-r--r--   0        0        0     3528 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/ember_mug/utils.py
+-rw-r--r--   0        0        0     2896 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/tests/cli/__init__.py
+-rw-r--r--   0        0        0     7846 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/tests/cli/test_commands.py
+-rw-r--r--   0        0        0     2663 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/tests/cli/test_helpers.py
+-rw-r--r--   0        0        0     1199 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/tests/conftest.py
+-rw-r--r--   0        0        0    20460 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/tests/test_connection.py
+-rw-r--r--   0        0        0     1115 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/tests/test_consts.py
+-rw-r--r--   0        0        0     2395 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/tests/test_data.py
+-rw-r--r--   0        0        0      534 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/tests/test_formatting.py
+-rw-r--r--   0        0        0     3428 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/tests/test_mug_data.py
+-rw-r--r--   0        0        0     2012 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/tests/test_scanner.py
+-rw-r--r--   0        0        0     2289 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/tests/test_utils.py
+-rw-r--r--   0        0        0     6490 1970-01-01 00:00:00.000000 python_ember_mug-0.7.0b7/PKG-INFO
```

### Comparing `python_ember_mug-0.7.0b6/LICENSE` & `python_ember_mug-0.7.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b6/README.md` & `python_ember_mug-0.7.0b7/README.md`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b6/ember_mug/cli/commands.py` & `python_ember_mug-0.7.0b7/ember_mug/cli/commands.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b6/ember_mug/cli/helpers.py` & `python_ember_mug-0.7.0b7/ember_mug/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b6/ember_mug/consts.py` & `python_ember_mug-0.7.0b7/ember_mug/consts.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b6/ember_mug/data.py` & `python_ember_mug-0.7.0b7/ember_mug/data.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b6/ember_mug/formatting.py` & `python_ember_mug-0.7.0b7/ember_mug/formatting.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b6/ember_mug/mug.py` & `python_ember_mug-0.7.0b7/ember_mug/mug.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,25 +126,23 @@
                     'If your mug is still in pairing mode (blinking blue) tap the button on the bottom to exit.',
                 )
             self._client = client
             await self.subscribe()
 
     async def _read(self, characteristic: MugCharacteristic) -> bytearray:
         """Helper to read characteristic from Mug."""
-        if self._operation_lock.locked():
-            logger.debug("Operation already in progress. waiting for it to complete")
+        self._check_operation_lock()
         async with self._operation_lock:
             data = await self._client.read_gatt_char(characteristic.uuid)
             logger.debug("Read attribute '%s' with value '%s'", characteristic, data)
             return data
 
     async def _write(self, characteristic: MugCharacteristic, data: bytearray) -> None:
         """Helper to write characteristic to Mug."""
-        if self._operation_lock.locked():
-            logger.debug("Operation already in progress. Waiting for it to complete")
+        self._check_operation_lock()
         async with self._operation_lock:
             await self._ensure_connection()
             try:
                 await self._client.write_gatt_char(characteristic.uuid, data)
                 logger.debug("Wrote '%s' to attribute '%s'", data, characteristic)
             except BleakError as e:
                 logger.error("Failed to write '%s' to attribute '%s': %s", data, characteristic, e)
@@ -170,14 +168,19 @@
 
     def _fire_callbacks(self) -> None:
         """Fire the callbacks."""
         logger.debug("Firing callbacks: %s", self._callbacks)
         for callback in self._callbacks:
             callback(self.data)
 
+    def _check_operation_lock(self) -> None:
+        """Check and print message if lock occupied."""
+        if self._operation_lock.locked():
+            logger.debug("Operation already in progress. waiting for it to complete")
+
     def register_callback(self, callback: Callable[[MugData], None]) -> Callable[[], None]:
         """Register a callback to be called when the state changes."""
         if existing_unregister_callback := self._callbacks.get(callback):
             logger.debug("Callback %s already registered", callback)
             return existing_unregister_callback
 
         def unregister_callback() -> None:
@@ -185,14 +188,24 @@
                 del self._callbacks[callback]
             logger.debug("Unregistered callback: %s", callback)
 
         self._callbacks[callback] = unregister_callback
         logger.debug("Registered callback: %s", callback)
         return unregister_callback
 
+    async def discover_services(self) -> dict[str, Any]:
+        """Discover services for development or debugging.
+
+        Call discover_services with this client, ensuring the connection is active first.
+        """
+        self._check_operation_lock()
+        async with self._operation_lock:
+            await self._ensure_connection()
+            return await discover_services(self._client)
+
     async def get_meta(self) -> MugMeta:
         """Fetch Meta info from the mug (Serial number and ID)."""
         return MugMeta.from_bytes(await self._read(MugCharacteristic.MUG_ID))
 
     async def get_battery(self) -> BatteryInfo:
         """Get Battery percent from mug gatt."""
         return BatteryInfo.from_bytes(await self._read(MugCharacteristic.BATTERY))
@@ -238,16 +251,16 @@
             raise NotImplementedError('The Mug and Cup do not have a volume level attribute')
         volume_bytes = await self._read(MugCharacteristic.VOLUME)
         volume_int = bytes_to_little_int(volume_bytes)
         return VolumeLevel.from_state(volume_int)
 
     async def set_volume_level(self, volume: int | VolumeLevel) -> None:
         """Set volume_level on Travel Mug."""
-        if volume not in (0, 1, 2):
-            raise ValueError('Volume level must be between 0 and 2 inclusively')
+        if not isinstance(volume, VolumeLevel) and isinstance(volume, int) and volume not in (0, 1, 2):
+            raise ValueError('Volume level value should be 0, 1, 2 or a VolumeLevel enum')
         if self.is_travel_mug is False:
             raise NotImplementedError('The Mug and Cup do not have a volume level attribute')
         volume_level = volume if isinstance(volume, VolumeLevel) else VolumeLevel.from_state(volume)
         await self._write(MugCharacteristic.VOLUME, bytearray([volume_level.state]))
         self.data.volume_level = volume_level
 
     async def get_liquid_state(self) -> LiquidState:
```

### Comparing `python_ember_mug-0.7.0b6/ember_mug/scanner.py` & `python_ember_mug-0.7.0b7/ember_mug/scanner.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b6/ember_mug/utils.py` & `python_ember_mug-0.7.0b7/ember_mug/utils.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b6/pyproject.toml` & `python_ember_mug-0.7.0b7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "python-ember-mug"
-version = "0.7.0b6"
+version = "0.7.0b7"
 homepage = "https://github.com/sopelj/python-ember-mug"
 description = "Python Library for Ember Mugs."
 authors = ["Jesse Sopel <jesse.sopel@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `python_ember_mug-0.7.0b6/tests/cli/test_commands.py` & `python_ember_mug-0.7.0b7/tests/cli/test_commands.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b6/tests/cli/test_helpers.py` & `python_ember_mug-0.7.0b7/tests/cli/test_helpers.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b6/tests/conftest.py` & `python_ember_mug-0.7.0b7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b6/tests/test_connection.py` & `python_ember_mug-0.7.0b7/tests/test_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,23 @@
 
 from unittest.mock import AsyncMock, Mock, patch
 
 import pytest
 from bleak import BleakError
 from bleak.backends.device import BLEDevice
 
-from ember_mug.consts import EMBER_MUG, EXTRA_ATTRS, INITIAL_ATTRS, UPDATE_ATTRS, MugCharacteristic, TemperatureUnit
+from ember_mug.consts import (
+    EMBER_MUG,
+    EXTRA_ATTRS,
+    INITIAL_ATTRS,
+    UPDATE_ATTRS,
+    MugCharacteristic,
+    TemperatureUnit,
+    VolumeLevel,
+)
 from ember_mug.data import Colour, Model
 from ember_mug.mug import EmberMug
 
 
 @patch('ember_mug.mug.IS_LINUX', True)
 async def test_adapter_with_bluez(ble_device: BLEDevice):
     mug = EmberMug(ble_device, adapter='hci0')
@@ -236,14 +244,42 @@
         ember_mug._ensure_connection.assert_called_once()
         ember_mug._client.write_gatt_char.assert_called_once_with(
             MugCharacteristic.LED.uuid,
             bytearray(b'\xf4\x00\xa1\xff'),
         )
 
 
+async def test_set_volume_level_travel_mug(ember_mug: AsyncMock):
+    ember_mug.is_travel_mug = True
+    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
+        await ember_mug.set_volume_level(VolumeLevel.HIGH)
+        ember_mug._ensure_connection.assert_called_once()
+        ember_mug._client.write_gatt_char.assert_called_once_with(
+            MugCharacteristic.VOLUME.uuid,
+            bytearray(b'\02'),
+        )
+        ember_mug._ensure_connection.reset_mock()
+        ember_mug._client.write_gatt_char.reset_mock()
+
+        await ember_mug.set_volume_level(0)
+        ember_mug._ensure_connection.assert_called_once()
+        ember_mug._client.write_gatt_char.assert_called_once_with(
+            MugCharacteristic.VOLUME.uuid,
+            bytearray(b'\00'),
+        )
+
+
+async def test_set_volume_level_mug(ember_mug: AsyncMock):
+    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
+        with pytest.raises(NotImplementedError):
+            await ember_mug.set_volume_level(VolumeLevel.HIGH)
+        ember_mug._ensure_connection.assert_not_called()
+        ember_mug._client.write_gatt_char.assert_not_called()
+
+
 async def test_get_mug_target_temp(ember_mug: AsyncMock):
     with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
         ember_mug._client.read_gatt_char.return_value = b'\xcd\x15'
         assert (await ember_mug.get_target_temp()) == 55.81
         ember_mug._client.read_gatt_char.assert_called_once_with(MugCharacteristic.TARGET_TEMPERATURE.uuid)
```

### Comparing `python_ember_mug-0.7.0b6/tests/test_consts.py` & `python_ember_mug-0.7.0b7/tests/test_consts.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b6/tests/test_data.py` & `python_ember_mug-0.7.0b7/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b6/tests/test_formatting.py` & `python_ember_mug-0.7.0b7/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b6/tests/test_mug_data.py` & `python_ember_mug-0.7.0b7/tests/test_mug_data.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b6/tests/test_scanner.py` & `python_ember_mug-0.7.0b7/tests/test_scanner.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b6/tests/test_utils.py` & `python_ember_mug-0.7.0b7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b6/PKG-INFO` & `python_ember_mug-0.7.0b7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ember-mug
-Version: 0.7.0b6
+Version: 0.7.0b7
 Summary: Python Library for Ember Mugs.
 Home-page: https://github.com/sopelj/python-ember-mug
 License: MIT
 Author: Jesse Sopel
 Author-email: jesse.sopel@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```

