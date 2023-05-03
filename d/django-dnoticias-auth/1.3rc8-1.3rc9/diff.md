# Comparing `tmp/django_dnoticias_auth-1.3rc8.tar.gz` & `tmp/django_dnoticias_auth-1.3rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/nelson/Development/dnoticias_auth/dist/tmpsspdp9se/django_dnoticias_auth-1.3rc8.tar", last modified: Wed Oct 19 13:28:12 2022, max compression
+gzip compressed data, was "/home/nelson/Development/dnoticias_auth/dist/tmpj43titra/django_dnoticias_auth-1.3rc9.tar", last modified: Wed Oct 19 15:04:33 2022, max compression
```

## Comparing `django_dnoticias_auth-1.3rc8.tar` & `django_dnoticias_auth-1.3rc9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-10-19 13:28:12.000000 django_dnoticias_auth-1.3rc8/
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     1082 2021-05-04 15:02:45.000000 django_dnoticias_auth-1.3rc8/LICENSE
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     3835 2022-10-19 13:28:12.000000 django_dnoticias_auth-1.3rc8/PKG-INFO
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     3520 2022-08-24 15:50:28.000000 django_dnoticias_auth-1.3rc8/README.md
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-10-19 13:28:12.000000 django_dnoticias_auth-1.3rc8/django_dnoticias_auth.egg-info/
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     3835 2022-10-19 13:28:12.000000 django_dnoticias_auth-1.3rc8/django_dnoticias_auth.egg-info/PKG-INFO
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     1210 2022-10-19 13:28:12.000000 django_dnoticias_auth-1.3rc8/django_dnoticias_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 nelson    (1000) nelson    (1000)        1 2022-10-19 13:28:12.000000 django_dnoticias_auth-1.3rc8/django_dnoticias_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      100 2022-10-19 13:28:12.000000 django_dnoticias_auth-1.3rc8/django_dnoticias_auth.egg-info/requires.txt
--rw-rw-r--   0 nelson    (1000) nelson    (1000)       15 2022-10-19 13:28:12.000000 django_dnoticias_auth-1.3rc8/django_dnoticias_auth.egg-info/top_level.txt
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-10-19 13:28:12.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/
--rw-rw-r--   0 nelson    (1000) nelson    (1000)        0 2021-05-04 15:02:45.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/__init__.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      102 2022-01-17 14:29:30.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/apps.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     6126 2022-10-19 10:47:58.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/backends.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      161 2022-09-13 09:16:02.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/context_processors.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      223 2022-10-18 13:20:59.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/cookies_consts.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)       52 2022-01-13 14:27:54.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/exceptions.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     3740 2022-09-13 09:20:55.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/forms.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)    13655 2022-10-19 10:49:41.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/middleware.py
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-10-19 13:28:12.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/migrations/
--rw-r--r--   0 nelson    (1000) nelson    (1000)     2873 2022-09-20 15:55:11.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/migrations/0001_initial.py
--rw-r--r--   0 nelson    (1000) nelson    (1000)      434 2022-09-28 10:25:30.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/migrations/0002_alter_user_id.py
--rw-r--r--   0 nelson    (1000) nelson    (1000)      473 2022-10-12 09:59:04.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/migrations/0003_alter_user_id.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)        0 2021-05-04 15:02:45.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/migrations/__init__.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      512 2022-09-13 09:34:51.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/models.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     5271 2022-10-19 13:25:42.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/redis.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     1174 2022-09-13 09:38:22.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/session.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      397 2022-09-13 09:38:58.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/signals.py
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-10-19 13:28:12.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/templates/
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-10-19 13:28:12.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/templates/authentication/
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      679 2022-02-03 11:59:00.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/templates/authentication/app-data.html
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-10-19 13:28:12.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/templates/authentication/includes/
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      331 2022-04-29 10:56:49.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/templates/authentication/includes/auth.html
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      316 2021-05-04 15:02:45.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/templates/authentication/includes/keycloak.html
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     7895 2022-02-15 17:57:17.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/templates/authentication/password-recovery.html
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     1011 2022-10-06 10:23:15.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/templates/authentication/silent-check-sso.html
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-10-19 13:28:12.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/templatetags/
--rw-rw-r--   0 nelson    (1000) nelson    (1000)        0 2021-08-20 09:37:45.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/templatetags/__init__.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     1961 2022-09-28 14:17:56.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/templatetags/auth_utils.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      702 2022-09-13 09:39:41.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/urls.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     9305 2022-10-19 13:18:29.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/utils.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     9914 2022-10-06 10:24:04.000000 django_dnoticias_auth-1.3rc8/dnoticias_auth/views.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)       38 2022-10-19 13:28:12.000000 django_dnoticias_auth-1.3rc8/setup.cfg
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      855 2022-10-19 13:26:47.000000 django_dnoticias_auth-1.3rc8/setup.py
+drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-10-19 15:04:33.000000 django_dnoticias_auth-1.3rc9/
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     1082 2021-05-04 15:02:45.000000 django_dnoticias_auth-1.3rc9/LICENSE
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     3835 2022-10-19 15:04:33.000000 django_dnoticias_auth-1.3rc9/PKG-INFO
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     3520 2022-08-24 15:50:28.000000 django_dnoticias_auth-1.3rc9/README.md
+drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-10-19 15:04:33.000000 django_dnoticias_auth-1.3rc9/django_dnoticias_auth.egg-info/
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     3835 2022-10-19 15:04:33.000000 django_dnoticias_auth-1.3rc9/django_dnoticias_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     1210 2022-10-19 15:04:33.000000 django_dnoticias_auth-1.3rc9/django_dnoticias_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)        1 2022-10-19 15:04:33.000000 django_dnoticias_auth-1.3rc9/django_dnoticias_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      100 2022-10-19 15:04:33.000000 django_dnoticias_auth-1.3rc9/django_dnoticias_auth.egg-info/requires.txt
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)       15 2022-10-19 15:04:33.000000 django_dnoticias_auth-1.3rc9/django_dnoticias_auth.egg-info/top_level.txt
+drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-10-19 15:04:33.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)        0 2021-05-04 15:02:45.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/__init__.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      102 2022-01-17 14:29:30.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/apps.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     6146 2022-10-19 14:59:51.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/backends.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      161 2022-09-13 09:16:02.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/context_processors.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      223 2022-10-18 13:20:59.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/cookies_consts.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)       52 2022-01-13 14:27:54.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/exceptions.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     3740 2022-09-13 09:20:55.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/forms.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)    13676 2022-10-19 14:59:40.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/middleware.py
+drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-10-19 15:04:33.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/migrations/
+-rw-r--r--   0 nelson    (1000) nelson    (1000)     2873 2022-09-20 15:55:11.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/migrations/0001_initial.py
+-rw-r--r--   0 nelson    (1000) nelson    (1000)      434 2022-09-28 10:25:30.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/migrations/0002_alter_user_id.py
+-rw-r--r--   0 nelson    (1000) nelson    (1000)      473 2022-10-12 09:59:04.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/migrations/0003_alter_user_id.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)        0 2021-05-04 15:02:45.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/migrations/__init__.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      512 2022-09-13 09:34:51.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/models.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     5271 2022-10-19 13:25:42.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/redis.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     1174 2022-09-13 09:38:22.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/session.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      397 2022-09-13 09:38:58.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/signals.py
+drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-10-19 15:04:33.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/templates/
+drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-10-19 15:04:33.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/templates/authentication/
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      679 2022-02-03 11:59:00.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/templates/authentication/app-data.html
+drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-10-19 15:04:33.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/templates/authentication/includes/
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      331 2022-04-29 10:56:49.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/templates/authentication/includes/auth.html
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      316 2021-05-04 15:02:45.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/templates/authentication/includes/keycloak.html
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     7895 2022-02-15 17:57:17.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/templates/authentication/password-recovery.html
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     1011 2022-10-06 10:23:15.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/templates/authentication/silent-check-sso.html
+drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-10-19 15:04:33.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/templatetags/
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)        0 2021-08-20 09:37:45.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/templatetags/__init__.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     1961 2022-09-28 14:17:56.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/templatetags/auth_utils.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      702 2022-09-13 09:39:41.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/urls.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     9869 2022-10-19 15:02:28.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/utils.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)    10171 2022-10-19 14:58:39.000000 django_dnoticias_auth-1.3rc9/dnoticias_auth/views.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)       38 2022-10-19 15:04:33.000000 django_dnoticias_auth-1.3rc9/setup.cfg
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      855 2022-10-19 15:03:33.000000 django_dnoticias_auth-1.3rc9/setup.py
```

### Comparing `django_dnoticias_auth-1.3rc8/LICENSE` & `django_dnoticias_auth-1.3rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `django_dnoticias_auth-1.3rc8/PKG-INFO` & `django_dnoticias_auth-1.3rc9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_dnoticias_auth
-Version: 1.3rc8
+Version: 1.3rc9
 Home-page: https://www.dnoticias.pt/
 Author: Pedro Mendes
 Author-email: pedro.trabalho.uma@gmail.com
 Maintainer: Nelson Gonçalves
 Maintainer-email: ngoncalves@dnoticias.pt
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `django_dnoticias_auth-1.3rc8/README.md` & `django_dnoticias_auth-1.3rc9/README.md`

 * *Files identical despite different names*

### Comparing `django_dnoticias_auth-1.3rc8/django_dnoticias_auth.egg-info/PKG-INFO` & `django_dnoticias_auth-1.3rc9/django_dnoticias_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dnoticias-auth
-Version: 1.3rc8
+Version: 1.3rc9
 Home-page: https://www.dnoticias.pt/
 Author: Pedro Mendes
 Author-email: pedro.trabalho.uma@gmail.com
 Maintainer: Nelson Gonçalves
 Maintainer-email: ngoncalves@dnoticias.pt
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `django_dnoticias_auth-1.3rc8/django_dnoticias_auth.egg-info/SOURCES.txt` & `django_dnoticias_auth-1.3rc9/django_dnoticias_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_dnoticias_auth-1.3rc8/dnoticias_auth/backends.py` & `django_dnoticias_auth-1.3rc9/dnoticias_auth/backends.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
                 
                 if user:
                     session_checker = SessionChecker(
                         user.email,
                         self.request.session.get("old_keycloak_session_id"),
                         keycloak_session_id
                     )
-                    session_checker.handle_event()
+                    session_checker.handle_event(SessionChecker.LOGIN)
                 return user
             except SuspiciousOperation as exc:
                 logger.warning('failed to get or create user: %s', exc)
                 return None
 
         return None
```

