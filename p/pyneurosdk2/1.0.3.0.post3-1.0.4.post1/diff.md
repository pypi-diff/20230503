# Comparing `tmp/pyneurosdk2-1.0.3.0.post3.tar.gz` & `tmp/pyneurosdk2-1.0.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyneurosdk2-1.0.3.0.post3.tar", last modified: Mon Dec  5 12:40:57 2022, max compression
+gzip compressed data, was "dist\pyneurosdk2-1.0.4.post1.tar", last modified: Wed May  3 11:32:49 2023, max compression
```

## Comparing `pyneurosdk2-1.0.3.0.post3.tar` & `pyneurosdk2-1.0.4.post1.tar`

### file list

```diff
@@ -1,21 +1,34 @@
-drwxrwxrwx   0        0        0        0 2022-12-05 12:40:57.000000 pyneurosdk2-1.0.3.0.post3/
--rw-rw-rw-   0        0        0     9582 2022-12-05 12:40:57.000000 pyneurosdk2-1.0.3.0.post3/PKG-INFO
--rw-rw-rw-   0        0        0     8774 2022-12-05 12:31:32.000000 pyneurosdk2-1.0.3.0.post3/README.md
-drwxrwxrwx   0        0        0        0 2022-12-05 12:40:57.000000 pyneurosdk2-1.0.3.0.post3/neurosdk/
--rw-rw-rw-   0        0        0    13032 2022-11-23 15:51:40.000000 pyneurosdk2-1.0.3.0.post3/neurosdk/__cmn_types.py
--rw-rw-rw-   0        0        0        0 2022-11-24 14:53:06.000000 pyneurosdk2-1.0.3.0.post3/neurosdk/__init__.py
--rw-rw-rw-   0        0        0      217 2022-10-25 15:13:26.000000 pyneurosdk2-1.0.3.0.post3/neurosdk/__utils.py
--rw-rw-rw-   0        0        0    12996 2022-12-05 12:33:23.000000 pyneurosdk2-1.0.3.0.post3/neurosdk/cmn_types.py
-drwxrwxrwx   0        0        0        0 2022-12-05 12:40:57.000000 pyneurosdk2-1.0.3.0.post3/neurosdk/libs/
--rw-rw-rw-   0        0        0  2002944 2022-11-18 15:28:36.000000 pyneurosdk2-1.0.3.0.post3/neurosdk/libs/neurosdk2-x32.dll
--rw-rw-rw-   0        0        0  2140160 2022-11-18 15:32:05.000000 pyneurosdk2-1.0.3.0.post3/neurosdk/libs/neurosdk2-x64.dll
--rw-rw-rw-   0        0        0     4957 2022-12-05 11:02:05.000000 pyneurosdk2-1.0.3.0.post3/neurosdk/sample.py
--rw-rw-rw-   0        0        0     7524 2022-11-24 14:53:23.000000 pyneurosdk2-1.0.3.0.post3/neurosdk/scanner.py
--rw-rw-rw-   0        0        0    77384 2022-12-05 11:02:04.000000 pyneurosdk2-1.0.3.0.post3/neurosdk/sensor.py
-drwxrwxrwx   0        0        0        0 2022-12-05 12:40:57.000000 pyneurosdk2-1.0.3.0.post3/pyneurosdk2.egg-info/
--rw-rw-rw-   0        0        0     9582 2022-12-05 12:40:57.000000 pyneurosdk2-1.0.3.0.post3/pyneurosdk2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2022-12-05 12:40:57.000000 pyneurosdk2-1.0.3.0.post3/pyneurosdk2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-05 12:40:57.000000 pyneurosdk2-1.0.3.0.post3/pyneurosdk2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-12-05 12:40:57.000000 pyneurosdk2-1.0.3.0.post3/pyneurosdk2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-05 12:40:57.000000 pyneurosdk2-1.0.3.0.post3/setup.cfg
--rw-rw-rw-   0        0        0      983 2022-12-05 12:33:38.000000 pyneurosdk2-1.0.3.0.post3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:32:49.000000 pyneurosdk2-1.0.4.post1/
+-rw-rw-rw-   0        0        0     1090 2023-04-19 10:44:40.000000 pyneurosdk2-1.0.4.post1/LICENSE
+-rw-rw-rw-   0        0        0     9709 2023-05-03 11:32:49.000000 pyneurosdk2-1.0.4.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     9186 2023-05-03 11:30:45.000000 pyneurosdk2-1.0.4.post1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 11:32:49.000000 pyneurosdk2-1.0.4.post1/neurosdk/
+-rw-rw-rw-   0        0        0     6424 2023-05-03 11:26:08.000000 pyneurosdk2-1.0.4.post1/neurosdk/__cmn_types.py
+-rw-rw-rw-   0        0        0        0 2022-11-24 14:53:06.000000 pyneurosdk2-1.0.4.post1/neurosdk/__init__.py
+-rw-rw-rw-   0        0        0      219 2023-02-28 10:25:36.000000 pyneurosdk2-1.0.4.post1/neurosdk/__utils.py
+-rw-rw-rw-   0        0        0     2228 2023-05-03 11:26:08.000000 pyneurosdk2-1.0.4.post1/neurosdk/amp_sensor.py
+-rw-rw-rw-   0        0        0      456 2023-05-03 11:26:08.000000 pyneurosdk2-1.0.4.post1/neurosdk/brainbit_black_sensor.py
+-rw-rw-rw-   0        0        0     4019 2023-05-03 11:26:08.000000 pyneurosdk2-1.0.4.post1/neurosdk/brainbit_sensor.py
+-rw-rw-rw-   0        0        0    23601 2023-05-03 11:26:08.000000 pyneurosdk2-1.0.4.post1/neurosdk/callibri_sensor.py
+-rw-rw-rw-   0        0        0     9161 2023-05-03 11:26:08.000000 pyneurosdk2-1.0.4.post1/neurosdk/cmn_types.py
+-rw-rw-rw-   0        0        0      890 2023-05-03 11:26:08.000000 pyneurosdk2-1.0.4.post1/neurosdk/electrode_sensor.py
+-rw-rw-rw-   0        0        0      880 2023-05-03 11:26:08.000000 pyneurosdk2-1.0.4.post1/neurosdk/envelope_sensor.py
+-rw-rw-rw-   0        0        0     5007 2023-05-03 11:26:08.000000 pyneurosdk2-1.0.4.post1/neurosdk/fpg_sensor.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:32:49.000000 pyneurosdk2-1.0.4.post1/neurosdk/libs/
+-rw-rw-rw-   0        0        0   679936 2023-04-19 10:35:49.000000 pyneurosdk2-1.0.4.post1/neurosdk/libs/neurosdk2-x32.dll
+-rw-rw-rw-   0        0        0   946688 2023-04-19 10:33:49.000000 pyneurosdk2-1.0.4.post1/neurosdk/libs/neurosdk2-x64.dll
+-rw-rw-rw-   0        0        0     4334 2023-05-03 11:26:08.000000 pyneurosdk2-1.0.4.post1/neurosdk/mems_sensor.py
+-rw-rw-rw-   0        0        0     1073 2023-05-03 11:26:08.000000 pyneurosdk2-1.0.4.post1/neurosdk/neuro_smart_sensor.py
+-rw-rw-rw-   0        0        0     1792 2023-05-03 11:26:08.000000 pyneurosdk2-1.0.4.post1/neurosdk/resist_sensor.py
+-rw-rw-rw-   0        0        0     1588 2023-05-03 11:26:08.000000 pyneurosdk2-1.0.4.post1/neurosdk/respiration_sensor.py
+-rw-rw-rw-   0        0        0     4478 2023-02-28 10:25:36.000000 pyneurosdk2-1.0.4.post1/neurosdk/sample.py
+-rw-rw-rw-   0        0        0     8522 2023-05-03 11:26:08.000000 pyneurosdk2-1.0.4.post1/neurosdk/scanner.py
+-rw-rw-rw-   0        0        0    17383 2023-03-13 10:24:36.000000 pyneurosdk2-1.0.4.post1/neurosdk/sensor.py
+-rw-rw-rw-   0        0        0      864 2023-05-03 11:26:08.000000 pyneurosdk2-1.0.4.post1/neurosdk/signal_sensor.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:32:49.000000 pyneurosdk2-1.0.4.post1/pyneurosdk2.egg-info/
+-rw-rw-rw-   0        0        0     9709 2023-05-03 11:32:48.000000 pyneurosdk2-1.0.4.post1/pyneurosdk2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      706 2023-05-03 11:32:48.000000 pyneurosdk2-1.0.4.post1/pyneurosdk2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 11:32:48.000000 pyneurosdk2-1.0.4.post1/pyneurosdk2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-03 11:32:48.000000 pyneurosdk2-1.0.4.post1/pyneurosdk2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 11:32:49.000000 pyneurosdk2-1.0.4.post1/setup.cfg
+-rw-rw-rw-   0        0        0     1506 2023-05-03 11:32:24.000000 pyneurosdk2-1.0.4.post1/setup.py
```

### Comparing `pyneurosdk2-1.0.3.0.post3/PKG-INFO` & `pyneurosdk2-1.0.4.post1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: pyneurosdk2
-Version: 1.0.3.0.post3
-Summary: Python wrapper for NeuroSDK2
-Home-page: https://gitlab.com/brainbit-inc/brainbit-sdk
-Author: Brainbit Inc.
-Author-email: support@brainbit.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # Python NeuroSDK 2
 
 Welcome to the Python NeuroSDK 2. The Neurosdk library is designed to work with BrainBit, BrainBitBlack, Callibri and Kolibri devices. The library is intended for python version 3.7 and higher, Windows version 10 and higher.
 
 ## Documentation
 
 - [Installing](#installing)
@@ -49,49 +34,49 @@
 ```python
 from neurosdk.scanner import Scanner
 ```
 
 - sensor - methods of interaction with the device
 
 ```python
-from neurosdk.sensor import Sensor
+from neurosdk.callibri_sensor import CallibriSensor
+from neurosdk.brainbit_sensor import BrainBitSensor
+from neurosdk.brainbit_black_sensor import BrainBitBlackSensor
 ```
 
 - types - implementation of all types of the library, you can either connect everything or only those necessary for a specific task
 
 ```python
 from neurosdk.cmn_types import *
 ```
 
-Here is a description of how to work with a BrainBit device.
-
 ## Searching device
 
 The `Scanner` class is used to search for a device. For a correct search, you must specify the list of device types. You can search for one or more device types at the same time. For example, to search for BrainBit and Callibri, you need to create a scanner as follows:
 
 ```python
 scanner = Scanner([SensorFamily.SensorLEBrainBit, SensorFamily.SensorLECallibri])
 ```
 
 Search start:
 
 ```python
-scanner.Start()
+scanner.start()
 ```
 
 Stop search:
 
 ```python
-scanner.Stop()
+scanner.stop()
 ```
 
 All found devices can be obtained using the method:
 
 ```python
-sensors = scanner.Sensors()
+sensors = scanner.sensors()
 ```
 
 During the search, an `sensorsChanged` callback will be called, which will display a list of found devices. If the device leaves the scanner's field of view for any reason, the device will disappear from the list after 12 seconds.
 
 ```python
 def sensorFound(scanner, sensors):
    for i in range(len(sensors)):
@@ -109,59 +94,59 @@
 - SerialNumber: str
 - PairingRequired: bool
 
 > Important!
 > The serial number of the Callibri and Kolibri does not appear in the SensorInfo recieving during the search. To get this value, you need to connect to the device and request the serial number manually:
 >
 > ```python
-> sn = sensor.SerialNumber
+> sn = sensor.serial_number
 > ```
 
 
 ## Connection
 
 Next, you can create any device from the list using the method:
 
 ```python
-sensor = scanner.CreateSensor(sensInfo)
+sensor = scanner.create_sensor(sensInfo)
 ```
 When created, the device will connect automatically. This is a blocking function, so it is desirable to call it from an separate thread. Upon successful connection, a sensor instance will be returned. If unsuccessful, an exception is thrown. On subsequent connections and disconnections, a callback will be called indicating the state of the device.
 
 To disconnect from the device, use the following method:
 
 ```python
-sensor.Disconnect()
+sensor.disconnect()
 ```
 
 To connect to a device created but not connected for any reason, the method:
 
 ```python
-sensor.Connect()
+sensor.connect()
 ```
 
 It is blocking too.
 
 ## Parameters
 
 SDK allows you to get information about the connected device:
 
 ```python
-print(sensor.SensFamily) # SensorFamily.SensorLEBrainBit
-print(sensor.Features) # [<SensorFeature.FeatureSignal: 0>, ...]
-print(sensor.Commands) # [<SensorCommand.CommandStartSignal: 0>,...]
-print(sensor.Parameters)
-print(sensor.Name) # BrainBit
-print(sensor.State) # SensorState.StateInRange
-print(sensor.Address) # AA:BB:CC:DD:EE:FF
-print(sensor.SerialNumber) # 123456
-print(sensor.BattPower) # 50
-print(sensor.SamplingFrequency) # SensorSamplingFrequency.FrequencyHz250
-print(sensor.Gain) # SensorGain.SensorGain6
-print(sensor.DataOffset) # SensorDataOffset.DataOffset0
-print(sensor.Version) # SensorVersion(FwMajor=50, FwMinor=0, FwPatch=0, HwMajor=1, HwMinor=0, HwPatch=0, ExtMajor=65)
+print(sensor.sens_family)  # SensorFamily.SensorLEBrainBit
+print(sensor.features)  # [<SensorFeature.FeatureSignal: 0>, ...]
+print(sensor.commands)  # [<SensorCommand.CommandStartSignal: 0>,...]
+print(sensor.parameters)
+print(sensor.name)  # BrainBit
+print(sensor.state)  # SensorState.StateInRange
+print(sensor.address)  # AA:BB:CC:DD:EE:FF
+print(sensor.serial_number)  # 123456
+print(sensor.batt_power)  # 50
+print(sensor.sampling_frequency)  # SensorSamplingFrequency.FrequencyHz250
+print(sensor.gain)  # SensorGain.SensorGain6
+print(sensor.data_offset)  # SensorDataOffset.DataOffset0
+print(sensor.version)  # SensorVersion(FwMajor=50, FwMinor=0, FwPatch=0, HwMajor=1, HwMinor=0, HwPatch=0, ExtMajor=65)
 ```
 
 >  You can distinguish BrainBit device from Flex by the firmware version number: if the `SensorVersion.FwMajor` is more than 100 - it's Flex, if it's less than BrainBit.
 
 If you need to change any property, you first need to check if it is writable. This can be done by reading the list of device parameters, where each parameter will have an access level:
 
 ```
@@ -169,31 +154,31 @@
  ParameterInfo(Param=<SensorParameter.ParameterState: 1>,  ParamAccess=<SensorParamAccess.ParamAccessReadNotify: 2>)
  ...]
 ```
 
 And also check the support of certain modules:
 
 ```python
