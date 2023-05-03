# Comparing `tmp/clams-python-0.5.3.tar.gz` & `tmp/clams-python-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clams-python-0.5.3.tar", last modified: Mon Mar 20 19:16:37 2023, max compression
+gzip compressed data, was "clams-python-0.6.0.tar", last modified: Wed May  3 02:46:30 2023, max compression
```

## Comparing `clams-python-0.5.3.tar` & `clams-python-0.6.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:16:37.525879 clams-python-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-03-20 19:16:18.000000 clams-python-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-20 19:16:18.000000 clams-python-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-03-20 19:16:37.525879 clams-python-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-03-20 19:16:18.000000 clams-python-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-20 19:16:18.000000 clams-python-0.5.3/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:16:37.521879 clams-python-0.5.3/clams/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-03-20 19:16:18.000000 clams-python-0.5.3/clams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:16:37.521879 clams-python-0.5.3/clams/app/
--rw-r--r--   0 runner    (1001) docker     (123)    11512 2023-03-20 19:16:18.000000 clams-python-0.5.3/clams/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:16:37.521879 clams-python-0.5.3/clams/appmetadata/
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-03-20 19:16:18.000000 clams-python-0.5.3/clams/appmetadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:16:37.521879 clams-python-0.5.3/clams/restify/
--rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-03-20 19:16:18.000000 clams-python-0.5.3/clams/restify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:16:37.521879 clams-python-0.5.3/clams/serve/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-20 19:16:18.000000 clams-python-0.5.3/clams/serve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:16:37.521879 clams-python-0.5.3/clams/source/
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-03-20 19:16:18.000000 clams-python-0.5.3/clams/source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:16:37.521879 clams-python-0.5.3/clams/ver/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-20 19:16:37.000000 clams-python-0.5.3/clams/ver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:16:37.521879 clams-python-0.5.3/clams_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-03-20 19:16:37.000000 clams-python-0.5.3/clams_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-20 19:16:37.000000 clams-python-0.5.3/clams_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 19:16:37.000000 clams-python-0.5.3/clams_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-20 19:16:37.000000 clams-python-0.5.3/clams_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-20 19:16:37.000000 clams-python-0.5.3/clams_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-20 19:16:37.000000 clams-python-0.5.3/clams_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-20 19:16:18.000000 clams-python-0.5.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 19:16:37.525879 clams-python-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-03-20 19:16:18.000000 clams-python-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:46:30.703936 clams-python-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-03 02:45:59.000000 clams-python-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-03 02:45:59.000000 clams-python-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-03 02:46:30.703936 clams-python-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-03 02:45:59.000000 clams-python-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 02:45:59.000000 clams-python-0.6.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:46:30.703936 clams-python-0.6.0/clams/
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-03 02:45:59.000000 clams-python-0.6.0/clams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:46:30.703936 clams-python-0.6.0/clams/app/
+-rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-05-03 02:45:59.000000 clams-python-0.6.0/clams/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:46:30.703936 clams-python-0.6.0/clams/appmetadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    16339 2023-05-03 02:45:59.000000 clams-python-0.6.0/clams/appmetadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:46:30.703936 clams-python-0.6.0/clams/develop/
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-03 02:45:59.000000 clams-python-0.6.0/clams/develop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:46:30.703936 clams-python-0.6.0/clams/restify/
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-05-03 02:45:59.000000 clams-python-0.6.0/clams/restify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:46:30.703936 clams-python-0.6.0/clams/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-03 02:45:59.000000 clams-python-0.6.0/clams/serve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:46:30.703936 clams-python-0.6.0/clams/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-05-03 02:45:59.000000 clams-python-0.6.0/clams/source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:46:30.703936 clams-python-0.6.0/clams/ver/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 02:46:30.000000 clams-python-0.6.0/clams/ver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:46:30.703936 clams-python-0.6.0/clams_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-03 02:46:30.000000 clams-python-0.6.0/clams_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-03 02:46:30.000000 clams-python-0.6.0/clams_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 02:46:30.000000 clams-python-0.6.0/clams_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-03 02:46:30.000000 clams-python-0.6.0/clams_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-03 02:46:30.000000 clams-python-0.6.0/clams_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 02:46:30.000000 clams-python-0.6.0/clams_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-03 02:45:59.000000 clams-python-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 02:46:30.703936 clams-python-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-03 02:45:59.000000 clams-python-0.6.0/setup.py
```

### Comparing `clams-python-0.5.3/LICENSE` & `clams-python-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clams-python-0.5.3/PKG-INFO` & `clams-python-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 0.5.3
+Version: 0.6.0
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 License: UNKNOWN
 Description: # CLAMS sdk for python
