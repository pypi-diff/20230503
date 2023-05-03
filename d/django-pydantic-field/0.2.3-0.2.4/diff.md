# Comparing `tmp/django-pydantic-field-0.2.3.tar.gz` & `tmp/django-pydantic-field-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pydantic-field-0.2.3.tar", last modified: Sat Feb 25 11:04:32 2023, max compression
+gzip compressed data, was "django-pydantic-field-0.2.4.tar", last modified: Wed May  3 19:03:01 2023, max compression
```

## Comparing `django-pydantic-field-0.2.3.tar` & `django-pydantic-field-0.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 11:04:32.039702 django-pydantic-field-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-25 11:04:20.000000 django-pydantic-field-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-02-25 11:04:32.039702 django-pydantic-field-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-02-25 11:04:20.000000 django-pydantic-field-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 11:04:32.039702 django-pydantic-field-0.2.3/django_pydantic_field/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-25 11:04:20.000000 django-pydantic-field-0.2.3/django_pydantic_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-02-25 11:04:20.000000 django-pydantic-field-0.2.3/django_pydantic_field/_migration_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-02-25 11:04:20.000000 django-pydantic-field-0.2.3/django_pydantic_field/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-02-25 11:04:20.000000 django-pydantic-field-0.2.3/django_pydantic_field/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-02-25 11:04:20.000000 django-pydantic-field-0.2.3/django_pydantic_field/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-02-25 11:04:20.000000 django-pydantic-field-0.2.3/django_pydantic_field/rest_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-02-25 11:04:20.000000 django-pydantic-field-0.2.3/django_pydantic_field/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 11:04:32.039702 django-pydantic-field-0.2.3/django_pydantic_field.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-02-25 11:04:32.000000 django-pydantic-field-0.2.3/django_pydantic_field.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-02-25 11:04:32.000000 django-pydantic-field-0.2.3/django_pydantic_field.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-25 11:04:32.000000 django-pydantic-field-0.2.3/django_pydantic_field.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-02-25 11:04:32.000000 django-pydantic-field-0.2.3/django_pydantic_field.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-25 11:04:32.000000 django-pydantic-field-0.2.3/django_pydantic_field.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-02-25 11:04:20.000000 django-pydantic-field-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-25 11:04:32.039702 django-pydantic-field-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 11:04:32.039702 django-pydantic-field-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-02-25 11:04:20.000000 django-pydantic-field-0.2.3/tests/test_base_marshalling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-02-25 11:04:20.000000 django-pydantic-field-0.2.3/tests/test_django_model_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-02-25 11:04:20.000000 django-pydantic-field-0.2.3/tests/test_drf_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-02-25 11:04:20.000000 django-pydantic-field-0.2.3/tests/test_form_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-02-25 11:04:20.000000 django-pydantic-field-0.2.3/tests/test_sample_app_migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:03:01.539575 django-pydantic-field-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-05-03 19:03:01.539575 django-pydantic-field-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:03:01.535575 django-pydantic-field-0.2.4/django_pydantic_field/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/django_pydantic_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/django_pydantic_field/_migration_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/django_pydantic_field/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/django_pydantic_field/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/django_pydantic_field/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/django_pydantic_field/rest_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/django_pydantic_field/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:03:01.535575 django-pydantic-field-0.2.4/django_pydantic_field.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-05-03 19:03:01.000000 django-pydantic-field-0.2.4/django_pydantic_field.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-03 19:03:01.000000 django-pydantic-field-0.2.4/django_pydantic_field.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:03:01.000000 django-pydantic-field-0.2.4/django_pydantic_field.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-03 19:03:01.000000 django-pydantic-field-0.2.4/django_pydantic_field.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 19:03:01.000000 django-pydantic-field-0.2.4/django_pydantic_field.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 19:03:01.539575 django-pydantic-field-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:03:01.539575 django-pydantic-field-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/tests/test_base_marshalling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/tests/test_django_model_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/tests/test_drf_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/tests/test_form_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/tests/test_sample_app_migrations.py
```

### Comparing `django-pydantic-field-0.2.3/LICENSE` & `django-pydantic-field-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.3/PKG-INFO` & `django-pydantic-field-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pydantic-field
-Version: 0.2.3
+Version: 0.2.4
 Summary: Django JSONField with Pydantic models as a Schema
 Author-email: Savva Surenkov <savva@surenkov.space>
 License: MIT License
         
         Copyright (c) 2023 Savva Surenkov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,14 +35,15 @@
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `django-pydantic-field-0.2.3/README.md` & `django-pydantic-field-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.3/django_pydantic_field/_migration_serializers.py` & `django-pydantic-field-0.2.4/django_pydantic_field/_migration_serializers.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.3/django_pydantic_field/base.py` & `django-pydantic-field-0.2.4/django_pydantic_field/base.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.3/django_pydantic_field/fields.py` & `django-pydantic-field-0.2.4/django_pydantic_field/fields.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,14 +66,22 @@
             self._prepare_model_schema()
         try:
             assert self.decoder is not None
             return self.decoder().decode(value)
         except pydantic.ValidationError as e:
             raise django_exceptions.ValidationError(e.errors())
 
+    def get_prep_value(self, value) -> t.Optional[str]:
+        if not self.is_prepared_schema:
+            self._prepare_model_schema()
+        prep_value = super().get_prep_value(value)
+        if prep_value is not None and not isinstance(prep_value, str):
+            prep_value = self.encoder().encode(prep_value)  # type: ignore
+        return prep_value
+
     def deconstruct(self):
         name, path, args, kwargs = super().deconstruct()
         self._deconstruct_schema(kwargs)
         self._deconstruct_default(kwargs)
         self._deconstruct_config(kwargs)
 
         kwargs.pop("decoder")
@@ -138,16 +146,14 @@
         default = kwargs.get("default", NOT_PROVIDED)
 
         if not (default is NOT_PROVIDED or callable(default)):
             # default value deconstruction with SchemaEncoder is meaningful
             # only if schema resolution is not deferred
             if self.is_prepared_schema:
                 plain_default = self.get_prep_value(default)
-                if plain_default is not None:
-                    plain_default = json.loads(plain_default)
             else:
                 plain_default = default
 
             kwargs.update(default=plain_default)
 
     def _deconstruct_schema(self, kwargs):
         schema = self.schema
```

