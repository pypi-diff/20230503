# Comparing `tmp/visualblocks-0.0.2.tar.gz` & `tmp/visualblocks-0.0.3.tar.gz`

## Comparing `visualblocks-0.0.2.tar` & `visualblocks-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 visualblocks-0.0.2/.editorconfig
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 visualblocks-0.0.2/src/visualblocks/__init__.py
--rw-r--r--   0        0        0    12436 2020-02-02 00:00:00.000000 visualblocks-0.0.2/src/visualblocks/server.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 visualblocks-0.0.2/.gitignore
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 visualblocks-0.0.2/README.pypi.md
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 visualblocks-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 visualblocks-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 visualblocks-0.0.3/.editorconfig
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 visualblocks-0.0.3/src/visualblocks/__init__.py
+-rw-r--r--   0        0        0    14606 2020-02-02 00:00:00.000000 visualblocks-0.0.3/src/visualblocks/server.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 visualblocks-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 visualblocks-0.0.3/README.pypi.md
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 visualblocks-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 visualblocks-0.0.3/PKG-INFO
```

### Comparing `visualblocks-0.0.2/src/visualblocks/server.py` & `visualblocks-0.0.3/src/visualblocks/server.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,36 +4,87 @@
 from flask import request
 from flask import send_from_directory
 from google.colab import _message
 from google.colab import output
 from google.colab.output import eval_js
 from IPython import display
 from IPython.utils import io
+from typing import Literal
 import json
 import logging
 import numpy as np
 import os
 import portpicker
 import requests
 import shutil
 import sys
 import threading
 import traceback
 import urllib.parse
 import zipfile
 
-_VISUAL_BLOCKS_BUNDLE_VERSION = '1681885544'
+_VISUAL_BLOCKS_BUNDLE_VERSION = '1683083994'
 
 # Disable logging from werkzeug.
 #
 # Without this, flask will show a warning about using dev server (which is OK
 # in our usecase).
 logging.getLogger('werkzeug').disabled = True
 
 
+# Function registrations.
+GENERIC_FNS = {}
+TEXT_TO_TEXT_FNS = {}
+TEXT_TO_TENSORS_FNS = {}
+
+
+def register_vb_fn(type: Literal['generic', 'text_to_text', 'text_to_tensors']='generic'):
+  """A function decorator to register python function with Visual Blocks.
+
+  Args:
+    type:
+      the type of function to register for.
+
+      Currently, VB supports the following function types:
+
+      generic:
+        A function or iterable of functions, defined in the same Colab notebook,
+        that Visual Blocks can call to implement a generic model runner block.
+
+        A generic inference function must take a single argument, the input
+        tensors as an iterable of numpy.ndarrays; run inference; and return the
+        output tensors, also as an iterable of numpy.ndarrays.
+
+      text_to_text:
+        A function or iterable of functions, defined in the same Colab notebook,
+        that Visual Blocks can call to implement a text-to-text model runner
+        block.
+
+        A text_to_text function must take a string and return a string.
+
+      text_to_tensors:
+        A function or iterable of functions, defined in the same Colab notebook,
+        that Visual Blocks can call to implement a text-to-tensors model runner
+        block.
+
+        A text_to_tensors function must take a string and return the output
+        tensors, as an iterable of numpy.ndarrays.
+  """
+  def decorator_register_vb_fn(func):
+    func_name = func.__name__
+    if type == 'generic':
+      GENERIC_FNS[func_name] = func
+    elif type == 'text_to_text':
+      TEXT_TO_TEXT_FNS[func_name] = func
+    elif type == 'text_to_tensors':
+      TEXT_TO_TENSORS_FNS[func_name] = func
+    return func
+  return decorator_register_vb_fn
+
+
 def js(script):
   display.display(display.Javascript(script))
 
 
 def html(script):
   display.display(display.HTML(script))
 
