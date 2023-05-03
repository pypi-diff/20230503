# Comparing `tmp/django_dnoticias_services-1.0.97.tar.gz` & `tmp/django_dnoticias_services-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_dnoticias_services-1.0.97.tar", last modified: Wed Mar 29 16:09:26 2023, max compression
+gzip compressed data, was "django_dnoticias_services-1.1.tar", max compression
```

## Comparing `django_dnoticias_services-1.0.97.tar` & `django_dnoticias_services-1.1.tar`

### file list

```diff
@@ -1,188 +1,54 @@
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-03-29 16:09:26.931105 django_dnoticias_services-1.0.97/
--rw-rw-r--   0 nelson    (1000) nelson    (1000)       73 2021-04-21 11:38:35.000000 django_dnoticias_services-1.0.97/MANIFEST.in
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     8797 2023-03-29 16:09:26.931105 django_dnoticias_services-1.0.97/PKG-INFO
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     8504 2022-05-23 10:44:57.000000 django_dnoticias_services-1.0.97/README.md
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-03-29 16:09:26.783101 django_dnoticias_services-1.0.97/django_dnoticias_services.egg-info/
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     8797 2023-03-29 16:09:26.000000 django_dnoticias_services-1.0.97/django_dnoticias_services.egg-info/PKG-INFO
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     9209 2023-03-29 16:09:26.000000 django_dnoticias_services-1.0.97/django_dnoticias_services.egg-info/SOURCES.txt
--rw-rw-r--   0 nelson    (1000) nelson    (1000)        1 2023-03-29 16:09:26.000000 django_dnoticias_services-1.0.97/django_dnoticias_services.egg-info/dependency_links.txt
--rw-rw-r--   0 nelson    (1000) nelson    (1000)       52 2023-03-29 16:09:26.000000 django_dnoticias_services-1.0.97/django_dnoticias_services.egg-info/requires.txt
--rw-rw-r--   0 nelson    (1000) nelson    (1000)       19 2023-03-29 16:09:26.000000 django_dnoticias_services-1.0.97/django_dnoticias_services.egg-info/top_level.txt
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-03-29 16:09:26.787101 django_dnoticias_services-1.0.97/dnoticias_services/
--rw-r--r--   0 nelson    (1000) nelson    (1000)        0 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/__init__.py
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-03-29 16:09:26.791102 django_dnoticias_services-1.0.97/dnoticias_services/__pycache__/
--rw-r--r--   0 nelson    (1000) nelson    (1000)      147 2022-09-09 15:14:50.000000 django_dnoticias_services-1.0.97/dnoticias_services/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      154 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      145 2022-05-26 14:57:29.000000 django_dnoticias_services-1.0.97/dnoticias_services/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      392 2023-03-22 16:58:10.000000 django_dnoticias_services-1.0.97/dnoticias_services/__pycache__/apps.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      393 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/__pycache__/apps.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     1866 2023-03-22 16:58:27.000000 django_dnoticias_services-1.0.97/dnoticias_services/__pycache__/base_service.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     1806 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/__pycache__/base_service.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     1851 2022-09-15 14:09:15.000000 django_dnoticias_services-1.0.97/dnoticias_services/__pycache__/base_service.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      617 2022-12-07 12:50:35.000000 django_dnoticias_services-1.0.97/dnoticias_services/__pycache__/mail.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      615 2022-09-09 13:35:05.000000 django_dnoticias_services-1.0.97/dnoticias_services/__pycache__/mail.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      880 2022-09-09 15:14:50.000000 django_dnoticias_services-1.0.97/dnoticias_services/__pycache__/models.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      862 2022-05-25 16:05:45.000000 django_dnoticias_services-1.0.97/dnoticias_services/__pycache__/models.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)    11062 2022-05-25 14:30:58.000000 django_dnoticias_services-1.0.97/dnoticias_services/__pycache__/views.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      110 2023-03-14 11:53:02.000000 django_dnoticias_services-1.0.97/dnoticias_services/apps.py
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-03-29 16:09:26.791102 django_dnoticias_services-1.0.97/dnoticias_services/authentication/
--rw-r--r--   0 nelson    (1000) nelson    (1000)        0 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/authentication/__init__.py
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-03-29 16:09:26.795102 django_dnoticias_services-1.0.97/dnoticias_services/authentication/__pycache__/
--rw-r--r--   0 nelson    (1000) nelson    (1000)      162 2022-09-09 15:14:50.000000 django_dnoticias_services-1.0.97/dnoticias_services/authentication/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      169 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/authentication/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      160 2022-05-26 14:57:29.000000 django_dnoticias_services-1.0.97/dnoticias_services/authentication/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)    16445 2023-02-14 14:46:17.000000 django_dnoticias_services-1.0.97/dnoticias_services/authentication/__pycache__/keycloak.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)    16237 2023-02-27 14:41:15.000000 django_dnoticias_services-1.0.97/dnoticias_services/authentication/__pycache__/keycloak.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)    16268 2022-09-14 09:17:36.000000 django_dnoticias_services-1.0.97/dnoticias_services/authentication/__pycache__/keycloak.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     1483 2022-12-12 15:00:42.000000 django_dnoticias_services-1.0.97/dnoticias_services/authentication/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     1469 2023-01-30 13:45:05.000000 django_dnoticias_services-1.0.97/dnoticias_services/authentication/__pycache__/utils.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)    19981 2023-02-14 14:46:15.000000 django_dnoticias_services-1.0.97/dnoticias_services/authentication/keycloak.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     1780 2022-12-12 11:52:10.000000 django_dnoticias_services-1.0.97/dnoticias_services/authentication/utils.py
--rw-r--r--   0 nelson    (1000) nelson    (1000)     1458 2023-03-14 11:53:06.000000 django_dnoticias_services-1.0.97/dnoticias_services/base_service.py
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-03-29 16:09:26.799102 django_dnoticias_services-1.0.97/dnoticias_services/communications/
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     9977 2022-05-31 09:52:15.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/README.md
--rw-r--r--   0 nelson    (1000) nelson    (1000)      546 2022-05-25 14:40:55.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/__init__.py
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-03-29 16:09:26.815102 django_dnoticias_services-1.0.97/dnoticias_services/communications/__pycache__/
--rw-r--r--   0 nelson    (1000) nelson    (1000)      636 2022-09-09 15:14:50.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      630 2022-05-25 14:40:56.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      634 2022-05-26 14:57:29.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      679 2022-09-09 15:14:50.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/__pycache__/base.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      663 2022-05-31 14:29:06.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/__pycache__/base.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      675 2022-06-03 10:41:21.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/__pycache__/base.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     2122 2022-09-09 15:14:50.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/__pycache__/campaign.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     2051 2022-06-15 09:52:06.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/__pycache__/campaign.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     2100 2022-06-15 09:52:05.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/__pycache__/campaign.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     8425 2023-03-16 17:07:13.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/__pycache__/forms.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     8312 2023-03-21 12:23:59.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/__pycache__/forms.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     7916 2022-06-24 16:58:25.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/__pycache__/forms.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     7330 2022-09-09 15:14:50.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/__pycache__/mail.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     7104 2022-08-11 13:26:55.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/__pycache__/mail.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     7228 2022-08-18 14:39:23.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/__pycache__/mail.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)    12557 2023-03-03 13:05:30.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/__pycache__/notification.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)    12711 2023-03-14 11:48:43.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/__pycache__/notification.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)    12583 2022-05-30 10:29:17.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/__pycache__/notification.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     1265 2022-05-25 16:30:02.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/__pycache__/urls.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)    10946 2023-03-01 10:32:33.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/__pycache__/views.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)    12614 2023-02-28 13:20:41.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/__pycache__/views.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)    11965 2022-05-26 17:07:52.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/__pycache__/views.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      312 2022-05-31 13:36:07.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/base.py
--rw-r--r--   0 nelson    (1000) nelson    (1000)     1932 2022-06-15 09:52:04.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/campaign.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      830 2022-05-27 11:36:17.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/context_processors.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     9992 2023-03-15 11:08:34.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/forms.py
--rw-r--r--   0 nelson    (1000) nelson    (1000)     7986 2022-08-08 13:32:02.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/mail.py
--rw-r--r--   0 nelson    (1000) nelson    (1000)    16467 2023-03-29 11:01:55.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/notification.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     1258 2022-05-25 16:30:00.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/urls.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     9535 2023-02-28 13:20:39.000000 django_dnoticias_services-1.0.97/dnoticias_services/communications/views.py
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-03-29 16:09:26.815102 django_dnoticias_services-1.0.97/dnoticias_services/editions/
--rw-r--r--   0 nelson    (1000) nelson    (1000)       69 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/editions/__init__.py
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-03-29 16:09:26.815102 django_dnoticias_services-1.0.97/dnoticias_services/editions/__pycache__/
--rw-r--r--   0 nelson    (1000) nelson    (1000)      244 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/editions/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      691 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/editions/__pycache__/base.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      801 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/editions/__pycache__/editions.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      318 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/editions/base.py
--rw-r--r--   0 nelson    (1000) nelson    (1000)      463 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/editions/editions.py
--rw-r--r--   0 nelson    (1000) nelson    (1000)      559 2023-03-14 11:53:08.000000 django_dnoticias_services-1.0.97/dnoticias_services/mail.py
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-03-29 16:09:26.815102 django_dnoticias_services-1.0.97/dnoticias_services/migrations/
--rw-r--r--   0 nelson    (1000) nelson    (1000)      911 2022-05-25 16:05:47.000000 django_dnoticias_services-1.0.97/dnoticias_services/migrations/0001_initial.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)        0 2022-05-25 16:04:02.000000 django_dnoticias_services-1.0.97/dnoticias_services/migrations/__init__.py
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-03-29 16:09:26.819102 django_dnoticias_services-1.0.97/dnoticias_services/migrations/__pycache__/
--rw-r--r--   0 nelson    (1000) nelson    (1000)      985 2022-09-09 15:14:51.000000 django_dnoticias_services-1.0.97/dnoticias_services/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      965 2022-05-25 16:05:54.000000 django_dnoticias_services-1.0.97/dnoticias_services/migrations/__pycache__/0001_initial.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      158 2022-09-09 15:14:51.000000 django_dnoticias_services-1.0.97/dnoticias_services/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      152 2022-05-25 16:04:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/migrations/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      600 2022-05-25 16:05:05.000000 django_dnoticias_services-1.0.97/dnoticias_services/models.py
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-03-29 16:09:26.819102 django_dnoticias_services-1.0.97/dnoticias_services/payments/
--rw-r--r--   0 nelson    (1000) nelson    (1000)      429 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/__init__.py
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-03-29 16:09:26.827102 django_dnoticias_services-1.0.97/dnoticias_services/payments/__pycache__/
--rw-r--r--   0 nelson    (1000) nelson    (1000)      705 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      716 2022-04-29 11:35:44.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      687 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/__pycache__/base.cpython-37.pyc
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      706 2022-04-29 11:35:44.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/__pycache__/base.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      418 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/__pycache__/choices.cpython-37.pyc
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      433 2022-04-29 11:35:44.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/__pycache__/choices.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     1350 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/__pycache__/coupons.cpython-37.pyc
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     1360 2022-04-29 11:35:44.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/__pycache__/coupons.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     3519 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/__pycache__/items.cpython-37.pyc
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     3509 2022-04-29 11:35:44.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/__pycache__/items.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     3302 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/__pycache__/orders.cpython-37.pyc
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     3257 2022-04-29 11:35:44.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/__pycache__/orders.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     2960 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/__pycache__/payments.cpython-37.pyc
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     2962 2022-04-29 11:35:44.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/__pycache__/payments.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      998 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/__pycache__/providers.cpython-37.pyc
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     1017 2022-04-29 11:35:44.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/__pycache__/providers.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     1159 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/__pycache__/subscriptions.cpython-37.pyc
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     1171 2022-04-29 11:35:44.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/__pycache__/subscriptions.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      315 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/base.py
--rw-r--r--   0 nelson    (1000) nelson    (1000)      118 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/choices.py
--rw-r--r--   0 nelson    (1000) nelson    (1000)      956 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/coupons.py
--rw-r--r--   0 nelson    (1000) nelson    (1000)     3989 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/items.py
--rw-r--r--   0 nelson    (1000) nelson    (1000)     3003 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/orders.py
--rw-r--r--   0 nelson    (1000) nelson    (1000)     2909 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/payments.py
--rw-r--r--   0 nelson    (1000) nelson    (1000)      641 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/providers.py
--rw-r--r--   0 nelson    (1000) nelson    (1000)      790 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/payments/subscriptions.py
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-03-29 16:09:26.831102 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/
--rw-r--r--   0 nelson    (1000) nelson    (1000)      380 2022-09-09 15:13:31.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__init__.py
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-03-29 16:09:26.911104 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/
--rw-r--r--   0 nelson    (1000) nelson    (1000)      666 2022-09-09 15:14:50.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      643 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      664 2022-09-15 14:09:15.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     2179 2022-09-09 15:14:50.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/address.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     2234 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/address.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     2219 2022-09-15 14:09:15.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/address.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      581 2022-09-09 15:14:50.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/base.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      582 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/base.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      577 2022-09-15 14:09:15.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/base.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     2025 2022-09-09 15:14:50.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/billing.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     2110 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/billing.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     2065 2022-09-15 14:09:15.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/billing.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      920 2022-09-09 15:14:50.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/coupons.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      913 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/coupons.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      916 2022-09-15 14:09:15.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/coupons.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     1327 2022-09-09 15:14:50.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/digital.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     1452 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/digital.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     1365 2022-09-15 14:09:15.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/digital.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     6819 2022-09-09 15:14:50.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/product.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     6695 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/product.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     6758 2022-09-15 14:09:15.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/product.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     1040 2022-09-09 15:14:50.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/subscription.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     1037 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/subscription.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     1038 2022-09-15 14:09:15.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/subscription.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     3160 2022-09-09 15:19:47.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/user.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     3069 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/user.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     3411 2022-09-15 14:09:15.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/__pycache__/user.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     2301 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/address.py
--rw-r--r--   0 nelson    (1000) nelson    (1000)      288 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/base.py
--rw-r--r--   0 nelson    (1000) nelson    (1000)     1825 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/billing.py
--rw-r--r--   0 nelson    (1000) nelson    (1000)      680 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/coupons.py
--rw-r--r--   0 nelson    (1000) nelson    (1000)     1120 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/digital.py
--rw-r--r--   0 nelson    (1000) nelson    (1000)     7402 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/product.py
--rw-r--r--   0 nelson    (1000) nelson    (1000)      728 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/subscription.py
--rw-r--r--   0 nelson    (1000) nelson    (1000)     2667 2022-09-09 15:19:18.000000 django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/user.py
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-03-29 16:09:26.779101 django_dnoticias_services-1.0.97/dnoticias_services/templates/
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-03-29 16:09:26.779101 django_dnoticias_services-1.0.97/dnoticias_services/templates/backoffice/
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-03-29 16:09:26.911104 django_dnoticias_services-1.0.97/dnoticias_services/templates/backoffice/fcm-notifications/
--rw-rw-r--   0 nelson    (1000) nelson    (1000)    31442 2022-05-26 11:25:32.000000 django_dnoticias_services-1.0.97/dnoticias_services/templates/backoffice/fcm-notifications/form.html
--rw-rw-r--   0 nelson    (1000) nelson    (1000)    13998 2023-03-14 12:08:55.000000 django_dnoticias_services-1.0.97/dnoticias_services/templates/backoffice/fcm-notifications/list.html
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-03-29 16:09:26.915104 django_dnoticias_services-1.0.97/dnoticias_services/templates/backoffice/fcm-topics/
--rw-rw-r--   0 nelson    (1000) nelson    (1000)    12182 2022-05-25 15:36:10.000000 django_dnoticias_services-1.0.97/dnoticias_services/templates/backoffice/fcm-topics/form.html
--rw-rw-r--   0 nelson    (1000) nelson    (1000)    11431 2022-05-26 14:30:21.000000 django_dnoticias_services-1.0.97/dnoticias_services/templates/backoffice/fcm-topics/list.html
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-03-29 16:09:26.779101 django_dnoticias_services-1.0.97/dnoticias_services/templates/frontoffice/
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-03-29 16:09:26.915104 django_dnoticias_services-1.0.97/dnoticias_services/templates/frontoffice/includes/
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     8239 2022-05-27 11:34:25.000000 django_dnoticias_services-1.0.97/dnoticias_services/templates/frontoffice/includes/firebase-notifications.js
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-03-29 16:09:26.919105 django_dnoticias_services-1.0.97/dnoticias_services/utils/
--rw-r--r--   0 nelson    (1000) nelson    (1000)      129 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/utils/__init__.py
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-03-29 16:09:26.931105 django_dnoticias_services-1.0.97/dnoticias_services/utils/__pycache__/
--rw-r--r--   0 nelson    (1000) nelson    (1000)      261 2022-09-09 15:14:50.000000 django_dnoticias_services-1.0.97/dnoticias_services/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      268 2022-05-25 13:23:14.000000 django_dnoticias_services-1.0.97/dnoticias_services/utils/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      259 2022-05-26 14:57:29.000000 django_dnoticias_services-1.0.97/dnoticias_services/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     1577 2022-10-12 11:04:20.000000 django_dnoticias_services-1.0.97/dnoticias_services/utils/__pycache__/request.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     1526 2022-10-24 10:27:30.000000 django_dnoticias_services-1.0.97/dnoticias_services/utils/__pycache__/request.cpython-37.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     1564 2022-05-26 14:57:29.000000 django_dnoticias_services-1.0.97/dnoticias_services/utils/__pycache__/request.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      387 2023-02-10 15:50:01.000000 django_dnoticias_services-1.0.97/dnoticias_services/utils/__pycache__/urls.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     5477 2023-02-14 11:01:36.000000 django_dnoticias_services-1.0.97/dnoticias_services/utils/__pycache__/views.cpython-310.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     1808 2022-09-09 13:35:06.000000 django_dnoticias_services-1.0.97/dnoticias_services/utils/__pycache__/views.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     1060 2022-10-12 11:04:19.000000 django_dnoticias_services-1.0.97/dnoticias_services/utils/request.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      227 2023-02-10 15:49:58.000000 django_dnoticias_services-1.0.97/dnoticias_services/utils/urls.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     4608 2023-02-14 11:01:33.000000 django_dnoticias_services-1.0.97/dnoticias_services/utils/views.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)       38 2023-03-29 16:09:26.931105 django_dnoticias_services-1.0.97/setup.cfg
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      953 2023-03-29 16:09:08.000000 django_dnoticias_services-1.0.97/setup.py
+-rw-r--r--   0        0        0     8504 2022-05-23 10:44:57.902943 django_dnoticias_services-1.1/README.md
+-rw-r--r--   0        0        0        0 2022-05-25 13:23:14.922229 django_dnoticias_services-1.1/dnoticias_services/__init__.py
+-rw-r--r--   0        0        0      110 2023-03-14 11:53:02.164481 django_dnoticias_services-1.1/dnoticias_services/apps.py
+-rw-r--r--   0        0        0        0 2022-05-25 13:23:14.922229 django_dnoticias_services-1.1/dnoticias_services/authentication/__init__.py
+-rw-r--r--   0        0        0    16268 2022-09-14 09:17:36.996105 django_dnoticias_services-1.1/dnoticias_services/authentication/__pycache__/keycloak.cpython-39.pyc
+-rw-r--r--   0        0        0    21793 2023-05-03 09:52:34.714117 django_dnoticias_services-1.1/dnoticias_services/authentication/keycloak.py
+-rw-r--r--   0        0        0     1780 2022-12-12 11:52:10.567533 django_dnoticias_services-1.1/dnoticias_services/authentication/utils.py
+-rw-r--r--   0        0        0     1458 2023-03-14 11:53:06.048556 django_dnoticias_services-1.1/dnoticias_services/base_service.py
+-rw-r--r--   0        0        0     9977 2022-05-31 09:52:15.081929 django_dnoticias_services-1.1/dnoticias_services/communications/README.md
+-rw-r--r--   0        0        0      546 2022-05-25 14:40:55.088980 django_dnoticias_services-1.1/dnoticias_services/communications/__init__.py
+-rw-r--r--   0        0        0      312 2022-05-31 13:36:07.428819 django_dnoticias_services-1.1/dnoticias_services/communications/base.py
+-rw-r--r--   0        0        0     1932 2022-06-15 09:52:04.884099 django_dnoticias_services-1.1/dnoticias_services/communications/campaign.py
+-rw-r--r--   0        0        0      830 2022-05-27 11:36:17.379337 django_dnoticias_services-1.1/dnoticias_services/communications/context_processors.py
+-rw-r--r--   0        0        0     9992 2023-03-15 11:08:34.805569 django_dnoticias_services-1.1/dnoticias_services/communications/forms.py
+-rw-r--r--   0        0        0     7986 2022-08-08 13:32:02.586796 django_dnoticias_services-1.1/dnoticias_services/communications/mail.py
+-rw-r--r--   0        0        0    16467 2023-03-29 11:01:55.674248 django_dnoticias_services-1.1/dnoticias_services/communications/notification.py
+-rw-r--r--   0        0        0     1258 2022-05-25 16:30:00.343321 django_dnoticias_services-1.1/dnoticias_services/communications/urls.py
+-rw-r--r--   0        0        0     9535 2023-02-28 13:20:39.922125 django_dnoticias_services-1.1/dnoticias_services/communications/views.py
+-rw-r--r--   0        0        0       69 2022-05-25 13:23:14.926229 django_dnoticias_services-1.1/dnoticias_services/editions/__init__.py
+-rw-r--r--   0        0        0      318 2022-05-25 13:23:14.926229 django_dnoticias_services-1.1/dnoticias_services/editions/base.py
+-rw-r--r--   0        0        0      463 2022-05-25 13:23:14.926229 django_dnoticias_services-1.1/dnoticias_services/editions/editions.py
+-rw-r--r--   0        0        0      559 2023-03-14 11:53:08.144596 django_dnoticias_services-1.1/dnoticias_services/mail.py
+-rw-r--r--   0        0        0      911 2022-05-25 16:05:47.245917 django_dnoticias_services-1.1/dnoticias_services/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-05-25 16:04:02.278616 django_dnoticias_services-1.1/dnoticias_services/migrations/__init__.py
+-rw-r--r--   0        0        0      600 2022-05-25 16:05:05.166185 django_dnoticias_services-1.1/dnoticias_services/models.py
+-rw-r--r--   0        0        0      429 2022-05-25 13:23:14.926229 django_dnoticias_services-1.1/dnoticias_services/payments/__init__.py
+-rw-r--r--   0        0        0      315 2022-05-25 13:23:14.926229 django_dnoticias_services-1.1/dnoticias_services/payments/base.py
+-rw-r--r--   0        0        0      118 2022-05-25 13:23:14.926229 django_dnoticias_services-1.1/dnoticias_services/payments/choices.py
+-rw-r--r--   0        0        0      956 2022-05-25 13:23:14.926229 django_dnoticias_services-1.1/dnoticias_services/payments/coupons.py
+-rw-r--r--   0        0        0     3989 2022-05-25 13:23:14.926229 django_dnoticias_services-1.1/dnoticias_services/payments/items.py
+-rw-r--r--   0        0        0     3003 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1/dnoticias_services/payments/orders.py
+-rw-r--r--   0        0        0     2909 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1/dnoticias_services/payments/payments.py
+-rw-r--r--   0        0        0      641 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1/dnoticias_services/payments/providers.py
+-rw-r--r--   0        0        0      790 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1/dnoticias_services/payments/subscriptions.py
+-rw-r--r--   0        0        0      380 2022-09-09 15:13:31.674218 django_dnoticias_services-1.1/dnoticias_services/subscriptions/__init__.py
+-rw-r--r--   0        0        0     2301 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1/dnoticias_services/subscriptions/address.py
+-rw-r--r--   0        0        0      288 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1/dnoticias_services/subscriptions/base.py
+-rw-r--r--   0        0        0     1825 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1/dnoticias_services/subscriptions/billing.py
+-rw-r--r--   0        0        0      680 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1/dnoticias_services/subscriptions/coupons.py
+-rw-r--r--   0        0        0     1120 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1/dnoticias_services/subscriptions/digital.py
+-rw-r--r--   0        0        0     7402 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1/dnoticias_services/subscriptions/product.py
+-rw-r--r--   0        0        0      728 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1/dnoticias_services/subscriptions/subscription.py
+-rw-r--r--   0        0        0     2667 2022-09-09 15:19:18.788266 django_dnoticias_services-1.1/dnoticias_services/subscriptions/user.py
+-rw-r--r--   0        0        0    31442 2022-05-26 11:25:32.824297 django_dnoticias_services-1.1/dnoticias_services/templates/backoffice/fcm-notifications/form.html
+-rw-r--r--   0        0        0    13998 2023-03-14 12:08:55.758648 django_dnoticias_services-1.1/dnoticias_services/templates/backoffice/fcm-notifications/list.html
+-rw-r--r--   0        0        0    12182 2022-05-25 15:36:10.049172 django_dnoticias_services-1.1/dnoticias_services/templates/backoffice/fcm-topics/form.html
+-rw-r--r--   0        0        0    11431 2022-05-26 14:30:21.971269 django_dnoticias_services-1.1/dnoticias_services/templates/backoffice/fcm-topics/list.html
+-rw-r--r--   0        0        0     8239 2022-05-27 11:34:25.955533 django_dnoticias_services-1.1/dnoticias_services/templates/frontoffice/includes/firebase-notifications.js
+-rw-r--r--   0        0        0      129 2022-05-25 13:23:14.934229 django_dnoticias_services-1.1/dnoticias_services/utils/__init__.py
+-rw-r--r--   0        0        0     1060 2022-10-12 11:04:19.148455 django_dnoticias_services-1.1/dnoticias_services/utils/request.py
+-rw-r--r--   0        0        0      227 2023-02-10 15:49:58.731527 django_dnoticias_services-1.1/dnoticias_services/utils/urls.py
+-rw-r--r--   0        0        0     4608 2023-02-14 11:01:33.706003 django_dnoticias_services-1.1/dnoticias_services/utils/views.py
+-rw-r--r--   0        0        0      699 2023-05-03 11:29:20.696188 django_dnoticias_services-1.1/pyproject.toml
+-rw-r--r--   0        0        0     9351 1970-01-01 00:00:00.000000 django_dnoticias_services-1.1/PKG-INFO
```

### Comparing `django_dnoticias_services-1.0.97/PKG-INFO` & `django_dnoticias_services-1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: django_dnoticias_services
-Version: 1.0.97
-Home-page: https://www.dnoticias.pt/
-Author: Pedro Mendes
-Author-email: pedro.trabalho.uma@gmail.com
-Maintainer: Nélson Gomes
-Maintainer-email: ngoncalves@dnoticias.pt
-License: MIT
-Description-Content-Type: text/markdown
-
 # dnoticias_services
 
 ## Import:
 
 `from dnoticias_services.<module> import <function_name>`
 
 `eg:`
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django_dnoticias_services-1.0.97/README.md` & `django_dnoticias_services-1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: django-dnoticias-services
+Version: 1.1
+Summary: Dnoticias Services
+License: MIT
+Author: Pedro Mendes
+Author-email: pedro.trabalho.uma@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: django
+Requires-Dist: django-dnoticias-services
+Requires-Dist: django-redis-sessions
+Requires-Dist: hiredis (==2.2.2)
+Requires-Dist: mozilla_django_oidc
+Requires-Dist: python-keycloak
+Requires-Dist: redis (==3.5.3)
+Requires-Dist: requests
+Description-Content-Type: text/markdown
+
 # dnoticias_services
 
 ## Import:
 
 `from dnoticias_services.<module> import <function_name>`
 
 `eg:`
