# Comparing `tmp/fcm-django-1.0.8.tar.gz` & `tmp/fcm-django-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcm-django-1.0.8.tar", last modified: Fri Jan  7 16:15:18 2022, max compression
+gzip compressed data, was "fcm-django-1.0.9.tar", last modified: Mon Mar 28 19:58:00 2022, max compression
```

## Comparing `fcm-django-1.0.8.tar` & `fcm-django-1.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 xtrinch   (1000) xtrinch   (1000)        0 2022-01-07 16:15:18.247395 fcm-django-1.0.8/
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)     1130 2021-04-11 10:41:31.000000 fcm-django-1.0.8/LICENSE.txt
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)       55 2021-04-11 10:41:31.000000 fcm-django-1.0.8/MANIFEST.in
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      995 2022-01-07 16:15:18.247395 fcm-django-1.0.8/PKG-INFO
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)    12975 2021-12-16 09:07:29.000000 fcm-django-1.0.8/README.rst
-drwxrwxr-x   0 xtrinch   (1000) xtrinch   (1000)        0 2022-01-07 16:15:18.247395 fcm-django-1.0.8/fcm_django/
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      309 2022-01-07 16:08:31.000000 fcm-django-1.0.8/fcm_django/__init__.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)     8044 2021-08-02 11:40:53.000000 fcm-django-1.0.8/fcm_django/admin.py
-drwxrwxr-x   0 xtrinch   (1000) xtrinch   (1000)        0 2022-01-07 16:15:18.247395 fcm-django-1.0.8/fcm_django/api/
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      341 2021-07-10 12:52:28.000000 fcm-django-1.0.8/fcm_django/api/__init__.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)     5899 2021-12-16 09:17:47.000000 fcm-django-1.0.8/fcm_django/api/rest_framework.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      806 2021-07-10 12:52:28.000000 fcm-django-1.0.8/fcm_django/api/tastypie.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      207 2022-01-07 16:08:01.000000 fcm-django-1.0.8/fcm_django/apps.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)     4149 2021-07-10 12:52:28.000000 fcm-django-1.0.8/fcm_django/fields.py
-drwxrwxr-x   0 xtrinch   (1000) xtrinch   (1000)        0 2022-01-07 16:15:18.247395 fcm-django-1.0.8/fcm_django/migrations/
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)     2555 2021-07-10 12:52:28.000000 fcm-django-1.0.8/fcm_django/migrations/0001_initial.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      598 2021-07-10 12:52:28.000000 fcm-django-1.0.8/fcm_django/migrations/0002_auto_20160808_1645.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      504 2021-07-10 12:52:28.000000 fcm-django-1.0.8/fcm_django/migrations/0003_auto_20170313_1314.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      444 2021-07-10 12:52:28.000000 fcm-django-1.0.8/fcm_django/migrations/0004_auto_20181128_1642.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      750 2021-07-10 12:52:28.000000 fcm-django-1.0.8/fcm_django/migrations/0005_auto_20170808_1145.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      610 2021-08-17 14:10:04.000000 fcm-django-1.0.8/fcm_django/migrations/0006_auto_20210802_1140.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      362 2021-12-16 09:07:29.000000 fcm-django-1.0.8/fcm_django/migrations/0007_auto_20211001_1440.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      477 2021-12-24 13:42:53.000000 fcm-django-1.0.8/fcm_django/migrations/0008_auto_20211224_1205.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)        0 2021-04-11 10:41:31.000000 fcm-django-1.0.8/fcm_django/migrations/__init__.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)    13243 2022-01-07 16:08:18.000000 fcm-django-1.0.8/fcm_django/models.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      779 2021-07-10 12:52:28.000000 fcm-django-1.0.8/fcm_django/settings.py
-drwxrwxr-x   0 xtrinch   (1000) xtrinch   (1000)        0 2022-01-07 16:15:18.247395 fcm-django-1.0.8/fcm_django.egg-info/
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      995 2022-01-07 16:15:18.000000 fcm-django-1.0.8/fcm_django.egg-info/PKG-INFO
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      851 2022-01-07 16:15:18.000000 fcm-django-1.0.8/fcm_django.egg-info/SOURCES.txt
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)        1 2022-01-07 16:15:18.000000 fcm-django-1.0.8/fcm_django.egg-info/dependency_links.txt
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)       28 2022-01-07 16:15:18.000000 fcm-django-1.0.8/fcm_django.egg-info/requires.txt
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)       48 2022-01-07 16:15:18.000000 fcm-django-1.0.8/fcm_django.egg-info/top_level.txt
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)       67 2022-01-07 16:15:18.251395 fcm-django-1.0.8/setup.cfg
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)     1302 2021-08-02 11:40:53.000000 fcm-django-1.0.8/setup.py
+drwxrwxr-x   0 xtrinch   (1000) xtrinch   (1000)        0 2022-03-28 19:58:00.597139 fcm-django-1.0.9/
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)     1130 2021-04-11 10:41:31.000000 fcm-django-1.0.9/LICENSE.txt
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)       55 2021-04-11 10:41:31.000000 fcm-django-1.0.9/MANIFEST.in
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)     1016 2022-03-28 19:58:00.597139 fcm-django-1.0.9/PKG-INFO
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)    12673 2022-03-28 19:44:13.000000 fcm-django-1.0.9/README.rst
+drwxrwxr-x   0 xtrinch   (1000) xtrinch   (1000)        0 2022-03-28 19:58:00.593139 fcm-django-1.0.9/fcm_django/
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      309 2022-03-28 19:52:13.000000 fcm-django-1.0.9/fcm_django/__init__.py
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)     8741 2022-03-28 19:45:14.000000 fcm-django-1.0.9/fcm_django/admin.py
+drwxrwxr-x   0 xtrinch   (1000) xtrinch   (1000)        0 2022-03-28 19:58:00.597139 fcm-django-1.0.9/fcm_django/api/
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      341 2021-07-10 12:52:28.000000 fcm-django-1.0.9/fcm_django/api/__init__.py
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)     5909 2022-03-28 19:42:44.000000 fcm-django-1.0.9/fcm_django/api/rest_framework.py
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      806 2021-07-10 12:52:28.000000 fcm-django-1.0.9/fcm_django/api/tastypie.py
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      207 2022-01-07 16:08:01.000000 fcm-django-1.0.9/fcm_django/apps.py
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)     4147 2022-03-28 19:56:39.000000 fcm-django-1.0.9/fcm_django/fields.py
+drwxrwxr-x   0 xtrinch   (1000) xtrinch   (1000)        0 2022-03-28 19:58:00.597139 fcm-django-1.0.9/fcm_django/migrations/
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)     2555 2021-07-10 12:52:28.000000 fcm-django-1.0.9/fcm_django/migrations/0001_initial.py
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      598 2021-07-10 12:52:28.000000 fcm-django-1.0.9/fcm_django/migrations/0002_auto_20160808_1645.py
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      504 2021-07-10 12:52:28.000000 fcm-django-1.0.9/fcm_django/migrations/0003_auto_20170313_1314.py
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      444 2021-07-10 12:52:28.000000 fcm-django-1.0.9/fcm_django/migrations/0004_auto_20181128_1642.py
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      750 2021-07-10 12:52:28.000000 fcm-django-1.0.9/fcm_django/migrations/0005_auto_20170808_1145.py
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      610 2021-08-17 14:10:04.000000 fcm-django-1.0.9/fcm_django/migrations/0006_auto_20210802_1140.py
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      362 2021-12-16 09:07:29.000000 fcm-django-1.0.9/fcm_django/migrations/0007_auto_20211001_1440.py
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      477 2021-12-24 13:42:53.000000 fcm-django-1.0.9/fcm_django/migrations/0008_auto_20211224_1205.py
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)        0 2021-04-11 10:41:31.000000 fcm-django-1.0.9/fcm_django/migrations/__init__.py
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)    13763 2022-03-28 19:42:44.000000 fcm-django-1.0.9/fcm_django/models.py
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      779 2021-07-10 12:52:28.000000 fcm-django-1.0.9/fcm_django/settings.py
+drwxrwxr-x   0 xtrinch   (1000) xtrinch   (1000)        0 2022-03-28 19:58:00.593139 fcm-django-1.0.9/fcm_django.egg-info/
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)     1016 2022-03-28 19:58:00.000000 fcm-django-1.0.9/fcm_django.egg-info/PKG-INFO
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      851 2022-03-28 19:58:00.000000 fcm-django-1.0.9/fcm_django.egg-info/SOURCES.txt
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)        1 2022-03-28 19:58:00.000000 fcm-django-1.0.9/fcm_django.egg-info/dependency_links.txt
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)       28 2022-03-28 19:58:00.000000 fcm-django-1.0.9/fcm_django.egg-info/requires.txt
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)       48 2022-03-28 19:58:00.000000 fcm-django-1.0.9/fcm_django.egg-info/top_level.txt
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)       67 2022-03-28 19:58:00.597139 fcm-django-1.0.9/setup.cfg
+-rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)     1329 2022-03-28 19:00:13.000000 fcm-django-1.0.9/setup.py
```

### Comparing `fcm-django-1.0.8/LICENSE.txt` & `fcm-django-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fcm-django-1.0.8/README.rst` & `fcm-django-1.0.9/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -227,21 +227,17 @@
     device.handle_topic_subscription(False, topic="TOPIC NAME"))
 
 Sending messages to topic
 -------------------------
 
 .. code-block:: python
 
