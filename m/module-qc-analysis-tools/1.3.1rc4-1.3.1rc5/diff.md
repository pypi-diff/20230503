# Comparing `tmp/module_qc_analysis_tools-1.3.1rc4.tar.gz` & `tmp/module_qc_analysis_tools-1.3.1rc5.tar.gz`

## Comparing `module_qc_analysis_tools-1.3.1rc4.tar` & `module_qc_analysis_tools-1.3.1rc5.tar`

### file list

```diff
@@ -1,40 +1,42 @@
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/.flake8
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/.gitmodules
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/tbump.toml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/__init__.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/_version.py
--rw-r--r--   0        0        0    10062 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py
--rw-r--r--   0        0        0    18774 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py
--rw-r--r--   0        0        0    12036 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py
--rw-r--r--   0        0        0     9548 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/IV_MEASURE.py
--rw-r--r--   0        0        0     3800 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py
--rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py
--rw-r--r--   0        0        0     8710 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py
--rw-r--r--   0        0        0    24858 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/SLDO.py
--rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/TUNING.py
--rw-r--r--   0        0        0    12915 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py
--rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/__init__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/__main__.py
--rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/globals.py
--rwxr-xr-x   0        0        0     8167 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/load_yarr_scans.py
--rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/main.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/overwrite_config.py
--rw-r--r--   0        0        0     8646 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/update_chip_config.py
--rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/data/analysis_cuts.json
--rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/data/pixel_classification.json
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/data/schema/info_schema.json
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/data/schema/input_yarr_schema.json
--rw-r--r--   0        0        0    25523 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/utils/analysis.py
--rw-r--r--   0        0        0    12471 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/utils/classification.py
--rw-r--r--   0        0        0    34039 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/utils/misc.py
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/tests/test_cli.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/tests/test_package.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/LICENSE
--rw-r--r--   0        0        0    21574 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/README.md
--rw-r--r--   0        0        0     4542 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/pyproject.toml
--rw-r--r--   0        0        0    23698 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/PKG-INFO
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/.flake8
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/.gitmodules
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/tbump.toml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/__init__.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/_version.py
+-rw-r--r--   0        0        0    10062 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py
+-rw-r--r--   0        0        0    18774 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py
+-rw-r--r--   0        0        0    12036 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py
+-rw-r--r--   0        0        0     9548 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/IV_MEASURE.py
+-rw-r--r--   0        0        0     9387 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/LP_MODE.py
+-rw-r--r--   0        0        0     3800 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py
+-rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py
+-rw-r--r--   0        0        0     8981 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/OVERVOLTAGE_PROTECTION.py
+-rw-r--r--   0        0        0     9342 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py
+-rw-r--r--   0        0        0    24858 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/SLDO.py
+-rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/TUNING.py
+-rw-r--r--   0        0        0    12915 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py
+-rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/__init__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/__main__.py
+-rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/globals.py
+-rwxr-xr-x   0        0        0     8167 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/load_yarr_scans.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/main.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/overwrite_config.py
+-rw-r--r--   0        0        0     8646 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/update_chip_config.py
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/data/analysis_cuts.json
+-rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/data/pixel_classification.json
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/data/schema/info_schema.json
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/data/schema/input_yarr_schema.json
+-rw-r--r--   0        0        0    25563 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/utils/analysis.py
+-rw-r--r--   0        0        0    14347 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/utils/classification.py
+-rw-r--r--   0        0        0    34961 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/utils/misc.py
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/tests/test_cli.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/tests/test_package.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/LICENSE
+-rw-r--r--   0        0        0    21574 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/README.md
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/pyproject.toml
+-rw-r--r--   0        0        0    23698 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/PKG-INFO
```

