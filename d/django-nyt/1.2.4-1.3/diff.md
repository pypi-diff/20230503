# Comparing `tmp/django-nyt-1.2.4.tar.gz` & `tmp/django_nyt-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-nyt-1.2.4.tar", last modified: Thu Nov 10 23:09:18 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `django-nyt-1.2.4.tar` & `django_nyt-1.3.tar`

### file list

```diff
@@ -1,70 +1,41 @@
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-11-10 23:09:18.402744 django-nyt-1.2.4/
--rw-r--r--   0 balder    (1000) balder    (1000)    11325 2014-01-10 20:27:12.000000 django-nyt-1.2.4/LICENSE
--rw-rw-r--   0 balder    (1000) balder    (1000)      135 2022-10-14 21:39:06.000000 django-nyt-1.2.4/MANIFEST.in
--rw-rw-r--   0 balder    (1000) balder    (1000)     7990 2022-11-10 23:09:18.402744 django-nyt-1.2.4/PKG-INFO
--rw-rw-r--   0 balder    (1000) balder    (1000)     5181 2021-04-10 19:57:21.000000 django-nyt-1.2.4/README.rst
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-11-10 23:09:18.390743 django-nyt-1.2.4/django_nyt/
--rw-rw-r--   0 balder    (1000) balder    (1000)      110 2022-11-10 23:09:04.000000 django-nyt-1.2.4/django_nyt/__init__.py
--rw-r--r--   0 balder    (1000) balder    (1000)     1008 2018-07-29 15:22:39.000000 django-nyt-1.2.4/django_nyt/admin.py
--rw-rw-r--   0 balder    (1000) balder    (1000)      184 2018-02-19 12:51:23.000000 django-nyt-1.2.4/django_nyt/apps.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     1671 2018-02-19 12:51:23.000000 django-nyt-1.2.4/django_nyt/consumers.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     1721 2022-02-12 22:18:48.000000 django-nyt-1.2.4/django_nyt/decorators.py
--rw-rw-r--   0 balder    (1000) balder    (1000)      214 2018-02-19 12:51:23.000000 django-nyt-1.2.4/django_nyt/forms.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-11-10 23:09:18.382743 django-nyt-1.2.4/django_nyt/locale/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-11-10 23:09:18.378743 django-nyt-1.2.4/django_nyt/locale/da/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-11-10 23:09:18.390743 django-nyt-1.2.4/django_nyt/locale/da/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)     2431 2022-11-10 23:09:17.000000 django-nyt-1.2.4/django_nyt/locale/da/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)     3472 2014-07-15 14:17:09.000000 django-nyt-1.2.4/django_nyt/locale/da/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-11-10 23:09:18.378743 django-nyt-1.2.4/django_nyt/locale/de/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-11-10 23:09:18.394744 django-nyt-1.2.4/django_nyt/locale/de/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)     2172 2022-11-10 23:09:17.000000 django-nyt-1.2.4/django_nyt/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     3120 2014-01-10 20:27:27.000000 django-nyt-1.2.4/django_nyt/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-11-10 23:09:18.382743 django-nyt-1.2.4/django_nyt/locale/fi/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-11-10 23:09:18.394744 django-nyt-1.2.4/django_nyt/locale/fi/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)     2452 2022-11-10 23:09:17.000000 django-nyt-1.2.4/django_nyt/locale/fi/LC_MESSAGES/django.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)     3505 2014-10-27 22:47:50.000000 django-nyt-1.2.4/django_nyt/locale/fi/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-11-10 23:09:18.382743 django-nyt-1.2.4/django_nyt/locale/ru/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-11-10 23:09:18.394744 django-nyt-1.2.4/django_nyt/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)     2573 2022-11-10 23:09:17.000000 django-nyt-1.2.4/django_nyt/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     3520 2014-01-10 20:27:27.000000 django-nyt-1.2.4/django_nyt/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-11-10 23:09:18.394744 django-nyt-1.2.4/django_nyt/management/
--rw-r--r--   0 balder    (1000) balder    (1000)        0 2014-07-09 10:00:47.000000 django-nyt-1.2.4/django_nyt/management/__init__.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-11-10 23:09:18.394744 django-nyt-1.2.4/django_nyt/management/commands/
--rw-r--r--   0 balder    (1000) balder    (1000)        0 2014-07-09 10:00:48.000000 django-nyt-1.2.4/django_nyt/management/commands/__init__.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     8826 2020-10-30 19:13:32.000000 django-nyt-1.2.4/django_nyt/management/commands/notifymail.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-11-10 23:09:18.398743 django-nyt-1.2.4/django_nyt/migrations/
--rw-r--r--   0 balder    (1000) balder    (1000)     1267 2018-07-29 15:22:39.000000 django-nyt-1.2.4/django_nyt/migrations/0001_initial.py
--rw-r--r--   0 balder    (1000) balder    (1000)     2855 2018-07-29 15:22:39.000000 django-nyt-1.2.4/django_nyt/migrations/0002_notification_settings.py
--rw-r--r--   0 balder    (1000) balder    (1000)     1930 2018-07-29 15:22:39.000000 django-nyt-1.2.4/django_nyt/migrations/0003_subscription.py
--rw-r--r--   0 balder    (1000) balder    (1000)      593 2018-07-29 15:22:39.000000 django-nyt-1.2.4/django_nyt/migrations/0004_notification_subscription.py
--rw-r--r--   0 balder    (1000) balder    (1000)     2608 2018-07-29 15:22:39.000000 django-nyt-1.2.4/django_nyt/migrations/0005__v_0_9_2.py
--rw-r--r--   0 balder    (1000) balder    (1000)      499 2018-07-29 15:22:39.000000 django-nyt-1.2.4/django_nyt/migrations/0006_auto_20141229_1630.py
--rw-r--r--   0 balder    (1000) balder    (1000)      650 2018-07-29 15:22:39.000000 django-nyt-1.2.4/django_nyt/migrations/0007_add_modified_and_default_settings.py
--rw-r--r--   0 balder    (1000) balder    (1000)     1081 2018-07-29 15:22:39.000000 django-nyt-1.2.4/django_nyt/migrations/0008_auto_20161023_1641.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     1080 2022-02-12 22:53:52.000000 django-nyt-1.2.4/django_nyt/migrations/0009_alter_notification_subscription_and_more.py
--rw-rw-r--   0 balder    (1000) balder    (1000)        0 2014-07-09 10:00:48.000000 django-nyt-1.2.4/django_nyt/migrations/__init__.py
--rw-r--r--   0 balder    (1000) balder    (1000)     9698 2020-02-16 10:53:43.000000 django-nyt-1.2.4/django_nyt/models.py
--rw-rw-r--   0 balder    (1000) balder    (1000)      269 2018-02-19 12:51:23.000000 django-nyt-1.2.4/django_nyt/routing.py
--rw-r--r--   0 balder    (1000) balder    (1000)     2551 2019-05-09 09:59:26.000000 django-nyt-1.2.4/django_nyt/settings.py
--rw-r--r--   0 balder    (1000) balder    (1000)      639 2018-07-29 15:22:39.000000 django-nyt-1.2.4/django_nyt/subscribers.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-11-10 23:09:18.382743 django-nyt-1.2.4/django_nyt/templates/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-11-10 23:09:18.398743 django-nyt-1.2.4/django_nyt/templates/emails/
--rw-rw-r--   0 balder    (1000) balder    (1000)      436 2016-02-29 15:17:36.000000 django-nyt-1.2.4/django_nyt/templates/emails/notification_email_message.txt
--rw-r--r--   0 balder    (1000) balder    (1000)      114 2014-01-10 20:27:27.000000 django-nyt-1.2.4/django_nyt/templates/emails/notification_email_subject.txt
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-11-10 23:09:18.402744 django-nyt-1.2.4/django_nyt/tests/
--rw-r--r--   0 balder    (1000) balder    (1000)      107 2018-07-29 15:22:39.000000 django-nyt-1.2.4/django_nyt/tests/__init__.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     1826 2020-10-30 19:13:32.000000 django-nyt-1.2.4/django_nyt/tests/test_basic.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     1443 2022-02-12 22:18:48.000000 django-nyt-1.2.4/django_nyt/tests/test_management.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     1185 2020-10-30 19:13:32.000000 django-nyt-1.2.4/django_nyt/tests/test_views.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     1101 2022-02-12 22:18:48.000000 django-nyt-1.2.4/django_nyt/urls.py
--rw-r--r--   0 balder    (1000) balder    (1000)     3112 2020-01-07 00:36:13.000000 django-nyt-1.2.4/django_nyt/utils.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     3607 2022-02-12 15:45:40.000000 django-nyt-1.2.4/django_nyt/views.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2022-11-10 23:09:18.390743 django-nyt-1.2.4/django_nyt.egg-info/
--rw-rw-r--   0 balder    (1000) balder    (1000)     7990 2022-11-10 23:09:18.000000 django-nyt-1.2.4/django_nyt.egg-info/PKG-INFO
--rw-rw-r--   0 balder    (1000) balder    (1000)     1739 2022-11-10 23:09:18.000000 django-nyt-1.2.4/django_nyt.egg-info/SOURCES.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)        1 2022-11-10 23:09:18.000000 django-nyt-1.2.4/django_nyt.egg-info/dependency_links.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)        1 2022-11-10 23:09:18.000000 django-nyt-1.2.4/django_nyt.egg-info/not-zip-safe
--rw-rw-r--   0 balder    (1000) balder    (1000)       17 2022-11-10 23:09:18.000000 django-nyt-1.2.4/django_nyt.egg-info/requires.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)       11 2022-11-10 23:09:18.000000 django-nyt-1.2.4/django_nyt.egg-info/top_level.txt
--rw-r--r--   0 balder    (1000) balder    (1000)      411 2022-11-10 23:09:18.402744 django-nyt-1.2.4/setup.cfg
--rw-rw-r--   0 balder    (1000) balder    (1000)     2094 2022-11-10 23:09:04.000000 django-nyt-1.2.4/setup.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/__init__.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/admin.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/apps.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/consumers.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/decorators.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/forms.py
+-rw-r--r--   0        0        0     9479 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/models.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/routing.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/settings.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/subscribers.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/urls.py
+-rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/utils.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/views.py
+-rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/locale/da/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/locale/fi/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/management/commands/__init__.py
+-rw-r--r--   0        0        0     8615 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/management/commands/notifymail.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/migrations/0001_initial.py
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/migrations/0002_notification_settings.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/migrations/0003_subscription.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/migrations/0004_notification_subscription.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/migrations/0005__v_0_9_2.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/migrations/0006_auto_20141229_1630.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/migrations/0007_add_modified_and_default_settings.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/migrations/0008_auto_20161023_1641.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/migrations/0009_alter_notification_subscription_and_more.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/migrations/__init__.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/templates/emails/notification_email_message.txt
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/templates/emails/notification_email_subject.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/tests/__init__.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/tests/test_basic.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/tests/test_management.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 django_nyt-1.3/django_nyt/tests/test_views.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 django_nyt-1.3/.gitignore
+-rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 django_nyt-1.3/LICENSE
+-rw-r--r--   0        0        0     5066 2020-02-02 00:00:00.000000 django_nyt-1.3/README.rst
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 django_nyt-1.3/pyproject.toml
+-rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 django_nyt-1.3/PKG-INFO
```

