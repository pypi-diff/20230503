# Comparing `tmp/drf-remotejwt-0.1.0.tar.gz` & `tmp/drf-remotejwt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-remotejwt-0.1.0.tar", last modified: Sun Apr 23 02:15:22 2023, max compression
+gzip compressed data, was "drf-remotejwt-0.1.2.tar", last modified: Wed May  3 01:00:45 2023, max compression
```

## Comparing `drf-remotejwt-0.1.0.tar` & `drf-remotejwt-0.1.2.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-23 02:15:22.296126 drf-remotejwt-0.1.0/
--rw-r--r--   0 garrethcain   (501) staff       (20)    33885 2023-04-21 05:14:06.000000 drf-remotejwt-0.1.0/LICENCE
--rw-r--r--   0 garrethcain   (501) staff       (20)      149 2023-04-21 05:14:06.000000 drf-remotejwt-0.1.0/MANIFEST.in
--rw-r--r--   0 garrethcain   (501) staff       (20)     7574 2023-04-23 02:15:22.296223 drf-remotejwt-0.1.0/PKG-INFO
--rw-r--r--   0 garrethcain   (501) staff       (20)       75 2023-04-21 05:14:06.000000 drf-remotejwt-0.1.0/README.rst
-drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-23 02:15:22.289161 drf-remotejwt-0.1.0/drf-remotejwt.egg-info/
--rw-r--r--   0 garrethcain   (501) staff       (20)     7574 2023-04-23 02:15:22.000000 drf-remotejwt-0.1.0/drf-remotejwt.egg-info/PKG-INFO
--rw-r--r--   0 garrethcain   (501) staff       (20)      740 2023-04-23 02:15:22.000000 drf-remotejwt-0.1.0/drf-remotejwt.egg-info/SOURCES.txt
--rw-r--r--   0 garrethcain   (501) staff       (20)        1 2023-04-23 02:15:22.000000 drf-remotejwt-0.1.0/drf-remotejwt.egg-info/dependency_links.txt
--rw-r--r--   0 garrethcain   (501) staff       (20)       57 2023-04-23 02:15:22.000000 drf-remotejwt-0.1.0/drf-remotejwt.egg-info/requires.txt
--rw-r--r--   0 garrethcain   (501) staff       (20)       25 2023-04-23 02:15:22.000000 drf-remotejwt-0.1.0/drf-remotejwt.egg-info/top_level.txt
--rw-r--r--   0 garrethcain   (501) staff       (20)      104 2023-04-21 05:14:06.000000 drf-remotejwt-0.1.0/pyproject.toml
-drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-23 02:15:22.291449 drf-remotejwt-0.1.0/remotejwt/
--rw-r--r--   0 garrethcain   (501) staff       (20)        0 2023-04-23 00:43:55.000000 drf-remotejwt-0.1.0/remotejwt/__init__.py
--rw-r--r--   0 garrethcain   (501) staff       (20)       63 2023-04-23 00:43:55.000000 drf-remotejwt-0.1.0/remotejwt/admin.py
--rw-r--r--   0 garrethcain   (501) staff       (20)      144 2023-04-23 00:43:55.000000 drf-remotejwt-0.1.0/remotejwt/apps.py
--rw-r--r--   0 garrethcain   (501) staff       (20)     7281 2023-04-23 00:43:55.000000 drf-remotejwt-0.1.0/remotejwt/authentication.py
-drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-23 02:15:22.291623 drf-remotejwt-0.1.0/remotejwt/migrations/
--rw-r--r--   0 garrethcain   (501) staff       (20)        0 2023-04-23 00:43:55.000000 drf-remotejwt-0.1.0/remotejwt/migrations/__init__.py
--rw-r--r--   0 garrethcain   (501) staff       (20)       57 2023-04-23 00:43:55.000000 drf-remotejwt-0.1.0/remotejwt/models.py
--rw-r--r--   0 garrethcain   (501) staff       (20)     1587 2023-04-23 00:43:55.000000 drf-remotejwt-0.1.0/remotejwt/serializers.py
--rw-r--r--   0 garrethcain   (501) staff       (20)     1971 2023-04-23 00:43:55.000000 drf-remotejwt-0.1.0/remotejwt/settings.py
--rw-r--r--   0 garrethcain   (501) staff       (20)       60 2023-04-23 00:43:55.000000 drf-remotejwt-0.1.0/remotejwt/tests.py
--rw-r--r--   0 garrethcain   (501) staff       (20)      370 2023-04-23 01:51:41.000000 drf-remotejwt-0.1.0/remotejwt/urls.py
--rw-r--r--   0 garrethcain   (501) staff       (20)     5546 2023-04-23 00:43:55.000000 drf-remotejwt-0.1.0/remotejwt/utils.py
--rw-r--r--   0 garrethcain   (501) staff       (20)     1518 2023-04-23 00:43:55.000000 drf-remotejwt-0.1.0/remotejwt/views.py
-drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-23 02:15:22.295824 drf-remotejwt-0.1.0/remotejwt_user/
--rw-r--r--   0 garrethcain   (501) staff       (20)        0 2023-04-23 00:46:13.000000 drf-remotejwt-0.1.0/remotejwt_user/__init__.py
--rw-r--r--   0 garrethcain   (501) staff       (20)     3324 2023-04-23 01:20:39.000000 drf-remotejwt-0.1.0/remotejwt_user/admin.py
--rw-r--r--   0 garrethcain   (501) staff       (20)      159 2023-04-23 01:20:52.000000 drf-remotejwt-0.1.0/remotejwt_user/apps.py
--rw-r--r--   0 garrethcain   (501) staff       (20)     8965 2023-04-23 00:46:13.000000 drf-remotejwt-0.1.0/remotejwt_user/models.py
--rw-r--r--   0 garrethcain   (501) staff       (20)        0 2023-04-23 00:46:13.000000 drf-remotejwt-0.1.0/remotejwt_user/permissions.py
--rw-r--r--   0 garrethcain   (501) staff       (20)      587 2023-04-23 00:46:13.000000 drf-remotejwt-0.1.0/remotejwt_user/serializers.py
--rw-r--r--   0 garrethcain   (501) staff       (20)       60 2023-04-23 00:46:13.000000 drf-remotejwt-0.1.0/remotejwt_user/tests.py
--rw-r--r--   0 garrethcain   (501) staff       (20)      168 2023-04-23 01:42:04.000000 drf-remotejwt-0.1.0/remotejwt_user/urls.py
--rw-r--r--   0 garrethcain   (501) staff       (20)      673 2023-04-23 00:48:32.000000 drf-remotejwt-0.1.0/remotejwt_user/views.py
--rw-r--r--   0 garrethcain   (501) staff       (20)     1221 2023-04-23 02:15:22.296691 drf-remotejwt-0.1.0/setup.cfg
--rw-r--r--   0 garrethcain   (501) staff       (20)       37 2023-04-21 05:14:06.000000 drf-remotejwt-0.1.0/setup.py
+drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-05-03 01:00:45.837069 drf-remotejwt-0.1.2/
+-rw-r--r--   0 garrethcain   (501) staff       (20)    33885 2023-04-21 05:14:06.000000 drf-remotejwt-0.1.2/LICENCE
+-rw-r--r--   0 garrethcain   (501) staff       (20)      149 2023-04-21 05:14:06.000000 drf-remotejwt-0.1.2/MANIFEST.in
+-rw-r--r--   0 garrethcain   (501) staff       (20)    20054 2023-05-03 01:00:45.837176 drf-remotejwt-0.1.2/PKG-INFO
+-rw-r--r--   0 garrethcain   (501) staff       (20)    18887 2023-05-03 00:57:17.000000 drf-remotejwt-0.1.2/README.MD
+-rw-r--r--   0 garrethcain   (501) staff       (20)       75 2023-04-21 05:14:06.000000 drf-remotejwt-0.1.2/README.rst
+drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-05-03 01:00:45.834335 drf-remotejwt-0.1.2/drf-remotejwt.egg-info/
+-rw-r--r--   0 garrethcain   (501) staff       (20)    20054 2023-05-03 01:00:45.000000 drf-remotejwt-0.1.2/drf-remotejwt.egg-info/PKG-INFO
+-rw-r--r--   0 garrethcain   (501) staff       (20)      750 2023-05-03 01:00:45.000000 drf-remotejwt-0.1.2/drf-remotejwt.egg-info/SOURCES.txt
+-rw-r--r--   0 garrethcain   (501) staff       (20)        1 2023-05-03 01:00:45.000000 drf-remotejwt-0.1.2/drf-remotejwt.egg-info/dependency_links.txt
+-rw-r--r--   0 garrethcain   (501) staff       (20)       57 2023-05-03 01:00:45.000000 drf-remotejwt-0.1.2/drf-remotejwt.egg-info/requires.txt
+-rw-r--r--   0 garrethcain   (501) staff       (20)       25 2023-05-03 01:00:45.000000 drf-remotejwt-0.1.2/drf-remotejwt.egg-info/top_level.txt
+-rw-r--r--   0 garrethcain   (501) staff       (20)      104 2023-04-21 05:14:06.000000 drf-remotejwt-0.1.2/pyproject.toml
+drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-05-03 01:00:45.835821 drf-remotejwt-0.1.2/remotejwt/
+-rw-r--r--   0 garrethcain   (501) staff       (20)        0 2023-05-03 00:57:17.000000 drf-remotejwt-0.1.2/remotejwt/__init__.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)       63 2023-05-03 00:57:17.000000 drf-remotejwt-0.1.2/remotejwt/admin.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)      144 2023-05-03 00:57:17.000000 drf-remotejwt-0.1.2/remotejwt/apps.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)     7281 2023-05-03 00:57:17.000000 drf-remotejwt-0.1.2/remotejwt/authentication.py
+drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-05-03 01:00:45.835954 drf-remotejwt-0.1.2/remotejwt/migrations/
+-rw-r--r--   0 garrethcain   (501) staff       (20)        0 2023-05-03 00:57:17.000000 drf-remotejwt-0.1.2/remotejwt/migrations/__init__.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)       57 2023-05-03 00:57:17.000000 drf-remotejwt-0.1.2/remotejwt/models.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)     1587 2023-05-03 00:57:17.000000 drf-remotejwt-0.1.2/remotejwt/serializers.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)     1971 2023-05-03 00:57:17.000000 drf-remotejwt-0.1.2/remotejwt/settings.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)       60 2023-05-03 00:57:17.000000 drf-remotejwt-0.1.2/remotejwt/tests.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)      370 2023-05-03 00:57:17.000000 drf-remotejwt-0.1.2/remotejwt/urls.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)     5546 2023-05-03 00:57:17.000000 drf-remotejwt-0.1.2/remotejwt/utils.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)     1518 2023-05-03 00:57:17.000000 drf-remotejwt-0.1.2/remotejwt/views.py
+drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-05-03 01:00:45.836942 drf-remotejwt-0.1.2/remotejwt_user/
+-rw-r--r--   0 garrethcain   (501) staff       (20)        0 2023-05-03 00:57:17.000000 drf-remotejwt-0.1.2/remotejwt_user/__init__.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)     3324 2023-05-03 00:57:17.000000 drf-remotejwt-0.1.2/remotejwt_user/admin.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)      159 2023-05-03 00:57:17.000000 drf-remotejwt-0.1.2/remotejwt_user/apps.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)     8965 2023-05-03 00:57:17.000000 drf-remotejwt-0.1.2/remotejwt_user/models.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)        0 2023-05-03 00:57:17.000000 drf-remotejwt-0.1.2/remotejwt_user/permissions.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)      587 2023-05-03 00:57:17.000000 drf-remotejwt-0.1.2/remotejwt_user/serializers.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)       60 2023-05-03 00:57:17.000000 drf-remotejwt-0.1.2/remotejwt_user/tests.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)      168 2023-05-03 00:57:17.000000 drf-remotejwt-0.1.2/remotejwt_user/urls.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)      673 2023-05-03 00:57:17.000000 drf-remotejwt-0.1.2/remotejwt_user/views.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)     1221 2023-05-03 01:00:45.837805 drf-remotejwt-0.1.2/setup.cfg
+-rw-r--r--   0 garrethcain   (501) staff       (20)       37 2023-04-21 05:14:06.000000 drf-remotejwt-0.1.2/setup.py
```

### Comparing `drf-remotejwt-0.1.0/LICENCE` & `drf-remotejwt-0.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `drf-remotejwt-0.1.0/drf-remotejwt.egg-info/SOURCES.txt` & `drf-remotejwt-0.1.2/drf-remotejwt.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENCE
 MANIFEST.in
+README.MD
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 drf-remotejwt.egg-info/PKG-INFO
 drf-remotejwt.egg-info/SOURCES.txt
 drf-remotejwt.egg-info/dependency_links.txt
```

