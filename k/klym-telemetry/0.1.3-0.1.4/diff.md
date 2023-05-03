# Comparing `tmp/klym-telemetry-0.1.3.tar.gz` & `tmp/klym-telemetry-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klym-telemetry-0.1.3.tar", last modified: Tue May  2 13:24:16 2023, max compression
+gzip compressed data, was "klym-telemetry-0.1.4.tar", last modified: Wed May  3 15:22:14 2023, max compression
```

## Comparing `klym-telemetry-0.1.3.tar` & `klym-telemetry-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 13:24:16.648459 klym-telemetry-0.1.3/
--rw-rw-rw-   0        0        0     4076 2023-05-02 13:24:16.647458 klym-telemetry-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3148 2023-05-01 21:12:52.000000 klym-telemetry-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 13:24:16.617560 klym-telemetry-0.1.3/klym_telemetry/
--rw-rw-rw-   0        0        0        0 2023-04-22 00:00:44.000000 klym-telemetry-0.1.3/klym_telemetry/__init__.py
--rw-rw-rw-   0        0        0     2612 2023-04-23 22:09:56.000000 klym-telemetry-0.1.3/klym_telemetry/helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:24:16.643456 klym-telemetry-0.1.3/klym_telemetry/instrumenters/
--rw-rw-rw-   0        0        0      647 2023-05-01 21:12:52.000000 klym-telemetry-0.1.3/klym_telemetry/instrumenters/__init__.py
--rw-rw-rw-   0        0        0     2131 2023-04-25 19:42:07.000000 klym-telemetry-0.1.3/klym_telemetry/instrumenters/base.py
--rw-rw-rw-   0        0        0      625 2023-04-27 14:15:23.000000 klym-telemetry-0.1.3/klym_telemetry/instrumenters/celery.py
--rw-rw-rw-   0        0        0      625 2023-04-25 20:14:35.000000 klym-telemetry-0.1.3/klym_telemetry/instrumenters/django.py
--rw-rw-rw-   0        0        0      992 2023-04-25 20:10:43.000000 klym-telemetry-0.1.3/klym_telemetry/instrumenters/fastapi.py
--rw-rw-rw-   0        0        0      515 2023-05-01 21:09:25.000000 klym-telemetry-0.1.3/klym_telemetry/instrumenters/postgres.py
--rw-rw-rw-   0        0        0     5693 2023-04-23 22:09:56.000000 klym-telemetry-0.1.3/klym_telemetry/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:24:16.627455 klym-telemetry-0.1.3/klym_telemetry.egg-info/
--rw-rw-rw-   0        0        0     4076 2023-05-02 13:24:16.000000 klym-telemetry-0.1.3/klym_telemetry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      521 2023-05-02 13:24:16.000000 klym-telemetry-0.1.3/klym_telemetry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 13:24:16.000000 klym-telemetry-0.1.3/klym_telemetry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      406 2023-05-02 13:24:16.000000 klym-telemetry-0.1.3/klym_telemetry.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-02 13:24:16.000000 klym-telemetry-0.1.3/klym_telemetry.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 13:24:16.648459 klym-telemetry-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1795 2023-05-02 13:22:48.000000 klym-telemetry-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 15:22:14.656577 klym-telemetry-0.1.4/
+-rw-rw-rw-   0        0        0     4076 2023-05-03 15:22:14.655755 klym-telemetry-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3148 2023-05-01 21:12:52.000000 klym-telemetry-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 15:22:14.616328 klym-telemetry-0.1.4/klym_telemetry/
+-rw-rw-rw-   0        0        0        0 2023-04-22 00:00:44.000000 klym-telemetry-0.1.4/klym_telemetry/__init__.py
+-rw-rw-rw-   0        0        0     2612 2023-04-23 22:09:56.000000 klym-telemetry-0.1.4/klym_telemetry/helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-03 15:22:14.651578 klym-telemetry-0.1.4/klym_telemetry/instrumenters/
+-rw-rw-rw-   0        0        0      760 2023-05-03 15:20:06.000000 klym-telemetry-0.1.4/klym_telemetry/instrumenters/__init__.py
+-rw-rw-rw-   0        0        0     2131 2023-04-25 19:42:07.000000 klym-telemetry-0.1.4/klym_telemetry/instrumenters/base.py
+-rw-rw-rw-   0        0        0      507 2023-05-03 15:19:21.000000 klym-telemetry-0.1.4/klym_telemetry/instrumenters/celery.py
+-rw-rw-rw-   0        0        0      507 2023-05-03 15:18:48.000000 klym-telemetry-0.1.4/klym_telemetry/instrumenters/django.py
+-rw-rw-rw-   0        0        0      947 2023-05-03 15:17:41.000000 klym-telemetry-0.1.4/klym_telemetry/instrumenters/fastapi.py
+-rw-rw-rw-   0        0        0      515 2023-05-01 21:09:25.000000 klym-telemetry-0.1.4/klym_telemetry/instrumenters/postgres.py
+-rw-rw-rw-   0        0        0      515 2023-05-03 15:19:21.000000 klym-telemetry-0.1.4/klym_telemetry/instrumenters/requests.py
+-rw-rw-rw-   0        0        0     5693 2023-04-23 22:09:56.000000 klym-telemetry-0.1.4/klym_telemetry/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-03 15:22:14.631353 klym-telemetry-0.1.4/klym_telemetry.egg-info/
+-rw-rw-rw-   0        0        0     4076 2023-05-03 15:22:14.000000 klym-telemetry-0.1.4/klym_telemetry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      562 2023-05-03 15:22:14.000000 klym-telemetry-0.1.4/klym_telemetry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 15:22:14.000000 klym-telemetry-0.1.4/klym_telemetry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      406 2023-05-03 15:22:14.000000 klym-telemetry-0.1.4/klym_telemetry.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-03 15:22:14.000000 klym-telemetry-0.1.4/klym_telemetry.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 15:22:14.657598 klym-telemetry-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1795 2023-05-03 15:21:54.000000 klym-telemetry-0.1.4/setup.py
```

### Comparing `klym-telemetry-0.1.3/PKG-INFO` & `klym-telemetry-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klym-telemetry
-Version: 0.1.3
+Version: 0.1.4
 Summary: Scaffold library
 Home-page: https://dummy.readthedocs.io/
 Author: Klym Telemetry
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `klym-telemetry-0.1.3/README.md` & `klym-telemetry-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.3/klym_telemetry/helpers.py` & `klym-telemetry-0.1.4/klym_telemetry/helpers.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.3/klym_telemetry/instrumenters/__init__.py` & `klym-telemetry-0.1.4/klym_telemetry/instrumenters/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from klym_telemetry.instrumenters.celery import _CeleryInstrumentor
 from klym_telemetry.instrumenters.django import _DjangoInstrumentor
 from klym_telemetry.instrumenters.fastapi import _FastAPIInstrumentor
 from klym_telemetry.instrumenters.postgres import _Psycopg2Instrumentor
+from klym_telemetry.instrumenters.requests import _RequestsInstrumentor
 
 FACTORIES = {
     "fastapi": _FastAPIInstrumentor,
     "django": _DjangoInstrumentor,
     "celery": _CeleryInstrumentor,
     "psycopg2": _Psycopg2Instrumentor,
+    "requests": _RequestsInstrumentor,
 }
 
 
 def instrument_app(app_type: str, **kwargs):
     if app_type in FACTORIES:
         return FACTORIES[app_type](**kwargs).instrument()
     raise ValueError(f"Invalid app type: {app_type}")
```

