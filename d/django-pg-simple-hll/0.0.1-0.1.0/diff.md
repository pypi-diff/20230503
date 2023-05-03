# Comparing `tmp/django_pg_simple_hll-0.0.1.tar.gz` & `tmp/django_pg_simple_hll-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pg_simple_hll-0.0.1.tar", max compression
+gzip compressed data, was "django_pg_simple_hll-0.1.0.tar", max compression
```

## Comparing `django_pg_simple_hll-0.0.1.tar` & `django_pg_simple_hll-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-04-28 13:44:11.124569 django_pg_simple_hll-0.0.1/LICENSE
--rw-r--r--   0        0        0    10638 2023-04-28 13:44:11.124569 django_pg_simple_hll-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-04-28 13:44:11.124569 django_pg_simple_hll-0.0.1/django_pg_simple_hll/__init__.py
--rw-r--r--   0        0        0      688 2023-04-28 13:44:11.124569 django_pg_simple_hll-0.0.1/django_pg_simple_hll/aggregate.py
--rw-r--r--   0        0        0      528 2023-04-28 13:44:11.124569 django_pg_simple_hll-0.0.1/django_pg_simple_hll/migrations/0001_initial.py
--rw-r--r--   0        0        0      344 2023-04-28 13:44:11.124569 django_pg_simple_hll-0.0.1/django_pg_simple_hll/migrations/0001_initial.reverse.sql
--rw-r--r--   0        0        0     5679 2023-04-28 13:44:11.124569 django_pg_simple_hll-0.0.1/django_pg_simple_hll/migrations/0001_initial.sql
--rw-r--r--   0        0        0        0 2023-04-28 13:44:11.124569 django_pg_simple_hll-0.0.1/django_pg_simple_hll/migrations/__init__.py
--rw-r--r--   0        0        0        0 2023-04-28 13:44:11.124569 django_pg_simple_hll-0.0.1/django_pg_simple_hll/py.typed
--rw-r--r--   0        0        0     2950 2023-04-28 13:44:11.124569 django_pg_simple_hll-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    11773 1970-01-01 00:00:00.000000 django_pg_simple_hll-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-03 13:43:44.557555 django_pg_simple_hll-0.1.0/LICENSE
+-rw-r--r--   0        0        0    10638 2023-05-03 13:43:44.557555 django_pg_simple_hll-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-03 13:43:44.557555 django_pg_simple_hll-0.1.0/django_pg_simple_hll/__init__.py
+-rw-r--r--   0        0        0      688 2023-05-03 13:43:44.557555 django_pg_simple_hll-0.1.0/django_pg_simple_hll/aggregate.py
+-rw-r--r--   0        0        0      528 2023-05-03 13:43:44.557555 django_pg_simple_hll-0.1.0/django_pg_simple_hll/migrations/0001_initial.py
+-rw-r--r--   0        0        0      344 2023-05-03 13:43:44.557555 django_pg_simple_hll-0.1.0/django_pg_simple_hll/migrations/0001_initial.reverse.sql
+-rw-r--r--   0        0        0     5679 2023-05-03 13:43:44.557555 django_pg_simple_hll-0.1.0/django_pg_simple_hll/migrations/0001_initial.sql
+-rw-r--r--   0        0        0        0 2023-05-03 13:43:44.557555 django_pg_simple_hll-0.1.0/django_pg_simple_hll/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:43:44.557555 django_pg_simple_hll-0.1.0/django_pg_simple_hll/py.typed
+-rw-r--r--   0        0        0     2957 2023-05-03 13:43:44.557555 django_pg_simple_hll-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    11780 1970-01-01 00:00:00.000000 django_pg_simple_hll-0.1.0/PKG-INFO
```

### Comparing `django_pg_simple_hll-0.0.1/LICENSE` & `django_pg_simple_hll-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pg_simple_hll-0.0.1/README.md` & `django_pg_simple_hll-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django_pg_simple_hll-0.0.1/django_pg_simple_hll/aggregate.py` & `django_pg_simple_hll-0.1.0/django_pg_simple_hll/aggregate.py`

 * *Files identical despite different names*

### Comparing `django_pg_simple_hll-0.0.1/django_pg_simple_hll/migrations/0001_initial.py` & `django_pg_simple_hll-0.1.0/django_pg_simple_hll/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_pg_simple_hll-0.0.1/django_pg_simple_hll/migrations/0001_initial.sql` & `django_pg_simple_hll-0.1.0/django_pg_simple_hll/migrations/0001_initial.sql`

 * *Files identical despite different names*

### Comparing `django_pg_simple_hll-0.0.1/pyproject.toml` & `django_pg_simple_hll-0.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django_pg_simple_hll"
-version = "0.0.1"
+version = "0.1.0"
 description = "A low-privilege implementation of hyperloglog for django and postgres"
-authors = ["Beauhurst <dev@beauhurst.com>"]
+authors = ["Beauhurst <opensource@beauhurst.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
   "Environment :: Web Environment",
   "Framework :: Django",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
```

### Comparing `django_pg_simple_hll-0.0.1/PKG-INFO` & `django_pg_simple_hll-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: django-pg-simple-hll
-Version: 0.0.1
+Version: 0.1.0
 Summary: A low-privilege implementation of hyperloglog for django and postgres
 License: MIT
 Author: Beauhurst
-Author-email: dev@beauhurst.com
+Author-email: opensource@beauhurst.com
 Requires-Python: >=3.9,<3.12
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
```