### Comparing `django_dnoticias_auth-1.3rc8/dnoticias_auth/forms.py` & `django_dnoticias_auth-1.3rc9/dnoticias_auth/forms.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_auth-1.3rc8/dnoticias_auth/middleware.py` & `django_dnoticias_auth-1.3rc9/dnoticias_auth/middleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,14 +325,14 @@
                 request.session["old_keycloak_session_value"] = keycloak_session_value
                 old_keycloak_session_value = keycloak_session_value
                 session_checker = SessionChecker(
                     request.user.email,
                     old_keycloak_session_value,
                     keycloak_session_value
                 )
-                session_checker.handle_event()
+                session_checker.handle_event(SessionChecker.UPDATE)
                 request.session.save()
 
             if old_keycloak_session_value:
                 response = set_cookie(old_keycloak_session_cookie, old_keycloak_session_value, response)
 
         return response
```

### Comparing `django_dnoticias_auth-1.3rc8/dnoticias_auth/migrations/0001_initial.py` & `django_dnoticias_auth-1.3rc9/dnoticias_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_auth-1.3rc8/dnoticias_auth/models.py` & `django_dnoticias_auth-1.3rc9/dnoticias_auth/models.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_auth-1.3rc8/dnoticias_auth/redis.py` & `django_dnoticias_auth-1.3rc9/dnoticias_auth/redis.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_auth-1.3rc8/dnoticias_auth/session.py` & `django_dnoticias_auth-1.3rc9/dnoticias_auth/session.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_auth-1.3rc8/dnoticias_auth/templates/authentication/app-data.html` & `django_dnoticias_auth-1.3rc9/dnoticias_auth/templates/authentication/app-data.html`

 * *Files identical despite different names*

### Comparing `django_dnoticias_auth-1.3rc8/dnoticias_auth/templates/authentication/password-recovery.html` & `django_dnoticias_auth-1.3rc9/dnoticias_auth/templates/authentication/password-recovery.html`

 * *Files identical despite different names*

### Comparing `django_dnoticias_auth-1.3rc8/dnoticias_auth/templates/authentication/silent-check-sso.html` & `django_dnoticias_auth-1.3rc9/dnoticias_auth/templates/authentication/silent-check-sso.html`

 * *Files identical despite different names*

### Comparing `django_dnoticias_auth-1.3rc8/dnoticias_auth/templatetags/auth_utils.py` & `django_dnoticias_auth-1.3rc9/dnoticias_auth/templatetags/auth_utils.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_auth-1.3rc8/dnoticias_auth/urls.py` & `django_dnoticias_auth-1.3rc9/dnoticias_auth/urls.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_auth-1.3rc8/dnoticias_auth/utils.py` & `django_dnoticias_auth-1.3rc9/dnoticias_auth/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 
 from django.http import HttpResponse, HttpResponseRedirect
 from django import VERSION as DJANGO_VERSION
 from django.conf import settings
 
 import requests
 from dnoticias_services.authentication.keycloak import (
+    delete_user_session as delete_session_kc,
     get_user_keycloak_info,
-    delete_user_session as delete_session_kc
 )
