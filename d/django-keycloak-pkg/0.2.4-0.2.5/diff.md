# Comparing `tmp/django-keycloak-pkg-0.2.4.tar.gz` & `tmp/django-keycloak-pkg-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-keycloak-pkg-0.2.4.tar", last modified: Wed Jan 18 13:18:05 2023, max compression
+gzip compressed data, was "django-keycloak-pkg-0.2.5.tar", last modified: Wed May  3 12:14:26 2023, max compression
```

## Comparing `django-keycloak-pkg-0.2.4.tar` & `django-keycloak-pkg-0.2.5.tar`

### file list

```diff
@@ -1,81 +1,82 @@
-drwxr-xr-x   0 adabo      (501) staff       (20)        0 2023-01-18 13:18:05.394000 django-keycloak-pkg-0.2.4/
--rw-r--r--   0 adabo      (501) staff       (20)     1068 2022-10-04 08:47:01.000000 django-keycloak-pkg-0.2.4/LICENSE
--rw-r--r--   0 adabo      (501) staff       (20)     3907 2023-01-18 13:18:05.394081 django-keycloak-pkg-0.2.4/PKG-INFO
--rw-r--r--   0 adabo      (501) staff       (20)     3267 2023-01-18 13:17:01.000000 django-keycloak-pkg-0.2.4/README.rst
--rw-r--r--   0 adabo      (501) staff       (20)      638 2023-01-18 13:17:01.000000 django-keycloak-pkg-0.2.4/pyproject.toml
--rw-r--r--   0 adabo      (501) staff       (20)      559 2023-01-18 13:18:05.394394 django-keycloak-pkg-0.2.4/setup.cfg
--rw-r--r--   0 adabo      (501) staff       (20)     1195 2023-01-18 13:17:01.000000 django-keycloak-pkg-0.2.4/setup.py
-drwxr-xr-x   0 adabo      (501) staff       (20)        0 2023-01-18 13:18:05.380704 django-keycloak-pkg-0.2.4/src/
-drwxr-xr-x   0 adabo      (501) staff       (20)        0 2023-01-18 13:18:05.384800 django-keycloak-pkg-0.2.4/src/django_keycloak/
--rw-r--r--   0 adabo      (501) staff       (20)      308 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/__init__.py
-drwxr-xr-x   0 adabo      (501) staff       (20)        0 2023-01-18 13:18:05.385532 django-keycloak-pkg-0.2.4/src/django_keycloak/admin/
--rw-r--r--   0 adabo      (501) staff       (20)      268 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/admin/__init__.py
--rw-r--r--   0 adabo      (501) staff       (20)     4239 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/admin/realm.py
--rw-r--r--   0 adabo      (501) staff       (20)      178 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/admin/server.py
--rw-r--r--   0 adabo      (501) staff       (20)      649 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/app_settings.py
--rw-r--r--   0 adabo      (501) staff       (20)      138 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/apps.py
-drwxr-xr-x   0 adabo      (501) staff       (20)        0 2023-01-18 13:18:05.385874 django-keycloak-pkg-0.2.4/src/django_keycloak/auth/
--rw-r--r--   0 adabo      (501) staff       (20)     2603 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/auth/__init__.py
--rw-r--r--   0 adabo      (501) staff       (20)     6202 2023-01-18 13:17:01.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/auth/backends.py
--rw-r--r--   0 adabo      (501) staff       (20)     1434 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/factories.py
--rw-r--r--   0 adabo      (501) staff       (20)      196 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/hashers.py
-drwxr-xr-x   0 adabo      (501) staff       (20)        0 2023-01-18 13:18:05.386144 django-keycloak-pkg-0.2.4/src/django_keycloak/management/
--rw-r--r--   0 adabo      (501) staff       (20)        0 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/management/__init__.py
-drwxr-xr-x   0 adabo      (501) staff       (20)        0 2023-01-18 13:18:05.386713 django-keycloak-pkg-0.2.4/src/django_keycloak/management/commands/
--rw-r--r--   0 adabo      (501) staff       (20)        0 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/management/commands/__init__.py
--rw-r--r--   0 adabo      (501) staff       (20)     1012 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/management/commands/keycloak_add_user.py
--rw-r--r--   0 adabo      (501) staff       (20)      547 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/management/commands/keycloak_refresh_realm.py
--rw-r--r--   0 adabo      (501) staff       (20)      850 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/management/commands/keycloak_sync_resources.py
--rw-r--r--   0 adabo      (501) staff       (20)     3789 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/middleware.py
-drwxr-xr-x   0 adabo      (501) staff       (20)        0 2023-01-18 13:18:05.388292 django-keycloak-pkg-0.2.4/src/django_keycloak/migrations/
--rw-r--r--   0 adabo      (501) staff       (20)     5561 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/migrations/0001_initial.py
--rw-r--r--   0 adabo      (501) staff       (20)     2020 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/migrations/0002_auto_20180322_2059.py
--rw-r--r--   0 adabo      (501) staff       (20)     1583 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/migrations/0003_auto_20190204_1949.py
--rw-r--r--   0 adabo      (501) staff       (20)      623 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/migrations/0004_client_service_account_profile.py
--rw-r--r--   0 adabo      (501) staff       (20)      823 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/migrations/0005_auto_20190219_2002.py
--rw-r--r--   0 adabo      (501) staff       (20)      345 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/migrations/0006_remove_client_service_account.py
--rw-r--r--   0 adabo      (501) staff       (20)     2190 2022-11-08 12:09:12.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/migrations/0007_alter_client_id_alter_exchangedtoken_id_and_more.py
--rw-r--r--   0 adabo      (501) staff       (20)        0 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/migrations/__init__.py
--rw-r--r--   0 adabo      (501) staff       (20)     7473 2022-10-06 05:06:16.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/models.py
--rw-r--r--   0 adabo      (501) staff       (20)     6215 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/remote_user.py
--rw-r--r--   0 adabo      (501) staff       (20)      723 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/response.py
-drwxr-xr-x   0 adabo      (501) staff       (20)        0 2023-01-18 13:18:05.389992 django-keycloak-pkg-0.2.4/src/django_keycloak/services/
--rw-r--r--   0 adabo      (501) staff       (20)        0 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/services/__init__.py
--rw-r--r--   0 adabo      (501) staff       (20)     3520 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/services/client.py
--rw-r--r--   0 adabo      (501) staff       (20)      102 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/services/exceptions.py
--rw-r--r--   0 adabo      (501) staff       (20)    10692 2022-10-06 05:08:38.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/services/oidc_profile.py
--rw-r--r--   0 adabo      (501) staff       (20)      967 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/services/permissions.py
--rw-r--r--   0 adabo      (501) staff       (20)     2144 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/services/realm.py
--rw-r--r--   0 adabo      (501) staff       (20)     1942 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/services/remote_client.py
--rw-r--r--   0 adabo      (501) staff       (20)     1665 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/services/uma.py
--rw-r--r--   0 adabo      (501) staff       (20)     1017 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/services/users.py
-drwxr-xr-x   0 adabo      (501) staff       (20)        0 2023-01-18 13:18:05.390755 django-keycloak-pkg-0.2.4/src/django_keycloak/tests/
--rw-r--r--   0 adabo      (501) staff       (20)        0 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/tests/__init__.py
-drwxr-xr-x   0 adabo      (501) staff       (20)        0 2023-01-18 13:18:05.390921 django-keycloak-pkg-0.2.4/src/django_keycloak/tests/backends/
--rw-r--r--   0 adabo      (501) staff       (20)        0 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/tests/backends/__init__.py
-drwxr-xr-x   0 adabo      (501) staff       (20)        0 2023-01-18 13:18:05.391465 django-keycloak-pkg-0.2.4/src/django_keycloak/tests/backends/keycloak_authorization_base/
--rw-r--r--   0 adabo      (501) staff       (20)        0 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/tests/backends/keycloak_authorization_base/__init__.py
--rw-r--r--   0 adabo      (501) staff       (20)     1687 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/tests/backends/keycloak_authorization_base/test_get_keycloak_permissions.py
--rw-r--r--   0 adabo      (501) staff       (20)     3047 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/tests/backends/keycloak_authorization_base/test_has_perm.py
--rw-r--r--   0 adabo      (501) staff       (20)      613 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/tests/mixins.py
-drwxr-xr-x   0 adabo      (501) staff       (20)        0 2023-01-18 13:18:05.391693 django-keycloak-pkg-0.2.4/src/django_keycloak/tests/services/
--rw-r--r--   0 adabo      (501) staff       (20)        0 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/tests/services/__init__.py
-drwxr-xr-x   0 adabo      (501) staff       (20)        0 2023-01-18 13:18:05.392762 django-keycloak-pkg-0.2.4/src/django_keycloak/tests/services/oidc_profile/
--rw-r--r--   0 adabo      (501) staff       (20)        0 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/tests/services/oidc_profile/__init__.py
--rw-r--r--   0 adabo      (501) staff       (20)     2661 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/tests/services/oidc_profile/test_get_active_access_token.py
--rw-r--r--   0 adabo      (501) staff       (20)     2014 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/tests/services/oidc_profile/test_get_entitlement.py
--rw-r--r--   0 adabo      (501) staff       (20)     5949 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/tests/services/oidc_profile/test_get_or_create_from_id_token.py
--rw-r--r--   0 adabo      (501) staff       (20)     4814 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/tests/services/oidc_profile/test_update_or_create.py
-drwxr-xr-x   0 adabo      (501) staff       (20)        0 2023-01-18 13:18:05.393211 django-keycloak-pkg-0.2.4/src/django_keycloak/tests/services/realm/
--rw-r--r--   0 adabo      (501) staff       (20)        0 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/tests/services/realm/__init__.py
--rw-r--r--   0 adabo      (501) staff       (20)     1701 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/tests/services/realm/test_get_realm_api_client.py
--rw-r--r--   0 adabo      (501) staff       (20)     1099 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/tests/services/realm/test_refresh_well_known_oidc.py
--rw-r--r--   0 adabo      (501) staff       (20)      910 2022-09-27 03:44:22.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/tests/settings.py
--rw-r--r--   0 adabo      (501) staff       (20)     1104 2022-09-27 03:46:41.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/urls.py
--rw-r--r--   0 adabo      (501) staff       (20)     4956 2022-11-03 15:03:57.000000 django-keycloak-pkg-0.2.4/src/django_keycloak/views.py
-drwxr-xr-x   0 adabo      (501) staff       (20)        0 2023-01-18 13:18:05.393838 django-keycloak-pkg-0.2.4/src/django_keycloak_pkg.egg-info/
--rw-r--r--   0 adabo      (501) staff       (20)     3907 2023-01-18 13:18:05.000000 django-keycloak-pkg-0.2.4/src/django_keycloak_pkg.egg-info/PKG-INFO
--rw-r--r--   0 adabo      (501) staff       (20)     2989 2023-01-18 13:18:05.000000 django-keycloak-pkg-0.2.4/src/django_keycloak_pkg.egg-info/SOURCES.txt
--rw-r--r--   0 adabo      (501) staff       (20)        1 2023-01-18 13:18:05.000000 django-keycloak-pkg-0.2.4/src/django_keycloak_pkg.egg-info/dependency_links.txt
--rw-r--r--   0 adabo      (501) staff       (20)      123 2023-01-18 13:18:05.000000 django-keycloak-pkg-0.2.4/src/django_keycloak_pkg.egg-info/requires.txt
--rw-r--r--   0 adabo      (501) staff       (20)       16 2023-01-18 13:18:05.000000 django-keycloak-pkg-0.2.4/src/django_keycloak_pkg.egg-info/top_level.txt
+drwxrwxr-x   0 innovadigits  (1000) innovadigits  (1000)        0 2023-05-03 12:14:26.031362 django-keycloak-pkg-0.2.5/
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     1068 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/LICENSE
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     3955 2023-05-03 12:14:26.031362 django-keycloak-pkg-0.2.5/PKG-INFO
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     3317 2023-04-30 14:37:46.000000 django-keycloak-pkg-0.2.5/README.md
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     3316 2023-04-30 14:38:22.000000 django-keycloak-pkg-0.2.5/README.rst
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)      638 2023-04-30 14:43:56.000000 django-keycloak-pkg-0.2.5/pyproject.toml
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)      559 2023-05-03 12:14:26.031362 django-keycloak-pkg-0.2.5/setup.cfg
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     1195 2023-04-30 14:44:40.000000 django-keycloak-pkg-0.2.5/setup.py
+drwxrwxr-x   0 innovadigits  (1000) innovadigits  (1000)        0 2023-05-03 12:14:26.019362 django-keycloak-pkg-0.2.5/src/
+drwxrwxr-x   0 innovadigits  (1000) innovadigits  (1000)        0 2023-05-03 12:14:26.023362 django-keycloak-pkg-0.2.5/src/django_keycloak/
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)      308 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/__init__.py
+drwxrwxr-x   0 innovadigits  (1000) innovadigits  (1000)        0 2023-05-03 12:14:26.023362 django-keycloak-pkg-0.2.5/src/django_keycloak/admin/
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)      268 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/admin/__init__.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     4239 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/admin/realm.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)      178 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/admin/server.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)      649 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/app_settings.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)      138 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/apps.py
+drwxrwxr-x   0 innovadigits  (1000) innovadigits  (1000)        0 2023-05-03 12:14:26.023362 django-keycloak-pkg-0.2.5/src/django_keycloak/auth/
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     2603 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/auth/__init__.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     6202 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/auth/backends.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     1434 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/factories.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)      196 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/hashers.py
+drwxrwxr-x   0 innovadigits  (1000) innovadigits  (1000)        0 2023-05-03 12:14:26.023362 django-keycloak-pkg-0.2.5/src/django_keycloak/management/
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)        0 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/management/__init__.py
+drwxrwxr-x   0 innovadigits  (1000) innovadigits  (1000)        0 2023-05-03 12:14:26.023362 django-keycloak-pkg-0.2.5/src/django_keycloak/management/commands/
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)        0 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/management/commands/__init__.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     1012 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/management/commands/keycloak_add_user.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)      547 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/management/commands/keycloak_refresh_realm.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)      850 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/management/commands/keycloak_sync_resources.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     3789 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/middleware.py
+drwxrwxr-x   0 innovadigits  (1000) innovadigits  (1000)        0 2023-05-03 12:14:26.027362 django-keycloak-pkg-0.2.5/src/django_keycloak/migrations/
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     5561 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/migrations/0001_initial.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     2020 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/migrations/0002_auto_20180322_2059.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     1583 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/migrations/0003_auto_20190204_1949.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)      623 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/migrations/0004_client_service_account_profile.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)      823 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/migrations/0005_auto_20190219_2002.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)      345 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/migrations/0006_remove_client_service_account.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     2190 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/migrations/0007_alter_client_id_alter_exchangedtoken_id_and_more.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)        0 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/migrations/__init__.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     7473 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/models.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     6215 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/remote_user.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)      723 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/response.py
+drwxrwxr-x   0 innovadigits  (1000) innovadigits  (1000)        0 2023-05-03 12:14:26.027362 django-keycloak-pkg-0.2.5/src/django_keycloak/services/
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)        0 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/services/__init__.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     3520 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/services/client.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)      102 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/services/exceptions.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)    10692 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/services/oidc_profile.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)      967 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/services/permissions.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     2144 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/services/realm.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     1942 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/services/remote_client.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     1665 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/services/uma.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     1017 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/services/users.py
+drwxrwxr-x   0 innovadigits  (1000) innovadigits  (1000)        0 2023-05-03 12:14:26.027362 django-keycloak-pkg-0.2.5/src/django_keycloak/tests/
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)        0 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/tests/__init__.py
+drwxrwxr-x   0 innovadigits  (1000) innovadigits  (1000)        0 2023-05-03 12:14:26.027362 django-keycloak-pkg-0.2.5/src/django_keycloak/tests/backends/
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)        0 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/tests/backends/__init__.py
+drwxrwxr-x   0 innovadigits  (1000) innovadigits  (1000)        0 2023-05-03 12:14:26.027362 django-keycloak-pkg-0.2.5/src/django_keycloak/tests/backends/keycloak_authorization_base/
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)        0 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/tests/backends/keycloak_authorization_base/__init__.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     1687 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/tests/backends/keycloak_authorization_base/test_get_keycloak_permissions.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     3047 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/tests/backends/keycloak_authorization_base/test_has_perm.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)      613 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/tests/mixins.py
+drwxrwxr-x   0 innovadigits  (1000) innovadigits  (1000)        0 2023-05-03 12:14:26.027362 django-keycloak-pkg-0.2.5/src/django_keycloak/tests/services/
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)        0 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/tests/services/__init__.py
+drwxrwxr-x   0 innovadigits  (1000) innovadigits  (1000)        0 2023-05-03 12:14:26.031362 django-keycloak-pkg-0.2.5/src/django_keycloak/tests/services/oidc_profile/
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)        0 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/tests/services/oidc_profile/__init__.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     2661 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/tests/services/oidc_profile/test_get_active_access_token.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     2014 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/tests/services/oidc_profile/test_get_entitlement.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     5949 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/tests/services/oidc_profile/test_get_or_create_from_id_token.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     4814 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/tests/services/oidc_profile/test_update_or_create.py
+drwxrwxr-x   0 innovadigits  (1000) innovadigits  (1000)        0 2023-05-03 12:14:26.031362 django-keycloak-pkg-0.2.5/src/django_keycloak/tests/services/realm/
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)        0 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/tests/services/realm/__init__.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     1701 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/tests/services/realm/test_get_realm_api_client.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     1099 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/tests/services/realm/test_refresh_well_known_oidc.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)      910 2023-04-20 12:57:12.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/tests/settings.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     1185 2023-04-20 13:23:20.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/urls.py
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     5940 2023-05-02 16:20:56.000000 django-keycloak-pkg-0.2.5/src/django_keycloak/views.py
+drwxrwxr-x   0 innovadigits  (1000) innovadigits  (1000)        0 2023-05-03 12:14:26.031362 django-keycloak-pkg-0.2.5/src/django_keycloak_pkg.egg-info/
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     3955 2023-05-03 12:14:26.000000 django-keycloak-pkg-0.2.5/src/django_keycloak_pkg.egg-info/PKG-INFO
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)     2999 2023-05-03 12:14:26.000000 django-keycloak-pkg-0.2.5/src/django_keycloak_pkg.egg-info/SOURCES.txt
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)        1 2023-05-03 12:14:26.000000 django-keycloak-pkg-0.2.5/src/django_keycloak_pkg.egg-info/dependency_links.txt
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)      123 2023-05-03 12:14:26.000000 django-keycloak-pkg-0.2.5/src/django_keycloak_pkg.egg-info/requires.txt
+-rw-rw-r--   0 innovadigits  (1000) innovadigits  (1000)       16 2023-05-03 12:14:26.000000 django-keycloak-pkg-0.2.5/src/django_keycloak_pkg.egg-info/top_level.txt
```

### Comparing `django-keycloak-pkg-0.2.4/LICENSE` & `django-keycloak-pkg-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/PKG-INFO` & `django-keycloak-pkg-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-keycloak-pkg
-Version: 0.2.4
+Version: 0.2.5
 Summary: Install Django Keycloak
 Home-page: https://github.com/dabocs/django-keycloak
 Author: Ahmad Dabo
 Author-email: Ahmad Dabo <dabo.cs@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/dabocs/django-keycloak
 Project-URL: Bug Tracker, https://github.com/dabocs/django-keycloak/issues
