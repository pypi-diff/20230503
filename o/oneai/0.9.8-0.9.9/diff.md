# Comparing `tmp/oneai-0.9.8.tar.gz` & `tmp/oneai-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oneai-0.9.8.tar", last modified: Sun Jan 22 17:45:42 2023, max compression
+gzip compressed data, was "oneai-0.9.9.tar", last modified: Sun Jan 22 19:40:56 2023, max compression
```

## Comparing `oneai-0.9.8.tar` & `oneai-0.9.9.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 michaelgur   (501) staff       (20)        0 2023-01-22 17:45:42.727458 oneai-0.9.8/
--rw-r--r--   0 michaelgur   (501) staff       (20)     1084 2022-07-27 08:48:35.000000 oneai-0.9.8/LICENSE
--rw-r--r--   0 michaelgur   (501) staff       (20)     7579 2023-01-22 17:45:42.727533 oneai-0.9.8/PKG-INFO
--rw-r--r--   0 michaelgur   (501) staff       (20)     7167 2022-08-27 22:48:27.000000 oneai-0.9.8/README.md
--rw-r--r--   0 michaelgur   (501) staff       (20)      104 2022-07-27 08:49:02.000000 oneai-0.9.8/pyproject.toml
--rw-r--r--   0 michaelgur   (501) staff       (20)      700 2023-01-22 17:45:42.727838 oneai-0.9.8/setup.cfg
-drwxr-xr-x   0 michaelgur   (501) staff       (20)        0 2023-01-22 17:45:42.722361 oneai-0.9.8/src/
-drwxr-xr-x   0 michaelgur   (501) staff       (20)        0 2023-01-22 17:45:42.725365 oneai-0.9.8/src/oneai/
--rw-r--r--   0 michaelgur   (501) staff       (20)     1299 2023-01-22 17:45:26.000000 oneai-0.9.8/src/oneai/__init__.py
-drwxr-xr-x   0 michaelgur   (501) staff       (20)        0 2023-01-22 17:45:42.727242 oneai-0.9.8/src/oneai/api/
--rw-r--r--   0 michaelgur   (501) staff       (20)      438 2022-12-18 06:49:48.000000 oneai-0.9.8/src/oneai/api/__init__.py
--rw-r--r--   0 michaelgur   (501) staff       (20)     3052 2022-12-18 06:49:48.000000 oneai-0.9.8/src/oneai/api/clustering.py
--rw-r--r--   0 michaelgur   (501) staff       (20)     2914 2022-11-14 20:26:11.000000 oneai-0.9.8/src/oneai/api/output.py
--rw-r--r--   0 michaelgur   (501) staff       (20)     3660 2023-01-02 10:24:42.000000 oneai-0.9.8/src/oneai/api/pipeline.py
--rw-r--r--   0 michaelgur   (501) staff       (20)    13662 2023-01-11 15:07:48.000000 oneai-0.9.8/src/oneai/classes.py
--rw-r--r--   0 michaelgur   (501) staff       (20)     6827 2023-01-03 13:45:25.000000 oneai-0.9.8/src/oneai/clustering.py
--rw-r--r--   0 michaelgur   (501) staff       (20)     2583 2022-09-22 14:06:15.000000 oneai-0.9.8/src/oneai/exceptions.py
--rw-r--r--   0 michaelgur   (501) staff       (20)     1008 2022-12-29 11:56:46.000000 oneai-0.9.8/src/oneai/logger.py
--rw-r--r--   0 michaelgur   (501) staff       (20)     6996 2022-12-18 07:31:42.000000 oneai-0.9.8/src/oneai/parsing.py
--rw-r--r--   0 michaelgur   (501) staff       (20)     9291 2022-12-25 10:43:59.000000 oneai-0.9.8/src/oneai/pipeline.py
--rw-r--r--   0 michaelgur   (501) staff       (20)     6499 2023-01-22 17:43:26.000000 oneai-0.9.8/src/oneai/process_scheduler.py
--rw-r--r--   0 michaelgur   (501) staff       (20)    20437 2023-01-19 13:40:49.000000 oneai-0.9.8/src/oneai/skills.py
-drwxr-xr-x   0 michaelgur   (501) staff       (20)        0 2023-01-22 17:45:42.726221 oneai-0.9.8/src/oneai.egg-info/
--rwxrwxrwx   0 michaelgur   (501) staff       (20)     7579 2023-01-22 17:45:42.000000 oneai-0.9.8/src/oneai.egg-info/PKG-INFO
--rwxrwxrwx   0 michaelgur   (501) staff       (20)      515 2023-01-22 17:45:42.000000 oneai-0.9.8/src/oneai.egg-info/SOURCES.txt
--rwxrwxrwx   0 michaelgur   (501) staff       (20)        1 2023-01-22 17:45:42.000000 oneai-0.9.8/src/oneai.egg-info/dependency_links.txt
--rwxrwxrwx   0 michaelgur   (501) staff       (20)      101 2023-01-22 17:45:42.000000 oneai-0.9.8/src/oneai.egg-info/requires.txt
--rwxrwxrwx   0 michaelgur   (501) staff       (20)        6 2023-01-22 17:45:42.000000 oneai-0.9.8/src/oneai.egg-info/top_level.txt
+drwxr-xr-x   0 michaelgur   (501) staff       (20)        0 2023-01-22 19:40:56.389530 oneai-0.9.9/
+-rw-r--r--   0 michaelgur   (501) staff       (20)     1084 2022-07-27 08:48:35.000000 oneai-0.9.9/LICENSE
+-rw-r--r--   0 michaelgur   (501) staff       (20)     7579 2023-01-22 19:40:56.389616 oneai-0.9.9/PKG-INFO
+-rw-r--r--   0 michaelgur   (501) staff       (20)     7167 2022-08-27 22:48:27.000000 oneai-0.9.9/README.md
+-rw-r--r--   0 michaelgur   (501) staff       (20)      104 2022-07-27 08:49:02.000000 oneai-0.9.9/pyproject.toml
+-rw-r--r--   0 michaelgur   (501) staff       (20)      700 2023-01-22 19:40:56.389949 oneai-0.9.9/setup.cfg
+drwxr-xr-x   0 michaelgur   (501) staff       (20)        0 2023-01-22 19:40:56.378584 oneai-0.9.9/src/
+drwxr-xr-x   0 michaelgur   (501) staff       (20)        0 2023-01-22 19:40:56.382346 oneai-0.9.9/src/oneai/
+-rw-r--r--   0 michaelgur   (501) staff       (20)     1325 2023-01-22 18:04:09.000000 oneai-0.9.9/src/oneai/__init__.py
+drwxr-xr-x   0 michaelgur   (501) staff       (20)        0 2023-01-22 19:40:56.389217 oneai-0.9.9/src/oneai/api/
+-rw-r--r--   0 michaelgur   (501) staff       (20)      438 2022-12-18 06:49:48.000000 oneai-0.9.9/src/oneai/api/__init__.py
+-rw-r--r--   0 michaelgur   (501) staff       (20)     3052 2022-12-18 06:49:48.000000 oneai-0.9.9/src/oneai/api/clustering.py
+-rw-r--r--   0 michaelgur   (501) staff       (20)     2914 2022-11-14 20:26:11.000000 oneai-0.9.9/src/oneai/api/output.py
+-rw-r--r--   0 michaelgur   (501) staff       (20)     3660 2023-01-02 10:24:42.000000 oneai-0.9.9/src/oneai/api/pipeline.py
+-rw-r--r--   0 michaelgur   (501) staff       (20)    14098 2023-01-22 19:39:04.000000 oneai-0.9.9/src/oneai/classes.py
+-rw-r--r--   0 michaelgur   (501) staff       (20)     6827 2023-01-03 13:45:25.000000 oneai-0.9.9/src/oneai/clustering.py
+-rw-r--r--   0 michaelgur   (501) staff       (20)     2583 2022-09-22 14:06:15.000000 oneai-0.9.9/src/oneai/exceptions.py
+-rw-r--r--   0 michaelgur   (501) staff       (20)     1008 2022-12-29 11:56:46.000000 oneai-0.9.9/src/oneai/logger.py
+-rw-r--r--   0 michaelgur   (501) staff       (20)     6996 2022-12-18 07:31:42.000000 oneai-0.9.9/src/oneai/parsing.py
+-rw-r--r--   0 michaelgur   (501) staff       (20)     9261 2023-01-22 19:37:16.000000 oneai-0.9.9/src/oneai/pipeline.py
+-rw-r--r--   0 michaelgur   (501) staff       (20)     6499 2023-01-22 19:32:24.000000 oneai-0.9.9/src/oneai/process_scheduler.py
+-rw-r--r--   0 michaelgur   (501) staff       (20)    20437 2023-01-19 13:40:49.000000 oneai-0.9.9/src/oneai/skills.py
+-rw-r--r--   0 michaelgur   (501) staff       (20)     1522 2023-01-22 19:39:34.000000 oneai-0.9.9/src/oneai/util.py
+drwxr-xr-x   0 michaelgur   (501) staff       (20)        0 2023-01-22 19:40:56.383421 oneai-0.9.9/src/oneai.egg-info/
+-rwxrwxrwx   0 michaelgur   (501) staff       (20)     7579 2023-01-22 19:40:56.000000 oneai-0.9.9/src/oneai.egg-info/PKG-INFO
+-rwxrwxrwx   0 michaelgur   (501) staff       (20)      533 2023-01-22 19:40:56.000000 oneai-0.9.9/src/oneai.egg-info/SOURCES.txt
+-rwxrwxrwx   0 michaelgur   (501) staff       (20)        1 2023-01-22 19:40:56.000000 oneai-0.9.9/src/oneai.egg-info/dependency_links.txt
+-rwxrwxrwx   0 michaelgur   (501) staff       (20)      101 2023-01-22 19:40:56.000000 oneai-0.9.9/src/oneai.egg-info/requires.txt
+-rwxrwxrwx   0 michaelgur   (501) staff       (20)        6 2023-01-22 19:40:56.000000 oneai-0.9.9/src/oneai.egg-info/top_level.txt
```

### Comparing `oneai-0.9.8/LICENSE` & `oneai-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oneai-0.9.8/PKG-INFO` & `oneai-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneai
-Version: 0.9.8
+Version: 0.9.9
 Summary: NLP as a Service
 Home-page: https://github.com/power-of-language/oneai-sdk-python
 Author: Michael Gur
 Author-email: devrel@oneai.com
 Project-URL: Bug Tracker, https://github.com/power-of-language/oneai-sdk-python/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: oneai Version: 0.9.8 Summary: NLP as a Service