-    from firebase_admin.messaging import Message
     from fcm_django.models import FCMDevice
 
-    # You can still use .filter() or any methods that return QuerySet (from the chain)
-    FCMDevice.objects.all().send_message(Message(data={...}, topic="TOPIC NAME"))
-    device = FCMDevice.objects.all().first()
-    device.send_message(Message(data={...}, topic="TOPIC NAME"))
+    FCMDevice.send_topic_message(Message(data={...}), "TOPIC NAME")
 
 Additional Parameters
 ---------------------
 
 You can add additional_registration_ids (Sequence) for manually
 sending registration IDs. It will append these IDs to the queryset
 lookup's returned registration IDs.
@@ -280,15 +276,15 @@
     - A device may be registered without associating it with a user
     - Will not allow duplicate registration_id's
 
 - ``FCMDeviceAuthorizedViewSet``
 
     - Permissions are ``IsAuthenticated`` and custom permission ``IsOwner``, which will only allow the ``request.user`` to get and update devices that belong to that user
     - Requires a user to be authenticated, so all devices will be associated with a user
-    - Will allow duplicate registration_id's for different users, so you are responsible for cleanup (if that is generally perceived as undesired behaviour or if the package itself should be doing the cleanup, open an issue or email me)
+    - Will allow duplicate registration_id's for different users, so you are responsible for cleanup (if you do not want duplicate registration id's, use the ``UPDATE_ON_DUPLICATE_REG_ID`` flag)
 
 Routes can be added one of two ways:
 
 - `Routers`_ (include all views)
 
 .. _Routers: http://www.django-rest-framework.org/tutorial/6-viewsets-and-routers#using-routers
