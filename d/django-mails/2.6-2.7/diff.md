# Comparing `tmp/django-mails-2.6.tar.gz` & `tmp/django-mails-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mails-2.6.tar", last modified: Thu Apr 20 10:44:05 2023, max compression
+gzip compressed data, was "django-mails-2.7.tar", last modified: Wed May  3 09:25:43 2023, max compression
```

## Comparing `django-mails-2.6.tar` & `django-mails-2.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-04-20 10:44:05.695774 django-mails-2.6/
--rw-rw-r--   0 manish    (1000) manish    (1000)     1076 2023-03-27 11:54:46.000000 django-mails-2.6/LICENSE
--rw-rw-r--   0 manish    (1000) manish    (1000)     2125 2023-04-20 10:44:05.695774 django-mails-2.6/PKG-INFO
--rw-rw-r--   0 manish    (1000) manish    (1000)     1312 2023-04-11 13:09:28.000000 django-mails-2.6/README.md
-drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-04-20 10:44:05.695774 django-mails-2.6/django_mails.egg-info/
--rw-rw-r--   0 manish    (1000) manish    (1000)     2125 2023-04-20 10:44:05.000000 django-mails-2.6/django_mails.egg-info/PKG-INFO
--rw-rw-r--   0 manish    (1000) manish    (1000)      457 2023-04-20 10:44:05.000000 django-mails-2.6/django_mails.egg-info/SOURCES.txt
--rw-rw-r--   0 manish    (1000) manish    (1000)        1 2023-04-20 10:44:05.000000 django-mails-2.6/django_mails.egg-info/dependency_links.txt
--rw-rw-r--   0 manish    (1000) manish    (1000)       97 2023-04-20 10:44:05.000000 django-mails-2.6/django_mails.egg-info/requires.txt
--rw-rw-r--   0 manish    (1000) manish    (1000)       14 2023-04-20 10:44:05.000000 django-mails-2.6/django_mails.egg-info/top_level.txt
-drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-04-20 10:44:05.695774 django-mails-2.6/email_service/
--rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-03-24 10:30:19.000000 django-mails-2.6/email_service/__init__.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      339 2023-04-11 12:57:14.000000 django-mails-2.6/email_service/admin.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      157 2023-04-11 12:56:41.000000 django-mails-2.6/email_service/apps.py
-drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-04-20 10:44:05.695774 django-mails-2.6/email_service/migrations/
--rw-rw-r--   0 manish    (1000) manish    (1000)     3361 2023-03-24 11:13:02.000000 django-mails-2.6/email_service/migrations/0001_initial.py
--rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-03-24 10:30:19.000000 django-mails-2.6/email_service/migrations/__init__.py
--rw-rw-r--   0 manish    (1000) manish    (1000)     2734 2023-03-27 07:58:51.000000 django-mails-2.6/email_service/models.py
--rw-rw-r--   0 manish    (1000) manish    (1000)     2568 2023-04-11 12:57:15.000000 django-mails-2.6/email_service/tests.py
--rw-rw-r--   0 manish    (1000) manish    (1000)     3246 2023-04-20 10:43:52.000000 django-mails-2.6/email_service/utils.py
--rw-rw-r--   0 manish    (1000) manish    (1000)       63 2023-03-24 10:30:19.000000 django-mails-2.6/email_service/views.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      966 2023-04-20 10:44:05.699774 django-mails-2.6/setup.cfg
--rw-rw-r--   0 manish    (1000) manish    (1000)       36 2023-03-28 03:53:50.000000 django-mails-2.6/setup.py
+drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-05-03 09:25:43.204150 django-mails-2.7/
+-rw-rw-r--   0 manish    (1000) manish    (1000)     1076 2023-03-27 11:54:46.000000 django-mails-2.7/LICENSE
+-rw-rw-r--   0 manish    (1000) manish    (1000)     2200 2023-05-03 09:25:43.204150 django-mails-2.7/PKG-INFO
+-rw-rw-r--   0 manish    (1000) manish    (1000)     1387 2023-05-03 09:25:28.000000 django-mails-2.7/README.md
+drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-05-03 09:25:43.200150 django-mails-2.7/django_mails.egg-info/
+-rw-rw-r--   0 manish    (1000) manish    (1000)     2200 2023-05-03 09:25:43.000000 django-mails-2.7/django_mails.egg-info/PKG-INFO
+-rw-rw-r--   0 manish    (1000) manish    (1000)      457 2023-05-03 09:25:43.000000 django-mails-2.7/django_mails.egg-info/SOURCES.txt
+-rw-rw-r--   0 manish    (1000) manish    (1000)        1 2023-05-03 09:25:43.000000 django-mails-2.7/django_mails.egg-info/dependency_links.txt
+-rw-rw-r--   0 manish    (1000) manish    (1000)       97 2023-05-03 09:25:43.000000 django-mails-2.7/django_mails.egg-info/requires.txt
+-rw-rw-r--   0 manish    (1000) manish    (1000)       14 2023-05-03 09:25:43.000000 django-mails-2.7/django_mails.egg-info/top_level.txt
+drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-05-03 09:25:43.200150 django-mails-2.7/email_service/
+-rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-03-24 10:30:19.000000 django-mails-2.7/email_service/__init__.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      355 2023-05-03 09:11:20.000000 django-mails-2.7/email_service/admin.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      173 2023-05-03 09:11:20.000000 django-mails-2.7/email_service/apps.py
+drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-05-03 09:25:43.200150 django-mails-2.7/email_service/migrations/
+-rw-rw-r--   0 manish    (1000) manish    (1000)     3361 2023-03-24 11:13:02.000000 django-mails-2.7/email_service/migrations/0001_initial.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-03-24 10:30:19.000000 django-mails-2.7/email_service/migrations/__init__.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)     2734 2023-03-27 07:58:51.000000 django-mails-2.7/email_service/models.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)     2584 2023-05-03 09:11:20.000000 django-mails-2.7/email_service/tests.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)     3773 2023-05-03 09:17:23.000000 django-mails-2.7/email_service/utils.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)       63 2023-03-24 10:30:19.000000 django-mails-2.7/email_service/views.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      966 2023-05-03 09:25:43.204150 django-mails-2.7/setup.cfg
+-rw-rw-r--   0 manish    (1000) manish    (1000)       36 2023-03-28 03:53:50.000000 django-mails-2.7/setup.py
```

### Comparing `django-mails-2.6/LICENSE` & `django-mails-2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mails-2.6/PKG-INFO` & `django-mails-2.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mails
-Version: 2.6
+Version: 2.7
 Summary: A Django Library to Send Simple/HTML Emails
 Home-page: https://www.example.com/
 Author: Harsh
 Author-email: harsh@hashtrust.in
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 4.1
@@ -45,14 +45,15 @@
     EMAIL_HOST_USER = ""
     EMAIL_HOST_PASSWORD = ""
     EMAIL_USE_TLS = True
     EMAIL_USE_SSL = False
     ```
 4. Add Templates path to your TEMPLATES in setting.py
 5. import method to send email ``from email_service.utils import send_custom_email``
+6. set ``LOGO_IMAGE_NAME`` variable in setting.py file to add logo in email
 
 Description
 -----------
 ```
 send_custom_email(
     recipient: List[str] | str,
     path: str | None = None,
@@ -65,8 +66,7 @@
 ```
 * recipient : List of Receivers emails
 * path : path to email html template under templates folder
 * template : Object of Template Model if exists (Optional)
 * template_prefix : html file name
 * context : context to replace variable name in template
 * subject : subject of email
-
```

### Comparing `django-mails-2.6/README.md` & `django-mails-2.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     EMAIL_HOST_USER = ""
     EMAIL_HOST_PASSWORD = ""
     EMAIL_USE_TLS = True
     EMAIL_USE_SSL = False
     ```
 4. Add Templates path to your TEMPLATES in setting.py
 5. import method to send email ``from email_service.utils import send_custom_email``
+6. set ``LOGO_IMAGE_NAME`` variable in setting.py file to add logo in email
 
 Description
 -----------
 ```
 send_custom_email(
     recipient: List[str] | str,
     path: str | None = None,
@@ -42,8 +43,7 @@
 ```
 * recipient : List of Receivers emails
 * path : path to email html template under templates folder
 * template : Object of Template Model if exists (Optional)
 * template_prefix : html file name
 * context : context to replace variable name in template
 * subject : subject of email
-
```

### Comparing `django-mails-2.6/django_mails.egg-info/PKG-INFO` & `django-mails-2.7/django_mails.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mails
-Version: 2.6
+Version: 2.7
 Summary: A Django Library to Send Simple/HTML Emails
 Home-page: https://www.example.com/
 Author: Harsh
 Author-email: harsh@hashtrust.in
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 4.1
@@ -45,14 +45,15 @@
     EMAIL_HOST_USER = ""
     EMAIL_HOST_PASSWORD = ""
     EMAIL_USE_TLS = True
     EMAIL_USE_SSL = False
     ```
 4. Add Templates path to your TEMPLATES in setting.py
 5. import method to send email ``from email_service.utils import send_custom_email``
+6. set ``LOGO_IMAGE_NAME`` variable in setting.py file to add logo in email
 
 Description
 -----------
 ```
 send_custom_email(
     recipient: List[str] | str,
     path: str | None = None,
@@ -65,8 +66,7 @@
 ```
 * recipient : List of Receivers emails
 * path : path to email html template under templates folder
 * template : Object of Template Model if exists (Optional)
 * template_prefix : html file name
 * context : context to replace variable name in template
 * subject : subject of email
-
```

### Comparing `django-mails-2.6/email_service/migrations/0001_initial.py` & `django-mails-2.7/email_service/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mails-2.6/email_service/models.py` & `django-mails-2.7/email_service/models.py`

 * *Files identical despite different names*

### Comparing `django-mails-2.6/email_service/tests.py` & `django-mails-2.7/email_service/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.test import TestCase
-from email_service.utils import send_custom_email
+from django_mail_app.email_service.utils import send_custom_email
 # Create your tests here.
 class TestEmail(TestCase):
 
     def setUp(self) -> None:
         self.recipients = ['harsh@hashtrust.in']
         self.path = "users"
         self.template = None
```

### Comparing `django-mails-2.6/email_service/utils.py` & `django-mails-2.7/email_service/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 from jinja2 import Template as JinjaTemplate
 
 # from django.utils.translation import gettext_lazy as _
 from django.conf import settings
 from django.core.mail.message import EmailMultiAlternatives
 from django.template.loader import render_to_string
 from django.utils import timezone
-
+from email.mime.image import MIMEImage
 logger = logging.getLogger("emails")
 
 
 def send_custom_email(
     recipient: List[str] | str,
     path: str | None = None,
     template: any = None,
     template_prefix: str | None = None,
     context: Dict = {},
     subject: str | None = None,
     body: str | None = None,
     attachement: any = None,
-    attachement_name : str | None = None
+    attachement_name : str | None = None,
+    enable_logo : bool = False
 ) -> None:
     from email_service.models import Email
 
     if not recipient or len(recipient) == 0:
         logger.error(
             "Please provide at least one recipient."
         )
@@ -71,14 +72,23 @@
         text_content = html2text.HTML2Text().handle(html_content)
         msg = EmailMultiAlternatives(
             subject or email_subject, text_content, from_email, to, bcc=[bcc_email]
         )
         msg.attach_alternative(html_content, "text/html")
         if attachement:
             msg.attach_file(f"{settings.BASE_DIR}/{attachement.url}")
+        
+        if enable_logo:
+            msg.content_subtype = 'html'
+            msg.mixed_subtype = 'related'
+            image_path = os.path.join(settings.BASE_DIR, f'/static/{settings.LOGO_IMAGE_NAME}')
+            with open(image_path, 'rb') as banner_image:
+                banner_image = MIMEImage(image_path.read())
+                banner_image.add_header('Content-ID', f'<{settings.LOGO_IMAGE_NAME}>')
+                msg.attach(banner_image)
         msg.send()
         return "Email Sent Successfully."
     except Exception as ex:
         logger.exception(
             f"""Caught exception {ex} while sending email with params:
             path-{path} template-{template_prefix}, recipient-{recipient},
             context-{context}, subject-{subject}, body-{body}"""
```

### Comparing `django-mails-2.6/setup.cfg` & `django-mails-2.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-mails
-version = 2.6
+version = 2.7
 description = A Django Library to Send Simple/HTML Emails
 readme = "README.md"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.example.com/
 author = Harsh
 author_email = harsh@hashtrust.in
```