```

### Comparing `clams-python-0.5.3/README.md` & `clams-python-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `clams-python-0.5.3/clams/app/__init__.py` & `clams-python-0.6.0/clams/app/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import pathlib
 import sys
 import warnings
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from urllib import parse as urlparser
 
 __all__ = ['ClamsApp']
@@ -19,44 +20,60 @@
     this class and then can be used with classes in :mod:`.restify` to work as
     web applications.
     """
     # A set of "universal runtime parameters that can be used for both GET and POST anytime".
     # The behavioral changes based on these parameters must be implemented on the SDK level. 
     universal_parameters = [
         {
-            'name': 'pretty', 'type': 'boolean', 'choices': None, 'default': False,
+            'name': 'pretty', 'type': 'boolean', 'choices': None, 'default': False, 'multivalued': False,
             'description': 'The JSON body of the HTTP response will be re-formatted with 2-space indentation',
         },
     ]
 
     def __init__(self):
-        self.metadata: AppMetadata = self._appmetadata()
+        self.metadata: AppMetadata = self._load_metadata()
         super().__init__()
         # data type specification for common parameters
         python_type = {"boolean": bool, "number": float, "integer": int, "string": str}
 
         self.metadata_param_spec = {}
         self.annotate_param_spec = {}
         for param in ClamsApp.universal_parameters:
             self.metadata.add_parameter(**param)
-            self.metadata_param_spec[param['name']] = python_type[param['type']]
+            self.metadata_param_spec[param['name']] = (python_type[param['type']], param.get('multivalued', False))
         for param_spec in self.metadata.parameters:
-            self.annotate_param_spec[param_spec.name] = python_type[param_spec.type]
+            self.annotate_param_spec[param_spec.name] = (python_type[param_spec.type], param_spec.multivalued)
 
     def appmetadata(self, **kwargs) -> str:
         """
         A public method to get metadata for this app as a string.
 
         :return: Serialized JSON string of the metadata
         """
         pretty = kwargs.pop('pretty') if 'pretty' in kwargs else False
-        if pretty:
-            return self.metadata.json(exclude_defaults=True, by_alias=True, indent=2)
+        return self.metadata.jsonify(pretty)
+    
+    def _load_metadata(self):
+        cwd = pathlib.Path(sys.modules[self.__module__].__file__).parent
+        
+        # metadata compilation priority
+        # 1. metadata.py
+        # 2. metadata.json
+        # 3. _appmetadata() method (for legacy)
+        
+        if (cwd / 'metadata.py').exists():
+            import metadata as metadatapy  # pytype: disable=import-error
+            metadata = metadatapy.appmetadata()
+        elif (cwd / 'metadata.json').exists():
+            import json
+            with open(cwd / 'metadata.json') as f:
+                metadata = json.load(f)
         else:
-            return self.metadata.json(exclude_defaults=True, by_alias=True)
+            metadata = self._appmetadata()
+        return metadata
 
     @abstractmethod
     def _appmetadata(self) -> AppMetadata:
         """
         An abstract method to generate (or load if stored elsewhere) the app metadata
         at runtime. All CLAMS app must implement this. For metadata specification, 
         see `https://sdk.clams.ai/appmetadata.jsonschema <../appmetadata.jsonschema>`_. 
