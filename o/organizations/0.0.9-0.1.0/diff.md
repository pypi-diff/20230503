# Comparing `tmp/organizations-0.0.9.tar.gz` & `tmp/organizations-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "organizations-0.0.9.tar", last modified: Thu Mar 16 09:19:18 2023, max compression
+gzip compressed data, was "organizations-0.1.0.tar", last modified: Wed May  3 12:35:01 2023, max compression
```

## Comparing `organizations-0.0.9.tar` & `organizations-0.1.0.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2023-03-16 09:19:18.439685 organizations-0.0.9/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1073 2023-03-13 16:26:58.000000 organizations-0.0.9/LICENSE
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      389 2023-03-16 09:19:18.435685 organizations-0.0.9/PKG-INFO
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)        0 2023-03-13 16:26:58.000000 organizations-0.0.9/README.md
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      962 2023-03-16 09:19:06.000000 organizations-0.0.9/pyproject.toml
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       38 2023-03-16 09:19:18.439685 organizations-0.0.9/setup.cfg
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2023-03-16 09:19:18.431685 organizations-0.0.9/src/
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2023-03-16 09:19:18.435685 organizations-0.0.9/src/organizations/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)        0 2023-03-13 16:26:58.000000 organizations-0.0.9/src/organizations/__init__.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      638 2023-03-13 16:26:58.000000 organizations-0.0.9/src/organizations/abstractions.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4817 2023-03-15 15:17:18.000000 organizations-0.0.9/src/organizations/admin.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      225 2023-03-13 16:26:58.000000 organizations-0.0.9/src/organizations/apps.py
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2023-03-16 09:19:18.435685 organizations-0.0.9/src/organizations/did_factory/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)        0 2023-03-13 16:26:58.000000 organizations-0.0.9/src/organizations/did_factory/__init__.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1177 2023-03-14 14:55:32.000000 organizations-0.0.9/src/organizations/did_factory/abstractions.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      238 2023-03-13 16:26:58.000000 organizations-0.0.9/src/organizations/did_factory/context.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      641 2023-03-13 16:26:58.000000 organizations-0.0.9/src/organizations/did_factory/factory.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      164 2023-03-13 16:26:58.000000 organizations-0.0.9/src/organizations/did_factory/models.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     9686 2023-03-15 08:59:33.000000 organizations-0.0.9/src/organizations/did_factory/strategy.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      234 2023-03-13 16:26:58.000000 organizations-0.0.9/src/organizations/enums.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      692 2023-03-13 16:26:58.000000 organizations-0.0.9/src/organizations/forms.py
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2023-03-16 09:19:18.435685 organizations-0.0.9/src/organizations/migrations/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     4814 2023-03-13 16:26:58.000000 organizations-0.0.9/src/organizations/migrations/0001_initial.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      693 2023-03-13 16:26:58.000000 organizations-0.0.9/src/organizations/migrations/0002_organization_networks.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      648 2023-03-13 16:26:58.000000 organizations-0.0.9/src/organizations/migrations/0003_alter_organization_networks.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      837 2023-03-13 16:26:58.000000 organizations-0.0.9/src/organizations/migrations/0004_alter_organization_email_and_more.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3591 2023-03-13 16:26:58.000000 organizations-0.0.9/src/organizations/migrations/0005_subject_alter_organization_networks_and_more.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1712 2023-03-13 16:26:58.000000 organizations-0.0.9/src/organizations/migrations/0006_alter_organization_networks_and_more.py
--rw-r--r--   0 alejandro  (1000) alejandro  (1000)      413 2023-03-15 15:26:45.000000 organizations-0.0.9/src/organizations/migrations/0007_alter_issuer_active.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)        0 2023-03-13 16:26:58.000000 organizations-0.0.9/src/organizations/migrations/__init__.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3378 2023-03-15 15:14:40.000000 organizations-0.0.9/src/organizations/models.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1070 2023-03-13 16:26:58.000000 organizations-0.0.9/src/organizations/serializers.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2327 2023-03-13 16:26:58.000000 organizations-0.0.9/src/organizations/service.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     3206 2023-03-14 14:55:33.000000 organizations-0.0.9/src/organizations/signals.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2578 2023-03-15 15:16:06.000000 organizations-0.0.9/src/organizations/tasks.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       60 2023-03-13 16:26:58.000000 organizations-0.0.9/src/organizations/tests.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      271 2023-03-13 16:26:58.000000 organizations-0.0.9/src/organizations/urls.py
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     2744 2023-03-13 16:26:58.000000 organizations-0.0.9/src/organizations/views.py
-drwxrwxr-x   0 alejandro  (1000) alejandro  (1000)        0 2023-03-16 09:19:18.435685 organizations-0.0.9/src/organizations.egg-info/
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      389 2023-03-16 09:19:18.000000 organizations-0.0.9/src/organizations.egg-info/PKG-INFO
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)     1379 2023-03-16 09:19:18.000000 organizations-0.0.9/src/organizations.egg-info/SOURCES.txt
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)        1 2023-03-16 09:19:18.000000 organizations-0.0.9/src/organizations.egg-info/dependency_links.txt
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)      307 2023-03-16 09:19:18.000000 organizations-0.0.9/src/organizations.egg-info/requires.txt
--rw-rw-r--   0 alejandro  (1000) alejandro  (1000)       14 2023-03-16 09:19:18.000000 organizations-0.0.9/src/organizations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 12:35:01.060121 organizations-0.1.0/
+-rw-rw-rw-   0        0        0     1091 2023-04-21 11:42:03.000000 organizations-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      434 2023-05-03 12:35:01.059123 organizations-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-21 11:42:03.000000 organizations-0.1.0/README.md
+-rw-rw-rw-   0        0        0     1083 2023-05-03 12:33:31.000000 organizations-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 12:35:01.061122 organizations-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 12:35:00.949126 organizations-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 12:35:00.993127 organizations-0.1.0/src/organizations/
+-rw-rw-rw-   0        0        0        0 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/__init__.py
+-rw-rw-rw-   0        0        0      664 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/abstractions.py
+-rw-rw-rw-   0        0        0     5265 2023-05-03 11:22:44.000000 organizations-0.1.0/src/organizations/admin.py
+-rw-rw-rw-   0        0        0      234 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/apps.py
+drwxrwxrwx   0        0        0        0 2023-05-03 12:35:01.021122 organizations-0.1.0/src/organizations/did_factory/
+-rw-rw-rw-   0        0        0        0 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/did_factory/__init__.py
+-rw-rw-rw-   0        0        0     1225 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/did_factory/abstractions.py
+-rw-rw-rw-   0        0        0      247 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/did_factory/context.py
+-rw-rw-rw-   0        0        0      816 2023-04-27 10:52:27.000000 organizations-0.1.0/src/organizations/did_factory/factory.py
+-rw-rw-rw-   0        0        0      173 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/did_factory/models.py
+-rw-rw-rw-   0        0        0    11061 2023-05-03 09:53:36.000000 organizations-0.1.0/src/organizations/did_factory/strategy.py
+-rw-rw-rw-   0        0        0      241 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/enums.py
+-rw-rw-rw-   0        0        0      712 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/forms.py
+drwxrwxrwx   0        0        0        0 2023-05-03 12:35:01.056123 organizations-0.1.0/src/organizations/migrations/
+-rw-rw-rw-   0        0        0     4963 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      720 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/migrations/0002_organization_networks.py
+-rw-rw-rw-   0        0        0      673 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/migrations/0003_alter_organization_networks.py
+-rw-rw-rw-   0        0        0      867 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/migrations/0004_alter_organization_email_and_more.py
+-rw-rw-rw-   0        0        0     3698 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/migrations/0005_subject_alter_organization_networks_and_more.py
+-rw-rw-rw-   0        0        0     1767 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/migrations/0006_alter_organization_networks_and_more.py
+-rw-rw-rw-   0        0        0      431 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/migrations/0007_alter_issuer_active.py
+-rw-rw-rw-   0        0        0      569 2023-04-27 13:47:50.000000 organizations-0.1.0/src/organizations/migrations/0008_alter_organization_networks.py
+-rw-rw-rw-   0        0        0      411 2023-05-02 15:49:34.000000 organizations-0.1.0/src/organizations/migrations/0009_issuer_name.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3613 2023-05-03 09:45:48.000000 organizations-0.1.0/src/organizations/models.py
+-rw-rw-rw-   0        0        0     1104 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/serializers.py
+-rw-rw-rw-   0        0        0     2391 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/service.py
+-rw-rw-rw-   0        0        0     3293 2023-05-03 12:34:28.000000 organizations-0.1.0/src/organizations/signals.py
+-rw-rw-rw-   0        0        0     2643 2023-05-03 12:34:37.000000 organizations-0.1.0/src/organizations/tasks.py
+-rw-rw-rw-   0        0        0       63 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/tests.py
+-rw-rw-rw-   0        0        0      282 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/urls.py
+-rw-rw-rw-   0        0        0     2820 2023-04-21 11:42:03.000000 organizations-0.1.0/src/organizations/views.py
+drwxrwxrwx   0        0        0        0 2023-05-03 12:35:01.005121 organizations-0.1.0/src/organizations.egg-info/
+-rw-rw-rw-   0        0        0      434 2023-05-03 12:35:00.000000 organizations-0.1.0/src/organizations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1493 2023-05-03 12:35:00.000000 organizations-0.1.0/src/organizations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 12:35:00.000000 organizations-0.1.0/src/organizations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      327 2023-05-03 12:35:00.000000 organizations-0.1.0/src/organizations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-03 12:35:00.000000 organizations-0.1.0/src/organizations.egg-info/top_level.txt
```

### Comparing `organizations-0.0.9/LICENSE` & `organizations-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `organizations-0.0.9/pyproject.toml` & `organizations-0.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,42 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "organizations"
-version = "0.0.9"
-authors = [
-  { name="Alejandro", email="agarrido@izertis.com" },
-]
-description = "A small organizations handler app for django"
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-dependencies = [
-  'alastria-identity',
-  'Django==4.1.3',
-  'djangorestframework==3.14.0',
-  'drf-yasg==1.21.4',
-  'pillow==9.3.0',
-  'pyjwt==2.6.0',
-  'qrcode==7.3.1',
-  'web3==5.31.3',
-  'network-service-client==0.0.2',
-  'alastria-service-client==0.0.12',
-  'django-waffle==3.0.0',
-  'celery==5.2.7',
-  'django-multiselectfield==0.1.12',
-  'mnemonic==0.20',
-  'templates-service-client==0.0.1',
-]
-[tool.setuptools.packages.find]
-where = ["src"]
-
-[tool.setuptools.package-data]
-"*" = ["*.html"]
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "organizations"
+version = "0.1.0"
+authors = [
+  { name="Alejandro", email="agarrido@izertis.com" },
+  { name="Iraia", email="iolabarrieta@izertis.com" },
+]
+description = "A small organizations handler app for django"
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dependencies = [
+  'alastria-identity',
+  'Django==4.1.3',
+  'djangorestframework==3.14.0',
+  'drf-yasg==1.21.4',
+  'pillow==9.3.0',
+  'pyjwt==2.6.0',
+  'qrcode==7.3.1',
+  'web3==5.31.3',
+  'network-service-client==0.0.4',
+  'alastria-service-client==0.0.12',
+  'django-waffle==3.0.0',
+  'celery==5.2.7',
+  'django-multiselectfield==0.1.12',
+  'mnemonic==0.20',
+  'templates-service-client==0.0.1',
+  'multiformats==0.2.1',
+]
+[tool.setuptools.packages.find]
+where = ["src"]
+
+[tool.setuptools.package-data]
+"*" = ["*.html"]
```

