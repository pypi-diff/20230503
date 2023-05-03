# Comparing `tmp/vmk_spectrum-0.0.5-cp311-cp311-win_amd64.whl.zip` & `tmp/vmk_spectrum-0.0.7-cp311-cp311-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,13 @@
-Zip file size: 78535 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat   161280 b- defN 23-Apr-30 09:20 _pyspectrum.cp311-win_amd64.pyd
--rw-rw-rw-  2.0 fat      130 b- defN 23-Apr-30 09:18 pyspectrum/__init__.py
--rw-rw-rw-  2.0 fat     4358 b- defN 23-Apr-30 09:18 pyspectrum/data.py
--rw-rw-rw-  2.0 fat      435 b- defN 23-Apr-30 09:18 pyspectrum/errors.py
--rw-rw-rw-  2.0 fat    10640 b- defN 23-Apr-30 09:18 pyspectrum/spectrometer.py
--rw-rw-rw-  2.0 fat      317 b- defN 23-Apr-30 09:20 vmk_spectrum-0.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Apr-30 09:20 vmk_spectrum-0.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       25 b- defN 23-Apr-30 09:20 vmk_spectrum-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      721 b- defN 23-Apr-30 09:20 vmk_spectrum-0.0.5.dist-info/RECORD
-9 files, 178008 bytes uncompressed, 77299 bytes compressed:  56.6%
+Zip file size: 80812 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat   161280 b- defN 23-May-03 19:02 _pyspectrum.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      159 b- defN 23-May-03 18:59 pyspectrum/__init__.py
+-rw-rw-rw-  2.0 fat     4358 b- defN 23-May-03 18:59 pyspectrum/data.py
+-rw-rw-rw-  2.0 fat     1257 b- defN 23-May-03 18:59 pyspectrum/device_factory.py
+-rw-rw-rw-  2.0 fat      435 b- defN 23-May-03 18:59 pyspectrum/errors.py
+-rw-rw-rw-  2.0 fat     4747 b- defN 23-May-03 18:59 pyspectrum/ethernet_device.py
+-rw-rw-rw-  2.0 fat     9575 b- defN 23-May-03 18:59 pyspectrum/spectrometer.py
+-rw-rw-rw-  2.0 fat      317 b- defN 23-May-03 19:02 vmk_spectrum-0.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-May-03 19:02 vmk_spectrum-0.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       25 b- defN 23-May-03 19:02 vmk_spectrum-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      891 b- defN 23-May-03 19:02 vmk_spectrum-0.0.7.dist-info/RECORD
+11 files, 183146 bytes uncompressed, 79310 bytes compressed:  56.7%
```

## zipnote {}

```diff
@@ -3,26 +3,32 @@
 
 Filename: pyspectrum/__init__.py
 Comment: 
 
 Filename: pyspectrum/data.py
 Comment: 
 
+Filename: pyspectrum/device_factory.py
+Comment: 
+
 Filename: pyspectrum/errors.py
 Comment: 
 
+Filename: pyspectrum/ethernet_device.py
+Comment: 
+
 Filename: pyspectrum/spectrometer.py
 Comment: 
 
-Filename: vmk_spectrum-0.0.5.dist-info/METADATA
+Filename: vmk_spectrum-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: vmk_spectrum-0.0.5.dist-info/WHEEL
+Filename: vmk_spectrum-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: vmk_spectrum-0.0.5.dist-info/top_level.txt
+Filename: vmk_spectrum-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: vmk_spectrum-0.0.5.dist-info/RECORD
+Filename: vmk_spectrum-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyspectrum/__init__.py

```diff
@@ -1,3 +1,4 @@
 from .errors import *
 from .data import Data, Spectrum
-from .spectrometer import Spectrometer, usb_spectrometer, FactoryConfig
+from .spectrometer import Spectrometer, FactoryConfig
+from .device_factory import UsbID, EthernetID
```

## pyspectrum/spectrometer.py

```diff
@@ -4,14 +4,15 @@
 from typing import Optional
 
 import _pyspectrum as internal
 import numpy as np
 from numpy.typing import NDArray
 
 from .data import Data, Spectrum
+from .device_factory import DeviceID, create_device
 from .errors import ConfigurationError, LoadError, DeviceClosedError
 
 
 def eprint(*args, **kwargs):
     print(*args, file=sys.stderr, **kwargs)
 
 
@@ -62,21 +63,21 @@
     n_times: int = 1  # количество измерений
     dark_signal_path: Optional[str] = None
 
 
 class Spectrometer:
     """Класс, представляющий высокоуровневую абстракцию над спектрометром"""
 
-    def __init__(self, device: internal.RawSpectrometer, factory_config: FactoryConfig = FactoryConfig.default()):
+    def __init__(self, device_id: DeviceID, factory_config: FactoryConfig = FactoryConfig.default(), reopen: bool = True):
         """
         Params:
-            device: Низкоуровневый объект устройства. В данный момент может быть получен только через `usb_spectrometer`
+            device_id: Идентификатор устройства. В настоящий момент поддерживаются UsbID, EthernetID
             factory_config: Заводские настройки
         """
-        self.__device: internal.RawSpectrometer = device
+        self.__device: internal.RawSpectrometer = create_device(device_id, reopen)
         self.__factory_config = factory_config
         self.__config = Config()
         self.__device.setTimer(self.__config.exposure)
         self.__dark_signal: Data | None = None
         self.__wavelengths: NDArray[float] | None = None
 
     def __check_opened(self):
@@ -86,15 +87,15 @@
     def close(self) -> None:
         """Закрыть устройство"""
         self.__device.close()
 
     # --------        dark signal        --------
 
     @property
-    def dark_signal(self) -> Data|None:
+    def dark_signal(self) -> Data | None:
         """Текущий темновой сигнал"""
         return self.__dark_signal
 
     def __load_dark_signal(self):
         try:
             data = Data.load(self.__config.dark_signal_path)
         except Exception:
@@ -234,29 +235,7 @@
 
         if (dark_signal_path is not None) and (dark_signal_path != self.__config.dark_signal_path):
             self.__config.dark_signal_path = dark_signal_path
             self.__load_dark_signal()
 
         if wavelength_calibration_path is not None:
             self.__load_wavelength_calibration(wavelength_calibration_path)
-
-
-__usb_device_cache: dict[tuple, internal.UsbRawSpectrometer] = dict()
-
-
-def usb_spectrometer(vid: int = 0x0403, pid: int = 0x6014, read_timeout: int = 10_000, serial: str = '', reopen: bool = False) -> internal.UsbRawSpectrometer:
-    """Create usb spectrometer for Spectrometer creation
-    Params:
-        vid: Usb vendor id
-        pid: Usb product id
-        read_timeout: таймаут чтения данных с устройства, ms
-        serial: Usb serial (по умполчанию открывается первое устройство с подходящими `vid` и `pid`)
-        reopen: Если `True`, предыдущий объект Spectrometer, использующий устройство, буде закрыт
-    Returns:
-        Device object needed for Spectrometer creation
-    """
-    device_id = (vid, pid, serial)
-    if reopen and (device_id in __usb_device_cache):
-        __usb_device_cache[device_id].close()
-    device = internal.UsbRawSpectrometer(vid, pid, serial, read_timeout)
-    __usb_device_cache[device_id] = device
-    return device
```