@@ -79,20 +96,14 @@
         :param runtime_params: An arbitrary set of k-v pairs to configure the app at runtime
         :return: Serialized JSON string of the output of the app
         """
         # TODO (krim @ 12/17/20): add documentation on what are "common" operations
         pretty = runtime_params.get('pretty', False)
         if not isinstance(mmif, Mmif):
             mmif = Mmif(mmif)
-        input_specver = mmif.metadata.mmif.rsplit('/')[-1]  # pytype: disable=attribute-error
-        if 'dev' not in __specver__ :
-            if not self._check_mmif_compatibility(__specver__, input_specver):
-                raise ValueError(f"Input MMIF file (versioned: {input_specver} is not compatible with the app "
-                                 f"targeting at {__specver__}. Make sure apps in the pipeline is all compatible. See "
-                                 f"https://mmif.clams.ai/versioning/ for information about MMIF compatibility. ") 
         issued_warnings = []
         for key in runtime_params:
             if key not in self.annotate_param_spec:
                 issued_warnings.append(UserWarning(f'An undefined parameter {key} (value: {runtime_params[key]}) is passed'))
         with warnings.catch_warnings(record=True) as ws:
             annotated = self._annotate(mmif, **runtime_params)
             if ws:
```

### Comparing `clams-python-0.5.3/clams/restify/__init__.py` & `clams-python-0.6.0/clams/restify/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from typing import Dict, Union
+from typing import Dict, Union, Any, Tuple, List
 
 import jsonschema
 from flask import Flask, request, Response
 from flask_restful import Resource, Api
 from mmif import Mmif
 
 from clams.app import ClamsApp
+from clams.appmetadata import primitives
 
 
 class Restifier(object):
     """
     Resitifier is a simple wrapper that takes a :class:`.ClamsApp` object and
     turn it into a flaks-based HTTP server. For mapping between Python API and
     HTTP API, it relies on :class:`.ClamsHTTPApi` class.
@@ -99,16 +100,16 @@
     ClamsHTTPApi provides mapping from HTTP verbs to Python API defined in :class:`.ClamsApp`.
 
     Constructor takes an instance of :class:`.ClamsApp`.
     """
     def __init__(self, cla_instance: ClamsApp):
         super().__init__()
         self.cla = cla_instance
-        self.metadata_param_caster = ParameterCaster(self.cla.metadata_param_spec)
-        self.annotate_param_caster = ParameterCaster(self.cla.annotate_param_spec)
+        self.metadata_param_caster = ParameterCaster(self.cla.metadata_param_spec)  # pytype: disable=wrong-arg-types
+        self.annotate_param_caster = ParameterCaster(self.cla.annotate_param_spec)  # pytype: disable=wrong-arg-types
 
     @staticmethod
     def json_to_response(json_str: str, status=200) -> Response:
         """
         Helper method to convert JSON output from a ClamsApp to a HTTP response.
 
         :param json_str: a serialized JSON .
@@ -131,17 +132,18 @@
         """
         Maps HTTP POST verb to :meth:`~clams.app.ClamsApp.annotate`.
         Note that for now HTTP PUT verbs is also mapped to :meth:`~clams.app.ClamsApp.annotate`.
 
         :return: Returns MMIF output from a ClamsApp in a HTTP response.
         """
         raw_data = request.get_data()
-        raw_params = request.args
+        # this will catch duplicate arguments with different values into a list under the key
+        raw_params = request.args.to_dict(False)
         try:
-            mmif = Mmif(raw_data)
+            _ = Mmif(raw_data)
         except jsonschema.exceptions.ValidationError as e:
             return Response(response="Invalid input data. See below for validation error.\n\n" + str(e), status=500, mimetype='text/plain')
         try:
             return self.json_to_response(self.cla.annotate(raw_data, **self.annotate_param_caster.cast(raw_params)))
         except Exception as e:
             return self.json_to_response(self.cla.record_error(raw_data, self.annotate_param_caster.cast(raw_params)).serialize(pretty=True), status=500)
 