### Comparing `organizations-0.0.9/src/organizations/abstractions.py` & `organizations-0.1.0/src/organizations/abstractions.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from __future__ import annotations
-from abc import ABC, abstractmethod
-from .models import Organization
-from typing import List
-from network_service_client.client import NetworksNames
-
-
-class AOrganizationsService(ABC):
-    @staticmethod
-    @abstractmethod
-    def get_organization_by_operator_email(email: str) -> Organization | None:
-        ...
-
-    @staticmethod
-    @abstractmethod
-    def set_did(email: str, did: str, network_name: str) -> None:
-        ...
-
-    @staticmethod
-    @abstractmethod
-    def get_did(
-        create_alastria_tx: str,
-        subject_address: str,
-        email: str,
-    ) -> List[dict]:
-        ...
+from __future__ import annotations
+from abc import ABC, abstractmethod
+from .models import Organization
+from typing import List
+from network_service_client.client import NetworksNames
+
+
+class AOrganizationsService(ABC):
+    @staticmethod
+    @abstractmethod
+    def get_organization_by_operator_email(email: str) -> Organization | None:
+        ...
+
+    @staticmethod
+    @abstractmethod
+    def set_did(email: str, did: str, network_name: str) -> None:
+        ...
+
+    @staticmethod
+    @abstractmethod
+    def get_did(
+        create_alastria_tx: str,
+        subject_address: str,
+        email: str,
+    ) -> List[dict]:
+        ...
```

### Comparing `organizations-0.0.9/src/organizations/admin.py` & `organizations-0.1.0/src/organizations/admin.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,167 +1,174 @@
-from django.contrib import admin
-from .models import (
-    Intermediary,
-    Organization,
-    OrganizationDID,
-    OrganizationKeys,
-    Issuer,
-    UserProxy,
-    OperatorDID,
-    Subject,
-    SubjectDID,
-    OrganizationOnboardingNotification,
-)
-from .enums import OrganizationsSwitches
-import waffle
-from .forms import UserProxyForm
-
-
-class OperatorDIDAdmin(admin.ModelAdmin):
-    model = OperatorDID
-
-    def get_model_perms(self, request):
-
-        if not waffle.switch_is_active(OrganizationsSwitches.Organizations.value):
-            return {}
-
-        return super(OperatorDIDAdmin, self).get_model_perms(request)
-
-
-class SubjectDIDAdmin(admin.ModelAdmin):
-    model = SubjectDID
-
-    def get_model_perms(self, request):
-
-        if (
-            not waffle.switch_is_active(OrganizationsSwitches.Organizations.value)
-            or waffle.switch_is_active(OrganizationsSwitches.Organizations.value)
-            and not waffle.switch_is_active(
-                OrganizationsSwitches.OrganizationsIntermediary.value
-            )
-        ):
-            return {}
-
-        return super(SubjectDIDAdmin, self).get_model_perms(request)
-
-
-class SubjectAdmin(admin.ModelAdmin):
-    model = Subject
-
-    def get_model_perms(self, request):
-
-        if (
-            not waffle.switch_is_active(OrganizationsSwitches.Organizations.value)
-            or waffle.switch_is_active(OrganizationsSwitches.Organizations.value)
-            and not waffle.switch_is_active(
-                OrganizationsSwitches.OrganizationsIntermediary.value
-            )
-        ):
-            return {}
-
-        return super(SubjectAdmin, self).get_model_perms(request)
-
-
-class IntermediaryAdmin(admin.ModelAdmin):
-    model = Intermediary
-
-    def get_model_perms(self, request):
-
-        if (
-            not waffle.switch_is_active(OrganizationsSwitches.Organizations.value)
-            or waffle.switch_is_active(OrganizationsSwitches.Organizations.value)
-            and not waffle.switch_is_active(
-                OrganizationsSwitches.OrganizationsIntermediary.value
-            )
-        ):
-            return {}
-
-        return super(IntermediaryAdmin, self).get_model_perms(request)
-
-
-class OrganizationAdmin(admin.ModelAdmin):
-    model = Organization
-
-    def get_model_perms(self, request):
-
-        if not waffle.switch_is_active(OrganizationsSwitches.Organizations.value):
-            return {}
-
-        return super(OrganizationAdmin, self).get_model_perms(request)
-
-
-class OrganizationDIDAdmin(admin.ModelAdmin):
-    model = OrganizationDID
-
-    def get_model_perms(self, request):
-
-        if not waffle.switch_is_active(OrganizationsSwitches.Organizations.value):
-            return {}
-
-        return super(OrganizationDIDAdmin, self).get_model_perms(request)
-
-
-class OrganizationKeysAdmin(admin.ModelAdmin):
-    model = OrganizationKeys
-
-    def get_model_perms(self, request):
-
-        if not waffle.switch_is_active(OrganizationsSwitches.Organizations.value):
-            return {}
-
-        return super(OrganizationKeysAdmin, self).get_model_perms(request)
-
-
-class IssuerAdmin(admin.ModelAdmin):
-    model = Issuer
-    readonly_fields = ["active"]
-
-    def get_model_perms(self, request):
-
-        if (
-            not waffle.switch_is_active(OrganizationsSwitches.Organizations.value)
-            or waffle.switch_is_active(OrganizationsSwitches.Organizations.value)
-            and not waffle.switch_is_active(
-                OrganizationsSwitches.OrganizationsIssuer.value
-            )
-        ):
-            return {}
-
-        return super(IssuerAdmin, self).get_model_perms(request)
-
-
-class UserProxyAdmin(admin.ModelAdmin):
-    form = UserProxyForm
-
-    def get_model_perms(self, request):
-
-        if not waffle.switch_is_active(OrganizationsSwitches.Organizations.value):
-            return {}
-
-        return super(UserProxyAdmin, self).get_model_perms(request)
-
-
-class OrganizationOnboardingNotificationAdmin(admin.ModelAdmin):
-    model = OrganizationOnboardingNotification
-
-    def get_model_perms(self, request):
-
-        if not waffle.switch_is_active(OrganizationsSwitches.Organizations.value):
-            return {}
-
-        return super(OrganizationOnboardingNotificationAdmin, self).get_model_perms(
-            request
-        )
-
-
-admin.site.register(
-    OrganizationOnboardingNotification, OrganizationOnboardingNotificationAdmin
-)
-admin.site.register(SubjectDID, SubjectDIDAdmin)
-admin.site.register(Subject, SubjectAdmin)
-admin.site.register(OperatorDID, OperatorDIDAdmin)
-admin.site.register(Intermediary, IntermediaryAdmin)
-admin.site.register(Organization, OrganizationAdmin)
-admin.site.register(OrganizationDID, OrganizationDIDAdmin)
-admin.site.register(OrganizationKeys, OrganizationKeysAdmin)
-admin.site.register(Issuer, IssuerAdmin)
-admin.site.register(UserProxy, UserProxyAdmin)
+from django.contrib import admin
+from .models import (
+    Intermediary,
+    Organization,
+    OrganizationDID,
+    OrganizationKeys,
+    Issuer,
+    UserProxy,
+    OperatorDID,
+    Subject,
+    SubjectDID,
+    OrganizationOnboardingNotification,
+)
+from .enums import OrganizationsSwitches
+import waffle
+from .forms import UserProxyForm
+
+
+class OperatorDIDAdmin(admin.ModelAdmin):
+    model = OperatorDID
+
+    def get_model_perms(self, request):
+
+        if not waffle.switch_is_active(OrganizationsSwitches.Organizations.value):
+            return {}
+
+        return super(OperatorDIDAdmin, self).get_model_perms(request)
+
+
+class SubjectDIDAdmin(admin.ModelAdmin):
+    model = SubjectDID
+
+    def get_model_perms(self, request):
+
+        if (
+            not waffle.switch_is_active(OrganizationsSwitches.Organizations.value)
+            or waffle.switch_is_active(OrganizationsSwitches.Organizations.value)
+            and not waffle.switch_is_active(
+                OrganizationsSwitches.OrganizationsIntermediary.value
+            )
+        ):
+            return {}
+
+        return super(SubjectDIDAdmin, self).get_model_perms(request)
+
+
+class SubjectAdmin(admin.ModelAdmin):
+    model = Subject
+
+    def get_model_perms(self, request):
+
+        if (
+            not waffle.switch_is_active(OrganizationsSwitches.Organizations.value)
+            or waffle.switch_is_active(OrganizationsSwitches.Organizations.value)
+            and not waffle.switch_is_active(
+                OrganizationsSwitches.OrganizationsIntermediary.value
+            )
+        ):
+            return {}
+
+        return super(SubjectAdmin, self).get_model_perms(request)
+
+
+class IntermediaryAdmin(admin.ModelAdmin):
+    model = Intermediary
+
+    def get_model_perms(self, request):
+
+        if (
+            not waffle.switch_is_active(OrganizationsSwitches.Organizations.value)
+            or waffle.switch_is_active(OrganizationsSwitches.Organizations.value)
+            and not waffle.switch_is_active(
+                OrganizationsSwitches.OrganizationsIntermediary.value
+            )
+        ):
+            return {}
+
+        return super(IntermediaryAdmin, self).get_model_perms(request)
+
+
+class OrganizationAdmin(admin.ModelAdmin):
+    model = Organization
+    list_filter = ['networks']
+    search_fields = ['name', 'email', 'phone',]
+    
+    def get_model_perms(self, request):
+
+        if not waffle.switch_is_active(OrganizationsSwitches.Organizations.value):
+            return {}
+
+        return super(OrganizationAdmin, self).get_model_perms(request)
+
+
+class OrganizationDIDAdmin(admin.ModelAdmin):
+    model = OrganizationDID
+    list_filter = ['network_name', 'organization']
+    search_fields = ['network_name', 'organization', 'did',]
+    
+    def get_model_perms(self, request):
+
+        if not waffle.switch_is_active(OrganizationsSwitches.Organizations.value):
+            return {}
+
+        return super(OrganizationDIDAdmin, self).get_model_perms(request)
+
+
+class OrganizationKeysAdmin(admin.ModelAdmin):
+    model = OrganizationKeys
+
+    def get_model_perms(self, request):
+
+        if not waffle.switch_is_active(OrganizationsSwitches.Organizations.value):
+            return {}
+
+        return super(OrganizationKeysAdmin, self).get_model_perms(request)
+
+
+class IssuerAdmin(admin.ModelAdmin):
+    model = Issuer
+    readonly_fields = ["active"]
+    list_filter = ['organization']
+
+
+    def get_model_perms(self, request):
+
+        if (
+            not waffle.switch_is_active(OrganizationsSwitches.Organizations.value)
+            or waffle.switch_is_active(OrganizationsSwitches.Organizations.value)
+            and not waffle.switch_is_active(
+                OrganizationsSwitches.OrganizationsIssuer.value
+            )
+        ):
+            return {}
+
+        return super(IssuerAdmin, self).get_model_perms(request)
+
+
+class UserProxyAdmin(admin.ModelAdmin):
+    form = UserProxyForm
+
+    def get_model_perms(self, request):
+
+        if not waffle.switch_is_active(OrganizationsSwitches.Organizations.value):
+            return {}
+
+        return super(UserProxyAdmin, self).get_model_perms(request)
+
+
+class OrganizationOnboardingNotificationAdmin(admin.ModelAdmin):
+    model = OrganizationOnboardingNotification
+    list_filter = ['organization']
+    
+    def get_model_perms(self, request):
+
+        if not waffle.switch_is_active(OrganizationsSwitches.Organizations.value):
+            return {}
+
+        return super(OrganizationOnboardingNotificationAdmin, self).get_model_perms(
+            request
+        )
+
+
+admin.site.register(
+    OrganizationOnboardingNotification, OrganizationOnboardingNotificationAdmin
+)
+admin.site.register(SubjectDID, SubjectDIDAdmin)
+admin.site.register(Subject, SubjectAdmin)
+admin.site.register(OperatorDID, OperatorDIDAdmin)
+admin.site.register(Intermediary, IntermediaryAdmin)
+admin.site.register(Organization, OrganizationAdmin)
+admin.site.register(OrganizationDID, OrganizationDIDAdmin)
+admin.site.register(OrganizationKeys, OrganizationKeysAdmin)
+admin.site.register(Issuer, IssuerAdmin)
+admin.site.register(UserProxy, UserProxyAdmin)
```

### Comparing `organizations-0.0.9/src/organizations/did_factory/factory.py` & `organizations-0.1.0/src/organizations/did_factory/factory.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,22 @@
-from .abstractions import AFactory, AContext
-from .strategy import AlastriaNetworkStrategy, LacchainNetworkStrategy
-from .context import Context
-from network_service_client.client import NetworksNames
-from .models import FactoryArgsModel
-
-
-class Creator(AFactory):
-    @staticmethod
-    def create_object(props: FactoryArgsModel) -> AContext:
-
-        if props.net.name == NetworksNames.AlastriaDefaultName:
-            return Context(AlastriaNetworkStrategy(props))
-        if props.net.name == NetworksNames.LacchainDefaultName:
-            return Context(LacchainNetworkStrategy(props))
-        raise Exception("Cant find any strategy.")
+from .abstractions import AFactory, AContext
+from .strategy import (
+    AlastriaNetworkStrategy,
+    EbsiNetworkStrategy,
+    LacchainNetworkStrategy,
+)
+from .context import Context
+from network_service_client.client import NetworksNames
+from .models import FactoryArgsModel
+
+
+class Creator(AFactory):
+    @staticmethod
+    def create_object(props: FactoryArgsModel) -> AContext:
+
+        if props.net.name == NetworksNames.AlastriaDefaultName:
+            return Context(AlastriaNetworkStrategy(props))
+        if props.net.name == NetworksNames.LacchainDefaultName:
+            return Context(LacchainNetworkStrategy(props))
+        if props.net.name == NetworksNames.EbsiDefaultName:
+            return Context(EbsiNetworkStrategy(props))
+        raise Exception("Cant find any strategy.")
```

### Comparing `organizations-0.0.9/src/organizations/did_factory/strategy.py` & `organizations-0.1.0/src/organizations/did_factory/strategy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,249 +1,287 @@
-from .abstractions import ANetworkStrategy
-from alastria_service_client.client import (
-    AClient as AlastriaAClinet,
-    Client as AlastriaClient,
-)
-from .models import FactoryArgsModel
-from network_service_client.enums import ContractsNames
-from alastria_service_client.validators import (
-    Address,
-    NetworkValidator,
-    OnlyNetworkValidator,
-    SignatureValidator,
-    RunRawTransaction,
-    PrepareIDValidator,
-    DelegateCallValidator,
-    CreateAlastriaIdentityValidator,
-    AddKeyValidator,
-    AddIdentityIssuerValidator,
-    EidasLevelEnum,
-)
-from django.conf import settings
-
-
-class AlastriaNetworkStrategy(ANetworkStrategy):
-    def __init__(self, props: FactoryArgsModel):
-        self.alastria_service_client: AlastriaAClinet = AlastriaClient(
-            service_host=settings.ALASTRIA_SERVICE_HOST
-        )
-        self.props = props
-        network_data = self.props.net
-        self.network_body = NetworkValidator(
-            provider=network_data.node["path"],
-            identity_manager_contract_address=list(
-                filter(
-                    lambda contract: contract["name"]
-                    == ContractsNames.AlastriaIdentityManager.value,
-                    network_data.contracts,
-                )
-            )[0]["address"],
-            identity_manager_contract_abi=list(
-                filter(
-                    lambda contract: contract["name"]
-                    == ContractsNames.AlastriaIdentityManager.value,
-                    network_data.contracts,
-                )
-            )[0]["abi"],
-            public_key_registry_contract_address=list(
-                filter(
-                    lambda contract: contract["name"]
-                    == ContractsNames.AlastriaPublicKeyRegistry.value,
-                    network_data.contracts,
-                )
-            )[0]["address"],
-            public_key_registry_contract_abi=list(
-                filter(
-                    lambda contract: contract["name"]
-                    == ContractsNames.AlastriaPublicKeyRegistry.value,
-                    network_data.contracts,
-                )
-            )[0]["abi"],
-            credential_registry_contract_abi=list(
-                filter(
-                    lambda contract: contract["name"]
-                    == ContractsNames.AlastriaCredentialRegistry.value,
-                    network_data.contracts,
-                )
-            )[0]["abi"],
-            credential_registry_contract_address=list(
-                filter(
-                    lambda contract: contract["name"]
-                    == ContractsNames.AlastriaCredentialRegistry.value,
-                    network_data.contracts,
-                )
-            )[0]["address"],
-            chainId=network_data.chain_id,
-        )
-
-    def register_issuer(
-        self,
-        new_issuer_address: Address = Address(""),
-        issuer_address: Address = Address(""),
-        issuer_private_key: str = "",
-    ) -> str:
-        self.alastria_service_client.run_raw_transaction(
-            RunRawTransaction(
-                raw_transaction=self.alastria_service_client.signature(
-                    SignatureValidator(
-                        transaction=self.alastria_service_client.delegate_call(
-                            DelegateCallValidator(
-                                data=self.alastria_service_client.add_identity_issuer(
-                                    AddIdentityIssuerValidator(
-                                        new_issuer_address=new_issuer_address,
-                                        network=self.network_body,
-                                        eidas_level=EidasLevelEnum.Low,
-                                    )
-                                ).response,
-                                issuer_address=issuer_address,
-                                network=self.network_body,
-                            ),
-                        ).response,
-                        private_key=issuer_private_key,
-                        network=self.network_body,
-                    )
-                ).response,
-                network=self.network_body,
-            )
-        )
-        return "OK"
-
-    def create_did(
-        self,
-        sign_address: Address = Address(""),
-        issuer_address: Address = Address(""),
-        public_key: str = "",
-        issuer_private_key: str = "",
-        new_issuer_private_key: str = "",
-    ) -> str:
-        self.alastria_service_client.run_raw_transaction(
-            RunRawTransaction(
-                raw_transaction=self.alastria_service_client.signature(
-                    SignatureValidator(
-                        transaction=self.alastria_service_client.delegate_call(
-                            DelegateCallValidator(
-                                data=self.alastria_service_client.prepare_alastria_id_encode_abi(
-                                    PrepareIDValidator(
-                                        sign_address=sign_address,
-                                        network=self.network_body,
-                                    )
-                                ).response,
-                                issuer_address=issuer_address,
-                                network=self.network_body,
-                            ),
-                        ).response,
-                        private_key=issuer_private_key,
-                        network=self.network_body,
-                    )
-                ).response,
-                network=self.network_body,
-            )
-        )
-        self.alastria_service_client.run_raw_transaction(
-            RunRawTransaction(
-                raw_transaction=self.alastria_service_client.signature(
-                    SignatureValidator(
-                        transaction=self.alastria_service_client.create_alastria_identity(
-                            CreateAlastriaIdentityValidator(
-                                add_public_key_call_data=self.alastria_service_client.add_key(
-                                    AddKeyValidator(
-                                        public_key=public_key,
-                                        network=self.network_body,
-                                    )
-                                ).response,
-                                issuer_address=sign_address,
-                                network=self.network_body,
-                            )
-                        ).response,
-                        private_key=new_issuer_private_key.encode("utf-8").strip(),
-                        network=self.network_body,
-                    )
-                ).response,
-                network=self.network_body,
-            )
-        )
-
-        return (
-            self.props.net.did_prefix
-            + self.alastria_service_client.identity_keys(
-                sign_address, OnlyNetworkValidator(network=self.network_body)
-            ).response[2:]
-        )
-
-    def create_did_from_external_source(
-        self,
-        tx: str,
-        subject_address: Address = Address(""),
-        issuer_address: Address = Address(""),
-        issuer_private_key: str = "",
-    ) -> str:
-
-        self.alastria_service_client.run_raw_transaction(
-            RunRawTransaction(
-                raw_transaction=self.alastria_service_client.signature(
-                    SignatureValidator(
-                        transaction=self.alastria_service_client.delegate_call(
-                            DelegateCallValidator(
-                                data=self.alastria_service_client.prepare_alastria_id_encode_abi(
-                                    PrepareIDValidator(
-                                        sign_address=Address(subject_address),
-                                        network=self.network_body,
-                                    )
-                                ).response,
-                                issuer_address=Address(issuer_address),
-                                network=self.network_body,
-                            )
-                        ).response,
-                        private_key=issuer_private_key,
-                        network=self.network_body,
-                    )
-                ).response,
-                network=self.network_body,
-            )
-        )
-        self.alastria_service_client.run_raw_transaction(
-            RunRawTransaction(raw_transaction=tx, network=self.network_body)
-        )
-        return (
-            self.props.net.did_prefix
-            + self.alastria_service_client.identity_keys(
-                Address(subject_address),
-                OnlyNetworkValidator(network=self.network_body),
-            ).response[2:]
-        )
-
-
-class LacchainNetworkStrategy(ANetworkStrategy):
-    def __init__(self, props: FactoryArgsModel):
-        self.props = props
-        self.prefix = props.net.did_prefix
-
-    def create_did(
-        self,
-        signAddress: Address = Address(""),
-        issuer_address: Address = Address(""),
-        public_key: str = "",
-        issuer_private_key: str = "",
-        new_issuer_private_key: str = "",
-    ) -> str:
-
-        # DID
-        did = self.prefix + issuer_address
-        return did
-
-    def create_did_from_external_source(
-        self,
-        tx: str,
-        subject_address: Address = Address(""),
-        issuer_address: Address = Address(""),
-        issuer_private_key: str = "",
-    ) -> str:
-        did = self.prefix + subject_address
-        return did
-
-    def register_issuer(
-        self,
-        new_issuer_address: Address = Address(""),
-        issuer_address: Address = Address(""),
-        issuer_private_key: str = "",
-    ) -> str:
-        return "OK"
+import random
+from .abstractions import ANetworkStrategy
+from alastria_service_client.client import (
+    AClient as AlastriaAClinet,
+    Client as AlastriaClient,
+)
+from .models import FactoryArgsModel
+from network_service_client.enums import ContractsNames
+from alastria_service_client.validators import (
+    Address,
+    NetworkValidator,
+    OnlyNetworkValidator,
+    SignatureValidator,
+    RunRawTransaction,
+    PrepareIDValidator,
+    DelegateCallValidator,
+    CreateAlastriaIdentityValidator,
+    AddKeyValidator,
+    AddIdentityIssuerValidator,
+    EidasLevelEnum,
+)
+from django.conf import settings
+from multiformats import multibase
+
+class AlastriaNetworkStrategy(ANetworkStrategy):
+    def __init__(self, props: FactoryArgsModel):
+        self.alastria_service_client: AlastriaAClinet = AlastriaClient(
+            service_host=settings.ALASTRIA_SERVICE_HOST
+        )
+        self.props = props
+        network_data = self.props.net
+        self.network_body = NetworkValidator(
+            provider=network_data.node["path"],
+            identity_manager_contract_address=list(
+                filter(
+                    lambda contract: contract["name"]
+                    == ContractsNames.AlastriaIdentityManager.value,
+                    network_data.contracts,
+                )
+            )[0]["address"],
+            identity_manager_contract_abi=list(
+                filter(
+                    lambda contract: contract["name"]
+                    == ContractsNames.AlastriaIdentityManager.value,
+                    network_data.contracts,
+                )
+            )[0]["abi"],
+            public_key_registry_contract_address=list(
+                filter(
+                    lambda contract: contract["name"]
+                    == ContractsNames.AlastriaPublicKeyRegistry.value,
+                    network_data.contracts,
+                )
+            )[0]["address"],
+            public_key_registry_contract_abi=list(
+                filter(
+                    lambda contract: contract["name"]
+                    == ContractsNames.AlastriaPublicKeyRegistry.value,
+                    network_data.contracts,
+                )
+            )[0]["abi"],
+            credential_registry_contract_abi=list(
+                filter(
+                    lambda contract: contract["name"]
+                    == ContractsNames.AlastriaCredentialRegistry.value,
+                    network_data.contracts,
+                )
+            )[0]["abi"],
+            credential_registry_contract_address=list(
+                filter(
+                    lambda contract: contract["name"]
+                    == ContractsNames.AlastriaCredentialRegistry.value,
+                    network_data.contracts,
+                )
+            )[0]["address"],
+            chainId=network_data.chain_id,
+        )
+
+    def register_issuer(
+        self,
+        new_issuer_address: Address = Address(""),
+        issuer_address: Address = Address(""),
+        issuer_private_key: str = "",
+    ) -> str:
+        self.alastria_service_client.run_raw_transaction(
+            RunRawTransaction(
+                raw_transaction=self.alastria_service_client.signature(
+                    SignatureValidator(
+                        transaction=self.alastria_service_client.delegate_call(
+                            DelegateCallValidator(
+                                data=self.alastria_service_client.add_identity_issuer(
+                                    AddIdentityIssuerValidator(
+                                        new_issuer_address=new_issuer_address,
+                                        network=self.network_body,
+                                        eidas_level=EidasLevelEnum.Low,
+                                    )
+                                ).response,
+                                issuer_address=issuer_address,
+                                network=self.network_body,
+                            ),
+                        ).response,
+                        private_key=issuer_private_key,
+                        network=self.network_body,
+                    )
+                ).response,
+                network=self.network_body,
+            )
+        )
+        return "OK"
+
+    def create_did(
+        self,
+        sign_address: Address = Address(""),
+        issuer_address: Address = Address(""),
+        public_key: str = "",
+        issuer_private_key: str = "",
+        new_issuer_private_key: str = "",
+    ) -> str:
+        self.alastria_service_client.run_raw_transaction(
+            RunRawTransaction(
+                raw_transaction=self.alastria_service_client.signature(
+                    SignatureValidator(
+                        transaction=self.alastria_service_client.delegate_call(
+                            DelegateCallValidator(
+                                data=self.alastria_service_client.prepare_alastria_id_encode_abi(
+                                    PrepareIDValidator(
+                                        sign_address=sign_address,
+                                        network=self.network_body,
+                                    )
+                                ).response,
+                                issuer_address=issuer_address,
+                                network=self.network_body,
+                            ),
+                        ).response,
+                        private_key=issuer_private_key,
+                        network=self.network_body,
+                    )
+                ).response,
+                network=self.network_body,
+            )
+        )
+        self.alastria_service_client.run_raw_transaction(
+            RunRawTransaction(
+                raw_transaction=self.alastria_service_client.signature(
+                    SignatureValidator(
+                        transaction=self.alastria_service_client.create_alastria_identity(
+                            CreateAlastriaIdentityValidator(
+                                add_public_key_call_data=self.alastria_service_client.add_key(
+                                    AddKeyValidator(
+                                        public_key=public_key,
+                                        network=self.network_body,
+                                    )
+                                ).response,
+                                issuer_address=sign_address,
+                                network=self.network_body,
+                            )
+                        ).response,
+                        private_key=new_issuer_private_key.encode("utf-8").strip(),
+                        network=self.network_body,
+                    )
+                ).response,
+                network=self.network_body,
+            )
+        )
+
+        return (
+            self.props.net.did_prefix
+            + self.alastria_service_client.identity_keys(
+                sign_address, OnlyNetworkValidator(network=self.network_body)
+            ).response[2:]
+        )
+
+    def create_did_from_external_source(
+        self,
+        tx: str,
+        subject_address: Address = Address(""),
+        issuer_address: Address = Address(""),
+        issuer_private_key: str = "",
+    ) -> str:
+
+        self.alastria_service_client.run_raw_transaction(
+            RunRawTransaction(
+                raw_transaction=self.alastria_service_client.signature(
+                    SignatureValidator(
+                        transaction=self.alastria_service_client.delegate_call(
+                            DelegateCallValidator(
+                                data=self.alastria_service_client.prepare_alastria_id_encode_abi(
+                                    PrepareIDValidator(
+                                        sign_address=Address(subject_address),
+                                        network=self.network_body,
+                                    )
+                                ).response,
+                                issuer_address=Address(issuer_address),
+                                network=self.network_body,
+                            )
+                        ).response,
+                        private_key=issuer_private_key,
+                        network=self.network_body,
+                    )
+                ).response,
+                network=self.network_body,
+            )
+        )
+        self.alastria_service_client.run_raw_transaction(
+            RunRawTransaction(raw_transaction=tx, network=self.network_body)
+        )
+        return (
+            self.props.net.did_prefix
+            + self.alastria_service_client.identity_keys(
+                Address(subject_address),
+                OnlyNetworkValidator(network=self.network_body),
+            ).response[2:]
+        )
+
+
+class LacchainNetworkStrategy(ANetworkStrategy):
+    def __init__(self, props: FactoryArgsModel):
+        self.props = props
+        self.prefix = props.net.did_prefix
+
+    def create_did(
+        self,
+        signAddress: Address = Address(""),
+        issuer_address: Address = Address(""),
+        public_key: str = "",
+        issuer_private_key: str = "",
+        new_issuer_private_key: str = "",
+    ) -> str:
+
+        # DID
+        did = self.prefix + signAddress
+        return did
+
+    def create_did_from_external_source(
+        self,
+        tx: str,
+        subject_address: Address = Address(""),
+        issuer_address: Address = Address(""),
+        issuer_private_key: str = "",
+    ) -> str:
+        did = self.prefix + subject_address
+        return did
+
+    def register_issuer(
+        self,
+        new_issuer_address: Address = Address(""),
+        issuer_address: Address = Address(""),
+        issuer_private_key: str = "",
+    ) -> str:
+        return "OK"
+
+
+class EbsiNetworkStrategy(ANetworkStrategy):
+    def __init__(self, props: FactoryArgsModel):
+        self.props = props
+        self.prefix = props.net.did_prefix
+
+    def create_did(
+        self,
+        signAddress: Address = Address(""),
+        issuer_address: Address = Address(""),
+        public_key: str = "",
+        issuer_private_key: str = "",
+        new_issuer_private_key: str = "",
+    ) -> str:
+
+        randomBytes = random.randbytes(16)
+        did = self.prefix + multibase.encode(randomBytes, "base58btc")
+        return did
+
+    def create_did_from_external_source(
+        self,
+        tx: str,
+        subject_address: Address = Address(""),
+        issuer_address: Address = Address(""),
+        issuer_private_key: str = "",
+    ) -> str:
+        did = self.prefix + subject_address
+        return did
+
+    def register_issuer(
+        self,
+        new_issuer_address: Address = Address(""),
+        issuer_address: Address = Address(""),
+        issuer_private_key: str = "",
+    ) -> str:
+        return "OK"
```

### Comparing `organizations-0.0.9/src/organizations/forms.py` & `organizations-0.1.0/src/organizations/forms.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from django.forms import ModelForm
-from .models import UserProxy
-from django import forms
-from uuid import uuid4
-
-
-def email_unique(value):
-    if UserProxy.objects.filter(email=value).first():
-        raise forms.ValidationError("That email already exists.")
-
-
-class UserProxyForm(ModelForm):
-    username = forms.CharField(max_length=255, required=False, empty_value=str(uuid4()))
-    first_name = forms.CharField(max_length=150, required=False)
-    last_name = forms.CharField(max_length=150, required=False)
-    email = forms.EmailField(required=True, validators=[email_unique])
-
-    class Meta:
-        model = UserProxy
-        fields = ["username", "first_name", "last_name", "email"]
+from django.forms import ModelForm
+from .models import UserProxy
+from django import forms
+from uuid import uuid4
+
+
+def email_unique(value):
+    if UserProxy.objects.filter(email=value).first():
+        raise forms.ValidationError("That email already exists.")
+
+
+class UserProxyForm(ModelForm):
+    username = forms.CharField(max_length=255, required=False, empty_value=str(uuid4()))
+    first_name = forms.CharField(max_length=150, required=False)
+    last_name = forms.CharField(max_length=150, required=False)
+    email = forms.EmailField(required=True, validators=[email_unique])
+
+    class Meta:
+        model = UserProxy
+        fields = ["username", "first_name", "last_name", "email"]
```

### Comparing `organizations-0.0.9/src/organizations/migrations/0002_organization_networks.py` & `organizations-0.1.0/src/organizations/migrations/0003_alter_organization_networks.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-# Generated by Django 4.1.3 on 2023-01-20 10:26
-
-from django.db import migrations
-import multiselectfield.db.fields
-
-
-class Migration(migrations.Migration):
-
-    dependencies = [
-        ("organizations", "0001_initial"),
-    ]
-
-    operations = [
-        migrations.AddField(
-            model_name="organization",
-            name="networks",
-            field=multiselectfield.db.fields.MultiSelectField(
-                choices=[
-                    ("AlastriaDefaultName", "Alastria"),
-                    ("LacchainDefaultName", "Lacchain"),
-                ],
-                default=1,
-                max_length=19,
-            ),
-            preserve_default=False,
-        ),
-    ]
+# Generated by Django 4.1.3 on 2023-01-20 10:27
+
+from django.db import migrations
+import multiselectfield.db.fields
+
+
+class Migration(migrations.Migration):
+
+    dependencies = [
+        ("organizations", "0002_organization_networks"),
+    ]
+
+    operations = [
+        migrations.AlterField(
+            model_name="organization",
+            name="networks",
+            field=multiselectfield.db.fields.MultiSelectField(
+                choices=[
+                    ("AlastriaDefaultName", "Alastria"),
+                    ("LacchainDefaultName", "Lacchain"),
+                ],
+                max_length=1000,
+            ),
+        ),
+    ]
```

### Comparing `organizations-0.0.9/src/organizations/models.py` & `organizations-0.1.0/src/organizations/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,106 +1,107 @@
-from django.db import models
-from django.contrib.auth.models import User
-from django.utils.translation import gettext_lazy as _
-from multiselectfield import MultiSelectField
-from network_service_client.client import NetworksNames
-
-
-class UserProxy(User):
-    class Meta:
-        proxy = True
-        verbose_name = _("Operator")
-        verbose_name_plural = _("Operators")
-
-    def __str__(self):
-        return f"{self.username} - {self.email}"
-
-
-class OrganizationKeys(models.Model):
-    address = models.CharField(max_length=100)
-    private_key = models.CharField(max_length=500)
-    public_key = models.CharField(max_length=500)
-    mnemonic = models.TextField()
-
-    def __str__(self) -> str:
-        return self.address
-
-
-class Organization(models.Model):
-    networks = MultiSelectField(
-        choices=NetworksNames.choices(), max_choices=2, max_length=1000
-    )
-    name = models.CharField(max_length=255)
-    email = models.EmailField(blank=True, null=True)
-    phone = models.CharField(max_length=255, blank=True, null=True)
-    keys = models.ForeignKey(
-        OrganizationKeys, on_delete=models.SET_NULL, blank=True, null=True
-    )
-    operators = models.ManyToManyField(UserProxy, blank=True)
-
-    def __str__(self) -> str:
-        return self.name
-
-
-class OperatorDID(models.Model):
-    network_name = models.CharField(max_length=2500)
-    operator = models.ForeignKey(UserProxy, on_delete=models.CASCADE)
-    did = models.CharField(max_length=255)
-
-    def __str__(self) -> str:
-        return f"{self.operator.email} - {self.network_name} - {self.did}"
-
-
-class OrganizationDID(models.Model):
-    network_name = models.CharField(max_length=2500)
-    organization = models.ForeignKey(Organization, on_delete=models.CASCADE)
-    did = models.CharField(max_length=255)
-
-    def __str__(self) -> str:
-        return self.organization.name
-
-
-class Issuer(models.Model):
-    organization = models.ForeignKey(Organization, on_delete=models.CASCADE)
-    active = models.BooleanField(default=False)
-
-    def __str__(self) -> str:
-        return self.organization.name
-
-
-class Intermediary(models.Model):
-    organization = models.ForeignKey(Organization, on_delete=models.CASCADE)
-    active = models.BooleanField(default=True)
-
-    def __str__(self) -> str:
-        return self.organization.name
-
-
-class Subject(models.Model):
-    email = models.EmailField(_("Email"), max_length=200, null=True, blank=True)
-    givenName = models.CharField(max_length=255, blank=True)
-    familyName = models.CharField(max_length=255, blank=True)
-    birthDate = models.DateField(blank=True, null=True)
-    intermediary = models.ForeignKey(Intermediary, on_delete=models.CASCADE)
-
-    class Meta:
-        verbose_name = _("Subject")
-        verbose_name_plural = _("Subjects")
-
-    def __str__(self) -> str:
-        display_text = self.email
-        return display_text
-
-
-class SubjectDID(models.Model):
-    network_name = models.CharField(max_length=2500)
-    subject = models.ForeignKey(Subject, on_delete=models.CASCADE)
-    did = models.CharField(max_length=255)
-
-    def __str__(self) -> str:
-        return self.organization.name
-
-
-class OrganizationOnboardingNotification(models.Model):
-    organization = models.ForeignKey(Organization, on_delete=models.CASCADE)
-    operator = models.ForeignKey(UserProxy, on_delete=models.CASCADE)
-    sended_at = models.DateTimeField()
+from django.db import models
+from django.contrib.auth.models import User
+from django.utils.translation import gettext_lazy as _
+from multiselectfield import MultiSelectField
+from network_service_client.client import NetworksNames
+
+
+class UserProxy(User):
+    class Meta:
+        proxy = True
+        verbose_name = _("Operator")
+        verbose_name_plural = _("Operators")
+
+    def __str__(self):
+        return f"{self.username} - {self.email}"
+
+
+class OrganizationKeys(models.Model):
+    address = models.CharField(max_length=100)
+    private_key = models.CharField(max_length=500)
+    public_key = models.CharField(max_length=500)
+    mnemonic = models.TextField()
+
+    def __str__(self) -> str:
+        return self.address
+
+
+class Organization(models.Model):
+    networks = MultiSelectField(
+        choices=NetworksNames.choices(), max_choices=2, max_length=1000
+    )
+    name = models.CharField(max_length=255, unique=True)
+    email = models.EmailField(blank=True, null=True)
+    phone = models.CharField(max_length=255, blank=True, null=True)
+    keys = models.ForeignKey(
+        OrganizationKeys, on_delete=models.SET_NULL, blank=True, null=True
+    )
+    operators = models.ManyToManyField(UserProxy, blank=True)
+
+    def __str__(self) -> str:
+        return self.name
+
+
+class OperatorDID(models.Model):
+    network_name = models.CharField(max_length=2500)
+    operator = models.ForeignKey(UserProxy, on_delete=models.CASCADE)
+    did = models.CharField(max_length=255)
+
+    def __str__(self) -> str:
+        return f"{self.operator.email} - {self.network_name} - {self.did}"
+
+
+class OrganizationDID(models.Model):
+    network_name = models.CharField(max_length=2500)
+    organization = models.ForeignKey(Organization, on_delete=models.CASCADE)
+    did = models.CharField(max_length=255)
+
+    def __str__(self) -> str:
+        return f"{self.network_name} - {self.organization.name}"
+
+
+class Issuer(models.Model):
+    name = models.CharField(max_length=2500, null=False, blank=True)
+    organization = models.ForeignKey(Organization, on_delete=models.CASCADE)
+    active = models.BooleanField(default=False)
+
+    def __str__(self) -> str:
+        return f"{self.name} - {self.organization.name}"
+
+
+class Intermediary(models.Model):
+    organization = models.ForeignKey(Organization, on_delete=models.CASCADE)
+    active = models.BooleanField(default=True)
+
+    def __str__(self) -> str:
+        return self.organization.name
+
+
+class Subject(models.Model):
+    email = models.EmailField(_("Email"), max_length=200, null=True, blank=True)
+    givenName = models.CharField(max_length=255, blank=True)
+    familyName = models.CharField(max_length=255, blank=True)
+    birthDate = models.DateField(blank=True, null=True)
+    intermediary = models.ForeignKey(Intermediary, on_delete=models.CASCADE)
+
+    class Meta:
+        verbose_name = _("Subject")
+        verbose_name_plural = _("Subjects")
+
+    def __str__(self) -> str:
+        display_text = self.email
+        return display_text
+
+
+class SubjectDID(models.Model):
+    network_name = models.CharField(max_length=2500)
+    subject = models.ForeignKey(Subject, on_delete=models.CASCADE)
+    did = models.CharField(max_length=255)
+
+    def __str__(self) -> str:
+        return self.organization.name
+
+
+class OrganizationOnboardingNotification(models.Model):
+    organization = models.ForeignKey(Organization, on_delete=models.CASCADE)
+    operator = models.ForeignKey(UserProxy, on_delete=models.CASCADE)
+    sended_at = models.DateTimeField()
```

### Comparing `organizations-0.0.9/src/organizations/serializers.py` & `organizations-0.1.0/src/organizations/serializers.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from rest_framework import serializers
-from .models import Organization
-from typing import List
-
-
-class OrganizationSerializer(serializers.ModelSerializer):
-    class Meta:
-        model = Organization
-        fields = ("networks", "name", "email", "phone", "keys")
-
-
-class SuccessOrganizationsResponseSerializer(serializers.Serializer):
-    response = serializers.CharField(max_length=2)
-
-
-class DIDSerializer(serializers.Serializer):
-    did = serializers.CharField(max_length=255)
-    network_name = serializers.CharField(max_length=255)
-
-
-class CreateDIDResponseSerializer(serializers.Serializer):
-    dids = List[DIDSerializer]
-
-
-class CreateDIDSerializer(serializers.Serializer):
-    create_alastria_tx = serializers.CharField(max_length=1255)
-    subject_address = serializers.CharField(max_length=255)
-    email = serializers.CharField(max_length=255)
-
-
-class OperatorDIDSerializer(serializers.Serializer):
-    did = serializers.CharField(max_length=255)
-    email = serializers.CharField(max_length=255)
-    network_name = serializers.CharField(max_length=255)
+from rest_framework import serializers
+from .models import Organization
+from typing import List
+
+
+class OrganizationSerializer(serializers.ModelSerializer):
+    class Meta:
+        model = Organization
+        fields = ("networks", "name", "email", "phone", "keys")
+
+
+class SuccessOrganizationsResponseSerializer(serializers.Serializer):
+    response = serializers.CharField(max_length=2)
+
+
+class DIDSerializer(serializers.Serializer):
+    did = serializers.CharField(max_length=255)
+    network_name = serializers.CharField(max_length=255)
+
+
+class CreateDIDResponseSerializer(serializers.Serializer):
+    dids = List[DIDSerializer]
+
+
+class CreateDIDSerializer(serializers.Serializer):
+    create_alastria_tx = serializers.CharField(max_length=1255)
+    subject_address = serializers.CharField(max_length=255)
+    email = serializers.CharField(max_length=255)
+
+
+class OperatorDIDSerializer(serializers.Serializer):
+    did = serializers.CharField(max_length=255)
+    email = serializers.CharField(max_length=255)
+    network_name = serializers.CharField(max_length=255)
```

### Comparing `organizations-0.0.9/src/organizations/signals.py` & `organizations-0.1.0/src/organizations/signals.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-from django.dispatch import receiver
-from .models import (
-    Organization,
-    OrganizationKeys,
-    UserProxy,
-    OrganizationOnboardingNotification,
-    Issuer,
-)
-from django.db.models.signals import post_save
-from mnemonic import Mnemonic
-from eth_account import Account
-from organizations.tasks import create_organization_did, register_issuer_task
-from django.conf import settings
-from django.contrib.auth.forms import PasswordResetForm
-from django.http.request import HttpRequest
-from django.core import mail
-from templates_service_client.client import Client
-from templates_service_client.validators import OperatorOnboardingValidator
-from .service import OrganizationsService
-from django.utils.timezone import now
-from django.utils.html import strip_tags
-
-
-@receiver(post_save, sender=UserProxy)
-def post_save_profile(sender, instance: UserProxy, **kwargs):
-    if kwargs.get("created") and settings.OPERATOR_AUTOMATIC_STAFF:
-        instance.is_staff = True
-        instance.save()
-
-
-@receiver(post_save, sender=OrganizationOnboardingNotification)
-def post_save_onboarding_request(
-    sender, instance: OrganizationOnboardingNotification, **kwargs
-):
-    template_client = Client(settings.TEMPLATES_SERVICE_HOST)
-    html_message = template_client.get_operators_onboarding_template_rendered(
-        OperatorOnboardingValidator(
-            project=settings.TEMPLATES_PROJECT_NAME,
-            organization_name=instance.organization.name,
-            app_path=settings.APP_PATH,
-            web_path=settings.WEB_PATH,
-        )
-    ).text.replace("\n", "")
-    try:
-        mail.send_mail(
-            "Onboarding",
-            strip_tags(html_message),
-            settings.DEFAULT_FROM_EMAIL,
-            [instance.operator.email],
-            html_message=html_message,
-        )
-    except Exception as e:
-        print(str(e))  # TODO MAYBE ADD THIS THO QUEUE ?
-
-
-@receiver(post_save, sender=Issuer)
-def post_save_issuer(sender, instance: Issuer, **kwargs):
-    if kwargs.get("created"):
-        register_issuer_task.delay(instance.organization.id)
-
-
-@receiver(post_save, sender=Organization)
-def post_save_organization(sender, instance: Organization, **kwargs):
-    if kwargs.get("created"):
-        mnemo = Mnemonic("english")
-        words = mnemo.generate(strength=256)
-        mnemo.to_seed(words)
-        mnemo.to_entropy(words)
-        new_organization_acct = Account.create(words)
-        organization_keys = OrganizationKeys(
-            address=new_organization_acct.address,
-            private_key=new_organization_acct.key.hex(),
-            public_key=new_organization_acct._key_obj.public_key,
-            mnemonic=words,
-        )
-        organization_keys.save()
-        instance.keys = organization_keys
-        instance.save()
-        create_organization_did.delay(instance.pk)
-    else:
-        for operator in instance.operators.all():  # TODO PUT IT IN A TASK
-            if not OrganizationOnboardingNotification.objects.filter(
-                organization=instance, operator=operator
-            ).first():
-                OrganizationOnboardingNotification(
-                    organization=instance, operator=operator, sended_at=now()
-                ).save()
+from django.dispatch import receiver
+from .models import (
+    Organization,
+    OrganizationKeys,
+    UserProxy,
+    OrganizationOnboardingNotification,
+    Issuer,
+)
+from django.db.models.signals import post_save
+from mnemonic import Mnemonic
+from eth_account import Account
+from organizations.tasks import create_organization_did, register_issuer_task
+from django.conf import settings
+from django.contrib.auth.forms import PasswordResetForm
+from django.http.request import HttpRequest
+from django.core import mail
+from templates_service_client.client import Client
+from templates_service_client.validators import OperatorOnboardingValidator
+from .service import OrganizationsService
+from django.utils.timezone import now
+from django.utils.html import strip_tags
+
+
+@receiver(post_save, sender=UserProxy)
+def post_save_profile(sender, instance: UserProxy, **kwargs):
+    if kwargs.get("created") and settings.OPERATOR_AUTOMATIC_STAFF:
+        instance.is_staff = True
+        instance.save()
+
+
+@receiver(post_save, sender=OrganizationOnboardingNotification)
+def post_save_onboarding_request(
+    sender, instance: OrganizationOnboardingNotification, **kwargs
+):
+    template_client = Client(settings.TEMPLATES_SERVICE_HOST)
+    html_message = template_client.get_operators_onboarding_template_rendered(
+        OperatorOnboardingValidator(
+            project=settings.TEMPLATES_PROJECT_NAME,
+            organization_name=instance.organization.name,
+            app_path=settings.APP_PATH,
+            web_path=settings.WEB_PATH,
+        )
+    ).text.replace("\n", "")
+    try:
+        mail.send_mail(
+            "Onboarding",
+            strip_tags(html_message),
+            settings.DEFAULT_FROM_EMAIL,
+            [instance.operator.email],
+            html_message=html_message,
+        )
+    except Exception as e:
+        print(str(e))  # TODO MAYBE ADD THIS THO QUEUE ?
+
+
+@receiver(post_save, sender=Issuer)
+def post_save_issuer(sender, instance: Issuer, **kwargs):
+    if kwargs.get("created"):
+        register_issuer_task.delay(instance.organization.id)
+
+
+@receiver(post_save, sender=Organization)
+def post_save_organization(sender, instance: Organization, **kwargs):
+    if kwargs.get("created"):
+        mnemo = Mnemonic("english")
+        words = mnemo.generate(strength=256)
+        mnemo.to_seed(words)
+        mnemo.to_entropy(words)
+        new_organization_acct = Account.create(words)
+        organization_keys = OrganizationKeys(
+            address=new_organization_acct.address,
+            private_key=new_organization_acct.key.hex(),
+            public_key=new_organization_acct._key_obj.public_key,
+            mnemonic=words,
+        )
+        organization_keys.save()
+        instance.keys = organization_keys
+        instance.save()
+        create_organization_did.delay(instance.pk)
+    else:
+        for operator in instance.operators.all():  # TODO PUT IT IN A TASK
+            if not OrganizationOnboardingNotification.objects.filter(
+                organization=instance, operator=operator
+            ).first():
+                OrganizationOnboardingNotification(
+                    organization=instance, operator=operator, sended_at=now()
+                ).save()
```

### Comparing `organizations-0.0.9/src/organizations/tasks.py` & `organizations-0.1.0/src/organizations/tasks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-from __future__ import annotations
-from celery import shared_task
-from django.conf import settings
-from network_service_client.client import (
-    Client as NetworkClient,
-    Network as NetworkDTO,
-    NetworksNames,
-)
-from organizations.did_factory.models import FactoryArgsModel
-from organizations.did_factory.factory import Creator
-from organizations.models import Organization, OrganizationDID, Issuer
-
-
-@shared_task
-def create_organization_did(organization_id: int) -> None:
-    organization = Organization.objects.get(pk=organization_id)
-    for net in organization.networks:
-        network_data: NetworkDTO = NetworkClient(
-            service_host=settings.NETWORK_SERVICE_HOST
-        ).get_network_by_name(NetworksNames[net])
-        props = FactoryArgsModel(net=network_data)
-        context = Creator().create_object(props).request()
-        did: str = context.create_did(
-            organization.keys.address,
-            settings.ISSUER_ADDRESS,
-            str(organization.keys.public_key),
-            settings.ISSUER_PRIVATE_KEY,
-            organization.keys.private_key,  # TODO: encrypt this
-        )
-
-        organization_did = OrganizationDID(
-            network_name=NetworksNames[net],
-            organization=organization,
-            did=did,
-        )
-
-        organization_did.save()
-
-
-@shared_task
-def register_issuer_by_network_task(organization_id: int, net: str) -> None:
-    organization = Organization.objects.get(pk=organization_id)
-    issuer: Issuer = Issuer.objects.get(organization=organization)
-    organization_did: OrganizationDID | None = OrganizationDID.objects.filter(
-        organization=organization, network_name=NetworksNames[net]
-    ).first()
-    if not organization_did:
-        raise Exception(
-            f"You cannot register an organization without DID as an issuer, organization: {organization.id} network: {NetworksNames[net]}"
-        )
-    network_data: NetworkDTO = NetworkClient(
-        service_host=settings.NETWORK_SERVICE_HOST
-    ).get_network_by_name(NetworksNames[net])
-    props = FactoryArgsModel(net=network_data)
-    context = Creator().create_object(props).request()
-    context.register_issuer(
-        organization.keys.address,
-        settings.ISSUER_ADDRESS,
-        settings.ISSUER_PRIVATE_KEY,
-    )
-    issuer.active = True
-    issuer.save()
-    
-
-@shared_task
-def register_issuer_task(organization_id: int) -> None:
-    organization = Organization.objects.get(pk=organization_id)
-    for net in organization.networks:
-        register_issuer_by_network_task.delay(organization_id, net)
+from __future__ import annotations
+from celery import shared_task
+from django.conf import settings
+from network_service_client.client import (
+    Client as NetworkClient,
+    Network as NetworkDTO,
+    NetworksNames,
+)
+from organizations.did_factory.models import FactoryArgsModel
+from organizations.did_factory.factory import Creator
+from organizations.models import Organization, OrganizationDID, Issuer
+
+
+@shared_task
+def create_organization_did(organization_id: int) -> None:
+    organization = Organization.objects.get(pk=organization_id)
+    for net in organization.networks:
+        network_data: NetworkDTO = NetworkClient(
+            service_host=settings.NETWORK_SERVICE_HOST
+        ).get_network_by_name(NetworksNames[net])
+        props = FactoryArgsModel(net=network_data)
+        context = Creator().create_object(props).request()
+        did: str = context.create_did(
+            organization.keys.address,
+            settings.ISSUER_ADDRESS,
+            str(organization.keys.public_key),
+            settings.ISSUER_PRIVATE_KEY,
+            organization.keys.private_key,  # TODO: encrypt this
+        )
+
+        organization_did = OrganizationDID(
+            network_name=NetworksNames[net],
+            organization=organization,
+            did=did,
+        )
+
+        organization_did.save()
+
+
+@shared_task
+def register_issuer_by_network_task(organization_id: int, net: str) -> None:
+    organization = Organization.objects.get(pk=organization_id)
+    issuer: Issuer = Issuer.objects.get(organization=organization)
+    organization_did: OrganizationDID | None = OrganizationDID.objects.filter(
+        organization=organization, network_name=NetworksNames[net]
+    ).first()
+    if not organization_did:
+        raise Exception(
+            f"You cannot register an organization without DID as an issuer, organization: {organization.id} network: {NetworksNames[net]}"
+        )
+    network_data: NetworkDTO = NetworkClient(
+        service_host=settings.NETWORK_SERVICE_HOST
+    ).get_network_by_name(NetworksNames[net])
+    props = FactoryArgsModel(net=network_data)
+    context = Creator().create_object(props).request()
+    context.register_issuer(
+        organization.keys.address,
+        settings.ISSUER_ADDRESS,
+        settings.ISSUER_PRIVATE_KEY,
+    )
+    issuer.active = True
+    issuer.save()
+
+
+@shared_task
+def register_issuer_task(organization_id: int) -> None:
+    organization = Organization.objects.get(pk=organization_id)
+    for net in organization.networks:
+        register_issuer_by_network_task.delay(organization_id, net)
```

### Comparing `organizations-0.0.9/src/organizations/views.py` & `organizations-0.1.0/src/organizations/views.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-from rest_framework.viewsets import ViewSet
-from rest_framework.permissions import AllowAny
-from drf_yasg import openapi
-from drf_yasg.utils import swagger_auto_schema
-from rest_framework.decorators import action
-from rest_framework.response import Response
-from waffle.decorators import waffle_switch
-from django.http.response import HttpResponseBadRequest
-from .enums import OrganizationsSwitches
-from .serializers import (
-    DIDSerializer,
-    OperatorDIDSerializer,
-    OrganizationSerializer,
-    SuccessOrganizationsResponseSerializer,
-    CreateDIDSerializer,
-    CreateDIDResponseSerializer,
-)
-
-from .service import OrganizationsService
-
-
-class OrganizationsView(ViewSet):
-    permission_classes = (AllowAny,)
-
-    @swagger_auto_schema(
-        method="get",
-        manual_parameters=[
-            openapi.Parameter(
-                "operator_email",
-                openapi.IN_QUERY,
-                description="",
-                type=openapi.TYPE_STRING,
-            )
-        ],
-        responses={200: openapi.Response("", OrganizationSerializer)},
-    )
-    @waffle_switch(OrganizationsSwitches.Organizations.value)
-    @action(detail=False, methods=["get"])
-    def get_organization_by_operator_email(self, request):
-        operator_email: str = request.GET["operator_email"]
-        organization = OrganizationsService.get_organization_by_operator_email(
-            operator_email
-        )
-        if organization:
-            return Response(OrganizationSerializer(organization).data)
-
-        return HttpResponseBadRequest("Invalid email.")
-
-    @swagger_auto_schema(
-        method="post",
-        request_body=CreateDIDSerializer,
-        responses={200: openapi.Response("", CreateDIDResponseSerializer)},
-    )
-    @waffle_switch(OrganizationsSwitches.Organizations.value)
-    @action(detail=False, methods=["post"])
-    def get_did(self, request):
-        create_alastria_tx: str = request.data["create_alastria_tx"]
-        subject_address: str = request.data["subject_address"]
-        email: str = request.data["email"]
-        return Response(
-            OrganizationsService.get_did(create_alastria_tx, subject_address, email)
-        )
-
-    @swagger_auto_schema(
-        method="post",
-        request_body=OperatorDIDSerializer,
-        responses={200: openapi.Response("", SuccessOrganizationsResponseSerializer)},
-    )
-    @waffle_switch(OrganizationsSwitches.Organizations.value)
-    @action(detail=False, methods=["post"])
-    def set_did(self, request):
-        email: str = request.data["email"]
-        did: str = request.data["did"]
-        network_name: str = request.data["network_name"]
-        OrganizationsService.set_did(email, did, network_name)
-        return Response({"response": "OK"})
+from rest_framework.viewsets import ViewSet
+from rest_framework.permissions import AllowAny
+from drf_yasg import openapi
+from drf_yasg.utils import swagger_auto_schema
+from rest_framework.decorators import action
+from rest_framework.response import Response
+from waffle.decorators import waffle_switch
+from django.http.response import HttpResponseBadRequest
+from .enums import OrganizationsSwitches
+from .serializers import (
+    DIDSerializer,
+    OperatorDIDSerializer,
+    OrganizationSerializer,
+    SuccessOrganizationsResponseSerializer,
+    CreateDIDSerializer,
+    CreateDIDResponseSerializer,
+)
+
+from .service import OrganizationsService
+
+
+class OrganizationsView(ViewSet):
+    permission_classes = (AllowAny,)
+
+    @swagger_auto_schema(
+        method="get",
+        manual_parameters=[
+            openapi.Parameter(
+                "operator_email",
+                openapi.IN_QUERY,
+                description="",
+                type=openapi.TYPE_STRING,
+            )
+        ],
+        responses={200: openapi.Response("", OrganizationSerializer)},
+    )
+    @waffle_switch(OrganizationsSwitches.Organizations.value)
+    @action(detail=False, methods=["get"])
+    def get_organization_by_operator_email(self, request):
+        operator_email: str = request.GET["operator_email"]
+        organization = OrganizationsService.get_organization_by_operator_email(
+            operator_email
+        )
+        if organization:
+            return Response(OrganizationSerializer(organization).data)
+
+        return HttpResponseBadRequest("Invalid email.")
+
+    @swagger_auto_schema(
+        method="post",
+        request_body=CreateDIDSerializer,
+        responses={200: openapi.Response("", CreateDIDResponseSerializer)},
+    )
+    @waffle_switch(OrganizationsSwitches.Organizations.value)
+    @action(detail=False, methods=["post"])
+    def get_did(self, request):
+        create_alastria_tx: str = request.data["create_alastria_tx"]
+        subject_address: str = request.data["subject_address"]
+        email: str = request.data["email"]
+        return Response(
+            OrganizationsService.get_did(create_alastria_tx, subject_address, email)
+        )
+
+    @swagger_auto_schema(
+        method="post",
+        request_body=OperatorDIDSerializer,
+        responses={200: openapi.Response("", SuccessOrganizationsResponseSerializer)},
+    )
+    @waffle_switch(OrganizationsSwitches.Organizations.value)
+    @action(detail=False, methods=["post"])
+    def set_did(self, request):
+        email: str = request.data["email"]
+        did: str = request.data["did"]
+        network_name: str = request.data["network_name"]
+        OrganizationsService.set_did(email, did, network_name)
+        return Response({"response": "OK"})
```

### Comparing `organizations-0.0.9/src/organizations.egg-info/SOURCES.txt` & `organizations-0.1.0/src/organizations.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -29,8 +29,10 @@
 src/organizations/migrations/0001_initial.py
 src/organizations/migrations/0002_organization_networks.py
 src/organizations/migrations/0003_alter_organization_networks.py
 src/organizations/migrations/0004_alter_organization_email_and_more.py
 src/organizations/migrations/0005_subject_alter_organization_networks_and_more.py
 src/organizations/migrations/0006_alter_organization_networks_and_more.py
 src/organizations/migrations/0007_alter_issuer_active.py
+src/organizations/migrations/0008_alter_organization_networks.py
+src/organizations/migrations/0009_issuer_name.py
 src/organizations/migrations/__init__.py
```