### Comparing `django-nyt-1.2.4/LICENSE` & `django_nyt-1.3/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -195,8 +195,7 @@
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
-
```

### Comparing `django-nyt-1.2.4/README.rst` & `django_nyt-1.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -35,21 +35,14 @@
 Channels (django-channels)
 --------------------------
 
 Starting from django-nyt 1.0, support for the upcoming
 `channels <https://channels.readthedocs.io/>`_ has been added together with
 Django 1.9 and 1.10 support.
 
-In order to install the prerelease, use an extra flag for pip:
-
-.. code:: bash
-
-    pip install django-nyt --pre
-
-
 Docs
 ----
 
 https://django-nyt.readthedocs.io/en/latest/
 
 
 Why should you do this?
```

### Comparing `django-nyt-1.2.4/django_nyt/admin.py` & `django_nyt-1.3/django_nyt/admin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 from django.contrib import admin
 from django.utils.translation import gettext as _
-from django_nyt import models, settings
+
+from django_nyt import models
+from django_nyt import settings
 
 
 class SettingsAdmin(admin.ModelAdmin):
-    raw_id_fields = ('user',)
-    list_display = ('user', 'interval',)
+    raw_id_fields = ("user",)
+    list_display = (
+        "user",
+        "interval",
+    )
 
 
 class SubscriptionAdmin(admin.ModelAdmin):
-    raw_id_fields = ('settings',)
-    list_display = ('display_user', 'notification_type', 'display_interval',)
+    raw_id_fields = ("settings",)
+    list_display = (
+        "display_user",
+        "notification_type",
+        "display_interval",
+    )
 
     def display_user(self, instance):
         return instance.settings.user
+
     display_user.short_description = _("user")
 
     def display_interval(self, instance):
         return instance.settings.interval
+
     display_interval.short_description = _("interval")
 
 
 class NotificationAdmin(admin.ModelAdmin):
 
-    raw_id_fields = ('user', 'subscription')
+    raw_id_fields = ("user", "subscription")
 
 
 if settings.ENABLE_ADMIN:
     admin.site.register(models.NotificationType)
     admin.site.register(models.Notification, NotificationAdmin)
     admin.site.register(models.Settings, SettingsAdmin)
     admin.site.register(models.Subscription, SubscriptionAdmin)
```

### Comparing `django-nyt-1.2.4/django_nyt/consumers.py` & `django_nyt-1.3/django_nyt/consumers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import logging
 
 from channels import Group
-from channels.auth import channel_session_user, channel_session_user_from_http
+from channels.auth import channel_session_user
+from channels.auth import channel_session_user_from_http
 