### Comparing `klym-telemetry-0.1.3/klym_telemetry/instrumenters/base.py` & `klym-telemetry-0.1.4/klym_telemetry/instrumenters/base.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.3/klym_telemetry/instrumenters/celery.py` & `klym-telemetry-0.1.4/klym_telemetry/instrumenters/requests.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-from opentelemetry.instrumentation.celery import CeleryInstrumentor
 from opentelemetry.instrumentation.requests import RequestsInstrumentor
 
 from klym_telemetry.instrumenters.base import KLYMInstrumentor
 
 
-class _CeleryInstrumentor(KLYMInstrumentor):
+class _RequestsInstrumentor(KLYMInstrumentor):
 
     def __init__(self, service_name: str, endpoint: str) -> None:
         super().__init__(service_name=service_name, endpoint=endpoint)
 
     def instrument(self):
-        CeleryInstrumentor().instrument(
+        RequestsInstrumentor().instrument(
             tracer_provider=self.tracer_provider,
             meter_provider=self.meter_provider
         )
-        RequestsInstrumentor().instrument()
```

### Comparing `klym-telemetry-0.1.3/klym_telemetry/instrumenters/django.py` & `klym-telemetry-0.1.4/klym_telemetry/instrumenters/postgres.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-from opentelemetry.instrumentation.django import DjangoInstrumentor
-from opentelemetry.instrumentation.requests import RequestsInstrumentor
+from opentelemetry.instrumentation.psycopg2 import Psycopg2Instrumentor
 
 from klym_telemetry.instrumenters.base import KLYMInstrumentor
 
 
-class _DjangoInstrumentor(KLYMInstrumentor):
+class _Psycopg2Instrumentor(KLYMInstrumentor):
 
     def __init__(self, service_name: str, endpoint: str) -> None:
         super().__init__(service_name=service_name, endpoint=endpoint)
 
     def instrument(self):
-        DjangoInstrumentor().instrument(
+        Psycopg2Instrumentor().instrument(
             tracer_provider=self.tracer_provider,
             meter_provider=self.meter_provider
         )
-        RequestsInstrumentor().instrument()
```

### Comparing `klym-telemetry-0.1.3/klym_telemetry/instrumenters/fastapi.py` & `klym-telemetry-0.1.4/klym_telemetry/instrumenters/fastapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,8 +18,7 @@
     def instrument(self):
         FastAPIInstrumentor.instrument_app(
             app=self._app,
             tracer_provider=self.tracer_provider,
             meter_provider=self.meter_provider,
             excluded_urls=self._excluded_urls,
         )
-        RequestsInstrumentor().instrument()
```

### Comparing `klym-telemetry-0.1.3/klym_telemetry/utils.py` & `klym-telemetry-0.1.4/klym_telemetry/utils.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.3/klym_telemetry.egg-info/PKG-INFO` & `klym-telemetry-0.1.4/klym_telemetry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klym-telemetry
-Version: 0.1.3
+Version: 0.1.4
 Summary: Scaffold library
 Home-page: https://dummy.readthedocs.io/
 Author: Klym Telemetry
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `klym-telemetry-0.1.3/klym_telemetry.egg-info/SOURCES.txt` & `klym-telemetry-0.1.4/klym_telemetry.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -9,8 +9,9 @@
 klym_telemetry.egg-info/requires.txt
 klym_telemetry.egg-info/top_level.txt
 klym_telemetry/instrumenters/__init__.py
 klym_telemetry/instrumenters/base.py
 klym_telemetry/instrumenters/celery.py
 klym_telemetry/instrumenters/django.py
 klym_telemetry/instrumenters/fastapi.py
-klym_telemetry/instrumenters/postgres.py
+klym_telemetry/instrumenters/postgres.py
+klym_telemetry/instrumenters/requests.py
```

### Comparing `klym-telemetry-0.1.3/setup.py` & `klym-telemetry-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="klym-telemetry",
-    version="0.1.3",
+    version="0.1.4",
     description="Scaffold library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://dummy.readthedocs.io/",
     author="Klym Telemetry",
     author_email="example@email.com",
     license="MIT",
```

