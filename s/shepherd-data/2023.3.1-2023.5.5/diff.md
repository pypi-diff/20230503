# Comparing `tmp/shepherd_data-2023.3.1.tar.gz` & `tmp/shepherd_data-2023.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shepherd_data-2023.3.1.tar", last modified: Mon Mar 27 18:12:01 2023, max compression
+gzip compressed data, was "shepherd_data-2023.5.5.tar", last modified: Wed May  3 19:30:07 2023, max compression
```

## Comparing `shepherd_data-2023.3.1.tar` & `shepherd_data-2023.5.5.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:12:01.529861 shepherd_data-2023.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-27 18:11:50.000000 shepherd_data-2023.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11634 2023-03-27 18:12:01.529861 shepherd_data-2023.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-03-27 18:11:50.000000 shepherd_data-2023.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-03-27 18:11:50.000000 shepherd_data-2023.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-03-27 18:12:01.529861 shepherd_data-2023.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:12:01.525861 shepherd_data-2023.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:12:01.529861 shepherd_data-2023.3.1/src/shepherd_data/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-27 18:11:50.000000 shepherd_data-2023.3.1/src/shepherd_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-03-27 18:11:50.000000 shepherd_data-2023.3.1/src/shepherd_data/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10785 2023-03-27 18:11:50.000000 shepherd_data-2023.3.1/src/shepherd_data/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-03-27 18:11:50.000000 shepherd_data-2023.3.1/src/shepherd_data/ivonne.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-03-27 18:11:50.000000 shepherd_data-2023.3.1/src/shepherd_data/mppt.py
--rw-r--r--   0 runner    (1001) docker     (123)    36078 2023-03-27 18:11:50.000000 shepherd_data-2023.3.1/src/shepherd_data/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13261 2023-03-27 18:11:50.000000 shepherd_data-2023.3.1/src/shepherd_data/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:12:01.529861 shepherd_data-2023.3.1/src/shepherd_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11634 2023-03-27 18:12:01.000000 shepherd_data-2023.3.1/src/shepherd_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-03-27 18:12:01.000000 shepherd_data-2023.3.1/src/shepherd_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:12:01.000000 shepherd_data-2023.3.1/src/shepherd_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-27 18:12:01.000000 shepherd_data-2023.3.1/src/shepherd_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-27 18:12:01.000000 shepherd_data-2023.3.1/src/shepherd_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-27 18:12:01.000000 shepherd_data-2023.3.1/src/shepherd_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:12:01.000000 shepherd_data-2023.3.1/src/shepherd_data.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:12:01.529861 shepherd_data-2023.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-27 18:11:50.000000 shepherd_data-2023.3.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-03-27 18:11:50.000000 shepherd_data-2023.3.1/tests/test_cli_downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-03-27 18:11:50.000000 shepherd_data-2023.3.1/tests/test_cli_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-03-27 18:11:50.000000 shepherd_data-2023.3.1/tests/test_cli_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-03-27 18:11:50.000000 shepherd_data-2023.3.1/tests/test_cli_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-03-27 18:11:50.000000 shepherd_data-2023.3.1/tests/test_ivonne.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-27 18:11:50.000000 shepherd_data-2023.3.1/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-03-27 18:11:50.000000 shepherd_data-2023.3.1/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:30:07.433923 shepherd_data-2023.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-05-03 19:30:07.433923 shepherd_data-2023.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-03 19:30:07.433923 shepherd_data-2023.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:30:07.429923 shepherd_data-2023.5.5/shepherd_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/shepherd_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10745 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/shepherd_data/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/shepherd_data/debug_resampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/shepherd_data/ivonne.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/shepherd_data/mppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24800 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/shepherd_data/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:30:07.433923 shepherd_data-2023.5.5/shepherd_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-05-03 19:30:07.000000 shepherd_data-2023.5.5/shepherd_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-03 19:30:07.000000 shepherd_data-2023.5.5/shepherd_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:30:07.000000 shepherd_data-2023.5.5/shepherd_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-03 19:30:07.000000 shepherd_data-2023.5.5/shepherd_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-03 19:30:07.000000 shepherd_data-2023.5.5/shepherd_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-03 19:30:07.000000 shepherd_data-2023.5.5/shepherd_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:30:07.000000 shepherd_data-2023.5.5/shepherd_data.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:30:07.433923 shepherd_data-2023.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/tests/test_cli_downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/tests/test_cli_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/tests/test_cli_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/tests/test_cli_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/tests/test_ivonne.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/tests/test_writer.py
```

### Comparing `shepherd_data-2023.3.1/PKG-INFO` & `shepherd_data-2023.5.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd_data
-Version: 2023.3.1
+Version: 2023.5.5
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Home-page: https://pypi.org/project/shepherd-data/
 Author: Ingmar Splitt, Kai Geissdoerfer
 Author-email: ingmar.splitt@tu-dresden.de
 Maintainer-email: ingmar.splitt@tu-dresden.de
 License: MIT
 Project-URL: Tracker, https://github.com/orgua/shepherd-datalib/issues
