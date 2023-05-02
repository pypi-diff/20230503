# Comparing `tmp/credoai-connect-0.1.1.tar.gz` & `tmp/credoai-connect-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "credoai-connect-0.1.1.tar", last modified: Wed Mar 29 21:09:18 2023, max compression
+gzip compressed data, was "credoai-connect-0.1.2.tar", last modified: Tue May  2 23:05:30 2023, max compression
```

## Comparing `credoai-connect-0.1.1.tar` & `credoai-connect-0.1.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:09:18.813807 credoai-connect-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-03-29 21:09:18.813807 credoai-connect-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:09:18.805807 credoai-connect-0.1.1/connect/
--rw-r--r--   0 runner    (1001) docker     (122)      278 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      212 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:09:18.809807 credoai-connect-0.1.1/connect/adapters/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6364 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/adapters/adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:09:18.809807 credoai-connect-0.1.1/connect/evidence/
--rw-r--r--   0 runner    (1001) docker     (122)      427 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/evidence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4700 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/evidence/containers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:09:18.809807 credoai-connect-0.1.1/connect/evidence/deepchecks_evidence/
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/evidence/deepchecks_evidence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/evidence/deepchecks_evidence/containers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/evidence/deepchecks_evidence/evidence.py
--rw-r--r--   0 runner    (1001) docker     (122)      495 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/evidence/deepchecks_evidence/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5928 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/evidence/evidence.py
--rw-r--r--   0 runner    (1001) docker     (122)      689 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/evidence/evidence_requirement.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:09:18.809807 credoai-connect-0.1.1/connect/evidence/lens_evidence/
--rw-r--r--   0 runner    (1001) docker     (122)       70 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/evidence/lens_evidence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/evidence/lens_evidence/containers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/evidence/lens_evidence/evidence.py
--rw-r--r--   0 runner    (1001) docker     (122)      523 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/evidence/lens_evidence/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:09:18.813807 credoai-connect-0.1.1/connect/governance/
--rw-r--r--   0 runner    (1001) docker     (122)       94 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/governance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5255 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/governance/credo_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     5695 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/governance/credo_api_client.py
--rw-r--r--   0 runner    (1001) docker     (122)    19128 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/governance/governance.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:09:18.813807 credoai-connect-0.1.1/connect/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4235 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     2729 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/utils/data_scrubbing.py
--rw-r--r--   0 runner    (1001) docker     (122)     2265 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)      988 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/connect/utils/version_check.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:09:18.813807 credoai-connect-0.1.1/credoai_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-03-29 21:09:18.000000 credoai-connect-0.1.1/credoai_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1152 2023-03-29 21:09:18.000000 credoai-connect-0.1.1/credoai_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-29 21:09:18.000000 credoai-connect-0.1.1/credoai_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-03-29 21:09:18.000000 credoai-connect-0.1.1/credoai_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-03-29 21:09:18.000000 credoai-connect-0.1.1/credoai_connect.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:09:18.813807 credoai-connect-0.1.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-29 21:09:18.817807 credoai-connect-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2090 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:09:18.813807 credoai-connect-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-29 21:09:10.000000 credoai-connect-0.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:30.514306 credoai-connect-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-05-02 23:05:30.510306 credoai-connect-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:30.510306 credoai-connect-0.1.2/connect/
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:30.510306 credoai-connect-0.1.2/connect/adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6364 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/adapters/adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:30.510306 credoai-connect-0.1.2/connect/evidence/
+-rw-r--r--   0 runner    (1001) docker     (122)      427 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/evidence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4700 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/evidence/containers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:30.510306 credoai-connect-0.1.2/connect/evidence/deepchecks_evidence/
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/evidence/deepchecks_evidence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/evidence/deepchecks_evidence/containers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/evidence/deepchecks_evidence/evidence.py
+-rw-r--r--   0 runner    (1001) docker     (122)      495 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/evidence/deepchecks_evidence/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5924 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/evidence/evidence.py
+-rw-r--r--   0 runner    (1001) docker     (122)      689 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/evidence/evidence_requirement.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:30.510306 credoai-connect-0.1.2/connect/evidence/lens_evidence/
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/evidence/lens_evidence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1911 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/evidence/lens_evidence/containers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/evidence/lens_evidence/evidence.py
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/evidence/lens_evidence/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:30.510306 credoai-connect-0.1.2/connect/governance/
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/governance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5255 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/governance/credo_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5695 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/governance/credo_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19128 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/governance/governance.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:30.510306 credoai-connect-0.1.2/connect/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4235 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2729 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/utils/data_scrubbing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2265 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)      988 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/connect/utils/version_check.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:30.510306 credoai-connect-0.1.2/credoai_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-05-02 23:05:30.000000 credoai-connect-0.1.2/credoai_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1152 2023-05-02 23:05:30.000000 credoai-connect-0.1.2/credoai_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 23:05:30.000000 credoai-connect-0.1.2/credoai_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-02 23:05:30.000000 credoai-connect-0.1.2/credoai_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-02 23:05:30.000000 credoai-connect-0.1.2/credoai_connect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:30.510306 credoai-connect-0.1.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-02 23:05:30.514306 credoai-connect-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:30.510306 credoai-connect-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 23:05:15.000000 credoai-connect-0.1.2/tests/__init__.py
```

### Comparing `credoai-connect-0.1.1/LICENSE` & `credoai-connect-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.1/PKG-INFO` & `credoai-connect-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: credoai-connect
-Version: 0.1.1
+Version: 0.1.2
 Summary: Credo AI Connect: Integration point for Credo AI Governance Platform
 Home-page: 
 Download-URL: https://github.com/credo-ai/credoai_connect
 Author: Ian Eisenberg
 Author-email: ian@credo.ai
 Maintainer: Ian Eisenberg
 Maintainer-email: ian@credo.ai
 Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
 --------------------------------------