### Comparing `django-pydantic-field-0.2.3/django_pydantic_field/forms.py` & `django-pydantic-field-0.2.4/django_pydantic_field/forms.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.3/django_pydantic_field/rest_framework.py` & `django-pydantic-field-0.2.4/django_pydantic_field/rest_framework.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.3/django_pydantic_field/utils.py` & `django-pydantic-field-0.2.4/django_pydantic_field/utils.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.3/django_pydantic_field.egg-info/PKG-INFO` & `django-pydantic-field-0.2.4/django_pydantic_field.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pydantic-field
-Version: 0.2.3
+Version: 0.2.4
 Summary: Django JSONField with Pydantic models as a Schema
 Author-email: Savva Surenkov <savva@surenkov.space>
 License: MIT License
         
         Copyright (c) 2023 Savva Surenkov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,14 +35,15 @@
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `django-pydantic-field-0.2.3/django_pydantic_field.egg-info/SOURCES.txt` & `django-pydantic-field-0.2.4/django_pydantic_field.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.3/pyproject.toml` & `django-pydantic-field-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-pydantic-field"
-version = "0.2.3"
+version = "0.2.4"
 description = "Django JSONField with Pydantic models as a Schema"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
     { name = "Savva Surenkov", email = "savva@surenkov.space" },
 ]
 
@@ -19,14 +19,15 @@
     "Framework :: Django",
     "Framework :: Django :: 3",
     "Framework :: Django :: 3.1",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4",
     "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
     "Framework :: Pydantic",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
```

### Comparing `django-pydantic-field-0.2.3/tests/test_base_marshalling.py` & `django-pydantic-field-0.2.4/tests/test_base_marshalling.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.3/tests/test_django_model_field.py` & `django-pydantic-field-0.2.4/tests/test_django_model_field.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.3/tests/test_drf_adapters.py` & `django-pydantic-field-0.2.4/tests/test_drf_adapters.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.3/tests/test_form_field.py` & `django-pydantic-field-0.2.4/tests/test_form_field.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.3/tests/test_sample_app_migrations.py` & `django-pydantic-field-0.2.4/tests/test_sample_app_migrations.py`

 * *Files identical despite different names*