```

### Comparing `fcm-django-1.0.8/fcm_django/admin.py` & `fcm-django-1.0.9/fcm_django/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     actions = (
         "send_message",
         "send_bulk_message",
         "subscribe_to_topic",
         "bulk_subscribe_to_topic",
         "unsubscribe_to_topic",
         "bulk_unsubscribe_to_topic",
+        "send_topic_message",
         "enable",
         "disable",
     )
     raw_id_fields = ("user",)
     list_select_related = ("user",)
 
     def get_search_fields(self, request):
@@ -191,15 +192,20 @@
                 break
             else:
                 response = device.handle_topic_subscription(
                     should_subscribe,
                     "test-topic",
                 )
                 single_responses.append(
-                    (response.response.errors[0], device.registration_id)
+                    (
+                        response.response.errors[0]
+                        if len(response.response.errors) > 0
+                        else "Success",
+                        device.registration_id,
+                    )
                 )
                 total_failure += len(response.deactivated_registration_ids)
 
         self._send_deactivated_message(request, single_responses, total_failure, True)
 
     def subscribe_to_topic(self, request, queryset):
         self.handle_topic_subscription(request, queryset, True)
@@ -217,14 +223,29 @@
     unsubscribe_to_topic.short_description = _("Unsubscribe to test topic")
 
     def bulk_unsubscribe_to_topic(self, request, queryset):
         self.handle_topic_subscription(request, queryset, False, True)
 
     bulk_unsubscribe_to_topic.short_description = _("Unsubscribe to test topic in bulk")
 
+    def handle_send_topic_message(self, request, queryset):
+        FCMDevice.send_topic_message(
+            Message(
+                notification=Notification(
+                    title="Test notification", body="Test single notification"
+                )
+            ),
+            "test-topic",
+        )
+
+    def send_topic_message(self, request, queryset):
+        self.handle_send_topic_message(request, queryset)
+
+    send_topic_message.short_description = _("Send message test topic")
+
     def enable(self, request, queryset):
         queryset.update(active=True)
 
     enable.short_description = _("Enable selected devices")
 
     def disable(self, request, queryset):
         queryset.update(active=False)
```

### Comparing `fcm-django-1.0.8/fcm_django/api/rest_framework.py` & `fcm-django-1.0.9/fcm_django/api/rest_framework.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     def get_queryset(self):
         # filter all devices to only those belonging to the current user
         return self.queryset.filter(user=self.request.user)
 
 
 # ViewSets
 class FCMDeviceViewSet(DeviceViewSetMixin, ModelViewSet):
-    queryset = FCMDevice.objects.all()
+    queryset = FCMDevice.objects.order_by("-id")
     serializer_class = FCMDeviceSerializer
 
 
 class FCMDeviceCreateOnlyViewSet(DeviceViewSetMixin, CreateModelMixin, GenericViewSet):
     queryset = FCMDevice.objects.all()
     serializer_class = FCMDeviceSerializer