-sensor.IsSupportedFeature(sensor_future)
-sensor.IsSupportedCommand(sensor_command)
-sensor.IsSupportedParameter(sensor_parameter)
+sensor.is_supported_feature(sensor_future)
+sensor.is_supported_command(sensor_command)
+sensor.is_supported_parameter(sensor_parameter)
 ```
 
 ## Receiving signal
 
 For any device that supports recieving signal, you can run the following commands for starting:
 
 ```python
-sensor.ExecCommand(SensorCommand.CommandStartSignal)
+sensor.exec_command(SensorCommand.CommandStartSignal)
 ```
 
 Stop:
 
 ```python
-sensor.ExecCommand(SensorCommand.CommandStopSignal)
+sensor.exec_command(SensorCommand.CommandStopSignal)
 ```
 
 ### BrainBit, BrainBitBlack, Flex
 
 You can get the signal value using the callback:
 
 ```python
@@ -246,20 +231,21 @@
 
 Resistance is only supported by BrainBit, BrainBitBlack and Flex. You can also check the availability of these features using the method `sensor.IsSupportedFeature(SensorFeature.FeatureResist)`.
 
 To get resistance values:
 
 ```python
 def onBrainBitResistDataReceived(sensor, data):
-   print(data)
+    print(data)
+
 
 sensor.brainBitResistDataReceived = onBrainBitResistDataReceived
 
-sensor.ExecCommand(SensorCommand.CommandStartResist)
-sensor.ExecCommand(SensorCommand.CommandStopResist)
+sensor.exec_command(SensorCommand.CommandStartResist)
+sensor.exec_command(SensorCommand.CommandStopResist)
 ```
 
 The callback returns one packet of samples, each packet contains the resistance values in volts:
 - O1: float
 - O2: float
 - T3: float
 - T4: float
