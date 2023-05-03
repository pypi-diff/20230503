# Comparing `tmp/django-mails-2.9.tar.gz` & `tmp/django-mails-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mails-2.9.tar", last modified: Wed May  3 09:40:27 2023, max compression
+gzip compressed data, was "django-mails-3.0.tar", last modified: Wed May  3 11:19:51 2023, max compression
```

## Comparing `django-mails-2.9.tar` & `django-mails-3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-05-03 09:40:27.721880 django-mails-2.9/
--rw-rw-r--   0 manish    (1000) manish    (1000)     1076 2023-03-27 11:54:46.000000 django-mails-2.9/LICENSE
--rw-rw-r--   0 manish    (1000) manish    (1000)     2200 2023-05-03 09:40:27.721880 django-mails-2.9/PKG-INFO
--rw-rw-r--   0 manish    (1000) manish    (1000)     1387 2023-05-03 09:25:28.000000 django-mails-2.9/README.md
-drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-05-03 09:40:27.721880 django-mails-2.9/django_mails.egg-info/
--rw-rw-r--   0 manish    (1000) manish    (1000)     2200 2023-05-03 09:40:27.000000 django-mails-2.9/django_mails.egg-info/PKG-INFO
--rw-rw-r--   0 manish    (1000) manish    (1000)      457 2023-05-03 09:40:27.000000 django-mails-2.9/django_mails.egg-info/SOURCES.txt
--rw-rw-r--   0 manish    (1000) manish    (1000)        1 2023-05-03 09:40:27.000000 django-mails-2.9/django_mails.egg-info/dependency_links.txt
--rw-rw-r--   0 manish    (1000) manish    (1000)       97 2023-05-03 09:40:27.000000 django-mails-2.9/django_mails.egg-info/requires.txt
--rw-rw-r--   0 manish    (1000) manish    (1000)       14 2023-05-03 09:40:27.000000 django-mails-2.9/django_mails.egg-info/top_level.txt
-drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-05-03 09:40:27.721880 django-mails-2.9/email_service/
--rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-03-24 10:30:19.000000 django-mails-2.9/email_service/__init__.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      339 2023-05-03 09:37:43.000000 django-mails-2.9/email_service/admin.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      157 2023-05-03 09:31:45.000000 django-mails-2.9/email_service/apps.py
-drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-05-03 09:40:27.721880 django-mails-2.9/email_service/migrations/
--rw-rw-r--   0 manish    (1000) manish    (1000)     3361 2023-03-24 11:13:02.000000 django-mails-2.9/email_service/migrations/0001_initial.py
--rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-03-24 10:30:19.000000 django-mails-2.9/email_service/migrations/__init__.py
--rw-rw-r--   0 manish    (1000) manish    (1000)     2734 2023-03-27 07:58:51.000000 django-mails-2.9/email_service/models.py
--rw-rw-r--   0 manish    (1000) manish    (1000)     2568 2023-05-03 09:32:11.000000 django-mails-2.9/email_service/tests.py
--rw-rw-r--   0 manish    (1000) manish    (1000)     3773 2023-05-03 09:17:23.000000 django-mails-2.9/email_service/utils.py
--rw-rw-r--   0 manish    (1000) manish    (1000)       63 2023-03-24 10:30:19.000000 django-mails-2.9/email_service/views.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      966 2023-05-03 09:40:27.725880 django-mails-2.9/setup.cfg
--rw-rw-r--   0 manish    (1000) manish    (1000)       36 2023-03-28 03:53:50.000000 django-mails-2.9/setup.py
+drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-05-03 11:19:51.115095 django-mails-3.0/
+-rw-rw-r--   0 manish    (1000) manish    (1000)     1076 2023-03-27 11:54:46.000000 django-mails-3.0/LICENSE
+-rw-rw-r--   0 manish    (1000) manish    (1000)     2500 2023-05-03 11:19:51.115095 django-mails-3.0/PKG-INFO
+-rw-rw-r--   0 manish    (1000) manish    (1000)     1687 2023-05-03 11:08:03.000000 django-mails-3.0/README.md
+drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-05-03 11:19:51.111095 django-mails-3.0/django_mails.egg-info/
+-rw-rw-r--   0 manish    (1000) manish    (1000)     2500 2023-05-03 11:19:51.000000 django-mails-3.0/django_mails.egg-info/PKG-INFO
+-rw-rw-r--   0 manish    (1000) manish    (1000)      457 2023-05-03 11:19:51.000000 django-mails-3.0/django_mails.egg-info/SOURCES.txt
+-rw-rw-r--   0 manish    (1000) manish    (1000)        1 2023-05-03 11:19:51.000000 django-mails-3.0/django_mails.egg-info/dependency_links.txt
+-rw-rw-r--   0 manish    (1000) manish    (1000)       97 2023-05-03 11:19:51.000000 django-mails-3.0/django_mails.egg-info/requires.txt
+-rw-rw-r--   0 manish    (1000) manish    (1000)       14 2023-05-03 11:19:51.000000 django-mails-3.0/django_mails.egg-info/top_level.txt
+drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-05-03 11:19:51.115095 django-mails-3.0/email_service/
+-rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-03-24 10:30:19.000000 django-mails-3.0/email_service/__init__.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      339 2023-05-03 09:37:43.000000 django-mails-3.0/email_service/admin.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      157 2023-05-03 09:31:45.000000 django-mails-3.0/email_service/apps.py
+drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-05-03 11:19:51.115095 django-mails-3.0/email_service/migrations/
+-rw-rw-r--   0 manish    (1000) manish    (1000)     3361 2023-03-24 11:13:02.000000 django-mails-3.0/email_service/migrations/0001_initial.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-03-24 10:30:19.000000 django-mails-3.0/email_service/migrations/__init__.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)     2734 2023-03-27 07:58:51.000000 django-mails-3.0/email_service/models.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)     2568 2023-05-03 09:32:11.000000 django-mails-3.0/email_service/tests.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)     3804 2023-05-03 11:00:15.000000 django-mails-3.0/email_service/utils.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)       63 2023-03-24 10:30:19.000000 django-mails-3.0/email_service/views.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      966 2023-05-03 11:19:51.115095 django-mails-3.0/setup.cfg
+-rw-rw-r--   0 manish    (1000) manish    (1000)       36 2023-03-28 03:53:50.000000 django-mails-3.0/setup.py
```

### Comparing `django-mails-2.9/LICENSE` & `django-mails-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mails-2.9/PKG-INFO` & `django-mails-3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mails
-Version: 2.9
+Version: 3.0
 Summary: A Django Library to Send Simple/HTML Emails
 Home-page: https://www.example.com/
 Author: Harsh
 Author-email: harsh@hashtrust.in
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 4.1
@@ -45,28 +45,34 @@
     EMAIL_HOST_USER = ""
     EMAIL_HOST_PASSWORD = ""
     EMAIL_USE_TLS = True
     EMAIL_USE_SSL = False
     ```
 4. Add Templates path to your TEMPLATES in setting.py
 5. import method to send email ``from email_service.utils import send_custom_email``
-6. set ``LOGO_IMAGE_NAME`` variable in setting.py file to add logo in email
+6. set ``LOGO_IMAGE_NAME`` variable in setting.py file to add logo in email (Name should include subfolder inside static folder)
 
 Description
 -----------
 ```
 send_custom_email(
     recipient: List[str] | str,
     path: str | None = None,
     template: any = None,
     template_prefix: str | None = None,
     context: Dict = {},
     subject: str | None = None,
     body: str | None = None,
+    attachement: any = None,
+    attachement_name : str | None = None,
+    enable_logo : bool = False
 )
 ```
 * recipient : List of Receivers emails
 * path : path to email html template under templates folder
 * template : Object of Template Model if exists (Optional)
 * template_prefix : html file name
 * context : context to replace variable name in template
 * subject : subject of email
+* attachement: attach file to send email as attachement
+* attachement_name : str | None = None,
+* enable_logo : set true to enable logo in email
```