+from keycloak import KeycloakDeleteError
 
 from .redis import KeycloakSessionStorage, GenericSessionStorage
 from keycloak import KeycloakOpenID
 from . import cookies_consts
 
 logger = logging.getLogger(__name__)
 
@@ -178,14 +179,18 @@
     token = keycloak_client.refresh_token(refresh_token)
     expires_in = int(time()) + token.get('expires_in', 0)
 
     return token.get("access_token"), token.get("refresh_token"), expires_in
 
 
 class SessionChecker:
+    LOGIN = "login"
+    LOGOUT = "logout"
+    UPDATE = "update"
+
     def __init__(
         self,
         email: str,
         old_keycloak_session_id: str,
         keycloak_session_id: str,
     ):
         self.old_keycloak_session_id = old_keycloak_session_id
@@ -247,25 +252,35 @@
             response.raise_for_status()
         except:
             logger.exception("Failed to notify user about deleted session")
 
     def delete_oldest_session(self):
         information = self.get_information()
         oldest_session = min(information, key=lambda k: information[k]["created_at"])
+        information.pop(oldest_session, None)
 
         try:
-            information.pop(oldest_session)
             delete_user_sessions(oldest_session)
             delete_session_kc(oldest_session)
-        except KeyError:
-            logger.exception("Failed to delete oldest session %s", oldest_session)
+        except KeycloakDeleteError:
+            logger.debug("Failed to delete oldest session %s", oldest_session)
         else:
             self.notify_deleted_session(oldest_session)
 
         self.redis.save(json.dumps(information))
 