@@ -189,7 +214,8 @@
     - ROLES_SELECT2_API_URL
     - USER_ROLES_API_URL
     - USER_SUBSCRIPTIONS_API_URL
     - SUBSCRIPTION_DELETE_COUPON_API_URL
 
 * Editions
     - EDITIONS_USER_CONSUMABLES_API_URL (https://edicao.dnoticias.pt/api/1_0/user/{}/consumables/)
+
```

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/__pycache__/mail.cpython-39.pyc` & `django_dnoticias_services-1.1/dnoticias_services/mail.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,35 @@
-00000000: 610d 0d0a 0000 0000 47a9 0463 2f02 0000  a.......G..c/...
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
-00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
-00000040: 6402 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
-00000050: 6d07 5a07 0100 6400 6403 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
-00000060: 0100 6400 6404 6c0a 6d0b 5a0b 0100 6405  ..d.d.l.m.Z...d.
-00000070: 5a0c 6406 5300 2907 e900 0000 0029 02da  Z.d.S.)......)..
-00000080: 0f63 7265 6174 655f 6361 6d70 6169 676e  .create_campaign
-00000090: da0d 7365 6e64 5f63 616d 7061 6967 6e29  ..send_campaign)
-000000a0: 04da 0a73 656e 645f 656d 6169 6cda 0f73  ...send_email..s
-000000b0: 656e 645f 656d 6169 6c5f 6275 6c6b da13  end_email_bulk..
-000000c0: 6765 745f 7573 6572 5f65 6d61 696c 5f6c  get_user_email_l
-000000d0: 6973 74da 1d67 6574 5f75 7365 725f 6461  ist..get_user_da
-000000e0: 7461 7461 626c 655f 656d 6169 6c5f 6c69  tatable_email_li
-000000f0: 7374 2901 da0d 4e6f 7469 6669 6361 7469  st)...Notificati
-00000100: 6f6e 7329 01da 0576 6965 7773 2907 7202  ons)...views).r.
-00000110: 0000 0072 0300 0000 7204 0000 0072 0500  ...r....r....r..
-00000120: 0000 7206 0000 0072 0700 0000 7208 0000  ..r....r....r...
-00000130: 004e 290d da2a 646e 6f74 6963 6961 735f  .N)..*dnoticias_
-00000140: 7365 7276 6963 6573 2e63 6f6d 6d75 6e69  services.communi
-00000150: 6361 7469 6f6e 732e 6361 6d70 6169 676e  cations.campaign
-00000160: 7202 0000 0072 0300 0000 da26 646e 6f74  r....r.....&dnot
-00000170: 6963 6961 735f 7365 7276 6963 6573 2e63  icias_services.c
-00000180: 6f6d 6d75 6e69 6361 7469 6f6e 732e 6d61  ommunications.ma
-00000190: 696c 7204 0000 0072 0500 0000 7206 0000  ilr....r....r...
-000001a0: 0072 0700 0000 da2e 646e 6f74 6963 6961  .r......dnoticia
-000001b0: 735f 7365 7276 6963 6573 2e63 6f6d 6d75  s_services.commu
-000001c0: 6e69 6361 7469 6f6e 732e 6e6f 7469 6669  nications.notifi
-000001d0: 6361 7469 6f6e 7208 0000 00da 2164 6e6f  cationr.....!dno
-000001e0: 7469 6369 6173 5f73 6572 7669 6365 732e  ticias_services.
-000001f0: 636f 6d6d 756e 6963 6174 696f 6e73 7209  communicationsr.
-00000200: 0000 00da 075f 5f61 6c6c 5f5f a900 720f  .....__all__..r.
-00000210: 0000 0072 0f00 0000 fa32 2f61 7070 2f64  ...r.....2/app/d
-00000220: 6e6f 7469 6369 6173 5f73 6572 7669 6365  noticias_service
-00000230: 732f 646e 6f74 6963 6961 735f 7365 7276  s/dnoticias_serv
-00000240: 6963 6573 2f6d 6169 6c2e 7079 da08 3c6d  ices/mail.py..<m
-00000250: 6f64 756c 653e 0200 0000 7308 0000 0010  odule>....s.....
-00000260: 0118 060c 010c 01                        .......
+00000000: 2320 4445 5052 4543 4154 4544 0a66 726f  # DEPRECATED.fro
+00000010: 6d20 646e 6f74 6963 6961 735f 7365 7276  m dnoticias_serv
+00000020: 6963 6573 2e63 6f6d 6d75 6e69 6361 7469  ices.communicati
+00000030: 6f6e 732e 6361 6d70 6169 676e 2069 6d70  ons.campaign imp
+00000040: 6f72 7420 6372 6561 7465 5f63 616d 7061  ort create_campa
+00000050: 6967 6e2c 2073 656e 645f 6361 6d70 6169  ign, send_campai
+00000060: 676e 0a66 726f 6d20 646e 6f74 6963 6961  gn.from dnoticia
+00000070: 735f 7365 7276 6963 6573 2e63 6f6d 6d75  s_services.commu
+00000080: 6e69 6361 7469 6f6e 732e 6d61 696c 2069  nications.mail i
+00000090: 6d70 6f72 7420 280a 2020 2020 7365 6e64  mport (.    send
+000000a0: 5f65 6d61 696c 2c0a 2020 2020 7365 6e64  _email,.    send
+000000b0: 5f65 6d61 696c 5f62 756c 6b2c 0a20 2020  _email_bulk,.   
+000000c0: 2067 6574 5f75 7365 725f 656d 6169 6c5f   get_user_email_
+000000d0: 6c69 7374 2c0a 2020 2020 6765 745f 7573  list,.    get_us
+000000e0: 6572 5f64 6174 6174 6162 6c65 5f65 6d61  er_datatable_ema
+000000f0: 696c 5f6c 6973 742c 0a29 0a66 726f 6d20  il_list,.).from 
+00000100: 646e 6f74 6963 6961 735f 7365 7276 6963  dnoticias_servic
+00000110: 6573 2e63 6f6d 6d75 6e69 6361 7469 6f6e  es.communication
+00000120: 732e 6e6f 7469 6669 6361 7469 6f6e 2069  s.notification i
+00000130: 6d70 6f72 7420 4e6f 7469 6669 6361 7469  mport Notificati
+00000140: 6f6e 730a 6672 6f6d 2064 6e6f 7469 6369  ons.from dnotici
+00000150: 6173 5f73 6572 7669 6365 732e 636f 6d6d  as_services.comm
+00000160: 756e 6963 6174 696f 6e73 2069 6d70 6f72  unications impor
+00000170: 7420 7669 6577 730a 5f5f 616c 6c5f 5f20  t views.__all__ 
+00000180: 3d20 280a 2020 2020 2263 7265 6174 655f  = (.    "create_
+00000190: 6361 6d70 6169 676e 222c 0a20 2020 2022  campaign",.    "
+000001a0: 7365 6e64 5f63 616d 7061 6967 6e22 2c0a  send_campaign",.
+000001b0: 2020 2020 2273 656e 645f 656d 6169 6c22      "send_email"
+000001c0: 2c0a 2020 2020 2273 656e 645f 656d 6169  ,.    "send_emai
+000001d0: 6c5f 6275 6c6b 222c 0a20 2020 2022 6765  l_bulk",.    "ge
+000001e0: 745f 7573 6572 5f65 6d61 696c 5f6c 6973  t_user_email_lis
+000001f0: 7422 2c0a 2020 2020 2267 6574 5f75 7365  t",.    "get_use
+00000200: 725f 6461 7461 7461 626c 655f 656d 6169  r_datatable_emai
+00000210: 6c5f 6c69 7374 222c 0a20 2020 2022 4e6f  l_list",.    "No
+00000220: 7469 6669 6361 7469 6f6e 7322 0a29 0a    tifications".).
```

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/authentication/__pycache__/keycloak.cpython-310.pyc` & `django_dnoticias_services-1.1/dnoticias_services/authentication/__pycache__/keycloak.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Feb 14 14:46:15 2023 UTC, .py size: 19981 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,1028 +1,1017 @@
-00000000: 6f0d 0d0a 0000 0000 b79e eb63 0d4e 0000  o..........c.N..
+00000000: 610d 0d0a 0000 0000 de54 2063 6149 0000  a........T caI..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 aa01 0000 6400  .....@...s....d.
+00000020: 0005 0000 0040 0000 0073 9601 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 0100 6400  d.l.m.Z.m.Z...d.
 00000070: 6405 6c0a 6d0b 5a0b 0100 6400 6406 6c0c  d.l.m.Z...d.d.l.
 00000080: 6d0d 5a0d 0100 6400 6407 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
-00000090: 0100 6400 6408 6c10 6d11 5a12 6d13 5a13  ..d.d.l.m.Z.m.Z.
-000000a0: 6d14 5a14 0100 6400 6409 6c15 6d16 5a16  m.Z...d.d.l.m.Z.
-000000b0: 0100 6400 640a 6c17 6d18 5a18 0100 640b  ..d.d.l.m.Z...d.
-000000c0: 640c 6c19 6d1a 5a1a 0100 6509 8300 5a1b  d.l.m.Z...e...Z.
-000000d0: 6500 a01c 651d a101 5a1e 4700 640d 640e  e...e...Z.G.d.d.
-000000e0: 8400 640e 6512 8303 5a11 4700 640f 6410  ..d.e...Z.G.d.d.
-000000f0: 8400 6410 8302 5a1f 4700 6411 6412 8400  ..d...Z.G.d.d...
+00000090: 0100 6400 6408 6c10 6d11 5a11 0100 6400  ..d.d.l.m.Z...d.
+000000a0: 6409 6c12 6d13 5a13 0100 6400 640a 6c14  d.l.m.Z...d.d.l.
+000000b0: 6d15 5a15 6d16 5a16 0100 6400 640b 6c17  m.Z.m.Z...d.d.l.
+000000c0: 6d18 5a18 0100 6509 8300 5a19 6500 a01a  m.Z...e...Z.e...
+000000d0: 651b a101 5a1c 4700 640c 640d 8400 640d  e...Z.G.d.d...d.
+000000e0: 651d 8303 5a1e 4700 640e 640f 8400 640f  e...Z.G.d.d...d.
+000000f0: 651e 6410 8d03 5a1f 4700 6411 6412 8400  e.d...Z.G.d.d...
 00000100: 6412 8302 5a20 4700 6413 6414 8400 6414  d...Z G.d.d...d.
 00000110: 8302 5a21 4700 6415 6416 8400 6416 8302  ..Z!G.d.d...d...
 00000120: 5a22 4700 6417 6418 8400 6418 8302 5a23  Z"G.d.d...d...Z#
 00000130: 4700 6419 641a 8400 641a 8302 5a24 4700  G.d.d...d...Z$G.
 00000140: 641b 641c 8400 641c 8302 5a25 4700 641d  d.d...d...Z%G.d.
 00000150: 641e 8400 641e 8302 5a26 4700 641f 6420  d...d...Z&G.d.d 
 00000160: 8400 6420 8302 5a27 4700 6421 6422 8400  ..d ..Z'G.d!d"..
 00000170: 6422 8302 5a28 4700 6423 6424 8400 6424  d"..Z(G.d#d$..d$
-00000180: 8302 5a29 4700 6425 6426 8400 6426 8302  ..Z)G.d%d&..d&..
-00000190: 5a2a 6521 8300 5a2b 6524 8300 5a2c 6522  Z*e!..Z+e$..Z,e"
-000001a0: 8300 5a2d 6523 8300 5a2e 6525 8300 5a2f  ..Z-e#..Z.e%..Z/
-000001b0: 6526 8300 5a30 6527 8300 5a31 6528 8300  e&..Z0e'..Z1e(..
-000001c0: 5a32 6529 8300 5a33 6520 8300 5a34 652a  Z2e)..Z3e ..Z4e*
-000001d0: 8300 5a35 6401 5300 2927 e900 0000 004e  ..Z5d.S.)'.....N
-000001e0: 2901 da09 7374 7274 6f62 6f6f 6c29 01da  )...strtobool)..
-000001f0: 084f 7074 696f 6e61 6c29 02da 0c67 6574  .Optional)...get
-00000200: 5f62 6163 6b65 6e64 73da 0e67 6574 5f75  _backends..get_u
-00000210: 7365 725f 6d6f 6465 6c29 01da 1353 7573  ser_model)...Sus
-00000220: 7069 6369 6f75 734f 7065 7261 7469 6f6e  piciousOperation
-00000230: 2901 da0c 4a73 6f6e 5265 7370 6f6e 7365  )...JsonResponse
-00000240: 2901 da08 7365 7474 696e 6773 2903 da0d  )...settings)...
-00000250: 4b65 7963 6c6f 616b 4164 6d69 6eda 0e4b  KeycloakAdmin..K
-00000260: 6579 636c 6f61 6b4f 7065 6e49 44da 134b  eycloakOpenID..K
-00000270: 6579 636c 6f61 6b44 656c 6574 6545 7272  eycloakDeleteErr
-00000280: 6f72 2901 da19 4f49 4443 4175 7468 656e  or)...OIDCAuthen
-00000290: 7469 6361 7469 6f6e 4261 636b 656e 6429  ticationBackend)
-000002a0: 01da 046d 6169 6ce9 0100 0000 2901 da19  ...mail.....)...
-000002b0: 7261 6973 655f 6572 726f 725f 6672 6f6d  raise_error_from
-000002c0: 5f72 6573 706f 6e73 6563 0000 0000 0000  _responsec......
-000002d0: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-000002e0: 0000 731a 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-000002f0: 0165 0366 0264 0264 0384 045a 0464 0453  .e.f.d.d...Z.d.S
-00000300: 0029 0572 0900 0000 da07 7365 7373 696f  .).r......sessio
-00000310: 6e63 0200 0000 0000 0000 0000 0000 0500  nc..............
-00000320: 0000 0600 0000 4300 0000 7330 0000 007c  ......C...s0...|
-00000330: 006a 007c 0164 019c 027d 0264 027d 037c  .j.|.d...}.d.}.|
-00000340: 00a0 017c 036a 0264 0469 007c 02a4 018e  ...|.j.d.i.|....
-00000350: 01a1 017d 0474 037c 0474 0483 0253 0029  ...}.t.|.t...S.)
-00000360: 057a ac44 656c 6574 6520 616e 2073 7065  .z.Delete an spe
-00000370: 6369 6669 6320 7573 6572 2073 6573 7369  cific user sessi
-00000380: 6f6e 206f 6e20 6b65 7963 6c6f 616b 2072  on on keycloak r
-00000390: 6561 6c6d 2e0a 0a20 2020 2020 2020 203a  ealm...        :
-000003a0: 7061 7261 6d20 7365 7373 696f 6e3a 2073  param session: s
-000003b0: 6573 7369 6f6e 2069 640a 2020 2020 2020  ession id.      
-000003c0: 2020 3a74 7970 6520 7365 7373 696f 6e3a    :type session:
-000003d0: 2073 7472 0a20 2020 2020 2020 203a 7265   str.        :re
-000003e0: 7475 726e 3a20 7265 616c 6d73 206c 6973  turn: realms lis
-000003f0: 740a 2020 2020 2020 2020 3a72 7479 7065  t.        :rtype
-00000400: 3a20 6c69 7374 0a20 2020 2020 2020 2029  : list.        )
-00000410: 02da 0572 6561 6c6d 7210 0000 007a 2761  ...realmr....z'a
-00000420: 646d 696e 2f72 6561 6c6d 732f 7b72 6561  dmin/realms/{rea
-00000430: 6c6d 7d2f 7365 7373 696f 6e73 2f7b 7365  lm}/sessions/{se
-00000440: 7373 696f 6e7d 4ea9 0029 05da 0a72 6561  ssion}N..)...rea
-00000450: 6c6d 5f6e 616d 655a 0a72 6177 5f64 656c  lm_nameZ.raw_del
-00000460: 6574 65da 0666 6f72 6d61 7472 0f00 0000  ete..formatr....
-00000470: 720b 0000 0029 05da 0473 656c 6672 1000  r....)...selfr..
-00000480: 0000 5a0b 7061 7261 6d73 5f70 6174 68da  ..Z.params_path.
-00000490: 0375 726c 5a08 6461 7461 5f72 6177 7212  .urlZ.data_rawr.
-000004a0: 0000 0072 1200 0000 fa45 2f61 7070 2f64  ...r.....E/app/d
-000004b0: 6e6f 7469 6369 6173 5f73 6572 7669 6365  noticias_service
-000004c0: 732f 646e 6f74 6963 6961 735f 7365 7276  s/dnoticias_serv
-000004d0: 6963 6573 2f61 7574 6865 6e74 6963 6174  ices/authenticat
-000004e0: 696f 6e2f 6b65 7963 6c6f 616b 2e70 79da  ion/keycloak.py.
-000004f0: 1364 656c 6574 655f 7573 6572 5f73 6573  .delete_user_ses
-00000500: 7369 6f6e 1700 0000 7308 0000 000c 0804  sion....s.......
-00000510: 0116 010a 017a 214b 6579 636c 6f61 6b41  .....z!KeycloakA
-00000520: 646d 696e 2e64 656c 6574 655f 7573 6572  dmin.delete_user
-00000530: 5f73 6573 7369 6f6e 4e29 05da 085f 5f6e  _sessionN)...__n
-00000540: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000550: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-00000560: 0373 7472 7218 0000 0072 1200 0000 7212  .strr....r....r.
-00000570: 0000 0072 1200 0000 7217 0000 0072 0900  ...r....r....r..
-00000580: 0000 1600 0000 7304 0000 0008 0012 0172  ......s........r
-00000590: 0900 0000 6300 0000 0000 0000 0000 0000  ....c...........
-000005a0: 0000 0000 0003 0000 0040 0000 0073 3600  .........@...s6.
-000005b0: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-000005c0: 6403 8400 5a04 6404 6405 8400 5a05 6406  d...Z.d.d...Z.d.
-000005d0: 6407 8400 5a06 6408 6507 6602 6409 640a  d...Z.d.e.f.d.d.
-000005e0: 8404 5a08 640b 5300 290c da0c 4261 7365  ..Z.d.S.)...Base
-000005f0: 4b65 7963 6c6f 616b 7a7f 4261 7365 2063  Keycloakz.Base c
-00000600: 6c61 7373 2074 6f20 636f 6e6e 6563 7420  lass to connect 
-00000610: 7769 7468 206b 6579 636c 6f61 6b0a 0a20  with keycloak.. 
-00000620: 2020 2054 6869 7320 636c 6173 7320 7573     This class us
-00000630: 6573 2061 2063 6f6e 7465 7874 206d 616e  es a context man
-00000640: 6167 6572 2074 6f20 6f70 656e 2061 6e64  ager to open and
-00000650: 2063 6c6f 7365 2074 6865 2063 6f6e 6e65   close the conne
-00000660: 6374 696f 6e20 7769 7468 206b 6579 636c  ction with keycl
-00000670: 6f61 6b2e 0a20 2020 2063 0100 0000 0000  oak..    c......
-00000680: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
-00000690: 0000 7376 0000 0074 00a0 0164 01a1 0101  ..sv...t...d....
-000006a0: 0074 0274 0364 0264 0383 037c 005f 0474  .t.t.d.d...|._.t
-000006b0: 0274 0364 0464 0383 037c 005f 0574 0274  .t.d.d...|._.t.t
-000006c0: 0364 0564 0383 0370 1b7c 006a 057c 005f  .d.d...p.|.j.|._
-000006d0: 0674 0274 0364 0664 0383 037c 005f 0774  .t.t.d.d...|._.t
-000006e0: 0274 0364 0764 0383 037c 005f 0874 0274  .t.d.d...|._.t.t
-000006f0: 0364 0864 0383 037c 005f 0974 0274 0364  .d.d...|._.t.t.d
-00000700: 0964 0383 037c 005f 0a64 0053 0029 0a4e  .d...|._.d.S.).N
-00000710: 7a46 5b4b 6579 636c 6f61 6b5d 2045 7374  zF[Keycloak] Est
-00000720: 6162 6c69 7368 696e 6720 6120 6e65 7720  ablishing a new 
-00000730: 636f 6e6e 6563 7469 6f6e 2077 6974 6820  connection with 
-00000740: 6175 7468 656e 7469 6361 7469 6f6e 2073  authentication s
-00000750: 6572 7665 722e 2e2e da13 4b45 5943 4c4f  erver.....KEYCLO
-00000760: 414b 5f53 4552 5645 525f 5552 4cda 00da  AK_SERVER_URL...
-00000770: 194b 4559 434c 4f41 4b5f 4144 4d49 4e5f  .KEYCLOAK_ADMIN_
-00000780: 5245 414c 4d5f 4e41 4d45 da18 4b45 5943  REALM_NAME..KEYC
-00000790: 4c4f 414b 5f55 5345 525f 5245 414c 4d5f  LOAK_USER_REALM_
-000007a0: 4e41 4d45 da17 4b45 5943 4c4f 414b 5f41  NAME..KEYCLOAK_A
-000007b0: 444d 494e 5f55 5345 524e 414d 45da 174b  DMIN_USERNAME..K
-000007c0: 4559 434c 4f41 4b5f 4144 4d49 4e5f 5041  EYCLOAK_ADMIN_PA
-000007d0: 5353 574f 5244 da12 4b45 5943 4c4f 414b  SSWORD..KEYCLOAK
-000007e0: 5f43 4c49 454e 545f 4944 da1a 4b45 5943  _CLIENT_ID..KEYC
-000007f0: 4c4f 414b 5f43 4c49 454e 545f 5345 4352  LOAK_CLIENT_SECR
-00000800: 4554 5f4b 4559 290b da06 6c6f 6767 6572  ET_KEY)...logger
-00000810: da05 6465 6275 67da 0767 6574 6174 7472  ..debug..getattr
-00000820: 7208 0000 00da 0a73 6572 7665 725f 7572  r......server_ur
-00000830: 6cda 1061 646d 696e 5f72 6561 6c6d 5f6e  l..admin_realm_n
-00000840: 616d 65da 0f75 7365 725f 7265 616c 6d5f  ame..user_realm_
-00000850: 6e61 6d65 da08 7573 6572 6e61 6d65 da08  name..username..
-00000860: 7061 7373 776f 7264 da09 636c 6965 6e74  password..client
-00000870: 5f69 64da 1163 6c69 656e 745f 7365 6372  _id..client_secr
-00000880: 6574 5f6b 6579 a901 7215 0000 0072 1200  et_key..r....r..
-00000890: 0000 7212 0000 0072 1700 0000 da08 5f5f  ..r....r......__
-000008a0: 696e 6974 5f5f 2a00 0000 7310 0000 000a  init__*...s.....
-000008b0: 010e 010e 0114 010e 010e 010e 0112 017a  ...............z
-000008c0: 1542 6173 654b 6579 636c 6f61 6b2e 5f5f  .BaseKeycloak.__
-000008d0: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
-000008e0: 0000 0001 0000 0009 0000 0043 0000 0073  ...........C...s
-000008f0: 4600 0000 7400 7c00 6a01 7c00 6a02 7c00  F...t.|.j.|.j.|.
-00000900: 6a03 7c00 6a04 7c00 6a05 6700 6401 a201  j.|.j.|.j.g.d...
-00000910: 6402 6403 8d07 7c00 5f06 7407 7c00 6a01  d.d...|._.t.|.j.
-00000920: 7c00 6a08 7c00 6a05 7c00 6a09 6402 6404  |.j.|.j.|.j.d.d.
-00000930: 8d05 7c00 5f0a 7c00 5300 2905 4e29 04da  ..|._.|.S.).N)..
-00000940: 0367 6574 da03 7075 74da 0470 6f73 74da  .get..put..post.
-00000950: 0664 656c 6574 6554 2907 7229 0000 0072  .deleteT).r)...r
-00000960: 2c00 0000 722d 0000 0072 1300 0000 722b  ,...r-...r....r+
-00000970: 0000 005a 1261 7574 6f5f 7265 6672 6573  ...Z.auto_refres
-00000980: 685f 746f 6b65 6eda 0676 6572 6966 7929  h_token..verify)
-00000990: 0572 2900 0000 722e 0000 0072 1300 0000  .r)...r....r....
-000009a0: 722f 0000 0072 3600 0000 290b 7209 0000  r/...r6...).r...
-000009b0: 0072 2900 0000 722c 0000 0072 2d00 0000  .r)...r,...r-...
-000009c0: 722a 0000 0072 2b00 0000 da0e 6b65 7963  r*...r+.....keyc
-000009d0: 6c6f 616b 5f61 646d 696e 720a 0000 0072  loak_adminr....r
-000009e0: 2e00 0000 722f 0000 00da 0f6b 6579 636c  ....r/.....keycl
-000009f0: 6f61 6b5f 6f70 656e 6964 7230 0000 0072  oak_openidr0...r
-00000a00: 1200 0000 7212 0000 0072 1700 0000 da09  ....r....r......
-00000a10: 5f5f 656e 7465 725f 5f34 0000 0073 2200  __enter__4...s".
-00000a20: 0000 0201 0401 0401 0401 0401 0401 0601  ................
-00000a30: 0201 08f9 020a 0401 0401 0401 0401 0201  ................
-00000a40: 08fb 0408 7a16 4261 7365 4b65 7963 6c6f  ....z.BaseKeyclo
-00000a50: 616b 2e5f 5f65 6e74 6572 5f5f 6304 0000  ak.__enter__c...
-00000a60: 0000 0000 0000 0000 0005 0000 0003 0000  ................
-00000a70: 0043 0000 0073 3200 0000 7400 a001 6401  .C...s2...t...d.
-00000a80: a101 0100 7c00 6a02 6a03 a004 6402 a101  ....|.j.j...d...
-00000a90: 7d04 7c04 7217 7c00 6a02 6a05 a006 7c04  }.|.r.|.j.j...|.
-00000aa0: a101 0100 6400 5300 6400 5300 2903 4e7a  ....d.S.d.S.).Nz
-00000ab0: 3b5b 4b65 7963 6c6f 616b 5d20 436c 6f73  ;[Keycloak] Clos
-00000ac0: 696e 6720 636f 6e6e 6563 7469 6f6e 2077  ing connection w
-00000ad0: 6974 6820 6175 7468 656e 7469 6361 7469  ith authenticati
-00000ae0: 6f6e 2073 6572 7665 722e 2e2e da0d 7265  on server.....re
-00000af0: 6672 6573 685f 746f 6b65 6e29 0772 2600  fresh_token).r&.
-00000b00: 0000 7227 0000 0072 3700 0000 da05 746f  ..r'...r7.....to
-00000b10: 6b65 6e72 3200 0000 7238 0000 00da 066c  kenr2...r8.....l
-00000b20: 6f67 6f75 7429 0572 1500 0000 da08 6578  ogout).r......ex
-00000b30: 635f 7479 7065 da09 6578 635f 7661 6c75  c_type..exc_valu
-00000b40: 65da 0974 7261 6365 6261 636b 5a13 6164  e..tracebackZ.ad
-00000b50: 6d69 6e5f 7265 6672 6573 685f 746f 6b65  min_refresh_toke
-00000b60: 6e72 1200 0000 7212 0000 0072 1700 0000  nr....r....r....
-00000b70: da08 5f5f 6578 6974 5f5f 4900 0000 730a  ..__exit__I...s.
-00000b80: 0000 000a 010e 0104 0212 0104 ff7a 1542  .............z.B
-00000b90: 6173 654b 6579 636c 6f61 6b2e 5f5f 6578  aseKeycloak.__ex
-00000ba0: 6974 5f5f da06 7265 7475 726e 6301 0000  it__..returnc...
-00000bb0: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00000bc0: 0043 0000 0073 2c00 0000 7400 8300 7d01  .C...s,...t...}.
-00000bd0: 7c01 4400 5d0c 7d02 7401 7c02 6a02 7403  |.D.].}.t.|.j.t.
-00000be0: 8302 7211 7c02 0200 0100 5300 7105 7404  ..r.|.....S.q.t.
-00000bf0: 6401 8301 8201 2902 7a6e 5265 7475 726e  d.....).znReturn
-00000c00: 7320 7468 6520 7573 6572 2062 6163 6b65  s the user backe
-00000c10: 6e64 0a20 2020 2020 2020 203a 7265 7475  nd.        :retu
-00000c20: 726e 3a20 5573 6572 2062 6163 6b65 6e64  rn: User backend
-00000c30: 2075 7365 640a 2020 2020 2020 2020 3a72   used.        :r
-00000c40: 7479 7065 3a20 4f49 4443 4175 7468 656e  type: OIDCAuthen
-00000c50: 7469 6361 7469 6f6e 4261 636b 656e 640a  ticationBackend.
-00000c60: 2020 2020 2020 2020 7a38 4e6f 2062 6163          z8No bac
-00000c70: 6b65 6e64 2074 6861 7420 6973 2073 7562  kend that is sub
-00000c80: 636c 6173 7320 6f66 204f 4944 4341 7574  class of OIDCAut
-00000c90: 6865 6e74 6963 6174 696f 6e42 6163 6b65  henticationBacke
-00000ca0: 6e64 2905 7204 0000 00da 0a69 7373 7562  nd).r......issub
-00000cb0: 636c 6173 73da 095f 5f63 6c61 7373 5f5f  class..__class__
-00000cc0: 720c 0000 00da 0a56 616c 7565 4572 726f  r......ValueErro
-00000cd0: 7229 0372 1500 0000 da08 6261 636b 656e  r).r......backen
-00000ce0: 6473 da07 6261 636b 656e 6472 1200 0000  ds..backendr....
-00000cf0: 7212 0000 0072 1700 0000 da0b 6765 745f  r....r......get_
-00000d00: 6261 636b 656e 6450 0000 0073 0c00 0000  backendP...s....
-00000d10: 0605 0802 0c01 0801 02ff 0803 7a18 4261  ............z.Ba
-00000d20: 7365 4b65 7963 6c6f 616b 2e67 6574 5f62  seKeycloak.get_b
-00000d30: 6163 6b65 6e64 4e29 0972 1900 0000 721a  ackendN).r....r.
-00000d40: 0000 0072 1b00 0000 da07 5f5f 646f 635f  ...r......__doc_
-00000d50: 5f72 3100 0000 7239 0000 0072 4000 0000  _r1...r9...r@...
-00000d60: 720c 0000 0072 4700 0000 7212 0000 0072  r....rG...r....r
-00000d70: 1200 0000 7212 0000 0072 1700 0000 721d  ....r....r....r.
-00000d80: 0000 0025 0000 0073 0c00 0000 0800 0401  ...%...s........
-00000d90: 0804 080a 0815 1207 721d 0000 0063 0000  ........r....c..
-00000da0: 0000 0000 0000 0000 0000 0000 0000 0500  ................
-00000db0: 0000 4000 0000 7326 0000 0065 005a 0164  ..@...s&...e.Z.d
-00000dc0: 005a 0264 015a 0364 0265 0464 0365 0565  .Z.d.Z.d.e.d.e.e
-00000dd0: 0619 0066 0464 0464 0584 045a 0764 0653  ...f.d.d...Z.d.S
-00000de0: 0029 07da 1347 6574 5573 6572 4b65 7963  .)...GetUserKeyc
-00000df0: 6c6f 616b 496e 666f 7a25 4765 7420 7468  loakInfoz%Get th
-00000e00: 6520 7573 6572 2061 7474 7269 6275 7465  e user attribute
-00000e10: 7320 6672 6f6d 206b 6579 636c 6f61 6bda  s from keycloak.
-00000e20: 0565 6d61 696c 7241 0000 0063 0200 0000  .emailrA...c....
-00000e30: 0000 0000 0000 0000 0600 0000 0800 0000  ................
-00000e40: 4300 0000 7364 0000 0064 017d 0274 0083  C...sd...d.}.t..
-00000e50: 008f 237d 037c 036a 01a0 027c 01a1 017d  ..#}.|.j...|...}
-00000e60: 047c 0464 0175 0072 1a64 027c 019b 0064  .|.d.u.r.d.|...d
-00000e70: 039d 037d 0574 037c 0583 0182 017c 036a  ...}.t.|.....|.j
-00000e80: 01a0 047c 04a1 017d 0257 0064 0104 0004  ...|...}.W.d....
-00000e90: 0083 0301 007c 0253 0031 0073 2b77 0101  .....|.S.1.s+w..
-00000ea0: 0001 0001 0059 0001 007c 0253 0029 047a  .....Y...|.S.).z
-00000eb0: f547 6574 7320 616c 6c20 7468 6520 7573  .Gets all the us
-00000ec0: 6572 2061 7474 7269 6275 7465 7320 6672  er attributes fr
-00000ed0: 6f6d 206b 6579 636c 6f61 6b0a 0a20 2020  om keycloak..   
-00000ee0: 2020 2020 203a 7061 7261 6d20 656d 6169       :param emai
-00000ef0: 6c3a 2055 7365 7220 656d 6169 6c0a 2020  l: User email.  
-00000f00: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
-00000f10: 2020 3a72 6574 7572 6e3a 2055 7365 7220    :return: User 
-00000f20: 6174 7472 6962 7574 6573 2064 6963 7420  attributes dict 
-00000f30: 6f72 204e 6f6e 650a 2020 2020 2020 2020  or None.        
-00000f40: 3a72 7479 7065 3a20 6469 6374 206f 7220  :rtype: dict or 
-00000f50: 4e6f 6e65 0a20 2020 2020 2020 203a 7261  None.        :ra
-00000f60: 6973 6573 3a20 5375 7370 6963 696f 7573  ises: Suspicious
-00000f70: 4f70 6572 6174 696f 6e20 6966 2075 7365  Operation if use
-00000f80: 7220 646f 6573 206e 6f74 2065 7869 7374  r does not exist
-00000f90: 7320 6f6e 206b 6579 636c 6f61 6b0a 2020  s on keycloak.  
-00000fa0: 2020 2020 2020 4e7a 0954 6865 2075 7365        Nz.The use
-00000fb0: 7220 7a1c 2064 6f65 7320 6e6f 7420 6578  r z. does not ex
-00000fc0: 6973 7473 206f 6e20 6b65 7963 6c6f 616b  ists on keycloak
-00000fd0: 2905 721d 0000 0072 3700 0000 da0b 6765  ).r....r7.....ge
-00000fe0: 745f 7573 6572 5f69 6472 0600 0000 da08  t_user_idr......
-00000ff0: 6765 745f 7573 6572 2906 7215 0000 0072  get_user).r....r
-00001000: 4a00 0000 da09 7573 6572 5f69 6e66 6fda  J.....user_info.
-00001010: 0462 6173 65da 1075 7365 725f 6964 5f6b  .base..user_id_k
-00001020: 6579 636c 6f61 6bda 076d 6573 7361 6765  eycloak..message
-00001030: 7212 0000 0072 1200 0000 7217 0000 00da  r....r....r.....
-00001040: 085f 5f63 616c 6c5f 5f61 0000 0073 1600  .__call__a...s..
-00001050: 0000 0409 0802 0c01 0802 0c01 0801 0e02  ................
-00001060: 0af9 0409 10f7 0409 7a1c 4765 7455 7365  ........z.GetUse
-00001070: 724b 6579 636c 6f61 6b49 6e66 6f2e 5f5f  rKeycloakInfo.__
-00001080: 6361 6c6c 5f5f 4e29 0872 1900 0000 721a  call__N).r....r.
-00001090: 0000 0072 1b00 0000 7248 0000 0072 1c00  ...r....rH...r..
-000010a0: 0000 7203 0000 00da 0464 6963 7472 5100  ..r......dictrQ.
-000010b0: 0000 7212 0000 0072 1200 0000 7212 0000  ..r....r....r...
-000010c0: 0072 1700 0000 7249 0000 005e 0000 0073  .r....rI...^...s
-000010d0: 0600 0000 0800 0401 1a02 7249 0000 0063  ..........rI...c
-000010e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000010f0: 1500 0000 4000 0000 7356 0000 0065 005a  ....@...sV...e.Z
-00001100: 0164 005a 0264 015a 0364 0264 0264 0364  .d.Z.d.Z.d.d.d.d
-00001110: 0464 0464 0564 0365 0483 0066 0864 0665  .d.d.d.e...f.d.e
-00001120: 0564 0765 0564 0865 0564 0965 0664 0a65  .d.e.d.e.d.e.d.e
-00001130: 0664 0b65 0664 0c65 0764 0d65 0664 0e65  .d.e.d.e.d.e.d.e
-00001140: 0464 0f65 0866 1464 1064 1184 055a 0964  .d.e.f.d.d...Z.d
-00001150: 1253 0029 13da 0a55 7064 6174 6555 7365  .S.)...UpdateUse
-00001160: 727a 3655 7064 6174 6573 2061 6e20 7573  rz6Updates an us
-00001170: 6572 2069 6e20 626f 7468 2073 6964 6573  er in both sides
-00001180: 2028 4b65 7963 6c6f 616b 2061 6e64 2062   (Keycloak and b
-00001190: 6163 6b65 6e64 7329 2e72 1f00 0000 5446  ackends).r....TF
-000011a0: e902 0000 0072 4a00 0000 da0a 6669 7273  .....rJ.....firs
-000011b0: 745f 6e61 6d65 da09 6c61 7374 5f6e 616d  t_name..last_nam
-000011c0: 65da 0765 6e61 626c 6564 da08 6973 5f73  e..enabled..is_s
-000011d0: 7461 6666 da0c 6973 5f73 7570 6572 7573  taff..is_superus
-000011e0: 6572 da0c 6d61 785f 7365 7373 696f 6e73  er..max_sessions
-000011f0: da11 7570 6461 7465 5f61 7474 7269 6275  ..update_attribu
-00001200: 7465 73da 1163 7573 746f 6d5f 6174 7472  tes..custom_attr
-00001210: 6962 7574 6573 7241 0000 0063 0a00 0000  ibutesrA...c....
-00001220: 0000 0000 0000 0000 1200 0000 0800 0000  ................
-00001230: 4300 0000 7314 0100 0074 0083 008f 7d7d  C...s....t....}}
-00001240: 0a7c 0a6a 01a0 027c 01a1 017d 0b7c 0b64  .|.j...|...}.|.d
-00001250: 0175 0072 1464 027d 0c74 037c 0c83 0182  .u.r.d.}.t.|....
-00001260: 017c 027c 037c 0464 039c 037d 0d7c 0872  .|.|.|.d...}.|.r
-00001270: 2d7c 057c 067c 0764 049c 037c 0d64 053c  -|.|.|.d...|.d.<
-00001280: 007c 0972 2d7c 0d64 0519 00a0 047c 09a1  .|.r-|.d.....|..
-00001290: 0101 007c 0a6a 016a 057c 0b7c 0d64 068d  ...|.j.j.|.|.d..
-000012a0: 0201 007c 0a6a 01a0 067c 0ba1 017d 0e7c  ...|.j...|...}.|
-000012b0: 0aa0 07a1 007d 0f7c 0fa0 087c 0ea1 017d  .....}.|...|...}
-000012c0: 107c 1073 4c64 077d 0c74 037c 0c83 0182  .|.sLd.}.t.|....
-000012d0: 017c 0fa0 097c 0ea1 017d 117c 027c 0e64  .|...|...}.|.|.d
-000012e0: 083c 007c 037c 0e64 093c 007c 047c 0e64  .<.|.|.d.<.|.|.d
-000012f0: 0a3c 007c 057c 0e64 0b3c 007c 067c 0e64  .<.|.|.d.<.|.|.d
-00001300: 0c3c 0074 0a7c 1183 0164 0d6b 0272 7a7c  .<.t.|...d.k.rz|
-00001310: 0fa0 057c 1164 0e19 007c 0ea1 0257 0002  ...|.d...|...W..
-00001320: 0064 0104 0004 0083 0301 0053 0064 0f7d  .d.........S.d.}
-00001330: 0c74 037c 0c83 0182 0131 0073 8377 0101  .t.|.....1.s.w..
-00001340: 0001 0001 0059 0001 0064 0153 0029 1061  .....Y...d.S.).a
-00001350: e502 0000 5570 6461 7465 7320 616e 2075  ....Updates an u
-00001360: 7365 7220 696e 2062 6163 6b65 6e64 2061  ser in backend a
-00001370: 6e64 206b 6579 636c 6f61 6b20 746f 206b  nd keycloak to k
-00001380: 6565 7020 7468 6520 6461 7461 2063 6f6e  eep the data con
-00001390: 7369 7374 656e 6379 0a20 2020 2020 2020  sistency.       
-000013a0: 200a 2020 2020 2020 2020 3a70 6172 616d   .        :param
-000013b0: 2065 6d61 696c 3a20 5573 6572 2065 6d61   email: User ema
-000013c0: 696c 2074 6861 7420 7765 2077 616e 7420  il that we want 
-000013d0: 746f 2075 7064 6174 650a 2020 2020 2020  to update.      
-000013e0: 2020 3a70 6172 616d 2066 6972 7374 5f6e    :param first_n
-000013f0: 616d 653a 204e 6577 2066 6972 7374 206e  ame: New first n
-00001400: 616d 652e 2044 6566 6175 6c74 3d27 270a  ame. Default=''.
-00001410: 2020 2020 2020 2020 3a70 6172 616d 206c          :param l
-00001420: 6173 745f 6e61 6d65 3a20 4e65 7720 6c61  ast_name: New la
-00001430: 7374 206e 616d 652e 2044 6566 6175 6c74  st name. Default
-00001440: 3d27 270a 2020 2020 2020 2020 3a70 6172  =''.        :par
-00001450: 616d 2065 6e61 626c 6564 3a20 5472 7565  am enabled: True
-00001460: 2069 6620 7468 6520 7573 6572 2069 7320   if the user is 
-00001470: 656e 6162 6c65 6420 2861 6374 6976 6529  enabled (active)
-00001480: 2e20 4465 6661 756c 743d 5472 7565 0a20  . Default=True. 
-00001490: 2020 2020 2020 203a 7061 7261 6d20 6973         :param is
-000014a0: 5f73 7461 6666 3a20 4966 2054 7275 652c  _staff: If True,
-000014b0: 2073 6574 7320 6973 5f73 7461 6666 2074   sets is_staff t
-000014c0: 6f20 5472 7565 2e20 4465 6661 756c 743d  o True. Default=
-000014d0: 4661 6c73 650a 2020 2020 2020 2020 3a70  False.        :p
-000014e0: 6172 616d 2069 735f 7375 7065 7275 7365  aram is_superuse
-000014f0: 723a 2049 6620 5472 7565 2c20 7365 7473  r: If True, sets
-00001500: 2069 735f 7375 7065 7275 7365 7220 746f   is_superuser to
-00001510: 2054 7275 652e 2044 6566 6175 6c74 3d46   True. Default=F
-00001520: 616c 7365 0a20 2020 2020 2020 203a 7061  alse.        :pa
-00001530: 7261 6d20 6d61 785f 7365 7373 696f 6e73  ram max_sessions
-00001540: 3a20 4d61 7820 7365 7373 696f 6e73 2061  : Max sessions a
-00001550: 6c6c 6f77 6564 2074 6f20 7468 6973 2075  llowed to this u
-00001560: 7365 722e 2044 6566 6175 6c74 3d32 0a20  ser. Default=2. 
-00001570: 2020 2020 2020 203a 7061 7261 6d20 7570         :param up
-00001580: 6461 7465 5f61 7474 7269 6275 7465 733a  date_attributes:
-00001590: 2055 7064 6174 6573 2074 6865 2069 735f   Updates the is_
-000015a0: 7374 6166 662c 2069 735f 7375 7065 7275  staff, is_superu
-000015b0: 7365 7220 616e 6420 6d61 785f 7365 7373  ser and max_sess
-000015c0: 696f 6e20 6f6e 206b 6579 636c 6f61 6b0a  ion on keycloak.
-000015d0: 2020 2020 2020 2020 6966 2069 7320 5472          if is Tr
-000015e0: 7565 2e20 4465 6661 756c 743a 2054 7275  ue. Default: Tru
-000015f0: 650a 2020 2020 2020 2020 2e2e 2e0a 2020  e.        ....  
-00001600: 2020 2020 2020 3a72 6574 7572 6e3a 2043        :return: C
-00001610: 7265 6174 6564 2075 7365 720a 2020 2020  reated user.    
-00001620: 2020 2020 3a72 7479 7065 3a20 5573 6572      :rtype: User
-00001630: 0a20 2020 2020 2020 204e 7a24 5468 6174  .        Nz$That
-00001640: 2075 7365 7220 646f 6573 6e27 7420 6578   user doesn't ex
-00001650: 6973 7473 2069 6e20 6b65 7963 6c6f 616b  ists in keycloak
-00001660: 2903 da09 6669 7273 744e 616d 65da 086c  )...firstName..l
-00001670: 6173 744e 616d 6572 5700 0000 a903 7258  astNamerW.....rX
-00001680: 0000 0072 5900 0000 725a 0000 00da 0a61  ...rY...rZ.....a
-00001690: 7474 7269 6275 7465 73a9 02da 0775 7365  ttributes....use
-000016a0: 725f 6964 da07 7061 796c 6f61 64fa 1a43  r_id..payload..C
-000016b0: 6c61 696d 7320 7665 7269 6669 6361 7469  laims verificati
-000016c0: 6f6e 2066 6169 6c65 64da 0a67 6976 656e  on failed..given
-000016d0: 5f6e 616d 65da 0b66 616d 696c 795f 6e61  _name..family_na
-000016e0: 6d65 da09 6973 5f61 6374 6976 6572 5800  me..is_activerX.
-000016f0: 0000 7259 0000 0072 0e00 0000 7201 0000  ..rY...r....r...
-00001700: 007a 4343 616e 6e6f 7420 7570 6461 7465  .zCCannot update
-00001710: 2074 6865 2075 7365 722e 2055 7365 7273   the user. Users
-00001720: 2072 6574 7572 6e65 6420 7a65 726f 206f   returned zero o
-00001730: 7220 6d6f 7265 2074 6861 6e20 6f6e 6520  r more than one 
-00001740: 656e 7472 792e 290b 721d 0000 0072 3700  entry.).r....r7.
-00001750: 0000 724b 0000 0072 0600 0000 da06 7570  ..rK...r......up
-00001760: 6461 7465 da0b 7570 6461 7465 5f75 7365  date..update_use
-00001770: 7272 4c00 0000 7247 0000 00da 0d76 6572  rrL...rG.....ver
-00001780: 6966 795f 636c 6169 6d73 da16 6669 6c74  ify_claims..filt
-00001790: 6572 5f75 7365 7273 5f62 795f 636c 6169  er_users_by_clai
-000017a0: 6d73 da03 6c65 6e29 1272 1500 0000 724a  ms..len).r....rJ
-000017b0: 0000 0072 5500 0000 7256 0000 0072 5700  ...rU...rV...rW.
-000017c0: 0000 7258 0000 0072 5900 0000 725a 0000  ..rX...rY...rZ..
-000017d0: 0072 5b00 0000 725c 0000 0072 4e00 0000  .r[...r\...rN...
-000017e0: 724f 0000 0072 5000 0000 7263 0000 0072  rO...rP...rc...r
-000017f0: 4d00 0000 7246 0000 00da 0f63 6c61 696d  M...rF.....claim
-00001800: 735f 7665 7269 6669 6564 da05 7573 6572  s_verified..user
-00001810: 7372 1200 0000 7212 0000 0072 1700 0000  sr....r....r....
-00001820: 7251 0000 007b 0000 0073 4c00 0000 081b  rQ...{...sL.....
-00001830: 0c01 0802 0401 0801 0203 0201 0201 06fd  ................
-00001840: 0406 0202 0201 0201 0afd 0406 0e01 0602  ................
-00001850: 0201 0201 06fe 0c05 0802 0a01 0402 0401  ................
-00001860: 0801 0a02 0802 0801 0801 0801 0801 0c02  ................
-00001870: 0e01 10d2 0430 0801 14cf 7a13 5570 6461  .....0....z.Upda
-00001880: 7465 5573 6572 2e5f 5f63 616c 6c5f 5f4e  teUser.__call__N
-00001890: 290a 7219 0000 0072 1a00 0000 721b 0000  ).r....r....r...
-000018a0: 0072 4800 0000 7252 0000 0072 1c00 0000  .rH...rR...r....
-000018b0: da04 626f 6f6c da03 696e 74da 0455 7365  ..bool..int..Use
-000018c0: 7272 5100 0000 7212 0000 0072 1200 0000  rrQ...r....r....
-000018d0: 7212 0000 0072 1700 0000 7253 0000 0078  r....r....rS...x
-000018e0: 0000 0073 3e00 0000 0800 0401 0205 0201  ...s>...........
-000018f0: 0201 0201 0201 0201 0201 0401 04f6 0202  ................
-00001900: 02fe 0203 02fd 0204 02fc 0205 02fb 0206  ................
-00001910: 02fa 0207 02f9 0208 02f8 0209 02f7 020a  ................
-00001920: 02f6 020b 0ef5 7253 0000 0063 0000 0000  ......rS...c....
-00001930: 0000 0000 0000 0000 0000 0000 1b00 0000  ................
-00001940: 4000 0000 739e 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-00001950: 0264 0164 0164 0264 0364 0464 0264 0364  .d.d.d.d.d.d.d.d
-00001960: 0364 0364 0565 0383 0066 0b64 0665 0464  .d.d.e...f.d.e.d
-00001970: 0765 0565 0419 0064 0865 0565 0419 0064  .e.e...d.e.e...d
-00001980: 0965 0565 0619 0064 0a65 0565 0619 0064  .e.e...d.e.e...d
-00001990: 0b65 0565 0419 0064 0c65 0565 0619 0064  .e.e...d.e.e...d
-000019a0: 0d65 0565 0619 0064 0e65 0565 0619 0064  .e.e...d.e.e...d
-000019b0: 0f65 0565 0619 0064 1065 0565 0719 0064  .e.e...d.e.e...d
-000019c0: 1165 0565 0319 0064 1265 0866 1a64 1364  .e.e...d.e.f.d.d
-000019d0: 1484 055a 0964 1565 0366 0264 1664 1784  ...Z.d.e.f.d.d..
-000019e0: 045a 0a64 0453 0029 18da 0a43 7265 6174  .Z.d.S.)...Creat
-000019f0: 6555 7365 7272 1f00 0000 5446 4e72 5400  eUserr....TFNrT.
-00001a00: 0000 724a 0000 0072 5500 0000 7256 0000  ..rJ...rU...rV..
-00001a10: 0072 5700 0000 da0e 656d 6169 6c5f 7665  .rW.....email_ve
-00001a20: 7269 6669 6564 722d 0000 00da 1274 656d  rifiedr-.....tem
-00001a30: 706f 7261 7279 5f70 6173 7377 6f72 6472  porary_passwordr
-00001a40: 5800 0000 7259 0000 00da 1273 656e 645f  X...rY.....send_
-00001a50: 656d 6169 6c5f 746f 5f75 7365 7272 5a00  email_to_userrZ.
-00001a60: 0000 725c 0000 0072 4100 0000 630d 0000  ..r\...rA...c...
-00001a70: 0000 0000 0000 0000 0019 0000 000d 0000  ................
-00001a80: 004b 0000 0073 6c02 0000 7400 8300 9001  .K...sl...t.....
-00001a90: 8f27 7d0e 7c0e 6a01 a002 7c01 a101 7d0f  .'}.|.j...|...}.
-00001aa0: 7c0f 0c00 7d10 7c10 727c 7c07 7219 7403  |...}.|.r||.r.t.
-00001ab0: 6a04 6a05 6401 6402 8d01 7d06 6403 6404  j.j.d.d...}.d.d.
-00001ac0: 6901 7d11 7c0d a006 6405 a101 7253 7c0d  i.}.|...d...rS|.
-00001ad0: a006 6406 a101 7253 7c0d 6406 1900 a006  ..d...rS|.d.....
-00001ae0: 6407 6408 a102 7d12 7c12 a007 a100 7d12  d.d...}.|.....}.
-00001af0: 7408 a009 7c12 a101 a00a a100 7c0d 6406  t...|.......|.d.
-00001b00: 1900 6407 3c00 740b a00c 7c0d a006 6405  ..d.<.t...|...d.
-00001b10: a101 a101 7c11 6409 3c00 740b a00c 7c0d  ....|.d.<.t...|.
-00001b20: a006 6406 a101 a101 7c11 640a 3c00 6e06  ..d.....|.d.<.n.
-00001b30: 740d 7c06 8301 7c11 640b 3c00 7c07 7c11  t.|...|.d.<.|.|.
-00001b40: 640c 3c00 7c08 7c09 7c0b 640d 9c03 7d13  d.<.|.|.|.d...}.
-00001b50: 7c0c 726a 7c13 a00e 7c0c a101 0100 7c0e  |.rj|...|.....|.
-00001b60: 6a01 a00f 7c01 7c01 7c02 7c03 7c04 7c05  j...|.|.|.|.|.|.
-00001b70: 7c11 6701 640e 6701 7c13 640f 9c09 a101  |.g.d.g.|.d.....
-00001b80: 7d0f 7c0e 6a01 a010 7c0f a101 7d14 7c00  }.|.j...|...}.|.
-00001b90: a011 7c14 a101 0100 7c14 a006 6410 a101  ..|.....|...d...
-00001ba0: 7d01 7c0e a012 a100 7d15 7c15 a013 7c14  }.|.....}.|...|.
-00001bb0: a101 7d16 7c16 739d 6411 7d17 7414 7c17  ..}.|.s.d.}.t.|.
-00001bc0: 8301 8201 7c15 a015 7c14 a101 7d18 7c14  ....|...|...}.|.
-00001bd0: a006 6412 7c02 a102 7c14 6413 3c00 7c14  ..d.|...|.d.<.|.
-00001be0: a006 6414 7c03 a102 7c14 6415 3c00 7c04  ..d.|...|.d.<.|.
-00001bf0: 7c14 6416 3c00 7c14 a006 6417 7c08 a102  |.d.<.|...d.|...
-00001c00: 7c14 6417 3c00 7c14 a006 6418 7c09 a102  |.d.<.|...d.|...
-00001c10: 7c14 6418 3c00 7416 7c18 8301 6419 6b02  |.d.<.t.|...d.k.
-00001c20: 72db 7c15 a017 7c18 641a 1900 7c14 a102  r.|...|.d...|...
-00001c30: 5700 0200 641b 0400 0400 8303 0100 5300  W...d.........S.
-00001c40: 7416 7c18 8301 6419 6b04 72e7 641c 7d17  t.|...d.k.r.d.}.
-00001c50: 7414 7c17 8301 8201 7c15 a018 641d 641e  t.|.....|...d.d.
-00001c60: a102 9001 7222 7c0a 9001 7216 7c10 9001  ....r"|...r.|...
-00001c70: 7216 7a18 7419 6a1a 7c01 741b 6a1c 741b  r.z.t.j.|.t.j.t.
-00001c80: 6a1d 741b 6a1e 741b 6a1f 7c02 7c03 7c01  j.t.j.t.j.|.|.|.
-00001c90: 740d 7c06 8301 641f 9c04 6420 8d06 0100  t.|...d...d ....
-00001ca0: 5700 6e09 0100 0100 0100 7420 a021 6421  W.n.......t .!d!
-00001cb0: a101 0100 5900 7c15 a00f 7c14 a101 5700  ....Y.|...|...W.
-00001cc0: 0200 641b 0400 0400 8303 0100 5300 0900  ..d.........S...
-00001cd0: 5700 641b 0400 0400 8303 0100 641b 5300  W.d.........d.S.
-00001ce0: 3100 9001 732f 7701 0100 0100 0100 5900  1...s/w.......Y.
-00001cf0: 0100 641b 5300 2922 61c3 0300 0043 7265  ..d.S.)"a....Cre
-00001d00: 6174 6573 2061 6e20 7573 6572 2069 6e20  ates an user in 
-00001d10: 6261 636b 656e 6420 616e 6420 6b65 7963  backend and keyc
-00001d20: 6c6f 616b 2073 6572 7665 720a 0a20 2020  loak server..   
-00001d30: 2020 2020 203a 7061 7261 6d20 656d 6169       :param emai
-00001d40: 6c3a 2055 7365 7220 656d 6169 6c20 7468  l: User email th
-00001d50: 6174 2077 6520 7761 6e74 2074 6f20 6372  at we want to cr
-00001d60: 6561 7465 0a20 2020 2020 2020 203a 7061  eate.        :pa
-00001d70: 7261 6d20 6669 7273 745f 6e61 6d65 3a20  ram first_name: 
-00001d80: 4e65 7720 6669 7273 7420 6e61 6d65 2e20  New first name. 
-00001d90: 4465 6661 756c 743d 2727 0a20 2020 2020  Default=''.     
-00001da0: 2020 203a 7061 7261 6d20 6c61 7374 5f6e     :param last_n
-00001db0: 616d 653a 204e 6577 206c 6173 7420 6e61  ame: New last na
-00001dc0: 6d65 2e20 4465 6661 756c 743d 2727 0a20  me. Default=''. 
-00001dd0: 2020 2020 2020 203a 7061 7261 6d20 656e         :param en
-00001de0: 6162 6c65 643a 2054 7275 6520 6966 2074  abled: True if t
-00001df0: 6865 2075 7365 7220 6973 2065 6e61 626c  he user is enabl
-00001e00: 6564 2028 6163 7469 7665 292e 2044 6566  ed (active). Def
-00001e10: 6175 6c74 3d54 7275 650a 2020 2020 2020  ault=True.      
-00001e20: 2020 3a70 6172 616d 2065 6d61 696c 5f76    :param email_v
-00001e30: 6572 6966 6965 643a 2054 7275 6520 6966  erified: True if
-00001e40: 2074 6865 2075 7365 7220 656d 6169 6c20   the user email 
-00001e50: 6973 2076 6572 6966 6965 642e 2044 6566  is verified. Def
-00001e60: 6175 6c74 3d46 616c 7365 0a20 2020 2020  ault=False.     
-00001e70: 2020 203a 7061 7261 6d20 7061 7373 776f     :param passwo
-00001e80: 7264 3a20 5573 6572 2070 6173 7377 6f72  rd: User passwor
-00001e90: 642e 2044 6566 6175 6c74 3d4e 6f6e 650a  d. Default=None.
-00001ea0: 2020 2020 2020 2020 3a70 6172 616d 2074          :param t
-00001eb0: 656d 706f 7261 7279 5f70 6173 7377 6f72  emporary_passwor
-00001ec0: 643a 2049 6620 7472 7565 2073 6574 7320  d: If true sets 
-00001ed0: 6120 7465 6d70 6f72 6172 7920 7061 7373  a temporary pass
-00001ee0: 776f 7264 2074 6f20 7573 6572 2e20 4465  word to user. De
-00001ef0: 6661 756c 743d 5472 7565 0a20 2020 2020  fault=True.     
-00001f00: 2020 203a 7061 7261 6d20 6973 5f73 7461     :param is_sta
-00001f10: 6666 3a20 4966 2054 7275 652c 2073 6574  ff: If True, set
-00001f20: 7320 6973 5f73 7461 6666 2074 6f20 5472  s is_staff to Tr
-00001f30: 7565 2e20 4465 6661 756c 743d 4661 6c73  ue. Default=Fals
-00001f40: 650a 2020 2020 2020 2020 3a70 6172 616d  e.        :param
-00001f50: 2069 735f 7375 7065 7275 7365 723a 2049   is_superuser: I
-00001f60: 6620 5472 7565 2c20 7365 7473 2069 735f  f True, sets is_
-00001f70: 7375 7065 7275 7365 7220 746f 2054 7275  superuser to Tru
-00001f80: 652e 2044 6566 6175 6c74 3d46 616c 7365  e. Default=False
-00001f90: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00001fa0: 7365 6e64 5f65 6d61 696c 5f74 6f5f 7573  send_email_to_us
-00001fb0: 6572 3a20 4966 2074 7275 652c 2073 656e  er: If true, sen
-00001fc0: 6473 2061 6e20 656d 6169 6c20 746f 2074  ds an email to t
-00001fd0: 6865 2075 7365 7220 6e6f 7469 6679 696e  he user notifyin
-00001fe0: 6720 7468 6174 2074 6865 0a20 2020 2020  g that the.     
-00001ff0: 2020 2061 6363 6f75 6e74 2077 6173 2063     account was c
-00002000: 7265 6174 6564 2e20 4465 6661 756c 743a  reated. Default:
-00002010: 2046 616c 7365 0a20 2020 2020 2020 203a   False.        :
-00002020: 7061 7261 6d20 6d61 785f 7365 7373 696f  param max_sessio
-00002030: 6e73 3a20 4d61 7820 7365 7373 696f 6e73  ns: Max sessions
-00002040: 2061 6c6c 6f77 6564 2074 6f20 7468 6973   allowed to this
-00002050: 2075 7365 722e 2044 6566 6175 6c74 3d32   user. Default=2
-00002060: 0a20 2020 2020 2020 2044 6566 6179 756c  .        Defayul
-00002070: 743a 2046 616c 7365 0a20 2020 2020 2020  t: False.       
-00002080: 202e 2e2e 0a20 2020 2020 2020 203a 7265   ....        :re
-00002090: 7475 726e 3a20 4372 6561 7465 6420 7573  turn: Created us
-000020a0: 6572 0a20 2020 2020 2020 203a 7274 7970  er.        :rtyp
-000020b0: 653a 2055 7365 720a 2020 2020 2020 2020  e: User.        
-000020c0: e90e 0000 00a9 01da 066c 656e 6774 68da  .........length.
-000020d0: 0474 7970 6572 2d00 0000 5a0f 6372 6564  .typer-...Z.cred
-000020e0: 656e 7469 616c 5f64 6174 615a 0b73 6563  ential_dataZ.sec
-000020f0: 7265 745f 6461 7461 da04 7361 6c74 721f  ret_data..saltr.
-00002100: 0000 005a 0e63 7265 6465 6e74 6961 6c44  ...Z.credentialD
-00002110: 6174 615a 0a73 6563 7265 7444 6174 61da  ataZ.secretData.
-00002120: 0576 616c 7565 da09 7465 6d70 6f72 6172  .value..temporar
-00002130: 7972 5f00 0000 5a0c 7573 6572 5f64 6566  yr_...Z.user_def
-00002140: 6175 6c74 2909 724a 0000 0072 2c00 0000  ault).rJ...r,...
-00002150: 725d 0000 0072 5e00 0000 7257 0000 005a  r]...r^...rW...Z
-00002160: 0d65 6d61 696c 5665 7269 6669 6564 da0b  .emailVerified..
-00002170: 6372 6564 656e 7469 616c 735a 0a72 6561  credentialsZ.rea
-00002180: 6c6d 526f 6c65 7372 6000 0000 724a 0000  lmRolesr`...rJ..
-00002190: 0072 6400 0000 725d 0000 0072 6500 0000  .rd...r]...re...
-000021a0: 725e 0000 0072 6600 0000 7267 0000 0072  r^...rf...rg...r
-000021b0: 5800 0000 7259 0000 0072 0e00 0000 7201  X...rY...r....r.
-000021c0: 0000 004e 7a17 4d75 6c74 6970 6c65 2075  ...Nz.Multiple u
-000021d0: 7365 7273 2072 6574 7572 6e65 645a 104f  sers returnedZ.O
-000021e0: 4944 435f 4352 4541 5445 5f55 5345 5254  IDC_CREATE_USERT
-000021f0: 2904 7255 0000 0072 5600 0000 724a 0000  ).rU...rV...rJ..
-00002200: 00da 0e70 6c61 696e 5f70 6173 7377 6f72  ...plain_passwor
-00002210: 64a9 0672 4a00 0000 da0a 6672 6f6d 5f65  d..rJ.....from_e
-00002220: 6d61 696c da0d 7465 6d70 6c61 7465 5f75  mail..template_u
-00002230: 7569 64da 1062 7261 6e64 5f67 726f 7570  uid..brand_group
-00002240: 5f75 7569 64da 0773 7562 6a65 6374 da07  _uuid..subject..
-00002250: 636f 6e74 6578 747a 1d43 616e 6e6f 7420  contextz.Cannot 
-00002260: 7365 6e64 2063 7265 6174 6520 7573 6572  send create user
-00002270: 2065 6d61 696c 2922 721d 0000 0072 3700   email)"r....r7.
-00002280: 0000 724b 0000 0072 7100 0000 da07 6f62  ..rK...rq.....ob
-00002290: 6a65 6374 73da 146d 616b 655f 7261 6e64  jects..make_rand
-000022a0: 6f6d 5f70 6173 7377 6f72 6472 3200 0000  om_passwordr2...
-000022b0: da06 656e 636f 6465 da06 6261 7365 3634  ..encode..base64
-000022c0: da09 6236 3465 6e63 6f64 65da 0664 6563  ..b64encode..dec
-000022d0: 6f64 65da 046a 736f 6eda 0564 756d 7073  ode..json..dumps
-000022e0: 721c 0000 0072 6800 0000 da0b 6372 6561  r....rh.....crea
-000022f0: 7465 5f75 7365 7272 4c00 0000 da13 6e6f  te_userrL.....no
-00002300: 726d 616c 697a 655f 7573 6572 5f69 6e66  rmalize_user_inf
-00002310: 6f72 4700 0000 726a 0000 0072 0600 0000  orG...rj...r....
-00002320: 726b 0000 0072 6c00 0000 7269 0000 005a  rk...rl...ri...Z
-00002330: 0c67 6574 5f73 6574 7469 6e67 7372 0d00  .get_settingsr..
-00002340: 0000 da0a 7365 6e64 5f65 6d61 696c 7208  ....send_emailr.
-00002350: 0000 00da 1244 4546 4155 4c54 5f46 524f  .....DEFAULT_FRO
-00002360: 4d5f 454d 4149 4cda 2445 4d41 494c 5f54  M_EMAIL.$EMAIL_T
-00002370: 454d 504c 4154 455f 5245 5345 545f 4c4f  EMPLATE_RESET_LO
-00002380: 4749 4e5f 494e 464f 5f55 5549 44da 1645  GIN_INFO_UUID..E
-00002390: 4d41 494c 5f42 5241 4e44 5f47 524f 5550  MAIL_BRAND_GROUP
-000023a0: 5f55 5549 44da 1b45 4d41 494c 5f55 5345  _UUID..EMAIL_USE
-000023b0: 525f 4352 4541 5449 4f4e 5f53 5542 4a45  R_CREATION_SUBJE
-000023c0: 4354 7226 0000 00da 0965 7863 6570 7469  CTr&.....excepti
-000023d0: 6f6e 2919 7215 0000 0072 4a00 0000 7255  on).r....rJ...rU
-000023e0: 0000 0072 5600 0000 7257 0000 0072 7300  ...rV...rW...rs.
-000023f0: 0000 722d 0000 0072 7400 0000 7258 0000  ..r-...rt...rX..
-00002400: 0072 5900 0000 7275 0000 0072 5a00 0000  .rY...ru...rZ...
-00002410: 725c 0000 00da 066b 7761 7267 7372 4e00  r\.....kwargsrN.
-00002420: 0000 724f 0000 005a 0b69 735f 6e65 775f  ..rO...Z.is_new_
-00002430: 7573 6572 727d 0000 0072 7a00 0000 7260  userr}...rz...r`
-00002440: 0000 0072 4d00 0000 7246 0000 0072 6d00  ...rM...rF...rm.
-00002450: 0000 da03 6d73 6772 6e00 0000 7212 0000  ....msgrn...r...
-00002460: 0072 1200 0000 7217 0000 0072 5100 0000  .r....r....rQ...
-00002470: cc00 0000 7396 0000 000a 230c 0106 0104  ....s.....#.....
-00002480: 0204 010e 0104 0304 ff14 0410 0108 0116  ................
-00002490: 0114 0116 010c 0208 0202 0302 0102 0106  ................
-000024a0: fd04 060a 0106 0202 0202 0102 0102 0102  ................
-000024b0: 0102 0104 0104 0102 0104 f704 ff0c 0e0a  ................
-000024c0: 010a 0208 020a 0104 0104 0108 010a 0310  ................
-000024d0: 0210 0108 0110 0110 010c 020e 0110 bd0c  ................
-000024e0: 4404 0308 010e 010c 0102 0104 0102 0104  D...............
-000024f0: 0104 0104 0104 0102 0202 0102 0106 0104  ................
-00002500: fc0a fa06 0d0c 0108 0210 a402 5e26 a27a  ............^&.z
-00002510: 1343 7265 6174 6555 7365 722e 5f5f 6361  .CreateUser.__ca
-00002520: 6c6c 5f5f 724d 0000 0063 0200 0000 0000  ll__rM...c......
-00002530: 0000 0000 0000 0500 0000 0900 0000 4300  ..............C.
-00002540: 0000 73c8 0000 007c 01a0 0064 0169 00a1  ..s....|...d.i..
-00002550: 027d 027c 0244 005d 547d 0374 017c 027c  .}.|.D.]T}.t.|.|
-00002560: 0319 0074 0283 0272 5c74 037c 027c 0319  ...t...r\t.|.|..
-00002570: 0083 0164 026b 0272 1f7c 027c 0319 0064  ...d.k.r.|.|...d
-00002580: 0319 006e 037c 027c 0319 007d 0474 047c  ...n.|.|...}.t.|
-00002590: 0483 0174 026b 0272 3374 037c 0483 0164  ...t.k.r3t.|...d
-000025a0: 036b 0472 337c 0464 0319 007d 047a 0a74  .k.r3|.d...}.z.t
-000025b0: 0574 067c 0483 0183 017c 027c 033c 0057  .t.|.....|.|.<.W
-000025c0: 0071 0804 0074 0779 4a01 0001 0001 007c  .q...t.yJ......|
-000025d0: 047c 027c 033c 0059 0071 0804 0074 0879  .|.|.<.Y.q...t.y
-000025e0: 5b01 0001 0001 0074 09a0 0a64 04a1 0101  [......t...d....
-000025f0: 007c 047c 027c 033c 0059 0071 0877 0071  .|.|.|.<.Y.q.w.q
-00002600: 087c 01a0 0b7c 02a1 0101 0064 0553 0029  .|...|.....d.S.)
-00002610: 067a 2a4e 6f72 6d61 6c69 7a65 7320 7468  .z*Normalizes th
-00002620: 6520 7573 6572 2069 6e66 6f72 6d61 7469  e user informati
-00002630: 6f6e 2064 6963 7469 6f6e 6172 7972 6000  on dictionaryr`.
-00002640: 0000 720e 0000 0072 0100 0000 7a16 4361  ..r....r....z.Ca
-00002650: 6e6e 6f74 2063 6f6e 7665 7274 2074 6f20  nnot convert to 
-00002660: 626f 6f6c 4e29 0c72 3200 0000 da0a 6973  boolN).r2.....is
-00002670: 696e 7374 616e 6365 da04 6c69 7374 726c  instance..listrl
-00002680: 0000 0072 7900 0000 726f 0000 0072 0200  ...ry...ro...r..
-00002690: 0000 7244 0000 00da 0e41 7474 7269 6275  ..rD.....Attribu
-000026a0: 7465 4572 726f 7272 2600 0000 7294 0000  teErrorr&...r...
-000026b0: 0072 6800 0000 2905 7215 0000 0072 4d00  .rh...).r....rM.
-000026c0: 0000 7260 0000 00da 036b 6579 727b 0000  ..r`.....keyr{..
-000026d0: 0072 1200 0000 7212 0000 0072 1700 0000  .r....r....r....
-000026e0: 728e 0000 004f 0100 0073 2000 0000 0c02  r....O...s .....
-000026f0: 0802 0e01 2401 1802 0801 0202 1401 0c01  ....$...........
-00002700: 0c01 0c01 0a01 0c01 02fe 02f6 0e0e 7a1e  ..............z.
-00002710: 4372 6561 7465 5573 6572 2e6e 6f72 6d61  CreateUser.norma
-00002720: 6c69 7a65 5f75 7365 725f 696e 666f 290b  lize_user_info).
-00002730: 7219 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
-00002740: 5200 0000 721c 0000 0072 0300 0000 726f  R...r....r....ro
-00002750: 0000 0072 7000 0000 7271 0000 0072 5100  ...rp...rq...rQ.
-00002760: 0000 728e 0000 0072 1200 0000 7212 0000  ..r....r....r...
-00002770: 0072 1200 0000 7217 0000 0072 7200 0000  .r....r....rr...
-00002780: ca00 0000 7352 0000 0008 0002 0502 0102  ....sR..........
-00002790: 0102 0102 0102 0102 0102 0102 0102 0104  ................
-000027a0: 0104 f302 0202 fe06 0302 fd06 0402 fc06  ................
-000027b0: 0502 fb06 0602 fa06 0702 f906 0802 f806  ................
-000027c0: 0902 f706 0a02 f606 0b02 f506 0c02 f406  ................
-000027d0: 0d02 f302 0f0a f100 7f12 0472 7200 0000  ...........rr...
-000027e0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000027f0: 000b 0000 0040 0000 0073 3600 0000 6500  .....@...s6...e.
-00002800: 5a01 6400 5a02 0901 0902 0902 640a 6403  Z.d.Z.......d.d.
-00002810: 6503 6404 6504 6503 1900 6405 6505 6406  e.d.e.e...d.e.d.
-00002820: 6505 6407 6506 660a 6408 6409 8405 5a07  e.d.e.f.d.d...Z.
-00002830: 6401 5300 290b da0e 5570 6461 7465 5061  d.S.)...UpdatePa
-00002840: 7373 776f 7264 4e46 724a 0000 0072 2d00  sswordNFrJ...r-.
-00002850: 0000 727c 0000 0072 7500 0000 7241 0000  ..r|...ru...rA..
-00002860: 0063 0500 0000 0000 0000 0000 0000 0a00  .c..............
-00002870: 0000 0b00 0000 4b00 0000 730a 0100 0064  ......K...s....d
-00002880: 017d 0664 0264 0364 0464 059c 037d 0774  .}.d.d.d.d...}.t
-00002890: 0083 008f 707d 087a 087c 086a 01a0 027c  ....p}.z.|.j...|
-000028a0: 01a1 017d 0957 006e 2101 0001 0001 0064  ...}.W.n!......d
-000028b0: 067c 0764 073c 0064 087c 0764 093c 0064  .|.d.<.d.|.d.<.d
-000028c0: 0a7c 0764 0b3c 0064 0c7d 0674 037c 0764  .|.d.<.d.}.t.|.d
-000028d0: 0d7c 0664 0e8d 0306 0059 0057 0002 0064  .|.d.....Y.W...d
-000028e0: 0f04 0004 0083 0301 0053 007c 0372 3f74  .........S.|.r?t
-000028f0: 046a 056a 0664 1064 118d 017d 027c 086a  .j.j.d.d...}.|.j
-00002900: 016a 077c 097c 027c 0364 128d 0301 007c  .j.|.|.|.d.....|
-00002910: 0472 6d7a 1974 086a 097c 0174 0a6a 0b74  .rmz.t.j.|.t.j.t
-00002920: 0a6a 0c74 0a6a 0d74 0a6a 0e7c 05a0 0f64  .j.t.j.t.j.|...d
-00002930: 1364 04a1 027c 017c 0264 149c 0364 158d  .d...|.|.d...d..
-00002940: 0601 0057 006e 0901 0001 0001 0074 10a0  ...W.n.......t..
-00002950: 1164 16a1 0101 0059 0074 037c 0764 0d7c  .d.....Y.t.|.d.|
-00002960: 0664 0e8d 0357 0002 0064 0f04 0004 0083  .d...W...d......
-00002970: 0301 0053 0031 0073 7e77 0101 0001 0001  ...S.1.s~w......
-00002980: 0059 0001 0064 0f53 0029 1761 2402 0000  .Y...d.S.).a$...
-00002990: 5570 6461 7465 7320 616e 2075 7365 7220  Updates an user 
-000029a0: 7061 7373 776f 7264 206f 6e20 6b65 7963  password on keyc
-000029b0: 6c6f 616b 0a0a 2020 2020 2020 2020 3a70  loak..        :p
-000029c0: 6172 616d 2065 6d61 696c 3a20 5573 6572  aram email: User
-000029d0: 2065 6d61 696c 2074 6861 7420 7765 2077   email that we w
-000029e0: 616e 7420 746f 2075 7064 6174 6520 7468  ant to update th
-000029f0: 6520 7061 7373 776f 7264 0a20 2020 2020  e password.     
-00002a00: 2020 203a 7061 7261 6d20 7061 7373 776f     :param passwo
-00002a10: 7264 3a20 4e65 7720 7061 7373 776f 7264  rd: New password
-00002a20: 2e20 4966 204e 6f6e 652c 2074 656d 706f  . If None, tempo
-00002a30: 7261 7279 206e 6565 6420 746f 2062 6520  rary need to be 
-00002a40: 5472 7565 2e20 4465 6661 756c 743d 4e6f  True. Default=No
-00002a50: 6e65 0a20 2020 2020 2020 203a 7061 7261  ne.        :para
-00002a60: 6d20 7465 6d70 6f72 6172 793a 2049 6620  m temporary: If 
-00002a70: 5472 7565 2074 6865 2075 7365 7220 7769  True the user wi
-00002a80: 6c6c 2068 6176 6520 6120 7465 6d70 6f72  ll have a tempor
-00002a90: 6172 7920 7061 7373 776f 7264 2e20 4465  ary password. De
-00002aa0: 6661 756c 743d 4661 6c73 650a 2020 2020  fault=False.    
-00002ab0: 2020 2020 3a70 6172 616d 2073 656e 645f      :param send_
-00002ac0: 656d 6169 6c5f 746f 5f75 7365 723a 2053  email_to_user: S
-00002ad0: 656e 6473 2061 6e20 656d 6169 6c20 746f  ends an email to
-00002ae0: 2074 6865 2075 7365 7220 6e6f 7469 6679   the user notify
-00002af0: 696e 6720 7468 6520 6e65 7720 7061 7373  ing the new pass
-00002b00: 776f 7264 2e0a 2020 2020 2020 2020 4465  word..        De
-00002b10: 6661 756c 743a 2046 616c 7365 0a20 2020  fault: False.   
-00002b20: 2020 2020 202e 2e2e 0a20 2020 2020 2020       ....       
-00002b30: 203a 7265 7475 726e 3a20 7b27 7265 7375   :return: {'resu
-00002b40: 6c74 273a 2027 4f4b 2f4b 4f27 2c20 2772  lt': 'OK/KO', 'r
-00002b50: 6561 736f 6e27 3a20 2727 2c20 276d 6573  eason': '', 'mes
-00002b60: 7361 6765 273a 2027 277d 2028 3230 3020  sage': ''} (200 
-00002b70: 6966 204f 4b2c 2035 3030 2069 6620 6b65  if OK, 500 if ke
-00002b80: 7963 6c6f 616b 2065 7272 6f72 290a 2020  ycloak error).  
-00002b90: 2020 2020 2020 3a72 6574 7970 653a 204a        :retype: J
-00002ba0: 736f 6e52 6573 706f 6e73 650a 2020 2020  sonResponse.    
-00002bb0: 2020 2020 e9c8 0000 00da 024f 4bda 0753      .......OK..S
-00002bc0: 5543 4345 5353 721f 0000 00a9 03da 0672  UCCESSr........r
-00002bd0: 6573 756c 74da 0672 6561 736f 6e72 5000  esult..reasonrP.
-00002be0: 0000 da02 4b4f 72a0 0000 00da 0545 5252  ....KOr......ERR
-00002bf0: 4f52 72a1 0000 007a 2545 7272 6f72 2074  ORr....z%Error t
-00002c00: 7279 696e 6720 746f 2066 696e 6420 7573  rying to find us
-00002c10: 6572 2069 6e20 6b65 7963 6c6f 616b 7250  er in keycloakrP
-00002c20: 0000 00e9 f401 0000 46a9 03da 0464 6174  ........F....dat
-00002c30: 61da 0473 6166 65da 0673 7461 7475 734e  a..safe..statusN
-00002c40: 7276 0000 0072 7700 0000 2903 7262 0000  rv...rw...).rb..
-00002c50: 0072 2d00 0000 727c 0000 00da 046e 616d  .r-...r|.....nam
-00002c60: 6529 0372 a900 0000 724a 0000 0072 7e00  e).r....rJ...r~.
-00002c70: 0000 727f 0000 007a 2143 616e 6e6f 7420  ..r....z!Cannot 
-00002c80: 7365 6e64 2075 7064 6174 6520 7061 7373  send update pass
-00002c90: 776f 7264 2065 6d61 696c 2912 721d 0000  word email).r...
-00002ca0: 0072 3700 0000 724b 0000 0072 0700 0000  .r7...rK...r....
-00002cb0: 7271 0000 0072 8500 0000 7286 0000 005a  rq...r....r....Z
-00002cc0: 1173 6574 5f75 7365 725f 7061 7373 776f  .set_user_passwo
-00002cd0: 7264 720d 0000 0072 8f00 0000 7208 0000  rdr....r....r...
-00002ce0: 0072 9000 0000 7291 0000 0072 9200 0000  .r....r....r....
-00002cf0: da28 454d 4149 4c5f 5553 4552 5f50 4153  .(EMAIL_USER_PAS
-00002d00: 5357 4f52 445f 4e4f 5449 4649 4341 5449  SWORD_NOTIFICATI
-00002d10: 4f4e 5f53 5542 4a45 4354 7232 0000 0072  ON_SUBJECTr2...r
-00002d20: 2600 0000 7294 0000 0029 0a72 1500 0000  &...r....).r....
-00002d30: 724a 0000 0072 2d00 0000 727c 0000 0072  rJ...r-...r|...r
-00002d40: 7500 0000 7295 0000 0072 a800 0000 72a6  u...r....r....r.
-00002d50: 0000 0072 4e00 0000 724f 0000 0072 1200  ...rN...rO...r..
-00002d60: 0000 7212 0000 0072 1700 0000 7251 0000  ..r....r....rQ..
-00002d70: 0067 0100 0073 4800 0000 0413 0c01 0802  .g...sH.........
-00002d80: 0201 1001 0601 0801 0801 0801 0401 1001  ................
-00002d90: 10f8 040a 0e01 0602 0201 0201 0201 06fd  ................
-00002da0: 0406 0201 0401 0201 0401 0401 0401 0401  ................
-00002db0: 0a02 0201 0201 04fd 0afa 060c 0c01 0c02  ................
-00002dc0: 24dc 7a17 5570 6461 7465 5061 7373 776f  $.z.UpdatePasswo
-00002dd0: 7264 2e5f 5f63 616c 6c5f 5f29 034e 4646  rd.__call__).NFF
-00002de0: 2908 7219 0000 0072 1a00 0000 721b 0000  ).r....r....r...
-00002df0: 0072 1c00 0000 7203 0000 0072 6f00 0000  .r....r....ro...
-00002e00: 7207 0000 0072 5100 0000 7212 0000 0072  r....rQ...r....r
-00002e10: 1200 0000 7212 0000 0072 1700 0000 729b  ....r....r....r.
-00002e20: 0000 0065 0100 0073 1e00 0000 0800 0205  ...e...s........
-00002e30: 0201 0201 04fb 0202 02fe 0603 02fd 0204  ................
-00002e40: 02fc 0205 02fb 0207 0ef9 729b 0000 0063  ..........r....c
-00002e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002e60: 0600 0000 4000 0000 732a 0000 0065 005a  ....@...s*...e.Z
-00002e70: 0164 005a 0264 0164 0284 005a 0364 0365  .d.Z.d.d...Z.d.e
-00002e80: 0464 0465 0464 0565 0566 0664 0664 0784  .d.e.d.e.f.d.d..
-00002e90: 045a 0664 0853 0029 09da 1153 656e 6455  .Z.d.S.)...SendU
-00002ea0: 7064 6174 6541 6363 6f75 6e74 6302 0000  pdateAccountc...
-00002eb0: 0000 0000 0000 0000 0003 0000 0003 0000  ................
-00002ec0: 0043 0000 0073 1000 0000 6401 7d02 7400  .C...s....d.}.t.
-00002ed0: 7c01 7c02 7600 8301 5300 2902 4e29 015a  |.|.v...S.).N).Z
-00002ee0: 0f55 5044 4154 455f 5041 5353 574f 5244  .UPDATE_PASSWORD
-00002ef0: 2901 726f 0000 0029 0372 1500 0000 da06  ).ro...).r......
-00002f00: 6163 7469 6f6e da07 6163 7469 6f6e 7372  action..actionsr
-00002f10: 1200 0000 7212 0000 0072 1700 0000 da0e  ....r....r......
-00002f20: 5f61 6374 696f 6e5f 6578 6973 7473 a601  _action_exists..
-00002f30: 0000 7304 0000 0004 010c 017a 2053 656e  ..s........z Sen
-00002f40: 6455 7064 6174 6541 6363 6f75 6e74 2e5f  dUpdateAccount._
-00002f50: 6163 7469 6f6e 5f65 7869 7374 7372 4a00  action_existsrJ.
-00002f60: 0000 72ac 0000 0072 4100 0000 6303 0000  ..r....rA...c...
-00002f70: 0000 0000 0000 0000 0007 0000 0008 0000  ................
-00002f80: 0043 0000 0073 b600 0000 6401 7d03 6402  .C...s....d.}.d.
-00002f90: 6403 6404 6405 9c03 7d04 7400 8300 8f46  d.d.d...}.t....F
-00002fa0: 7d05 7c00 a001 7c02 a101 7317 6406 7c04  }.|...|...s.d.|.
-00002fb0: 6407 3c00 6408 7d03 7a1c 7c05 6a02 a003  d.<.d.}.z.|.j...
-00002fc0: 7c01 a101 7d06 7c05 6a02 6a04 7c06 7405  |...}.|.j.j.|.t.
-00002fd0: a006 7c02 6701 a101 6409 8d02 0100 640a  ..|.g...d.....d.
-00002fe0: 7c04 640b 3c00 640c 7c04 640d 3c00 5700  |.d.<.d.|.d.<.W.
-00002ff0: 6e0f 0100 0100 0100 640e 7d03 7407 a008  n.......d.}.t...
-00003000: 640f a101 0100 6410 7c04 6407 3c00 5900  d.....d.|.d.<.Y.
-00003010: 7409 7c04 6411 7c03 6412 8d03 5700 0200  t.|.d.|.d...W...
-00003020: 6400 0400 0400 8303 0100 5300 3100 7354  d.........S.1.sT
-00003030: 7701 0100 0100 0100 5900 0100 6400 5300  w.......Y...d.S.
-00003040: 2913 4e72 9c00 0000 72a2 0000 0072 a300  ).Nr....r....r..
-00003050: 0000 721f 0000 0072 9f00 0000 7a23 5468  ..r....r....z#Th
-00003060: 6520 7072 6f76 6964 6564 2061 6374 696f  e provided actio
-00003070: 6e20 646f 6573 6e27 7420 6578 6973 7473  n doesn't exists
-00003080: 2e72 5000 0000 6990 0100 0072 6100 0000  .rP...i....ra...
-00003090: 729d 0000 0072 a000 0000 729e 0000 0072  r....r....r....r
-000030a0: a100 0000 72a4 0000 007a 3d45 7272 6f72  ....r....z=Error
-000030b0: 206f 6e20 5570 6461 7465 4163 636f 756e   on UpdateAccoun
-000030c0: 7420 7365 7276 6963 6520 2864 6e6f 7469  t service (dnoti
-000030d0: 6369 6173 5f73 6572 7669 6365 203e 206b  cias_service > k
-000030e0: 6579 636c 6f61 6b29 7a2b 416e 2065 7272  eycloak)z+An err
-000030f0: 6f72 2068 6173 2062 6565 6e20 6f63 7572  or has been ocur
-00003100: 7265 6420 6f6e 2075 7064 6174 6520 6163  red on update ac
-00003110: 636f 756e 7446 72a5 0000 0029 0a72 1d00  countFr....).r..
-00003120: 0000 72ae 0000 0072 3700 0000 724b 0000  ..r....r7...rK..
-00003130: 00da 1373 656e 645f 7570 6461 7465 5f61  ...send_update_a
-00003140: 6363 6f75 6e74 728b 0000 0072 8c00 0000  ccountr....r....
-00003150: 7226 0000 0072 9400 0000 7207 0000 0029  r&...r....r....)
-00003160: 0772 1500 0000 724a 0000 0072 ac00 0000  .r....rJ...r....
-00003170: 72a8 0000 0072 a600 0000 724e 0000 0072  r....r....rN...r
-00003180: 6200 0000 7212 0000 0072 1200 0000 7217  b...r....r....r.
-00003190: 0000 0072 5100 0000 aa01 0000 7328 0000  ...rQ.......s(..
-000031a0: 0004 010c 0108 020a 0108 0104 0102 020c  ................
-000031b0: 0106 0102 010a 0106 fe08 040c 0106 0104  ................
-000031c0: 010a 010a 010c 0224 ee7a 1a53 656e 6455  .......$.z.SendU
-000031d0: 7064 6174 6541 6363 6f75 6e74 2e5f 5f63  pdateAccount.__c
-000031e0: 616c 6c5f 5f4e 2907 7219 0000 0072 1a00  all__N).r....r..
-000031f0: 0000 721b 0000 0072 ae00 0000 721c 0000  ..r....r....r...
-00003200: 0072 0700 0000 7251 0000 0072 1200 0000  .r....rQ...r....
-00003210: 7212 0000 0072 1200 0000 7217 0000 0072  r....r....r....r
-00003220: ab00 0000 a401 0000 7306 0000 0008 0008  ........s.......
-00003230: 021a 0472 ab00 0000 6300 0000 0000 0000  ...r....c.......
-00003240: 0000 0000 0000 0000 0006 0000 0040 0000  .............@..
-00003250: 0073 2200 0000 6500 5a01 6400 5a02 6401  .s"...e.Z.d.Z.d.
-00003260: 6503 6402 6503 6403 6504 6606 6404 6405  e.d.e.d.e.f.d.d.
-00003270: 8404 5a05 6406 5300 2907 da08 4765 7454  ..Z.d.S.)...GetT
-00003280: 6f6b 656e 724a 0000 0072 2d00 0000 7241  okenrJ...r-...rA
-00003290: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
-000032a0: 0400 0000 0800 0000 4300 0000 7338 0000  ........C...s8..
-000032b0: 0074 0083 008f 0f7d 037c 036a 01a0 027c  .t.....}.|.j...|
-000032c0: 017c 02a1 0257 0002 0064 0104 0004 0083  .|...W...d......
-000032d0: 0301 0053 0031 0073 1577 0101 0001 0001  ...S.1.s.w......
-000032e0: 0059 0001 0064 0153 0029 027a e547 6574  .Y...d.S.).z.Get
-000032f0: 2074 6865 2075 7365 7220 746f 6b65 6e20   the user token 
-00003300: 616e 6420 6372 6561 7465 7320 6120 6e65  and creates a ne
-00003310: 7720 7365 7373 696f 6e20 6f6e 206b 6579  w session on key
-00003320: 636c 6f61 6b0a 2020 2020 2020 2020 0a20  cloak.        . 
-00003330: 2020 2020 2020 203a 7061 7261 6d20 656d         :param em
-00003340: 6169 6c3a 2055 7365 7220 656d 6169 6c0a  ail: User email.
-00003350: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
-00003360: 6173 7377 6f72 643a 2055 7365 7220 7061  assword: User pa
-00003370: 7373 776f 7264 0a20 2020 2020 2020 202e  ssword.        .
-00003380: 2e2e 0a20 2020 2020 2020 203a 7265 7475  ...        :retu
-00003390: 726e 3a20 4163 6365 7373 2074 6f6b 656e  rn: Access token
-000033a0: 2c20 7265 6672 6573 6820 746f 6b65 6e20  , refresh token 
-000033b0: 6469 6374 0a20 2020 2020 2020 203a 7274  dict.        :rt
-000033c0: 7970 653a 2064 6963 740a 2020 2020 2020  ype: dict.      
-000033d0: 2020 4e29 0372 1d00 0000 7238 0000 0072    N).r....r8...r
-000033e0: 3b00 0000 2904 7215 0000 0072 4a00 0000  ;...).r....rJ...
-000033f0: 722d 0000 0072 4e00 0000 7212 0000 0072  r-...rN...r....r
-00003400: 1200 0000 7217 0000 0072 5100 0000 c501  ....r....rQ.....
-00003410: 0000 7306 0000 0008 090c 0124 ff7a 1147  ..s........$.z.G
-00003420: 6574 546f 6b65 6e2e 5f5f 6361 6c6c 5f5f  etToken.__call__
-00003430: 4ea9 0672 1900 0000 721a 0000 0072 1b00  N..r....r....r..
-00003440: 0000 721c 0000 0072 5200 0000 7251 0000  ..r....rR...rQ..
-00003450: 0072 1200 0000 7212 0000 0072 1200 0000  .r....r....r....
-00003460: 7217 0000 0072 b000 0000 c301 0000 7304  r....r........s.
-00003470: 0000 0008 001a 0272 b000 0000 6300 0000  .......r....c...
-00003480: 0000 0000 0000 0000 0000 0000 0004 0000  ................
-00003490: 0040 0000 00f3 1e00 0000 6500 5a01 6400  .@........e.Z.d.
-000034a0: 5a02 6401 6503 6402 6504 6604 6403 6404  Z.d.e.d.e.f.d.d.
-000034b0: 8404 5a05 6405 5300 2906 da0c 5265 6672  ..Z.d.S.)...Refr
-000034c0: 6573 6854 6f6b 656e 723a 0000 0072 4100  eshTokenr:...rA.
-000034d0: 0000 6302 0000 0000 0000 0000 0000 0003  ..c.............
-000034e0: 0000 0008 0000 0043 0000 00f3 3600 0000  .......C....6...
-000034f0: 7400 8300 8f0e 7d02 7c02 6a01 a002 7c01  t.....}.|.j...|.
-00003500: a101 5700 0200 6401 0400 0400 8303 0100  ..W...d.........
-00003510: 5300 3100 7314 7701 0100 0100 0100 5900  S.1.s.w.......Y.
-00003520: 0100 6401 5300 2902 7af9 5265 6672 6573  ..d.S.).z.Refres
-00003530: 6820 7468 6520 746f 6b65 6e20 6f6e 206b  h the token on k
-00003540: 6579 636c 6f61 6b20 616e 6420 7265 7475  eycloak and retu
-00003550: 726e 7320 7468 6520 6e65 7720 6765 6e65  rns the new gene
-00003560: 7261 7465 6420 746f 6b65 6e0a 2020 2020  rated token.    
-00003570: 2020 2020 0a20 2020 2020 2020 203a 7061      .        :pa
-00003580: 7261 6d20 7265 6672 6573 685f 746f 6b65  ram refresh_toke
-00003590: 6e3a 2052 6566 7265 7368 2074 6f6b 656e  n: Refresh token
-000035a0: 2075 7365 6420 746f 2067 656e 6572 6174   used to generat
-000035b0: 6520 6120 6e65 7720 6163 6365 7373 5f74  e a new access_t
-000035c0: 6f6b 656e 0a20 2020 2020 2020 202e 2e2e  oken.        ...
-000035d0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-000035e0: 3a20 4163 6365 7373 2054 6f6b 656e 2061  : Access Token a
-000035f0: 6e64 2052 6566 7265 7368 2054 6f6b 656e  nd Refresh Token
-00003600: 2064 6963 740a 2020 2020 2020 2020 3a72   dict.        :r
-00003610: 7479 7065 3a20 6469 6374 0a20 2020 2020  type: dict.     
-00003620: 2020 204e 2903 721d 0000 0072 3800 0000     N).r....r8...
-00003630: 723a 0000 00a9 0372 1500 0000 723a 0000  r:.....r....r:..
-00003640: 0072 4e00 0000 7212 0000 0072 1200 0000  .rN...r....r....
-00003650: 7217 0000 0072 5100 0000 d401 0000 f306  r....rQ.........
-00003660: 0000 0008 080a 0124 ff7a 1552 6566 7265  .......$.z.Refre
-00003670: 7368 546f 6b65 6e2e 5f5f 6361 6c6c 5f5f  shToken.__call__
-00003680: 4e72 b100 0000 7212 0000 0072 1200 0000  Nr....r....r....
-00003690: 7212 0000 0072 1700 0000 72b3 0000 00d2  r....r....r.....
-000036a0: 0100 00f3 0400 0000 0800 1602 72b3 0000  ............r...
-000036b0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-000036c0: 0000 0400 0000 4000 0000 72b2 0000 0029  ......@...r....)
-000036d0: 06da 0a4c 6f67 6f75 7455 7365 7272 3a00  ...LogoutUserr:.
-000036e0: 0000 7241 0000 0063 0200 0000 0000 0000  ..rA...c........
-000036f0: 0000 0000 0300 0000 0800 0000 4300 0000  ............C...
-00003700: 72b4 0000 0029 027a 7f4c 6f67 6f75 7473  r....).z.Logouts
+00000180: 8302 5a29 6521 8300 5a2a 6524 8300 5a2b  ..Z)e!..Z*e$..Z+
+00000190: 6522 8300 5a2c 6523 8300 5a2d 6525 8300  e"..Z,e#..Z-e%..
+000001a0: 5a2e 6526 8300 5a2f 6527 8300 5a30 6528  Z.e&..Z/e'..Z0e(
+000001b0: 8300 5a31 6529 8300 5a32 6520 8300 5a33  ..Z1e)..Z2e ..Z3
+000001c0: 6401 5300 2925 e900 0000 004e 2901 da09  d.S.)%.....N)...
+000001d0: 7374 7274 6f62 6f6f 6c29 01da 084f 7074  strtobool)...Opt
+000001e0: 696f 6e61 6c29 02da 0c67 6574 5f62 6163  ional)...get_bac
+000001f0: 6b65 6e64 73da 0e67 6574 5f75 7365 725f  kends..get_user_
+00000200: 6d6f 6465 6c29 01da 1353 7573 7069 6369  model)...Suspici
+00000210: 6f75 734f 7065 7261 7469 6f6e 2901 da0c  ousOperation)...
+00000220: 4a73 6f6e 5265 7370 6f6e 7365 2901 da05  JsonResponse)...
+00000230: 6361 6368 6529 01da 0873 6574 7469 6e67  cache)...setting
+00000240: 7329 01da 194f 4944 4341 7574 6865 6e74  s)...OIDCAuthent
+00000250: 6963 6174 696f 6e42 6163 6b65 6e64 2902  icationBackend).
+00000260: da0d 4b65 7963 6c6f 616b 4164 6d69 6eda  ..KeycloakAdmin.
+00000270: 0e4b 6579 636c 6f61 6b4f 7065 6e49 4429  .KeycloakOpenID)
+00000280: 01da 046d 6169 6c63 0000 0000 0000 0000  ...mailc........
+00000290: 0000 0000 0000 0000 0300 0000 0000 0000  ................
+000002a0: 7320 0000 0065 005a 0164 005a 0269 005a  s ...e.Z.d.Z.i.Z
+000002b0: 0387 0066 0164 0164 0284 085a 0487 0004  ...f.d.d...Z....
+000002c0: 005a 0553 0029 03da 0953 696e 676c 6574  .Z.S.)...Singlet
+000002d0: 6f6e 6301 0000 0000 0000 0000 0000 0003  onc.............
+000002e0: 0000 0004 0000 000f 0000 0073 3000 0000  ...........s0...
+000002f0: 7c00 7c00 6a00 7601 7226 7401 7402 7c00  |.|.j.v.r&t.t.|.
+00000300: 8302 6a03 7c01 6900 7c02 a401 8e01 7c00  ..j.|.i.|.....|.
+00000310: 6a00 7c00 3c00 7c00 6a00 7c00 1900 5300  j.|.<.|.j.|...S.
+00000320: a901 4e29 04da 0a5f 696e 7374 616e 6365  ..N)..._instance
+00000330: 73da 0573 7570 6572 720e 0000 00da 085f  s..superr......_
+00000340: 5f63 616c 6c5f 5f29 03da 0363 6c73 da04  _call__)...cls..
+00000350: 6172 6773 da06 6b77 6172 6773 a901 da09  args..kwargs....
+00000360: 5f5f 636c 6173 735f 5fa9 00fa 452f 6170  __class__...E/ap
+00000370: 702f 646e 6f74 6963 6961 735f 7365 7276  p/dnoticias_serv
+00000380: 6963 6573 2f64 6e6f 7469 6369 6173 5f73  ices/dnoticias_s
+00000390: 6572 7669 6365 732f 6175 7468 656e 7469  ervices/authenti
+000003a0: 6361 7469 6f6e 2f6b 6579 636c 6f61 6b2e  cation/keycloak.
+000003b0: 7079 7212 0000 0017 0000 0073 0600 0000  pyr........s....
+000003c0: 0001 0a01 1c02 7a12 5369 6e67 6c65 746f  ......z.Singleto
+000003d0: 6e2e 5f5f 6361 6c6c 5f5f 2906 da08 5f5f  n.__call__)...__
+000003e0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+000003f0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00000400: 7210 0000 0072 1200 0000 da0d 5f5f 636c  r....r......__cl
+00000410: 6173 7363 656c 6c5f 5f72 1800 0000 7218  asscell__r....r.
+00000420: 0000 0072 1600 0000 7219 0000 0072 0e00  ...r....r....r..
+00000430: 0000 1500 0000 7304 0000 0008 0104 0172  ......s........r
+00000440: 0e00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000450: 0000 0000 0003 0000 0040 0000 0073 2600  .........@...s&.
+00000460: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
+00000470: 6403 8400 5a04 6505 6404 9c01 6405 6406  d...Z.e.d...d.d.
+00000480: 8404 5a06 6407 5300 2908 da0c 4261 7365  ..Z.d.S.)...Base
+00000490: 4b65 7963 6c6f 616b 7a9f 4573 7461 626c  Keycloakz.Establ
+000004a0: 6973 6820 616e 2061 646d 696e 2063 6f6e  ish an admin con
+000004b0: 6e65 6374 696f 6e20 7769 7468 204b 6579  nection with Key
+000004c0: 636c 6f61 6b2e 0a20 2020 2049 6d70 6c65  cloak..    Imple
+000004d0: 6d65 6e74 6564 2077 6974 6820 5369 6e67  mented with Sing
+000004e0: 6c65 746f 6e20 746f 2061 766f 6964 2069  leton to avoid i
+000004f0: 6e73 7461 6e63 6961 7465 2065 7665 7279  nstanciate every
+00000500: 2074 696d 6520 7765 2075 7365 200a 2020   time we use .  
+00000510: 2020 6372 6561 7465 2f75 7064 6174 652f    create/update/
+00000520: 6368 616e 6765 2070 6173 7377 6f72 642f  change password/
+00000530: 6574 632e 0a20 2020 2063 0100 0000 0000  etc..    c......
+00000540: 0000 0000 0000 0100 0000 0800 0000 4300  ..............C.
+00000550: 0000 73b2 0000 0074 00a0 0164 01a1 0101  ..s....t...d....
+00000560: 0074 0274 0364 0264 0383 037c 005f 0474  .t.t.d.d...|._.t
+00000570: 0274 0364 0464 0383 037c 005f 0574 0274  .t.d.d...|._.t.t
+00000580: 0364 0564 0383 0370 367c 006a 057c 005f  .d.d...p6|.j.|._
+00000590: 0674 0274 0364 0664 0383 037c 005f 0774  .t.t.d.d...|._.t
+000005a0: 0274 0364 0764 0383 037c 005f 0874 0274  .t.d.d...|._.t.t
+000005b0: 0364 0864 0383 037c 005f 0974 0274 0364  .d.d...|._.t.t.d
+000005c0: 0964 0383 037c 005f 0a74 0b7c 006a 047c  .d...|._.t.|.j.|
+000005d0: 006a 077c 006a 087c 006a 057c 006a 0664  .j.|.j.|.j.|.j.d
+000005e0: 0a64 0b8d 067c 005f 0c74 0d7c 006a 047c  .d...|._.t.|.j.|
+000005f0: 006a 097c 006a 067c 006a 0a64 0a64 0c8d  .j.|.j.|.j.d.d..
+00000600: 057c 005f 0e64 0053 0029 0d4e 7a46 5b4b  .|._.d.S.).NzF[K
+00000610: 6579 636c 6f61 6b5d 2045 7374 6162 6c69  eycloak] Establi
+00000620: 7368 696e 6720 6120 6e65 7720 636f 6e6e  shing a new conn
+00000630: 6563 7469 6f6e 2077 6974 6820 6175 7468  ection with auth
+00000640: 656e 7469 6361 7469 6f6e 2073 6572 7665  entication serve
+00000650: 722e 2e2e da13 4b45 5943 4c4f 414b 5f53  r.....KEYCLOAK_S
+00000660: 4552 5645 525f 5552 4cda 00da 194b 4559  ERVER_URL....KEY
+00000670: 434c 4f41 4b5f 4144 4d49 4e5f 5245 414c  CLOAK_ADMIN_REAL
+00000680: 4d5f 4e41 4d45 da18 4b45 5943 4c4f 414b  M_NAME..KEYCLOAK
+00000690: 5f55 5345 525f 5245 414c 4d5f 4e41 4d45  _USER_REALM_NAME
+000006a0: da17 4b45 5943 4c4f 414b 5f41 444d 494e  ..KEYCLOAK_ADMIN
+000006b0: 5f55 5345 524e 414d 45da 174b 4559 434c  _USERNAME..KEYCL
+000006c0: 4f41 4b5f 4144 4d49 4e5f 5041 5353 574f  OAK_ADMIN_PASSWO
+000006d0: 5244 da12 4b45 5943 4c4f 414b 5f43 4c49  RD..KEYCLOAK_CLI
+000006e0: 454e 545f 4944 da1a 4b45 5943 4c4f 414b  ENT_ID..KEYCLOAK
+000006f0: 5f43 4c49 454e 545f 5345 4352 4554 5f4b  _CLIENT_SECRET_K
+00000700: 4559 5429 06da 0a73 6572 7665 725f 7572  EYT)...server_ur
+00000710: 6cda 0875 7365 726e 616d 65da 0870 6173  l..username..pas
+00000720: 7377 6f72 64da 0a72 6561 6c6d 5f6e 616d  sword..realm_nam
+00000730: 65da 0f75 7365 725f 7265 616c 6d5f 6e61  e..user_realm_na
+00000740: 6d65 da06 7665 7269 6679 2905 7227 0000  me..verify).r'..
+00000750: 00da 0963 6c69 656e 745f 6964 722a 0000  ...client_idr*..
+00000760: 00da 1163 6c69 656e 745f 7365 6372 6574  ...client_secret
+00000770: 5f6b 6579 722c 0000 0029 0fda 066c 6f67  _keyr,...)...log
+00000780: 6765 72da 0469 6e66 6fda 0767 6574 6174  ger..info..getat
+00000790: 7472 7209 0000 0072 2700 0000 5a10 6164  trr....r'...Z.ad
+000007a0: 6d69 6e5f 7265 616c 6d5f 6e61 6d65 722b  min_realm_namer+
+000007b0: 0000 0072 2800 0000 7229 0000 0072 2d00  ...r(...r)...r-.
+000007c0: 0000 722e 0000 0072 0b00 0000 da0e 6b65  ..r....r......ke
+000007d0: 7963 6c6f 616b 5f61 646d 696e 720c 0000  ycloak_adminr...
+000007e0: 00da 0f6b 6579 636c 6f61 6b5f 6f70 656e  ...keycloak_open
+000007f0: 6964 a901 da04 7365 6c66 7218 0000 0072  id....selfr....r
+00000800: 1800 0000 7219 0000 00da 085f 5f69 6e69  ....r......__ini
+00000810: 745f 5f23 0000 0073 2e00 0000 0001 0a01  t__#...s........
+00000820: 0e01 0e01 1401 0e01 0e01 0e01 0e02 0201  ................
+00000830: 0401 0401 0401 0401 0401 02fa 0809 0201  ................
+00000840: 0401 0401 0401 0401 02fb 7a15 4261 7365  ..........z.Base
+00000850: 4b65 7963 6c6f 616b 2e5f 5f69 6e69 745f  Keycloak.__init_
+00000860: 5fa9 01da 0672 6574 7572 6e63 0100 0000  _....returnc....
+00000870: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00000880: 4300 0000 7330 0000 0074 0083 007d 017c  C...s0...t...}.|
+00000890: 0144 005d 187d 0274 017c 026a 0274 0383  .D.].}.t.|.j.t..
+000008a0: 0272 0a7c 0202 0001 0053 0071 0a74 0464  .r.|.....S.q.t.d
+000008b0: 0183 0182 0164 0253 0029 037a 6e52 6574  .....d.S.).znRet
+000008c0: 7572 6e73 2074 6865 2075 7365 7220 6261  urns the user ba
+000008d0: 636b 656e 640a 2020 2020 2020 2020 3a72  ckend.        :r
+000008e0: 6574 7572 6e3a 2055 7365 7220 6261 636b  eturn: User back
+000008f0: 656e 6420 7573 6564 0a20 2020 2020 2020  end used.       
+00000900: 203a 7274 7970 653a 204f 4944 4341 7574   :rtype: OIDCAut
+00000910: 6865 6e74 6963 6174 696f 6e42 6163 6b65  henticationBacke
+00000920: 6e64 0a20 2020 2020 2020 207a 384e 6f20  nd.        z8No 
+00000930: 6261 636b 656e 6420 7468 6174 2069 7320  backend that is 
+00000940: 7375 6263 6c61 7373 206f 6620 4f49 4443  subclass of OIDC
+00000950: 4175 7468 656e 7469 6361 7469 6f6e 4261  AuthenticationBa
+00000960: 636b 656e 644e 2905 7204 0000 00da 0a69  ckendN).r......i
+00000970: 7373 7562 636c 6173 7372 1700 0000 720a  ssubclassr....r.
+00000980: 0000 00da 0a56 616c 7565 4572 726f 7229  .....ValueError)
+00000990: 0372 3500 0000 da08 6261 636b 656e 6473  .r5.....backends
+000009a0: da07 6261 636b 656e 6472 1800 0000 7218  ..backendr....r.
+000009b0: 0000 0072 1900 0000 da0b 6765 745f 6261  ...r......get_ba
+000009c0: 636b 656e 643e 0000 0073 0a00 0000 0005  ckend>...s......
+000009d0: 0602 0801 0c01 0a02 7a18 4261 7365 4b65  ........z.BaseKe
+000009e0: 7963 6c6f 616b 2e67 6574 5f62 6163 6b65  ycloak.get_backe
+000009f0: 6e64 4e29 0772 1a00 0000 721b 0000 0072  ndN).r....r....r
+00000a00: 1c00 0000 da07 5f5f 646f 635f 5f72 3600  ......__doc__r6.
+00000a10: 0000 720a 0000 0072 3d00 0000 7218 0000  ..r....r=...r...
+00000a20: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00000a30: 721e 0000 001e 0000 0073 0600 0000 0801  r........s......
+00000a40: 0404 081b 721e 0000 0029 01da 096d 6574  ....r....)...met
+00000a50: 6163 6c61 7373 6300 0000 0000 0000 0000  aclassc.........
+00000a60: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
+00000a70: 3200 0000 6500 5a01 6400 5a02 6401 5a03  2...e.Z.d.Z.d.Z.
+00000a80: 6402 6403 9c01 6404 6405 8404 5a04 6505  d.d...d.d...Z.e.
+00000a90: 6506 6507 1900 6406 9c02 6407 6408 8404  e.e...d...d.d...
+00000aa0: 5a08 6402 5300 2909 da13 4765 7455 7365  Z.d.S.)...GetUse
+00000ab0: 724b 6579 636c 6f61 6b49 6e66 6f7a 2547  rKeycloakInfoz%G
+00000ac0: 6574 2074 6865 2075 7365 7220 6174 7472  et the user attr
+00000ad0: 6962 7574 6573 2066 726f 6d20 6b65 7963  ibutes from keyc
+00000ae0: 6c6f 616b 4e72 3700 0000 6301 0000 0000  loakNr7...c.....
+00000af0: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+00000b00: 0000 0073 0c00 0000 7400 8300 7c00 5f01  ...s....t...|._.
+00000b10: 6400 5300 720f 0000 00a9 0272 1e00 0000  d.S.r......r....
+00000b20: da04 6261 7365 7234 0000 0072 1800 0000  ..baser4...r....
+00000b30: 7218 0000 0072 1900 0000 7236 0000 004e  r....r....r6...N
+00000b40: 0000 0073 0200 0000 0001 7a1c 4765 7455  ...s......z.GetU
+00000b50: 7365 724b 6579 636c 6f61 6b49 6e66 6f2e  serKeycloakInfo.
+00000b60: 5f5f 696e 6974 5f5f a902 da05 656d 6169  __init__....emai
+00000b70: 6c72 3800 0000 6302 0000 0000 0000 0000  lr8...c.........
+00000b80: 0000 0005 0000 0003 0000 0043 0000 0073  ...........C...s
+00000b90: 4800 0000 7c00 6a00 6a01 a002 a100 0100  H...|.j.j.......
+00000ba0: 7c00 6a00 6a01 a003 7c01 a101 7d02 7c02  |.j.j...|...}.|.
+00000bb0: 6401 7500 7236 6402 7c01 9b00 6403 9d03  d.u.r6d.|...d...
+00000bc0: 7d03 7404 7c03 8301 8201 7c00 6a00 6a01  }.t.|.....|.j.j.
+00000bd0: a005 7c02 a101 7d04 7c04 5300 2904 7afd  ..|...}.|.S.).z.
+00000be0: 4765 7473 2061 6c6c 2074 6865 2075 7365  Gets all the use
+00000bf0: 7220 6174 7472 6962 7574 6573 2066 726f  r attributes fro
+00000c00: 6d20 6b65 7963 6c6f 616b 0a20 2020 2020  m keycloak.     
+00000c10: 2020 200a 2020 2020 2020 2020 3a70 6172     .        :par
+00000c20: 616d 2065 6d61 696c 3a20 5573 6572 2065  am email: User e
+00000c30: 6d61 696c 0a20 2020 2020 2020 202e 2e2e  mail.        ...
+00000c40: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00000c50: 3a20 5573 6572 2061 7474 7269 6275 7465  : User attribute
+00000c60: 7320 6469 6374 206f 7220 4e6f 6e65 0a20  s dict or None. 
+00000c70: 2020 2020 2020 203a 7274 7970 653a 2064         :rtype: d
+00000c80: 6963 7420 6f72 204e 6f6e 650a 2020 2020  ict or None.    
+00000c90: 2020 2020 3a72 6169 7365 733a 2053 7573      :raises: Sus
+00000ca0: 7069 6369 6f75 734f 7065 7261 7469 6f6e  piciousOperation
+00000cb0: 2069 6620 7573 6572 2064 6f65 7320 6e6f   if user does no
+00000cc0: 7420 6578 6973 7473 206f 6e20 6b65 7963  t exists on keyc
+00000cd0: 6c6f 616b 0a20 2020 2020 2020 204e 7a09  loak.        Nz.
+00000ce0: 5468 6520 7573 6572 207a 1c20 646f 6573  The user z. does
+00000cf0: 206e 6f74 2065 7869 7374 7320 6f6e 206b   not exists on k
+00000d00: 6579 636c 6f61 6b29 0672 4200 0000 7232  eycloak).rB...r2
+00000d10: 0000 00da 0d72 6566 7265 7368 5f74 6f6b  .....refresh_tok
+00000d20: 656e da0b 6765 745f 7573 6572 5f69 6472  en..get_user_idr
+00000d30: 0600 0000 da08 6765 745f 7573 6572 2905  ......get_user).
+00000d40: 7235 0000 0072 4400 0000 da10 7573 6572  r5...rD.....user
+00000d50: 5f69 645f 6b65 7963 6c6f 616b da07 6d65  _id_keycloak..me
+00000d60: 7373 6167 65da 0975 7365 725f 696e 666f  ssage..user_info
+00000d70: 7218 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
+00000d80: 1200 0000 5100 0000 730e 0000 0000 090c  ....Q...s.......
+00000d90: 010e 0208 010c 0108 020e 027a 1c47 6574  ...........z.Get
+00000da0: 5573 6572 4b65 7963 6c6f 616b 496e 666f  UserKeycloakInfo
+00000db0: 2e5f 5f63 616c 6c5f 5f29 0972 1a00 0000  .__call__).r....
+00000dc0: 721b 0000 0072 1c00 0000 723e 0000 0072  r....r....r>...r
+00000dd0: 3600 0000 da03 7374 7272 0300 0000 da04  6.....strr......
+00000de0: 6469 6374 7212 0000 0072 1800 0000 7218  dictr....r....r.
+00000df0: 0000 0072 1800 0000 7219 0000 0072 4000  ...r....r....r@.
+00000e00: 0000 4c00 0000 7306 0000 0008 0104 010e  ..L...s.........
+00000e10: 0372 4000 0000 6300 0000 0000 0000 0000  .r@...c.........
+00000e20: 0000 0000 0000 000c 0000 0040 0000 0073  ...........@...s
+00000e30: 5200 0000 6500 5a01 6400 5a02 6401 5a03  R...e.Z.d.Z.d.Z.
+00000e40: 6402 6403 9c01 6404 6405 8404 5a04 6406  d.d...d.d...Z.d.
+00000e50: 6406 6407 6408 6408 6409 6407 6505 8300  d.d.d.d.d.d.e...
+00000e60: 6608 6506 6506 6506 6507 6507 6507 6508  f.e.e.e.e.e.e.e.
+00000e70: 6507 6505 6509 640a 9c0a 640b 640c 8405  e.e.e.d...d.d...
+00000e80: 5a0a 6402 5300 290d da0a 5570 6461 7465  Z.d.S.)...Update
+00000e90: 5573 6572 7a36 5570 6461 7465 7320 616e  Userz6Updates an
+00000ea0: 2075 7365 7220 696e 2062 6f74 6820 7369   user in both si
+00000eb0: 6465 7320 284b 6579 636c 6f61 6b20 616e  des (Keycloak an
+00000ec0: 6420 6261 636b 656e 6473 292e 4e72 3700  d backends).Nr7.
+00000ed0: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
+00000ee0: 0000 0002 0000 0043 0000 0073 0c00 0000  .......C...s....
+00000ef0: 7400 8300 7c00 5f01 6400 5300 720f 0000  t...|._.d.S.r...
+00000f00: 0072 4100 0000 7234 0000 0072 1800 0000  .rA...r4...r....
+00000f10: 7218 0000 0072 1900 0000 7236 0000 0068  r....r....r6...h
+00000f20: 0000 0073 0200 0000 0001 7a13 5570 6461  ...s......z.Upda
+00000f30: 7465 5573 6572 2e5f 5f69 6e69 745f 5f72  teUser.__init__r
+00000f40: 2000 0000 5446 e902 0000 0029 0a72 4400   ...TF.....).rD.
+00000f50: 0000 da0a 6669 7273 745f 6e61 6d65 da09  ....first_name..
+00000f60: 6c61 7374 5f6e 616d 65da 0765 6e61 626c  last_name..enabl
+00000f70: 6564 da08 6973 5f73 7461 6666 da0c 6973  ed..is_staff..is
+00000f80: 5f73 7570 6572 7573 6572 da0c 6d61 785f  _superuser..max_
+00000f90: 7365 7373 696f 6e73 da11 7570 6461 7465  sessions..update
+00000fa0: 5f61 7474 7269 6275 7465 73da 1163 7573  _attributes..cus
+00000fb0: 746f 6d5f 6174 7472 6962 7574 6573 7238  tom_attributesr8
+00000fc0: 0000 0063 0a00 0000 0000 0000 0000 0000  ...c............
+00000fd0: 1100 0000 0400 0000 4300 0000 7302 0100  ........C...s...
+00000fe0: 007c 006a 006a 01a0 02a1 0001 007c 006a  .|.j.j.......|.j
+00000ff0: 006a 01a0 037c 01a1 017d 0a7c 0a64 0175  .j...|...}.|.d.u
+00001000: 0072 2e64 027d 0b74 047c 0b83 0182 017c  .r.d.}.t.|.....|
+00001010: 027c 037c 0464 039c 037d 0c7c 0872 607c  .|.|.d...}.|.r`|
+00001020: 057c 067c 0764 049c 037c 0c64 053c 007c  .|.|.d...|.d.<.|
+00001030: 0972 607c 0c64 0519 00a0 057c 09a1 0101  .r`|.d.....|....
+00001040: 007c 006a 006a 016a 067c 0a7c 0c64 068d  .|.j.j.j.|.|.d..
+00001050: 0201 007c 006a 006a 01a0 077c 0aa1 017d  ...|.j.j...|...}
+00001060: 0d7c 006a 00a0 08a1 007d 0e7c 0ea0 097c  .|.j.....}.|...|
+00001070: 0da1 017d 0f7c 0f73 a464 077d 0b74 047c  ...}.|.s.d.}.t.|
+00001080: 0b83 0182 017c 0ea0 0a7c 0da1 017d 107c  .....|...|...}.|
+00001090: 027c 0d64 083c 007c 037c 0d64 093c 007c  .|.d.<.|.|.d.<.|
+000010a0: 047c 0d64 0a3c 007c 057c 0d64 0b3c 007c  .|.d.<.|.|.d.<.|
+000010b0: 067c 0d64 0c3c 0074 0b7c 1083 0164 0d6b  .|.d.<.t.|...d.k
+000010c0: 0272 f27c 0ea0 067c 1064 0e19 007c 0da1  .r.|...|.d...|..
+000010d0: 0253 0064 0f7d 0b74 047c 0b83 0182 0164  .S.d.}.t.|.....d
+000010e0: 0153 0029 1061 e502 0000 5570 6461 7465  .S.).a....Update
+000010f0: 7320 616e 2075 7365 7220 696e 2062 6163  s an user in bac
+00001100: 6b65 6e64 2061 6e64 206b 6579 636c 6f61  kend and keycloa
+00001110: 6b20 746f 206b 6565 7020 7468 6520 6461  k to keep the da
+00001120: 7461 2063 6f6e 7369 7374 656e 6379 0a20  ta consistency. 
+00001130: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00001140: 3a70 6172 616d 2065 6d61 696c 3a20 5573  :param email: Us
+00001150: 6572 2065 6d61 696c 2074 6861 7420 7765  er email that we
+00001160: 2077 616e 7420 746f 2075 7064 6174 650a   want to update.
+00001170: 2020 2020 2020 2020 3a70 6172 616d 2066          :param f
+00001180: 6972 7374 5f6e 616d 653a 204e 6577 2066  irst_name: New f
+00001190: 6972 7374 206e 616d 652e 2044 6566 6175  irst name. Defau
+000011a0: 6c74 3d27 270a 2020 2020 2020 2020 3a70  lt=''.        :p
+000011b0: 6172 616d 206c 6173 745f 6e61 6d65 3a20  aram last_name: 
+000011c0: 4e65 7720 6c61 7374 206e 616d 652e 2044  New last name. D
+000011d0: 6566 6175 6c74 3d27 270a 2020 2020 2020  efault=''.      
+000011e0: 2020 3a70 6172 616d 2065 6e61 626c 6564    :param enabled
+000011f0: 3a20 5472 7565 2069 6620 7468 6520 7573  : True if the us
+00001200: 6572 2069 7320 656e 6162 6c65 6420 2861  er is enabled (a
+00001210: 6374 6976 6529 2e20 4465 6661 756c 743d  ctive). Default=
+00001220: 5472 7565 0a20 2020 2020 2020 203a 7061  True.        :pa
+00001230: 7261 6d20 6973 5f73 7461 6666 3a20 4966  ram is_staff: If
+00001240: 2054 7275 652c 2073 6574 7320 6973 5f73   True, sets is_s
+00001250: 7461 6666 2074 6f20 5472 7565 2e20 4465  taff to True. De
+00001260: 6661 756c 743d 4661 6c73 650a 2020 2020  fault=False.    
+00001270: 2020 2020 3a70 6172 616d 2069 735f 7375      :param is_su
+00001280: 7065 7275 7365 723a 2049 6620 5472 7565  peruser: If True
+00001290: 2c20 7365 7473 2069 735f 7375 7065 7275  , sets is_superu
+000012a0: 7365 7220 746f 2054 7275 652e 2044 6566  ser to True. Def
+000012b0: 6175 6c74 3d46 616c 7365 0a20 2020 2020  ault=False.     
+000012c0: 2020 203a 7061 7261 6d20 6d61 785f 7365     :param max_se
+000012d0: 7373 696f 6e73 3a20 4d61 7820 7365 7373  ssions: Max sess
+000012e0: 696f 6e73 2061 6c6c 6f77 6564 2074 6f20  ions allowed to 
+000012f0: 7468 6973 2075 7365 722e 2044 6566 6175  this user. Defau
+00001300: 6c74 3d32 0a20 2020 2020 2020 203a 7061  lt=2.        :pa
+00001310: 7261 6d20 7570 6461 7465 5f61 7474 7269  ram update_attri
+00001320: 6275 7465 733a 2055 7064 6174 6573 2074  butes: Updates t
+00001330: 6865 2069 735f 7374 6166 662c 2069 735f  he is_staff, is_
+00001340: 7375 7065 7275 7365 7220 616e 6420 6d61  superuser and ma
+00001350: 785f 7365 7373 696f 6e20 6f6e 206b 6579  x_session on key
+00001360: 636c 6f61 6b0a 2020 2020 2020 2020 6966  cloak.        if
+00001370: 2069 7320 5472 7565 2e20 4465 6661 756c   is True. Defaul
+00001380: 743a 2054 7275 650a 2020 2020 2020 2020  t: True.        
+00001390: 2e2e 2e0a 2020 2020 2020 2020 3a72 6574  ....        :ret
+000013a0: 7572 6e3a 2043 7265 6174 6564 2075 7365  urn: Created use
+000013b0: 720a 2020 2020 2020 2020 3a72 7479 7065  r.        :rtype
+000013c0: 3a20 5573 6572 0a20 2020 2020 2020 204e  : User.        N
+000013d0: 7a24 5468 6174 2075 7365 7220 646f 6573  z$That user does
+000013e0: 6e27 7420 6578 6973 7473 2069 6e20 6b65  n't exists in ke
+000013f0: 7963 6c6f 616b 2903 da09 6669 7273 744e  ycloak)...firstN
+00001400: 616d 65da 086c 6173 744e 616d 6572 5100  ame..lastNamerQ.
+00001410: 0000 a903 7252 0000 0072 5300 0000 7254  ....rR...rS...rT
+00001420: 0000 00da 0a61 7474 7269 6275 7465 73a9  .....attributes.
+00001430: 02da 0775 7365 725f 6964 da07 7061 796c  ...user_id..payl
+00001440: 6f61 64fa 1a43 6c61 696d 7320 7665 7269  oad..Claims veri
+00001450: 6669 6361 7469 6f6e 2066 6169 6c65 64da  fication failed.
+00001460: 0a67 6976 656e 5f6e 616d 65da 0b66 616d  .given_name..fam
+00001470: 696c 795f 6e61 6d65 da09 6973 5f61 6374  ily_name..is_act
+00001480: 6976 6572 5200 0000 7253 0000 00e9 0100  iverR...rS......
+00001490: 0000 7201 0000 007a 4343 616e 6e6f 7420  ..r....zCCannot 
+000014a0: 7570 6461 7465 2074 6865 2075 7365 722e  update the user.
+000014b0: 2055 7365 7273 2072 6574 7572 6e65 6420   Users returned 
+000014c0: 7a65 726f 206f 7220 6d6f 7265 2074 6861  zero or more tha
+000014d0: 6e20 6f6e 6520 656e 7472 792e 290c 7242  n one entry.).rB
+000014e0: 0000 0072 3200 0000 7245 0000 0072 4600  ...r2...rE...rF.
+000014f0: 0000 7206 0000 00da 0675 7064 6174 65da  ..r......update.
+00001500: 0b75 7064 6174 655f 7573 6572 7247 0000  .update_userrG..
+00001510: 0072 3d00 0000 da0d 7665 7269 6679 5f63  .r=.....verify_c
+00001520: 6c61 696d 73da 1666 696c 7465 725f 7573  laims..filter_us
+00001530: 6572 735f 6279 5f63 6c61 696d 73da 036c  ers_by_claims..l
+00001540: 656e 2911 7235 0000 0072 4400 0000 724f  en).r5...rD...rO
+00001550: 0000 0072 5000 0000 7251 0000 0072 5200  ...rP...rQ...rR.
+00001560: 0000 7253 0000 0072 5400 0000 7255 0000  ..rS...rT...rU..
+00001570: 0072 5600 0000 7248 0000 0072 4900 0000  .rV...rH...rI...
+00001580: 725d 0000 0072 4a00 0000 723c 0000 00da  r]...rJ...r<....
+00001590: 0f63 6c61 696d 735f 7665 7269 6669 6564  .claims_verified
+000015a0: da05 7573 6572 7372 1800 0000 7218 0000  ..usersr....r...
+000015b0: 0072 1900 0000 7212 0000 006b 0000 0073  .r....r....k...s
+000015c0: 4800 0000 001b 0c01 0e02 0801 0401 0803  H...............
+000015d0: 0201 0201 02fd 0606 0402 0201 0201 02fd  ................
+000015e0: 0a06 0401 0e02 0801 0201 02fe 0605 0e02  ................
+000015f0: 0a01 0a02 0401 0401 0802 0a02 0801 0801  ................
+00001600: 0801 0801 0802 0c01 1002 0401 7a13 5570  ............z.Up
+00001610: 6461 7465 5573 6572 2e5f 5f63 616c 6c5f  dateUser.__call_
+00001620: 5f29 0b72 1a00 0000 721b 0000 0072 1c00  _).r....r....r..
+00001630: 0000 723e 0000 0072 3600 0000 724c 0000  ..r>...r6...rL..
+00001640: 0072 4b00 0000 da04 626f 6f6c da03 696e  .rK.....bool..in
+00001650: 74da 0455 7365 7272 1200 0000 7218 0000  t..Userr....r...
+00001660: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00001670: 724d 0000 0066 0000 0073 2c00 0000 0801  rM...f...s,.....
+00001680: 0401 0e06 0201 0201 0201 0201 0201 0201  ................
+00001690: 0201 04f6 0202 0201 0201 0201 0201 0201  ................
+000016a0: 0201 0201 0201 0201 02f5 724d 0000 0063  ..........rM...c
+000016b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000016c0: 1000 0000 4000 0000 739c 0000 0065 005a  ....@...s....e.Z
+000016d0: 0164 005a 0264 0164 029c 0164 0364 0484  .d.Z.d.d...d.d..
+000016e0: 045a 0364 0564 0564 0664 0764 0164 0664  .Z.d.d.d.d.d.d.d
+000016f0: 0764 0764 0764 0865 0483 0064 0766 0c65  .d.d.d.e...d.f.e
+00001700: 0565 0665 0519 0065 0665 0519 0065 0665  .e.e...e.e...e.e
+00001710: 0719 0065 0665 0719 0065 0665 0519 0065  ...e.e...e.e...e
+00001720: 0665 0719 0065 0665 0719 0065 0665 0719  .e...e.e...e.e..
+00001730: 0065 0665 0719 0065 0665 0819 0065 0665  .e.e...e.e...e.e
+00001740: 0419 0065 0665 0719 0065 0964 099c 0e64  ...e.e...e.d...d
+00001750: 0a64 0b84 055a 0a65 0464 0c9c 0164 0d64  .d...Z.e.d...d.d
+00001760: 0e84 045a 0b64 0153 0029 0fda 0a43 7265  ...Z.d.S.)...Cre
+00001770: 6174 6555 7365 724e 7237 0000 0063 0100  ateUserNr7...c..
+00001780: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00001790: 0000 4300 0000 730c 0000 0074 0083 007c  ..C...s....t...|
+000017a0: 005f 0164 0053 0072 0f00 0000 7241 0000  ._.d.S.r....rA..
+000017b0: 0072 3400 0000 7218 0000 0072 1800 0000  .r4...r....r....
+000017c0: 7219 0000 0072 3600 0000 bb00 0000 7302  r....r6.......s.
+000017d0: 0000 0000 017a 1343 7265 6174 6555 7365  .....z.CreateUse
+000017e0: 722e 5f5f 696e 6974 5f5f 7220 0000 0054  r.__init__r ...T
+000017f0: 4672 4e00 0000 290e 7244 0000 0072 4f00  FrN...).rD...rO.
+00001800: 0000 7250 0000 0072 5100 0000 da0e 656d  ..rP...rQ.....em
+00001810: 6169 6c5f 7665 7269 6669 6564 7229 0000  ail_verifiedr)..
+00001820: 00da 1274 656d 706f 7261 7279 5f70 6173  ...temporary_pas
+00001830: 7377 6f72 6472 5200 0000 7253 0000 00da  swordrR...rS....
+00001840: 1273 656e 645f 656d 6169 6c5f 746f 5f75  .send_email_to_u
+00001850: 7365 7272 5400 0000 7256 0000 00da 1075  serrT...rV.....u
+00001860: 7365 5f63 6163 6865 645f 746f 6b65 6e72  se_cached_tokenr
+00001870: 3800 0000 630e 0000 0000 0000 0000 0000  8...c...........
+00001880: 0019 0000 000c 0000 004b 0000 0073 5402  .........K...sT.
+00001890: 0000 7c0d 7230 6401 7d0f 7400 a001 7c0f  ..|.r0d.}.t...|.
+000018a0: a101 733c 7c00 6a02 6a03 a004 a100 0100  ..s<|.j.j.......
+000018b0: 7400 6a05 7c0f 6402 6403 6404 8d03 0100  t.j.|.d.d.d.....
+000018c0: 6e0c 7c00 6a02 6a03 a004 a100 0100 7c00  n.|.j.j.......|.
+000018d0: 6a02 6a03 a006 7c01 a101 7d10 7c10 6405  j.j...|...}.|.d.
+000018e0: 7500 9001 7230 7c07 7266 7407 6a08 6a09  u...r0|.rft.j.j.
+000018f0: 6406 6407 8d01 7d06 6408 6409 6901 7d11  d.d...}.d.d.i.}.
+00001900: 7c0e a001 640a a101 72da 7c0e a001 640b  |...d...r.|...d.
+00001910: a101 72da 7c0e 640b 1900 a001 640c 640d  ..r.|.d.....d.d.
+00001920: a102 7d12 7c12 a00a a100 7d12 740b a00c  ..}.|.....}.t...
+00001930: 7c12 a101 a00d a100 7c0e 640b 1900 640c  |.......|.d...d.
+00001940: 3c00 740e a00f 7c0e a001 640a a101 a101  <.t...|...d.....
+00001950: 7c11 640e 3c00 740e a00f 7c0e a001 640b  |.d.<.t...|...d.
+00001960: a101 a101 7c11 640f 3c00 6e0c 7410 7c06  ....|.d.<.n.t.|.
+00001970: 8301 7c11 6410 3c00 7c07 7c11 6411 3c00  ..|.d.<.|.|.d.<.
+00001980: 7c08 7c09 7c0b 6412 9c03 7d13 7c0c 9001  |.|.|.d...}.|...
+00001990: 720a 7c13 a011 7c0c a101 0100 7c00 6a02  r.|...|.....|.j.
+000019a0: 6a03 a012 7c01 7c01 7c02 7c03 7c04 7c05  j...|.|.|.|.|.|.
+000019b0: 7c11 6701 6413 6701 7c13 6414 9c09 a101  |.g.d.g.|.d.....
+000019c0: 7d10 7c00 6a02 6a03 a013 7c10 a101 7d14  }.|.j.j...|...}.
+000019d0: 7c00 a014 7c14 a101 0100 7c14 a001 6415  |...|.....|...d.
+000019e0: a101 7d01 7c00 6a02 a015 a100 7d15 7c15  ..}.|.j.....}.|.
+000019f0: a016 7c14 a101 7d16 7c16 9001 7378 6416  ..|...}.|...sxd.
+00001a00: 7d17 7417 7c17 8301 8201 7c15 a018 7c14  }.t.|.....|...|.
+00001a10: a101 7d18 7c02 7c14 6417 3c00 7c03 7c14  ..}.|.|.d.<.|.|.
+00001a20: 6418 3c00 7c04 7c14 6419 3c00 7c08 7c14  d.<.|.|.d.<.|.|.
+00001a30: 641a 3c00 7c09 7c14 641b 3c00 7419 7c18  d.<.|.|.d.<.t.|.
+00001a40: 8301 641c 6b02 9001 72c8 7c15 a01a 7c18  ..d.k...r.|...|.
+00001a50: 641d 1900 7c14 a102 5300 7419 7c18 8301  d...|...S.t.|...
+00001a60: 641c 6b04 9001 72e4 641e 7d17 7417 7c17  d.k...r.d.}.t.|.
+00001a70: 8301 8201 6e6c 7c15 a01b 641f 6402 a102  ....nl|...d.d...
+00001a80: 9002 7250 7c0a 9002 7246 7c10 9002 7346  ..rP|...rF|...sF
+00001a90: 7a30 741c 6a1d 7c01 741e 6a1f 741e 6a20  z0t.j.|.t.j.t.j 
+00001aa0: 741e 6a21 741e 6a22 7c02 7c03 7c01 7410  t.j!t.j"|.|.|.t.
+00001ab0: 7c06 8301 6420 9c04 6421 8d06 0100 5700  |...d ..d!....W.
+00001ac0: 6e16 0100 0100 0100 7423 a024 6422 a101  n.......t#.$d"..
+00001ad0: 0100 5900 6e02 3000 7c15 a012 7c14 a101  ..Y.n.0.|...|...
+00001ae0: 5300 6405 5300 2923 6121 0400 0043 7265  S.d.S.)#a!...Cre
+00001af0: 6174 6573 2061 6e20 7573 6572 2069 6e20  ates an user in 
+00001b00: 6261 636b 656e 6420 616e 6420 6b65 7963  backend and keyc
+00001b10: 6c6f 616b 2073 6572 7665 720a 0a20 2020  loak server..   
+00001b20: 2020 2020 203a 7061 7261 6d20 656d 6169       :param emai
+00001b30: 6c3a 2055 7365 7220 656d 6169 6c20 7468  l: User email th
+00001b40: 6174 2077 6520 7761 6e74 2074 6f20 6372  at we want to cr
+00001b50: 6561 7465 0a20 2020 2020 2020 203a 7061  eate.        :pa
+00001b60: 7261 6d20 6669 7273 745f 6e61 6d65 3a20  ram first_name: 
+00001b70: 4e65 7720 6669 7273 7420 6e61 6d65 2e20  New first name. 
+00001b80: 4465 6661 756c 743d 2727 0a20 2020 2020  Default=''.     
+00001b90: 2020 203a 7061 7261 6d20 6c61 7374 5f6e     :param last_n
+00001ba0: 616d 653a 204e 6577 206c 6173 7420 6e61  ame: New last na
+00001bb0: 6d65 2e20 4465 6661 756c 743d 2727 0a20  me. Default=''. 
+00001bc0: 2020 2020 2020 203a 7061 7261 6d20 656e         :param en
+00001bd0: 6162 6c65 643a 2054 7275 6520 6966 2074  abled: True if t
+00001be0: 6865 2075 7365 7220 6973 2065 6e61 626c  he user is enabl
+00001bf0: 6564 2028 6163 7469 7665 292e 2044 6566  ed (active). Def
+00001c00: 6175 6c74 3d54 7275 650a 2020 2020 2020  ault=True.      
+00001c10: 2020 3a70 6172 616d 2065 6d61 696c 5f76    :param email_v
+00001c20: 6572 6966 6965 643a 2054 7275 6520 6966  erified: True if
+00001c30: 2074 6865 2075 7365 7220 656d 6169 6c20   the user email 
+00001c40: 6973 2076 6572 6966 6965 642e 2044 6566  is verified. Def
+00001c50: 6175 6c74 3d46 616c 7365 0a20 2020 2020  ault=False.     
+00001c60: 2020 203a 7061 7261 6d20 7061 7373 776f     :param passwo
+00001c70: 7264 3a20 5573 6572 2070 6173 7377 6f72  rd: User passwor
+00001c80: 642e 2044 6566 6175 6c74 3d4e 6f6e 650a  d. Default=None.
+00001c90: 2020 2020 2020 2020 3a70 6172 616d 2074          :param t
+00001ca0: 656d 706f 7261 7279 5f70 6173 7377 6f72  emporary_passwor
+00001cb0: 643a 2049 6620 7472 7565 2073 6574 7320  d: If true sets 
+00001cc0: 6120 7465 6d70 6f72 6172 7920 7061 7373  a temporary pass
+00001cd0: 776f 7264 2074 6f20 7573 6572 2e20 4465  word to user. De
+00001ce0: 6661 756c 743d 5472 7565 0a20 2020 2020  fault=True.     
+00001cf0: 2020 203a 7061 7261 6d20 6973 5f73 7461     :param is_sta
+00001d00: 6666 3a20 4966 2054 7275 652c 2073 6574  ff: If True, set
+00001d10: 7320 6973 5f73 7461 6666 2074 6f20 5472  s is_staff to Tr
+00001d20: 7565 2e20 4465 6661 756c 743d 4661 6c73  ue. Default=Fals
+00001d30: 650a 2020 2020 2020 2020 3a70 6172 616d  e.        :param
+00001d40: 2069 735f 7375 7065 7275 7365 723a 2049   is_superuser: I
+00001d50: 6620 5472 7565 2c20 7365 7473 2069 735f  f True, sets is_
+00001d60: 7375 7065 7275 7365 7220 746f 2054 7275  superuser to Tru
+00001d70: 652e 2044 6566 6175 6c74 3d46 616c 7365  e. Default=False
+00001d80: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00001d90: 7365 6e64 5f65 6d61 696c 5f74 6f5f 7573  send_email_to_us
+00001da0: 6572 3a20 4966 2074 7275 652c 2073 656e  er: If true, sen
+00001db0: 6473 2061 6e20 656d 6169 6c20 746f 2074  ds an email to t
+00001dc0: 6865 2075 7365 7220 6e6f 7469 6679 696e  he user notifyin
+00001dd0: 6720 7468 6174 2074 6865 0a20 2020 2020  g that the.     
+00001de0: 2020 2061 6363 6f75 6e74 2077 6173 2063     account was c
+00001df0: 7265 6174 6564 2e20 4465 6661 756c 743a  reated. Default:
+00001e00: 2046 616c 7365 0a20 2020 2020 2020 203a   False.        :
+00001e10: 7061 7261 6d20 6d61 785f 7365 7373 696f  param max_sessio
+00001e20: 6e73 3a20 4d61 7820 7365 7373 696f 6e73  ns: Max sessions
+00001e30: 2061 6c6c 6f77 6564 2074 6f20 7468 6973   allowed to this
+00001e40: 2075 7365 722e 2044 6566 6175 6c74 3d32   user. Default=2
+00001e50: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00001e60: 7573 655f 6361 6368 6564 5f74 6f6b 656e  use_cached_token
+00001e70: 3a20 4966 2074 7275 652c 2077 696c 6c20  : If true, will 
+00001e80: 6e6f 7420 7265 6672 6573 6820 7468 6520  not refresh the 
+00001e90: 746f 6b65 6e20 756e 7469 6c20 7468 6520  token until the 
+00001ea0: 6361 6368 6520 6578 7069 7265 732e 0a20  cache expires.. 
+00001eb0: 2020 2020 2020 2044 6566 6179 756c 743a         Defayult:
+00001ec0: 2046 616c 7365 0a20 2020 2020 2020 202e   False.        .
+00001ed0: 2e2e 0a20 2020 2020 2020 203a 7265 7475  ...        :retu
+00001ee0: 726e 3a20 4372 6561 7465 6420 7573 6572  rn: Created user
+00001ef0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00001f00: 2055 7365 720a 2020 2020 2020 2020 5a14   User.        Z.
+00001f10: 6b65 7963 6c6f 616b 5f61 646d 696e 5f74  keycloak_admin_t
+00001f20: 6f6b 656e 5469 5802 0000 2901 da07 7469  okenTiX...)...ti
+00001f30: 6d65 6f75 744e e90e 0000 00a9 01da 066c  meoutN.........l
+00001f40: 656e 6774 68da 0474 7970 6572 2900 0000  ength..typer)...
+00001f50: 5a0f 6372 6564 656e 7469 616c 5f64 6174  Z.credential_dat
+00001f60: 615a 0b73 6563 7265 745f 6461 7461 da04  aZ.secret_data..
+00001f70: 7361 6c74 7220 0000 005a 0e63 7265 6465  saltr ...Z.crede
+00001f80: 6e74 6961 6c44 6174 615a 0a73 6563 7265  ntialDataZ.secre
+00001f90: 7444 6174 61da 0576 616c 7565 da09 7465  tData..value..te
+00001fa0: 6d70 6f72 6172 7972 5900 0000 5a0c 7573  mporaryrY...Z.us
+00001fb0: 6572 5f64 6566 6175 6c74 2909 7244 0000  er_default).rD..
+00001fc0: 0072 2800 0000 7257 0000 0072 5800 0000  .r(...rW...rX...
+00001fd0: 7251 0000 005a 0d65 6d61 696c 5665 7269  rQ...Z.emailVeri
+00001fe0: 6669 6564 da0b 6372 6564 656e 7469 616c  fied..credential
+00001ff0: 735a 0a72 6561 6c6d 526f 6c65 7372 5a00  sZ.realmRolesrZ.
+00002000: 0000 7244 0000 0072 5e00 0000 725f 0000  ..rD...r^...r_..
+00002010: 0072 6000 0000 7261 0000 0072 5200 0000  .r`...ra...rR...
+00002020: 7253 0000 0072 6200 0000 7201 0000 007a  rS...rb...r....z
+00002030: 174d 756c 7469 706c 6520 7573 6572 7320  .Multiple users 
+00002040: 7265 7475 726e 6564 5a10 4f49 4443 5f43  returnedZ.OIDC_C
+00002050: 5245 4154 455f 5553 4552 2904 724f 0000  REATE_USER).rO..
+00002060: 0072 5000 0000 7244 0000 00da 0e70 6c61  .rP...rD.....pla
+00002070: 696e 5f70 6173 7377 6f72 64a9 0672 4400  in_password..rD.
+00002080: 0000 da0a 6672 6f6d 5f65 6d61 696c da0d  ....from_email..
+00002090: 7465 6d70 6c61 7465 5f75 7569 64da 1062  template_uuid..b
+000020a0: 7261 6e64 5f67 726f 7570 5f75 7569 64da  rand_group_uuid.
+000020b0: 0773 7562 6a65 6374 da07 636f 6e74 6578  .subject..contex
+000020c0: 747a 1d43 616e 6e6f 7420 7365 6e64 2063  tz.Cannot send c
+000020d0: 7265 6174 6520 7573 6572 2065 6d61 696c  reate user email
+000020e0: 2925 7208 0000 00da 0367 6574 7242 0000  )%r......getrB..
+000020f0: 0072 3200 0000 7245 0000 00da 0373 6574  .r2...rE.....set
+00002100: 7246 0000 0072 6c00 0000 da07 6f62 6a65  rF...rl.....obje
+00002110: 6374 73da 146d 616b 655f 7261 6e64 6f6d  cts..make_random
+00002120: 5f70 6173 7377 6f72 64da 0665 6e63 6f64  _password..encod
+00002130: 65da 0662 6173 6536 34da 0962 3634 656e  e..base64..b64en
+00002140: 636f 6465 da06 6465 636f 6465 da04 6a73  code..decode..js
+00002150: 6f6e da05 6475 6d70 7372 4b00 0000 7263  on..dumpsrK...rc
+00002160: 0000 00da 0b63 7265 6174 655f 7573 6572  .....create_user
+00002170: 7247 0000 00da 136e 6f72 6d61 6c69 7a65  rG.....normalize
+00002180: 5f75 7365 725f 696e 666f 723d 0000 0072  _user_infor=...r
+00002190: 6500 0000 7206 0000 0072 6600 0000 7267  e...r....rf...rg
+000021a0: 0000 0072 6400 0000 5a0c 6765 745f 7365  ...rd...Z.get_se
+000021b0: 7474 696e 6773 720d 0000 00da 0a73 656e  ttingsr......sen
+000021c0: 645f 656d 6169 6c72 0900 0000 da12 4445  d_emailr......DE
+000021d0: 4641 554c 545f 4652 4f4d 5f45 4d41 494c  FAULT_FROM_EMAIL
+000021e0: da24 454d 4149 4c5f 5445 4d50 4c41 5445  .$EMAIL_TEMPLATE
+000021f0: 5f52 4553 4554 5f4c 4f47 494e 5f49 4e46  _RESET_LOGIN_INF
+00002200: 4f5f 5555 4944 da16 454d 4149 4c5f 4252  O_UUID..EMAIL_BR
+00002210: 414e 445f 4752 4f55 505f 5555 4944 da1b  AND_GROUP_UUID..
+00002220: 454d 4149 4c5f 5553 4552 5f43 5245 4154  EMAIL_USER_CREAT
+00002230: 494f 4e5f 5355 424a 4543 5472 2f00 0000  ION_SUBJECTr/...
+00002240: da09 6578 6365 7074 696f 6e29 1972 3500  ..exception).r5.
+00002250: 0000 7244 0000 0072 4f00 0000 7250 0000  ..rD...rO...rP..
+00002260: 0072 5100 0000 726e 0000 0072 2900 0000  .rQ...rn...r)...
+00002270: 726f 0000 0072 5200 0000 7253 0000 0072  ro...rR...rS...r
+00002280: 7000 0000 7254 0000 0072 5600 0000 7271  p...rT...rV...rq
+00002290: 0000 0072 1500 0000 da03 6b65 7972 4800  ...r......keyrH.
+000022a0: 0000 727a 0000 0072 7700 0000 725a 0000  ..rz...rw...rZ..
+000022b0: 0072 4a00 0000 723c 0000 0072 6800 0000  .rJ...r<...rh...
+000022c0: da03 6d73 6772 6900 0000 7218 0000 0072  ..msgri...r....r
+000022d0: 1800 0000 7219 0000 0072 1200 0000 be00  ....r....r......
+000022e0: 0000 7398 0000 0000 2504 0104 020a 010c  ..s.....%.......
+000022f0: 0112 030c 020e 020a 0104 010e 0304 ff04  ................
+00002300: 0414 0110 0108 0116 0114 0116 020c 0208  ................
+00002310: 0302 0102 0102 fd06 0606 010a 0208 0202  ................
+00002320: 0102 0102 0102 0102 0102 0104 0104 0102  ................
+00002330: f704 ff04 0e0e 010a 020a 020a 010a 0106  ................
+00002340: 0104 0108 030a 0208 0108 0108 0108 0108  ................
+00002350: 020e 0110 010e 0304 010a 010e 010c 0102  ................
+00002360: 0104 0102 0104 0104 0104 0104 0202 0102  ................
+00002370: 0102 0106 fc04 fa0a 0d06 0110 020a 027a  ...............z
+00002380: 1343 7265 6174 6555 7365 722e 5f5f 6361  .CreateUser.__ca
+00002390: 6c6c 5f5f 2901 724a 0000 0063 0200 0000  ll__).rJ...c....
+000023a0: 0000 0000 0000 0000 0600 0000 0b00 0000  ................
+000023b0: 4300 0000 7398 0000 007c 01a0 0064 0169  C...s....|...d.i
+000023c0: 00a1 027d 027c 0244 005d 787d 0374 017c  ...}.|.D.]x}.t.|
+000023d0: 027c 0319 0074 0283 0272 1074 037c 027c  .|...t...r.t.|.|
+000023e0: 0319 0083 0164 026b 0272 3e7c 027c 0319  .....d.k.r>|.|..
+000023f0: 0064 0319 006e 067c 027c 0319 007d 047a  .d...n.|.|...}.z
+00002400: 1474 0474 057c 0483 0183 017c 027c 033c  .t.t.|.....|.|.<
+00002410: 0057 0071 1004 0074 0679 8601 007d 0501  .W.q...t.y...}..
+00002420: 007a 147c 047c 027c 033c 0057 0059 0064  .z.|.|.|.<.W.Y.d
+00002430: 047d 057e 0571 1064 047d 057e 0530 0030  .}.~.q.d.}.~.0.0
+00002440: 0071 107c 01a0 077c 02a1 0101 0064 0453  .q.|...|.....d.S
+00002450: 0029 057a 2a4e 6f72 6d61 6c69 7a65 7320  .).z*Normalizes 
+00002460: 7468 6520 7573 6572 2069 6e66 6f72 6d61  the user informa
+00002470: 7469 6f6e 2064 6963 7469 6f6e 6172 7972  tion dictionaryr
+00002480: 5a00 0000 7262 0000 0072 0100 0000 4e29  Z...rb...r....N)
+00002490: 0872 8200 0000 da0a 6973 696e 7374 616e  .r......isinstan
+000024a0: 6365 da04 6c69 7374 7267 0000 0072 6a00  ce..listrg...rj.
+000024b0: 0000 7202 0000 0072 3a00 0000 7263 0000  ..r....r:...rc..
+000024c0: 0029 0672 3500 0000 724a 0000 0072 5a00  .).r5...rJ...rZ.
+000024d0: 0000 7294 0000 0072 7800 0000 da01 6572  ..r....rx.....er
+000024e0: 1800 0000 7218 0000 0072 1900 0000 728d  ....r....r....r.
+000024f0: 0000 004b 0100 0073 1200 0000 0002 0c02  ...K...s........
+00002500: 0801 0e01 2401 0201 1401 0e01 2002 7a1e  ....$....... .z.
+00002510: 4372 6561 7465 5573 6572 2e6e 6f72 6d61  CreateUser.norma
+00002520: 6c69 7a65 5f75 7365 725f 696e 666f 290c  lize_user_info).
+00002530: 721a 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
+00002540: 3600 0000 724c 0000 0072 4b00 0000 7203  6...rL...rK...r.
+00002550: 0000 0072 6a00 0000 726b 0000 0072 6c00  ...rj...rk...rl.
+00002560: 0000 7212 0000 0072 8d00 0000 7218 0000  ..r....r....r...
+00002570: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00002580: 726d 0000 00ba 0000 0073 3e00 0000 0801  rm.......s>.....
+00002590: 0e06 0201 0201 0201 0201 0201 0201 0201  ................
+000025a0: 0201 0201 0201 0401 02f2 0202 0201 0601  ................
+000025b0: 0601 0601 0601 0601 0601 0601 0601 0601  ................
+000025c0: 0601 0601 0602 02f0 0c7f 000e 726d 0000  ............rm..
+000025d0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+000025e0: 0000 0700 0000 4000 0000 7336 0000 0065  ......@...s6...e
+000025f0: 005a 0164 005a 0264 0164 029c 0164 0364  .Z.d.Z.d.d...d.d
+00002600: 0484 045a 0364 0965 0465 0565 0419 0065  ...Z.d.e.e.e...e
+00002610: 0665 0665 0764 069c 0564 0764 0884 055a  .e.e.d...d.d...Z
+00002620: 0864 0153 0029 0ada 0e55 7064 6174 6550  .d.S.)...UpdateP
+00002630: 6173 7377 6f72 644e 7237 0000 0063 0100  asswordNr7...c..
+00002640: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00002650: 0000 4300 0000 730c 0000 0074 0083 007c  ..C...s....t...|
+00002660: 005f 0164 0053 0072 0f00 0000 7241 0000  ._.d.S.r....rA..
+00002670: 0072 3400 0000 7218 0000 0072 1800 0000  .r4...r....r....
+00002680: 7219 0000 0072 3600 0000 5b01 0000 7302  r....r6...[...s.
+00002690: 0000 0000 017a 1755 7064 6174 6550 6173  .....z.UpdatePas
+000026a0: 7377 6f72 642e 5f5f 696e 6974 5f5f 4629  sword.__init__F)
+000026b0: 0572 4400 0000 7229 0000 0072 7900 0000  .rD...r)...ry...
+000026c0: 7270 0000 0072 3800 0000 6305 0000 0000  rp...r8...c.....
+000026d0: 0000 0000 0000 0009 0000 000a 0000 004b  ...............K
+000026e0: 0000 0073 e800 0000 7c00 6a00 6a01 a002  ...s....|.j.j...
+000026f0: a100 0100 6401 7d06 6402 6403 6404 6405  ....d.}.d.d.d.d.
+00002700: 9c03 7d07 7a12 7c00 6a00 6a01 a003 7c01  ..}.z.|.j.j...|.
+00002710: a101 7d08 5700 6e36 0100 0100 0100 6406  ..}.W.n6......d.
+00002720: 7c07 6407 3c00 6408 7c07 6409 3c00 640a  |.d.<.d.|.d.<.d.
+00002730: 7c07 640b 3c00 640c 7d06 7404 7c07 640d  |.d.<.d.}.t.|.d.
+00002740: 7c06 640e 8d03 0600 5900 5300 3000 7c03  |.d.....Y.S.0.|.
+00002750: 7278 7405 6a06 6a07 640f 6410 8d01 7d02  rxt.j.j.d.d...}.
+00002760: 7c00 6a00 6a01 6a08 7c08 7c02 7c03 6411  |.j.j.j.|.|.|.d.
+00002770: 8d03 0100 7c04 72da 7a32 7409 6a0a 7c01  ....|.r.z2t.j.|.
+00002780: 740b 6a0c 740b 6a0d 740b 6a0e 740b 6a0f  t.j.t.j.t.j.t.j.
+00002790: 7c05 a010 6412 6404 a102 7c01 7c02 6413  |...d.d...|.|.d.
+000027a0: 9c03 6414 8d06 0100 5700 6e16 0100 0100  ..d.....W.n.....
+000027b0: 0100 7411 a012 6415 a101 0100 5900 6e02  ..t...d.....Y.n.
+000027c0: 3000 7404 7c07 640d 7c06 640e 8d03 5300  0.t.|.d.|.d...S.
+000027d0: 2916 612c 0200 0055 7064 6174 6573 2061  ).a,...Updates a
+000027e0: 6e20 7573 6572 2070 6173 7377 6f72 6420  n user password 
+000027f0: 6f6e 206b 6579 636c 6f61 6b0a 2020 2020  on keycloak.    
+00002800: 2020 2020 0a20 2020 2020 2020 203a 7061      .        :pa
+00002810: 7261 6d20 656d 6169 6c3a 2055 7365 7220  ram email: User 
+00002820: 656d 6169 6c20 7468 6174 2077 6520 7761  email that we wa
+00002830: 6e74 2074 6f20 7570 6461 7465 2074 6865  nt to update the
+00002840: 2070 6173 7377 6f72 640a 2020 2020 2020   password.      
+00002850: 2020 3a70 6172 616d 2070 6173 7377 6f72    :param passwor
+00002860: 643a 204e 6577 2070 6173 7377 6f72 642e  d: New password.
+00002870: 2049 6620 4e6f 6e65 2c20 7465 6d70 6f72   If None, tempor
+00002880: 6172 7920 6e65 6564 2074 6f20 6265 2054  ary need to be T
+00002890: 7275 652e 2044 6566 6175 6c74 3d4e 6f6e  rue. Default=Non
+000028a0: 650a 2020 2020 2020 2020 3a70 6172 616d  e.        :param
+000028b0: 2074 656d 706f 7261 7279 3a20 4966 2054   temporary: If T
+000028c0: 7275 6520 7468 6520 7573 6572 2077 696c  rue the user wil
+000028d0: 6c20 6861 7665 2061 2074 656d 706f 7261  l have a tempora
+000028e0: 7279 2070 6173 7377 6f72 642e 2044 6566  ry password. Def
+000028f0: 6175 6c74 3d46 616c 7365 0a20 2020 2020  ault=False.     
+00002900: 2020 203a 7061 7261 6d20 7365 6e64 5f65     :param send_e
+00002910: 6d61 696c 5f74 6f5f 7573 6572 3a20 5365  mail_to_user: Se
+00002920: 6e64 7320 616e 2065 6d61 696c 2074 6f20  nds an email to 
+00002930: 7468 6520 7573 6572 206e 6f74 6966 7969  the user notifyi
+00002940: 6e67 2074 6865 206e 6577 2070 6173 7377  ng the new passw
+00002950: 6f72 642e 0a20 2020 2020 2020 2044 6566  ord..        Def
+00002960: 6175 6c74 3a20 4661 6c73 650a 2020 2020  ault: False.    
+00002970: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
+00002980: 3a72 6574 7572 6e3a 207b 2772 6573 756c  :return: {'resul
+00002990: 7427 3a20 274f 4b2f 4b4f 272c 2027 7265  t': 'OK/KO', 're
+000029a0: 6173 6f6e 273a 2027 272c 2027 6d65 7373  ason': '', 'mess
+000029b0: 6167 6527 3a20 2727 7d20 2832 3030 2069  age': ''} (200 i
+000029c0: 6620 4f4b 2c20 3530 3020 6966 206b 6579  f OK, 500 if key
+000029d0: 636c 6f61 6b20 6572 726f 7229 0a20 2020  cloak error).   
+000029e0: 2020 2020 203a 7265 7479 7065 3a20 4a73       :retype: Js
+000029f0: 6f6e 5265 7370 6f6e 7365 0a20 2020 2020  onResponse.     
+00002a00: 2020 20e9 c800 0000 da02 4f4b da07 5355     .......OK..SU
+00002a10: 4343 4553 5372 2000 0000 a903 da06 7265  CCESSr .......re
+00002a20: 7375 6c74 da06 7265 6173 6f6e 7249 0000  sult..reasonrI..
+00002a30: 00da 024b 4f72 9e00 0000 da05 4552 524f  ...KOr......ERRO
+00002a40: 5272 9f00 0000 7a25 4572 726f 7220 7472  Rr....z%Error tr
+00002a50: 7969 6e67 2074 6f20 6669 6e64 2075 7365  ying to find use
+00002a60: 7220 696e 206b 6579 636c 6f61 6b72 4900  r in keycloakrI.
+00002a70: 0000 e9f4 0100 0046 a903 da04 6461 7461  .......F....data
+00002a80: da04 7361 6665 da06 7374 6174 7573 7273  ..safe..statusrs
+00002a90: 0000 0072 7400 0000 2903 725c 0000 0072  ...rt...).r\...r
+00002aa0: 2900 0000 7279 0000 00da 046e 616d 6529  )...ry.....name)
+00002ab0: 0372 a700 0000 7244 0000 0072 7b00 0000  .r....rD...r{...
+00002ac0: 727c 0000 007a 2143 616e 6e6f 7420 7365  r|...z!Cannot se
+00002ad0: 6e64 2075 7064 6174 6520 7061 7373 776f  nd update passwo
+00002ae0: 7264 2065 6d61 696c 2913 7242 0000 0072  rd email).rB...r
+00002af0: 3200 0000 7245 0000 0072 4600 0000 7207  2...rE...rF...r.
+00002b00: 0000 0072 6c00 0000 7284 0000 0072 8500  ...rl...r....r..
+00002b10: 0000 5a11 7365 745f 7573 6572 5f70 6173  ..Z.set_user_pas
+00002b20: 7377 6f72 6472 0d00 0000 728e 0000 0072  swordr....r....r
+00002b30: 0900 0000 728f 0000 0072 9000 0000 7291  ....r....r....r.
+00002b40: 0000 00da 2845 4d41 494c 5f55 5345 525f  ....(EMAIL_USER_
+00002b50: 5041 5353 574f 5244 5f4e 4f54 4946 4943  PASSWORD_NOTIFIC
+00002b60: 4154 494f 4e5f 5355 424a 4543 5472 8200  ATION_SUBJECTr..
+00002b70: 0000 722f 0000 0072 9300 0000 2909 7235  ..r/...r....).r5
+00002b80: 0000 0072 4400 0000 7229 0000 0072 7900  ...rD...r)...ry.
+00002b90: 0000 7270 0000 0072 1500 0000 72a6 0000  ..rp...r....r...
+00002ba0: 0072 a400 0000 7248 0000 0072 1800 0000  .r....rH...r....
+00002bb0: 7218 0000 0072 1900 0000 7212 0000 005e  r....r....r....^
+00002bc0: 0100 0073 4400 0000 0013 0c01 0401 0c02  ...sD...........
+00002bd0: 0201 1201 0601 0801 0801 0801 0401 1402  ................
+00002be0: 0401 0e02 0801 0201 0201 02fd 0606 0401  ................
+00002bf0: 0201 0401 0201 0401 0401 0401 0402 0a01  ................
+00002c00: 0201 02fd 04fa 0a0c 0601 1002 7a17 5570  ............z.Up
+00002c10: 6461 7465 5061 7373 776f 7264 2e5f 5f63  datePassword.__c
+00002c20: 616c 6c5f 5f29 034e 4646 2909 721a 0000  all__).NFF).r...
+00002c30: 0072 1b00 0000 721c 0000 0072 3600 0000  .r....r....r6...
+00002c40: 724b 0000 0072 0300 0000 726a 0000 0072  rK...r....rj...r
+00002c50: 0700 0000 7212 0000 0072 1800 0000 7218  ....r....r....r.
+00002c60: 0000 0072 1800 0000 7219 0000 0072 9900  ...r....r....r..
+00002c70: 0000 5a01 0000 7316 0000 0008 010e 0600  ..Z...s.........
+00002c80: 0100 0100 fb02 0202 0106 0102 0102 0202  ................
+00002c90: f972 9900 0000 6300 0000 0000 0000 0000  .r....c.........
+00002ca0: 0000 0000 0000 0004 0000 0040 0000 0073  ...........@...s
+00002cb0: 3400 0000 6500 5a01 6400 5a02 6401 6402  4...e.Z.d.Z.d.d.
+00002cc0: 9c01 6403 6404 8404 5a03 6405 6406 8400  ..d.d...Z.d.d...
+00002cd0: 5a04 6505 6505 6506 6407 9c03 6408 6409  Z.e.e.e.d...d.d.
+00002ce0: 8404 5a07 6401 5300 290a da11 5365 6e64  ..Z.d.S.)...Send
+00002cf0: 5570 6461 7465 4163 636f 756e 744e 7237  UpdateAccountNr7
+00002d00: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00002d10: 0100 0000 0200 0000 4300 0000 730c 0000  ........C...s...
+00002d20: 0074 0083 007c 005f 0164 0053 0072 0f00  .t...|._.d.S.r..
+00002d30: 0000 7241 0000 0072 3400 0000 7218 0000  ..rA...r4...r...
+00002d40: 0072 1800 0000 7219 0000 0072 3600 0000  .r....r....r6...
+00002d50: 9c01 0000 7302 0000 0000 017a 1a53 656e  ....s......z.Sen
+00002d60: 6455 7064 6174 6541 6363 6f75 6e74 2e5f  dUpdateAccount._
+00002d70: 5f69 6e69 745f 5f63 0200 0000 0000 0000  _init__c........
+00002d80: 0000 0000 0300 0000 0300 0000 4300 0000  ............C...
+00002d90: 7310 0000 0064 017d 0274 007c 017c 0276  s....d.}.t.|.|.v
+00002da0: 0083 0153 0029 024e 2901 5a0f 5550 4441  ...S.).N).Z.UPDA
+00002db0: 5445 5f50 4153 5357 4f52 4429 0172 6a00  TE_PASSWORD).rj.
+00002dc0: 0000 2903 7235 0000 00da 0661 6374 696f  ..).r5.....actio
+00002dd0: 6eda 0761 6374 696f 6e73 7218 0000 0072  n..actionsr....r
+00002de0: 1800 0000 7219 0000 00da 0e5f 6163 7469  ....r......_acti
+00002df0: 6f6e 5f65 7869 7374 739f 0100 0073 0400  on_exists....s..
+00002e00: 0000 0001 0401 7a20 5365 6e64 5570 6461  ......z SendUpda
+00002e10: 7465 4163 636f 756e 742e 5f61 6374 696f  teAccount._actio
+00002e20: 6e5f 6578 6973 7473 2903 7244 0000 0072  n_exists).rD...r
+00002e30: aa00 0000 7238 0000 0063 0300 0000 0000  ....r8...c......
+00002e40: 0000 0000 0000 0600 0000 0600 0000 4300  ..............C.
+00002e50: 0000 73a0 0000 0064 017d 0364 0264 0364  ..s....d.}.d.d.d
+00002e60: 0464 059c 037d 047c 00a0 007c 02a1 0173  .d...}.|...|...s
+00002e70: 2664 067c 0464 073c 0064 087d 037a 487c  &d.|.d.<.d.}.zH|
+00002e80: 006a 016a 02a0 03a1 0001 007c 006a 016a  .j.j.......|.j.j
+00002e90: 02a0 047c 01a1 017d 057c 006a 016a 026a  ...|...}.|.j.j.j
+00002ea0: 057c 0574 06a0 077c 0267 01a1 0164 098d  .|.t...|.g...d..
+00002eb0: 0201 0064 0a7c 0464 0b3c 0064 0c7c 0464  ...d.|.d.<.d.|.d
+00002ec0: 0d3c 0057 006e 2201 0001 0001 0064 0e7d  .<.W.n"......d.}
+00002ed0: 0374 08a0 0964 0fa1 0101 0064 107c 0464  .t...d.....d.|.d
+00002ee0: 073c 0059 006e 0230 0074 0a7c 0464 117c  .<.Y.n.0.t.|.d.|
+00002ef0: 0364 128d 0353 0029 134e 729a 0000 0072  .d...S.).Nr....r
+00002f00: a000 0000 72a1 0000 0072 2000 0000 729d  ....r....r ...r.
+00002f10: 0000 007a 2354 6865 2070 726f 7669 6465  ...z#The provide
+00002f20: 6420 6163 7469 6f6e 2064 6f65 736e 2774  d action doesn't
+00002f30: 2065 7869 7374 732e 7249 0000 0069 9001   exists.rI...i..
+00002f40: 0000 725b 0000 0072 9b00 0000 729e 0000  ..r[...r....r...
+00002f50: 0072 9c00 0000 729f 0000 0072 a200 0000  .r....r....r....
+00002f60: 7a3d 4572 726f 7220 6f6e 2055 7064 6174  z=Error on Updat
+00002f70: 6541 6363 6f75 6e74 2073 6572 7669 6365  eAccount service
+00002f80: 2028 646e 6f74 6963 6961 735f 7365 7276   (dnoticias_serv
+00002f90: 6963 6520 3e20 6b65 7963 6c6f 616b 297a  ice > keycloak)z
+00002fa0: 2b41 6e20 6572 726f 7220 6861 7320 6265  +An error has be
+00002fb0: 656e 206f 6375 7272 6564 206f 6e20 7570  en ocurred on up
+00002fc0: 6461 7465 2061 6363 6f75 6e74 4672 a300  date accountFr..
+00002fd0: 0000 290b 72ac 0000 0072 4200 0000 7232  ..).r....rB...r2
+00002fe0: 0000 0072 4500 0000 7246 0000 00da 1373  ...rE...rF.....s
+00002ff0: 656e 645f 7570 6461 7465 5f61 6363 6f75  end_update_accou
+00003000: 6e74 728a 0000 0072 8b00 0000 722f 0000  ntr....r....r/..
+00003010: 0072 9300 0000 7207 0000 0029 0672 3500  .r....r....).r5.
+00003020: 0000 7244 0000 0072 aa00 0000 72a6 0000  ..rD...r....r...
+00003030: 0072 a400 0000 725c 0000 0072 1800 0000  .r....r\...r....
+00003040: 7218 0000 0072 1900 0000 7212 0000 00a3  r....r....r.....
+00003050: 0100 0073 2600 0000 0001 0401 0c02 0a01  ...s&...........
+00003060: 0801 0402 0201 0c01 0e01 0801 0201 0afe  ................
+00003070: 0604 0801 0c01 0601 0401 0a01 0e02 7a1a  ..............z.
+00003080: 5365 6e64 5570 6461 7465 4163 636f 756e  SendUpdateAccoun
+00003090: 742e 5f5f 6361 6c6c 5f5f 2908 721a 0000  t.__call__).r...
+000030a0: 0072 1b00 0000 721c 0000 0072 3600 0000  .r....r....r6...
+000030b0: 72ac 0000 0072 4b00 0000 7207 0000 0072  r....rK...r....r
+000030c0: 1200 0000 7218 0000 0072 1800 0000 7218  ....r....r....r.
+000030d0: 0000 0072 1900 0000 72a9 0000 009b 0100  ...r....r.......
+000030e0: 0073 0600 0000 0801 0e03 0804 72a9 0000  .s..........r...
+000030f0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00003100: 0000 0400 0000 4000 0000 732c 0000 0065  ......@...s,...e
+00003110: 005a 0164 005a 0264 0164 029c 0164 0364  .Z.d.Z.d.d...d.d
+00003120: 0484 045a 0365 0465 0465 0564 059c 0364  ...Z.e.e.e.d...d
+00003130: 0664 0784 045a 0664 0153 0029 08da 0847  .d...Z.d.S.)...G
+00003140: 6574 546f 6b65 6e4e 7237 0000 0063 0100  etTokenNr7...c..
+00003150: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00003160: 0000 4300 0000 730c 0000 0074 0083 007c  ..C...s....t...|
+00003170: 005f 0164 0053 0072 0f00 0000 7241 0000  ._.d.S.r....rA..
+00003180: 0072 3400 0000 7218 0000 0072 1800 0000  .r4...r....r....
+00003190: 7219 0000 0072 3600 0000 bd01 0000 7302  r....r6.......s.
+000031a0: 0000 0000 017a 1147 6574 546f 6b65 6e2e  .....z.GetToken.
+000031b0: 5f5f 696e 6974 5f5f 2903 7244 0000 0072  __init__).rD...r
+000031c0: 2900 0000 7238 0000 0063 0300 0000 0000  )...r8...c......
+000031d0: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
+000031e0: 0000 7310 0000 007c 006a 006a 01a0 027c  ..s....|.j.j...|
+000031f0: 017c 02a1 0253 0029 017a e547 6574 2074  .|...S.).z.Get t
+00003200: 6865 2075 7365 7220 746f 6b65 6e20 616e  he user token an
+00003210: 6420 6372 6561 7465 7320 6120 6e65 7720  d creates a new 
+00003220: 7365 7373 696f 6e20 6f6e 206b 6579 636c  session on keycl
+00003230: 6f61 6b0a 2020 2020 2020 2020 0a20 2020  oak.        .   
+00003240: 2020 2020 203a 7061 7261 6d20 656d 6169       :param emai
+00003250: 6c3a 2055 7365 7220 656d 6169 6c0a 2020  l: User email.  
+00003260: 2020 2020 2020 3a70 6172 616d 2070 6173        :param pas
+00003270: 7377 6f72 643a 2055 7365 7220 7061 7373  sword: User pass
+00003280: 776f 7264 0a20 2020 2020 2020 202e 2e2e  word.        ...
+00003290: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+000032a0: 3a20 4163 6365 7373 2074 6f6b 656e 2c20  : Access token, 
+000032b0: 7265 6672 6573 6820 746f 6b65 6e20 6469  refresh token di
+000032c0: 6374 0a20 2020 2020 2020 203a 7274 7970  ct.        :rtyp
+000032d0: 653a 2064 6963 740a 2020 2020 2020 2020  e: dict.        
+000032e0: 2903 7242 0000 0072 3300 0000 da05 746f  ).rB...r3.....to
+000032f0: 6b65 6e29 0372 3500 0000 7244 0000 0072  ken).r5...rD...r
+00003300: 2900 0000 7218 0000 0072 1800 0000 7219  )...r....r....r.
+00003310: 0000 0072 1200 0000 c001 0000 7302 0000  ...r........s...
+00003320: 0000 097a 1147 6574 546f 6b65 6e2e 5f5f  ...z.GetToken.__
+00003330: 6361 6c6c 5f5f a907 721a 0000 0072 1b00  call__..r....r..
+00003340: 0000 721c 0000 0072 3600 0000 724b 0000  ..r....r6...rK..
+00003350: 0072 4c00 0000 7212 0000 0072 1800 0000  .rL...r....r....
+00003360: 7218 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
+00003370: ae00 0000 bc01 0000 7304 0000 0008 010e  ........s.......
+00003380: 0372 ae00 0000 6300 0000 0000 0000 0000  .r....c.........
+00003390: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
+000033a0: 2a00 0000 6500 5a01 6400 5a02 6401 6402  *...e.Z.d.Z.d.d.
+000033b0: 9c01 6403 6404 8404 5a03 6504 6505 6405  ..d.d...Z.e.e.d.
+000033c0: 9c02 6406 6407 8404 5a06 6401 5300 2908  ..d.d...Z.d.S.).
+000033d0: da0c 5265 6672 6573 6854 6f6b 656e 4e72  ..RefreshTokenNr
+000033e0: 3700 0000 6301 0000 0000 0000 0000 0000  7...c...........
+000033f0: 0001 0000 0002 0000 0043 0000 0073 0c00  .........C...s..
+00003400: 0000 7400 8300 7c00 5f01 6400 5300 720f  ..t...|._.d.S.r.
+00003410: 0000 0072 4100 0000 7234 0000 0072 1800  ...rA...r4...r..
+00003420: 0000 7218 0000 0072 1900 0000 7236 0000  ..r....r....r6..
+00003430: 00cd 0100 0073 0200 0000 0001 7a15 5265  .....s......z.Re
+00003440: 6672 6573 6854 6f6b 656e 2e5f 5f69 6e69  freshToken.__ini
+00003450: 745f 5fa9 0272 4500 0000 7238 0000 0063  t__..rE...r8...c
+00003460: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00003470: 0300 0000 4300 0000 730e 0000 007c 006a  ....C...s....|.j
+00003480: 006a 01a0 027c 01a1 0153 0029 017a f952  .j...|...S.).z.R
+00003490: 6566 7265 7368 2074 6865 2074 6f6b 656e  efresh the token
+000034a0: 206f 6e20 6b65 7963 6c6f 616b 2061 6e64   on keycloak and
+000034b0: 2072 6574 7572 6e73 2074 6865 206e 6577   returns the new
+000034c0: 2067 656e 6572 6174 6564 2074 6f6b 656e   generated token
+000034d0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000034e0: 2020 3a70 6172 616d 2072 6566 7265 7368    :param refresh
+000034f0: 5f74 6f6b 656e 3a20 5265 6672 6573 6820  _token: Refresh 
+00003500: 746f 6b65 6e20 7573 6564 2074 6f20 6765  token used to ge
+00003510: 6e65 7261 7465 2061 206e 6577 2061 6363  nerate a new acc
+00003520: 6573 735f 746f 6b65 6e0a 2020 2020 2020  ess_token.      
+00003530: 2020 2e2e 2e0a 2020 2020 2020 2020 3a72    ....        :r
+00003540: 6574 7572 6e3a 2041 6363 6573 7320 546f  eturn: Access To
+00003550: 6b65 6e20 616e 6420 5265 6672 6573 6820  ken and Refresh 
+00003560: 546f 6b65 6e20 6469 6374 0a20 2020 2020  Token dict.     
+00003570: 2020 203a 7274 7970 653a 2064 6963 740a     :rtype: dict.
+00003580: 2020 2020 2020 2020 2903 7242 0000 0072          ).rB...r
+00003590: 3300 0000 7245 0000 00a9 0272 3500 0000  3...rE.....r5...
+000035a0: 7245 0000 0072 1800 0000 7218 0000 0072  rE...r....r....r
+000035b0: 1900 0000 7212 0000 00d0 0100 0073 0200  ....r........s..
+000035c0: 0000 0008 7a15 5265 6672 6573 6854 6f6b  ....z.RefreshTok
+000035d0: 656e 2e5f 5f63 616c 6c5f 5f72 b000 0000  en.__call__r....
+000035e0: 7218 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
+000035f0: 1900 0000 72b1 0000 00cc 0100 0073 0400  ....r........s..
+00003600: 0000 0801 0e03 72b1 0000 0063 0000 0000  ......r....c....
+00003610: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00003620: 4000 0000 732a 0000 0065 005a 0164 005a  @...s*...e.Z.d.Z
+00003630: 0264 0164 029c 0164 0364 0484 045a 0365  .d.d...d.d...Z.e
+00003640: 0465 0564 059c 0264 0664 0784 045a 0664  .e.d...d.d...Z.d
+00003650: 0153 0029 08da 0a4c 6f67 6f75 7455 7365  .S.)...LogoutUse
+00003660: 724e 7237 0000 0063 0100 0000 0000 0000  rNr7...c........
+00003670: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+00003680: 730c 0000 0074 0083 007c 005f 0164 0053  s....t...|._.d.S
+00003690: 0072 0f00 0000 7241 0000 0072 3400 0000  .r....rA...r4...
+000036a0: 7218 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
+000036b0: 3600 0000 dc01 0000 7302 0000 0000 017a  6.......s......z
+000036c0: 134c 6f67 6f75 7455 7365 722e 5f5f 696e  .LogoutUser.__in
+000036d0: 6974 5f5f 72b2 0000 0063 0200 0000 0000  it__r....c......
+000036e0: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+000036f0: 0000 730e 0000 007c 006a 006a 01a0 027c  ..s....|.j.j...|
+00003700: 01a1 0153 0029 017a 7f4c 6f67 6f75 7473  ...S.).z.Logouts
 00003710: 2061 6e20 7573 6572 206f 6e20 6b65 7963   an user on keyc
 00003720: 6c6f 616b 2028 6e6f 7420 6261 636b 656e  loak (not backen
 00003730: 6429 0a20 2020 2020 2020 200a 2020 2020  d).        .    
 00003740: 2020 2020 3a70 6172 616d 2072 6566 7265      :param refre
 00003750: 7368 5f74 6f6b 656e 3a20 5265 6672 6573  sh_token: Refres
 00003760: 6820 746f 6b65 6e20 7573 6564 2074 6f20  h token used to 
 00003770: 6c6f 676f 7574 2074 6865 2075 7365 720a  logout the user.
-00003780: 2020 2020 2020 2020 4e29 0372 1d00 0000          N).r....
-00003790: 7238 0000 0072 3c00 0000 72b5 0000 0072  r8...r<...r....r
-000037a0: 1200 0000 7212 0000 0072 1700 0000 7251  ....r....r....rQ
-000037b0: 0000 00e2 0100 0073 0600 0000 0805 0a01  .......s........
-000037c0: 24ff 7a13 4c6f 676f 7574 5573 6572 2e5f  $.z.LogoutUser._
-000037d0: 5f63 616c 6c5f 5f4e 72b1 0000 0072 1200  _call__Nr....r..
-000037e0: 0000 7212 0000 0072 1200 0000 7217 0000  ..r....r....r...
-000037f0: 0072 b800 0000 e001 0000 72b7 0000 0072  .r........r....r
-00003800: b800 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00003810: 0000 0000 0004 0000 0040 0000 0072 b200  .........@...r..
-00003820: 0000 2906 da0c 4765 7454 6f6b 656e 496e  ..)...GetTokenIn
-00003830: 666f da0c 6163 6365 7373 5f74 6f6b 656e  fo..access_token
-00003840: 7241 0000 0063 0200 0000 0000 0000 0000  rA...c..........
-00003850: 0000 0300 0000 0800 0000 4300 0000 72b4  ..........C...r.
-00003860: 0000 0029 027a e947 6574 7320 7468 6520  ...).z.Gets the 
-00003870: 746f 6b65 6e20 696e 666f 2066 726f 6d20  token info from 
-00003880: 6b65 7963 6c6f 616b 2028 6163 6365 7373  keycloak (access
-00003890: 2c20 7265 6672 6573 682c 2065 7870 6972  , refresh, expir
-000038a0: 6174 696f 6e2c 2065 7463 290a 2020 2020  ation, etc).    
-000038b0: 2020 2020 0a20 2020 2020 2020 203a 7061      .        :pa
-000038c0: 7261 6d20 6163 6365 7373 5f74 6f6b 656e  ram access_token
-000038d0: 3a20 4163 6365 7373 2074 6f6b 656e 2075  : Access token u
-000038e0: 7365 6420 746f 2072 6574 7269 6576 6520  sed to retrieve 
-000038f0: 7468 6520 746f 6b65 6e20 696e 666f 0a20  the token info. 
-00003900: 2020 2020 2020 202e 2e2e 0a20 2020 2020         ....     
-00003910: 2020 203a 7265 7475 726e 3a20 546f 6b65     :return: Toke
-00003920: 6e20 7573 6572 2069 6e66 6f72 6d61 7469  n user informati
-00003930: 6f6e 0a20 2020 2020 2020 203a 7274 7970  on.        :rtyp
-00003940: 653a 2064 6963 740a 2020 2020 2020 2020  e: dict.        
-00003950: 4e29 0372 1d00 0000 7238 0000 005a 0a69  N).r....r8...Z.i
-00003960: 6e74 726f 7370 6563 7429 0372 1500 0000  ntrospect).r....
-00003970: 72ba 0000 0072 4e00 0000 7212 0000 0072  r....rN...r....r
-00003980: 1200 0000 7217 0000 0072 5100 0000 ed01  ....r....rQ.....
-00003990: 0000 72b6 0000 007a 1547 6574 546f 6b65  ..r....z.GetToke
-000039a0: 6e49 6e66 6f2e 5f5f 6361 6c6c 5f5f 4e72  nInfo.__call__Nr
-000039b0: b100 0000 7212 0000 0072 1200 0000 7212  ....r....r....r.
-000039c0: 0000 0072 1700 0000 72b9 0000 00eb 0100  ...r....r.......
-000039d0: 0072 b700 0000 72b9 0000 0063 0000 0000  .r....r....c....
-000039e0: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-000039f0: 4000 0000 72b2 0000 0029 06da 124b 6579  @...r....)...Key
-00003a00: 636c 6f61 6b55 7365 7245 7869 7374 7372  cloakUserExistsr
-00003a10: 4a00 0000 7241 0000 0063 0200 0000 0000  J...rA...c......
-00003a20: 0000 0000 0000 0300 0000 0800 0000 4300  ..............C.
-00003a30: 0000 7342 0000 007c 0173 0464 0153 0074  ..sB...|.s.d.S.t
-00003a40: 0083 008f 107d 0274 017c 026a 02a0 037c  .....}.t.|.j...|
-00003a50: 01a1 0183 0157 0002 0064 0204 0004 0083  .....W...d......
-00003a60: 0301 0053 0031 0073 1a77 0101 0001 0001  ...S.1.s.w......
-00003a70: 0059 0001 0064 0253 0029 037a d156 6572  .Y...d.S.).z.Ver
-00003a80: 6966 6965 7320 6966 2074 6865 2065 6d61  ifies if the ema
-00003a90: 696c 2067 6976 656e 2065 7869 7374 7320  il given exists 
-00003aa0: 696e 206b 6579 636c 6f61 6b0a 2020 2020  in keycloak.    
-00003ab0: 2020 2020 0a20 2020 2020 2020 203a 7061      .        :pa
-00003ac0: 7261 6d20 656d 6169 6c3a 2045 6d61 696c  ram email: Email
-00003ad0: 2077 6520 7769 6c6c 2063 6865 636b 2069   we will check i
-00003ae0: 6620 6578 6973 7473 0a20 2020 2020 2020  f exists.       
-00003af0: 202e 2e2e 0a20 2020 2020 2020 203a 7265   ....        :re
-00003b00: 7475 726e 3a20 5472 7565 2069 6620 7468  turn: True if th
-00003b10: 6520 656d 6169 6c20 6578 6973 7473 2c20  e email exists, 
-00003b20: 4661 6c73 6520 6974 2064 6f65 736e 2774  False it doesn't
-00003b30: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00003b40: 2062 6f6f 6c0a 2020 2020 2020 2020 464e   bool.        FN
-00003b50: 2904 721d 0000 0072 6f00 0000 7237 0000  ).r....ro...r7..
-00003b60: 0072 4b00 0000 2903 7215 0000 0072 4a00  .rK...).r....rJ.
-00003b70: 0000 724e 0000 0072 1200 0000 7212 0000  ..rN...r....r...
-00003b80: 0072 1700 0000 7251 0000 00fb 0100 0073  .r....rQ.......s
-00003b90: 0a00 0000 0408 0401 0802 0e01 24ff 7a1b  ............$.z.
-00003ba0: 4b65 7963 6c6f 616b 5573 6572 4578 6973  KeycloakUserExis
-00003bb0: 7473 2e5f 5f63 616c 6c5f 5f4e a906 7219  ts.__call__N..r.
-00003bc0: 0000 0072 1a00 0000 721b 0000 0072 1c00  ...r....r....r..
-00003bd0: 0000 726f 0000 0072 5100 0000 7212 0000  ..ro...rQ...r...
-00003be0: 0072 1200 0000 7212 0000 0072 1700 0000  .r....r....r....
-00003bf0: 72bb 0000 00f9 0100 0072 b700 0000 72bb  r........r....r.
-00003c00: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00003c10: 0000 0000 0400 0000 4000 0000 72b2 0000  ........@...r...
-00003c20: 0029 06da 1144 656c 6574 6555 7365 7253  .)...DeleteUserS
-00003c30: 6573 7369 6f6e 7210 0000 0072 4100 0000  essionr....rA...
-00003c40: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-00003c50: 0008 0000 0043 0000 0073 3e00 0000 7c01  .....C...s>...|.
-00003c60: 7304 6401 5300 7400 8300 8f0e 7d02 7c02  s.d.S.t.....}.|.
-00003c70: 6a01 a002 7c01 a101 5700 0200 6402 0400  j...|...W...d...
-00003c80: 0400 8303 0100 5300 3100 7318 7701 0100  ......S.1.s.w...
-00003c90: 0100 0100 5900 0100 6402 5300 2903 7aa6  ....Y...d.S.).z.
-00003ca0: 4465 6c65 7465 7320 616e 2073 7065 6369  Deletes an speci
-00003cb0: 6669 6320 7365 7373 696f 6e20 6964 0a0a  fic session id..
-00003cc0: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
-00003cd0: 6573 7369 6f6e 3a20 5365 7373 696f 6e20  ession: Session 
-00003ce0: 6964 2074 6f20 6465 6c65 7465 0a20 2020  id to delete.   
-00003cf0: 2020 2020 203a 7265 7475 726e 3a20 5472       :return: Tr
-00003d00: 7565 2069 6620 7468 6520 656d 6169 6c20  ue if the email 
-00003d10: 6578 6973 7473 2c20 4661 6c73 6520 6974  exists, False it
-00003d20: 2064 6f65 736e 2774 0a20 2020 2020 2020   doesn't.       
-00003d30: 203a 7274 7970 653a 2062 6f6f 6c0a 2020   :rtype: bool.  
-00003d40: 2020 2020 2020 464e 2903 721d 0000 0072        FN).r....r
-00003d50: 3700 0000 7218 0000 0029 0372 1500 0000  7...r....).r....
-00003d60: 7210 0000 0072 4e00 0000 7212 0000 0072  r....rN...r....r
-00003d70: 1200 0000 7217 0000 0072 5100 0000 0c02  ....r....rQ.....
-00003d80: 0000 730a 0000 0004 0704 0108 020a 0124  ..s............$
-00003d90: ff7a 1a44 656c 6574 6555 7365 7253 6573  .z.DeleteUserSes
-00003da0: 7369 6f6e 2e5f 5f63 616c 6c5f 5f4e 72bc  sion.__call__Nr.
-00003db0: 0000 0072 1200 0000 7212 0000 0072 1200  ...r....r....r..
-00003dc0: 0000 7217 0000 0072 bd00 0000 0a02 0000  ..r....r........
-00003dd0: 72b7 0000 0072 bd00 0000 2936 da07 6c6f  r....r....)6..lo
-00003de0: 6767 696e 6772 8800 0000 728b 0000 005a  ggingr....r....Z
-00003df0: 0e64 6973 7475 7469 6c73 2e75 7469 6c72  .distutils.utilr
-00003e00: 0200 0000 da06 7479 7069 6e67 7203 0000  ......typingr...
-00003e10: 00da 1364 6a61 6e67 6f2e 636f 6e74 7269  ...django.contri
-00003e20: 622e 6175 7468 7204 0000 0072 0500 0000  b.authr....r....
-00003e30: da16 646a 616e 676f 2e63 6f72 652e 6578  ..django.core.ex
-00003e40: 6365 7074 696f 6e73 7206 0000 00da 0b64  ceptionsr......d
-00003e50: 6a61 6e67 6f2e 6874 7470 7207 0000 00da  jango.httpr.....
-00003e60: 0b64 6a61 6e67 6f2e 636f 6e66 7208 0000  .django.confr...
-00003e70: 005a 086b 6579 636c 6f61 6b72 0900 0000  .Z.keycloakr....
-00003e80: 5a11 4261 7365 4b65 7963 6c6f 616b 4164  Z.BaseKeycloakAd
-00003e90: 6d69 6e72 0a00 0000 720b 0000 005a 186d  minr....r....Z.m
-00003ea0: 6f7a 696c 6c61 5f64 6a61 6e67 6f5f 6f69  ozilla_django_oi
-00003eb0: 6463 2e61 7574 6872 0c00 0000 da21 646e  dc.authr.....!dn
-00003ec0: 6f74 6963 6961 735f 7365 7276 6963 6573  oticias_services
-00003ed0: 2e63 6f6d 6d75 6e69 6361 7469 6f6e 7372  .communicationsr
-00003ee0: 0d00 0000 da05 7574 696c 7372 0f00 0000  ......utilsr....
-00003ef0: 7271 0000 00da 0967 6574 4c6f 6767 6572  rq.....getLogger
-00003f00: 7219 0000 0072 2600 0000 721d 0000 0072  r....r&...r....r
-00003f10: 4900 0000 7253 0000 0072 7200 0000 729b  I...rS...rr...r.
-00003f20: 0000 0072 ab00 0000 72b0 0000 0072 b300  ...r....r....r..
-00003f30: 0000 72b8 0000 0072 b900 0000 72bb 0000  ..r....r....r...
-00003f40: 0072 bd00 0000 7269 0000 0072 af00 0000  .r....ri...r....
-00003f50: 728d 0000 00da 0f75 7064 6174 655f 7061  r......update_pa
-00003f60: 7373 776f 7264 da09 6765 745f 746f 6b65  ssword..get_toke
-00003f70: 6e72 3a00 0000 5a0b 6c6f 676f 7574 5f75  nr:...Z.logout_u
-00003f80: 7365 725a 0e67 6574 5f74 6f6b 656e 5f69  serZ.get_token_i
-00003f90: 6e66 6f5a 146b 6579 636c 6f61 6b5f 7573  nfoZ.keycloak_us
-00003fa0: 6572 5f65 7869 7374 735a 1667 6574 5f75  er_existsZ.get_u
-00003fb0: 7365 725f 6b65 7963 6c6f 616b 5f69 6e66  ser_keycloak_inf
-00003fc0: 6f72 1800 0000 7212 0000 0072 1200 0000  or....r....r....
-00003fd0: 7212 0000 0072 1700 0000 da08 3c6d 6f64  r....r......<mod
-00003fe0: 756c 653e 0100 0000 7350 0000 0008 0008  ule>....sP......
-00003ff0: 0108 010c 010c 0110 020c 010c 010c 0114  ................
-00004000: 020c 010c 010c 0206 020a 0110 030e 0f0e  ................
-00004010: 390e 1a0e 5200 7f0e 1c0e 3f0e 1f0e 0f0e  9...R.....?.....
-00004020: 0e0e 0b0e 0e0e 1106 1006 0106 0106 0106  ................
-00004030: 0106 0106 0106 0106 0106 010a 01         .............
+00003780: 2020 2020 2020 2020 2903 7242 0000 0072          ).rB...r
+00003790: 3300 0000 da06 6c6f 676f 7574 72b3 0000  3.....logoutr...
+000037a0: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+000037b0: 7212 0000 00df 0100 0073 0200 0000 0005  r........s......
+000037c0: 7a13 4c6f 676f 7574 5573 6572 2e5f 5f63  z.LogoutUser.__c
+000037d0: 616c 6c5f 5f72 b000 0000 7218 0000 0072  all__r....r....r
+000037e0: 1800 0000 7218 0000 0072 1900 0000 72b4  ....r....r....r.
+000037f0: 0000 00db 0100 0073 0400 0000 0801 0e03  .......s........
+00003800: 72b4 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00003810: 0000 0000 0000 0300 0000 4000 0000 732a  ..........@...s*
+00003820: 0000 0065 005a 0164 005a 0264 0164 029c  ...e.Z.d.Z.d.d..
+00003830: 0164 0364 0484 045a 0365 0465 0564 059c  .d.d...Z.e.e.d..
+00003840: 0264 0664 0784 045a 0664 0153 0029 08da  .d.d...Z.d.S.)..
+00003850: 0c47 6574 546f 6b65 6e49 6e66 6f4e 7237  .GetTokenInfoNr7
+00003860: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00003870: 0100 0000 0200 0000 4300 0000 730c 0000  ........C...s...
+00003880: 0074 0083 007c 005f 0164 0053 0072 0f00  .t...|._.d.S.r..
+00003890: 0000 7241 0000 0072 3400 0000 7218 0000  ..rA...r4...r...
+000038a0: 0072 1800 0000 7219 0000 0072 3600 0000  .r....r....r6...
+000038b0: e801 0000 7302 0000 0000 017a 1547 6574  ....s......z.Get
+000038c0: 546f 6b65 6e49 6e66 6f2e 5f5f 696e 6974  TokenInfo.__init
+000038d0: 5f5f 2902 da0c 6163 6365 7373 5f74 6f6b  __)...access_tok
+000038e0: 656e 7238 0000 0063 0200 0000 0000 0000  enr8...c........
+000038f0: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
+00003900: 730e 0000 007c 006a 006a 01a0 027c 01a1  s....|.j.j...|..
+00003910: 0153 0029 017a e947 6574 7320 7468 6520  .S.).z.Gets the 
+00003920: 746f 6b65 6e20 696e 666f 2066 726f 6d20  token info from 
+00003930: 6b65 7963 6c6f 616b 2028 6163 6365 7373  keycloak (access
+00003940: 2c20 7265 6672 6573 682c 2065 7870 6972  , refresh, expir
+00003950: 6174 696f 6e2c 2065 7463 290a 2020 2020  ation, etc).    
+00003960: 2020 2020 0a20 2020 2020 2020 203a 7061      .        :pa
+00003970: 7261 6d20 6163 6365 7373 5f74 6f6b 656e  ram access_token
+00003980: 3a20 4163 6365 7373 2074 6f6b 656e 2075  : Access token u
+00003990: 7365 6420 746f 2072 6574 7269 6576 6520  sed to retrieve 
+000039a0: 7468 6520 746f 6b65 6e20 696e 666f 0a20  the token info. 
+000039b0: 2020 2020 2020 202e 2e2e 0a20 2020 2020         ....     
+000039c0: 2020 203a 7265 7475 726e 3a20 546f 6b65     :return: Toke
+000039d0: 6e20 7573 6572 2069 6e66 6f72 6d61 7469  n user informati
+000039e0: 6f6e 0a20 2020 2020 2020 203a 7274 7970  on.        :rtyp
+000039f0: 653a 2064 6963 740a 2020 2020 2020 2020  e: dict.        
+00003a00: 2903 7242 0000 0072 3300 0000 5a0a 696e  ).rB...r3...Z.in
+00003a10: 7472 6f73 7065 6374 2902 7235 0000 0072  trospect).r5...r
+00003a20: b700 0000 7218 0000 0072 1800 0000 7219  ....r....r....r.
+00003a30: 0000 0072 1200 0000 eb01 0000 7302 0000  ...r........s...
+00003a40: 0000 087a 1547 6574 546f 6b65 6e49 6e66  ...z.GetTokenInf
+00003a50: 6f2e 5f5f 6361 6c6c 5f5f 72b0 0000 0072  o.__call__r....r
+00003a60: 1800 0000 7218 0000 0072 1800 0000 7219  ....r....r....r.
+00003a70: 0000 0072 b600 0000 e701 0000 7304 0000  ...r........s...
+00003a80: 0008 010e 0372 b600 0000 6300 0000 0000  .....r....c.....
+00003a90: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+00003aa0: 0000 0073 2a00 0000 6500 5a01 6400 5a02  ...s*...e.Z.d.Z.
+00003ab0: 6401 6402 9c01 6403 6404 8404 5a03 6504  d.d...d.d...Z.e.
+00003ac0: 6505 6405 9c02 6406 6407 8404 5a06 6401  e.d...d.d...Z.d.
+00003ad0: 5300 2908 da12 4b65 7963 6c6f 616b 5573  S.)...KeycloakUs
+00003ae0: 6572 4578 6973 7473 4e72 3700 0000 6301  erExistsNr7...c.
+00003af0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+00003b00: 0000 0043 0000 0073 0c00 0000 7400 8300  ...C...s....t...
+00003b10: 7c00 5f01 6400 5300 720f 0000 0072 4100  |._.d.S.r....rA.
+00003b20: 0000 7234 0000 0072 1800 0000 7218 0000  ..r4...r....r...
+00003b30: 0072 1900 0000 7236 0000 00f7 0100 0073  .r....r6.......s
+00003b40: 0200 0000 0001 7a1b 4b65 7963 6c6f 616b  ......z.Keycloak
+00003b50: 5573 6572 4578 6973 7473 2e5f 5f69 6e69  UserExists.__ini
+00003b60: 745f 5f72 4300 0000 6302 0000 0000 0000  t__rC...c.......
+00003b70: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+00003b80: 0073 2600 0000 7c00 6a00 6a01 a002 a100  .s&...|.j.j.....
+00003b90: 0100 7c01 7314 6401 5300 7403 7c00 6a00  ..|.s.d.S.t.|.j.
+00003ba0: 6a01 a004 7c01 a101 8301 5300 2902 7ad1  j...|.....S.).z.
+00003bb0: 5665 7269 6669 6573 2069 6620 7468 6520  Verifies if the 
+00003bc0: 656d 6169 6c20 6769 7665 6e20 6578 6973  email given exis
+00003bd0: 7473 2069 6e20 6b65 7963 6c6f 616b 0a20  ts in keycloak. 
+00003be0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00003bf0: 3a70 6172 616d 2065 6d61 696c 3a20 456d  :param email: Em
+00003c00: 6169 6c20 7765 2077 696c 6c20 6368 6563  ail we will chec
+00003c10: 6b20 6966 2065 7869 7374 730a 2020 2020  k if exists.    
+00003c20: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
+00003c30: 3a72 6574 7572 6e3a 2054 7275 6520 6966  :return: True if
+00003c40: 2074 6865 2065 6d61 696c 2065 7869 7374   the email exist
+00003c50: 732c 2046 616c 7365 2069 7420 646f 6573  s, False it does
+00003c60: 6e27 740a 2020 2020 2020 2020 3a72 7479  n't.        :rty
+00003c70: 7065 3a20 626f 6f6c 0a20 2020 2020 2020  pe: bool.       
+00003c80: 2046 2905 7242 0000 0072 3200 0000 7245   F).rB...r2...rE
+00003c90: 0000 0072 6a00 0000 7246 0000 0029 0272  ...rj...rF...).r
+00003ca0: 3500 0000 7244 0000 0072 1800 0000 7218  5...rD...r....r.
+00003cb0: 0000 0072 1900 0000 7212 0000 00fa 0100  ...r....r.......
+00003cc0: 0073 0800 0000 0008 0c02 0401 0402 7a1b  .s............z.
+00003cd0: 4b65 7963 6c6f 616b 5573 6572 4578 6973  KeycloakUserExis
+00003ce0: 7473 2e5f 5f63 616c 6c5f 5f29 0772 1a00  ts.__call__).r..
+00003cf0: 0000 721b 0000 0072 1c00 0000 7236 0000  ..r....r....r6..
+00003d00: 0072 4b00 0000 726a 0000 0072 1200 0000  .rK...rj...r....
+00003d10: 7218 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
+00003d20: 1900 0000 72b8 0000 00f6 0100 0073 0400  ....r........s..
+00003d30: 0000 0801 0e03 72b8 0000 0029 34da 076c  ......r....)4..l
+00003d40: 6f67 6769 6e67 7287 0000 0072 8a00 0000  oggingr....r....
+00003d50: 5a0e 6469 7374 7574 696c 732e 7574 696c  Z.distutils.util
+00003d60: 7202 0000 00da 0674 7970 696e 6772 0300  r......typingr..
+00003d70: 0000 da13 646a 616e 676f 2e63 6f6e 7472  ....django.contr
+00003d80: 6962 2e61 7574 6872 0400 0000 7205 0000  ib.authr....r...
+00003d90: 00da 1664 6a61 6e67 6f2e 636f 7265 2e65  ...django.core.e
+00003da0: 7863 6570 7469 6f6e 7372 0600 0000 da0b  xceptionsr......
+00003db0: 646a 616e 676f 2e68 7474 7072 0700 0000  django.httpr....
+00003dc0: da11 646a 616e 676f 2e63 6f72 652e 6361  ..django.core.ca
+00003dd0: 6368 6572 0800 0000 da0b 646a 616e 676f  cher......django
+00003de0: 2e63 6f6e 6672 0900 0000 5a18 6d6f 7a69  .confr....Z.mozi
+00003df0: 6c6c 615f 646a 616e 676f 5f6f 6964 632e  lla_django_oidc.
+00003e00: 6175 7468 720a 0000 005a 086b 6579 636c  authr....Z.keycl
+00003e10: 6f61 6b72 0b00 0000 720c 0000 00da 2164  oakr....r.....!d
+00003e20: 6e6f 7469 6369 6173 5f73 6572 7669 6365  noticias_service
+00003e30: 732e 636f 6d6d 756e 6963 6174 696f 6e73  s.communications
+00003e40: 720d 0000 0072 6c00 0000 da09 6765 744c  r....rl.....getL
+00003e50: 6f67 6765 7272 1a00 0000 722f 0000 0072  oggerr....r/...r
+00003e60: 7600 0000 720e 0000 0072 1e00 0000 7240  v...r....r....r@
+00003e70: 0000 0072 4d00 0000 726d 0000 0072 9900  ...rM...rm...r..
+00003e80: 0000 72a9 0000 0072 ae00 0000 72b1 0000  ..r....r....r...
+00003e90: 0072 b400 0000 72b6 0000 0072 b800 0000  .r....r....r....
+00003ea0: 7264 0000 0072 ad00 0000 728c 0000 005a  rd...r....r....Z
+00003eb0: 0f75 7064 6174 655f 7061 7373 776f 7264  .update_password
+00003ec0: da09 6765 745f 746f 6b65 6e72 4500 0000  ..get_tokenrE...
+00003ed0: 5a0b 6c6f 676f 7574 5f75 7365 725a 0e67  Z.logout_userZ.g
+00003ee0: 6574 5f74 6f6b 656e 5f69 6e66 6f5a 146b  et_token_infoZ.k
+00003ef0: 6579 636c 6f61 6b5f 7573 6572 5f65 7869  eycloak_user_exi
+00003f00: 7374 735a 1667 6574 5f75 7365 725f 6b65  stsZ.get_user_ke
+00003f10: 7963 6c6f 616b 5f69 6e66 6f72 1800 0000  ycloak_infor....
+00003f20: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
+00003f30: 083c 6d6f 6475 6c65 3e01 0000 0073 4a00  .<module>....sJ.
+00003f40: 0000 0801 0801 0801 0c01 0c02 1001 0c01  ................
+00003f50: 0c01 0c01 0c02 0c01 1001 0c02 0601 0a03  ................
+00003f60: 1009 122e 0e1a 0e54 0e7f 0021 0e41 0e21  .......T...!.A.!
+00003f70: 0e10 0e0f 0e0c 0e0f 0e14 0601 0601 0601  ................
+00003f80: 0601 0601 0601 0601 0601 0601            ............
```

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/authentication/keycloak.py` & `django_dnoticias_services-1.1/dnoticias_services/authentication/keycloak.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Optional
 
 from django.contrib.auth import get_backends, get_user_model
 from django.core.exceptions import SuspiciousOperation
 from django.http import JsonResponse
 from django.conf import settings
 
+import requests
 from keycloak import KeycloakAdmin as BaseKeycloakAdmin, KeycloakOpenID, KeycloakDeleteError
 from mozilla_django_oidc.auth import OIDCAuthenticationBackend
 from dnoticias_services.communications import mail
 
 from .utils import raise_error_from_response
 
 User = get_user_model()
@@ -119,35 +120,36 @@
 
 class UpdateUser:
     """Updates an user in both sides (Keycloak and backends)."""
 
     def __call__(
         self,
         email: str,
-        first_name: str='',
-        last_name: str='',
-        enabled: bool=True,
-        is_staff: bool=False,
-        is_superuser: bool=False,
-        max_sessions: int=2,
-        update_attributes: bool=True,
-        custom_attributes: dict=dict()
+        first_name: Optional[str] = '',
+        last_name: Optional[str] = '',
+        enabled: Optional[bool] = True,
+        email_verified: Optional[bool] = None,
+        is_staff: Optional[bool] = False,
+        is_superuser: Optional[bool] = False,
+        max_sessions: Optional[int] = 2,
+        update_attributes: Optional[bool] = True,
+        custom_attributes: Optional[dict] = dict()
     ) -> User:
         """Updates an user in backend and keycloak to keep the data consistency
         
         :param email: User email that we want to update
         :param first_name: New first name. Default=''
         :param last_name: New last name. Default=''
         :param enabled: True if the user is enabled (active). Default=True
+        :param email_verified: True if the user email is verified. Default=None
         :param is_staff: If True, sets is_staff to True. Default=False
         :param is_superuser: If True, sets is_superuser to True. Default=False
         :param max_sessions: Max sessions allowed to this user. Default=2
         :param update_attributes: Updates the is_staff, is_superuser and max_session on keycloak
         if is True. Default: True
-        ...
         :return: Created user
         :rtype: User
         """
         with BaseKeycloak() as base:
             user_id_keycloak = base.keycloak_admin.get_user_id(email)
 
             if user_id_keycloak is None:
@@ -156,14 +158,17 @@
 
             payload = {
                 'firstName': first_name,
                 'lastName': last_name,
                 'enabled': enabled,
             }
 
+            if email_verified is not None:
+                payload['emailVerified'] = email_verified
+
             if update_attributes:
                 payload['attributes'] = {
                     'is_staff': is_staff,
                     'is_superuser': is_superuser,
                     'max_sessions': max_sessions,
                 }
 
@@ -531,18 +536,66 @@
         if not session:
             return False
 
         with BaseKeycloak() as base:
             return base.keycloak_admin.delete_user_session(session)
 
 
+class UpdateUserVerification:
+    def __call__(self, email: str, verified: Optional[bool] = True) -> bool:
+        if not email:
+            return False
+
+        with BaseKeycloak() as base:
+            keycloak_user_id = base.keycloak_admin.get_user_id(email)
+            return base.keycloak_admin.update_user(
+                keycloak_user_id,
+                {"emailVerified": verified}
+            )
+        
+
+class UserIsVerified:
+    """Get the user attributes from keycloak"""
+
+    def __call__(self, email: str) -> Optional[dict]:
+        user_info = None
+        email_verified = False
+
+        with BaseKeycloak() as base:
+            user_id_keycloak = base.keycloak_admin.get_user_id(email)
+
+            if user_id_keycloak is None:
+                message = f"The user {email} does not exists on keycloak"
+                raise SuspiciousOperation(message)
+
+            user_info = base.keycloak_admin.get_user(user_id_keycloak)
+            email_verified = user_info.get("emailVerified", False)
+
+        return email_verified
+
+
+class SendVerificationEmail:
+    """Send a verification email to the user"""
+
+    def __call__(self, email: str) -> Optional[dict]:
+        response = requests.post(
+            settings.SUBSCRIPTIONS_SEND_VERIFICATION_EMAIL_URL,
+            json={"email": email}
+        )
+
+        return response
+
+
 update_user = UpdateUser()
 send_update_account = SendUpdateAccount()
 create_user = CreateUser()
 update_password = UpdatePassword()
 get_token = GetToken()
 refresh_token = RefreshToken()
 logout_user = LogoutUser()
 get_token_info = GetTokenInfo()
 keycloak_user_exists = KeycloakUserExists()
 get_user_keycloak_info = GetUserKeycloakInfo()
 delete_user_session = DeleteUserSession()
+update_user_verification = UpdateUserVerification()
+user_is_verified = UserIsVerified()
+send_verification_email = SendVerificationEmail()
```

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/authentication/utils.py` & `django_dnoticias_services-1.1/dnoticias_services/authentication/utils.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/base_service.py` & `django_dnoticias_services-1.1/dnoticias_services/base_service.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/communications/README.md` & `django_dnoticias_services-1.1/dnoticias_services/communications/README.md`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/communications/__init__.py` & `django_dnoticias_services-1.1/dnoticias_services/communications/__init__.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/communications/campaign.py` & `django_dnoticias_services-1.1/dnoticias_services/communications/campaign.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/communications/context_processors.py` & `django_dnoticias_services-1.1/dnoticias_services/communications/context_processors.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/communications/forms.py` & `django_dnoticias_services-1.1/dnoticias_services/communications/forms.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/communications/mail.py` & `django_dnoticias_services-1.1/dnoticias_services/communications/mail.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/communications/notification.py` & `django_dnoticias_services-1.1/dnoticias_services/communications/notification.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/communications/urls.py` & `django_dnoticias_services-1.1/dnoticias_services/communications/urls.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/communications/views.py` & `django_dnoticias_services-1.1/dnoticias_services/communications/views.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/migrations/0001_initial.py` & `django_dnoticias_services-1.1/dnoticias_services/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/models.py` & `django_dnoticias_services-1.1/dnoticias_services/models.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/payments/coupons.py` & `django_dnoticias_services-1.1/dnoticias_services/payments/coupons.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/payments/items.py` & `django_dnoticias_services-1.1/dnoticias_services/payments/items.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/payments/orders.py` & `django_dnoticias_services-1.1/dnoticias_services/payments/orders.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/payments/payments.py` & `django_dnoticias_services-1.1/dnoticias_services/payments/payments.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/payments/providers.py` & `django_dnoticias_services-1.1/dnoticias_services/payments/providers.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/payments/subscriptions.py` & `django_dnoticias_services-1.1/dnoticias_services/payments/subscriptions.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/address.py` & `django_dnoticias_services-1.1/dnoticias_services/subscriptions/address.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/billing.py` & `django_dnoticias_services-1.1/dnoticias_services/subscriptions/billing.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/coupons.py` & `django_dnoticias_services-1.1/dnoticias_services/subscriptions/coupons.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/digital.py` & `django_dnoticias_services-1.1/dnoticias_services/subscriptions/digital.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/product.py` & `django_dnoticias_services-1.1/dnoticias_services/subscriptions/product.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/subscription.py` & `django_dnoticias_services-1.1/dnoticias_services/subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/subscriptions/user.py` & `django_dnoticias_services-1.1/dnoticias_services/subscriptions/user.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/templates/backoffice/fcm-notifications/form.html` & `django_dnoticias_services-1.1/dnoticias_services/templates/backoffice/fcm-notifications/form.html`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/templates/backoffice/fcm-notifications/list.html` & `django_dnoticias_services-1.1/dnoticias_services/templates/backoffice/fcm-notifications/list.html`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/templates/backoffice/fcm-topics/form.html` & `django_dnoticias_services-1.1/dnoticias_services/templates/backoffice/fcm-topics/form.html`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/templates/backoffice/fcm-topics/list.html` & `django_dnoticias_services-1.1/dnoticias_services/templates/backoffice/fcm-topics/list.html`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/templates/frontoffice/includes/firebase-notifications.js` & `django_dnoticias_services-1.1/dnoticias_services/templates/frontoffice/includes/firebase-notifications.js`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/utils/request.py` & `django_dnoticias_services-1.1/dnoticias_services/utils/request.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.0.97/dnoticias_services/utils/views.py` & `django_dnoticias_services-1.1/dnoticias_services/utils/views.py`

 * *Files identical despite different names*