### Comparing `module_qc_analysis_tools-1.3.1rc4/.gitlab-ci.yml` & `module_qc_analysis_tools-1.3.1rc5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc4/.pre-commit-config.yaml` & `module_qc_analysis_tools-1.3.1rc5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc4/tbump.toml` & `module_qc_analysis_tools-1.3.1rc5/tbump.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2231 2e33 2e31 7263 3422 0a0a  t = "1.3.1rc4"..
+00000010: 7420 3d20 2231 2e33 2e31 7263 3522 0a0a  t = "1.3.1rc5"..
 00000020: 2320 4578 616d 706c 6520 6f66 2061 2073  # Example of a s
 00000030: 656d 7665 7220 7265 6765 7870 2e0a 2320  emver regexp..# 
 00000040: 4d61 6b65 2073 7572 6520 7468 6973 206d  Make sure this m
 00000050: 6174 6368 6573 2063 7572 7265 6e74 5f76  atches current_v
 00000060: 6572 7369 6f6e 2062 6566 6f72 650a 2320  ersion before.# 
 00000070: 7573 696e 6720 7462 756d 700a 7265 6765  using tbump.rege
 00000080: 7820 3d20 2727 270a 2020 283f 503c 6d61  x = '''.  (?P<ma
@@ -15,15 +15,15 @@
 000000e0: 290a 2020 293f 0a20 2027 2727 0a0a 5b67  ).  )?.  '''..[g
 000000f0: 6974 5d0a 2320 5468 6520 6375 7272 656e  it].# The curren
 00000100: 7420 7665 7273 696f 6e20 7769 6c6c 2067  t version will g
 00000110: 6574 2075 7064 6174 6564 2077 6865 6e20  et updated when 
 00000120: 7462 756d 7020 6973 2072 756e 0a6d 6573  tbump is run.mes
 00000130: 7361 6765 5f74 656d 706c 6174 6520 3d20  sage_template = 
 00000140: 2242 756d 7020 7665 7273 696f 6e3a 2031  "Bump version: 1
-00000150: 2e33 2e31 7263 3420 e286 9220 7b6e 6577  .3.1rc4 ... {new
+00000150: 2e33 2e31 7263 3520 e286 9220 7b6e 6577  .3.1rc5 ... {new
 00000160: 5f76 6572 7369 6f6e 7d22 0a74 6167 5f74  _version}".tag_t
 00000170: 656d 706c 6174 6520 3d20 2276 7b6e 6577  emplate = "v{new
 00000180: 5f76 6572 7369 6f6e 7d22 0a0a 2320 466f  _version}"..# Fo
 00000190: 7220 6561 6368 2066 696c 6520 746f 2070  r each file to p
 000001a0: 6174 6368 2c20 6164 6420 6120 5b5b 6669  atch, add a [[fi
 000001b0: 6c65 5d5d 2063 6f6e 6669 670a 2320 7365  le]] config.# se
 000001c0: 6374 696f 6e20 636f 6e74 6169 6e69 6e67  ction containing
```

### Comparing `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py` & `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py` & `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py` & `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/IV_MEASURE.py` & `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/IV_MEASURE.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py` & `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py` & `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py` & `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py`

 * *Files 9% similar despite different names*

```diff
@@ -229,14 +229,24 @@
                 + f"{passes_qc}"
                 + bcolors.ENDC
             )
         log.info("")
         log.removeHandler(chiplog)
         chiplog.close()
 
+        # Add placeholders for future selection here
+        data.add_parameter("PIXEL_FAILURE_MERGED_BUMPS", -1)
+        data.add_parameter("PIXEL_FAILURE_SOURCE_SCAN_DONE", False)
+        data.add_parameter("PIXEL_FAILURE_DISCONNECTED_BUMPS_SOURCE_SCAN", -1)
+        data.add_parameter("PIXEL_FAILURE_BAD_PIXELS_ZERO_BIAS_SCAN", -1)
+        data.add_parameter("PIXEL_FAILURE_DISCONNECTED_BUMPS_ZERO_BIAS_SCAN", -1)
+        data.add_parameter("PIXEL_FAILURE_BAD_PIXELS_DISCONNECTED_BUMPS_SCAN", -1)
+        data.add_parameter("PIXEL_FAILURE_DISCONNECTED_PIXELS", -1)
+        data.add_parameter("PIXEL_FAILURE_FAILING_PIXELS", -1)
+
         outputDF.set_results(data)
         outputDF.set_pass_flag(passes_qc)
 
         if permodule:
             alloutput += [outputDF.to_dict(True)]
         else:
             outfile = output_dir.joinpath(f"{chipName}.json")