@@ -59,34 +110,41 @@
   body = json.dumps(obj)
   resp = make_response(body)
   resp.headers['Content-Type'] = 'application/json'
   return resp
 
 
 def _ensure_iterable(x):
-  """Turn x into an iterable if not already iterable, unless it is None."""
-  if x is None or hasattr(x, '__iter__'):
+  """Turn x into an iterable if not already iterable."""
+  if x is None:
+    return ()
+  elif hasattr(x, '__iter__'):
     return x
   else:
     return (x,)
 
 
-def _find_fn(name:str, functions):
-  """Find a function in a list of functions by its string name."""
-  names = [fn.__name__ for fn in functions]
-  i = names.index(name)
-  return functions[i]
+def _add_to_registry(fns, registry):
+  """Adds the functions to the given registry (dict)."""
+  for fn in fns:
+    registry[fn.__name__] = fn
+
+
+def _is_list_of_nd_array(obj):
+  return isinstance(obj, list) and all(isinstance(elem, np.ndarray) for elem in obj)
 
 
 def Server(generic=None, text_to_text=None, text_to_tensors=None, height=900, tmp_dir='/tmp', read_saved_pipeline=True):
   """Creates a server that serves visual blocks web app in an iFrame.
 
   Other than serving the web app, it will also listen to requests sent from the
   web app at various API end points. Once a request is received, it will use the
-  data in the request body to call the corresponding functions passed in.
+  data in the request body to call the corresponding functions that users have
+  registered with VB, either through the '@register_vb_fn' decorator, or passed
+  in when creating the server.
 
   Args:
     generic:
       A function or iterable of functions, defined in the same Colab notebook,
       that Visual Blocks can call to implement a generic model runner block.
 
       A generic inference function must take a single argument, the input
@@ -114,17 +172,17 @@
     tmp_dir:
       The tmp dir where the server stores the web app's static resources.
 
     read_saved_pipeline:
       Whether to read the saved pipeline in the notebook or not.
   """
 
-  generic = _ensure_iterable(generic)
-  text_to_text = _ensure_iterable(text_to_text)
-  text_to_tensors = _ensure_iterable(text_to_tensors)
+  _add_to_registry(_ensure_iterable(generic), GENERIC_FNS)
+  _add_to_registry(_ensure_iterable(text_to_text), TEXT_TO_TEXT_FNS)
+  _add_to_registry(_ensure_iterable(text_to_tensors), TEXT_TO_TENSORS_FNS)
 
   app = Flask(__name__)
 
   # Disable startup messages.
   cli = sys.modules['flask.cli']
   cli.show_server_banner = lambda *x: None
 
@@ -155,75 +213,79 @@
     dt_string = now.strftime("%d/%m/%Y %H:%M:%S")
     with open(log_file_path, "a") as log_file:
       log_file.write("{}: {}\n".format(dt_string, msg))
 
   @app.route('/api/list_inference_functions')
   def list_inference_functions():
     result = {}
-    if generic:
-      result['generic'] = [fn.__name__ for fn in generic]
-    if text_to_text:
-      result['text_to_text'] = [fn.__name__ for fn in text_to_text]
-    if text_to_tensors:
-      result['text_to_tensors'] = [fn.__name__ for fn in text_to_tensors]
+    if len(GENERIC_FNS):
+      result['generic'] = list(GENERIC_FNS.keys())
+      result['generic'].sort()
+    if len(TEXT_TO_TEXT_FNS):
+      result['text_to_text'] = list(TEXT_TO_TEXT_FNS.keys())
+      result['text_to_text'].sort()
+    if len(TEXT_TO_TENSORS_FNS):
+      result['text_to_tensors'] = list(TEXT_TO_TENSORS_FNS.keys())
+      result['text_to_tensors'].sort()
     return _make_json_response(result)
 
   # Note: using "/api/..." for POST requests is not allowed.
   @app.route('/apipost/inference', methods=['POST'])
   def inference_generic():
     """Handler for the generic api endpoint."""
     result = {}
     try:
-      try:
-        inference_fn = _find_fn(request.json['function'], generic)
-      except KeyError:
-        # TODO: remove this fallback try-block after .js implments function key
-        inference_fn = generic[0]
+      func_name = request.json['function']
+      inference_fn = GENERIC_FNS[func_name]
       input_tensors = [_json_to_ndarray(x) for x in request.json['tensors']]
       output_tensors = inference_fn(input_tensors)
-      result['tensors'] = [_ndarray_to_json(x) for x in output_tensors]
+      if not _is_list_of_nd_array(output_tensors):
+        result = {'error': 'The returned value from %s is not a list of ndarray' % func_name}
+      else:
+        result['tensors'] = [_ndarray_to_json(x) for x in output_tensors]
     except Exception as e:
       msg = ''.join(traceback.format_exception(type(e), e, e.__traceback__))
       result = {'error': msg}
     finally:
       return _make_json_response(result)
 
   # Note: using "/api/..." for POST requests is not allowed.
   @app.route('/apipost/inference_text_to_text', methods=['POST'])
   def inference_text_to_text():
     """Handler for the text_to_text api endpoint."""
     result = {}
     try:
-      try:
-        inference_fn = _find_fn(request.json['function'], text_to_text)
-      except KeyError:
-        # TODO: remove this fallback try-block after .js implments function key
-        inference_fn = text_to_text[0]
+      func_name = request.json['function']
+      inference_fn = TEXT_TO_TEXT_FNS[func_name]
       text = request.json['text']
-      result['text'] = inference_fn(text)
+      ret = inference_fn(text)
+      if not isinstance(ret, str):
+        result = {'error': 'The returned value from %s is not a string' % func_name}
+      else:
+        result['text'] = ret
     except Exception as e:
       msg = ''.join(traceback.format_exception(type(e), e, e.__traceback__))
       result = {'error': msg}
     finally:
       return _make_json_response(result)
 
   # Note: using "/api/..." for POST requests is not allowed.
   @app.route('/apipost/inference_text_to_tensors', methods=['POST'])
   def inference_text_to_tensors():
     """Handler for the text_to_tensors api endpoint."""
     result = {}
     try:
-      try:
-        inference_fn = _find_fn(request.json['function'], text_to_tensors)
-      except KeyError:
-        # TODO: remove this fallback try-block after .js implments function key
-        inference_fn = text_to_tensors[0]
+      func_name = request.json['function']
+      inference_fn = TEXT_TO_TENSORS_FNS[func_name]
       text = request.json['text']
       output_tensors = inference_fn(text)
-      result['tensors'] = [_ndarray_to_json(x) for x in output_tensors]
+      if not _is_list_of_nd_array(output_tensors):
+        result = {'error': 'The returned value from %s is not a list of ndarray' % func_name}
+      else:
+        result['tensors'] = [_ndarray_to_json(x) for x in output_tensors]
     except Exception as e:
       msg = ''.join(traceback.format_exception(type(e), e, e.__traceback__))
       result = {'error': msg}
     finally:
       return _make_json_response(result)
 
   @app.route('/<path:path>')
```

### Comparing `visualblocks-0.0.2/README.pypi.md` & `visualblocks-0.0.3/README.pypi.md`

 * *Files identical despite different names*

### Comparing `visualblocks-0.0.2/pyproject.toml` & `visualblocks-0.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "visualblocks"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Google LLC", email="opensource@google.com" },
 ]
 description = "Visual Blocks for Google Colaboratory"
 readme = "README.pypi.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `visualblocks-0.0.2/PKG-INFO` & `visualblocks-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visualblocks
-Version: 0.0.2
+Version: 0.0.3
 Summary: Visual Blocks for Google Colaboratory
 Project-URL: Homepage, https://github.com/google/visualblocks
 Project-URL: Bug Tracker, https://github.com/google/visualblocks/issues
 Author-email: Google LLC <opensource@google.com>
 Classifier: Environment :: Other Environment
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