-from . import models, settings
+from . import models
+from . import settings
 
 logger = logging.getLogger(__name__)
 
 
 def get_subscriptions(message):
     """
     :return: Subscription query for a given message's user
@@ -50,8 +52,8 @@
 
 def ws_receive(message):
     """
     Receives messages, this is currently just for debugging purposes as there
     is no communication API for the websockets.
     """
     logger.debug("Received a message, responding with a non-API message")
-    message.reply_channel.send({'text': 'OK'})
+    message.reply_channel.send({"text": "OK"})
```

### Comparing `django-nyt-1.2.4/django_nyt/decorators.py` & `django_nyt-1.3/django_nyt/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,60 @@
 import json
 from functools import wraps
 
-import django_nyt
 from django.contrib.auth.decorators import login_required
 from django.http import HttpResponse
 
+import django_nyt
+
 
 def disable_notify(f):
     """Disable notifications. Example:
 
     @disable_notify
     def your_function():
         notify("no one will be notified", ...)
     """
+
     @wraps(f)
     def wrapper(request, *args, **kwargs):
         django_nyt._disable_notifications = True
         response = f(request, *args, **kwargs)
         django_nyt._disable_notifications = False
         return response
+
     return wrapper
 
 
 def login_required_ajax(f):
     """Similar to login_required. But if the request is an ajax request, then
     it returns an error in json with a 403 status code."""
 
     @wraps(f)
     def wrapper(request, *args, **kwargs):
-        if request.headers.get('x-requested-with') == 'XMLHttpRequest':
+        if request.headers.get("x-requested-with") == "XMLHttpRequest":
             if not request.user or not request.user.is_authenticated:
-                return json_view(lambda *a,
-                                 **kw: {'error': 'not logged in'})(request,
-                                                                   status=403)
+                return json_view(lambda *a, **kw: {"error": "not logged in"})(
+                    request, status=403
+                )
             return f(request, *args, **kwargs)
         else:
             return login_required(f)(request, *args, **kwargs)
+
     return wrapper
 
 
 def data2jsonresponse(data, **kwargs):
     json_data = json.dumps(data, ensure_ascii=False)
-    status = kwargs.get('status', 200)
-    response = HttpResponse(content_type='application/json', status=status)
+    status = kwargs.get("status", 200)
+    response = HttpResponse(content_type="application/json", status=status)
     response.write(json_data)
     return response
 
 
 def json_view(f):
     @wraps(f)
     def wrapper(request, *args, **kwargs):
         data = f(request, *args, **kwargs)
         return data2jsonresponse(data, **kwargs)
+
     return wrapper
```

### Comparing `django-nyt-1.2.4/django_nyt/locale/da/LC_MESSAGES/django.po` & `django_nyt-1.3/django_nyt/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-nyt-1.2.4/django_nyt/locale/de/LC_MESSAGES/django.po` & `django_nyt-1.3/django_nyt/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-nyt-1.2.4/django_nyt/locale/fi/LC_MESSAGES/django.po` & `django_nyt-1.3/django_nyt/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-nyt-1.2.4/django_nyt/locale/ru/LC_MESSAGES/django.po` & `django_nyt-1.3/django_nyt/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-nyt-1.2.4/django_nyt/management/commands/notifymail.py` & `django_nyt-1.3/django_nyt/management/commands/notifymail.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,112 +21,110 @@
 SLEEP_TIME = 120
 
 
 class Command(BaseCommand):
     can_import_settings = True
     # @ReservedAssignment
     help = (
-        'Sends notification emails to subscribed users taking into account '
-        'the subscription interval'
+        "Sends notification emails to subscribed users taking into account "
+        "the subscription interval"
     )
 
     def add_arguments(self, parser):
         parser.add_argument(
-            '--daemon', '-d',
-            action='store_true',
-            dest='daemon',
-            help='Go to daemon mode and exit'
+            "--daemon",
+            "-d",
+            action="store_true",
+            dest="daemon",
+            help="Go to daemon mode and exit",
         )
         parser.add_argument(
-            '--cron', '-c',
-            action='store_true',
-            dest='cron',
-            help='Do not loop, just send out emails once and exit'
+            "--cron",
+            "-c",
+            action="store_true",
+            dest="cron",
+            help="Do not loop, just send out emails once and exit",
         )
         parser.add_argument(
-            '--pid-file',
-            action='store',
-            dest='pid',
-            help='Where to write PID before exiting',
-            default='/tmp/nyt_daemon.pid'
+            "--pid-file",
+            action="store",
+            dest="pid",
+            help="Where to write PID before exiting",
+            default="/tmp/nyt_daemon.pid",
         )
         parser.add_argument(
-            '--log-file',
-            action='store',
-            dest='log',
-            help='Where daemon should write its log',
-            default='/tmp/nyt_daemon.log'
+            "--log-file",
+            action="store",
+            dest="log",
+            help="Where daemon should write its log",
+            default="/tmp/nyt_daemon.log",
         )
         parser.add_argument(
-            '--no-sys-exit',
-            action='store_true',
-            dest='no_sys_exit',
-            help='Skip sys-exit after forking daemon (for testing purposes)'
+            "--no-sys-exit",
+            action="store_true",
+            dest="no_sys_exit",
+            help="Skip sys-exit after forking daemon (for testing purposes)",
         )
         parser.add_argument(
-            '--daemon-sleep-interval',
-            action='store',
-            dest='sleep_time',
-            help='Minimum sleep between each polling of the database.',
-            default=SLEEP_TIME
+            "--daemon-sleep-interval",
+            action="store",
+            dest="sleep_time",
+            help="Minimum sleep between each polling of the database.",
+            default=SLEEP_TIME,
         )
 
     def _send_user_notifications(self, context, connection):
         subject = _(nyt_settings.EMAIL_SUBJECT)
 
-        message = render_to_string(
-            'emails/notification_email_message.txt',
-            context
-        )
+        message = render_to_string("emails/notification_email_message.txt", context)
         email = mail.EmailMessage(
-            subject, message, nyt_settings.EMAIL_SENDER,
-            [context['user'].email], connection=connection
+            subject,
+            message,
+            nyt_settings.EMAIL_SENDER,
+            [context["user"].email],
+            connection=connection,
         )
-        self.logger.info("Sending to: %s" % context['user'].email)
+        self.logger.info("Sending to: %s" % context["user"].email)
         email.send(fail_silently=False)
 
     def _daemonize(self):
         self.logger.info("Daemon mode enabled, forking")
         try:
             fpid = os.fork()
             if fpid > 0:
                 # Running as daemon now. PID is fpid
                 self.logger.info("PID: %s" % str(fpid))
-                with open(self.options['pid'], "w") as pid_file:
+                with open(self.options["pid"], "w") as pid_file:
                     pid_file.write(str(fpid))
-                if not self.options['no_sys_exit']:
+                if not self.options["no_sys_exit"]:
                     sys.exit(0)
         except OSError as e:
-            sys.stderr.write(
-                "fork failed: %d (%s)\n" %
-                (e.errno, e.strerror))
+            sys.stderr.write("fork failed: %d (%s)\n" % (e.errno, e.strerror))
             sys.exit(1)
 
     def handle(self, *args, **options):  # noqa: max-complexity=12
         # activate the language
         activate(settings.LANGUAGE_CODE)
 
-        options.setdefault('daemon', False)
-        options.setdefault('cron', False)
-        options.setdefault('no_sys_exit', False)
+        options.setdefault("daemon", False)
+        options.setdefault("cron", False)
+        options.setdefault("no_sys_exit", False)
 
         self.options = options
 
-        daemon = options['daemon']
-        cron = options['cron']
+        daemon = options["daemon"]
+        cron = options["cron"]
 
-        assert not (daemon and cron), (
-            "You cannot both choose cron and daemon options"
-        )
+        assert not (daemon and cron), "You cannot both choose cron and daemon options"
 
-        self.logger = logging.getLogger('django_nyt')
+        self.logger = logging.getLogger("django_nyt")
 
         if not self.logger.handlers:
             if daemon:
-                handler = logging.FileHandler(filename=options['log'])
+                handler = logging.FileHandler(filename=options["log"])
             else:
                 handler = logging.StreamHandler(self.stdout)
             self.logger.addHandler(handler)
             self.logger.setLevel(logging.INFO)
 
         self.logger.info("Starting django_nyt e-mail dispatcher")
 
@@ -144,129 +142,122 @@
         if cron:
             self.send_mails(connection)
             return
 
         if not daemon:
             print("Entering send-loop, CTRL+C to exit")
         try:
-            self.send_loop(connection, int(options['sleep_time']))
+            self.send_loop(connection, int(options["sleep_time"]))
         except KeyboardInterrupt:
             print("\nQuitting...")
 
         # deactivate the language
         deactivate()
 
     def send_loop(self, connection, sleep_time):
 
         # This could be /improved by looking up the last notified person
         last_sent = None
 
         while True:
 
             started_sending_at = datetime.now()
-            self.logger.info(
-                "Starting send loop at %s" %
-                str(started_sending_at))
+            self.logger.info("Starting send loop at %s" % str(started_sending_at))
             if last_sent:
                 user_settings = models.Settings.objects.filter(
-                    interval__lte=(
-                        (started_sending_at - last_sent).seconds // 60) // 60
-                ).order_by('user')
+                    interval__lte=((started_sending_at - last_sent).seconds // 60) // 60
+                ).order_by("user")
             else:
                 user_settings = None
 
             self.send_mails(
-                connection,
-                last_sent=last_sent,
-                user_settings=user_settings
+                connection, last_sent=last_sent, user_settings=user_settings
             )
 
             connection.close()
             last_sent = datetime.now()
             elapsed_seconds = (last_sent - started_sending_at).seconds
             time.sleep(
                 max(
                     (min(nyt_settings.INTERVALS)[0] - elapsed_seconds) * 60,
                     sleep_time,
-                    0
+                    0,
                 )
             )
 
     def _send_batch(self, context, connection, setting):
         """
         Loops through emails in a list of notifications and tries to send
         to each recepient
 
         """
         # STMP connection send loop
-        notifications = context['notifications']
+        notifications = context["notifications"]
 
-        if len(context['notifications']) == 0:
+        if len(context["notifications"]) == 0:
             return
 
         while True:
             try:
                 self._send_user_notifications(context, connection)
                 for n in notifications:
                     n.is_emailed = True
                     n.save()
                 break
             except smtplib.SMTPSenderRefused:
                 self.logger.error(
-                    (
-                        "E-mail refused by SMTP server ({}), "
-                        "skipping!"
-                    ).format(setting.user.email))
+                    ("E-mail refused by SMTP server ({}), " "skipping!").format(
+                        setting.user.email
+                    )
+                )
                 continue
             except smtplib.SMTPException as e:
                 self.logger.error(
                     (
                         "You have an error with your SMTP server "
                         "connection, error is: {}"
-                    ).format(e))
+                    ).format(e)
+                )
                 self.logger.error("Sleeping for 30s then retrying...")
                 time.sleep(30)
             except Exception as e:
                 self.logger.error(
-                    (
-                        "Unhandled exception while sending, giving "
-                        "up: {}"
-                    ).format(e))
+                    ("Unhandled exception while sending, giving " "up: {}").format(e)
+                )
                 raise
 
     def send_mails(self, connection, last_sent=None, user_settings=None):
         """
         Does the lookups and sends out email digests to anyone who has them
         due.
         """
 
         self.logger.debug("Entering send_mails()")
 
         connection.open()
 
         if not user_settings:
-            user_settings = models.Settings.objects.all().order_by('user')
+            user_settings = models.Settings.objects.all().order_by("user")
 
-        context = {'user': None,
-                   'username': None,
-                   'notifications': None,
-                   'digest': None,
-                   'site': Site.objects.get_current()}
+        context = {
+            "user": None,
+            "username": None,
+            "notifications": None,
+            "digest": None,
+            "site": Site.objects.get_current(),
+        }
 
         for setting in user_settings:
-            context['user'] = setting.user
-            context['username'] = getattr(
-                setting.user, setting.user.USERNAME_FIELD)
+            context["user"] = setting.user
+            context["username"] = getattr(setting.user, setting.user.USERNAME_FIELD)
             # Which notifications are remaining for the user's settings
-            context['notifications'] = []
+            context["notifications"] = []
             # get the index of the tuple corresponding to the interval and
             # get the string name
-            idx = [y[0] for y in nyt_settings.INTERVALS].index(
-                setting.interval)
-            context['digest'] = nyt_settings.INTERVALS[idx][1]
+            idx = [y[0] for y in nyt_settings.INTERVALS].index(setting.interval)
+            context["digest"] = nyt_settings.INTERVALS[idx][1]
             for subscription in setting.subscription_set.filter(
-                send_emails=True,
-                latest__is_emailed=False
+                send_emails=True, latest__is_emailed=False
             ):
-                context['notifications'].append(subscription.latest)
+                context["notifications"].append(subscription.latest)
 
             self._send_batch(context, connection, setting)
```

### Comparing `django-nyt-1.2.4/django_nyt/migrations/0001_initial.py` & `django_nyt-1.3/django_nyt/migrations/0001_initial.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,52 @@
-from django.db import migrations, models
+from django.db import migrations
+from django.db import models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('contenttypes', '__first__'),
+        ("contenttypes", "__first__"),
     ]
 
     operations = [
         migrations.CreateModel(
-            name='NotificationType',
+            name="NotificationType",
             fields=[
-                ('key',
-                 models.CharField(
-                     verbose_name='unique key',
-                     serialize=False,
-                     max_length=128,
-                     primary_key=True,
-                     unique=True)),
-                ('label',
-                 models.CharField(
-                     verbose_name='verbose name',
-                     null=True,
-                     max_length=128,
-                     blank=True)),
-                ('content_type',
-                 models.ForeignKey(
-                     to_field='id',
-                     to='contenttypes.ContentType',
-                     blank=True,
-                     null=True, on_delete=models.CASCADE)),
+                (
+                    "key",
+                    models.CharField(
+                        verbose_name="unique key",
+                        serialize=False,
+                        max_length=128,
+                        primary_key=True,
+                        unique=True,
+                    ),
+                ),
+                (
+                    "label",
+                    models.CharField(
+                        verbose_name="verbose name",
+                        null=True,
+                        max_length=128,
+                        blank=True,
+                    ),
+                ),
+                (
+                    "content_type",
+                    models.ForeignKey(
+                        to_field="id",
+                        to="contenttypes.ContentType",
+                        blank=True,
+                        null=True,
+                        on_delete=models.CASCADE,
+                    ),
+                ),
             ],
             options={
-                'verbose_name': 'type',
-                'db_table': 'nyt_notificationtype',
-                            'verbose_name_plural': 'types',
+                "verbose_name": "type",
+                "db_table": "nyt_notificationtype",
+                "verbose_name_plural": "types",
             },
-            bases=(
-                models.Model,
-            ),
+            bases=(models.Model,),
         ),
     ]
```

### Comparing `django-nyt-1.2.4/django_nyt/migrations/0003_subscription.py` & `django_nyt-1.3/django_nyt/migrations/0003_subscription.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,68 @@
-from django.db import migrations, models
+from django.db import migrations
+from django.db import models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('django_nyt', '0002_notification_settings'),
+        ("django_nyt", "0002_notification_settings"),
     ]
 
     operations = [
         migrations.CreateModel(
-            name='Subscription', fields=[
+            name="Subscription",
+            fields=[
                 (
-                    'id',
+                    "id",
                     models.AutoField(
-                        auto_created=True, verbose_name='ID', serialize=False, primary_key=True
-                    )
-                ), (
-                    'settings',
+                        auto_created=True,
+                        verbose_name="ID",
+                        serialize=False,
+                        primary_key=True,
+                    ),
+                ),
+                (
+                    "settings",
                     models.ForeignKey(
-                        to_field='id', to='django_nyt.Settings', on_delete=models.CASCADE
-                    )
-                ), (
-                    'notification_type',
+                        to_field="id",
+                        to="django_nyt.Settings",
+                        on_delete=models.CASCADE,
+                    ),
+                ),
+                (
+                    "notification_type",
                     models.ForeignKey(
-                        to_field='key', to='django_nyt.NotificationType', on_delete=models.CASCADE
-                    )
-                ), (
-                    'object_id',
+                        to_field="key",
+                        to="django_nyt.NotificationType",
+                        on_delete=models.CASCADE,
+                    ),
+                ),
+                (
+                    "object_id",
                     models.CharField(
-                        help_text='Leave this blank to subscribe to any kind of object',
+                        help_text="Leave this blank to subscribe to any kind of object",
                         null=True,
                         max_length=64,
-                        blank=True
-                    )
-                ), (
-                    'send_emails', models.BooleanField(
-                        default=True
-                    )
-                ), (
-                    'latest',
+                        blank=True,
+                    ),
+                ),
+                ("send_emails", models.BooleanField(default=True)),
+                (
+                    "latest",
                     models.ForeignKey(
-                        to_field='id',
-                        to='django_nyt.Notification',
+                        to_field="id",
+                        to="django_nyt.Notification",
                         blank=True,
                         null=True,
-                        on_delete=models.CASCADE
-                    )
+                        on_delete=models.CASCADE,
+                    ),
                 ),
             ],
             options={
-                'verbose_name': 'subscription', 'db_table': 'nyt_subscription', 'verbose_name_plural': 'subscriptions',
+                "verbose_name": "subscription",
+                "db_table": "nyt_subscription",
+                "verbose_name_plural": "subscriptions",
             },
-            bases=(
-                models.Model,
-            ),
+            bases=(models.Model,),
         ),
     ]
```

### Comparing `django-nyt-1.2.4/django_nyt/migrations/0004_notification_subscription.py` & `django_nyt-1.3/django_nyt/migrations/0004_notification_subscription.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import django.db.models.deletion
-from django.db import migrations, models
+from django.db import migrations
+from django.db import models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('django_nyt', '0003_subscription'),
+        ("django_nyt", "0003_subscription"),
     ]
 
     operations = [
         migrations.AddField(
-            model_name='notification',
-            name='subscription',
+            model_name="notification",
+            name="subscription",
             field=models.ForeignKey(
-                to_field='id',
-                to='django_nyt.Subscription',
+                to_field="id",
+                to="django_nyt.Subscription",
                 blank=True,
                 on_delete=django.db.models.deletion.SET_NULL,
-                null=True),
+                null=True,
+            ),
             preserve_default=True,
         ),
     ]
```

### Comparing `django-nyt-1.2.4/django_nyt/migrations/0005__v_0_9_2.py` & `django_nyt-1.3/django_nyt/migrations/0002_notification_settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,92 @@
-import django.db.models.deletion
 from django.conf import settings
-from django.db import migrations, models
+from django.db import migrations
+from django.db import models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
-        ('django_nyt', '0004_notification_subscription'),
+        ("django_nyt", "0001_initial"),
     ]
 
     operations = [
-        migrations.AddField(
-            model_name='notification',
-            name='user',
-            field=models.ForeignKey(verbose_name='user', to_field='id', blank=True, to=settings.AUTH_USER_MODEL, null=True, on_delete=models.CASCADE),
-            preserve_default=True,
-        ),
-        migrations.AlterField(
-            model_name='subscription',
-            name='latest',
-            field=models.ForeignKey(verbose_name='latest notification', to_field='id', blank=True, to='django_nyt.Notification', null=True, on_delete=models.CASCADE),
-        ),
-        migrations.AlterField(
-            model_name='settings',
-            name='user',
-            field=models.ForeignKey(to=settings.AUTH_USER_MODEL, to_field='id', verbose_name='user', on_delete=models.CASCADE),
-        ),
-        migrations.AlterField(
-            model_name='subscription',
-            name='settings',
-            field=models.ForeignKey(to='django_nyt.Settings', to_field='id', verbose_name='settings', on_delete=models.CASCADE),
-        ),
-        migrations.AlterField(
-            model_name='subscription',
-            name='notification_type',
-            field=models.ForeignKey(to='django_nyt.NotificationType', to_field='key', verbose_name='notification type', on_delete=models.CASCADE),
-        ),
-        migrations.AlterField(
-            model_name='notificationtype',
-            name='label',
-            field=models.CharField(max_length=128, null=True, verbose_name='optional label', blank=True),
-        ),
-        migrations.AlterField(
-            model_name='subscription',
-            name='object_id',
-            field=models.CharField(help_text='Leave this blank to subscribe to any kind of object', max_length=64, null=True, verbose_name='object ID', blank=True),
-        ),
-        migrations.AlterField(
-            model_name='subscription',
-            name='send_emails',
-            field=models.BooleanField(default=True, verbose_name='send emails'),
-        ),
-        migrations.AlterField(
-            model_name='notification',
-            name='subscription',
-            field=models.ForeignKey(on_delete=django.db.models.deletion.SET_NULL, verbose_name='subscription', to_field='id', blank=True, to='django_nyt.Subscription', null=True),
+        migrations.CreateModel(
+            name="Settings",
+            fields=[
+                (
+                    "id",
+                    models.AutoField(
+                        auto_created=True,
+                        verbose_name="ID",
+                        serialize=False,
+                        primary_key=True,
+                    ),
+                ),
+                (
+                    "user",
+                    models.ForeignKey(
+                        to_field="id",
+                        to=settings.AUTH_USER_MODEL,
+                        on_delete=models.CASCADE,
+                    ),
+                ),
+                (
+                    "interval",
+                    models.SmallIntegerField(
+                        choices=[(0, "instantly"), (1380, "daily"), (9660, "weekly")],
+                        default=0,
+                        verbose_name="interval",
+                    ),
+                ),
+            ],
+            options={
+                "verbose_name": "settings",
+                "db_table": "nyt_settings",
+                "verbose_name_plural": "settings",
+            },
+            bases=(models.Model,),
+        ),
+        migrations.CreateModel(
+            name="Notification",
+            fields=[
+                (
+                    "id",
+                    models.AutoField(
+                        auto_created=True,
+                        verbose_name="ID",
+                        serialize=False,
+                        primary_key=True,
+                    ),
+                ),
+                ("message", models.TextField()),
+                (
+                    "url",
+                    models.CharField(
+                        verbose_name="link for notification",
+                        null=True,
+                        max_length=200,
+                        blank=True,
+                    ),
+                ),
+                ("is_viewed", models.BooleanField(default=False)),
+                ("is_emailed", models.BooleanField(default=False)),
+                ("created", models.DateTimeField(auto_now_add=True)),
+                (
+                    "occurrences",
+                    models.PositiveIntegerField(
+                        help_text="If the same notification was fired multiple times with no intermediate notifications",
+                        default=1,
+                        verbose_name="occurrences",
+                    ),
+                ),
+            ],
+            options={
+                "verbose_name": "notification",
+                "db_table": "nyt_notification",
+                "ordering": ("-id",),
+                "verbose_name_plural": "notifications",
+            },
+            bases=(models.Model,),
         ),
     ]
```

### Comparing `django-nyt-1.2.4/django_nyt/migrations/0007_add_modified_and_default_settings.py` & `django_nyt-1.3/django_nyt/migrations/0007_add_modified_and_default_settings.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-from django.db import migrations, models
+from django.db import migrations
+from django.db import models
 from django.utils import timezone
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('django_nyt', '0006_auto_20141229_1630'),
+        ("django_nyt", "0006_auto_20141229_1630"),
     ]
 
     operations = [
         migrations.AddField(
-            model_name='notification',
-            name='modified',
+            model_name="notification",
+            name="modified",
             field=models.DateTimeField(auto_now=True, default=timezone.now()),
             preserve_default=False,
         ),
         migrations.AddField(
-            model_name='settings',
-            name='is_default',
-            field=models.BooleanField(default=False, verbose_name='Default for new subscriptions'),
+            model_name="settings",
+            name="is_default",
+            field=models.BooleanField(
+                default=False, verbose_name="Default for new subscriptions"
+            ),
         ),
     ]
```

### Comparing `django-nyt-1.2.4/django_nyt/models.py` & `django_nyt-1.3/django_nyt/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,42 +15,33 @@
 class NotificationType(models.Model):
     """
     Notification types are added on-the-fly by the
     applications adding new notifications
     """
 
     key = models.CharField(
-        max_length=128,
-        primary_key=True,
-        verbose_name=_('unique key'),
-        unique=True
+        max_length=128, primary_key=True, verbose_name=_("unique key"), unique=True
     )
 
     # TODO: This isn't translatable
     label = models.CharField(
-        max_length=128,
-        verbose_name=_('optional label'),
-        blank=True,
-        null=True
+        max_length=128, verbose_name=_("optional label"), blank=True, null=True
     )
 
     content_type = models.ForeignKey(
-        ContentType,
-        blank=True,
-        null=True,
-        on_delete=models.SET_NULL
+        ContentType, blank=True, null=True, on_delete=models.SET_NULL
     )
 
     def __str__(self):
         return self.key
 
     class Meta:
-        db_table = settings.DB_TABLE_PREFIX + '_notificationtype'
-        verbose_name = _('type')
-        verbose_name_plural = _('types')
+        db_table = settings.DB_TABLE_PREFIX + "_notificationtype"
+        verbose_name = _("type")
+        verbose_name_plural = _("types")
 
     @classmethod
     def get_by_key(cls, key, content_type=None):
         if key in _notification_type_cache:
             return _notification_type_cache[key]
         try:
             nt = cls.objects.get(key=key)
@@ -71,37 +62,36 @@
     Reusable settings object for a subscription
     """
 
     user = models.ForeignKey(
         settings.USER_MODEL,
         on_delete=models.CASCADE,  # If a user is deleted, remove all settings
         verbose_name=_("user"),
-        related_name='nyt_settings',
+        related_name="nyt_settings",
     )
 
     interval = models.SmallIntegerField(
         choices=settings.INTERVALS,
-        verbose_name=_('interval'),
+        verbose_name=_("interval"),
         default=settings.INTERVALS_DEFAULT,
     )
 
     is_default = models.BooleanField(
         default=False,
         verbose_name=_("Default for new subscriptions"),
     )
 
     def __str__(self):