-    def handle_event(self):
-        self.update_session_information()
+    def delete_session(self):
+        information = self.get_information()
+        information.pop(self.keycloak_session_id, None)
+        self.redis.save(json.dumps(information))
 
-        if self.get_session_count() > self.get_user_max_sessions():
-            logger.info("Deleting old session for %s", self.email)
-            self.delete_oldest_session()
+    def handle_event(self, event: str):
+        if event == self.LOGIN:
+            logger.debug("Handling login event for %s", self.email)
+            self.update_session_information()
+
+            if self.get_session_count() > self.get_user_max_sessions():
+                logger.debug("Deleting old session for %s", self.email)
+                self.delete_oldest_session()
+        elif event == self.LOGOUT:
+            logger.debug("Handling logout event for %s", self.email)
+            self.delete_session()
```

### Comparing `django_dnoticias_auth-1.3rc8/dnoticias_auth/views.py` & `django_dnoticias_auth-1.3rc9/dnoticias_auth/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     OIDCLogoutView,
     OIDCAuthenticationCallbackView
 )
 
 from .forms import PasswordRecoveryDCSForm
 from . import cookies_consts
 from .utils import (
+    SessionChecker,
     set_cookie,
     delete_oidc_cookies,
     delete_user_sessions,
     refresh_keycloak_token,
 )
 
 logger = logging.getLogger(__name__)
@@ -84,14 +85,20 @@
         """
         keycloak_session_id = request.session.get("keycloak_session_id")
         cookies: dict = request.COOKIES
 
         if not keycloak_session_id:
             keycloak_session_id = cookies.get(cookies_consts.KC_SESSION_ID)
 
+        session_checker = SessionChecker(
+            request.user.email,
+            request.session.get("old_keycloak_session_id"),
+            keycloak_session_id,
+        )
+        session_checker.handle_event(SessionChecker.LOGOUT)
         delete_user_sessions(keycloak_session_id)
         super().post(request)
 
         return delete_oidc_cookies(self.redirect_url, request.COOKIES)
 
 
 class DnoticiasOIDCAuthenticationCallbackView(OIDCAuthenticationCallbackView):
```

### Comparing `django_dnoticias_auth-1.3rc8/setup.py` & `django_dnoticias_auth-1.3rc9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="django_dnoticias_auth",
-    version='1.3rc8',
+    version='1.3rc9',
     url="https://www.dnoticias.pt/",
     author="Pedro Mendes",
     author_email="pedro.trabalho.uma@gmail.com",
     maintainer="Nelson Gonçalves",
     maintainer_email="ngoncalves@dnoticias.pt",
     license="MIT",
     long_description=long_description,
```