+Metadata-Version: 2.1 Name: oneai Version: 0.9.9 Summary: NLP as a Service
 Home-page: https://github.com/power-of-language/oneai-sdk-python Author:
 Michael Gur Author-email: devrel@oneai.com Project-URL: Bug Tracker, https://
 github.com/power-of-language/oneai-sdk-python/issues Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE
 [./oneai_logo_light_cropped.svg]
 # Python SDK One AI is a NLP as a service platform. Our API enables language
```

### Comparing `oneai-0.9.8/README.md` & `oneai-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `oneai-0.9.8/setup.cfg` & `oneai-0.9.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `oneai-0.9.8/src/oneai/__init__.py` & `oneai-0.9.9/src/oneai/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 __package__ = "oneai"
 
 from typing_extensions import Final
 import oneai.logger
 import oneai.skills as skills
 from oneai.classes import *
 from oneai.pipeline import Pipeline
 import oneai.clustering as clustering
 import oneai.parsing as parsing
+import oneai.util as util
 
 URL: Final[str] = "https://api.oneai.com"
 """
 Base URL for the pipeline API. Only change if you know what you're doing.
 """
 
 api_key = None
```

### Comparing `oneai-0.9.8/src/oneai/api/clustering.py` & `oneai-0.9.9/src/oneai/api/clustering.py`

 * *Files identical despite different names*

### Comparing `oneai-0.9.8/src/oneai/api/output.py` & `oneai-0.9.9/src/oneai/api/output.py`

 * *Files identical despite different names*

### Comparing `oneai-0.9.8/src/oneai/api/pipeline.py` & `oneai-0.9.9/src/oneai/api/pipeline.py`

 * *Files identical despite different names*

### Comparing `oneai-0.9.8/src/oneai/classes.py` & `oneai-0.9.9/src/oneai/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
     Union,