-        obj_name = _("Settings for %s") % getattr(
-            self.user, self.user.USERNAME_FIELD)
+        obj_name = _("Settings for %s") % getattr(self.user, self.user.USERNAME_FIELD)
         return obj_name
 
     class Meta:
-        db_table = settings.DB_TABLE_PREFIX + '_settings'
-        verbose_name = _('settings')
-        verbose_name_plural = _('settings')
+        db_table = settings.DB_TABLE_PREFIX + "_settings"
+        verbose_name = _("settings")
+        verbose_name_plural = _("settings")
 
     def clean(self):
         if not self.is_default and self.pk and self.user:
             default_settings = Settings.objects.filter(
                 user=self.user,
                 is_default=True,
             ).exclude(pk=self.pk)
@@ -131,66 +121,62 @@
                 non_default_settings[0].save()
             else:
                 raise ValueError("A user must have a default settings object")
         super(Settings, self).save(*args, **kwargs)
 
     @classmethod
     def get_default_setting(cls, user):
-        return cls.objects.get_or_create(
-            user=user,
-            is_default=True
-        )[0]
+        return cls.objects.get_or_create(user=user, is_default=True)[0]
 
 
 class Subscription(models.Model):
 
     # If settings are deleted, remove all subscriptions (CASCADE)
     settings = models.ForeignKey(
         Settings,
         verbose_name=_("settings"),
         on_delete=models.CASCADE,
     )
 
     notification_type = models.ForeignKey(
-        NotificationType,
-        verbose_name=_("notification type"),
-        on_delete=models.CASCADE
+        NotificationType, verbose_name=_("notification type"), on_delete=models.CASCADE
     )
 
     object_id = models.CharField(
         max_length=64,
         null=True,
         blank=True,
-        help_text=_('Leave this blank to subscribe to any kind of object'),
+        help_text=_("Leave this blank to subscribe to any kind of object"),
         verbose_name=_("object ID"),
     )
 
     send_emails = models.BooleanField(
         default=True,
         verbose_name=_("send emails"),
     )
 
     latest = models.ForeignKey(
-        'Notification',
+        "Notification",
         null=True,
         blank=True,
-        related_name='latest_for',
+        related_name="latest_for",
         verbose_name=_("latest notification"),
         on_delete=models.CASCADE,
     )
 
     def __str__(self):
         obj_name = _("Subscription for: %s") % (
-            getattr(self.settings.user, self.settings.user.USERNAME_FIELD))
+            getattr(self.settings.user, self.settings.user.USERNAME_FIELD)
+        )
         return obj_name
 
     class Meta:
-        db_table = settings.DB_TABLE_PREFIX + '_subscription'
-        verbose_name = _('subscription')
-        verbose_name_plural = _('subscriptions')
+        db_table = settings.DB_TABLE_PREFIX + "_subscription"
+        verbose_name = _("subscription")
+        verbose_name_plural = _("subscriptions")
 
 
 class Notification(models.Model):
 
     #: Either set the subscription
     subscription = models.ForeignKey(
         Subscription,
@@ -204,22 +190,22 @@
     # If a user is deleted, remove all notifications (CASCADE)
     user = models.ForeignKey(
         settings.USER_MODEL,
         null=True,
         blank=True,
         on_delete=models.CASCADE,
         verbose_name=_("user"),
-        related_name='nyt_notifications',
+        related_name="nyt_notifications",
     )
 
     message = models.TextField()
 
     # TODO: Why 200?
     url = models.CharField(
-        verbose_name=_('link for notification'),
+        verbose_name=_("link for notification"),
         blank=True,
         null=True,
         max_length=200,
     )
 
     is_viewed = models.BooleanField(default=False)
 
@@ -227,18 +213,18 @@
 
     created = models.DateTimeField(auto_now_add=True)
 
     modified = models.DateTimeField(auto_now=True)
 
     occurrences = models.PositiveIntegerField(
         default=1,
-        verbose_name=_('occurrences'),
+        verbose_name=_("occurrences"),
         help_text=_(
-            'If the same notification was fired multiple '
-            'times with no intermediate notifications'
+            "If the same notification was fired multiple "
+            "times with no intermediate notifications"
         ),
     )
 
     def save(self, *args, **kwargs):
         assert self.user or self.subscription
         if not self.user:
             self.user = self.subscription.settings.user
@@ -250,70 +236,66 @@
         Creates notifications directly in database -- do not call directly,
         use django_nyt.notify(...)
 
         This is the old interface.
         """
 
         if not key or not isinstance(key, str):
-            raise KeyError('No notification key (string) specified.')
+            raise KeyError("No notification key (string) specified.")
 
-        object_id = kwargs.pop('object_id', None)
-        filter_exclude = kwargs.pop('filter_exclude', {})
-        recipient_users = kwargs.pop('recipient_users', None)
+        object_id = kwargs.pop("object_id", None)
+        filter_exclude = kwargs.pop("filter_exclude", {})
+        recipient_users = kwargs.pop("recipient_users", None)
 
         objects_created = []
-        subscriptions = Subscription.objects.filter(
-            notification_type__key=key
-        ).exclude(
+        subscriptions = Subscription.objects.filter(notification_type__key=key).exclude(
             **filter_exclude
         )
         if object_id:
             subscriptions = subscriptions.filter(
                 Q(object_id=object_id) | Q(object_id=None)
             )
         if recipient_users:
             subscriptions = subscriptions.filter(
                 settings__user__in=recipient_users,
             )
 
-        subscriptions = subscriptions.prefetch_related('latest', 'settings')
-        subscriptions = subscriptions.order_by('settings__user')
+        subscriptions = subscriptions.prefetch_related("latest", "settings")
+        subscriptions = subscriptions.order_by("settings__user")
         prev_user = None
 
         for subscription in subscriptions:
             # Don't alert the same user several times even though overlapping
             # subscriptions occur.
             if subscription.settings.user == prev_user:
                 continue
 
             # Check if it's the same as the previous message
             latest = subscription.latest
-            if latest and (latest.message == kwargs.get('message', None)
-                           and latest.url == kwargs.get('url', None)
-                           and latest.is_viewed is False):
+            if latest and (
+                latest.message == kwargs.get("message", None)
+                and latest.url == kwargs.get("url", None)
+                and latest.is_viewed is False
+            ):
                 # Both message and URL are the same, and it hasn't been viewed
                 # so just increment occurrence count.
                 latest.occurrences = latest.occurrences + 1
                 latest.is_emailed = False
                 latest.save()
             else:
                 # Insert a new notification
-                new_obj = cls.objects.create(
-                    subscription=subscription,
-                    **kwargs)
-                objects_created.append(
-                    new_obj
-                )
+                new_obj = cls.objects.create(subscription=subscription, **kwargs)
+                objects_created.append(new_obj)
                 subscription.latest = new_obj
                 subscription.save()
             prev_user = subscription.settings.user
 
         return objects_created
 
     def __str__(self):
         return "%s: %s" % (self.user, self.message)
 
     class Meta:
-        db_table = settings.DB_TABLE_PREFIX + '_notification'
-        verbose_name = _('notification')
-        verbose_name_plural = _('notifications')
-        ordering = ('-id',)
+        db_table = settings.DB_TABLE_PREFIX + "_notification"
+        verbose_name = _("notification")
+        verbose_name_plural = _("notifications")
+        ordering = ("-id",)
```

### Comparing `django-nyt-1.2.4/django_nyt/subscribers.py` & `django_nyt-1.3/django_nyt/subscribers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import logging
 
 from channels import Group
 
-from . import models, settings
+from . import models
+from . import settings
 
 logger = logging.getLogger(__name__)
 
 
 def notify_subscribers(notifications, key):
     """
     Notify all open channels about new notifications
     """
 
     logger.debug("Broadcasting to subscribers")
 
-    notification_type_ids = models.NotificationType.objects.values('key').filter(key=key)
+    notification_type_ids = models.NotificationType.objects.values("key").filter(
+        key=key
+    )
 
     for notification_type in notification_type_ids:
         g = Group(
             settings.NOTIFICATION_CHANNEL.format(
-                notification_key=notification_type['key']
+                notification_key=notification_type["key"]
             )
         )
-        g.send(
-            {'text': 'new-notification'}
-        )
+        g.send({"text": "new-notification"})
```

### Comparing `django-nyt-1.2.4/django_nyt/tests/test_basic.py` & `django_nyt-1.3/django_nyt/tests/test_basic.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,35 +4,33 @@
 from django_nyt import models
 from django_nyt import utils
 
 User = get_user_model()
 
 
 class NotifyTestBase(TestCase):
-
     def setUp(self):
         super(NotifyTestBase, self).setUp()
-        self.TEST_KEY = 'test_key'
+        self.TEST_KEY = "test_key"
 
         # These two users are created by migrations in testproject.testapp
         # Reason is to make the testproject easy to setup and use.
-        self.user1 = User.objects.get(username='alice')
+        self.user1 = User.objects.get(username="alice")
         self.user1_settings = models.Settings.get_default_setting(self.user1)
-        self.user2 = User.objects.get(username='bob')
+        self.user2 = User.objects.get(username="bob")
         self.user2_settings = models.Settings.get_default_setting(self.user2)
 
     def tearDown(self):
         self.user1.delete()
         self.user2.delete()
         models._notification_type_cache = {}
         super().tearDown()
 
 
 class NotifyTest(NotifyTestBase):
-
     def test_notify(self):
 
         # Subscribe User 1 to test key
         utils.subscribe(self.user1_settings, self.TEST_KEY)
         utils.notify("Test is a test", self.TEST_KEY)
 
         # Check that there is exactly 1 notification
```

### Comparing `django-nyt-1.2.4/django_nyt/tests/test_management.py` & `django_nyt-1.3/django_nyt/tests/test_management.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,45 +7,48 @@
 
 from .. import models
 from .. import utils
 from .test_basic import NotifyTestBase
 
 
 class CommandTest(NotifyTestBase):
-
     def tearDown(self):
         models._notification_type_cache = {}
         super().tearDown()
 
     def test_notifymail(self):
 
         utils.subscribe(self.user2_settings, self.TEST_KEY)
         utils.subscribe(self.user1_settings, self.TEST_KEY)
         utils.notify("This notification goes out by mail!", self.TEST_KEY)
 
         call_command("notifymail", cron=True)
 
         # No un-mailed notifications can be left!
-        self.assertEqual(models.Notification.objects.filter(is_emailed=False).count(), 0)
+        self.assertEqual(
+            models.Notification.objects.filter(is_emailed=False).count(), 0
+        )
 
         # Test that calling it again works but nothing gets sent
         call_command("notifymail", cron=True)
 
         # Now try the daemon
         pid_file = NamedTemporaryFile(delete=False)
         # Close it so its available for the other command
         pid_file.close()
 
         try:
-            call_command('notifymail', daemon=True, pid=pid_file.name, no_sys_exit=False)
+            call_command(
+                "notifymail", daemon=True, pid=pid_file.name, no_sys_exit=False
+            )
         except SystemExit:
             # It's normal for this command to exit
             pass
 
-        with open(pid_file.name, 'r') as fp:
+        with open(pid_file.name, "r") as fp:
             pid = fp.read()
         os.unlink(pid_file.name)
 
         # Give it a second to start
         time.sleep(1)
 
         os.kill(int(pid), signal.SIGTERM)
```

### Comparing `django-nyt-1.2.4/django_nyt/tests/test_views.py` & `django_nyt-1.3/django_nyt/tests/test_views.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,32 +6,28 @@
 from django_nyt import utils
 
 
 User = get_user_model()
 
 
 class TestViews(TestCase):
-
     def setUp(self):
         super().setUp()
-        self.TEST_KEY = 'test_key'
+        self.TEST_KEY = "test_key"
         self.user = User.objects.create_user(
-            'lalala',
-            password='password',
+            "lalala",
+            password="password",
         )
         self.user_settings = models.Settings.get_default_setting(self.user)
 
     def tearDown(self):
         super().tearDown()
         models._notification_type_cache = {}
 
     def test_mark_read(self):
         utils.subscribe(self.user_settings, self.TEST_KEY)
         utils.notify("Test Is a Test", self.TEST_KEY)
-        self.assertEqual(models.Notification.objects.filter(is_viewed=False).count(),
-                         1)
+        self.assertEqual(models.Notification.objects.filter(is_viewed=False).count(), 1)
         nid = models.Notification.objects.get().id
-        self.client.login(username=self.user.username,
-                          password='password')
-        self.client.get(reverse('nyt:json_mark_read', args=(nid,)))
-        self.assertEqual(models.Notification.objects.filter(is_viewed=False).count(),
-                         0)
+        self.client.login(username=self.user.username, password="password")
+        self.client.get(reverse("nyt:json_mark_read", args=(nid,)))
+        self.assertEqual(models.Notification.objects.filter(is_viewed=False).count(), 0)
```

### Comparing `django-nyt-1.2.4/django_nyt/urls.py` & `django_nyt-1.3/django_nyt/urls.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,34 @@
-from django.urls import include, re_path as url
+from django.urls import include
+from django.urls import re_path as url
 
 from . import views
 
-app_name = 'nyt'
+app_name = "nyt"
 
 urlpatterns = [
-    url(r'^json/get/$', views.get_notifications, name='json_get'),
-    url(r'^json/get/(?P<latest_id>\d+)/$', views.get_notifications, name='json_get'),
-    url(r'^json/mark-read/$', views.mark_read, name='json_mark_read_base'),
-    url(r'^json/mark-read/(\d+)/$', views.mark_read, name='json_mark_read'),
-    url(r'^json/mark-read/(?P<id_lte>\d+)/(?P<id_gte>\d+)/$', views.mark_read, name='json_mark_read'),
-    url(r'^goto/(?P<notification_id>\d+)/$', views.goto, name='goto'),
-    url(r'^goto/$', views.goto, name='goto_base'),
+    url(r"^json/get/$", views.get_notifications, name="json_get"),
+    url(r"^json/get/(?P<latest_id>\d+)/$", views.get_notifications, name="json_get"),
+    url(r"^json/mark-read/$", views.mark_read, name="json_mark_read_base"),
+    url(r"^json/mark-read/(\d+)/$", views.mark_read, name="json_mark_read"),
+    url(
+        r"^json/mark-read/(?P<id_lte>\d+)/(?P<id_gte>\d+)/$",
+        views.mark_read,
+        name="json_mark_read",
+    ),
+    url(r"^goto/(?P<notification_id>\d+)/$", views.goto, name="goto"),
+    url(r"^goto/$", views.goto, name="goto_base"),
 ]
 
 
 def get_pattern(app_name=app_name, namespace="nyt"):
     """Every url resolution takes place as "nyt:view_name".
-       https://docs.djangoproject.com/en/dev/topics/http/urls/#topics-http-reversing-url-namespaces
+    https://docs.djangoproject.com/en/dev/topics/http/urls/#topics-http-reversing-url-namespaces
     """
     import warnings
+
     warnings.warn(
-        'django_nyt.urls.get_pattern is deprecated and will be removed in next version,'
-        ' just use include(\'django_nyt.urls\')', DeprecationWarning
+        "django_nyt.urls.get_pattern is deprecated and will be removed in next version,"
+        " just use include('django_nyt.urls')",
+        DeprecationWarning,
     )
-    return include('django_nyt.urls')
+    return include("django_nyt.urls")
```

### Comparing `django-nyt-1.2.4/django_nyt/utils.py` & `django_nyt-1.3/django_nyt/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from django.db.models import Model
 from django.utils.translation import gettext as _
 
-from . import _disable_notifications, models, settings
+from . import _disable_notifications
+from . import models
+from . import settings
 
 
-def notify(message, key, target_object=None, url=None, filter_exclude={}, recipient_users=None):
+def notify(
+    message, key, target_object=None, url=None, filter_exclude={}, recipient_users=None
+):
     """
     Notify subscribing users of a new event. Key can be any kind of string,
     just make sure to reuse it where applicable.
 
     notify("there was a response to your comment", "comment_response",
            target_object=PostersObject,
            url=reverse('comments:view', args=(PostersObject.id,)))
@@ -32,15 +36,18 @@
 
     if _disable_notifications:
         return 0
 
     if target_object:
         if not isinstance(target_object, Model):
             raise TypeError(
-                _("You supplied a target_object that's not an instance of a django Model."))
+                _(
+                    "You supplied a target_object that's not an instance of a django Model."
+                )
+            )
         object_id = target_object.id
     else:
         object_id = None
 
     objects = models.Notification.create_notifications(
         key,
         object_id=object_id,
@@ -49,14 +56,15 @@
         filter_exclude=filter_exclude,
         recipient_users=recipient_users,
     )
 
     # Notify channel subscribers if we have channels enabled
     if settings.ENABLE_CHANNELS:
         from django_nyt import subscribers