### Comparing `django-mails-2.9/django_mails.egg-info/PKG-INFO` & `django-mails-3.0/django_mails.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mails
-Version: 2.9
+Version: 3.0
 Summary: A Django Library to Send Simple/HTML Emails
 Home-page: https://www.example.com/
 Author: Harsh
 Author-email: harsh@hashtrust.in
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 4.1
@@ -45,28 +45,34 @@
     EMAIL_HOST_USER = ""
     EMAIL_HOST_PASSWORD = ""
     EMAIL_USE_TLS = True
     EMAIL_USE_SSL = False
     ```
 4. Add Templates path to your TEMPLATES in setting.py
 5. import method to send email ``from email_service.utils import send_custom_email``
-6. set ``LOGO_IMAGE_NAME`` variable in setting.py file to add logo in email
+6. set ``LOGO_IMAGE_NAME`` variable in setting.py file to add logo in email (Name should include subfolder inside static folder)
 
 Description
 -----------
 ```
 send_custom_email(
     recipient: List[str] | str,
     path: str | None = None,
     template: any = None,
     template_prefix: str | None = None,
     context: Dict = {},
     subject: str | None = None,
     body: str | None = None,
+    attachement: any = None,
+    attachement_name : str | None = None,
+    enable_logo : bool = False
 )
 ```
 * recipient : List of Receivers emails
 * path : path to email html template under templates folder
 * template : Object of Template Model if exists (Optional)
 * template_prefix : html file name
 * context : context to replace variable name in template
 * subject : subject of email
+* attachement: attach file to send email as attachement
+* attachement_name : str | None = None,
+* enable_logo : set true to enable logo in email
```

### Comparing `django-mails-2.9/email_service/migrations/0001_initial.py` & `django-mails-3.0/email_service/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mails-2.9/email_service/models.py` & `django-mails-3.0/email_service/models.py`

 * *Files identical despite different names*

### Comparing `django-mails-2.9/email_service/tests.py` & `django-mails-3.0/email_service/tests.py`

 * *Files identical despite different names*

### Comparing `django-mails-2.9/email_service/utils.py` & `django-mails-3.0/email_service/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,17 +76,18 @@
         msg.attach_alternative(html_content, "text/html")
         if attachement:
             msg.attach_file(f"{settings.BASE_DIR}/{attachement.url}")
         
         if enable_logo:
             msg.content_subtype = 'html'
             msg.mixed_subtype = 'related'
-            image_path = os.path.join(settings.BASE_DIR, f'/static/{settings.LOGO_IMAGE_NAME}')
+            image_path = os.path.join(settings.BASE_DIR, f'static/{settings.LOGO_IMAGE_NAME}')
+            print(image_path)
             with open(image_path, 'rb') as banner_image:
-                banner_image = MIMEImage(image_path.read())
+                banner_image = MIMEImage(banner_image.read())
                 banner_image.add_header('Content-ID', f'<{settings.LOGO_IMAGE_NAME}>')
                 msg.attach(banner_image)
         msg.send()
         return "Email Sent Successfully."
     except Exception as ex:
         logger.exception(
             f"""Caught exception {ex} while sending email with params:
```

### Comparing `django-mails-2.9/setup.cfg` & `django-mails-3.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-mails
-version = 2.9
+version = 3.0
 description = A Django Library to Send Simple/HTML Emails
 readme = "README.md"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.example.com/
 author = Harsh
 author_email = harsh@hashtrust.in
```