+    Hashable,
 )
 from warnings import warn
 
 
 from oneai.exceptions import InputError
 
 if TYPE_CHECKING:
@@ -294,16 +295,16 @@
         Additional data associated with the label.
     """
 
     type: str = ""
     skill: str = ""
     name: str = ""
     _span: List[int] = field(default_factory=lambda: [0, 0], repr=False)
-    output_spans: List[int] = field(default_factory=list)
-    input_spans: List[int] = field(default_factory=list)
+    output_spans: List[Span] = field(default_factory=list)
+    input_spans: List[Span] = field(default_factory=list)
     span_text: str = ""
     timestamp: timedelta = None
     timestamp_end: timedelta = None
     value: str = ""
     data: dict = field(default_factory=dict)
 
     @property
@@ -423,7 +424,22 @@
 
     def __repr__(self) -> str:
         result = f"oneai.Output(text={repr(self.text)}"
         for skill in self.skills:
             attr = skill.output_attr or skill.api_name
             result += f", {attr}={repr(getattr(self, attr))}"
         return result + ")"
+
+
+class BatchResponse:
+    def __init__(self):
+        self._data: Dict[Input, Output] = {}
+
+    def __setitem__(self, key: Input, value: Output):
+        self._data[key] = value
+
+    def __getitem__(self, key: Input) -> Output:
+        return (
+            self._data[key]
+            if isinstance(key, Hashable) and key in self._data
+            else next(v for k, v in self._data.items() if k.text == key)
+        )
```

### Comparing `oneai-0.9.8/src/oneai/clustering.py` & `oneai-0.9.9/src/oneai/clustering.py`

 * *Files identical despite different names*

### Comparing `oneai-0.9.8/src/oneai/exceptions.py` & `oneai-0.9.9/src/oneai/exceptions.py`

 * *Files identical despite different names*

### Comparing `oneai-0.9.8/src/oneai/logger.py` & `oneai-0.9.9/src/oneai/logger.py`

 * *Files identical despite different names*

### Comparing `oneai-0.9.8/src/oneai/parsing.py` & `oneai-0.9.9/src/oneai/parsing.py`

 * *Files identical despite different names*

### Comparing `oneai-0.9.8/src/oneai/pipeline.py` & `oneai-0.9.9/src/oneai/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import concurrent.futures
 from io import IOBase
 import os
 import sys
 from typing import Awaitable, Callable, Dict, Iterable, List
 
 import oneai
-from oneai.classes import Output, PipelineInput, Skill, TextContent
+from oneai.classes import BatchResponse, Output, PipelineInput, Skill, TextContent
 from oneai.process_scheduler import *
 
 
 class Pipeline:
     """
     Language AI pipelines allow invoking and chaining multiple Language Skills to process your input text with a single API call.
 