@@ -88,14 +88,19 @@
     $ git push origin master --tags
 
 Release Notes
 =============
 
 **unreleased**
 
+**v0.2.5**
+
+* Add registeration redirect view
+
+
 **v0.2.4**
 
 * Fixed refresh token expiration date exists
 
 
 **v0.2.3**
```

### Comparing `django-keycloak-pkg-0.2.4/README.rst` & `django-keycloak-pkg-0.2.5/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,19 @@
     $ git push origin master --tags
 
 Release Notes
 =============
 
 **unreleased**
 
+**v0.2.5**
+
+* Add registeration redirect view
+
+
 **v0.2.4**
 
 * Fixed refresh token expiration date exists
 
 **v0.2.3**
 
 * Fixed ENTTITLMENT issue by commenting the code temporarily, till fully fixed
@@ -112,8 +117,8 @@
 
 **v0.1.0**
 
 * Correctly extract email field name on UserModel (thanks to `swist <https://github.com/swist>`_)
 * Add support for Oauth2 Token Exchange to exchange tokens with remote clients.
   Handy when using multiple applications with different clients which have to
   communicate with each other.
-* Support for session iframe
+* Support for session iframe
```

### Comparing `django-keycloak-pkg-0.2.4/pyproject.toml` & `django-keycloak-pkg-0.2.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","python-keycloak-client-pkg==0.3.0", "Django>=4.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-keycloak-pkg"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="Ahmad Dabo", email="dabo.cs@gmail.com" },
 ]
 description = "Install Django Keycloak"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `django-keycloak-pkg-0.2.4/setup.cfg` & `django-keycloak-pkg-0.2.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.4
+current_version = 0.2.5
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}
 	{major}.{minor}.{patch}
```

