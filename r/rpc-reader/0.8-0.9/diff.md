# Comparing `tmp/rpc_reader-0.8.tar.gz` & `tmp/rpc_reader-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rpc_reader-0.8.tar", last modified: Tue Aug 30 19:39:35 2022, max compression
+gzip compressed data, was "rpc_reader-0.9.tar", last modified: Wed May  3 20:10:03 2023, max compression
```

## Comparing `rpc_reader-0.8.tar` & `rpc_reader-0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-30 19:39:35.000000 rpc_reader-0.8/
--rw-rw-rw-   0 root         (0) root         (0)    35171 2022-08-30 19:39:20.000000 rpc_reader-0.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      123 2022-08-30 19:39:20.000000 rpc_reader-0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3005 2022-08-30 19:39:35.000000 rpc_reader-0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2491 2022-08-30 19:39:20.000000 rpc_reader-0.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-08-30 19:39:20.000000 rpc_reader-0.8/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-30 19:39:35.000000 rpc_reader-0.8/rpc_reader/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-30 19:39:20.000000 rpc_reader-0.8/rpc_reader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-30 19:39:35.000000 rpc_reader-0.8/rpc_reader/lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-30 19:39:20.000000 rpc_reader-0.8/rpc_reader/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1714 2022-08-30 19:39:20.000000 rpc_reader-0.8/rpc_reader/lib/print_progressbar.py
--rw-rw-rw-   0 root         (0) root         (0)    17227 2022-08-30 19:39:20.000000 rpc_reader-0.8/rpc_reader/rpc_reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-30 19:39:35.000000 rpc_reader-0.8/rpc_reader.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3005 2022-08-30 19:39:35.000000 rpc_reader-0.8/rpc_reader.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      408 2022-08-30 19:39:35.000000 rpc_reader-0.8/rpc_reader.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-30 19:39:35.000000 rpc_reader-0.8/rpc_reader.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2022-08-30 19:39:35.000000 rpc_reader-0.8/rpc_reader.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2022-08-30 19:39:35.000000 rpc_reader-0.8/rpc_reader.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-08-30 19:39:35.000000 rpc_reader-0.8/rpc_reader.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-30 19:39:35.000000 rpc_reader-0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      933 2022-08-30 19:39:20.000000 rpc_reader-0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-30 19:39:35.000000 rpc_reader-0.8/test/
--rw-rw-rw-   0 root         (0) root         (0)     7481 2022-08-30 19:39:20.000000 rpc_reader-0.8/test/test_unittests_data_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 20:10:03.079133 rpc_reader-0.9/
+-rw-rw-rw-   0 root         (0) root         (0)    35171 2023-05-03 20:09:44.000000 rpc_reader-0.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-05-03 20:09:44.000000 rpc_reader-0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3108 2023-05-03 20:10:03.079133 rpc_reader-0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2594 2023-05-03 20:09:44.000000 rpc_reader-0.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-03 20:09:44.000000 rpc_reader-0.9/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 20:10:03.076132 rpc_reader-0.9/rpc_reader/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 20:09:44.000000 rpc_reader-0.9/rpc_reader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 20:10:03.078132 rpc_reader-0.9/rpc_reader/lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 20:09:44.000000 rpc_reader-0.9/rpc_reader/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2023-05-03 20:09:44.000000 rpc_reader-0.9/rpc_reader/lib/print_progressbar.py
+-rw-rw-rw-   0 root         (0) root         (0)    18091 2023-05-03 20:09:44.000000 rpc_reader-0.9/rpc_reader/rpc_reader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 20:10:03.078132 rpc_reader-0.9/rpc_reader.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3108 2023-05-03 20:10:02.000000 rpc_reader-0.9/rpc_reader.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-03 20:10:03.000000 rpc_reader-0.9/rpc_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 20:10:02.000000 rpc_reader-0.9/rpc_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-03 20:10:02.000000 rpc_reader-0.9/rpc_reader.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-03 20:10:02.000000 rpc_reader-0.9/rpc_reader.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-03 20:10:02.000000 rpc_reader-0.9/rpc_reader.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 20:10:03.080133 rpc_reader-0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      933 2023-05-03 20:09:44.000000 rpc_reader-0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 20:10:03.079133 rpc_reader-0.9/test/
+-rw-rw-rw-   0 root         (0) root         (0)    10365 2023-05-03 20:09:45.000000 rpc_reader-0.9/test/test_unittests_data_manager.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rpc_reader-0.8/LICENSE` & `rpc_reader-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rpc_reader-0.8/PKG-INFO` & `rpc_reader-0.9/rpc_reader.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rpc_reader
-Version: 0.8
+Name: rpc-reader
+Version: 0.9
 Summary: Application to read MTS PRC3 files
 Home-page: https://gitlab.com/t8237/rpc_reader
 Author: Niklas Melin
 Author-email: niklas.melin@scania.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -15,16 +15,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # rpc_reader
 
 [![PyPI version](https://img.shields.io/pypi/v/rpc-reader.svg)](https://pypi.org/project/rpc-reader/)
 [![Build Status](https://gitlab.com/t8237/rpc_reader/badges/master/pipeline.svg)](https://gitlab.com/t8237/rpc_reader/-/commits/master)
-[![codecov](https://gitlab.com/t8237/rpc_reader/badges/master/coverage.svg)](https://gitlab.com/t8237/rpc_reader/-/commits/master)
-
+[![coverage report](https://gitlab.com/t8237/rpc_reader/badges/RC_0.9/coverage.svg)](https://gitlab.com/t8237/rpc_reader/-/commits/RC_0.9)
 
 
 A RPC III file is a data file conforming to the RPC III file specification developed by MTS corporation. This utility reads RPC format and store the data using Numpy arrays. 
 
 This reader does not have the capacity to read all variants specified in the [documentation](https://corp.mts.com/cs/groups/public/documents/library/mts_007569.pdf) provided by MTS.
 
 ## Installation
@@ -39,50 +38,53 @@
 
 
 ## Usage
 ### Python module
 
 ```python
 import pathlib
-from rpc_reader import rpc_reader
+import rpc_reader
 
 # Set path to file
-rpc_file_path = pathlib.Path('rpc_file_path.prc')
+rpc_file_path = pathlib.Path('rpc_file_path.rpc')
 
 # Instantiate reader object
-prc_object = rpc_reader.ReadRPC(rpc_file_path)
+rpc_object = rpc_reader.ReadRPC(rpc_file_path)
 
 # Import data
-prc_object.import_rpc_data_from_file()
+rpc_object.import_rpc_data_from_file()
 
 # Export data to numpy as compressed npz file
-prc_object.save_npy_data_to_file()
+rpc_object.save_npy_data_to_file()
 
 # Get headers
-headers = prc_object.get_headers()
+headers = rpc_object.get_headers()
 
 # Get channels
-channels = prc_object.get_channels()
+channels = rpc_object.get_channels()
 
 # Get measurement data as a numpy array
-data = prc_object.get_data()
+data = rpc_object.get_data()
 ```
 
 ### Command line usage
 The command line version will read the content of the rpc-file and export it as a Numpy compressed npz file.
 
 ```bash
 # This will export source data to path_to_file.npz
 rpc_reader path_to_file.rpc
 
 # Add extra headers missing in the source data and export it to path_to_file.npz
-rpc_reader path_to_file.rpc -extra-header MY_HEADER MY_HEADER_VALUE -extra-header ENGINEER_NAME BAT_MAN
+rpc_reader path_to_file.rpc --extra-header MY_HEADER MY_HEADER_VALUE --extra-header ENGINEER_NAME BAT_MAN
 ```
 
 # Version history
+## 0.9
+ - Bug fixes for FLOATING_POINT DATA_TYPE
+ - Type hints introduced
 ## 0.8
  - Added possibility to add extra headers from command line
 ## 0.7
  - Minor cleanup of code
 ## 0.6
  - Corrected header reading
  - Allow for reading of demultiplexed data
@@ -93,10 +95,12 @@
  - First  public version with working basic functionality
 
 # Contribution and bug reports
 Please use this issue tracker in the on gitlab.com for issues and enhancements!
 [rpc-reader issues](https://gitlab.com/t8237/rpc_reader/-/issues)  
 
 ## Contributors
-Niklas Melin
+Niklas Melin \
+Michal Galuszka \
+Zhang Xing Jing
```

### Comparing `rpc_reader-0.8/README.md` & `rpc_reader-0.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # rpc_reader
 
 [![PyPI version](https://img.shields.io/pypi/v/rpc-reader.svg)](https://pypi.org/project/rpc-reader/)
 [![Build Status](https://gitlab.com/t8237/rpc_reader/badges/master/pipeline.svg)](https://gitlab.com/t8237/rpc_reader/-/commits/master)
-[![codecov](https://gitlab.com/t8237/rpc_reader/badges/master/coverage.svg)](https://gitlab.com/t8237/rpc_reader/-/commits/master)
-
+[![coverage report](https://gitlab.com/t8237/rpc_reader/badges/RC_0.9/coverage.svg)](https://gitlab.com/t8237/rpc_reader/-/commits/RC_0.9)
 
 
 A RPC III file is a data file conforming to the RPC III file specification developed by MTS corporation. This utility reads RPC format and store the data using Numpy arrays. 
 
 This reader does not have the capacity to read all variants specified in the [documentation](https://corp.mts.com/cs/groups/public/documents/library/mts_007569.pdf) provided by MTS.
 
 ## Installation
@@ -22,50 +21,53 @@
 
 
 ## Usage
 ### Python module
 
 ```python
 import pathlib
-from rpc_reader import rpc_reader
+import rpc_reader
 
 # Set path to file
-rpc_file_path = pathlib.Path('rpc_file_path.prc')
+rpc_file_path = pathlib.Path('rpc_file_path.rpc')
 
 # Instantiate reader object
-prc_object = rpc_reader.ReadRPC(rpc_file_path)
+rpc_object = rpc_reader.ReadRPC(rpc_file_path)
 
 # Import data
-prc_object.import_rpc_data_from_file()
+rpc_object.import_rpc_data_from_file()
 
 # Export data to numpy as compressed npz file
-prc_object.save_npy_data_to_file()
+rpc_object.save_npy_data_to_file()
 
 # Get headers
-headers = prc_object.get_headers()
+headers = rpc_object.get_headers()
 
 # Get channels
-channels = prc_object.get_channels()
+channels = rpc_object.get_channels()
 
 # Get measurement data as a numpy array
-data = prc_object.get_data()
+data = rpc_object.get_data()
 ```
 
 ### Command line usage
 The command line version will read the content of the rpc-file and export it as a Numpy compressed npz file.
 
 ```bash
 # This will export source data to path_to_file.npz
 rpc_reader path_to_file.rpc
 
 # Add extra headers missing in the source data and export it to path_to_file.npz
-rpc_reader path_to_file.rpc -extra-header MY_HEADER MY_HEADER_VALUE -extra-header ENGINEER_NAME BAT_MAN
+rpc_reader path_to_file.rpc --extra-header MY_HEADER MY_HEADER_VALUE --extra-header ENGINEER_NAME BAT_MAN
 ```
 
 # Version history
+## 0.9
+ - Bug fixes for FLOATING_POINT DATA_TYPE
+ - Type hints introduced
 ## 0.8
  - Added possibility to add extra headers from command line
 ## 0.7
  - Minor cleanup of code
 ## 0.6
  - Corrected header reading
  - Allow for reading of demultiplexed data
@@ -76,8 +78,10 @@
  - First  public version with working basic functionality
 
 # Contribution and bug reports
 Please use this issue tracker in the on gitlab.com for issues and enhancements!
 [rpc-reader issues](https://gitlab.com/t8237/rpc_reader/-/issues)  
 
 ## Contributors
-Niklas Melin
+Niklas Melin \
+Michal Galuszka \
+Zhang Xing Jing
```

### Comparing `rpc_reader-0.8/rpc_reader/lib/print_progressbar.py` & `rpc_reader-0.9/rpc_reader/lib/print_progressbar.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-def print_progressbar(iteration,
-                      total,
-                      prefix='',
-                      suffix='',
-                      decimals=1,
-                      length=100,
-                      fill='█',
-                      print_end="\r"):
+def print_progressbar(iteration: int,
+                      total: int,
+                      prefix: str = '',
+                      suffix: str = '',
+                      decimals: int = 1,
+                      length: int = 100,
+                      fill: str = '█',
+                      print_end: str = "\r"):
     """
     Call in a loop to create terminal progress bar
     @params:
         iteration   - Required  : current iteration (Int)
         total       - Required  : total iterations (Int)
         prefix      - Optional  : prefix string (Str)
         suffix      - Optional  : suffix string (Str)
@@ -24,19 +24,7 @@
     percent = ("{0:." + str(decimals) + "f}").format(100 * (iteration / float(total)))
     filled_length = int(length * iteration // total)
     bar = fill * filled_length + '-' * (length - filled_length)
     print(f'\r\t{prefix} |{bar}| {percent}% {suffix}', end=print_end, flush=True)
     # Print New Line on Complete
     if iteration == total:
         print()
-
-
-if __name__ == "__main__":
-    # Initial call to print 0% progress
-    import time
-    totals = 100
-    print_progressbar(0, totals, prefix='Progress:', suffix='Complete', length=50)
-    for i in range(totals):
-        # Do stuff...
-        time.sleep(0.05)
-        # Update Progress Bar
-        print_progressbar(i + 1, totals, prefix='Progress:', suffix='Complete', length=50)
```

### Comparing `rpc_reader-0.8/rpc_reader/rpc_reader.py` & `rpc_reader-0.9/rpc_reader/rpc_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,67 +4,68 @@
 
 import numpy
 import os
 import pathlib
 import struct
 import sys
 import textwrap
+import typing
 
 # Import custom modules
-from rpc_reader.lib.print_progressbar import print_progressbar
+from .lib.print_progressbar import print_progressbar
 
 # Allow for multiple data types from header DATA_TYPE.
 DATA_TYPES = {'FLOATING_POINT': {'unpack_char': 'f', 'bytes': 4},
               'SHORT_INTEGER': {'unpack_char': 'h', 'bytes': 2}}
 
 
 class ReadRPC(object):
     """
     Read RPC III files.
     A RPC III file is a data  file conforming to the RPC III  file specification developed by MTS corporation.
 
-    In this implementation the full data structure of the PRC file is NOT supported.
+    In this implementation the full data structure of the RPC file is NOT supported.
 
     TODO:
         Support demultiplexed data format. Here it is assumed that only one frame exist in every group but this is
         generally not the case.
 
     Niklas Melin
     2022-02-26
     """
 
-    def __init__(self, _file, extra_headers=None, debug=False):
+    def __init__(self, _file: typing.Union[str, pathlib.Path], extra_headers: dict = None, debug: bool = False):
 
         if extra_headers is None:
             extra_headers = []
-        self.debug = debug
-        self.headers = dict()
-        self.channels = dict()
-        self.data = None
-        self.time = None
-        self.__data_type__ = None
-        self.__file_size__ = None
-        self.__headers_read__ = False
-        self.__data_read__ = False
-        self.__extra_headers__ = dict()
+        self.debug: bool = debug
+        self.headers: dict = dict()
+        self.channels: dict = dict()
+        self.data: typing.Optional[numpy.array] = None
+        self.time: typing.Optional[numpy.array] = None
+        self.__data_type__: typing.Optional[str] = None
+        self.__file_size__: typing.Optional[int] = None
+        self.__headers_read__: bool = False
+        self.__data_read__: bool = False
+        self.__extra_headers__: dict = dict()
 
         # Standard integer full scale
         self.integer_standard_full_scale = 32768
 
         # Check received _file
         if not isinstance(_file, pathlib.Path):
             _file = pathlib.Path(_file)
         if not _file.is_file():
-            sys.exit("ERROR: The PRC test data file is invalid")
+            sys.exit("ERROR: The RPC test data file is invalid")
         self.file = _file
 
         try:
             for header_name, header_value in extra_headers:
                 self.__extra_headers__[header_name.upper()] = header_value.upper()
-        except:
+        except Exception:
             if 'header_name' in locals() and 'header_value' in locals():
                 msg = 'ERROR: Additional headers could not be interpreted!' \
                       f'\n\t Header name:  {header_name}' \
                       f'\n\t Header value: {header_value}'
             else:
                 msg = 'ERROR: Header data could not be interpreted! Check input...'
             sys.exit(msg)
@@ -79,16 +80,16 @@
             file_handle.seek(0, 0)
 
     def __read_header__(self, file_handle):
         def __header__():
             try:
                 # Read header
                 __head__, __value__ = struct.unpack('<32s96s', file_handle.read(128))
-                __value__ = __value__.rstrip(b'\0').decode('utf-8')
-                __head__ = __head__.rstrip(b'\0').decode('utf-8')
+                __value__ = __value__.replace(b'\0', b'').decode('windows-1252').replace('\n', '')
+                __head__ = __head__.replace(b'\0', b'').decode('windows-1252').replace('\n', '')
                 return __head__, __value__
             except struct.error:
                 sys.exit('ERROR: Header of the file does not contain sufficient data to read 128 bytes')
             except UnicodeDecodeError:
                 sys.exit('ERROR: Header of the file could not be decoded properly, exiting!')
 
         # Read first three records, which are mandatory and also position sensitive
@@ -134,16 +135,20 @@
         try:
             self.headers['NUM_HEADER_BLOCKS'] = int(self.headers['NUM_HEADER_BLOCKS'])
             self.headers['CHANNELS'] = int(self.headers['CHANNELS'])
             self.headers['DELTA_T'] = float(self.headers['DELTA_T'])
             self.headers['PTS_PER_FRAME'] = int(self.headers['PTS_PER_FRAME'])
             self.headers['PTS_PER_GROUP'] = int(self.headers['PTS_PER_GROUP'])
             self.headers['FRAMES'] = int(self.headers['FRAMES'])
-            self.headers['INT_FULL_SCALE'] = int(self.headers['INT_FULL_SCALE'])
             self.__data_type__ = self.headers['DATA_TYPE']
+
+            # Require INT_FULL_SCALE only if DATA_TYPE is SHORT_INTEGER
+            if self.__data_type__ == 'SHORT_INTEGER':
+                self.headers['INT_FULL_SCALE'] = int(self.headers['INT_FULL_SCALE'])
+
         except KeyError as expected_header:
             sys.exit(f'ERROR: A mandatory header is missing: {expected_header}')
 
         # Structure channel data structure
         for channel in range(int(self.headers['CHANNELS'])):
             try:
                 self.channels[channel] = {}
@@ -238,28 +243,29 @@
 
                     r1 = (frame - 1) * point_per_frame
                     r2 = frame * point_per_frame
                     self.data[r1:r2, channel] = data
 
             print_progressbar(frame, frames, prefix='Progress:', suffix='Complete', length=50)
 
-        # Scale channel data
-        for channel in range(channels):
-            # Channel scale
-            channel_scale = self.channels[channel]['Scale']
-            # Standard integer full scale
-            int_standard_full_scale = self.integer_standard_full_scale
-            # RPC integer full scale
-            int_rpc_full_scale = self.headers['INT_FULL_SCALE']
+        # Scale channel data - valid only if DATA_TYPE is SHORT_INTEGER
+        if self.__data_type__ == 'SHORT_INTEGER':
+            for channel in range(channels):
+                # Channel scale
+                channel_scale = self.channels[channel]['Scale']
+                # Standard integer full scale
+                int_standard_full_scale = self.integer_standard_full_scale
+                # RPC integer full scale
+                int_rpc_full_scale = self.headers['INT_FULL_SCALE']
 
-            # Compute scale factor
-            scale_factor = int_rpc_full_scale / int_standard_full_scale * channel_scale
+                # Compute scale factor
+                scale_factor = int_rpc_full_scale / int_standard_full_scale * channel_scale
 
-            # Scale data
-            self.data[:, channel] = self.data[:, channel] * scale_factor
+                # Scale data
+                self.data[:, channel] = self.data[:, channel] * scale_factor
 
         # Create matching time history array
         self.time = numpy.arange(1, frames * point_per_frame + 1, dtype=numpy.float32) * self.headers['DELTA_T']
 
         # Indicate that the data has been read
         self.__data_read__ = True
 
@@ -273,15 +279,15 @@
             self.__read_data__(file_handle)
 
     def save_npy_data_to_file(self, overwrite=False):
 
         file_path_data = self.file.with_suffix('.npz')
 
         if file_path_data.is_file() and not overwrite:
-            print(f' ERROR: A _file exists and over write mode is: {overwrite}')
+            print(f' ERROR: A numpy result file exists and over write mode is: {overwrite}')
             return
         data = self.data
         times = self.time
         headers = self.headers
         channels = self.channels
         numpy.savez(file_path_data,
                     data=data,
@@ -311,49 +317,49 @@
 
         # Set data available
         self.__data_read__ = True
         self.__headers_read__ = True
 
         print(f' Data was imported from _file: {file_path_data.as_posix()}')
 
-    def get_data(self):
+    def get_data(self) -> typing.Union[numpy.array, bool]:
         if not self.__data_read__:
-            print('ERROR: No data has been read!')
+            print(' ERROR: No data has been read!')
             return False
         return self.data
 
-    def get_time(self):
+    def get_time(self) -> typing.Union[typing.Tuple[numpy.array, float], bool]:
         if not self.__data_read__:
-            print('ERROR: No data has been read!')
+            print(' ERROR: No data has been read!')
             return False
 
         return self.time, self.time[-1]
 
-    def get_data_size(self):
+    def get_data_size(self) -> typing.Union[typing.Tuple[int], bool]:
         if not self.__data_read__:
-            print('ERROR: No data has been read!')
+            print(' ERROR: No data has been read!')
             return False
         return self.data.shape
 
-    def get_channels(self):
+    def get_channels(self) -> typing.Union[int, bool]:
         if not self.__headers_read__:
             print(' ERROR: No data loaded')
             return False
         return self.channels
 
-    def get_headers(self):
+    def get_headers(self) -> typing.Union[dict, bool]:
         if not self.__headers_read__:
             print(' ERROR: No data loaded')
             return False
         return self.headers
 
     def print_channel_header_data(self):
         if not self.__headers_read__:
             print(' ERROR: No data loaded')
-            return
+            return False
 
         for channel, data in self.channels.items():
             print(f' Channel: {channel + 1}')
             for key, value in data.items():
                 print(f' \t {key:20s} : {value}')
 
 
@@ -375,15 +381,15 @@
     # Set-up parsing of input arguments
     parser = argparse.ArgumentParser(
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description=textwrap.dedent('''
 
              Description:
              -----------------------------------------------------------------------------------------------------------
-             Application for reading PRC 3 data files into numpy arrays. In the command line version, the provided file
+             Application for reading RPC 3 data files into numpy arrays. In the command line version, the provided file
              is converted into a numpy .npz file. To load the data use the numpy.load module which will load the numpy
              data as a dictionary with the following keys:
 
                 header   - Header data
                 time     - Time array
                 channels - Channel data
                 data     - The actual measurement data
@@ -399,23 +405,27 @@
                         metavar='INPUT_PATH',
                         help="Select file containing something important \
                               \n\t  /path/to/my/input/file.rpc")
     parser.add_argument('-e', '--extra-header', action='append', nargs=2,
                         metavar=('name', 'value'), help='Set missing header and value. Repeated usage allowed!')
     parser.add_argument("--debug", "--d",
                         action="store_true",
+                        default=False,
                         help="If debug is set, significant additional output is requested.\n")
 
     # Parse arguments into a dictionary
     cmd_line_args = vars(parser.parse_args())
 
     # Get arguments
     print(cmd_line_args.items())
     input_path = cmd_line_args['input_path']
-    extra_headers = cmd_line_args['extra_header']
+    if 'extra_header' in cmd_line_args:
+        extra_headers = cmd_line_args['extra_header']
+    else:
+        extra_headers = None
     debug = cmd_line_args['debug']
 
     # Start batch process
     reader_object = ReadRPC(input_path, extra_headers=extra_headers, debug=debug)
     reader_object.import_rpc_data_from_file()
     reader_object.save_npy_data_to_file()
```

### Comparing `rpc_reader-0.8/rpc_reader.egg-info/PKG-INFO` & `rpc_reader-0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rpc-reader
-Version: 0.8
+Name: rpc_reader
+Version: 0.9
 Summary: Application to read MTS PRC3 files
 Home-page: https://gitlab.com/t8237/rpc_reader
 Author: Niklas Melin
 Author-email: niklas.melin@scania.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -15,16 +15,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # rpc_reader
 
 [![PyPI version](https://img.shields.io/pypi/v/rpc-reader.svg)](https://pypi.org/project/rpc-reader/)
 [![Build Status](https://gitlab.com/t8237/rpc_reader/badges/master/pipeline.svg)](https://gitlab.com/t8237/rpc_reader/-/commits/master)
-[![codecov](https://gitlab.com/t8237/rpc_reader/badges/master/coverage.svg)](https://gitlab.com/t8237/rpc_reader/-/commits/master)
-
+[![coverage report](https://gitlab.com/t8237/rpc_reader/badges/RC_0.9/coverage.svg)](https://gitlab.com/t8237/rpc_reader/-/commits/RC_0.9)
 
 
 A RPC III file is a data file conforming to the RPC III file specification developed by MTS corporation. This utility reads RPC format and store the data using Numpy arrays. 
 
 This reader does not have the capacity to read all variants specified in the [documentation](https://corp.mts.com/cs/groups/public/documents/library/mts_007569.pdf) provided by MTS.
 
 ## Installation
@@ -39,50 +38,53 @@
 
 
 ## Usage
 ### Python module
 
 ```python
 import pathlib
-from rpc_reader import rpc_reader
+import rpc_reader
 
 # Set path to file
-rpc_file_path = pathlib.Path('rpc_file_path.prc')
+rpc_file_path = pathlib.Path('rpc_file_path.rpc')
 
 # Instantiate reader object
-prc_object = rpc_reader.ReadRPC(rpc_file_path)
+rpc_object = rpc_reader.ReadRPC(rpc_file_path)
 
 # Import data
-prc_object.import_rpc_data_from_file()
+rpc_object.import_rpc_data_from_file()
 
 # Export data to numpy as compressed npz file
-prc_object.save_npy_data_to_file()
+rpc_object.save_npy_data_to_file()
 
 # Get headers
-headers = prc_object.get_headers()
+headers = rpc_object.get_headers()
 
 # Get channels
-channels = prc_object.get_channels()
+channels = rpc_object.get_channels()
 
 # Get measurement data as a numpy array
-data = prc_object.get_data()
+data = rpc_object.get_data()
 ```
 
 ### Command line usage
 The command line version will read the content of the rpc-file and export it as a Numpy compressed npz file.
 
 ```bash
 # This will export source data to path_to_file.npz
 rpc_reader path_to_file.rpc
 
 # Add extra headers missing in the source data and export it to path_to_file.npz
-rpc_reader path_to_file.rpc -extra-header MY_HEADER MY_HEADER_VALUE -extra-header ENGINEER_NAME BAT_MAN
+rpc_reader path_to_file.rpc --extra-header MY_HEADER MY_HEADER_VALUE --extra-header ENGINEER_NAME BAT_MAN
 ```
 
 # Version history
+## 0.9
+ - Bug fixes for FLOATING_POINT DATA_TYPE
+ - Type hints introduced
 ## 0.8
  - Added possibility to add extra headers from command line
 ## 0.7
  - Minor cleanup of code
 ## 0.6
  - Corrected header reading
  - Allow for reading of demultiplexed data
@@ -93,10 +95,12 @@
  - First  public version with working basic functionality
 
 # Contribution and bug reports
 Please use this issue tracker in the on gitlab.com for issues and enhancements!
 [rpc-reader issues](https://gitlab.com/t8237/rpc_reader/-/issues)  
 
 ## Contributors
-Niklas Melin
+Niklas Melin \
+Michal Galuszka \
+Zhang Xing Jing
```

### Comparing `rpc_reader-0.8/setup.py` & `rpc_reader-0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rpc_reader",
-    version="0.8",
+    version="0.9",
     author="Niklas Melin",
     author_email="niklas.melin@scania.com",
     description="Application to read MTS PRC3 files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/t8237/rpc_reader",
     packages=setuptools.find_packages(),
```

### Comparing `rpc_reader-0.8/test/test_unittests_data_manager.py` & `rpc_reader-0.9/test/test_unittests_data_manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import argparse
 import unittest
+from unittest import mock
 import pathlib
 import numpy as np
 
 # Get location of this file
 __this_file__ = pathlib.Path(__file__)
 __this_path__ = __this_file__.parent.resolve()
 
@@ -112,14 +114,17 @@
         data_object = ReadRPC(test_data_file)
         # Read data from file
         data_object.import_rpc_data_from_file()
 
         # Export data
         data_object.save_npy_data_to_file(overwrite=True)
 
+        # Export data again with overwrite False
+        data_object.save_npy_data_to_file(overwrite=False)
+
         self.assertTrue(True)
 
     def test_004_import_rpc_data(self):
         """
             Test import of npz data
         """
         from rpc_reader.rpc_reader import ReadRPC
@@ -169,14 +174,66 @@
 
         # Compare data RPC Pro and read data. It will not be identical due to different accuracy of float representation
         equal = np.allclose(csv_data, data_object.data, atol=0.0001, rtol=0.001)
 
         # Assert the result of the comparison
         self.assertTrue(equal, msg=' All values were not equal')
 
+    def test_006_check_non_loaded(self):
+        """
+            Compare data read data with csv data exported from RPC Pro
+        """
+
+        from rpc_reader.rpc_reader import ReadRPC
+        print(f' Reading data from file: \n\t{test_data_file.as_posix()}\n')
+
+        # Expected outcome
+        expected = [False, False, False, False, False, False]
+
+        # Instantiate instance
+        data_object = ReadRPC(test_data_file)
+
+        return_false = [data_object.print_channel_header_data(),
+                        data_object.get_headers(),
+                        data_object.get_channels(),
+                        data_object.get_data_size(),
+                        data_object.get_data(),
+                        data_object.get_time()]
+        self.assertEquals(return_false, expected, msg='All returns were not false')
+
+    def test_007_check_loaded(self):
+        """
+            Compare data read data with csv data exported from RPC Pro
+        """
+
+
+        # Expect all to be non-False
+        expected = False
+
+        from rpc_reader.rpc_reader import ReadRPC
+        print(f' Reading data from file: \n\t{test_data_file.as_posix()}\n')
+
+        # Instantiate instance
+        data_object = ReadRPC(test_data_file)
+
+        # Import data from rpc _file
+        data_object.import_rpc_data_from_file()
+
+        # Test get-methods
+        return_non_false = [data_object.print_channel_header_data(),
+                            data_object.get_headers(),
+                            data_object.get_channels(),
+                            data_object.get_data_size(),
+                            data_object.get_data(),
+                            data_object.get_time()]
+
+        false_in_return = not any(return_non_false)
+
+        self.assertEquals(false_in_return, expected, msg='All returns were not false')
+
     def test_102_progressbar(self):
         """
             Test reading of rpc data
         """
         from rpc_reader.lib.print_progressbar import print_progressbar
         import time
         total = 100
@@ -213,10 +270,35 @@
         time, test_end_time = data_object.get_time()
 
         print(f'\n Test data points read:\n\tChannels: {channels}'
               f'\n\tSamples:  {samples}'
               f'\n\tDuration: {np.round(test_end_time, 4)} seconds')
         self.assertTrue(True)
 
+    def test_401_main_read_rpc_file_2(self):
+        """
+            Test reading of rpc data - Test file 2
+        """
+        from rpc_reader.rpc_reader import ReadRPC
+        print(f' Reading data from file: \n\t{test_data_file_2.as_posix()}\n')
+
+        from unittest.mock import patch
 
-if __name__ == '__main__':
-    unittest.main()
+        # Check with extra headers
+        with patch('argparse._sys.argv',
+                   ['python',
+                    test_data_file_2.as_posix(),
+                    '--extra-header',
+                    'test_header',
+                    'test_header_value']):
+            from rpc_reader.rpc_reader import main, ReadRPC
+            main()
+
+        # Check debug and no extra header
+        with patch('argparse._sys.argv',
+                   ['python',
+                    test_data_file_2.as_posix(),
+                    '--debug']):
+            from rpc_reader.rpc_reader import main, ReadRPC
+            main()
+
+        self.assertTrue(True)
```