+
         subscribers.notify_subscribers(objects, key)
 
     return len(objects)
 
 
 def subscribe(settings, key, content_type=None, object_id=None, **kwargs):
     """
@@ -68,15 +76,17 @@
 
     :param: settings: A models.Settings instance
     :param: key: The unique key that the Settings should subscribe to
     :param: content_type: If notifications are regarding a specific ContentType, it should be set
     :param: object_id: If the notifications should only regard a specific object_id
     :param: **kwargs: Additional models.Subscription field values
     """
-    notification_type = models.NotificationType.get_by_key(key, content_type=content_type)
+    notification_type = models.NotificationType.get_by_key(
+        key, content_type=content_type
+    )
 
     return models.Subscription.objects.get_or_create(
         settings=settings,
         notification_type=notification_type,
         object_id=object_id,
         **kwargs
     )[0]
```

### Comparing `django-nyt-1.2.4/django_nyt/views.py` & `django_nyt-1.3/django_nyt/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,19 +7,15 @@
 from django_nyt import models
 from django_nyt.decorators import json_view
 from django_nyt.decorators import login_required_ajax
 
 
 @login_required_ajax
 @json_view
-def get_notifications(
-        request,
-        latest_id=None,
-        is_viewed=False,
-        max_results=10):
+def get_notifications(request, latest_id=None, is_viewed=False, max_results=10):
     """
     View that returns a JSON list of notifications for the current user as according
     to ``request.user``.
 
     :param: latest_id: The latest id of a notification. Use this to avoid
     retrieving the same notifications multiple times.
     :param: is_viewed: Set this to ``True`` if you also want to retrieve
@@ -46,61 +42,69 @@
         notifications = notifications.filter(is_viewed=is_viewed)
 
     total_count = notifications.count()
 
     if latest_id is not None:
         notifications = notifications.filter(id__gt=latest_id)
 
-    notifications = notifications.order_by('-id')
+    notifications = notifications.order_by("-id")
     notifications = notifications.prefetch_related(
-        'subscription',
-        'subscription__notification_type')
+        "subscription", "subscription__notification_type"
+    )
 
     from django.contrib.humanize.templatetags.humanize import naturaltime
 
-    return {'success': True,
-            'total_count': total_count,
-            'objects': [{'pk': n.pk,
-                         'message': n.message,
-                         'url': n.url,
-                         'occurrences': n.occurrences,
-                         'occurrences_msg': _('%d times') % n.occurrences,
-                         'type': n.subscription.notification_type.key if n.subscription else None,
-                         'since': naturaltime(n.created)} for n in notifications[:max_results]]}
+    return {
+        "success": True,
+        "total_count": total_count,
+        "objects": [
+            {
+                "pk": n.pk,
+                "message": n.message,
+                "url": n.url,
+                "occurrences": n.occurrences,
+                "occurrences_msg": _("%d times") % n.occurrences,
+                "type": n.subscription.notification_type.key
+                if n.subscription
+                else None,
+                "since": naturaltime(n.created),
+            }
+            for n in notifications[:max_results]
+        ],
+    }
 
 
 @login_required
 def goto(request, notification_id=None):
-    referer = request.META.get('HTTP_REFERER', '')
+    referer = request.META.get("HTTP_REFERER", "")
     if not notification_id:
         return redirect(referer)
     notification = get_object_or_404(
         models.Notification,
         Q(subscription__settings__user=request.user) | Q(user=request.user),
-        id=notification_id
+        id=notification_id,
     )
     notification.is_viewed = True
     notification.save()
     if notification.url:
         return redirect(notification.url)
     return redirect(referer)
 
 
 @login_required_ajax
 @json_view
 def mark_read(request, id_lte, notification_type_id=None, id_gte=None):
 
     notifications = models.Notification.objects.filter(
         Q(subscription__settings__user=request.user) | Q(user=request.user),
-        id__lte=id_lte
+        id__lte=id_lte,
     )
 
     if notification_type_id:
-        notifications = notifications.filter(
-            notification_type__id=notification_type_id)
+        notifications = notifications.filter(notification_type__id=notification_type_id)
 
     if id_gte:
         notifications = notifications.filter(id__gte=id_gte)
 
     notifications.update(is_viewed=True)
 
-    return {'success': True}
+    return {"success": True}
```