```

### Comparing `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/SLDO.py` & `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/SLDO.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/TUNING.py` & `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/TUNING.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py` & `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py` & `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/globals.py` & `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/globals.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/load_yarr_scans.py` & `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/load_yarr_scans.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/main.py` & `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,20 @@
 from module_qc_analysis_tools.cli.ANALOG_READBACK import main as analog_readback
 from module_qc_analysis_tools.cli.globals import CONTEXT_SETTINGS
 from module_qc_analysis_tools.cli.INJECTION_CAPACITANCE import (
     main as injection_capacitance,
 )
 from module_qc_analysis_tools.cli.IV_MEASURE import main as iv_measure
 from module_qc_analysis_tools.cli.load_yarr_scans import main as load_yarr_scans
+from module_qc_analysis_tools.cli.LP_MODE import main as lp_mode
 from module_qc_analysis_tools.cli.MASS_MEASUREMENT import main as mass
 from module_qc_analysis_tools.cli.MIN_HEALTH_TEST import main as min_health_test
+from module_qc_analysis_tools.cli.OVERVOLTAGE_PROTECTION import (
+    main as overvoltage_protection,
+)
 from module_qc_analysis_tools.cli.overwrite_config import main as overwrite_config
 from module_qc_analysis_tools.cli.PIXEL_FAILURE_ANALYSIS import (
     main as pixel_failure_analysis,
 )
 from module_qc_analysis_tools.cli.SLDO import main as sldo
 from module_qc_analysis_tools.cli.TUNING import main as tuning
 from module_qc_analysis_tools.cli.update_chip_config import main as update_chip_config
@@ -53,14 +57,16 @@
 
 
 app_analysis.command("adc-calibration")(adc_calibration)
 app_analysis.command("analog-readback")(analog_readback)
 app_analysis.command("injection-capacitance")(injection_capacitance)
 app_analysis.command("sldo")(sldo)
 app_analysis.command("vcal-calibration")(vcal_calibration)
+app_analysis.command("overvoltage-protection")(overvoltage_protection)
+app_analysis.command("lp-mode")(lp_mode)
 app_analysis.command("mass-measurement")(mass)
 app_analysis.command("iv-measure")(iv_measure)
 app_analysis.command("visual-inspection")(visual_inspection)
 app_config.command("overwrite")(overwrite_config)
 app_config.command("update")(update_chip_config)
 app_config.command("load-yarr-scans")(load_yarr_scans)
 app_config.command("min-health-test")(min_health_test)