@@ -268,21 +254,21 @@
 
 ```python
 sensor.brainBitResistDataReceived = None
 ```
 
 > BrainBit cannot be in the resistance and signal readout mode at the same time, so you must first get the resistance values, but only after this signal, or vice versa. For example:
 > ```python
-> sensor.ExecCommand(SensorCommand.CommandStartResist)
+> sensor.exec_command(SensorCommand.CommandStartResist)
 > sleep(10)
-> sensor.ExecCommand(SensorCommand.CommandStopResist)
+> sensor.exec_command(SensorCommand.CommandStopResist)
 > ...
-> sensor.ExecCommand(SensorCommand.CommandStartSignal)
+> sensor.exec_command(SensorCommand.CommandStartSignal)
 > sleep(10)
-> sensor.ExecCommand(SensorCommand.CommandStopSignal)
+> sensor.exec_command(SensorCommand.CommandStopSignal)
 > ```
 
 ## Electrodes connection
 
 Electrode placement check is available for Callibri and Kolibri devices. This data shows whether the electrodes are attached to the skin.
 
 ```python
```

### Comparing `pyneurosdk2-1.0.3.0.post3/README.md` & `pyneurosdk2-1.0.4.post1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,306 +1,323 @@
-# Python NeuroSDK 2
-
-Welcome to the Python NeuroSDK 2. The Neurosdk library is designed to work with BrainBit, BrainBitBlack, Callibri and Kolibri devices. The library is intended for python version 3.7 and higher, Windows version 10 and higher.
-
-## Documentation
-
-- [Installing](#installing)
-- [Description](#description)
-- [Searching device](#searching-device)
-- [Connection](#connection)
-- [Parameters](#paramaters)
-- [Receiving signal](#receiving-signal)
-- [Receiving resistance](#receiving-resistance)
-- [Electrodes connection](#electrodes-connection)
-- [Clean up](#clean_up)
-
-## Installing
-
-```
-pip install pyneurosdk2
-```
-
-## Description
-
-The package has the following structure:
- - neurosdk - the main package with the implementation of methods
- - sample - is into the neurosdk package, file `sample.py`
- - libs - also into neurosdk package, contain dll library files
-
-The library provides three main modules:
-
-- scanner - to search for devices
-
-```python
-from neurosdk.scanner import Scanner
-```
-
-- sensor - methods of interaction with the device
-
-```python
-from neurosdk.sensor import Sensor
-```
-
-- types - implementation of all types of the library, you can either connect everything or only those necessary for a specific task
-
-```python
-from neurosdk.cmn_types import *
-```
-
-Here is a description of how to work with a BrainBit device.
-
-## Searching device
-
-The `Scanner` class is used to search for a device. For a correct search, you must specify the list of device types. You can search for one or more device types at the same time. For example, to search for BrainBit and Callibri, you need to create a scanner as follows:
-
-```python
-scanner = Scanner([SensorFamily.SensorLEBrainBit, SensorFamily.SensorLECallibri])
-```
-
-Search start:
-
-```python
-scanner.Start()
-```
-
-Stop search:
-
-```python
-scanner.Stop()
-```
-
-All found devices can be obtained using the method:
-
-```python
-sensors = scanner.Sensors()
-```
-
-During the search, an `sensorsChanged` callback will be called, which will display a list of found devices. If the device leaves the scanner's field of view for any reason, the device will disappear from the list after 12 seconds.
-
-```python
-def sensorFound(scanner, sensors):
-   for i in range(len(sensors)):
-       print('Sensor %s' % sensors[i])
-
-scanner.sensorsChanged = sensorFound
-```
-
-The sensor's list will contain records of the SensorInfo type with fields:
-
-- SensFamily: SensorFamily
-- SensModel: int
-- Name: str
-- Address: str
-- SerialNumber: str
-- PairingRequired: bool
-
-> Important!
-> The serial number of the Callibri and Kolibri does not appear in the SensorInfo recieving during the search. To get this value, you need to connect to the device and request the serial number manually:
->
-> ```python
-> sn = sensor.SerialNumber
-> ```
-
-
-## Connection
-
-Next, you can create any device from the list using the method:
-
-```python
-sensor = scanner.CreateSensor(sensInfo)
-```
-When created, the device will connect automatically. This is a blocking function, so it is desirable to call it from an separate thread. Upon successful connection, a sensor instance will be returned. If unsuccessful, an exception is thrown. On subsequent connections and disconnections, a callback will be called indicating the state of the device.
-
-To disconnect from the device, use the following method:
-
-```python
-sensor.Disconnect()
-```
-
-To connect to a device created but not connected for any reason, the method:
-
-```python
-sensor.Connect()
-```
-
-It is blocking too.
-
-## Parameters
-
-SDK allows you to get information about the connected device:
-
-```python
-print(sensor.SensFamily) # SensorFamily.SensorLEBrainBit
-print(sensor.Features) # [<SensorFeature.FeatureSignal: 0>, ...]
-print(sensor.Commands) # [<SensorCommand.CommandStartSignal: 0>,...]
-print(sensor.Parameters)
-print(sensor.Name) # BrainBit
-print(sensor.State) # SensorState.StateInRange
-print(sensor.Address) # AA:BB:CC:DD:EE:FF
-print(sensor.SerialNumber) # 123456
-print(sensor.BattPower) # 50
-print(sensor.SamplingFrequency) # SensorSamplingFrequency.FrequencyHz250
-print(sensor.Gain) # SensorGain.SensorGain6
-print(sensor.DataOffset) # SensorDataOffset.DataOffset0
-print(sensor.Version) # SensorVersion(FwMajor=50, FwMinor=0, FwPatch=0, HwMajor=1, HwMinor=0, HwPatch=0, ExtMajor=65)
-```
-
->  You can distinguish BrainBit device from Flex by the firmware version number: if the `SensorVersion.FwMajor` is more than 100 - it's Flex, if it's less than BrainBit.
-
-If you need to change any property, you first need to check if it is writable. This can be done by reading the list of device parameters, where each parameter will have an access level:
-
-```
-[ParameterInfo(Param=<SensorParameter.ParameterOffset: 8>, ParamAccess=<SensorParamAccess.ParamAccessRead: 0>),  
- ParameterInfo(Param=<SensorParameter.ParameterState: 1>,  ParamAccess=<SensorParamAccess.ParamAccessReadNotify: 2>)
- ...]
-```
-
-And also check the support of certain modules:
-
-```python
-sensor.IsSupportedFeature(sensor_future)
-sensor.IsSupportedCommand(sensor_command)
-sensor.IsSupportedParameter(sensor_parameter)
-```
-
-## Receiving signal
-
-For any device that supports recieving signal, you can run the following commands for starting:
-
-```python
-sensor.ExecCommand(SensorCommand.CommandStartSignal)
-```
-
-Stop:
-
-```python
-sensor.ExecCommand(SensorCommand.CommandStopSignal)
-```
-
-### BrainBit, BrainBitBlack, Flex
-
-You can get the signal value using the callback:
-
-```python
-def onBrainBitSignalDataReceived(sensor, data):
-   print(data)
-
-sensor.brainBitSignalDataReceived = onBrainBitSignalDataReceived
-```
-
-After you have finished working with the signal, you can unsubscribe from the callback as follows:
-
-```python
-sensor.brainBitSignalDataReceived = None
-```
-
-It gives a list of packages. Each package contains:
-- PackNum: int
-- Marker: int
-- O1: float
-- O2: float
-- T3: float
-- T4: float
-
-It is values from 4 channels in volts, a number for each packet and a marker if it was sent and this feature is supported by the device.
-
-### Callibri, Kolibri
-
-You can get the signal value using the callback:
-
-```python
-def onCallibriSignalDataReceived(sensor, data):
-   print(data)
-
-sensor.callibriSignalDataReceived = onCallibriSignalDataReceived
-```
-
-After you have finished working with the signal, you can unsubscribe from the callback as follows:
-
-```python
-sensor.callibriSignalDataReceived = None
-```
-
-It gives a list of packages. Each package contains:
- - PackNum: int
- - Samples: [float]
-
-It is values in volts and a number for each packet.
-
-## Receiving resistance
-
-Resistance is only supported by BrainBit, BrainBitBlack and Flex. You can also check the availability of these features using the method `sensor.IsSupportedFeature(SensorFeature.FeatureResist)`.
-
-To get resistance values:
-
-```python
-def onBrainBitResistDataReceived(sensor, data):
-   print(data)
-
-sensor.brainBitResistDataReceived = onBrainBitResistDataReceived
-
-sensor.ExecCommand(SensorCommand.CommandStartResist)
-sensor.ExecCommand(SensorCommand.CommandStopResist)
-```
-
-The callback returns one packet of samples, each packet contains the resistance values in volts:
-- O1: float
-- O2: float
-- T3: float
-- T4: float
-
-After you have finished working with the resistance, you can unsubscribe from the callback as follows:
-
-```python
-sensor.brainBitResistDataReceived = None
-```
-
-> BrainBit cannot be in the resistance and signal readout mode at the same time, so you must first get the resistance values, but only after this signal, or vice versa. For example:
-> ```python
-> sensor.ExecCommand(SensorCommand.CommandStartResist)
-> sleep(10)
-> sensor.ExecCommand(SensorCommand.CommandStopResist)
-> ...
-> sensor.ExecCommand(SensorCommand.CommandStartSignal)
-> sleep(10)
-> sensor.ExecCommand(SensorCommand.CommandStopSignal)
-> ```
-
-## Electrodes connection
-
-Electrode placement check is available for Callibri and Kolibri devices. This data shows whether the electrodes are attached to the skin.
-
-```python
-def onCallibriElectrodeStateChanged(sensor, data):
-   print(data)
-
-sensor.callibriElectrodeStateChanged = onCallibriElectrodeStateChanged
-```
-
-For unsubscribe from callback:
-
-```python
-sensor.callibriElectrodeStateChanged = None
-```
-
-Electrodes state can be one of values of enum:
-- ElStNormal = 0
-- ElStHighResistance = 1
-- ElStDetached = 2
-
-To get the state of the electrodes, you need to start a signal from the device.You can receive electrode and signal values at the same time.
-
-## Clean up
-
-After you finish working with the device, you need to clean up the resources used. This happens in the destructor of the scanner and sensor, so if they were not called by the system, you must call them manually.
-
-```python
-del sensor
-del scanner
-```
-
-## License
-
-Copyright (c) Brainbit Inc. All rights reserved.
-
-Licensed under the [MIT license](LICENSE).
+Metadata-Version: 2.1
+Name: pyneurosdk2
+Version: 1.0.4.post1
+Summary: Python wrapper for NeuroSDK2
+Home-page: https://gitlab.com/brainbit-inc/brainbit-sdk
+Author: Brainbit Inc.
+Author-email: support@brainbit.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Python NeuroSDK 2
+
+Welcome to the Python NeuroSDK 2. The Neurosdk library is designed to work with BrainBit, BrainBitBlack, Callibri and Kolibri devices. The library is intended for python version 3.7 and higher, Windows version 10 and higher.
+
+## Documentation
+
+- [Installing](#installing)
+- [Description](#description)
+- [Searching device](#searching-device)
+- [Connection](#connection)
+- [Parameters](#paramaters)
+- [Receiving signal](#receiving-signal)
+- [Receiving resistance](#receiving-resistance)
+- [Electrodes connection](#electrodes-connection)
+- [Clean up](#clean_up)
+
+## Installing
+
+```
+pip install pyneurosdk2
+```
+
+## Description
+
+The package has the following structure:
+ - neurosdk - the main package with the implementation of methods
+ - sample - is into the neurosdk package, file `sample.py`
+ - libs - also into neurosdk package, contain dll library files
+
+The library provides three main modules:
+
+- scanner - to search for devices
+
+```python
+from neurosdk.scanner import Scanner
+```
+
+- sensor - methods of interaction with the device
+
+```python
+from neurosdk.callibri_sensor import CallibriSensor
+from neurosdk.brainbit_sensor import BrainBitSensor
+from neurosdk.brainbit_black_sensor import BrainBitBlackSensor
+```
+
+- types - implementation of all types of the library, you can either connect everything or only those necessary for a specific task
+
+```python
+from neurosdk.cmn_types import *
+```
+
+## Searching device
+
+The `Scanner` class is used to search for a device. For a correct search, you must specify the list of device types. You can search for one or more device types at the same time. For example, to search for BrainBit and Callibri, you need to create a scanner as follows:
+
+```python
+scanner = Scanner([SensorFamily.SensorLEBrainBit, SensorFamily.SensorLECallibri])
+```
+
+Search start:
+
+```python
+scanner.start()
+```
+
+Stop search:
+
+```python
+scanner.stop()
+```
+
+All found devices can be obtained using the method:
+
+```python
+sensors = scanner.sensors()
+```
+
+During the search, an `sensorsChanged` callback will be called, which will display a list of found devices. If the device leaves the scanner's field of view for any reason, the device will disappear from the list after 12 seconds.
+
+```python
+def sensorFound(scanner, sensors):
+   for i in range(len(sensors)):
+       print('Sensor %s' % sensors[i])
+
+scanner.sensorsChanged = sensorFound
+```
+
+The sensor's list will contain records of the SensorInfo type with fields:
+
+- SensFamily: SensorFamily
+- SensModel: int
+- Name: str
+- Address: str
+- SerialNumber: str
+- PairingRequired: bool
+
+> Important!
+> The serial number of the Callibri and Kolibri does not appear in the SensorInfo recieving during the search. To get this value, you need to connect to the device and request the serial number manually:
+>
+> ```python
+> sn = sensor.serial_number
+> ```
+
+
+## Connection
+
+Next, you can create any device from the list using the method:
+
+```python
+sensor = scanner.create_sensor(sensInfo)
+```
+When created, the device will connect automatically. This is a blocking function, so it is desirable to call it from an separate thread. Upon successful connection, a sensor instance will be returned. If unsuccessful, an exception is thrown. On subsequent connections and disconnections, a callback will be called indicating the state of the device.
+
+To disconnect from the device, use the following method:
+
+```python
+sensor.disconnect()
+```
+
+To connect to a device created but not connected for any reason, the method:
+
+```python
+sensor.connect()
+```
+
+It is blocking too.
+
+## Parameters
+
+SDK allows you to get information about the connected device:
+
+```python
+print(sensor.sens_family)  # SensorFamily.SensorLEBrainBit
+print(sensor.features)  # [<SensorFeature.FeatureSignal: 0>, ...]
+print(sensor.commands)  # [<SensorCommand.CommandStartSignal: 0>,...]
+print(sensor.parameters)
+print(sensor.name)  # BrainBit
+print(sensor.state)  # SensorState.StateInRange
+print(sensor.address)  # AA:BB:CC:DD:EE:FF
+print(sensor.serial_number)  # 123456
+print(sensor.batt_power)  # 50
+print(sensor.sampling_frequency)  # SensorSamplingFrequency.FrequencyHz250
+print(sensor.gain)  # SensorGain.SensorGain6
+print(sensor.data_offset)  # SensorDataOffset.DataOffset0
+print(sensor.version)  # SensorVersion(FwMajor=50, FwMinor=0, FwPatch=0, HwMajor=1, HwMinor=0, HwPatch=0, ExtMajor=65)
+```
+
+>  You can distinguish BrainBit device from Flex by the firmware version number: if the `SensorVersion.FwMajor` is more than 100 - it's Flex, if it's less than BrainBit.
+
+If you need to change any property, you first need to check if it is writable. This can be done by reading the list of device parameters, where each parameter will have an access level:
+
+```
+[ParameterInfo(Param=<SensorParameter.ParameterOffset: 8>, ParamAccess=<SensorParamAccess.ParamAccessRead: 0>),  
+ ParameterInfo(Param=<SensorParameter.ParameterState: 1>,  ParamAccess=<SensorParamAccess.ParamAccessReadNotify: 2>)
+ ...]
+```
+
+And also check the support of certain modules:
+
+```python
+sensor.is_supported_feature(sensor_future)
+sensor.is_supported_command(sensor_command)
+sensor.is_supported_parameter(sensor_parameter)
+```
+
+## Receiving signal
+
+For any device that supports recieving signal, you can run the following commands for starting:
+
+```python
+sensor.exec_command(SensorCommand.CommandStartSignal)
+```
+
+Stop:
+
+```python
+sensor.exec_command(SensorCommand.CommandStopSignal)
+```
+
+### BrainBit, BrainBitBlack, Flex
+
+You can get the signal value using the callback:
+
+```python
+def onBrainBitSignalDataReceived(sensor, data):
+   print(data)
+
+sensor.brainBitSignalDataReceived = onBrainBitSignalDataReceived
+```
+
+After you have finished working with the signal, you can unsubscribe from the callback as follows:
+
+```python
+sensor.brainBitSignalDataReceived = None
+```
+
+It gives a list of packages. Each package contains:
+- PackNum: int
+- Marker: int
+- O1: float
+- O2: float
+- T3: float
+- T4: float
+
+It is values from 4 channels in volts, a number for each packet and a marker if it was sent and this feature is supported by the device.
+
+### Callibri, Kolibri
+
+You can get the signal value using the callback:
+
+```python
+def onCallibriSignalDataReceived(sensor, data):
+   print(data)
+
+sensor.callibriSignalDataReceived = onCallibriSignalDataReceived
+```
+
+After you have finished working with the signal, you can unsubscribe from the callback as follows:
+
+```python
+sensor.callibriSignalDataReceived = None
+```
+
+It gives a list of packages. Each package contains:
+ - PackNum: int
+ - Samples: [float]
+
+It is values in volts and a number for each packet.
+
+## Receiving resistance
+
+Resistance is only supported by BrainBit, BrainBitBlack and Flex. You can also check the availability of these features using the method `sensor.IsSupportedFeature(SensorFeature.FeatureResist)`.
+
+To get resistance values:
+
+```python
+def onBrainBitResistDataReceived(sensor, data):
+    print(data)
+
+
+sensor.brainBitResistDataReceived = onBrainBitResistDataReceived
+
+sensor.exec_command(SensorCommand.CommandStartResist)
+sensor.exec_command(SensorCommand.CommandStopResist)
+```
+
+The callback returns one packet of samples, each packet contains the resistance values in volts:
+- O1: float
+- O2: float
+- T3: float
+- T4: float
+
+After you have finished working with the resistance, you can unsubscribe from the callback as follows:
+
+```python
+sensor.brainBitResistDataReceived = None
+```
+
+> BrainBit cannot be in the resistance and signal readout mode at the same time, so you must first get the resistance values, but only after this signal, or vice versa. For example:
+> ```python
+> sensor.exec_command(SensorCommand.CommandStartResist)
+> sleep(10)
+> sensor.exec_command(SensorCommand.CommandStopResist)
+> ...
+> sensor.exec_command(SensorCommand.CommandStartSignal)
+> sleep(10)
+> sensor.exec_command(SensorCommand.CommandStopSignal)
+> ```
+
+## Electrodes connection
+
+Electrode placement check is available for Callibri and Kolibri devices. This data shows whether the electrodes are attached to the skin.
+
+```python
+def onCallibriElectrodeStateChanged(sensor, data):
+   print(data)
+
+sensor.callibriElectrodeStateChanged = onCallibriElectrodeStateChanged
+```
+
+For unsubscribe from callback:
+
+```python
+sensor.callibriElectrodeStateChanged = None
+```
+
+Electrodes state can be one of values of enum:
+- ElStNormal = 0
+- ElStHighResistance = 1
+- ElStDetached = 2
+
+To get the state of the electrodes, you need to start a signal from the device.You can receive electrode and signal values at the same time.
+
+## Clean up
+
+After you finish working with the device, you need to clean up the resources used. This happens in the destructor of the scanner and sensor, so if they were not called by the system, you must call them manually.
+
+```python
+del sensor
+del scanner
+```
+
+## License
+
+Copyright (c) Brainbit Inc. All rights reserved.
+
+Licensed under the [MIT license](LICENSE).
```

### Comparing `pyneurosdk2-1.0.3.0.post3/neurosdk/sample.py` & `pyneurosdk2-1.0.4.post1/neurosdk/sample.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,143 +2,138 @@
 from cmn_types import *
 
 import concurrent.futures
 from time import sleep
 
 
 def sensor_found(scanner, sensors):
-    for i in range(len(sensors)):
-        print('Sensor found: %s' % sensors[i])
+    for index in range(len(sensors)):
+        print('Sensor found: %s' % sensors[index])
 
 
 def on_sensor_state_changed(sensor, state):
-    print('Sensor {0} is {1}'.format(sensor.Name, state))
+    print('Sensor {0} is {1}'.format(sensor.name, state))
 
 
 def on_battery_changed(sensor, battery):
     print('Battery: {0}'.format(battery))
 
 
-def on_brain_bit_signal_data_received(sensor, data):
+def on_signal_data_received(sensor, data):
     print(data)
 
 
-def on_brain_bit_resist_data_received(sensor, data):
+def on_resist_data_received(sensor, data):
     print(data)
 
 
-def on_callibri_signal_data_received(sensor, data):
+def on_electrodes_state_changed(sensor, data):
     print(data)
 
 
-def on_callibri_electrodes_state_changed(sensor, data):
+def on_envelope_received(sensor, data):
     print(data)
 
 
-def on_callibri_envelope_received(sensor, data):
-    print(data)
-
-
-def on_callibri_respiration_data_received(sensor, data):
+def on_respiration_data_received(sensor, data):
     print(data)
 
 
 try:
-    scanner = Scanner([SensorFamily.SensorLEBrainBitBlack, SensorFamily.SensorLEHeadband, SensorFamily.SensorLEBrainBit,
-                   SensorFamily.SensorLECallibri])
+    scanner = Scanner([SensorFamily.SensorLEBrainBitBlack, SensorFamily.SensorLEBrainBit,
+                       SensorFamily.SensorLECallibri])
 
     scanner.sensorsChanged = sensor_found
-    scanner.Start()
-    print("Starting search for 30 sek...")
-    sleep(10)
-    scanner.Stop()
-
-    sensInfos = scanner.Sensors()
-    for i in range(len(sensInfos)):
-        sensor_info = sensInfos[i]
-        print(sensInfos[i])
+    scanner.start()
+    print("Starting search for 5 sec...")
+    sleep(5)
+    scanner.stop()
+
+    sensorsInfo = scanner.sensors()
+    for i in range(len(sensorsInfo)):
+        current_sensor_info = sensorsInfo[i]
+        print(sensorsInfo[i])
+
 
         def device_connection(sensor_info):
-            return scanner.CreateSensor(sensor_info)
+            return scanner.create_sensor(sensor_info)
 
 
         with concurrent.futures.ThreadPoolExecutor() as executor:
-            future = executor.submit(device_connection, sensor_info)
+            future = executor.submit(device_connection, current_sensor_info)
             sensor = future.result()
             print("Device connected")
 
         sensor.sensorStateChanged = on_sensor_state_changed
         sensor.batteryChanged = on_battery_changed
 
-        sensFamily = sensor.SensFamily
+        sensFamily = sensor.sens_family
 
         print(sensFamily)
-        print(sensor.Features)
-        print(sensor.Commands)
-        print(sensor.Parameters)
-        print(sensor.Name)
-        print(sensor.State)
-        print(sensor.Address)
-        print(sensor.SerialNumber)
-        print(sensor.BattPower)
-        print(sensor.SamplingFrequency)
-        print(sensor.Gain)
-        print(sensor.DataOffset)
-        print(sensor.Version)
-
-        if sensFamily == SensorFamily.SensorLEBrainBit or sensFamily == SensorFamily.SensorLEBrainBitBlack:
-            sensor.brainBitSignalDataReceived = on_brain_bit_signal_data_received
-            sensor.brainBitResistDataReceived = on_brain_bit_resist_data_received
-
-        if sensFamily == SensorFamily.SensorLECallibri:
-            if sensor.IsSupportedFeature(SensorFeature.FeatureSignal):
-                sensor.callibriSignalDataReceived = on_callibri_signal_data_received
-                sensor.callibriElectrodeStateChanged = on_callibri_electrodes_state_changed
-            if sensor.IsSupportedFeature(SensorFeature.FeatureEnvelope):
-                sensor.callibriEnvelopeDataReceived = on_callibri_envelope_received
-            if sensor.IsSupportedFeature(SensorFeature.FeatureRespiration):
-                sensor.callibriRespirationDataReceived = on_callibri_respiration_data_received
+        print(sensor.features)
+        print(sensor.commands)
+        print(sensor.parameters)
+        print(sensor.name)
+        print(sensor.state)
+        print(sensor.address)
+        print(sensor.serial_number)
+        print(sensor.batt_power)
+        print(sensor.sampling_frequency)
+        print(sensor.gain)
+        print(sensor.data_offset)
+        print(sensor.version)
+
+        if sensor.is_supported_feature(SensorFeature.FeatureSignal):
+            sensor.signalDataReceived = on_signal_data_received
+
+        if sensor.is_supported_feature(SensorFeature.FeatureResist):
+            sensor.resistDataReceived = on_resist_data_received
+
+        if sensor.is_supported_feature(SensorFeature.FeatureRespiration):
+            sensor.respirationDataReceived = on_respiration_data_received
+
+        if sensor.is_supported_feature(SensorFeature.FeatureEnvelope):
+            sensor.envelopeDataReceived = on_envelope_received
 
-        if sensor.IsSupportedCommand(SensorCommand.CommandStartSignal):
-            sensor.ExecCommand(SensorCommand.CommandStartSignal)
+        if sensor.is_supported_command(SensorCommand.CommandStartSignal):
+            sensor.exec_command(SensorCommand.CommandStartSignal)
             print("Start signal")
-            sleep(10)
-            sensor.ExecCommand(SensorCommand.CommandStopSignal)
+            sleep(5)
+            sensor.exec_command(SensorCommand.CommandStopSignal)
             print("Stop signal")
 
-        if sensor.IsSupportedCommand(SensorCommand.CommandStopResist):
-            sensor.ExecCommand(SensorCommand.CommandStartResist)
+        if sensor.is_supported_command(SensorCommand.CommandStartResist):
+            sensor.exec_command(SensorCommand.CommandStartResist)
             print("Start resist")
-            sleep(10)
-            print("Timer end")
-            sensor.ExecCommand(SensorCommand.CommandStopResist)
+            sleep(5)
+            sensor.exec_command(SensorCommand.CommandStopResist)
             print("Stop resist")
 
-        if sensor.IsSupportedCommand(SensorCommand.CommandStartEnvelope):
-            sensor.ExecCommand(SensorCommand.CommandStartEnvelope)
+        if sensor.is_supported_command(SensorCommand.CommandStartEnvelope):
+            sensor.exec_command(SensorCommand.CommandStartEnvelope)
             print("Start envelope")
-            sleep(10)
-            sensor.ExecCommand(SensorCommand.CommandStopEnvelope)
+            sleep(5)
+            sensor.exec_command(SensorCommand.CommandStopEnvelope)
             print("Stop envelope")
 
-        if sensor.IsSupportedCommand(SensorCommand.CommandStartRespiration):
-            sensor.ExecCommand(SensorCommand.CommandStartRespiration)
+        if sensor.is_supported_command(SensorCommand.CommandStartRespiration):
+            sensor.exec_command(SensorCommand.CommandStartRespiration)
             print("Start respiration")
-            sleep(10)
-            sensor.ExecCommand(SensorCommand.CommandStopRespiration)
+            sleep(5)
+            sensor.exec_command(SensorCommand.CommandStopRespiration)
             print("Stop respiration")
 
-        if sensor.IsSupportedFeature(SensorFeature.FeatureCurrentStimulator):
-            sensor.ExecCommand(SensorCommand.CommandStartCurrentStimulation)
+        if sensor.is_supported_command(SensorCommand.CommandStartCurrentStimulation):
+            sensor.exec_command(SensorCommand.CommandStartCurrentStimulation)
             print("Start CurrentStimulation")
-            sleep(10)
-            sensor.ExecCommand(SensorCommand.CommandStopCurrentStimulation)
+            sleep(5)
+            sensor.exec_command(SensorCommand.CommandStopCurrentStimulation)
             print("Stop CurrentStimulation")
 
-        sensor.Disconnect()
+        sensor.disconnect()
         print("Disconnect from sensor")
         del sensor
 
     del scanner
     print('Remove scanner')
 except Exception as err:
-        print(err)
+    print(err)
```

### Comparing `pyneurosdk2-1.0.3.0.post3/neurosdk/scanner.py` & `pyneurosdk2-1.0.4.post1/neurosdk/scanner.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,24 @@
-from neurosdk.__utils import raise_exception_if
+import contextlib
+
+from neurosdk.callibri_sensor import CallibriSensor
+from neurosdk.brainbit_sensor import BrainBitSensor
+from neurosdk.brainbit_black_sensor import BrainBitBlackSensor
 
 from neurosdk.__cmn_types import *
-from neurosdk.cmn_types import SensorInfo, SensorFamily
-from neurosdk.sensor import Sensor
+from neurosdk.cmn_types import *
+from neurosdk.__utils import raise_exception_if
 
 import platform
 import pathlib
 import sys
 
+from neurosdk.sensor import Sensor
+
+_libname = None
 if sys.platform == "win32":
     arc = platform.architecture()
     if arc[0].__contains__("64"):
         _libname = pathlib.Path(__file__).parent.resolve() / "libs" / "neurosdk2-x64.dll"
     else:
         _libname = pathlib.Path(__file__).parent.resolve() / "libs" / "neurosdk2-x32.dll"
 elif sys.platform.startswith("linux"):
@@ -33,44 +40,43 @@
         :raises BaseException:
             If an internal error occurred while creating scanner
         """
         _neuro_lib.createScanner.argtypes = [POINTER(c_ubyte), c_uint, POINTER(OpStatus)]
         _neuro_lib.createScanner.restype = SensorScannerPointer
         _neuro_lib.freeScanner.argtypes = [SensorScannerPointer]
         _neuro_lib.freeScanner.restype = c_void_p
-        _neuro_lib.startScanner.argtypes = [SensorScannerPointer]
-        _neuro_lib.startScanner.restype = OpStatus
-        _neuro_lib.stopScanner.argtypes = [SensorScannerPointer]
-        _neuro_lib.stopScanner.restype = OpStatus
-        _neuro_lib.sensorsScanner.argtypes = [SensorScannerPointer, POINTER(NativeSensorInfo), POINTER(c_int32)]
-        _neuro_lib.sensorsScanner.restype = OpStatus
+        _neuro_lib.startScanner.argtypes = [SensorScannerPointer, POINTER(OpStatus), c_int32]
+        _neuro_lib.startScanner.restype = c_uint8
+        _neuro_lib.stopScanner.argtypes = [SensorScannerPointer, POINTER(OpStatus)]
+        _neuro_lib.stopScanner.restype = c_uint8
+        _neuro_lib.sensorsScanner.argtypes = [SensorScannerPointer, POINTER(NativeSensorInfo), POINTER(c_int32),
+                                              POINTER(OpStatus)]
+        _neuro_lib.sensorsScanner.restype = c_uint8
         _neuro_lib.addSensorsCallbackScanner.argtypes = [SensorScannerPointer, SensorCallbackScanner, c_void_p,
-                                                         ctypes.py_object]
-        _neuro_lib.addSensorsCallbackScanner.restype = OpStatus
-        _neuro_lib.removeSensorsCallbackScanner.argtypes = [SensorsListenerHandle]
+                                                         ctypes.py_object, POINTER(OpStatus)]
+        _neuro_lib.addSensorsCallbackScanner.restype = c_uint8
+        _neuro_lib.removeSensorsCallbackScanner.argtypes = [SensorsListenerHandle, POINTER(OpStatus)]
         _neuro_lib.removeSensorsCallbackScanner.restype = c_void_p
-        _neuro_lib.createSensor.argtypes = [SensorScannerPointer, NativeSensorInfo, POINTER(OpStatus)]
+        _neuro_lib.createSensor.argtypes = [SensorScannerPointer, NativeSensorInfo]
         _neuro_lib.createSensor.restype = SensorPointer
 
         self.__create_scanner(filters)
         self.__add_sensors_callback_scanner()
         self.sensorsChanged = None
 
         self.__closed = False
 
     def __del__(self):
-        try:
+        with contextlib.suppress(Exception):
             if not self.__closed:
                 self.__closed = True
                 self.sensorsChanged = None
                 _neuro_lib.removeSensorsCallbackScanner(self.__sensorsCallbackHandle)
                 _neuro_lib.freeScanner(self.__ptr)
                 self.__ptr = None
-        except:
-            pass
 
     def __create_scanner(self, filters: list):
         filters_len = len(filters)
         status = OpStatus()
         filters_values = (c_ubyte * filters_len)(*[filters[i].value for i in range(filters_len)])
         self.__ptr = _neuro_lib.createScanner(filters_values, filters_len, byref(status))
         raise_exception_if(status)
@@ -82,82 +88,100 @@
                                   Name=''.join([chr(c) for c in sensors_ptr[i].Name]).rstrip('\x00'),
                                   Address=''.join([chr(c) for c in sensors_ptr[i].Address]).rstrip('\x00'),
                                   SerialNumber=''.join([chr(c) for c in sensors_ptr[i].SerialNumber]).rstrip('\x00'),
                                   PairingRequired=bool(int(sensors_ptr[i].PairingRequired))) for i in range(sz_sensors)]
             if user_data.sensorsChanged is not None:
                 user_data.sensorsChanged(user_data, sensors)
 
+        status = OpStatus()
         self.__sensorsCallback = SensorCallbackScanner(__py_sensor_callback_scanner)
         self.__sensorsCallbackHandle = SensorsListenerHandle()
-        raise_exception_if(_neuro_lib.addSensorsCallbackScanner(self.__ptr, self.__sensorsCallback,
-                                                                byref(self.__sensorsCallbackHandle), py_object(self)))
+        _neuro_lib.addSensorsCallbackScanner(self.__ptr, self.__sensorsCallback,
+                                             byref(self.__sensorsCallbackHandle), py_object(self),
+                                             byref(status))
+        raise_exception_if(status)
 
-    def Sensors(self) -> [SensorInfo]:
+    def sensors(self) -> [SensorInfo]:
         """
         The method requests all found and valid devices in the current search session
 
         :return:
             List of founded devices
 
         :raises BaseException:
             If an internal error occurred while getting sensors list
         """
+        status = OpStatus()
         sz_sensors_in_out = SizeType(c_int32(64))
-        SIP = POINTER(NativeSensorInfo)
-        sensors = SIP(NativeSensorInfo())
-        raise_exception_if(_neuro_lib.sensorsScanner(self.__ptr, sensors, sz_sensors_in_out))
-        infos = []
+        sip = POINTER(NativeSensorInfo)
+        sensors = sip(NativeSensorInfo())
+        _neuro_lib.sensorsScanner(self.__ptr, sensors, sz_sensors_in_out, byref(status))
+        raise_exception_if(status)
+        sensors_info = []
         for i in range(sz_sensors_in_out.contents.value):
-            infos.append(SensorInfo(SensFamily=SensorFamily(sensors[i].SensFamily),
-                                    SensModel=sensors[i].SensModel,
-                                    Name=''.join([chr(c) for c in sensors[i].Name]).rstrip('\x00'),
-                                    Address=''.join([chr(c) for c in sensors[i].Address]).rstrip('\x00'),
-                                    SerialNumber=''.join([chr(c) for c in sensors[i].SerialNumber]).rstrip('\x00'),
-                                    PairingRequired=bool(int(sensors[i].PairingRequired))))
-        return infos
+            sensors_info.append(
+                SensorInfo(SensFamily=SensorFamily(sensors[i].SensFamily),
+                           SensModel=sensors[i].SensModel,
+                           Name=''.join([chr(c) for c in sensors[i].Name]).rstrip('\x00'),
+                           Address=''.join([chr(c) for c in sensors[i].Address]).rstrip('\x00'),
+                           SerialNumber=''.join([chr(c) for c in sensors[i].SerialNumber]).rstrip(
+                           '\x00'),
+                           PairingRequired=bool(int(sensors[i].PairingRequired))))
+        return sensors_info
 
-    def Start(self):
+    def start(self):
         """
         Starts the process of searching for devices according to the specified parameters. If the device is found,
-        sensorsChanged callback will be called. If the device leaves the scope for any reason, it will disappear from the list of
-        found devices after 12 seconds
+        sensorsChanged callback will be called. If the device leaves the scope for any reason, it will disappear from
+        the list of found devices after 12 seconds
 
         :raises BaseException:
             If an internal error occurred while starting search
         """
-        raise_exception_if(_neuro_lib.startScanner(self.__ptr))
+        status = OpStatus()
+        _neuro_lib.startScanner(self.__ptr, byref(status), 1)
+        raise_exception_if(status)
 
-    def Stop(self):
+    def stop(self):
         """
         Stops the process of searching for devices
 
         :raises BaseException:
             If an internal error occurred while stopping search
         """
-        raise_exception_if(_neuro_lib.stopScanner(self.__ptr))
-
-    def CreateSensor(self, sensor_info: SensorInfo) -> Sensor:
+        status = OpStatus()
+        _neuro_lib.stopScanner(self.__ptr, byref(status))
+        raise_exception_if(status)
+        
+    def create_sensor(self, sensor_info: SensorInfo) -> Sensor:
         """
         Creates an instance of the device according to the information received, and automatically connects to it. The
         connection callback will not be called. If the connection is successful, a Sensor instance will be returned,
         otherwise an exception will be thrown
 
         :param sensor_info: SensorInfo
             Info about device.
         :return: Sensor
             Connected device object
         :raises BaseException:
             If an internal error occurred while creating device
-
         """
+
         status = OpStatus()
         si = NativeSensorInfo()
         si.SensFamily = sensor_info.SensFamily.value
         si.SensorModel = sensor_info.SensModel
         si.Name = sensor_info.Name.encode('utf-8')
         si.Address = sensor_info.Address.encode('utf-8')
         si.SerialNumber = sensor_info.SerialNumber.encode('utf-8')
         si.PairingRequired = int(sensor_info.PairingRequired)
 
         sensor_ptr = _neuro_lib.createSensor(self.__ptr, si, byref(status))
         raise_exception_if(status)
-        return Sensor(sensor_ptr)
+        family = sensor_info.SensFamily
+        if family in (SensorFamily.SensorLECallibri, SensorFamily.SensorLEKolibri):
+            return CallibriSensor(sensor_ptr)
+        if family is SensorFamily.SensorLEBrainBit:
+            return BrainBitSensor(sensor_ptr)
+        if family is SensorFamily.SensorLEBrainBitBlack:
+            return BrainBitBlackSensor(sensor_ptr)
+        return Sensor(sensor_info)
```

### Comparing `pyneurosdk2-1.0.3.0.post3/pyneurosdk2.egg-info/PKG-INFO` & `pyneurosdk2-1.0.4.post1/pyneurosdk2.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pyneurosdk2
-Version: 1.0.3.0.post3
+Version: 1.0.4.post1
 Summary: Python wrapper for NeuroSDK2
 Home-page: https://gitlab.com/brainbit-inc/brainbit-sdk
 Author: Brainbit Inc.
 Author-email: support@brainbit.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Python NeuroSDK 2
 
 Welcome to the Python NeuroSDK 2. The Neurosdk library is designed to work with BrainBit, BrainBitBlack, Callibri and Kolibri devices. The library is intended for python version 3.7 and higher, Windows version 10 and higher.
 
 ## Documentation
 
@@ -49,49 +50,49 @@
 ```python
 from neurosdk.scanner import Scanner
 ```
 
 - sensor - methods of interaction with the device
 
 ```python
-from neurosdk.sensor import Sensor
+from neurosdk.callibri_sensor import CallibriSensor
+from neurosdk.brainbit_sensor import BrainBitSensor
+from neurosdk.brainbit_black_sensor import BrainBitBlackSensor
 ```
 
 - types - implementation of all types of the library, you can either connect everything or only those necessary for a specific task
 
 ```python
 from neurosdk.cmn_types import *
 ```
 
-Here is a description of how to work with a BrainBit device.
-
 ## Searching device
 
 The `Scanner` class is used to search for a device. For a correct search, you must specify the list of device types. You can search for one or more device types at the same time. For example, to search for BrainBit and Callibri, you need to create a scanner as follows:
 
 ```python
 scanner = Scanner([SensorFamily.SensorLEBrainBit, SensorFamily.SensorLECallibri])
 ```
 
 Search start:
 
 ```python
-scanner.Start()
+scanner.start()
 ```
 
 Stop search:
 
 ```python
-scanner.Stop()
+scanner.stop()
 ```
 
 All found devices can be obtained using the method:
 
 ```python
-sensors = scanner.Sensors()
+sensors = scanner.sensors()
 ```
 
 During the search, an `sensorsChanged` callback will be called, which will display a list of found devices. If the device leaves the scanner's field of view for any reason, the device will disappear from the list after 12 seconds.
 
 ```python
 def sensorFound(scanner, sensors):
    for i in range(len(sensors)):
@@ -109,59 +110,59 @@
 - SerialNumber: str
 - PairingRequired: bool
 
 > Important!
 > The serial number of the Callibri and Kolibri does not appear in the SensorInfo recieving during the search. To get this value, you need to connect to the device and request the serial number manually:
 >
 > ```python
-> sn = sensor.SerialNumber
+> sn = sensor.serial_number
 > ```
 
 
 ## Connection
 
 Next, you can create any device from the list using the method:
 
 ```python
-sensor = scanner.CreateSensor(sensInfo)
+sensor = scanner.create_sensor(sensInfo)
 ```
 When created, the device will connect automatically. This is a blocking function, so it is desirable to call it from an separate thread. Upon successful connection, a sensor instance will be returned. If unsuccessful, an exception is thrown. On subsequent connections and disconnections, a callback will be called indicating the state of the device.
 
 To disconnect from the device, use the following method:
 
 ```python
-sensor.Disconnect()
+sensor.disconnect()
 ```
 
 To connect to a device created but not connected for any reason, the method:
 
 ```python
-sensor.Connect()
+sensor.connect()
 ```
 
 It is blocking too.
 
 ## Parameters
 
 SDK allows you to get information about the connected device:
 
 ```python
-print(sensor.SensFamily) # SensorFamily.SensorLEBrainBit
-print(sensor.Features) # [<SensorFeature.FeatureSignal: 0>, ...]
-print(sensor.Commands) # [<SensorCommand.CommandStartSignal: 0>,...]
-print(sensor.Parameters)
-print(sensor.Name) # BrainBit
-print(sensor.State) # SensorState.StateInRange
-print(sensor.Address) # AA:BB:CC:DD:EE:FF
-print(sensor.SerialNumber) # 123456
-print(sensor.BattPower) # 50
-print(sensor.SamplingFrequency) # SensorSamplingFrequency.FrequencyHz250
-print(sensor.Gain) # SensorGain.SensorGain6
-print(sensor.DataOffset) # SensorDataOffset.DataOffset0
-print(sensor.Version) # SensorVersion(FwMajor=50, FwMinor=0, FwPatch=0, HwMajor=1, HwMinor=0, HwPatch=0, ExtMajor=65)
+print(sensor.sens_family)  # SensorFamily.SensorLEBrainBit
+print(sensor.features)  # [<SensorFeature.FeatureSignal: 0>, ...]
+print(sensor.commands)  # [<SensorCommand.CommandStartSignal: 0>,...]
+print(sensor.parameters)
+print(sensor.name)  # BrainBit
+print(sensor.state)  # SensorState.StateInRange
+print(sensor.address)  # AA:BB:CC:DD:EE:FF
+print(sensor.serial_number)  # 123456
+print(sensor.batt_power)  # 50
+print(sensor.sampling_frequency)  # SensorSamplingFrequency.FrequencyHz250
+print(sensor.gain)  # SensorGain.SensorGain6
+print(sensor.data_offset)  # SensorDataOffset.DataOffset0
+print(sensor.version)  # SensorVersion(FwMajor=50, FwMinor=0, FwPatch=0, HwMajor=1, HwMinor=0, HwPatch=0, ExtMajor=65)
 ```
 
 >  You can distinguish BrainBit device from Flex by the firmware version number: if the `SensorVersion.FwMajor` is more than 100 - it's Flex, if it's less than BrainBit.
 
 If you need to change any property, you first need to check if it is writable. This can be done by reading the list of device parameters, where each parameter will have an access level:
 
 ```
@@ -169,31 +170,31 @@
  ParameterInfo(Param=<SensorParameter.ParameterState: 1>,  ParamAccess=<SensorParamAccess.ParamAccessReadNotify: 2>)
  ...]
 ```
 
 And also check the support of certain modules:
 
 ```python
-sensor.IsSupportedFeature(sensor_future)
-sensor.IsSupportedCommand(sensor_command)
-sensor.IsSupportedParameter(sensor_parameter)
+sensor.is_supported_feature(sensor_future)
+sensor.is_supported_command(sensor_command)
+sensor.is_supported_parameter(sensor_parameter)
 ```
 
 ## Receiving signal
 
 For any device that supports recieving signal, you can run the following commands for starting:
 
 ```python
-sensor.ExecCommand(SensorCommand.CommandStartSignal)
+sensor.exec_command(SensorCommand.CommandStartSignal)
 ```
 
 Stop:
 
 ```python
-sensor.ExecCommand(SensorCommand.CommandStopSignal)
+sensor.exec_command(SensorCommand.CommandStopSignal)
 ```
 
 ### BrainBit, BrainBitBlack, Flex
 
 You can get the signal value using the callback:
 
 ```python
@@ -246,20 +247,21 @@
 
 Resistance is only supported by BrainBit, BrainBitBlack and Flex. You can also check the availability of these features using the method `sensor.IsSupportedFeature(SensorFeature.FeatureResist)`.
 
 To get resistance values:
 
 ```python
 def onBrainBitResistDataReceived(sensor, data):
-   print(data)
+    print(data)
+
 
 sensor.brainBitResistDataReceived = onBrainBitResistDataReceived
 
-sensor.ExecCommand(SensorCommand.CommandStartResist)
-sensor.ExecCommand(SensorCommand.CommandStopResist)
+sensor.exec_command(SensorCommand.CommandStartResist)
+sensor.exec_command(SensorCommand.CommandStopResist)
 ```
 
 The callback returns one packet of samples, each packet contains the resistance values in volts:
 - O1: float
 - O2: float
 - T3: float
 - T4: float
@@ -268,21 +270,21 @@
 
 ```python
 sensor.brainBitResistDataReceived = None
 ```
 
 > BrainBit cannot be in the resistance and signal readout mode at the same time, so you must first get the resistance values, but only after this signal, or vice versa. For example:
 > ```python
-> sensor.ExecCommand(SensorCommand.CommandStartResist)
+> sensor.exec_command(SensorCommand.CommandStartResist)
 > sleep(10)
-> sensor.ExecCommand(SensorCommand.CommandStopResist)
+> sensor.exec_command(SensorCommand.CommandStopResist)
 > ...
-> sensor.ExecCommand(SensorCommand.CommandStartSignal)
+> sensor.exec_command(SensorCommand.CommandStartSignal)
 > sleep(10)
-> sensor.ExecCommand(SensorCommand.CommandStopSignal)
+> sensor.exec_command(SensorCommand.CommandStopSignal)
 > ```
 
 ## Electrodes connection
 
 Electrode placement check is available for Callibri and Kolibri devices. This data shows whether the electrodes are attached to the skin.
 
 ```python
```