```

### Comparing `credoai-connect-0.1.1/README.md` & `credoai-connect-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.1/connect/adapters/adapters.py` & `credoai-connect-0.1.2/connect/adapters/adapters.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.1/connect/evidence/containers.py` & `credoai-connect-0.1.2/connect/evidence/containers.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.1/connect/evidence/deepchecks_evidence/containers.py` & `credoai-connect-0.1.2/connect/evidence/deepchecks_evidence/containers.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.1/connect/evidence/deepchecks_evidence/evidence.py` & `credoai-connect-0.1.2/connect/evidence/deepchecks_evidence/evidence.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.1/connect/evidence/evidence.py` & `credoai-connect-0.1.2/connect/evidence/evidence.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         self._data = table_data
         super().__init__("table", additional_labels, **metadata)
 
     @property
     def data(self):
         columns = [
             {"value": k, "type": self._transform_type(v)}
-            for k, v in self._data.dtypes.iteritems()
+            for k, v in self._data.dtypes.items()
         ]
         return {
             "columns": columns,
             "value": self._data.values.tolist(),
         }
 
     @property
```

### Comparing `credoai-connect-0.1.1/connect/evidence/evidence_requirement.py` & `credoai-connect-0.1.2/connect/evidence/evidence_requirement.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.1/connect/evidence/lens_evidence/containers.py` & `credoai-connect-0.1.2/connect/evidence/lens_evidence/containers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import numpy as np
 
 from connect.evidence import EvidenceContainer
 from connect.utils import Scrubber, ValidationError
 
 from .evidence import DataProfilerEvidence, ModelProfilerEvidence
-from .utils import get_pandas_profile_type
+from .utils import get_ydata_profile_type
 
-PandasProfileType = get_pandas_profile_type()
+ydataProfileType = get_ydata_profile_type()
 
 
 class DataProfilerContainer(EvidenceContainer):
     """Container for all profiler type evidence"""
 
     def __init__(self, data, labels: dict = None, metadata: dict = None):
         super().__init__(DataProfilerEvidence, data, labels, metadata)
@@ -26,17 +26,17 @@
             )
         ]
 
     def _validate(self, data):
         pass
 
     def _validate_inputs(self, data):
-        if not isinstance(data, PandasProfileType):
+        if not isinstance(data, ydataProfileType):
             raise ValidationError(
-                "'data' must be a pandas_profiling.profile_report.ProfileReport"
+                "'data' must be a ydata_profiling.profile_report.ProfileReport"
             )
 
 
 class ModelProfilerContainer(EvidenceContainer):
     """Container for Model Profiler type evidence"""
 
     def __init__(self, data, labels=None, metadata=None):
```

### Comparing `credoai-connect-0.1.1/connect/evidence/lens_evidence/evidence.py` & `credoai-connect-0.1.2/connect/evidence/lens_evidence/evidence.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.1/connect/governance/credo_api.py` & `credoai-connect-0.1.2/connect/governance/credo_api.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.1/connect/governance/credo_api_client.py` & `credoai-connect-0.1.2/connect/governance/credo_api_client.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.1/connect/governance/governance.py` & `credoai-connect-0.1.2/connect/governance/governance.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.1/connect/utils/common.py` & `credoai-connect-0.1.2/connect/utils/common.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.1/connect/utils/data_scrubbing.py` & `credoai-connect-0.1.2/connect/utils/data_scrubbing.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.1/connect/utils/logging.py` & `credoai-connect-0.1.2/connect/utils/logging.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.1/connect/utils/version_check.py` & `credoai-connect-0.1.2/connect/utils/version_check.py`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.1/credoai_connect.egg-info/PKG-INFO` & `credoai-connect-0.1.2/credoai_connect.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: credoai-connect
-Version: 0.1.1
+Version: 0.1.2
 Summary: Credo AI Connect: Integration point for Credo AI Governance Platform
 Home-page: 
 Download-URL: https://github.com/credo-ai/credoai_connect
 Author: Ian Eisenberg
 Author-email: ian@credo.ai
 Maintainer: Ian Eisenberg
 Maintainer-email: ian@credo.ai
 Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
 --------------------------------------
```

### Comparing `credoai-connect-0.1.1/credoai_connect.egg-info/SOURCES.txt` & `credoai-connect-0.1.2/credoai_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `credoai-connect-0.1.1/setup.py` & `credoai-connect-0.1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 DISTNAME = "credoai-connect"
 MAINTAINER = "Ian Eisenberg"
 MAINTAINER_EMAIL = "ian@credo.ai"
 URL = ""
 LICENSE = ""
 DOWNLOAD_URL = "https://github.com/credo-ai/credoai_connect"
 VERSION = __version__
-PYTHON_REQUIRES = ">=3.8"
+PYTHON_REQUIRES = ">=3.7"
 
 # Fetch ReadMe
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
 # Use requirements.txt to set the install_requires
 with open("requirements.txt") as f:
@@ -32,26 +32,27 @@
 
 dev_requirements += doc_requirements
 
 EXTRAS_REQUIRES = {"dev": dev_requirements}
 
 CLASSIFIERS = [
     "Intended Audience :: Information Technology",
-    "Intended Audience :: Science/Research",
+    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Operating System :: OS Independent",
 ]
 
 PACKAGE_DATA = {}
 
 
 if __name__ == "__main__":
-
     import sys
 
     from setuptools import setup
 
     setup(
         name=DISTNAME,
         author=MAINTAINER,
```