@@ -28,15 +28,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
-License-File: LICENSE
 
 # Shepherd - Data
 
 [![PyPiVersion](https://img.shields.io/pypi/v/shepherd_data.svg)](https://pypi.org/project/shepherd_data)
 [![Pytest](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml/badge.svg)](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml)
 [![CodeStyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
@@ -160,14 +159,54 @@
   - `example_generate_sawtooth.py` is using Writer to generate a 60s ramp with 1h repetition and uses Reader to dump metadata of that file
   - `example_plot_traces.py` demos some mpl-plots with various zoom levels
   - `example_repair_recordings.py` makes old recordings from shepherd 1.x fit for v2
   - `jogging_10m.iv`
       - 50 Hz measurement with Short-Circuit-Current and two other parameters
       - recorded with "IVonne"
 
+### Functionality Update (WIP)
+
+- `BaseReader`
+  - `read_buffers`
+  - `get_calibration_data`
+  - `get_window_samples`
+  - `get_mode`
+  - `get_config`
+  - `get_hostname`
+  - `get_datatype`
+  - `get_hrv_config`
+  - `is_valid`
+
+- `BaseWriter(BaseReader)`
+  - `append_iv_data_raw`
+  - `append_iv_data_si`
+  - `set_config`
+  - `set_window_samples`
+  - `set_hostname`
+
+- `Reader(BaseReader)`
+  - `__repr__()`
+  - `check_timediffs()`
+  - `data_timediffs()`
+  - `get_metadata()`
+  - `save_metadata()`
+  - `energy()`
+  - `save_csv()`
+  - `save_log()`
+  - `downsample()`
+  - `resample()`
+  - `generate_plot_data()`
+  - `assemble_plot()`
+  - `plot_to_file()`
+  - `multiplot_to_file()`
+- `Writer(BaseWriter)`
+  - (no extending methods)
+
+
+
 ## CLI-Interface
 
 After installing the module the datalib offers some often needed functionality on the command line:
 
 **Validate Recordings**
 
 - takes a file or directory as an argument
@@ -271,56 +310,7 @@
   emu_120s_lzf_to_gz1.h5 	-> emulator, cpu_util [%] = 63.18, data-rate =  352.0 KiB/s
   emu_120s_lzf_to_lzf.h5 	-> emulator, cpu_util [%] = 58.60, data-rate =  686.0 KiB/s
   emu_120s_lzf_to_unc.h5 	-> emulator, cpu_util [%] = 55.75, data-rate = 1564.0 KiB/s
   emu_120s_unc_to_gz1.h5 	-> emulator, cpu_util [%] = 63.84, data-rate =  351.0 KiB/s
   emu_120s_unc_to_lzf.h5 	-> emulator, cpu_util [%] = 57.28, data-rate =  686.0 KiB/s
   emu_120s_unc_to_unc.h5 	-> emulator, cpu_util [%] = 51.69, data-rate = 1564.0 KiB/s
 ```
-
-## Release-Procedure
-
-- increase version number in __init__.py
-- install and run pre-commit, for QA-Checks, see steps below
-- every commit get automatically tested by Github
-- put together a release on Github - the tag should match current version-number
-- Github automatically pushes release to pypi
-
-```shell
-pip3 install pre-commit
-
-pre-commit run --all-files
-```
-
-## Open Tasks
-
-- [click progressbar](https://click.palletsprojects.com/en/8.1.x/api/#click.progressbar) -> could replace tqdm
-- implementations for this lib
-  - generalize up- and down-sampling, use out_sample_rate instead of ds-factor
-    - lib samplerate (tested) -> promising, but designed for float32 and range of +-1.0
-    - lib resampy (tested) -> could be problematic with slice-iterator
-    - https://stackoverflow.com/questions/29085268/resample-a-numpy-array
-    - scipy.signal.resample, https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.resample.html
-    - scipy.signal.decimate, https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.decimate.html
-    - scipy.signal.resample_poly, https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.resample_poly.html#scipy.signal.resample_poly
-    - timestamps could be regenerated with np.arange( tmin, tmax, 1e9/samplerate)
-  - generalize converters (currently in IVonne)
-    - isc&voc <-> ivcurve
-    - ivcurve -> ivsample
-  - plotting and downsampling for IVCurves ()
-  - plotting more generalized (power, cpu-util, ..., if IV then offer power as well)
-  - some metadata is calculated wrong (non-scalar datasets)
-  - unittests & codecoverage -> 79% with v22.5.4, https://pytest-cov.readthedocs.io/en/latest/config.html
-    - test example: https://github.com/kvas-it/pytest-console-scripts
-    - use coverage to test some edge-cases
-  - sub-divide valid() into healthy()
-  - add gain/factor to time, with repair-code
-  - add https://pypi.org/project/nessie-recorder/#files
-- main shepherd-code
-  - proper validation first
-  - update commentary
-  - pin-description should be in yaml (and other descriptions for cpu, io, ...)
-  - datatype-hint in h5-file (ivcurve, ivsample, isc_voc), add mechanism to prevent misuse
-  - hostname for emulation
-  - full and minimal config into h5
-  - use the datalib as a base
-  - isc-voc-harvesting
-  - directly process isc-voc -> resample to ivcurve?
```

### Comparing `shepherd_data-2023.3.1/README.md` & `shepherd_data-2023.5.5/shepherd_data.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,42 @@
+Metadata-Version: 2.1
+Name: shepherd-data
+Version: 2023.5.5
+Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
+Home-page: https://pypi.org/project/shepherd-data/
+Author: Ingmar Splitt, Kai Geissdoerfer
+Author-email: ingmar.splitt@tu-dresden.de
+Maintainer-email: ingmar.splitt@tu-dresden.de
+License: MIT
+Project-URL: Tracker, https://github.com/orgua/shepherd-datalib/issues
+Project-URL: Source, https://github.com/orgua/shepherd-datalib
+Keywords: testbed,beaglebone,pru,batteryless,energyharvesting,solar
+Platform: unix
+Platform: linux
+Platform: osx
+Platform: cygwin
+Platform: win32
+Platform: win64
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Natural Language :: English
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
+
 # Shepherd - Data
 
 [![PyPiVersion](https://img.shields.io/pypi/v/shepherd_data.svg)](https://pypi.org/project/shepherd_data)
 [![Pytest](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml/badge.svg)](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml)
 [![CodeStyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 This Python Module eases the handling of hdf5-recordings used by the [shepherd](https://github.com/orgua/shepherd)-testbed. Users can read, validate and create files and also extract, down-sample and plot information.
@@ -124,14 +159,54 @@
   - `example_generate_sawtooth.py` is using Writer to generate a 60s ramp with 1h repetition and uses Reader to dump metadata of that file
   - `example_plot_traces.py` demos some mpl-plots with various zoom levels
   - `example_repair_recordings.py` makes old recordings from shepherd 1.x fit for v2
   - `jogging_10m.iv`
       - 50 Hz measurement with Short-Circuit-Current and two other parameters
       - recorded with "IVonne"
 
+### Functionality Update (WIP)
+
+- `BaseReader`
+  - `read_buffers`
+  - `get_calibration_data`
+  - `get_window_samples`
+  - `get_mode`
+  - `get_config`
+  - `get_hostname`
+  - `get_datatype`
+  - `get_hrv_config`
+  - `is_valid`
+
+- `BaseWriter(BaseReader)`
+  - `append_iv_data_raw`
+  - `append_iv_data_si`
+  - `set_config`
+  - `set_window_samples`
+  - `set_hostname`
+
+- `Reader(BaseReader)`
+  - `__repr__()`
+  - `check_timediffs()`
+  - `data_timediffs()`
+  - `get_metadata()`
+  - `save_metadata()`
+  - `energy()`
+  - `save_csv()`
+  - `save_log()`
+  - `downsample()`
+  - `resample()`
+  - `generate_plot_data()`
+  - `assemble_plot()`
+  - `plot_to_file()`
+  - `multiplot_to_file()`
+- `Writer(BaseWriter)`
+  - (no extending methods)
+
+
+
 ## CLI-Interface
 
 After installing the module the datalib offers some often needed functionality on the command line:
 
 **Validate Recordings**
 
 - takes a file or directory as an argument
@@ -235,56 +310,7 @@
   emu_120s_lzf_to_gz1.h5 	-> emulator, cpu_util [%] = 63.18, data-rate =  352.0 KiB/s
   emu_120s_lzf_to_lzf.h5 	-> emulator, cpu_util [%] = 58.60, data-rate =  686.0 KiB/s
   emu_120s_lzf_to_unc.h5 	-> emulator, cpu_util [%] = 55.75, data-rate = 1564.0 KiB/s
   emu_120s_unc_to_gz1.h5 	-> emulator, cpu_util [%] = 63.84, data-rate =  351.0 KiB/s
   emu_120s_unc_to_lzf.h5 	-> emulator, cpu_util [%] = 57.28, data-rate =  686.0 KiB/s
   emu_120s_unc_to_unc.h5 	-> emulator, cpu_util [%] = 51.69, data-rate = 1564.0 KiB/s
 ```
-
-## Release-Procedure
-
-- increase version number in __init__.py
-- install and run pre-commit, for QA-Checks, see steps below
-- every commit get automatically tested by Github
-- put together a release on Github - the tag should match current version-number
-- Github automatically pushes release to pypi
-
-```shell
-pip3 install pre-commit
-
-pre-commit run --all-files
-```
-
-## Open Tasks
-
-- [click progressbar](https://click.palletsprojects.com/en/8.1.x/api/#click.progressbar) -> could replace tqdm
-- implementations for this lib
-  - generalize up- and down-sampling, use out_sample_rate instead of ds-factor
-    - lib samplerate (tested) -> promising, but designed for float32 and range of +-1.0
-    - lib resampy (tested) -> could be problematic with slice-iterator
-    - https://stackoverflow.com/questions/29085268/resample-a-numpy-array
-    - scipy.signal.resample, https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.resample.html
-    - scipy.signal.decimate, https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.decimate.html
-    - scipy.signal.resample_poly, https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.resample_poly.html#scipy.signal.resample_poly
-    - timestamps could be regenerated with np.arange( tmin, tmax, 1e9/samplerate)
-  - generalize converters (currently in IVonne)
-    - isc&voc <-> ivcurve
-    - ivcurve -> ivsample
-  - plotting and downsampling for IVCurves ()
-  - plotting more generalized (power, cpu-util, ..., if IV then offer power as well)
-  - some metadata is calculated wrong (non-scalar datasets)
-  - unittests & codecoverage -> 79% with v22.5.4, https://pytest-cov.readthedocs.io/en/latest/config.html
-    - test example: https://github.com/kvas-it/pytest-console-scripts
-    - use coverage to test some edge-cases
-  - sub-divide valid() into healthy()
-  - add gain/factor to time, with repair-code
-  - add https://pypi.org/project/nessie-recorder/#files
-- main shepherd-code
-  - proper validation first
-  - update commentary
-  - pin-description should be in yaml (and other descriptions for cpu, io, ...)
-  - datatype-hint in h5-file (ivcurve, ivsample, isc_voc), add mechanism to prevent misuse
-  - hostname for emulation
-  - full and minimal config into h5
-  - use the datalib as a base
-  - isc-voc-harvesting
-  - directly process isc-voc -> resample to ivcurve?
```

### Comparing `shepherd_data-2023.3.1/setup.cfg` & `shepherd_data-2023.5.5/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -28,54 +28,56 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Natural Language :: English
 
 [options]
 packages = find:
 package_dir = 
-	=src
+	=.
 zip_safe = True
 include_package_data = True
 python_requires = >= 3.7
 install_requires = 
+	shepherd-core
 	click
 	h5py
 	matplotlib  # full-version
 	numpy
-	pandas  # full-version
+	pandas<2.0.0  # full-version
 	pyYAML
 	scipy   # full-version
 	tqdm    # full-version
 
 [options.extras_require]
 dev = 
 	black
 	pylint
 	flake8
 	twine
 	pre-commit
 	pyright
 	pandas-stubs
+	ruff
 test = 
 	pytest
 	pytest-click
 	coverage
 
 [options.entry_points]
 console_scripts = 
 	shepherd-data = shepherd_data.cli:cli
 
 [options.packages.find]
-where = src
+where = .
 
 [options.package_data]
 * = README.md
 shepherd_data = 
-	src/examples/*.py
-	src/examples/*.iv
+	examples/*.py
+	examples/*.iv
 
 [aliases]
 test = pytest
 
 [tool:pytest]
 addopts = -vvv
```

### Comparing `shepherd_data-2023.3.1/src/shepherd_data/cli.py` & `shepherd_data-2023.5.5/shepherd_data/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,35 +6,22 @@
 import sys
 from pathlib import Path
 from typing import List
 from typing import Optional
 
 import click
 
+from shepherd_core import get_verbose_level
+from shepherd_core import set_verbose_level
+
 from . import Reader
 from . import Writer
 from . import __version__
 
 logger = logging.getLogger("SHPData.cli")
-verbose_level = 2
-
-
-def config_logger(verbose: int) -> None:
-    # TODO: put in __init__, provide logger, ditch global var
-    if verbose == 0:
-        logger.setLevel(logging.ERROR)
-    elif verbose == 1:
-        logger.setLevel(logging.WARNING)
-    elif verbose == 2:
-        logger.setLevel(logging.INFO)
-    elif verbose > 2:
-        logger.setLevel(logging.DEBUG)
-    global verbose_level
-    verbose_level = verbose
-    logging.basicConfig(format="%(message)s")  # reduce internals
 
 
 def path_to_flist(data_path: Path) -> List[Path]:
     """every path gets transformed to a list of paths
     - if directory: list of files inside
     - if existing file: list with 1 element
     - or else: empty list
@@ -57,35 +44,37 @@
 @click.option(
     "-v",
     "--verbose",
     count=True,
     default=0,
     help="4 Levels [0..3](Error, Warning, Info, Debug)",
 )
+@click.option(
+    "--version",
+    is_flag=True,
+    help="Prints version-info at start (combinable with -v)",
+)
 @click.pass_context  # TODO: is the ctx-type correct?
-def cli(ctx: click.Context, verbose: int) -> None:
-    """Shepherd: Synchronized Energy Harvesting Emulator and Recorder
-
-    Args:
-        ctx:
-        verbose:
-    """
-    config_logger(verbose)
-    logger.info("Shepherd-Data v%s", __version__)
-    logger.debug("Python v%s", sys.version)
-    logger.debug("Click v%s", click.__version__)
+def cli(ctx: click.Context, verbose: int, version: bool) -> None:
+    """Shepherd: Synchronized Energy Harvesting Emulator and Recorder"""
+    set_verbose_level(verbose)
+    if version:
+        logger.info("Shepherd-Data v%s", __version__)
+        logger.debug("Python v%s", sys.version)
+        logger.debug("Click v%s", click.__version__)
     if not ctx.invoked_subcommand:
         click.echo("Please specify a valid command")
 
 
 @cli.command(short_help="Validates a file or directory containing shepherd-recordings")
 @click.argument("in_data", type=click.Path(exists=True, resolve_path=True))
 def validate(in_data: Path) -> None:
     """Validates a file or directory containing shepherd-recordings"""
     files = path_to_flist(in_data)
+    verbose_level = get_verbose_level()  # TODO: should be stored and passed in ctx
     valid_dir = True
     for file in files:
         logger.info("Validating '%s' ...", file.name)
         valid_file = True
         with Reader(file, verbose=verbose_level >= 2) as shpr:
             valid_file &= shpr.is_valid()
             valid_file &= shpr.check_timediffs()
@@ -110,14 +99,15 @@
     default=";",
     type=click.STRING,
     help="Set an individual csv-separator",
 )
 def extract(in_data: Path, ds_factor: float, separator: str) -> None:
     """Extracts recorded IVSamples and stores it to csv"""
     files = path_to_flist(in_data)
+    verbose_level = get_verbose_level()
     if not isinstance(ds_factor, (float, int)) or ds_factor < 1:
         ds_factor = 1000
         logger.info("DS-Factor was invalid was reset to 1'000")
     for file in files:
         logger.info("Extracting IV-Samples from '%s' ...", file.name)
         with Reader(file, verbose=verbose_level >= 2) as shpr:
             # will create a downsampled h5-file (if not existing) and then saving to csv
@@ -159,14 +149,15 @@
     default=";",
     type=click.STRING,
     help="Set an individual csv-separator",
 )
 def extract_meta(in_data: Path, separator: str) -> None:
     """Extracts metadata and logs from file or directory containing shepherd-recordings"""
     files = path_to_flist(in_data)
+    verbose_level = get_verbose_level()
     for file in files:
         logger.info("Extracting metadata & logs from '%s' ...", file.name)
         with Reader(file, verbose=verbose_level >= 2) as shpr:
             elements = shpr.save_metadata()
 
             if "sysutil" in elements:
                 shpr.save_csv(shpr["sysutil"], separator)
@@ -209,14 +200,15 @@
         ds_factor = int(Reader.samplerate_sps_default / sample_rate)
     if isinstance(ds_factor, (float, int)) and ds_factor >= 1:
         ds_list = [ds_factor]
     else:
         ds_list = [5, 25, 100, 500, 2_500, 10_000, 50_000, 250_000, 1_000_000]
 
     files = path_to_flist(in_data)
+    verbose_level = get_verbose_level()
     for file in files:
         with Reader(file, verbose=verbose_level >= 2) as shpr:
             for _factor in ds_list:
                 if shpr.ds_time.shape[0] / _factor < 1000:
                     logger.warning(
                         "will skip downsampling for %s because resulting sample-size is too small"
                     )
@@ -287,14 +279,15 @@
     end: Optional[float],
     width: int,
     height: int,
     multiplot: bool,
 ) -> None:
     """Plots IV-trace from file or directory containing shepherd-recordings"""
     files = path_to_flist(in_data)
+    verbose_level = get_verbose_level()
     multiplot = multiplot and len(files) > 1
     data = []
     for file in files:
         logger.info("Generating plot for '%s' ...", file.name)
         with Reader(file, verbose=verbose_level >= 2) as shpr:
             if multiplot:
                 data.append(shpr.generate_plot_data(start, end, relative_ts=True))
```

### Comparing `shepherd_data-2023.3.1/src/shepherd_data/ivonne.py` & `shepherd_data-2023.5.5/shepherd_data/ivonne.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.3.1/src/shepherd_data/mppt.py` & `shepherd_data-2023.5.5/shepherd_data/mppt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Harvesters, simple and fast approach.
 Might be exchanged by shepherds py-model of pru-harvesters
 """
 import numpy as np
 import pandas as pd
 
-from .calibration import T_calc
+from shepherd_core.calibration import T_calc
 
 
 def iv_model(voltages: T_calc, coeffs: pd.Series) -> T_calc:
     """Simple diode based model of a solar panel IV curve.
 
     Args:
         :param voltages: Load voltage of the solar panel
```

### Comparing `shepherd_data-2023.3.1/src/shepherd_data/reader.py` & `shepherd_data-2023.5.5/shepherd_data/reader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,239 +1,49 @@
 """
 Reader-Baseclass
 """
 import contextlib
-import errno
-import logging
 import math
-import os
 from datetime import datetime
-from itertools import product
 from pathlib import Path
 from typing import Dict
-from typing import Generator
 from typing import List
 from typing import Optional
 from typing import Union
 
 import h5py
 import numpy as np
 import pandas as pd
 import yaml
 from matplotlib import pyplot as plt
 from scipy import signal
 from tqdm import trange
 
-from .calibration import raw_to_si
+from shepherd_core import BaseReader
+from shepherd_core import raw_to_si
 
 # import samplerate  # TODO: just a test-fn for now
 
 
-class Reader:
+class Reader(BaseReader):
     """Sequentially Reads shepherd-data from HDF5 file.
 
     Args:
         file_path: Path of hdf5 file containing shepherd data with iv-samples, iv-curves or isc&voc
         verbose: more info during usage, 'None' skips the setter
     """
 
-    samples_per_buffer: int = 10_000
-    samplerate_sps_default: int = 100_000
-
-    mode_dtype_dict = {
-        "harvester": ["ivsample", "ivcurve", "isc_voc"],
-        "emulator": ["ivsample"],
-    }
-
     def __init__(self, file_path: Optional[Path], verbose: Optional[bool] = True):
-        if not hasattr(self, "_file_path"):
-            self._file_path: Optional[Path] = None
-            if isinstance(file_path, (Path, str)):
-                self._file_path = Path(file_path)
-
-        if not hasattr(self, "_logger"):
-            self._logger: logging.Logger = logging.getLogger("SHPData.Reader")
-        if verbose is not None:
-            self._logger.setLevel(logging.INFO if verbose else logging.WARNING)
-
-        self.samplerate_sps: int = 100_000
-        self.sample_interval_ns: int = int(10**9 // self.samplerate_sps)
-        self.sample_interval_s: float = 1 / self.samplerate_sps
-
-        self.max_elements: int = (
-            40 * self.samplerate_sps
-        )  # per iteration (40s full res, < 200 MB RAM use)
-
-        # init stats
-        self.runtime_s: float = 0
-        self.file_size: int = 0
-        self.data_rate: float = 0
-
-        # open file (if not already done by writer)
-        if not hasattr(self, "h5file"):
-            if not isinstance(self._file_path, Path):
-                raise ValueError("Provide a valid Path-Object to Reader!")
-            if not self._file_path.exists():
-                raise FileNotFoundError(
-                    errno.ENOENT, os.strerror(errno.ENOENT), self._file_path.name
-                )
-
-            self.h5file = h5py.File(self._file_path, "r")  # = readonly
-
-            if self.is_valid():
-                self._logger.info("File is available now")
-            else:
-                self._logger.error(
-                    "File is faulty! Will try to open but there might be dragons"
-                )
-
-        if not isinstance(self.h5file, h5py.File):
-            raise TypeError("Type of opened file is not h5py.File")
-
-        self.ds_time: h5py.Dataset = self.h5file["data"]["time"]
-        self.ds_voltage: h5py.Dataset = self.h5file["data"]["voltage"]
-        self.ds_current: h5py.Dataset = self.h5file["data"]["current"]
-
-        if not hasattr(self, "_cal"):
-            self._cal: Dict[str, Dict[str, float]] = {
-                "voltage": {
-                    "gain": self.ds_voltage.attrs["gain"],
-                    "offset": self.ds_voltage.attrs["offset"],
-                },
-                "current": {
-                    "gain": self.ds_current.attrs["gain"],
-                    "offset": self.ds_current.attrs["offset"],
-                },
-            }
-
-        self._refresh_file_stats()
-
-        if file_path is not None:
-            # file opened by this reader
-            self._logger.info(
-                "Reading data from '%s'\n"
-                "\t- runtime %s s\n"
-                "\t- mode = %s\n"
-                "\t- window_size = %s\n"
-                "\t- size = %s MiB\n"
-                "\t- rate = %s KiB/s",
-                self._file_path,
-                self.runtime_s,
-                self.get_mode(),
-                self.get_window_samples(),
-                round(self.file_size / 2**20),
-                round(self.data_rate / 2**10),
-            )
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, *exc):  # type: ignore
-        if isinstance(self._file_path, Path):
-            self.h5file.close()
+        super().__init__(file_path, verbose)
 
     def __repr__(self):
         return yaml.safe_dump(
             self.get_metadata(minimal=True), default_flow_style=False, sort_keys=False
         )
 
-    def _refresh_file_stats(self) -> None:
-        """update internal states, helpful after resampling or other changes in data-group"""
-        self.h5file.flush()
-        if self.ds_time.shape[0] > 1:
-            self.sample_interval_ns = int(self.ds_time[1] - self.ds_time[0])
-            self.samplerate_sps = max(int(10**9 // self.sample_interval_ns), 1)
-            self.sample_interval_s = 1.0 / self.samplerate_sps
-        self.runtime_s = round(self.ds_time.shape[0] / self.samplerate_sps, 1)
-        if isinstance(self._file_path, Path):
-            self.file_size = self._file_path.stat().st_size
-        else:
-            self.file_size = 0
-        self.data_rate = self.file_size / self.runtime_s if self.runtime_s > 0 else 0
-
-    def read_buffers(
-        self, start_n: int = 0, end_n: Optional[int] = None, is_raw: bool = False
-    ) -> Generator[tuple, None, None]:
-        """Generator that reads the specified range of buffers from the hdf5 file.
-        can be configured on first call
-
-        Args:
-            :param start_n: (int) Index of first buffer to be read
-            :param end_n: (int) Index of last buffer to be read
-            :param is_raw: (bool) output original data, not transformed to SI-Units
-        Yields:
-            Buffers between start and end (tuple with time, voltage, current)
-        """
-        if end_n is None:
-            end_n = int(self.ds_time.shape[0] // self.samples_per_buffer)
-        self._logger.debug(
-            "Reading blocks from %s to %s from source-file", start_n, end_n
-        )
-        _raw = is_raw
-
-        for i in range(start_n, end_n):
-            idx_start = i * self.samples_per_buffer
-            idx_end = idx_start + self.samples_per_buffer
-            if _raw:
-                yield (
-                    self.ds_time[idx_start:idx_end],
-                    self.ds_voltage[idx_start:idx_end],
-                    self.ds_current[idx_start:idx_end],
-                )
-            else:
-                yield (
-                    self.ds_time[idx_start:idx_end] * 1e-9,
-                    raw_to_si(self.ds_voltage[idx_start:idx_end], self._cal["voltage"]),
-                    raw_to_si(self.ds_current[idx_start:idx_end], self._cal["current"]),
-                )
-
-    def get_calibration_data(self) -> dict:
-        """Reads calibration-data from hdf5 file.
-
-        :return: Calibration data as CalibrationData object
-        """
-        return self._cal
-
-    def get_window_samples(self) -> int:
-        """
-        :return:
-        """
-        if "window_samples" in self.h5file["data"].attrs:
-            return int(self.h5file["data"].attrs["window_samples"])
-        return 0
-
-    def get_mode(self) -> str:
-        if "mode" in self.h5file.attrs:
-            return self.h5file.attrs["mode"]
-        return ""
-
-    def get_config(self) -> Dict:
-        if "config" in self.h5file["data"].attrs:
-            return yaml.safe_load(self.h5file["data"].attrs["config"])
-        return {}
-
-    def get_hostname(self) -> str:
-        if "hostname" in self.h5file.attrs:
-            return self.h5file.attrs["hostname"]
-        return "unknown"
-
-    def get_datatype(self) -> str:
-        if "datatype" in self.h5file["data"].attrs:
-            return self.h5file["data"].attrs["datatype"]
-        return ""
-
-    def get_hrv_config(self) -> dict:
-        """essential info for harvester
-        :return: config-dict directly for vHarvester to be used during emulation
-        """
-        return {
-            "dtype": self.get_datatype(),
-            "window_samples": self.get_window_samples(),
-        }
-
     def data_timediffs(self) -> List[float]:
         """calculate list of (unique) time-deltas between buffers [s]
             -> optimized version that only looks at the start of each buffer
 
         :return: list of (unique) time-deltas between buffers [s]
         """
         iterations = math.ceil(self.ds_time.shape[0] / self.max_elements)
@@ -270,103 +80,14 @@
         diffs = self.data_timediffs()
         if len(diffs) > 1:
             self._logger.warning(
                 "Time-jumps detected -> expected equal steps, but got: %s s", diffs
             )
         return len(diffs) <= 1
 
-    def is_valid(self) -> bool:
-        """checks file for plausibility
-
-        :return: state of validity
-        """
-        # hard criteria
-        if "data" not in self.h5file.keys():
-            self._logger.error("root data-group not found (@Validator)")
-            return False
-        for attr in ["mode"]:
-            if attr not in self.h5file.attrs.keys():
-                self._logger.error(
-                    "attribute '%s' not found in file (@Validator)", attr
-                )
-                return False
-            if self.h5file.attrs["mode"] not in self.mode_dtype_dict:
-                self._logger.error("unsupported mode '%s' (@Validator)", attr)
-                return False
-        for attr in ["window_samples", "datatype"]:
-            if attr not in self.h5file["data"].attrs.keys():
-                self._logger.error(
-                    "attribute '%s' not found in data-group (@Validator)", attr
-                )
-                return False
-        for dset in ["time", "current", "voltage"]:
-            if dset not in self.h5file["data"].keys():
-                self._logger.error("dataset '%s' not found (@Validator)", dset)
-                return False
-        for dset, attr in product(["current", "voltage"], ["gain", "offset"]):
-            if attr not in self.h5file["data"][dset].attrs.keys():
-                self._logger.error(
-                    "attribute '%s' not found in dataset '%s' (@Validator)", attr, dset
-                )
-                return False
-        if self.get_datatype() not in self.mode_dtype_dict[self.get_mode()]:
-            self._logger.error(
-                "unsupported type '%s' for mode '%s' (@Validator)",
-                self.get_datatype(),
-                self.get_mode(),
-            )
-            return False
-
-        if self.get_datatype() == "ivcurve" and self.get_window_samples() < 1:
-            self._logger.error(
-                "window size / samples is < 1 -> invalid for ivcurves-datatype (@Validator)"
-            )
-            return False
-
-        # soft-criteria:
-        if self.get_datatype() != "ivcurve" and self.get_window_samples() > 0:
-            self._logger.warning(
-                "window size / samples is > 0 despite not using the ivcurves-datatype (@Validator)"
-            )
-        # same length of datasets:
-        ds_time_size = self.h5file["data"]["time"].shape[0]
-        for dset in ["current", "voltage"]:
-            ds_size = self.h5file["data"][dset].shape[0]
-            if ds_time_size != ds_size:
-                self._logger.warning(
-                    "dataset '%s' has different size (=%s), "
-                    "compared to time-ds (=%s) (@Validator)",
-                    dset,
-                    ds_size,
-                    ds_time_size,
-                )
-        # dataset-length should be multiple of buffersize
-        remaining_size = ds_time_size % self.samples_per_buffer
-        if remaining_size != 0:
-            self._logger.warning(
-                "datasets are not aligned with buffer-size (@Validator)"
-            )
-        # check compression
-        for dset in ["time", "current", "voltage"]:
-            comp = self.h5file["data"][dset].compression
-            opts = self.h5file["data"][dset].compression_opts
-            if comp not in [None, "gzip", "lzf"]:
-                self._logger.warning(
-                    "unsupported compression found (%s != None, lzf, gzip) (@Validator)",
-                    comp,
-                )
-            if (comp == "gzip") and (opts is not None) and (int(opts) > 1):
-                self._logger.warning(
-                    "gzip compression is too high (%s > 1) for BBone (@Validator)", opts
-                )
-        # host-name
-        if self.get_hostname() == "unknown":
-            self._logger.warning("Hostname was not set (@Validator)")
-        return True
-
     def get_metadata(
         self, node: Union[h5py.Dataset, h5py.Group, None] = None, minimal: bool = False
     ) -> Dict[str, dict]:
         """recursive FN to capture the structure of the file
 
         :param node: starting node, leave free to go through whole file
         :param minimal: just provide a bare tree (much faster)
@@ -433,26 +154,14 @@
             )  # {"h5root": self.get_metadata(self.h5file)}
             with open(yml_path, "w", encoding="utf-8-sig") as yfd:
                 yaml.safe_dump(metadata, yfd, default_flow_style=False, sort_keys=False)
         else:
             metadata = {}
         return metadata
 
-    def __getitem__(self, key: str):
-        """returns attribute or (if none found) a handle for a group or dataset (if found)
-
-        :param key: attribute, group, dataset
-        :return: value of that key, or handle of object
-        """
-        if key in self.h5file.attrs:
-            return self.h5file.attrs.__getitem__(key)
-        if key in self.h5file:
-            return self.h5file.__getitem__(key)
-        raise KeyError
-
     def energy(self) -> float:
         """determine the recorded energy of the trace
         # multiprocessing: https://stackoverflow.com/a/71898911
         # -> failed with multiprocessing.pool and pathos.multiprocessing.ProcessPool
 
         :return: sampled energy in Ws (watt-seconds)
         """
```

### Comparing `shepherd_data-2023.3.1/tests/test_cli_downsample.py` & `shepherd_data-2023.5.5/tests/test_cli_downsample.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.3.1/tests/test_cli_extract.py` & `shepherd_data-2023.5.5/tests/test_cli_extract.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.3.1/tests/test_cli_plot.py` & `shepherd_data-2023.5.5/tests/test_cli_plot.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.3.1/tests/test_ivonne.py` & `shepherd_data-2023.5.5/tests/test_ivonne.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from shepherd_data import ivonne
 from shepherd_data import mppt
 
 
 @pytest.fixture
 def example_path() -> Path:
     here = Path(__file__).absolute().parent
-    return here.parent / "src" / "examples"
+    return here.parent / "examples"
 
 
 def test_convert_ivonne(tmp_path: Path, example_path: Path) -> None:
     input_file = "jogging_10m"
     inp_path = example_path / (input_file + ".iv")
     isc_path = tmp_path / (input_file + "_isc.h5")
     ivc_path = tmp_path / (input_file + "_ivc.h5")
```

### Comparing `shepherd_data-2023.3.1/tests/test_reader.py` & `shepherd_data-2023.5.5/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.3.1/tests/test_writer.py` & `shepherd_data-2023.5.5/tests/test_writer.py`

 * *Files identical despite different names*