@@ -149,15 +149,15 @@
         batch: Iterable[PipelineInput[TextContent]],
         api_key: str = None,
         on_output: Callable[
             [PipelineInput[TextContent], Output[TextContent]], None
         ] = None,
         on_error: Callable[[PipelineInput[TextContent], Exception], None] = None,
         multilingual: bool = False,
-    ) -> Dict[PipelineInput[TextContent], Output[TextContent]]:
+    ) -> BatchResponse:
         """
         Runs the pipeline on a batch of input texts.
 
         ## Parameters
 
         `batch: Iterable[PipelineInput]`
             The input texts to be processed.
@@ -187,15 +187,15 @@
         batch: Iterable[PipelineInput[TextContent]],
         api_key: str = None,
         on_output: Callable[
             [PipelineInput[TextContent], Output[TextContent]], None
         ] = None,
         on_error: Callable[[PipelineInput[TextContent], Exception], None] = None,
         multilingual: bool = False,
-    ) -> Awaitable[Dict[PipelineInput, Output]]:
+    ) -> Awaitable[BatchResponse]:
         """
         Runs the pipeline on a batch of input texts asynchronously.
 
         ## Parameters
 
         `batch: Iterable[str | Input]`
             The input texts to be processed.
@@ -212,15 +212,15 @@
 
         ## Raises
 
         `InputError` if the input is is invalid or is of an incompatible type for the pipeline.
         `APIKeyError` if the API key is invalid, expired, or missing quota.
         `ServerError` if an internal server error occured.
         """
-        outputs = dict()
+        outputs = BatchResponse()
         await process_batch(
             batch,
             self.steps,
             on_output if on_output else outputs.__setitem__,
             on_error if on_error else outputs.__setitem__,
             api_key=api_key or self.api_key or oneai.api_key,
             multilingual=multilingual or self.multilingual or oneai.multilingual,
```

### Comparing `oneai-0.9.8/src/oneai/process_scheduler.py` & `oneai-0.9.9/src/oneai/process_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     successful = 0  # total successful responses
     failed = 0  # number of exceptions occurred
     time_total = timedelta()  # total time spent on all requests
     # length = len(batch) if hasattr(batch, "__len__") else 0
 
     def next_input():  # distribute batch to workers
         try:
-            return next(iterator)
+            return Input.wrap(next(iterator))
         except StopIteration:
             return None  # we need to break loop for each worker, so we ignore StopIteration
 
     def log_progress(
         time_delta=timedelta(), start=False, end=False
     ):  # todo progress bar for iterables with __len__
         nonlocal successful, failed, time_total
@@ -129,15 +129,15 @@
         nonlocal successful, failed
 
         time_start = datetime.now()
         input = next_input()
         while input:
             try:
                 output = await _run_internal(
-                    session, Input.wrap(input), steps, api_key, multilingual
+                    session, input, steps, api_key, multilingual
                 )
                 on_output(input, output)
                 successful += 1
             except Exception as e:  # todo: break loop for some error types
                 logger.error(f"Input {successful + failed}: {repr(e)}")
                 on_error(input, e)
                 failed += 1
```

### Comparing `oneai-0.9.8/src/oneai/skills.py` & `oneai-0.9.9/src/oneai/skills.py`

 * *Files identical despite different names*

### Comparing `oneai-0.9.8/src/oneai.egg-info/PKG-INFO` & `oneai-0.9.9/src/oneai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneai
-Version: 0.9.8
+Version: 0.9.9
 Summary: NLP as a Service
 Home-page: https://github.com/power-of-language/oneai-sdk-python
 Author: Michael Gur
 Author-email: devrel@oneai.com
 Project-URL: Bug Tracker, https://github.com/power-of-language/oneai-sdk-python/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: oneai Version: 0.9.8 Summary: NLP as a Service
+Metadata-Version: 2.1 Name: oneai Version: 0.9.9 Summary: NLP as a Service
 Home-page: https://github.com/power-of-language/oneai-sdk-python Author:
 Michael Gur Author-email: devrel@oneai.com Project-URL: Bug Tracker, https://
 github.com/power-of-language/oneai-sdk-python/issues Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE
 [./oneai_logo_light_cropped.svg]
 # Python SDK One AI is a NLP as a service platform. Our API enables language
```

### Comparing `oneai-0.9.8/src/oneai.egg-info/SOURCES.txt` & `oneai-0.9.9/src/oneai.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/oneai/clustering.py
 src/oneai/exceptions.py
 src/oneai/logger.py
 src/oneai/parsing.py
 src/oneai/pipeline.py
 src/oneai/process_scheduler.py
 src/oneai/skills.py
+src/oneai/util.py
 src/oneai.egg-info/PKG-INFO
 src/oneai.egg-info/SOURCES.txt
 src/oneai.egg-info/dependency_links.txt
 src/oneai.egg-info/requires.txt
 src/oneai.egg-info/top_level.txt
 src/oneai/api/__init__.py
 src/oneai/api/clustering.py
```