### Comparing `drf-remotejwt-0.1.0/remotejwt/authentication.py` & `drf-remotejwt-0.1.2/remotejwt/authentication.py`

 * *Files identical despite different names*

### Comparing `drf-remotejwt-0.1.0/remotejwt/serializers.py` & `drf-remotejwt-0.1.2/remotejwt/serializers.py`

 * *Files identical despite different names*

### Comparing `drf-remotejwt-0.1.0/remotejwt/settings.py` & `drf-remotejwt-0.1.2/remotejwt/settings.py`

 * *Files identical despite different names*

### Comparing `drf-remotejwt-0.1.0/remotejwt/utils.py` & `drf-remotejwt-0.1.2/remotejwt/utils.py`

 * *Files identical despite different names*

### Comparing `drf-remotejwt-0.1.0/remotejwt/views.py` & `drf-remotejwt-0.1.2/remotejwt/views.py`

 * *Files identical despite different names*

### Comparing `drf-remotejwt-0.1.0/remotejwt_user/admin.py` & `drf-remotejwt-0.1.2/remotejwt_user/admin.py`

 * *Files identical despite different names*

### Comparing `drf-remotejwt-0.1.0/remotejwt_user/models.py` & `drf-remotejwt-0.1.2/remotejwt_user/models.py`

 * *Files identical despite different names*

### Comparing `drf-remotejwt-0.1.0/remotejwt_user/serializers.py` & `drf-remotejwt-0.1.2/remotejwt_user/serializers.py`

 * *Files identical despite different names*

### Comparing `drf-remotejwt-0.1.0/remotejwt_user/views.py` & `drf-remotejwt-0.1.2/remotejwt_user/views.py`

 * *Files identical despite different names*

### Comparing `drf-remotejwt-0.1.0/setup.cfg` & `drf-remotejwt-0.1.2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = drf-remotejwt
-version = 0.1.0
+version = 0.1.2
 description = A package to authenticate against a remote Authentication Service that support JWTs, think microservice authentication backend.
 long_description = file: README.MD
 long_description_content_type = text/markdown
 readme = "README.MD"
 url = https://github.com/garrethcain/drf-remotejwt
 author = Garreth Cain
 author_email = garrethccain@gmail.com
```