### Comparing `django-keycloak-pkg-0.2.4/setup.py` & `django-keycloak-pkg-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from setuptools import setup, find_packages
 
-VERSION = '0.2.4'
+VERSION = '0.2.5'
 
 with open(os.path.join(os.path.dirname(__file__), 'README.rst')) as readme:
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
```

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/admin/realm.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/admin/realm.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/app_settings.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/auth/__init__.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/auth/backends.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/auth/backends.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/factories.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/factories.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/management/commands/keycloak_add_user.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/management/commands/keycloak_add_user.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/management/commands/keycloak_refresh_realm.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/management/commands/keycloak_refresh_realm.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/management/commands/keycloak_sync_resources.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/management/commands/keycloak_sync_resources.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/middleware.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/middleware.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/migrations/0001_initial.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/migrations/0002_auto_20180322_2059.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/migrations/0002_auto_20180322_2059.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/migrations/0003_auto_20190204_1949.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/migrations/0003_auto_20190204_1949.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/migrations/0004_client_service_account_profile.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/migrations/0004_client_service_account_profile.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/migrations/0005_auto_20190219_2002.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/migrations/0005_auto_20190219_2002.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/migrations/0007_alter_client_id_alter_exchangedtoken_id_and_more.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/migrations/0007_alter_client_id_alter_exchangedtoken_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/models.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/models.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/remote_user.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/remote_user.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/response.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/response.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/services/client.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/services/client.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/services/oidc_profile.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/services/oidc_profile.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/services/permissions.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/services/permissions.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/services/realm.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/services/realm.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/services/remote_client.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/services/remote_client.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/services/uma.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/services/uma.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/services/users.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/services/users.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/tests/backends/keycloak_authorization_base/test_get_keycloak_permissions.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/tests/backends/keycloak_authorization_base/test_get_keycloak_permissions.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/tests/backends/keycloak_authorization_base/test_has_perm.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/tests/backends/keycloak_authorization_base/test_has_perm.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/tests/mixins.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/tests/services/oidc_profile/test_get_active_access_token.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/tests/services/oidc_profile/test_get_active_access_token.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/tests/services/oidc_profile/test_get_entitlement.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/tests/services/oidc_profile/test_get_entitlement.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/tests/services/oidc_profile/test_get_or_create_from_id_token.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/tests/services/oidc_profile/test_get_or_create_from_id_token.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/tests/services/oidc_profile/test_update_or_create.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/tests/services/oidc_profile/test_update_or_create.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/tests/services/realm/test_get_realm_api_client.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/tests/services/realm/test_get_realm_api_client.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/tests/services/realm/test_refresh_well_known_oidc.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/tests/services/realm/test_refresh_well_known_oidc.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/tests/settings.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/urls.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/urls.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,9 +18,10 @@
 
 urlpatterns = [
     re_path(r'^login$', views.Login.as_view(), name='keycloak_login'),
     re_path(r'^login-complete$', views.LoginComplete.as_view(),
         name='keycloak_login_complete'),
     re_path(r'^logout$', views.Logout.as_view(), name='keycloak_logout'),
     re_path(r'^session-iframe', views.SessionIframe.as_view(),
-        name='keycloak_session_iframe')
+        name='keycloak_session_iframe'),
+    re_path(r'^register$', views.Register.as_view(), name='keycloak_register'),
 ]
```

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak/views.py` & `django-keycloak-pkg-0.2.5/src/django_keycloak/views.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,16 +21,17 @@
 )
 from django.urls.base import reverse
 from django.views.generic.base import (
     RedirectView,
     TemplateView
 )
 