@@ -151,43 +153,50 @@
 class ParameterCaster(object):
     """
     A helper class to convert parameters passed by HTTP query strings to
     proper python data types.
 
     :param param_spec: A specification of a data types of parameters
     """
-    def __init__(self, param_spec: Dict[str, type]):
+    def __init__(self, param_spec: Dict[str, Tuple[primitives, bool]]):
         self.param_spec = param_spec
 
-    def cast(self, args: Dict[str, str]) -> Dict[str, Union[int, float, str, bool]]:
+    def cast(self, args: Dict[str, List[str]]) -> Dict[str, Union[primitives, List[primitives]]]:
         """
         Given parameter specification, tries to cast values of args to specified Python data types.
         Note that this caster deals with query strings, thus all keys and values in the input args are plain strings. 
         Also note that the caster does not handle "unexpected" parameters came as an input. 
         Handling (raising an exception or issuing a warning upon receiving) an unexpected runtime parameter 
         must be done within the app itself.
         Thus, when a key is not found in the parameter specifications, it should just pass it as a vanilla string.
 
         :param args: k-v pairs
         :return: A new dictionary of type-casted args
         """
         casted = {}
-        for k, v in args.items():
-            if k in self.param_spec:
-                if self.param_spec[k] == bool:
-                    casted[k] = self.bool_param(v)
-                elif self.param_spec[k] == float:
-                    casted[k] = self.float_param(v)
-                elif self.param_spec[k] == int:
-                    casted[k] = self.int_param(v)
-                elif self.param_spec[k] == str:
-                    casted[k] = self.str_param(v)
-            else:
-                casted[k] = v
-                
+        for k, vs in args.items():
+            for v in vs:
+                if k in self.param_spec:
+                    type_, multivalued = self.param_spec[k]
+                    if multivalued or k not in casted:  # effectively only keeps the first value for non-multi params
+                        if type_ == bool:
+                            v = self.bool_param(v)
+                        elif type_ == float:
+                            v = self.float_param(v)
+                        elif type_ == int:
+                            v = self.int_param(v)
+                        elif type_ == str:
+                            v = self.str_param(v)
+                        if not multivalued:
+                            casted[k] = v
+                        else:
+                            casted.setdefault(k, []).append(v)
+                else:
+                    casted[k] = v[0]  # just keep the first value
+                    
         return casted
 
     @staticmethod
     def bool_param(value):
         """
         Helper function to convert string values to bool type.
         """
```

### Comparing `clams-python-0.5.3/clams/source/__init__.py` & `clams-python-0.6.0/clams/source/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -213,16 +213,19 @@
             mime=mime,
             location=location
         )
         pl.add_document(doc)
     return pl.produce().serialize(pretty=True)
 
 
-def prep_argparser():
-    parser = argparse.ArgumentParser()
+def prep_argparser(**kwargs):
+    """
+    provides CLI to create a "source" MMIF json. A source MMIF is a MMIF with a list of source documents but empty views. It can be used as a starting point for a CLAMS pipeline. 
+    """
+    parser = argparse.ArgumentParser(**kwargs)
     parser.add_argument(
         'documents',
         default=None,
         action='store',
         nargs='+',
         help="This list of documents should be colon-joined pairs of document types and file paths. A document type "
              "can be one of ``audio``, ``video``, ``text``, ``image``, or a MIME type string (such as video/mp4). The "
```

### Comparing `clams-python-0.5.3/clams_python.egg-info/PKG-INFO` & `clams-python-0.6.0/clams_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 0.5.3
+Version: 0.6.0
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 License: UNKNOWN
 Description: # CLAMS sdk for python
```

### Comparing `clams-python-0.5.3/setup.py` & `clams-python-0.6.0/setup.py`

 * *Files identical despite different names*