```

### Comparing `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/overwrite_config.py` & `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/overwrite_config.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/update_chip_config.py` & `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/update_chip_config.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/data/analysis_cuts.json` & `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/data/analysis_cuts.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'LP_MODE'": "OrderedDict([('LP_VINA', OrderedDict([('LZero', [1.468, 1.518]), ('LOne', [1.468, "*

 * *              "1.518]), ('LTwo', [1.468, 1.518])])), ('LP_VIND', OrderedDict([('LZero', [1.468, "*

 * *              "1.518]), ('LOne', [1.468, 1.518]), ('LTwo', [1.468, 1.518])])), ('LP_VOFFS', "*

 * *              "OrderedDict([('LZero', [1.304, 1.354]), ('LOne', [1.304, 1.354]), ('LTwo', [1.304, "*

 * *              "1.354])])), ('LP_IINA', [0.18, 0.22]), ('LP_IIND', [0.28, 0.32]), ('LP_ISHUNTA', "*

 * *              "[0.0001, […]*

```diff
@@ -167,14 +167,74 @@
     },
     "INJECTION_CAPACITANCE": {
         "INJ_CAPACITANCE": [
             6.74,
             9.0
         ]
     },
+    "LP_MODE": {
+        "LP_IINA": [
+            0.18,
+            0.22
+        ],
+        "LP_IIND": [
+            0.28,
+            0.32
+        ],
+        "LP_ISHUNTA": [
+            0.0001,
+            0.1
+        ],
+        "LP_ISHUNTD": [
+            0.0001,
+            0.1
+        ],
+        "LP_VINA": {
+            "LOne": [
+                1.468,
+                1.518
+            ],
+            "LTwo": [
+                1.468,
+                1.518
+            ],
+            "LZero": [
+                1.468,
+                1.518
+            ]
+        },
+        "LP_VIND": {
+            "LOne": [
+                1.468,
+                1.518
+            ],
+            "LTwo": [
+                1.468,
+                1.518
+            ],
+            "LZero": [
+                1.468,
+                1.518
+            ]
+        },
+        "LP_VOFFS": {
+            "LOne": [
+                1.304,
+                1.354
+            ],
+            "LTwo": [
+                1.304,
+                1.354
+            ],
+            "LZero": [
+                1.304,
+                1.354
+            ]
+        }
+    },
     "MASS_MEASUREMENT": {},
     "MIN_HEALTH_TEST": {
         "BAD_ANALOG_INTEGRATED": [
             0,
             153.6
         ],
         "HIGH_ENC_INDEPENDENT": [
@@ -182,14 +242,76 @@
             1536
         ],
         "THRESHOLD_FAILED_FITS_INDEPENDENT": [
             0,
             1536
         ]
     },
+    "OVERVOLTAGE_PROTECTION": {
+        "OVP_IINA": {
+            "LOne": [
+                0.681,
+                0.735
+            ],
+            "LTwo": [
+                0.567,
+                0.626
+            ],
+            "LZero": [
+                0.788,
+                0.85
+            ]
+        },
+        "OVP_IIND": {
+            "LOne": [
+                0.917,
+                0.971
+            ],
+            "LTwo": [
+                0.846,
+                0.905
+            ],
+            "LZero": [
+                1.177,
+                1.24
+            ]
+        },
+        "OVP_VINA": {
+            "LOne": [
+                1.469,
+                1.519
+            ],
+            "LTwo": [
+                1.468,
+                1.518
+            ],
+            "LZero": [
+                1.473,
+                1.523
+            ]
+        },
+        "OVP_VIND": {
+            "LOne": [
+                1.469,
+                1.519
+            ],
+            "LTwo": [
+                1.468,
+                1.518
+            ],
+            "LZero": [
+                1.473,
+                1.523
+            ]
+        },
+        "OVP_VREFOVP": [
+            1.95,
+            2.05
+        ]
+    },
     "PIXEL_FAILURE_ANALYSIS": {
         "ELECTRICALLY_FAILED": [
             0,
             153.6
         ]
     },
     "SLDO": {
```

### Comparing `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/data/pixel_classification.json` & `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/data/pixel_classification.json`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/data/schema/info_schema.json` & `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/data/schema/info_schema.json`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json` & `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/utils/analysis.py` & `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/utils/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 import logging
 import sys
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 import numpy as np
 
-from module_qc_analysis_tools.utils.misc import bcolors, getImuxMap, getVmuxMap
+from module_qc_analysis_tools.utils.misc import (
+    bcolors,
+    getImuxMap,
+    getVmuxMap,
+    prettyprint,
+)
 
 log = logging.getLogger("analysis")
 
 
 def format_text():
     return " {:^30}: {:^20}: {:^20}: {:^5}"
 
@@ -23,29 +28,29 @@
 
 def print_output_pass(key, results, lower_bound, upper_bound):
     txt = format_text()
     log.info(
         bcolors.OKGREEN
         + txt.format(
             key,
-            round(results, 4),
+            prettyprint(results),
             f"[{lower_bound}, {upper_bound}]",
             "PASS",
         )
         + bcolors.ENDC
     )
 
 
 def print_output_fail(key, results, lower_bound, upper_bound):
     txt = format_text()
     log.info(
         bcolors.BADRED
         + txt.format(
             key,
-            round(results, 4),
+            prettyprint(results),
             f"[{lower_bound}, {upper_bound}]",
             "FAIL",
         )
         + bcolors.ENDC
     )
```

### Comparing `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/utils/classification.py` & `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/utils/classification.py`

 * *Files 8% similar despite different names*

```diff
@@ -335,45 +335,99 @@
     return pix_fail, record
 
 
 def print_pixel_classification(failure_summary, test_type, outputdir, chipname):
     txt = format_text_short()
     log.info(txt.format("Classification", "Number of pixels"))
     log.info("------------------------------------------------------------------")
-    counts = []
+    counts_dep = []
+    counts_indep = []
     binlabels = []
     for criteria, failures in failure_summary.items():
         log.info(txt.format(criteria, failures.get("dependent")))
-        counts += [failures.get("dependent")]
+        counts_dep += [failures.get("dependent")]
+        counts_indep += [failures.get("independent")]
         binlabels += [criteria.replace("_", "\n")]
     log.info("------------------------------------------------------------------")
     log.info(
         txt.format(
             "TOTAL FAILING", list(failure_summary.values())[-1].get("integrated")
         )
     )
-    counts += [list(failure_summary.values())[-1].get("integrated")]
+    counts_dep += [list(failure_summary.values())[-1].get("integrated")]
+    counts_indep += [list(failure_summary.values())[-1].get("integrated")]
     binlabels += ["TOTAL\nFAILING"]
+    bins = range(len(counts_dep) + 1)
     log.info("------------------------------------------------------------------")
 
     # Turn off matplotlib DEBUG messages
     plt.set_loglevel(level="warning")
 
+    # Plot dependent categorization
     fig, ax = plt.subplots()
     ax.set_title(f"{chipname} ({test_type})")
-    plt.stairs(counts, range(len(counts) + 1), fill=True, color="cornflowerblue")
-    ax.set_ylim(0, max(counts) + max(counts) / 10)
+    ax.set_ylim(0, max(counts_dep) + max(counts_dep) / 2)
+    plt.stairs(counts_dep[:-1], bins[:-1], fill=True, color="cornflowerblue")
+    plt.stairs([counts_dep[-1]], bins[-2:], fill=True, color="lightcoral")
 
     # Label bins
-    plt.xticks([x + 0.5 for x in range(len(counts))], labels=binlabels, rotation=0)
+    plt.xticks([x + 0.5 for x in range(len(counts_dep))], labels=binlabels, rotation=0)
     ax.set_ylabel("Number of pixels")
+    plt.text(0.02, 0.92, "Dependent categorization", transform=ax.transAxes)
+    plt.text(
+        0.02,
+        0.85,
+        "(Failing pixels included in single category)",
+        transform=ax.transAxes,
+    )
+
+    # Print bin contents
+    for i in range(0, len(counts_dep)):
+        if counts_dep[i] > 0:
+            plt.text(
+                i + 0.5,
+                counts_dep[i] + max(counts_dep) / 60,
+                counts_dep[i],
+                ha="center",
+            )
+
+    fig.tight_layout()
+    plt.subplots_adjust(bottom=0.3)
+    plt.savefig(outputdir.joinpath(f"{chipname}_depclassification.png"))
+    log.info("Saving " + str(outputdir.joinpath(f"{chipname}_depclassification.png")))
+    plt.close()
+
+    # Plot independent categorization
+    fig, ax = plt.subplots()
+    ax.set_title(f"{chipname} ({test_type})")
+    ax.set_ylim(0, max(counts_indep) + max(counts_indep) / 2)
+    plt.stairs(counts_indep[:-1], bins[:-1], fill=True, color="mediumseagreen")
+    plt.stairs([counts_indep[-1]], bins[-2:], fill=True, color="lightcoral")
+
+    # Label bins
+    plt.xticks(
+        [x + 0.5 for x in range(len(counts_indep))], labels=binlabels, rotation=0
+    )
+    ax.set_ylabel("Number of pixels")
+    plt.text(0.02, 0.92, "Independent categorization", transform=ax.transAxes)
+    plt.text(
+        0.02,
+        0.85,
+        "(Failing pixels can be included in several categories)",
+        transform=ax.transAxes,
+    )
 
     # Print bin contents
-    for i in range(0, len(counts)):
-        if counts[i] > 0:
-            plt.text(i + 0.5, counts[i] + max(counts) / 60, counts[i], ha="center")
+    for i in range(0, len(counts_indep)):
+        if counts_indep[i] > 0:
+            plt.text(
+                i + 0.5,
+                counts_indep[i] + max(counts_indep) / 60,
+                counts_indep[i],
+                ha="center",
+            )
 
     fig.tight_layout()
     plt.subplots_adjust(bottom=0.3)
-    plt.savefig(outputdir.joinpath(f"{chipname}_classification.png"))
-    log.info("Saving " + str(outputdir.joinpath(f"{chipname}_classification.png")))
+    plt.savefig(outputdir.joinpath(f"{chipname}_indepclassification.png"))
+    log.info("Saving " + str(outputdir.joinpath(f"{chipname}_indepclassification.png")))
     plt.close()
```

### Comparing `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/utils/misc.py` & `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,14 +208,41 @@
                     "required_keys": [
                         "Vmux34",
                         "Vmux38",
                         "Vmux30",
                     ],
                 },
             },
+            "OVERVOLTAGE_PROTECTION": {
+                "required_keys": [
+                    "Temperature",
+                    "Current",
+                    "Vmux30",
+                    "Vmux32",
+                    "Imux28",
+                    "Imux30",
+                    "Imux63",
+                ],
+            },
+            "LP_MODE": {
+                "required_keys": [
+                    "Temperature",
+                    "Current",
+                    "Vmux30",
+                    "Vmux33",
+                    "Vmux36",
+                    "Vmux37",
+                    "Imux0",
+                    "Imux28",
+                    "Imux29",
+                    "Imux30",
+                    "Imux31",
+                    "Imux63",
+                ]
+            },
         }
 
     def check_testtype(self):
         if self.inputdataframe._subtestType != "":
             self.sub_test_type = self.inputdataframe._subtestType
             required_testtype = self.qc_type
             self.required_keywords = self.dict_map[self.qc_type][self.sub_test_type][
@@ -1140,7 +1167,13 @@
             _v = lookup(v, search_key, stack)
             if _v is not None:
                 if stack is not None:
                     stack.append(k)
                 return _v
 
     return None
+
+
+def prettyprint(number):
+    if abs(number) > 1e5 or abs(number) < 1e-3:
+        return f"{number:.2e}"
+    return str(round(number, 4))
```

### Comparing `module_qc_analysis_tools-1.3.1rc4/tests/test_cli.py` & `module_qc_analysis_tools-1.3.1rc5/tests/test_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -112,7 +112,47 @@
         catch_exceptions=False,
     )
     assert result.exit_code == 0, result.stderr
     for chip_id in range(1, 5):
         assert (
             f"Chip dummy_chip{chip_id} passes QC? False" in caplog.text
         ), f"Failure for chip {chip_id}"
+
+
+def test_lp_mode(runner, base_path, caplog):
+    result = runner.invoke(
+        app,
+        args=[
+            "analysis",
+            "lp-mode",
+            "-i",
+            base_path.joinpath("LP_MODE/1000000001//"),
+            "-v",
+            "DEBUG",
+        ],
+        catch_exceptions=False,
+    )
+    assert result.exit_code == 0, result.stderr
+    for chip_id in range(1, 5):
+        assert (
+            f"Chip dummy_chip{chip_id} passes QC? False" in caplog.text
+        ), f"Failure for chip {chip_id}"
+
+
+def test_ov_protection(runner, base_path, caplog):
+    result = runner.invoke(
+        app,
+        args=[
+            "analysis",
+            "overvoltage-protection",
+            "-i",
+            base_path.joinpath("OVERVOLTAGE_PROTECTION/1000000001//"),
+            "-v",
+            "DEBUG",
+        ],
+        catch_exceptions=False,
+    )
+    assert result.exit_code == 0, result.stderr
+    for chip_id in range(1, 5):
+        assert (
+            f"Chip dummy_chip{chip_id} passes QC? False" in caplog.text
+        ), f"Failure for chip {chip_id}"
```

### Comparing `module_qc_analysis_tools-1.3.1rc4/.gitignore` & `module_qc_analysis_tools-1.3.1rc5/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc4/LICENSE` & `module_qc_analysis_tools-1.3.1rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc4/README.md` & `module_qc_analysis_tools-1.3.1rc5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# module-qc-analysis-tools v1.3.1rc4
+# module-qc-analysis-tools v1.3.1rc5
 
 A general python tool for running ITkPixV1.1 module QC test analysis. An
 overview of the steps in the module QC procedure is documented in the
 [Electrical specification and QC procedures for ITkPixV1.1 modules](https://gitlab.cern.ch/atlas-itk/pixel/module/itkpix-electrical-qc/)
 document and in
 [this spreadsheet](https://docs.google.com/spreadsheets/d/1qGzrCl4iD9362RwKlstZASbhphV_qTXPeBC-VSttfgE/edit#gid=989740987).
 The analysis scripts in this repository require input files with measurement
@@ -69,15 +69,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-analysis-tools==1.3.1rc4
+python -m pip install -U pip module-qc-analysis-tools==1.3.1rc5
 ```
 
 Note that users should use the latest python version (check python version via
 `python3 -V`). Python3.7 is the minimum requirement for developers. See
 [For Developer](#for-developer) section.
 
 ## Scripts
```

### Comparing `module_qc_analysis_tools-1.3.1rc4/pyproject.toml` & `module_qc_analysis_tools-1.3.1rc5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -37,19 +37,21 @@
 module-qc-analysis-tools = "module_qc_analysis_tools.cli:app"
 "mqat" = "module_qc_analysis_tools.cli:app"
 analysis-ADC-CALIBRATION = "module_qc_analysis_tools.cli.ADC_CALIBRATION:app"
 analysis-ANALOG-READBACK = "module_qc_analysis_tools.cli.ANALOG_READBACK:app"
 analysis-INJECTION-CAPACITANCE = "module_qc_analysis_tools.cli.INJECTION_CAPACITANCE:app"
 analysis-SLDO = "module_qc_analysis_tools.cli.SLDO:app"
 analysis-VCAL-CALIBRATION = "module_qc_analysis_tools.cli.VCAL_CALIBRATION:app"
+analysis-LP-MODE = "module_qc_analysis_tools.cli.LP_MODE:app"
 analysis-MASS-MEASUREMENT = "module_qc_analysis_tools.cli.MASS_MEASUREMENT:app"
 analysis-IV-MEASURE = "module_qc_analysis_tools.cli.IV_MEASURE:app"
 analysis-VISUAL-INSPECTION = "module_qc_analysis_tools.cli.VISUAL_INSPECTION:app"
 analysis-overwrite-config = "module_qc_analysis_tools.cli.overwrite_config:app"
 analysis-update-chip-config = "module_qc_analysis_tools.cli.update_chip_config:app"
+analysis-OVERVOLTAGE-PROTECTION = "module_qc_analysis_tools.cli.OVERVOLTAGE_PROTECTION:app"
 analysis-load-yarr-scans = "module_qc_analysis_tools.cli.load_yarr_scans:app"
 analysis-MIN-HEALTH-TEST = "module_qc_analysis_tools.cli.MIN_HEALTH_TEST:app"
 analysis-TUNING = "module_qc_analysis_tools.cli.TUNING:app"
 analysis-PIXEL-FAILURE-ANALYSIS = "module_qc_analysis_tools.cli.PIXEL_FAILURE_ANALYSIS:app"
 
 [tool.hatch.version]
 source = "vcs"
```

### Comparing `module_qc_analysis_tools-1.3.1rc4/PKG-INFO` & `module_qc_analysis_tools-1.3.1rc5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module-qc-analysis-tools
-Version: 1.3.1rc4
+Version: 1.3.1rc5
 Summary: Module qc analysis tools
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools/-/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools
 Author-email: Jay Chan <jay.chan@cern.ch>
 Maintainer-email: Giordon Stark <gstark@cern.ch>
 License: Copyright (c) 2018 The Python Packaging Authority
@@ -34,15 +34,15 @@
 Requires-Dist: importlib-resources>=1.4.0; python_version < '3.9'
 Requires-Dist: matplotlib
 Requires-Dist: module-qc-data-tools>=1.0.6
 Requires-Dist: numpy
 Requires-Dist: typer
 Description-Content-Type: text/markdown
 
-# module-qc-analysis-tools v1.3.1rc4
+# module-qc-analysis-tools v1.3.1rc5
 
 A general python tool for running ITkPixV1.1 module QC test analysis. An
 overview of the steps in the module QC procedure is documented in the
 [Electrical specification and QC procedures for ITkPixV1.1 modules](https://gitlab.cern.ch/atlas-itk/pixel/module/itkpix-electrical-qc/)
 document and in
 [this spreadsheet](https://docs.google.com/spreadsheets/d/1qGzrCl4iD9362RwKlstZASbhphV_qTXPeBC-VSttfgE/edit#gid=989740987).
 The analysis scripts in this repository require input files with measurement
@@ -109,15 +109,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-analysis-tools==1.3.1rc4
+python -m pip install -U pip module-qc-analysis-tools==1.3.1rc5
 ```
 
 Note that users should use the latest python version (check python version via
 `python3 -V`). Python3.7 is the minimum requirement for developers. See
 [For Developer](#for-developer) section.
 
 ## Scripts
```