-from django_keycloak.models import Nonce
+from django_keycloak.models import Nonce, Server, Client, Realm
 from django_keycloak.auth import remote_user_login
+from urllib.parse import urlencode
 
 
 logger = logging.getLogger(__name__)
 
 
 class Login(RedirectView):
 
@@ -150,7 +151,35 @@
         return super(SessionIframe, self).get_context_data(
             client_id=self.client_id,
             identity_server=self.request.realm.server.url,
             op_location=self.op_location,
             cookie_name=getattr(settings, 'KEYCLOAK_SESSION_STATE_COOKIE_NAME',
                                 'session_state')
         )
+
+
+class Register(RedirectView):
+    """Generate link for user registration with Keycloak."""
+
+    def get_redirect_url(self, *args, **kwargs):
+        server = Server.objects.last()
+        realm = Realm.objects.last()
+        client = Client.objects.last()
+        lang = self.request.GET.get('lang')
+
+        keycloack_register_url = f"{server.url.rstrip('/')}/realms/{realm.name}/protocol/openid-connect/registrations"
+
+        registration_url = (
+            keycloack_register_url
+            + "?"
+            + urlencode(
+                {
+                    "client_id": client.client_id,
+                    "response_type": "code",
+                    "scope": "openid email",
+                    "redirect_uri": self.request.build_absolute_uri(location=reverse('keycloak_login')),
+                    "kc_locale": lang if lang else 'ar',
+                }
+            )
+        )
+
+        return registration_url
```

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak_pkg.egg-info/PKG-INFO` & `django-keycloak-pkg-0.2.5/src/django_keycloak_pkg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-keycloak-pkg
-Version: 0.2.4
+Version: 0.2.5
 Summary: Install Django Keycloak
 Home-page: https://github.com/dabocs/django-keycloak
 Author: Ahmad Dabo
 Author-email: Ahmad Dabo <dabo.cs@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/dabocs/django-keycloak
 Project-URL: Bug Tracker, https://github.com/dabocs/django-keycloak/issues
@@ -88,14 +88,19 @@
     $ git push origin master --tags
 
 Release Notes
 =============
 
 **unreleased**
 
+**v0.2.5**
+
+* Add registeration redirect view
+
+
 **v0.2.4**
 
 * Fixed refresh token expiration date exists
 
 
 **v0.2.3**
```

### Comparing `django-keycloak-pkg-0.2.4/src/django_keycloak_pkg.egg-info/SOURCES.txt` & `django-keycloak-pkg-0.2.5/src/django_keycloak_pkg.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+README.md
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 src/django_keycloak/__init__.py
 src/django_keycloak/app_settings.py
 src/django_keycloak/apps.py
```