```

### Comparing `fcm-django-1.0.8/fcm_django/api/tastypie.py` & `fcm-django-1.0.9/fcm_django/api/tastypie.py`

 * *Files identical despite different names*

### Comparing `fcm-django-1.0.8/fcm_django/fields.py` & `fcm-django-1.0.9/fcm_django/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from django import forms
 from django.core.validators import MaxValueValidator, MinValueValidator, RegexValidator
 from django.db import connection, models
 from django.utils.translation import gettext_lazy as _
 
 UNSIGNED_64BIT_INT_MIN_VALUE = 0
-UNSIGNED_64BIT_INT_MAX_VALUE = 2 ** 64 - 1
+UNSIGNED_64BIT_INT_MAX_VALUE = 2**64 - 1
 
 __all__ = ["HexadecimalField", "HexIntegerField"]
 
 hex_re = re.compile(r"^(([0-9A-f])|(0x[0-9A-f]))+$")
 signed_integer_engines = [
     "django.db.backends.postgresql",
     "django.db.backends.postgresql_psycopg2",
```

### Comparing `fcm-django-1.0.8/fcm_django/migrations/0001_initial.py` & `fcm-django-1.0.9/fcm_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `fcm-django-1.0.8/fcm_django/migrations/0002_auto_20160808_1645.py` & `fcm-django-1.0.9/fcm_django/migrations/0002_auto_20160808_1645.py`

 * *Files identical despite different names*

### Comparing `fcm-django-1.0.8/fcm_django/migrations/0005_auto_20170808_1145.py` & `fcm-django-1.0.9/fcm_django/migrations/0005_auto_20170808_1145.py`

 * *Files identical despite different names*

### Comparing `fcm-django-1.0.8/fcm_django/migrations/0006_auto_20210802_1140.py` & `fcm-django-1.0.9/fcm_django/migrations/0006_auto_20210802_1140.py`

 * *Files identical despite different names*

### Comparing `fcm-django-1.0.8/fcm_django/models.py` & `fcm-django-1.0.9/fcm_django/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,19 @@
     )
     active = models.BooleanField(
         verbose_name=_("Is active"),
         default=True,
         help_text=_("Inactive devices will not be sent notifications"),
     )
     user = models.ForeignKey(
-        SETTINGS["USER_MODEL"], blank=True, null=True, on_delete=models.CASCADE
+        SETTINGS["USER_MODEL"],
+        blank=True,
+        null=True,
+        on_delete=models.CASCADE,
+        related_query_name=_("device"),
     )
     date_created = models.DateTimeField(
         verbose_name=_("Creation date"), auto_now_add=True, null=True
     )
 
     class Meta:
         abstract = True
@@ -345,12 +349,27 @@
     def deactivate_devices_with_error_result(
         cls, registration_id, firebase_exc, name=None
     ) -> List[str]:
         return cls.objects.deactivate_devices_with_error_results(
             [registration_id], [messaging.SendResponse({"name": name}, firebase_exc)]
         )
 
+    @staticmethod
+    def send_topic_message(
+        message: messaging.Message,
+        topic_name: str,
+        **more_send_message_kwargs,
+    ) -> Union[Optional[messaging.SendResponse], FirebaseError]:
+        message.topic = topic_name
+
+        try:
+            return messaging.SendResponse(
+                {"name": messaging.send(message, **more_send_message_kwargs)}, None
+            )
+        except FirebaseError as e:
+            return e
+
 
 class FCMDevice(AbstractFCMDevice):
     class Meta:
         verbose_name = _("FCM device")
         verbose_name_plural = _("FCM devices")
```

### Comparing `fcm-django-1.0.8/fcm_django/settings.py` & `fcm-django-1.0.9/fcm_django/settings.py`

 * *Files identical despite different names*

### Comparing `fcm-django-1.0.8/fcm_django.egg-info/SOURCES.txt` & `fcm-django-1.0.9/fcm_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fcm-django-1.0.8/setup.py` & `fcm-django-1.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 setup(
     name="fcm-django",
     packages=[
         "fcm_django",
         "fcm_django/api",
         "fcm_django/migrations",
     ],
+    python_requires=">=3",
     install_requires=["firebase-admin>=5,<6", "Django"],
     author=fcm_django.__author__,
     author_email=fcm_django.__email__,
     classifiers=CLASSIFIERS,
     description="Send push notifications to mobile devices & browsers through "
     "FCM in Django.",
     download_url="https://github.com/xtrinch/fcm-django/tarball/master",
```

