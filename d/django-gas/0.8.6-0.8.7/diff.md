# Comparing `tmp/django-gas-0.8.6.tar.gz` & `tmp/django-gas-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-gas-0.8.6.tar", last modified: Thu Sep  1 09:26:40 2022, max compression
+gzip compressed data, was "django-gas-0.8.7.tar", last modified: Wed May  3 14:08:01 2023, max compression
```

## Comparing `django-gas-0.8.6.tar` & `django-gas-0.8.7.tar`

### file list

```diff
@@ -1,331 +1,220 @@
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.120090 django-gas-0.8.6/
--rw-r--r--   0 shagi     (1000) shagi     (1000)    35147 2020-12-15 14:37:13.000000 django-gas-0.8.6/LICENSE.txt
--rw-r--r--   0 shagi     (1000) shagi     (1000)      133 2021-04-14 15:40:48.000000 django-gas-0.8.6/MANIFEST.in
--rw-r--r--   0 shagi     (1000) shagi     (1000)     4258 2022-09-01 09:26:40.120090 django-gas-0.8.6/PKG-INFO
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.016090 django-gas-0.8.6/django_gas.egg-info/
--rw-r--r--   0 shagi     (1000) shagi     (1000)     4258 2022-09-01 09:26:39.000000 django-gas-0.8.6/django_gas.egg-info/PKG-INFO
--rw-r--r--   0 shagi     (1000) shagi     (1000)    11175 2022-09-01 09:26:39.000000 django-gas-0.8.6/django_gas.egg-info/SOURCES.txt
--rw-r--r--   0 shagi     (1000) shagi     (1000)        1 2022-09-01 09:26:39.000000 django-gas-0.8.6/django_gas.egg-info/dependency_links.txt
--rw-r--r--   0 shagi     (1000) shagi     (1000)        4 2022-09-01 09:26:39.000000 django-gas-0.8.6/django_gas.egg-info/top_level.txt
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.016090 django-gas-0.8.6/gas/
--rw-r--r--   0 shagi     (1000) shagi     (1000)        0 2022-02-21 10:20:58.000000 django-gas-0.8.6/gas/__init__.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)      193 2022-02-21 10:22:59.000000 django-gas-0.8.6/gas/admin.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)      324 2022-02-21 10:21:41.000000 django-gas-0.8.6/gas/apps.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)     2348 2022-07-06 06:13:41.000000 django-gas-0.8.6/gas/forms.py
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.016090 django-gas-0.8.6/gas/gas/
--rw-r--r--   0 shagi     (1000) shagi     (1000)        0 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/gas/__init__.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)      293 2021-05-11 14:13:50.000000 django-gas-0.8.6/gas/gas/config.py
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.020089 django-gas-0.8.6/gas/gas/core/
--rw-r--r--   0 shagi     (1000) shagi     (1000)        0 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/gas/core/__init__.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)      417 2020-12-13 10:43:46.000000 django-gas-0.8.6/gas/gas/core/urls.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)     1382 2022-06-16 15:35:09.000000 django-gas-0.8.6/gas/gas/core/views.py
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.020089 django-gas-0.8.6/gas/gas/users/
--rw-r--r--   0 shagi     (1000) shagi     (1000)        0 2020-12-12 10:08:24.000000 django-gas-0.8.6/gas/gas/users/__init__.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)      898 2020-12-20 09:31:22.000000 django-gas-0.8.6/gas/gas/users/forms.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)      455 2020-12-12 16:15:11.000000 django-gas-0.8.6/gas/gas/users/urls.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)     3238 2022-06-16 15:35:09.000000 django-gas-0.8.6/gas/gas/users/views.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)      258 2021-05-11 14:14:02.000000 django-gas-0.8.6/gas/gas/users_config.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)      582 2021-01-07 16:03:14.000000 django-gas-0.8.6/gas/gas_settings.py
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:39.996089 django-gas-0.8.6/gas/locale/
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:39.996089 django-gas-0.8.6/gas/locale/es/
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.020089 django-gas-0.8.6/gas/locale/es/LC_MESSAGES/
--rw-r--r--   0 shagi     (1000) shagi     (1000)     2940 2021-04-14 15:16:05.000000 django-gas-0.8.6/gas/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 shagi     (1000) shagi     (1000)     4945 2021-05-12 14:16:36.000000 django-gas-0.8.6/gas/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:39.996089 django-gas-0.8.6/gas/locale/eu/
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.020089 django-gas-0.8.6/gas/locale/eu/LC_MESSAGES/
--rw-r--r--   0 shagi     (1000) shagi     (1000)     2995 2021-04-14 15:16:05.000000 django-gas-0.8.6/gas/locale/eu/LC_MESSAGES/django.mo
--rw-r--r--   0 shagi     (1000) shagi     (1000)     5042 2021-05-12 14:16:36.000000 django-gas-0.8.6/gas/locale/eu/LC_MESSAGES/django.po
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.020089 django-gas-0.8.6/gas/migrations/
--rw-r--r--   0 shagi     (1000) shagi     (1000)      956 2020-12-22 17:04:20.000000 django-gas-0.8.6/gas/migrations/0001_initial.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)        0 2020-12-11 16:57:02.000000 django-gas-0.8.6/gas/migrations/__init__.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)      606 2020-12-19 08:42:53.000000 django-gas-0.8.6/gas/models.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)     3589 2021-05-12 14:12:38.000000 django-gas-0.8.6/gas/sites.py
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:39.996089 django-gas-0.8.6/gas/static/
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:39.996089 django-gas-0.8.6/gas/static/gas/
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.020089 django-gas-0.8.6/gas/static/gas/css/
--rw-r--r--   0 shagi     (1000) shagi     (1000)     3813 2022-06-02 11:01:27.000000 django-gas-0.8.6/gas/static/gas/css/gas.css
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.024089 django-gas-0.8.6/gas/static/gas/css/img/
--rw-r--r--   0 shagi     (1000) shagi     (1000)     2478 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/gas/css/img/logo.svg
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.024089 django-gas-0.8.6/gas/static/gas/js/
--rw-r--r--   0 shagi     (1000) shagi     (1000)     2442 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/gas/js/add_popups.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)     2912 2021-05-11 16:50:23.000000 django-gas-0.8.6/gas/static/gas/js/gas.js
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.024089 django-gas-0.8.6/gas/static/vendor/
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.024089 django-gas-0.8.6/gas/static/vendor/font-awesome/
--rw-r--r--   0 shagi     (1000) shagi     (1000)     1548 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/LICENSE.txt
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.032090 django-gas-0.8.6/gas/static/vendor/font-awesome/css/
--rw-r--r--   0 shagi     (1000) shagi     (1000)    70942 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/css/all.css
--rw-r--r--   0 shagi     (1000) shagi     (1000)    57180 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/css/all.min.css
--rw-r--r--   0 shagi     (1000) shagi     (1000)      714 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/css/brands.css
--rw-r--r--   0 shagi     (1000) shagi     (1000)      661 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/css/brands.min.css
--rw-r--r--   0 shagi     (1000) shagi     (1000)    69327 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/css/fontawesome.css
--rw-r--r--   0 shagi     (1000) shagi     (1000)    55753 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/css/fontawesome.min.css
--rw-r--r--   0 shagi     (1000) shagi     (1000)      733 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/css/regular.css
--rw-r--r--   0 shagi     (1000) shagi     (1000)      676 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/css/regular.min.css
--rw-r--r--   0 shagi     (1000) shagi     (1000)      726 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/css/solid.css
--rw-r--r--   0 shagi     (1000) shagi     (1000)      668 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/css/solid.min.css
--rw-r--r--   0 shagi     (1000) shagi     (1000)     8077 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/css/svg-with-js.css
--rw-r--r--   0 shagi     (1000) shagi     (1000)     6359 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/css/svg-with-js.min.css
--rw-r--r--   0 shagi     (1000) shagi     (1000)    41312 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/css/v4-shims.css
--rw-r--r--   0 shagi     (1000) shagi     (1000)    26702 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/css/v4-shims.min.css
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.052090 django-gas-0.8.6/gas/static/vendor/font-awesome/js/
--rw-r--r--   0 shagi     (1000) shagi     (1000)  1209064 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/js/all.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)  1144185 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/js/all.min.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)   436422 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/js/brands.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)   429332 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/js/brands.min.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)    33664 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/js/conflict-detection.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)    13354 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/js/conflict-detection.min.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)    78307 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/js/fontawesome.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)    36835 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/js/fontawesome.min.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)   107110 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/js/regular.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)   103386 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/js/regular.min.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)   587783 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/js/solid.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)   575193 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/js/solid.min.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)    17459 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/js/v4-shims.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)    15055 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/js/v4-shims.min.js
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.068090 django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/
--rw-r--r--   0 shagi     (1000) shagi     (1000)   131930 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-brands-400.eot
--rw-r--r--   0 shagi     (1000) shagi     (1000)   708706 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-brands-400.svg
--rw-r--r--   0 shagi     (1000) shagi     (1000)   131624 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0 shagi     (1000) shagi     (1000)    89100 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-brands-400.woff
--rw-r--r--   0 shagi     (1000) shagi     (1000)    75936 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0 shagi     (1000) shagi     (1000)    34390 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-regular-400.eot
--rw-r--r--   0 shagi     (1000) shagi     (1000)   144322 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-regular-400.svg
--rw-r--r--   0 shagi     (1000) shagi     (1000)    34092 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0 shagi     (1000) shagi     (1000)    16800 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-regular-400.woff
--rw-r--r--   0 shagi     (1000) shagi     (1000)    13576 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0 shagi     (1000) shagi     (1000)   194066 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-solid-900.eot
--rw-r--r--   0 shagi     (1000) shagi     (1000)   849145 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-solid-900.svg
--rw-r--r--   0 shagi     (1000) shagi     (1000)   193780 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0 shagi     (1000) shagi     (1000)    98996 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-solid-900.woff
--rw-r--r--   0 shagi     (1000) shagi     (1000)    76084 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.068090 django-gas-0.8.6/gas/static/vendor/jquery/
--rw-r--r--   0 shagi     (1000) shagi     (1000)      729 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/.bower.json
--rw-r--r--   0 shagi     (1000) shagi     (1000)     1099 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/MIT-LICENSE.txt
--rw-r--r--   0 shagi     (1000) shagi     (1000)      426 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/bower.json
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.068090 django-gas-0.8.6/gas/static/vendor/jquery/dist/
--rw-r--r--   0 shagi     (1000) shagi     (1000)   244963 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/dist/jquery.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)    83615 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/dist/jquery.min.js
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.080089 django-gas-0.8.6/gas/static/vendor/jquery/src/
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.080089 django-gas-0.8.6/gas/static/vendor/jquery/src/ajax/
--rw-r--r--   0 shagi     (1000) shagi     (1000)     2516 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/ajax/jsonp.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)     1654 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/ajax/load.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)      222 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/ajax/parseJSON.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)      485 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/ajax/parseXML.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)     1271 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/ajax/script.js
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.080089 django-gas-0.8.6/gas/static/vendor/jquery/src/ajax/var/
--rw-r--r--   0 shagi     (1000) shagi     (1000)       73 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/ajax/var/nonce.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)       40 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/ajax/var/rquery.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)     3346 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/ajax/xhr.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)    21719 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/ajax.js
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.080089 django-gas-0.8.6/gas/static/vendor/jquery/src/attributes/
--rw-r--r--   0 shagi     (1000) shagi     (1000)     3484 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/attributes/attr.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)     4155 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/attributes/classes.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)     1934 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/attributes/prop.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)      970 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/attributes/support.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)     3677 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/attributes/val.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)      200 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/attributes.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)     5506 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/callbacks.js
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.084090 django-gas-0.8.6/gas/static/vendor/jquery/src/core/
--rw-r--r--   0 shagi     (1000) shagi     (1000)     1210 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/core/access.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)     3410 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/core/init.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)      938 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/core/parseHTML.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)     2340 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/core/ready.js
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.084090 django-gas-0.8.6/gas/static/vendor/jquery/src/core/var/
--rw-r--r--   0 shagi     (1000) shagi     (1000)       91 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/core/var/rsingleTag.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)    11757 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/core.js
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.084090 django-gas-0.8.6/gas/static/vendor/jquery/src/css/
--rw-r--r--   0 shagi     (1000) shagi     (1000)      590 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/css/addGetHookIf.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)     1462 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/css/curCSS.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)     1836 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/css/defaultDisplay.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)      380 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/css/hiddenVisibleSelectors.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)     3009 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/css/support.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)      555 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/css/swap.js
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.088090 django-gas-0.8.6/gas/static/vendor/jquery/src/css/var/
--rw-r--r--   0 shagi     (1000) shagi     (1000)       70 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/css/var/cssExpand.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)      127 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/css/var/getStyles.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)      355 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/css/var/isHidden.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)       45 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/css/var/rmargin.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)      113 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/css/var/rnumnonpx.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)    12883 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/css.js
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.088090 django-gas-0.8.6/gas/static/vendor/jquery/src/data/
--rw-r--r--   0 shagi     (1000) shagi     (1000)     4889 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/data/Data.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)      383 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/data/accepts.js
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.088090 django-gas-0.8.6/gas/static/vendor/jquery/src/data/var/
--rw-r--r--   0 shagi     (1000) shagi     (1000)       66 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/data/var/data_priv.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)       66 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/data/var/data_user.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)     4817 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/data.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)     4414 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/deferred.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)      223 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/deprecated.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)     1776 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/dimensions.js
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.088090 django-gas-0.8.6/gas/static/vendor/jquery/src/effects/
--rw-r--r--   0 shagi     (1000) shagi     (1000)     3031 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/effects/Tween.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)      225 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/effects/animatedSelector.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)    16602 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/effects.js
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.088090 django-gas-0.8.6/gas/static/vendor/jquery/src/event/
--rw-r--r--   0 shagi     (1000) shagi     (1000)     1094 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/event/alias.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)      123 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/event/support.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)    24299 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/event.js
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.088090 django-gas-0.8.6/gas/static/vendor/jquery/src/exports/
--rw-r--r--   0 shagi     (1000) shagi     (1000)      691 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/exports/amd.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)      641 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/exports/global.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)     1405 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/intro.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)      557 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/jquery.js
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.092090 django-gas-0.8.6/gas/static/vendor/jquery/src/manipulation/
--rw-r--r--   0 shagi     (1000) shagi     (1000)      240 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/manipulation/_evalUrl.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)      776 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/manipulation/support.js
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.092090 django-gas-0.8.6/gas/static/vendor/jquery/src/manipulation/var/
--rw-r--r--   0 shagi     (1000) shagi     (1000)       59 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/manipulation/var/rcheckableType.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)    15110 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/manipulation.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)     5481 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/offset.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)        5 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/outro.js
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.092090 django-gas-0.8.6/gas/static/vendor/jquery/src/queue/
--rw-r--r--   0 shagi     (1000) shagi     (1000)      561 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/queue/delay.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)     3090 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/queue.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)     4413 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/selector-native.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)      294 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/selector-sizzle.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)       33 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/selector.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)     3214 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/serialize.js
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.000090 django-gas-0.8.6/gas/static/vendor/jquery/src/sizzle/
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.092090 django-gas-0.8.6/gas/static/vendor/jquery/src/sizzle/dist/
--rw-r--r--   0 shagi     (1000) shagi     (1000)    57549 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/sizzle/dist/sizzle.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)    18404 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/sizzle/dist/sizzle.min.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)    28824 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/sizzle/dist/sizzle.min.map
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.092090 django-gas-0.8.6/gas/static/vendor/jquery/src/traversing/
--rw-r--r--   0 shagi     (1000) shagi     (1000)     2464 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/traversing/findFilter.js
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.092090 django-gas-0.8.6/gas/static/vendor/jquery/src/traversing/var/
--rw-r--r--   0 shagi     (1000) shagi     (1000)      110 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/traversing/var/rneedsContext.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)     4559 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/traversing.js
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.096089 django-gas-0.8.6/gas/static/vendor/jquery/src/var/
--rw-r--r--   0 shagi     (1000) shagi     (1000)       36 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/var/arr.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)       64 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/var/class2type.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)       63 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/var/concat.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)       92 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/var/hasOwn.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)       64 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/var/indexOf.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)       80 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/var/pnum.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)       61 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/var/push.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)       42 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/var/rnotwhite.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)       62 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/var/slice.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)       50 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/var/strundefined.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)       99 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/var/support.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)       86 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/var/toString.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)       41 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/var/trim.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)     1468 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery/src/wrap.js
--rw-r--r--   0 shagi     (1000) shagi     (1000)    12738 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/static/vendor/jquery.formset.js
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.100090 django-gas-0.8.6/gas/static/vendor/select2/
--rw-rw-r--   0 shagi     (1000) shagi     (1000)       66 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/.editorconfig
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.100090 django-gas-0.8.6/gas/static/vendor/select2/.github/
--rw-rw-r--   0 shagi     (1000) shagi     (1000)    11677 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/.github/CONTRIBUTING.md
--rw-rw-r--   0 shagi     (1000) shagi     (1000)       24 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/.github/FUNDING.yml
--rw-rw-r--   0 shagi     (1000) shagi     (1000)     2426 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/.github/ISSUE_TEMPLATE.md
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      193 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/.github/PULL_REQUEST_TEMPLATE.md
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      654 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/.github/stale.yml
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.100090 django-gas-0.8.6/gas/static/vendor/select2/.github/workflows/
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      701 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/.github/workflows/docs-deploy.yml
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      995 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/.github/workflows/main.yml
--rw-rw-r--   0 shagi     (1000) shagi     (1000)     1679 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/.github/workflows/package-deploy.yml
--rw-rw-r--   0 shagi     (1000) shagi     (1000)       48 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/.gitignore
--rw-rw-r--   0 shagi     (1000) shagi     (1000)       74 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/.jshintignore
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      433 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/.jshintrc
--rw-rw-r--   0 shagi     (1000) shagi     (1000)     1124 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/LICENSE.md
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.100090 django-gas-0.8.6/gas/static/vendor/select2/css/
--rw-rw-r--   0 shagi     (1000) shagi     (1000)    17358 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/css/select2.css
--rw-rw-r--   0 shagi     (1000) shagi     (1000)    14966 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/css/select2.min.css
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.104090 django-gas-0.8.6/gas/static/vendor/select2/js/
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.116089 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      866 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/af.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      905 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/ar.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      721 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/az.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      968 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/bg.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)     1291 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/bn.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      965 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/bs.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      900 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/ca.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)     1292 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/cs.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      828 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/da.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      866 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/de.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)     1017 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/dsb.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)     1182 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/el.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      844 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/en.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      922 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/es.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      801 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/et.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      868 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/eu.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)     1023 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/fa.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      803 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/fi.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      924 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/fr.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      924 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/gl.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      984 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/he.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)     1175 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/hi.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      852 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/hr.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)     1018 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/hsb.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      831 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/hu.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)     1028 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/hy.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      768 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/id.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      807 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/is.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      897 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/it.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      862 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/ja.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)     1195 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/ka.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)     1088 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/km.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      855 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/ko.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      944 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/lt.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      900 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/lv.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)     1038 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/mk.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      811 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/ms.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      778 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/nb.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)     1357 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/ne.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      904 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/nl.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      947 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/pl.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)     1049 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/ps.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      876 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/pt-BR.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      878 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/pt.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      938 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/ro.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)     1171 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/ru.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)     1306 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/sk.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      925 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/sl.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      903 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/sq.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)     1109 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/sr-Cyrl.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      980 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/sr.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      786 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/sv.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)     1074 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/th.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      771 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/tk.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      775 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/tr.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)     1156 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/uk.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      796 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/vi.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      768 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/zh-CN.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)      707 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/i18n/zh-TW.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)   171737 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/select2.full.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)    78627 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/select2.full.min.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)   151811 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/select2.js
--rw-rw-r--   0 shagi     (1000) shagi     (1000)    70357 2019-11-06 01:34:17.000000 django-gas-0.8.6/gas/static/vendor/select2/js/select2.min.js
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.000090 django-gas-0.8.6/gas/templates/
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.116089 django-gas-0.8.6/gas/templates/gas/
--rw-r--r--   0 shagi     (1000) shagi     (1000)     4140 2022-09-01 09:19:51.000000 django-gas-0.8.6/gas/templates/gas/base.html
--rw-r--r--   0 shagi     (1000) shagi     (1000)     1287 2022-07-01 07:20:02.000000 django-gas-0.8.6/gas/templates/gas/base_form.html
--rw-r--r--   0 shagi     (1000) shagi     (1000)      534 2021-01-05 17:45:34.000000 django-gas-0.8.6/gas/templates/gas/base_list.html
--rw-r--r--   0 shagi     (1000) shagi     (1000)      861 2022-06-16 15:35:09.000000 django-gas-0.8.6/gas/templates/gas/delete_confirmation.html
--rw-r--r--   0 shagi     (1000) shagi     (1000)      132 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/templates/gas/index.html
--rw-r--r--   0 shagi     (1000) shagi     (1000)      731 2021-05-11 16:41:10.000000 django-gas-0.8.6/gas/templates/gas/login.html
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.116089 django-gas-0.8.6/gas/templates/gas/tags/
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.120090 django-gas-0.8.6/gas/templates/gas/tags/forms/
--rw-r--r--   0 shagi     (1000) shagi     (1000)      387 2021-01-05 16:13:06.000000 django-gas-0.8.6/gas/templates/gas/tags/forms/checkbox.html
--rw-r--r--   0 shagi     (1000) shagi     (1000)      431 2021-02-11 15:53:01.000000 django-gas-0.8.6/gas/templates/gas/tags/forms/errors.html
--rw-r--r--   0 shagi     (1000) shagi     (1000)      634 2021-01-11 15:02:11.000000 django-gas-0.8.6/gas/templates/gas/tags/forms/field.html
--rw-r--r--   0 shagi     (1000) shagi     (1000)      745 2021-05-11 16:43:55.000000 django-gas-0.8.6/gas/templates/gas/tags/navigation.html
--rw-r--r--   0 shagi     (1000) shagi     (1000)      893 2021-03-23 17:39:11.000000 django-gas-0.8.6/gas/templates/gas/tags/pagination.html
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.120090 django-gas-0.8.6/gas/templates/gas/users/
--rw-r--r--   0 shagi     (1000) shagi     (1000)     1479 2020-12-15 19:15:56.000000 django-gas-0.8.6/gas/templates/gas/users/user_list.html
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.120090 django-gas-0.8.6/gas/templatetags/
--rw-r--r--   0 shagi     (1000) shagi     (1000)        0 2020-12-10 16:12:45.000000 django-gas-0.8.6/gas/templatetags/__init__.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)     1632 2021-05-18 16:17:35.000000 django-gas-0.8.6/gas/templatetags/form_tags.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)     1292 2021-03-31 06:33:28.000000 django-gas-0.8.6/gas/templatetags/gas_tags.py
-drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2022-09-01 09:26:40.120090 django-gas-0.8.6/gas/tests/
--rw-r--r--   0 shagi     (1000) shagi     (1000)        0 2020-12-14 15:41:27.000000 django-gas-0.8.6/gas/tests/__init__.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)     1246 2020-12-18 10:33:25.000000 django-gas-0.8.6/gas/tests/test_core_views.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)      451 2020-12-17 15:53:39.000000 django-gas-0.8.6/gas/tests/test_models.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)     4956 2021-05-12 13:52:28.000000 django-gas-0.8.6/gas/tests/test_site.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)     2838 2020-12-20 09:31:24.000000 django-gas-0.8.6/gas/tests/test_user_forms.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)     1238 2021-06-10 15:13:12.000000 django-gas-0.8.6/gas/tests/test_utils.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)    15954 2022-09-01 09:21:34.000000 django-gas-0.8.6/gas/tests/test_views.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)      133 2020-12-15 17:46:42.000000 django-gas-0.8.6/gas/tests/urls.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)      545 2021-06-10 15:13:12.000000 django-gas-0.8.6/gas/utils.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)     9947 2022-09-01 09:19:00.000000 django-gas-0.8.6/gas/views.py
--rw-r--r--   0 shagi     (1000) shagi     (1000)      868 2022-09-01 09:26:40.124090 django-gas-0.8.6/setup.cfg
--rw-r--r--   0 shagi     (1000) shagi     (1000)       38 2021-03-02 19:32:16.000000 django-gas-0.8.6/setup.py
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:01.023626 django-gas-0.8.7/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    35147 2023-05-03 13:47:07.000000 django-gas-0.8.7/LICENSE.txt
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      133 2023-05-03 13:47:03.000000 django-gas-0.8.7/MANIFEST.in
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     4288 2023-05-03 14:08:01.023626 django-gas-0.8.7/PKG-INFO
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:00.999626 django-gas-0.8.7/django_gas.egg-info/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     4288 2023-05-03 14:08:00.000000 django-gas-0.8.7/django_gas.egg-info/PKG-INFO
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     7186 2023-05-03 14:08:00.000000 django-gas-0.8.7/django_gas.egg-info/SOURCES.txt
+-rw-r--r--   0 shagi     (1000) shagi     (1000)        1 2023-05-03 14:08:00.000000 django-gas-0.8.7/django_gas.egg-info/dependency_links.txt
+-rw-r--r--   0 shagi     (1000) shagi     (1000)        4 2023-05-03 14:08:00.000000 django-gas-0.8.7/django_gas.egg-info/top_level.txt
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:00.999626 django-gas-0.8.7/gas/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)        0 2023-05-03 13:46:27.000000 django-gas-0.8.7/gas/__init__.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      193 2023-05-03 13:46:26.000000 django-gas-0.8.7/gas/admin.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      324 2023-05-03 13:46:27.000000 django-gas-0.8.7/gas/apps.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     2340 2023-05-03 13:46:26.000000 django-gas-0.8.7/gas/forms.py
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:00.999626 django-gas-0.8.7/gas/gas/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)        0 2023-05-03 13:46:26.000000 django-gas-0.8.7/gas/gas/__init__.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      293 2023-05-03 13:46:26.000000 django-gas-0.8.7/gas/gas/config.py
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:00.999626 django-gas-0.8.7/gas/gas/core/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)        0 2023-05-03 13:46:26.000000 django-gas-0.8.7/gas/gas/core/__init__.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      417 2023-05-03 13:46:26.000000 django-gas-0.8.7/gas/gas/core/urls.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1382 2023-05-03 13:46:26.000000 django-gas-0.8.7/gas/gas/core/views.py
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:00.999626 django-gas-0.8.7/gas/gas/users/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)        0 2023-05-03 13:46:26.000000 django-gas-0.8.7/gas/gas/users/__init__.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      898 2023-05-03 13:46:26.000000 django-gas-0.8.7/gas/gas/users/forms.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      455 2023-05-03 13:46:26.000000 django-gas-0.8.7/gas/gas/users/urls.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     3238 2023-05-03 13:46:26.000000 django-gas-0.8.7/gas/gas/users/views.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      258 2023-05-03 13:46:26.000000 django-gas-0.8.7/gas/gas/users_config.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      576 2023-05-03 13:51:46.000000 django-gas-0.8.7/gas/gas_settings.py
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:00.995626 django-gas-0.8.7/gas/locale/
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:00.995626 django-gas-0.8.7/gas/locale/es/
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:00.999626 django-gas-0.8.7/gas/locale/es/LC_MESSAGES/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     2996 2023-05-03 14:02:01.000000 django-gas-0.8.7/gas/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     5304 2023-05-03 14:01:14.000000 django-gas-0.8.7/gas/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:00.995626 django-gas-0.8.7/gas/locale/eu/
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:00.999626 django-gas-0.8.7/gas/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     3096 2023-05-03 14:02:01.000000 django-gas-0.8.7/gas/locale/eu/LC_MESSAGES/django.mo
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     5404 2023-05-03 14:01:32.000000 django-gas-0.8.7/gas/locale/eu/LC_MESSAGES/django.po
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:00.999626 django-gas-0.8.7/gas/migrations/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      956 2023-05-03 13:46:27.000000 django-gas-0.8.7/gas/migrations/0001_initial.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)        0 2023-05-03 13:46:27.000000 django-gas-0.8.7/gas/migrations/__init__.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      606 2023-05-03 13:46:27.000000 django-gas-0.8.7/gas/models.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     3589 2023-05-03 13:46:27.000000 django-gas-0.8.7/gas/sites.py
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:00.995626 django-gas-0.8.7/gas/static/
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:00.995626 django-gas-0.8.7/gas/static/gas/
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:00.999626 django-gas-0.8.7/gas/static/gas/css/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     3813 2023-05-03 13:46:23.000000 django-gas-0.8.7/gas/static/gas/css/gas.css
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:00.999626 django-gas-0.8.7/gas/static/gas/css/img/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     2478 2023-05-03 13:46:23.000000 django-gas-0.8.7/gas/static/gas/css/img/logo.svg
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:01.003625 django-gas-0.8.7/gas/static/gas/js/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     2442 2023-05-03 13:46:23.000000 django-gas-0.8.7/gas/static/gas/js/add_popups.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     2912 2023-05-03 13:46:23.000000 django-gas-0.8.7/gas/static/gas/js/gas.js
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:01.003625 django-gas-0.8.7/gas/static/vendor/
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:01.003625 django-gas-0.8.7/gas/static/vendor/font-awesome/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1548 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/LICENSE.txt
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:01.003625 django-gas-0.8.7/gas/static/vendor/font-awesome/css/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    70942 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/css/all.css
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    57180 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/css/all.min.css
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      714 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/css/brands.css
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      661 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/css/brands.min.css
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    69327 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/css/fontawesome.css
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    55753 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/css/fontawesome.min.css
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      733 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/css/regular.css
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      676 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/css/regular.min.css
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      726 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/css/solid.css
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      668 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/css/solid.min.css
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     8077 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/css/svg-with-js.css
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     6359 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/css/svg-with-js.min.css
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    41312 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/css/v4-shims.css
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    26702 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/css/v4-shims.min.css
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:01.011626 django-gas-0.8.7/gas/static/vendor/font-awesome/js/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)  1209064 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/js/all.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)  1144185 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/js/all.min.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)   436422 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/js/brands.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)   429332 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/js/brands.min.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    33664 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/js/conflict-detection.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    13354 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/js/conflict-detection.min.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    78307 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/js/fontawesome.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    36835 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/js/fontawesome.min.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)   107110 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/js/regular.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)   103386 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/js/regular.min.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)   587783 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/js/solid.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)   575193 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/js/solid.min.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    17459 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/js/v4-shims.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    15055 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/js/v4-shims.min.js
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:01.015626 django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)   131930 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-brands-400.eot
+-rw-r--r--   0 shagi     (1000) shagi     (1000)   708706 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-brands-400.svg
+-rw-r--r--   0 shagi     (1000) shagi     (1000)   131624 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    89100 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-brands-400.woff
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    75936 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    34390 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-regular-400.eot
+-rw-r--r--   0 shagi     (1000) shagi     (1000)   144322 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-regular-400.svg
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    34092 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    16800 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-regular-400.woff
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    13576 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 shagi     (1000) shagi     (1000)   194066 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-solid-900.eot
+-rw-r--r--   0 shagi     (1000) shagi     (1000)   849145 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-solid-900.svg
+-rw-r--r--   0 shagi     (1000) shagi     (1000)   193780 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    98996 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-solid-900.woff
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    76084 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    89795 2023-05-03 13:51:08.000000 django-gas-0.8.7/gas/static/vendor/jquery-3.6.4.min.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    12738 2023-05-03 13:46:25.000000 django-gas-0.8.7/gas/static/vendor/jquery.formset.js
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:01.015626 django-gas-0.8.7/gas/static/vendor/select2/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)       66 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/.editorconfig
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:01.015626 django-gas-0.8.7/gas/static/vendor/select2/.github/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    11677 2023-05-03 13:46:23.000000 django-gas-0.8.7/gas/static/vendor/select2/.github/CONTRIBUTING.md
+-rw-r--r--   0 shagi     (1000) shagi     (1000)       24 2023-05-03 13:46:23.000000 django-gas-0.8.7/gas/static/vendor/select2/.github/FUNDING.yml
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     2426 2023-05-03 13:46:23.000000 django-gas-0.8.7/gas/static/vendor/select2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      193 2023-05-03 13:46:23.000000 django-gas-0.8.7/gas/static/vendor/select2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      654 2023-05-03 13:46:23.000000 django-gas-0.8.7/gas/static/vendor/select2/.github/stale.yml
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:01.015626 django-gas-0.8.7/gas/static/vendor/select2/.github/workflows/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      701 2023-05-03 13:46:23.000000 django-gas-0.8.7/gas/static/vendor/select2/.github/workflows/docs-deploy.yml
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      995 2023-05-03 13:46:23.000000 django-gas-0.8.7/gas/static/vendor/select2/.github/workflows/main.yml
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1679 2023-05-03 13:46:23.000000 django-gas-0.8.7/gas/static/vendor/select2/.github/workflows/package-deploy.yml
+-rw-r--r--   0 shagi     (1000) shagi     (1000)       48 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/.gitignore
+-rw-r--r--   0 shagi     (1000) shagi     (1000)       74 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/.jshintignore
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      433 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/.jshintrc
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1124 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/LICENSE.md
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:01.015626 django-gas-0.8.7/gas/static/vendor/select2/css/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    17358 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/css/select2.css
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    14966 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/css/select2.min.css
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:01.015626 django-gas-0.8.7/gas/static/vendor/select2/js/
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:01.023626 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      866 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/af.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      905 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/ar.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      721 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/az.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      968 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/bg.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1291 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/bn.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      965 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/bs.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      900 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/ca.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1292 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/cs.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      828 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/da.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      866 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/de.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1017 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/dsb.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1182 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/el.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      844 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/en.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      922 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/es.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      801 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/et.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      868 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/eu.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1023 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/fa.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      803 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/fi.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      924 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/fr.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      924 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/gl.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      984 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/he.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1175 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/hi.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      852 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/hr.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1018 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/hsb.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      831 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/hu.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1028 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/hy.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      768 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/id.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      807 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/is.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      897 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/it.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      862 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/ja.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1195 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/ka.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1088 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/km.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      855 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/ko.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      944 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/lt.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      900 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/lv.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1038 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/mk.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      811 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/ms.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      778 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/nb.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1357 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/ne.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      904 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/nl.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      947 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/pl.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1049 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/ps.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      876 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/pt-BR.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      878 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/pt.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      938 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/ro.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1171 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/ru.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1306 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/sk.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      925 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/sl.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      903 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/sq.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1109 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/sr-Cyrl.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      980 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/sr.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      786 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/sv.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1074 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/th.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      771 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/tk.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      775 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/tr.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1156 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/uk.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      796 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/vi.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      768 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/zh-CN.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      707 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/i18n/zh-TW.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)   171737 2023-05-03 13:46:23.000000 django-gas-0.8.7/gas/static/vendor/select2/js/select2.full.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    78627 2023-05-03 13:46:23.000000 django-gas-0.8.7/gas/static/vendor/select2/js/select2.full.min.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)   151811 2023-05-03 13:46:24.000000 django-gas-0.8.7/gas/static/vendor/select2/js/select2.js
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    70357 2023-05-03 13:46:23.000000 django-gas-0.8.7/gas/static/vendor/select2/js/select2.min.js
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:00.999626 django-gas-0.8.7/gas/templates/
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:01.023626 django-gas-0.8.7/gas/templates/gas/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     4140 2023-05-03 13:46:27.000000 django-gas-0.8.7/gas/templates/gas/base.html
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1287 2023-05-03 13:46:27.000000 django-gas-0.8.7/gas/templates/gas/base_form.html
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      534 2023-05-03 13:46:27.000000 django-gas-0.8.7/gas/templates/gas/base_list.html
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      861 2023-05-03 13:46:27.000000 django-gas-0.8.7/gas/templates/gas/delete_confirmation.html
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      132 2023-05-03 13:46:27.000000 django-gas-0.8.7/gas/templates/gas/index.html
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      731 2023-05-03 13:46:27.000000 django-gas-0.8.7/gas/templates/gas/login.html
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:01.023626 django-gas-0.8.7/gas/templates/gas/tags/
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:01.023626 django-gas-0.8.7/gas/templates/gas/tags/forms/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      387 2023-05-03 13:46:27.000000 django-gas-0.8.7/gas/templates/gas/tags/forms/checkbox.html
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      431 2023-05-03 13:46:27.000000 django-gas-0.8.7/gas/templates/gas/tags/forms/errors.html
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      634 2023-05-03 13:46:27.000000 django-gas-0.8.7/gas/templates/gas/tags/forms/field.html
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      745 2023-05-03 13:46:27.000000 django-gas-0.8.7/gas/templates/gas/tags/navigation.html
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      893 2023-05-03 13:46:27.000000 django-gas-0.8.7/gas/templates/gas/tags/pagination.html
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:01.023626 django-gas-0.8.7/gas/templates/gas/users/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1479 2023-05-03 13:46:27.000000 django-gas-0.8.7/gas/templates/gas/users/user_list.html
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:01.023626 django-gas-0.8.7/gas/templatetags/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)        0 2023-05-03 13:46:26.000000 django-gas-0.8.7/gas/templatetags/__init__.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1632 2023-05-03 13:46:26.000000 django-gas-0.8.7/gas/templatetags/form_tags.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1292 2023-05-03 13:46:26.000000 django-gas-0.8.7/gas/templatetags/gas_tags.py
+drwxr-xr-x   0 shagi     (1000) shagi     (1000)        0 2023-05-03 14:08:01.023626 django-gas-0.8.7/gas/tests/
+-rw-r--r--   0 shagi     (1000) shagi     (1000)        0 2023-05-03 13:46:23.000000 django-gas-0.8.7/gas/tests/__init__.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1246 2023-05-03 13:46:23.000000 django-gas-0.8.7/gas/tests/test_core_views.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      451 2023-05-03 13:46:23.000000 django-gas-0.8.7/gas/tests/test_models.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     4956 2023-05-03 13:46:23.000000 django-gas-0.8.7/gas/tests/test_site.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     2838 2023-05-03 13:46:23.000000 django-gas-0.8.7/gas/tests/test_user_forms.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     1238 2023-05-03 13:46:23.000000 django-gas-0.8.7/gas/tests/test_utils.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)    15954 2023-05-03 13:46:23.000000 django-gas-0.8.7/gas/tests/test_views.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      133 2023-05-03 13:46:23.000000 django-gas-0.8.7/gas/tests/urls.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      545 2023-05-03 13:46:26.000000 django-gas-0.8.7/gas/utils.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)     9947 2023-05-03 13:46:26.000000 django-gas-0.8.7/gas/views.py
+-rw-r--r--   0 shagi     (1000) shagi     (1000)      868 2023-05-03 14:08:01.023626 django-gas-0.8.7/setup.cfg
+-rw-r--r--   0 shagi     (1000) shagi     (1000)       38 2023-05-03 13:46:27.000000 django-gas-0.8.7/setup.py
```

### Comparing `django-gas-0.8.6/LICENSE.txt` & `django-gas-0.8.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/PKG-INFO` & `django-gas-0.8.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-gas
-Version: 0.8.6
+Version: 0.8.7
 Summary: An alternative to django admin
 Home-page: https://git.negromate.rocks/shagi/gas
 Author: Ales (Shagi) Zabala Alava
 Author-email: shagi@gisa-elkartea.org
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -93,14 +93,19 @@
 
 The license of the code is GPLv3, but in the `gas/static/vendor` folder there
 is some external code with different licenses.
 
 Changelog
 =========
 
+0.8.7
+-----
+
+* Update jquery
+
 0.8.6
 -----
 
 * Allow overriding home url
 
 0.8.5
 -----
```

### Comparing `django-gas-0.8.6/django_gas.egg-info/PKG-INFO` & `django-gas-0.8.7/django_gas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-gas
-Version: 0.8.6
+Version: 0.8.7
 Summary: An alternative to django admin
 Home-page: https://git.negromate.rocks/shagi/gas
 Author: Ales (Shagi) Zabala Alava
 Author-email: shagi@gisa-elkartea.org
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -93,14 +93,19 @@
 
 The license of the code is GPLv3, but in the `gas/static/vendor` folder there
 is some external code with different licenses.
 
 Changelog
 =========
 
+0.8.7
+-----
+
+* Update jquery
+
 0.8.6
 -----
 
 * Allow overriding home url
 
 0.8.5
 -----
```

### Comparing `django-gas-0.8.6/gas/forms.py` & `django-gas-0.8.7/gas/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         required=old_field.required,
         help_text=old_field.help_text,
         initial=old_field.initial,
         validators=old_field.validators,
         localize=old_field.localize,
         disabled=old_field.disabled,
         input_date_formats=("%Y-%m-%d",),
-        input_time_formats=("%H:%M", "%H:%M"),
+        input_time_formats=("%H:%M",),
         widget=forms.SplitDateTimeWidget(
             date_format='%Y-%m-%d',
             time_format='%H:%M',
             time_attrs={'placeholder': '00:00'},
         ),
     )
     new_field.widget.widgets[0].input_type = 'date'
```

### Comparing `django-gas-0.8.6/gas/gas/core/views.py` & `django-gas-0.8.7/gas/gas/core/views.py`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/gas/users/forms.py` & `django-gas-0.8.7/gas/gas/users/forms.py`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/gas/users/views.py` & `django-gas-0.8.7/gas/gas/users/views.py`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/gas_settings.py` & `django-gas-0.8.7/gas/gas_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 MEDIA = getattr(settings, 'GAS_MEDIA', {
     'css': [
         'vendor/font-awesome/css/all.css',
         'vendor/select2/css/select2.css',
         'gas/css/gas.css',
     ],
     'js': [
-        'vendor/jquery/dist/jquery.min.js',
+        'vendor/jquery-3.6.4.min.js',
         'vendor/jquery.formset.js',
         'vendor/select2/js/select2.full.min.js',
         'gas/js/add_popups.js',
         'gas/js/gas.js',
     ],
 })
```

### Comparing `django-gas-0.8.6/gas/locale/es/LC_MESSAGES/django.mo` & `django-gas-0.8.7/gas/locale/es/LC_MESSAGES/django.mo`

 * *Files 13% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"PO-Revision-Date: 2023-05-03 16:01+0200\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -43,14 +43,17 @@
 
 msgid "Change your password"
 msgstr "Cambiar tu contraseña"
 
 msgid "Change {username} user password"
 msgstr "Cambiar la contraseña del usuario {username}"
 
+msgid "Close"
+msgstr "Cerrar"
+
 msgid "Create"
 msgstr "Crear"
 
 msgid "Create user"
 msgstr "Crear usuario"
 
 msgid "Delete"
@@ -113,15 +116,15 @@
 msgid "Summary"
 msgstr "Resumen"
 
 msgid "Update"
 msgstr "Actualizar"
 
 msgid "Update user"
-msgstr "Actulizar usuario"
+msgstr "Actualizar usuario"
 
 msgid "User created"
 msgstr "Usuario creado"
 
 msgid "User deleted"
 msgstr "Usuario borrado"
 
@@ -139,14 +142,17 @@
 
 msgid "Users with access to everithing inside control panel."
 msgstr "Usuarios con acceso a todo el panel de control."
 
 msgid "Users with access to gas control panel."
 msgstr "Usuarios con acceso al panel de control."
 
+msgid "lazy"
+msgstr "lazy"
+
 msgid "role"
 msgstr "rol"
 
 msgid "roles"
 msgstr "roles"
 
 msgid "user"
```

### Comparing `django-gas-0.8.6/gas/locale/es/LC_MESSAGES/django.po` & `django-gas-0.8.7/gas/locale/es/LC_MESSAGES/django.po`

 * *Files 14% similar despite different names*

```diff
@@ -4,225 +4,231 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-04-14 16:22+0000\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"POT-Creation-Date: 2023-02-07 10:45+0000\n"
+"PO-Revision-Date: 2023-05-03 16:01+0200\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: apps.py:8
+#: gas/apps.py:8
 msgid "GAS"
 msgstr "GAS"
 
-#: forms.py:25
+#: gas/forms.py:25
 msgid "roles"
 msgstr "roles"
 
-#: gas/config.py:6
+#: gas/gas/config.py:6
 msgid "Users with access to gas control panel."
 msgstr "Usuarios con acceso al panel de control."
 
-#: gas/config.py:7
+#: gas/gas/config.py:7
 msgid "Users with access to everithing inside control panel."
 msgstr "Usuarios con acceso a todo el panel de control."
 
-#: gas/config.py:14 gas/users/views.py:31 gas/users/views.py:39
-#: gas/users/views.py:49 gas/users/views.py:60 gas/users/views.py:96
-#: gas/users/views.py:108
-msgid "Users"
-msgstr "Usuarios"
-
-#: gas/core/views.py:21
+#: gas/gas/core/views.py:38
 msgid "Change your password"
 msgstr "Cambiar tu contraseña"
 
-#: gas/core/views.py:22
+#: gas/gas/core/views.py:39
 msgid "Password changed."
 msgstr "Contraseña cambiada."
 
-#: gas/users/forms.py:9 templates/gas/users/user_list.html:10
+#: gas/gas/users/forms.py:9 gas/templates/gas/users/user_list.html:10
 msgid "Username"
 msgstr "Usuario"
 
-#: gas/users/forms.py:10 templates/gas/users/user_list.html:11
+#: gas/gas/users/forms.py:10 gas/templates/gas/users/user_list.html:11
 msgid "Active"
 msgstr "Activo"
 
-#: gas/users/forms.py:12 templates/gas/users/user_list.html:12
+#: gas/gas/users/forms.py:12 gas/templates/gas/users/user_list.html:12
 msgid "Roles"
 msgstr "Roles"
 
-#: gas/users/views.py:32
+#: gas/gas/users/views.py:31 gas/gas/users/views.py:39
+#: gas/gas/users/views.py:49 gas/gas/users/views.py:60
+#: gas/gas/users/views.py:99 gas/gas/users/views.py:111
+#: gas/gas/users_config.py:9
+msgid "Users"
+msgstr "Usuarios"
+
+#: gas/gas/users/views.py:32
 msgid "Manage users and set roles."
 msgstr "Gestionar usuarios y asignar roles."
 
-#: gas/users/views.py:34
+#: gas/gas/users/views.py:34
 msgid "New user"
 msgstr "Nuevo usuario"
 
-#: gas/users/views.py:44
+#: gas/gas/users/views.py:44
 msgid "Create user"
 msgstr "Crear usuario"
 
-#: gas/users/views.py:45
+#: gas/gas/users/views.py:45
 msgid "User created"
 msgstr "Usuario creado"
 
-#: gas/users/views.py:50
+#: gas/gas/users/views.py:50
 msgid "Create"
 msgstr "Crear"
 
-#: gas/users/views.py:55
+#: gas/gas/users/views.py:55
 msgid "Update user"
 msgstr "Actualizar usuario"
 
-#: gas/users/views.py:56
+#: gas/gas/users/views.py:56
 msgid "User updated"
 msgstr "Usuario actualizado"
 
-#: gas/users/views.py:62
+#: gas/gas/users/views.py:62
 msgid "Update"
 msgstr "Actualizar"
 
-#: gas/users/views.py:69
+#: gas/gas/users/views.py:69
 msgid "User password updated"
 msgstr "Contraseña de usuario actualizada"
 
-#: gas/users/views.py:76
+#: gas/gas/users/views.py:76
 #, python-brace-format
 msgid "Change {username} user password"
 msgstr "Cambiar la contraseña del usuario {username}"
 
-#: gas/users/views.py:98 templates/gas/base.html:23
-#: templates/gas/users/user_list.html:29
+#: gas/gas/users/views.py:101 gas/templates/gas/base.html:23
+#: gas/templates/gas/users/user_list.html:29
 msgid "Change password"
 msgstr "Cambiar contraseña"
 
-#: gas/users/views.py:103
+#: gas/gas/users/views.py:106
 msgid "Delete user"
 msgstr "Borrar usuario"
 
-#: gas/users/views.py:104
+#: gas/gas/users/views.py:107
 msgid "User deleted"
 msgstr "Usuario borrado"
 
-#: gas/users/views.py:110 templates/gas/delete_confirmation.html:20
-#: templates/gas/users/user_list.html:30
+#: gas/gas/users/views.py:113 gas/templates/gas/delete_confirmation.html:25
+#: gas/templates/gas/users/user_list.html:30
 msgid "Delete"
 msgstr "Borrar"
 
-#: models.py:8
+#: gas/models.py:8
 msgid "role"
 msgstr "rol"
 
-#: models.py:10
+#: gas/models.py:10
 msgid "user"
 msgstr "usuario"
 
-#: models.py:14
+#: gas/models.py:14
 msgid "user role"
 msgstr "rol de usuario"
 
-#: models.py:15
+#: gas/models.py:15
 msgid "user roles"
 msgstr "roles de usuario"
 
-#: templates/gas/base.html:24
+#: gas/templates/gas/base.html:24
 msgid "Logout"
 msgstr "Salir"
 
-#: templates/gas/base.html:44
+#: gas/templates/gas/base.html:44 gas/templates/gas/tags/navigation.html:5
 msgid "Home"
 msgstr "Inicio"
 
-#: templates/gas/base.html:66
+#: gas/templates/gas/base.html:66
 msgid "Close"
 msgstr "Cerrar"
 
-#: templates/gas/base_form.html:23 templates/gas/delete_confirmation.html:21
+#: gas/templates/gas/base_form.html:26
+#: gas/templates/gas/delete_confirmation.html:26
 msgid "Cancel"
 msgstr "Cancelar"
 
-#: templates/gas/base_form.html:26
+#: gas/templates/gas/base_form.html:29
 msgid "Save"
 msgstr "Guardar"
 
-#: templates/gas/base_form.html:29
+#: gas/templates/gas/base_form.html:32
 msgid "Save and continue"
 msgstr "Guardar y continuar"
 
-#: templates/gas/base_list.html:14
+#: gas/templates/gas/base_list.html:14
 msgid "Filter"
 msgstr "Filtrar"
 
-#: templates/gas/delete_confirmation.html:5
+#: gas/templates/gas/delete_confirmation.html:6
 msgid "Delete confirmation"
 msgstr "Confirmación de borrado"
 
-#: templates/gas/delete_confirmation.html:10
+#: gas/templates/gas/delete_confirmation.html:13
 msgid "Summary"
 msgstr "Resumen"
 
-#: templates/gas/delete_confirmation.html:16
+#: gas/templates/gas/delete_confirmation.html:19
 msgid "Objects"
 msgstr "Objetos"
 
-#: templates/gas/login.html:6 templates/gas/login.html:15
+#: gas/templates/gas/login.html:6 gas/templates/gas/login.html:17
 msgid "Login"
 msgstr "Login"
 
-#: templates/gas/tags/pagination.html:9
+#: gas/templates/gas/tags/pagination.html:9
 msgid "Previous"
 msgstr "Anterior"
 
-#: templates/gas/tags/pagination.html:13
+#: gas/templates/gas/tags/pagination.html:13
 #, python-format
 msgid ""
 "\n"
 "            Page %(number)s of %(total)s\n"
 "            "
 msgstr ""
 "\n"
 "            Página %(number)s de %(total)s\n"
 "            "
 
-#: templates/gas/tags/pagination.html:18
+#: gas/templates/gas/tags/pagination.html:18
 msgid "Next"
 msgstr "Siguiente"
 
-#: templates/gas/tags/pagination.html:23
+#: gas/templates/gas/tags/pagination.html:23
 #, python-format
 msgid ""
 "\n"
 "        From %(start)s to %(end)s of %(total_objects)s total items.\n"
 "        "
 msgstr ""
 "\n"
 "        De %(start)s a %(end)s de un total de %(total_objects)s items.\n"
 "        "
 
-#: templates/gas/users/user_list.html:28
+#: gas/templates/gas/users/user_list.html:28
 msgid "Edit"
 msgstr "Editar"
 
-#: views.py:45
+#: gas/tests/test_utils.py:22
+msgid "lazy"
+msgstr "lazy"
+
+#: gas/views.py:82
 msgid "Operation successful."
 msgstr "Operación realizada."
 
-#: views.py:181
+#: gas/views.py:242
 #, python-brace-format
 msgid "Are you sure you want to delete {object}?"
 msgstr "¿Seguro que quieres borrar {object}?"
 
-#: views.py:182
+#: gas/views.py:243
 #, python-brace-format
 msgid "{object} deleted."
 msgstr "{object} borrado"
```

### Comparing `django-gas-0.8.6/gas/locale/eu/LC_MESSAGES/django.mo` & `django-gas-0.8.7/gas/locale/eu/LC_MESSAGES/django.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"PO-Revision-Date: 2023-05-03 16:01+0200\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -43,14 +43,17 @@
 
 msgid "Change your password"
 msgstr "Zure pasahitza aldatu"
 
 msgid "Change {username} user password"
 msgstr "Aldatu {username} erabiltzailearen pasahitza"
 
+msgid "Close"
+msgstr "Itxi"
+
 msgid "Create"
 msgstr "Sortu"
 
 msgid "Create user"
 msgstr "Erabiltzailea sortu"
 
 msgid "Delete"
@@ -64,14 +67,17 @@
 
 msgid "Edit"
 msgstr "Editatu"
 
 msgid "Filter"
 msgstr "Iragazi"
 
+msgid "GAS"
+msgstr "GAS"
+
 msgid "Home"
 msgstr "Hasiera"
 
 msgid "Login"
 msgstr "Sartu"
 
 msgid "Logout"
@@ -136,14 +142,17 @@
 
 msgid "Users with access to everithing inside control panel."
 msgstr "Kontrol panel guztian sartzeko baimena duten erabiltzaileak."
 
 msgid "Users with access to gas control panel."
 msgstr "Kontrol panelera sartzeko baimena duten erabiltzaileak."
 
+msgid "lazy"
+msgstr "lazy"
+
 msgid "role"
 msgstr "rola"
 
 msgid "roles"
 msgstr "rolak"
 
 msgid "user"
```

### Comparing `django-gas-0.8.6/gas/migrations/0001_initial.py` & `django-gas-0.8.7/gas/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/models.py` & `django-gas-0.8.7/gas/models.py`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/sites.py` & `django-gas-0.8.7/gas/sites.py`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/gas/css/gas.css` & `django-gas-0.8.7/gas/static/gas/css/gas.css`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/gas/css/img/logo.svg` & `django-gas-0.8.7/gas/static/gas/css/img/logo.svg`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/gas/js/add_popups.js` & `django-gas-0.8.7/gas/static/gas/js/add_popups.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/gas/js/gas.js` & `django-gas-0.8.7/gas/static/gas/js/gas.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/LICENSE.txt` & `django-gas-0.8.7/gas/static/vendor/font-awesome/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/css/all.css` & `django-gas-0.8.7/gas/static/vendor/font-awesome/css/all.css`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/css/all.min.css` & `django-gas-0.8.7/gas/static/vendor/font-awesome/css/all.min.css`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/css/brands.css` & `django-gas-0.8.7/gas/static/vendor/font-awesome/css/brands.css`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/css/brands.min.css` & `django-gas-0.8.7/gas/static/vendor/font-awesome/css/brands.min.css`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/css/fontawesome.css` & `django-gas-0.8.7/gas/static/vendor/font-awesome/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/css/fontawesome.min.css` & `django-gas-0.8.7/gas/static/vendor/font-awesome/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/css/regular.css` & `django-gas-0.8.7/gas/static/vendor/font-awesome/css/regular.css`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/css/regular.min.css` & `django-gas-0.8.7/gas/static/vendor/font-awesome/css/regular.min.css`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/css/solid.css` & `django-gas-0.8.7/gas/static/vendor/font-awesome/css/solid.css`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/css/solid.min.css` & `django-gas-0.8.7/gas/static/vendor/font-awesome/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/css/svg-with-js.css` & `django-gas-0.8.7/gas/static/vendor/font-awesome/css/svg-with-js.css`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/css/svg-with-js.min.css` & `django-gas-0.8.7/gas/static/vendor/font-awesome/css/svg-with-js.min.css`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/css/v4-shims.css` & `django-gas-0.8.7/gas/static/vendor/font-awesome/css/v4-shims.css`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/css/v4-shims.min.css` & `django-gas-0.8.7/gas/static/vendor/font-awesome/css/v4-shims.min.css`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/js/all.js` & `django-gas-0.8.7/gas/static/vendor/font-awesome/js/all.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/js/all.min.js` & `django-gas-0.8.7/gas/static/vendor/font-awesome/js/all.min.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/js/brands.js` & `django-gas-0.8.7/gas/static/vendor/font-awesome/js/brands.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/js/brands.min.js` & `django-gas-0.8.7/gas/static/vendor/font-awesome/js/brands.min.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/js/conflict-detection.js` & `django-gas-0.8.7/gas/static/vendor/font-awesome/js/conflict-detection.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/js/conflict-detection.min.js` & `django-gas-0.8.7/gas/static/vendor/font-awesome/js/conflict-detection.min.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/js/fontawesome.js` & `django-gas-0.8.7/gas/static/vendor/font-awesome/js/fontawesome.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/js/fontawesome.min.js` & `django-gas-0.8.7/gas/static/vendor/font-awesome/js/fontawesome.min.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/js/regular.js` & `django-gas-0.8.7/gas/static/vendor/font-awesome/js/regular.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/js/regular.min.js` & `django-gas-0.8.7/gas/static/vendor/font-awesome/js/regular.min.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/js/solid.js` & `django-gas-0.8.7/gas/static/vendor/font-awesome/js/solid.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/js/solid.min.js` & `django-gas-0.8.7/gas/static/vendor/font-awesome/js/solid.min.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/js/v4-shims.js` & `django-gas-0.8.7/gas/static/vendor/font-awesome/js/v4-shims.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/js/v4-shims.min.js` & `django-gas-0.8.7/gas/static/vendor/font-awesome/js/v4-shims.min.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-brands-400.eot` & `django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-brands-400.svg` & `django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-brands-400.ttf` & `django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-brands-400.woff` & `django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-brands-400.woff2` & `django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-regular-400.eot` & `django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-regular-400.svg` & `django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-regular-400.ttf` & `django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-regular-400.woff` & `django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-regular-400.woff2` & `django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-solid-900.eot` & `django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-solid-900.svg` & `django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-solid-900.ttf` & `django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-solid-900.woff` & `django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/font-awesome/webfonts/fa-solid-900.woff2` & `django-gas-0.8.7/gas/static/vendor/font-awesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/jquery/dist/jquery.min.js` & `django-gas-0.8.7/gas/static/vendor/jquery-3.6.4.min.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -1,3076 +1,3244 @@
-/*! jQuery v2.1.0 | (c) 2005, 2014 jQuery Foundation, Inc. | jquery.org/license */ ! function(a, b) {
-    "object" == typeof module && "object" == typeof module.exports ? module.exports = a.document ? b(a, !0) : function(a) {
-        if (!a.document) throw new Error("jQuery requires a window with a document");
-        return b(a)
-    } : b(a)
-}("undefined" != typeof window ? window : this, function(a, b) {
-    var c = [],
-        d = c.slice,
-        e = c.concat,
-        f = c.push,
-        g = c.indexOf,
-        h = {},
-        i = h.toString,
-        j = h.hasOwnProperty,
-        k = "".trim,
-        l = {},
-        m = a.document,
-        n = "2.1.0",
-        o = function(a, b) {
-            return new o.fn.init(a, b)
-        },
-        p = /^-ms-/,
-        q = /-([\da-z])/gi,
-        r = function(a, b) {
-            return b.toUpperCase()
+/*! jQuery v3.6.4 | (c) OpenJS Foundation and other contributors | jquery.org/license */ ! function(e, t) {
+    "use strict";
+    "object" == typeof module && "object" == typeof module.exports ? module.exports = e.document ? t(e, !0) : function(e) {
+        if (!e.document) throw new Error("jQuery requires a window with a document");
+        return t(e)
+    } : t(e)
+}("undefined" != typeof window ? window : this, function(C, e) {
+    "use strict";
+    var t = [],
+        r = Object.getPrototypeOf,
+        s = t.slice,
+        g = t.flat ? function(e) {
+            return t.flat.call(e)
+        } : function(e) {
+            return t.concat.apply([], e)
+        },
+        u = t.push,
+        i = t.indexOf,
+        n = {},
+        o = n.toString,
+        y = n.hasOwnProperty,
+        a = y.toString,
+        l = a.call(Object),
+        v = {},
+        m = function(e) {
+            return "function" == typeof e && "number" != typeof e.nodeType && "function" != typeof e.item
+        },
+        x = function(e) {
+            return null != e && e === e.window
+        },
+        E = C.document,
+        c = {
+            type: !0,
+            src: !0,
+            nonce: !0,
+            noModule: !0
         };
-    o.fn = o.prototype = {
-        jquery: n,
-        constructor: o,
-        selector: "",
+
+    function b(e, t, n) {
+        var r, i, o = (n = n || E).createElement("script");
+        if (o.text = e, t)
+            for (r in c)(i = t[r] || t.getAttribute && t.getAttribute(r)) && o.setAttribute(r, i);
+        n.head.appendChild(o).parentNode.removeChild(o)
+    }
+
+    function w(e) {
+        return null == e ? e + "" : "object" == typeof e || "function" == typeof e ? n[o.call(e)] || "object" : typeof e
+    }
+    var f = "3.6.4",
+        S = function(e, t) {
+            return new S.fn.init(e, t)
+        };
+
+    function p(e) {
+        var t = !!e && "length" in e && e.length,
+            n = w(e);
+        return !m(e) && !x(e) && ("array" === n || 0 === t || "number" == typeof t && 0 < t && t - 1 in e)
+    }
+    S.fn = S.prototype = {
+        jquery: f,
+        constructor: S,
         length: 0,
         toArray: function() {
-            return d.call(this)
+            return s.call(this)
         },
-        get: function(a) {
-            return null != a ? 0 > a ? this[a + this.length] : this[a] : d.call(this)
+        get: function(e) {
+            return null == e ? s.call(this) : e < 0 ? this[e + this.length] : this[e]
         },
-        pushStack: function(a) {
-            var b = o.merge(this.constructor(), a);
-            return b.prevObject = this, b.context = this.context, b
+        pushStack: function(e) {
+            var t = S.merge(this.constructor(), e);
+            return t.prevObject = this, t
         },
-        each: function(a, b) {
-            return o.each(this, a, b)
+        each: function(e) {
+            return S.each(this, e)
         },
-        map: function(a) {
-            return this.pushStack(o.map(this, function(b, c) {
-                return a.call(b, c, b)
+        map: function(n) {
+            return this.pushStack(S.map(this, function(e, t) {
+                return n.call(e, t, e)
             }))
         },
         slice: function() {
-            return this.pushStack(d.apply(this, arguments))
+            return this.pushStack(s.apply(this, arguments))
         },
         first: function() {
             return this.eq(0)
         },
         last: function() {
             return this.eq(-1)
         },
-        eq: function(a) {
-            var b = this.length,
-                c = +a + (0 > a ? b : 0);
-            return this.pushStack(c >= 0 && b > c ? [this[c]] : [])
+        even: function() {
+            return this.pushStack(S.grep(this, function(e, t) {
+                return (t + 1) % 2
+            }))
+        },
+        odd: function() {
+            return this.pushStack(S.grep(this, function(e, t) {
+                return t % 2
+            }))
+        },
+        eq: function(e) {
+            var t = this.length,
+                n = +e + (e < 0 ? t : 0);
+            return this.pushStack(0 <= n && n < t ? [this[n]] : [])
         },
         end: function() {
-            return this.prevObject || this.constructor(null)
+            return this.prevObject || this.constructor()
         },
-        push: f,
-        sort: c.sort,
-        splice: c.splice
-    }, o.extend = o.fn.extend = function() {
-        var a, b, c, d, e, f, g = arguments[0] || {},
-            h = 1,
-            i = arguments.length,
-            j = !1;
-        for ("boolean" == typeof g && (j = g, g = arguments[h] || {}, h++), "object" == typeof g || o.isFunction(g) || (g = {}), h === i && (g = this, h--); i > h; h++)
-            if (null != (a = arguments[h]))
-                for (b in a) c = g[b], d = a[b], g !== d && (j && d && (o.isPlainObject(d) || (e = o.isArray(d))) ? (e ? (e = !1, f = c && o.isArray(c) ? c : []) : f = c && o.isPlainObject(c) ? c : {}, g[b] = o.extend(j, f, d)) : void 0 !== d && (g[b] = d));
-        return g
-    }, o.extend({
-        expando: "jQuery" + (n + Math.random()).replace(/\D/g, ""),
+        push: u,
+        sort: t.sort,
+        splice: t.splice
+    }, S.extend = S.fn.extend = function() {
+        var e, t, n, r, i, o, a = arguments[0] || {},
+            s = 1,
+            u = arguments.length,
+            l = !1;
+        for ("boolean" == typeof a && (l = a, a = arguments[s] || {}, s++), "object" == typeof a || m(a) || (a = {}), s === u && (a = this, s--); s < u; s++)
+            if (null != (e = arguments[s]))
+                for (t in e) r = e[t], "__proto__" !== t && a !== r && (l && r && (S.isPlainObject(r) || (i = Array.isArray(r))) ? (n = a[t], o = i && !Array.isArray(n) ? [] : i || S.isPlainObject(n) ? n : {}, i = !1, a[t] = S.extend(l, o, r)) : void 0 !== r && (a[t] = r));
+        return a
+    }, S.extend({
+        expando: "jQuery" + (f + Math.random()).replace(/\D/g, ""),
         isReady: !0,
-        error: function(a) {
-            throw new Error(a)
+        error: function(e) {
+            throw new Error(e)
         },
         noop: function() {},
-        isFunction: function(a) {
-            return "function" === o.type(a)
-        },
-        isArray: Array.isArray,
-        isWindow: function(a) {
-            return null != a && a === a.window
-        },
-        isNumeric: function(a) {
-            return a - parseFloat(a) >= 0
-        },
-        isPlainObject: function(a) {
-            if ("object" !== o.type(a) || a.nodeType || o.isWindow(a)) return !1;
-            try {
-                if (a.constructor && !j.call(a.constructor.prototype, "isPrototypeOf")) return !1
-            } catch (b) {
-                return !1
-            }
-            return !0
-        },
-        isEmptyObject: function(a) {
-            var b;
-            for (b in a) return !1;
+        isPlainObject: function(e) {
+            var t, n;
+            return !(!e || "[object Object]" !== o.call(e)) && (!(t = r(e)) || "function" == typeof(n = y.call(t, "constructor") && t.constructor) && a.call(n) === l)
+        },
+        isEmptyObject: function(e) {
+            var t;
+            for (t in e) return !1;
             return !0
         },
-        type: function(a) {
-            return null == a ? a + "" : "object" == typeof a || "function" == typeof a ? h[i.call(a)] || "object" : typeof a
-        },
-        globalEval: function(a) {
-            var b, c = eval;
-            a = o.trim(a), a && (1 === a.indexOf("use strict") ? (b = m.createElement("script"), b.text = a, m.head.appendChild(b).parentNode.removeChild(b)) : c(a))
-        },
-        camelCase: function(a) {
-            return a.replace(p, "ms-").replace(q, r)
-        },
-        nodeName: function(a, b) {
-            return a.nodeName && a.nodeName.toLowerCase() === b.toLowerCase()
-        },
-        each: function(a, b, c) {
-            var d, e = 0,
-                f = a.length,
-                g = s(a);
-            if (c) {
-                if (g) {
-                    for (; f > e; e++)
-                        if (d = b.apply(a[e], c), d === !1) break
-                } else
-                    for (e in a)
-                        if (d = b.apply(a[e], c), d === !1) break
-            } else if (g) {
-                for (; f > e; e++)
-                    if (d = b.call(a[e], e, a[e]), d === !1) break
+        globalEval: function(e, t, n) {
+            b(e, {
+                nonce: t && t.nonce
+            }, n)
+        },
+        each: function(e, t) {
+            var n, r = 0;
+            if (p(e)) {
+                for (n = e.length; r < n; r++)
+                    if (!1 === t.call(e[r], r, e[r])) break
             } else
-                for (e in a)
-                    if (d = b.call(a[e], e, a[e]), d === !1) break;
-            return a
-        },
-        trim: function(a) {
-            return null == a ? "" : k.call(a)
-        },
-        makeArray: function(a, b) {
-            var c = b || [];
-            return null != a && (s(Object(a)) ? o.merge(c, "string" == typeof a ? [a] : a) : f.call(c, a)), c
-        },
-        inArray: function(a, b, c) {
-            return null == b ? -1 : g.call(b, a, c)
-        },
-        merge: function(a, b) {
-            for (var c = +b.length, d = 0, e = a.length; c > d; d++) a[e++] = b[d];
-            return a.length = e, a
-        },
-        grep: function(a, b, c) {
-            for (var d, e = [], f = 0, g = a.length, h = !c; g > f; f++) d = !b(a[f], f), d !== h && e.push(a[f]);
+                for (r in e)
+                    if (!1 === t.call(e[r], r, e[r])) break;
             return e
         },
-        map: function(a, b, c) {
-            var d, f = 0,
-                g = a.length,
-                h = s(a),
-                i = [];
-            if (h)
-                for (; g > f; f++) d = b(a[f], f, c), null != d && i.push(d);
+        makeArray: function(e, t) {
+            var n = t || [];
+            return null != e && (p(Object(e)) ? S.merge(n, "string" == typeof e ? [e] : e) : u.call(n, e)), n
+        },
+        inArray: function(e, t, n) {
+            return null == t ? -1 : i.call(t, e, n)
+        },
+        merge: function(e, t) {
+            for (var n = +t.length, r = 0, i = e.length; r < n; r++) e[i++] = t[r];
+            return e.length = i, e
+        },
+        grep: function(e, t, n) {
+            for (var r = [], i = 0, o = e.length, a = !n; i < o; i++) !t(e[i], i) !== a && r.push(e[i]);
+            return r
+        },
+        map: function(e, t, n) {
+            var r, i, o = 0,
+                a = [];
+            if (p(e))
+                for (r = e.length; o < r; o++) null != (i = t(e[o], o, n)) && a.push(i);
             else
-                for (f in a) d = b(a[f], f, c), null != d && i.push(d);
-            return e.apply([], i)
+                for (o in e) null != (i = t(e[o], o, n)) && a.push(i);
+            return g(a)
         },
         guid: 1,
-        proxy: function(a, b) {
-            var c, e, f;
-            return "string" == typeof b && (c = a[b], b = a, a = c), o.isFunction(a) ? (e = d.call(arguments, 2), f = function() {
-                return a.apply(b || this, e.concat(d.call(arguments)))
-            }, f.guid = a.guid = a.guid || o.guid++, f) : void 0
-        },
-        now: Date.now,
-        support: l
-    }), o.each("Boolean Number String Function Array Date RegExp Object Error".split(" "), function(a, b) {
-        h["[object " + b + "]"] = b.toLowerCase()
+        support: v
+    }), "function" == typeof Symbol && (S.fn[Symbol.iterator] = t[Symbol.iterator]), S.each("Boolean Number String Function Array Date RegExp Object Error Symbol".split(" "), function(e, t) {
+        n["[object " + t + "]"] = t.toLowerCase()
     });
-
-    function s(a) {
-        var b = a.length,
-            c = o.type(a);
-        return "function" === c || o.isWindow(a) ? !1 : 1 === a.nodeType && b ? !0 : "array" === c || 0 === b || "number" == typeof b && b > 0 && b - 1 in a
-    }
-    var t = function(a) {
-        var b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s = "sizzle" + -new Date,
-            t = a.document,
-            u = 0,
-            v = 0,
-            w = eb(),
-            x = eb(),
-            y = eb(),
-            z = function(a, b) {
-                return a === b && (j = !0), 0
-            },
-            A = "undefined",
-            B = 1 << 31,
-            C = {}.hasOwnProperty,
-            D = [],
-            E = D.pop,
-            F = D.push,
-            G = D.push,
-            H = D.slice,
-            I = D.indexOf || function(a) {
-                for (var b = 0, c = this.length; c > b; b++)
-                    if (this[b] === a) return b;
+    var d = function(n) {
+        var e, d, b, o, i, h, f, g, w, u, l, T, C, a, E, y, s, c, v, S = "sizzle" + 1 * new Date,
+            p = n.document,
+            k = 0,
+            r = 0,
+            m = ue(),
+            x = ue(),
+            A = ue(),
+            N = ue(),
+            j = function(e, t) {
+                return e === t && (l = !0), 0
+            },
+            D = {}.hasOwnProperty,
+            t = [],
+            q = t.pop,
+            L = t.push,
+            H = t.push,
+            O = t.slice,
+            P = function(e, t) {
+                for (var n = 0, r = e.length; n < r; n++)
+                    if (e[n] === t) return n;
                 return -1
             },
-            J = "checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|ismap|loop|multiple|open|readonly|required|scoped",
-            K = "[\\x20\\t\\r\\n\\f]",
-            L = "(?:\\\\.|[\\w-]|[^\\x00-\\xa0])+",
-            M = L.replace("w", "w#"),
-            N = "\\[" + K + "*(" + L + ")" + K + "*(?:([*^$|!~]?=)" + K + "*(?:(['\"])((?:\\\\.|[^\\\\])*?)\\3|(" + M + ")|)|)" + K + "*\\]",
-            O = ":(" + L + ")(?:\\(((['\"])((?:\\\\.|[^\\\\])*?)\\3|((?:\\\\.|[^\\\\()[\\]]|" + N.replace(3, 8) + ")*)|.*)\\)|)",
-            P = new RegExp("^" + K + "+|((?:^|[^\\\\])(?:\\\\.)*)" + K + "+$", "g"),
-            Q = new RegExp("^" + K + "*," + K + "*"),
-            R = new RegExp("^" + K + "*([>+~]|" + K + ")" + K + "*"),
-            S = new RegExp("=" + K + "*([^\\]'\"]*?)" + K + "*\\]", "g"),
-            T = new RegExp(O),
-            U = new RegExp("^" + M + "$"),
-            V = {
-                ID: new RegExp("^#(" + L + ")"),
-                CLASS: new RegExp("^\\.(" + L + ")"),
-                TAG: new RegExp("^(" + L.replace("w", "w*") + ")"),
-                ATTR: new RegExp("^" + N),
-                PSEUDO: new RegExp("^" + O),
-                CHILD: new RegExp("^:(only|first|last|nth|nth-last)-(child|of-type)(?:\\(" + K + "*(even|odd|(([+-]|)(\\d*)n|)" + K + "*(?:([+-]|)" + K + "*(\\d+)|))" + K + "*\\)|)", "i"),
-                bool: new RegExp("^(?:" + J + ")$", "i"),
-                needsContext: new RegExp("^" + K + "*[>+~]|:(even|odd|eq|gt|lt|nth|first|last)(?:\\(" + K + "*((?:-\\d)?\\d*)" + K + "*\\)|)(?=[^-]|$)", "i")
-            },
-            W = /^(?:input|select|textarea|button)$/i,
-            X = /^h\d$/i,
-            Y = /^[^{]+\{\s*\[native \w/,
+            R = "checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|ismap|loop|multiple|open|readonly|required|scoped",
+            M = "[\\x20\\t\\r\\n\\f]",
+            I = "(?:\\\\[\\da-fA-F]{1,6}" + M + "?|\\\\[^\\r\\n\\f]|[\\w-]|[^\0-\\x7f])+",
+            W = "\\[" + M + "*(" + I + ")(?:" + M + "*([*^$|!~]?=)" + M + "*(?:'((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\"|(" + I + "))|)" + M + "*\\]",
+            F = ":(" + I + ")(?:\\((('((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\")|((?:\\\\.|[^\\\\()[\\]]|" + W + ")*)|.*)\\)|)",
+            $ = new RegExp(M + "+", "g"),
+            B = new RegExp("^" + M + "+|((?:^|[^\\\\])(?:\\\\.)*)" + M + "+$", "g"),
+            _ = new RegExp("^" + M + "*," + M + "*"),
+            z = new RegExp("^" + M + "*([>+~]|" + M + ")" + M + "*"),
+            U = new RegExp(M + "|>"),
+            X = new RegExp(F),
+            V = new RegExp("^" + I + "$"),
+            G = {
+                ID: new RegExp("^#(" + I + ")"),
+                CLASS: new RegExp("^\\.(" + I + ")"),
+                TAG: new RegExp("^(" + I + "|[*])"),
+                ATTR: new RegExp("^" + W),
+                PSEUDO: new RegExp("^" + F),
+                CHILD: new RegExp("^:(only|first|last|nth|nth-last)-(child|of-type)(?:\\(" + M + "*(even|odd|(([+-]|)(\\d*)n|)" + M + "*(?:([+-]|)" + M + "*(\\d+)|))" + M + "*\\)|)", "i"),
+                bool: new RegExp("^(?:" + R + ")$", "i"),
+                needsContext: new RegExp("^" + M + "*[>+~]|:(even|odd|eq|gt|lt|nth|first|last)(?:\\(" + M + "*((?:-\\d)?\\d*)" + M + "*\\)|)(?=[^-]|$)", "i")
+            },
+            Y = /HTML$/i,
+            Q = /^(?:input|select|textarea|button)$/i,
+            J = /^h\d$/i,
+            K = /^[^{]+\{\s*\[native \w/,
             Z = /^(?:#([\w-]+)|(\w+)|\.([\w-]+))$/,
-            $ = /[+~]/,
-            _ = /'|\\/g,
-            ab = new RegExp("\\\\([\\da-f]{1,6}" + K + "?|(" + K + ")|.)", "ig"),
-            bb = function(a, b, c) {
-                var d = "0x" + b - 65536;
-                return d !== d || c ? b : 0 > d ? String.fromCharCode(d + 65536) : String.fromCharCode(d >> 10 | 55296, 1023 & d | 56320)
-            };
+            ee = /[+~]/,
+            te = new RegExp("\\\\[\\da-fA-F]{1,6}" + M + "?|\\\\([^\\r\\n\\f])", "g"),
+            ne = function(e, t) {
+                var n = "0x" + e.slice(1) - 65536;
+                return t || (n < 0 ? String.fromCharCode(n + 65536) : String.fromCharCode(n >> 10 | 55296, 1023 & n | 56320))
+            },
+            re = /([\0-\x1f\x7f]|^-?\d)|^-$|[^\0-\x1f\x7f-\uFFFF\w-]/g,
+            ie = function(e, t) {
+                return t ? "\0" === e ? "\ufffd" : e.slice(0, -1) + "\\" + e.charCodeAt(e.length - 1).toString(16) + " " : "\\" + e
+            },
+            oe = function() {
+                T()
+            },
+            ae = be(function(e) {
+                return !0 === e.disabled && "fieldset" === e.nodeName.toLowerCase()
+            }, {
+                dir: "parentNode",
+                next: "legend"
+            });
         try {
-            G.apply(D = H.call(t.childNodes), t.childNodes), D[t.childNodes.length].nodeType
-        } catch (cb) {
-            G = {
-                apply: D.length ? function(a, b) {
-                    F.apply(a, H.call(b))
-                } : function(a, b) {
-                    var c = a.length,
-                        d = 0;
-                    while (a[c++] = b[d++]);
-                    a.length = c - 1
+            H.apply(t = O.call(p.childNodes), p.childNodes), t[p.childNodes.length].nodeType
+        } catch (e) {
+            H = {
+                apply: t.length ? function(e, t) {
+                    L.apply(e, O.call(t))
+                } : function(e, t) {
+                    var n = e.length,
+                        r = 0;
+                    while (e[n++] = t[r++]);
+                    e.length = n - 1
                 }
             }
         }
 
-        function db(a, b, d, e) {
-            var f, g, h, i, j, m, p, q, u, v;
-            if ((b ? b.ownerDocument || b : t) !== l && k(b), b = b || l, d = d || [], !a || "string" != typeof a) return d;
-            if (1 !== (i = b.nodeType) && 9 !== i) return [];
-            if (n && !e) {
-                if (f = Z.exec(a))
-                    if (h = f[1]) {
-                        if (9 === i) {
-                            if (g = b.getElementById(h), !g || !g.parentNode) return d;
-                            if (g.id === h) return d.push(g), d
-                        } else if (b.ownerDocument && (g = b.ownerDocument.getElementById(h)) && r(b, g) && g.id === h) return d.push(g), d
+        function se(t, e, n, r) {
+            var i, o, a, s, u, l, c, f = e && e.ownerDocument,
+                p = e ? e.nodeType : 9;
+            if (n = n || [], "string" != typeof t || !t || 1 !== p && 9 !== p && 11 !== p) return n;
+            if (!r && (T(e), e = e || C, E)) {
+                if (11 !== p && (u = Z.exec(t)))
+                    if (i = u[1]) {
+                        if (9 === p) {
+                            if (!(a = e.getElementById(i))) return n;
+                            if (a.id === i) return n.push(a), n
+                        } else if (f && (a = f.getElementById(i)) && v(e, a) && a.id === i) return n.push(a), n
                     } else {
-                        if (f[2]) return G.apply(d, b.getElementsByTagName(a)), d;
-                        if ((h = f[3]) && c.getElementsByClassName && b.getElementsByClassName) return G.apply(d, b.getElementsByClassName(h)), d
-                    } if (c.qsa && (!o || !o.test(a))) {
-                    if (q = p = s, u = b, v = 9 === i && a, 1 === i && "object" !== b.nodeName.toLowerCase()) {
-                        m = ob(a), (p = b.getAttribute("id")) ? q = p.replace(_, "\\$&") : b.setAttribute("id", q), q = "[id='" + q + "'] ", j = m.length;
-                        while (j--) m[j] = q + pb(m[j]);
-                        u = $.test(a) && mb(b.parentNode) || b, v = m.join(",")
+                        if (u[2]) return H.apply(n, e.getElementsByTagName(t)), n;
+                        if ((i = u[3]) && d.getElementsByClassName && e.getElementsByClassName) return H.apply(n, e.getElementsByClassName(i)), n
+                    } if (d.qsa && !N[t + " "] && (!y || !y.test(t)) && (1 !== p || "object" !== e.nodeName.toLowerCase())) {
+                    if (c = t, f = e, 1 === p && (U.test(t) || z.test(t))) {
+                        (f = ee.test(t) && ve(e.parentNode) || e) === e && d.scope || ((s = e.getAttribute("id")) ? s = s.replace(re, ie) : e.setAttribute("id", s = S)), o = (l = h(t)).length;
+                        while (o--) l[o] = (s ? "#" + s : ":scope") + " " + xe(l[o]);
+                        c = l.join(",")
                     }
-                    if (v) try {
-                        return G.apply(d, u.querySelectorAll(v)), d
-                    } catch (w) {} finally {
-                        p || b.removeAttribute("id")
+                    try {
+                        return H.apply(n, f.querySelectorAll(c)), n
+                    } catch (e) {
+                        N(t, !0)
+                    } finally {
+                        s === S && e.removeAttribute("id")
                     }
                 }
             }
-            return xb(a.replace(P, "$1"), b, d, e)
+            return g(t.replace(B, "$1"), e, n, r)
         }
 
-        function eb() {
-            var a = [];
-
-            function b(c, e) {
-                return a.push(c + " ") > d.cacheLength && delete b[a.shift()], b[c + " "] = e
+        function ue() {
+            var r = [];
+            return function e(t, n) {
+                return r.push(t + " ") > b.cacheLength && delete e[r.shift()], e[t + " "] = n
             }
-            return b
         }
 
-        function fb(a) {
-            return a[s] = !0, a
+        function le(e) {
+            return e[S] = !0, e
         }
 
-        function gb(a) {
-            var b = l.createElement("div");
+        function ce(e) {
+            var t = C.createElement("fieldset");
             try {
-                return !!a(b)
-            } catch (c) {
+                return !!e(t)
+            } catch (e) {
                 return !1
             } finally {
-                b.parentNode && b.parentNode.removeChild(b), b = null
+                t.parentNode && t.parentNode.removeChild(t), t = null
             }
         }
 
-        function hb(a, b) {
-            var c = a.split("|"),
-                e = a.length;
-            while (e--) d.attrHandle[c[e]] = b
+        function fe(e, t) {
+            var n = e.split("|"),
+                r = n.length;
+            while (r--) b.attrHandle[n[r]] = t
         }
 
-        function ib(a, b) {
-            var c = b && a,
-                d = c && 1 === a.nodeType && 1 === b.nodeType && (~b.sourceIndex || B) - (~a.sourceIndex || B);
-            if (d) return d;
-            if (c)
-                while (c = c.nextSibling)
-                    if (c === b) return -1;
-            return a ? 1 : -1
+        function pe(e, t) {
+            var n = t && e,
+                r = n && 1 === e.nodeType && 1 === t.nodeType && e.sourceIndex - t.sourceIndex;
+            if (r) return r;
+            if (n)
+                while (n = n.nextSibling)
+                    if (n === t) return -1;
+            return e ? 1 : -1
         }
 
-        function jb(a) {
-            return function(b) {
-                var c = b.nodeName.toLowerCase();
-                return "input" === c && b.type === a
+        function de(t) {
+            return function(e) {
+                return "input" === e.nodeName.toLowerCase() && e.type === t
             }
         }
 
-        function kb(a) {
-            return function(b) {
-                var c = b.nodeName.toLowerCase();
-                return ("input" === c || "button" === c) && b.type === a
+        function he(n) {
+            return function(e) {
+                var t = e.nodeName.toLowerCase();
+                return ("input" === t || "button" === t) && e.type === n
             }
         }
 
-        function lb(a) {
-            return fb(function(b) {
-                return b = +b, fb(function(c, d) {
-                    var e, f = a([], c.length, b),
-                        g = f.length;
-                    while (g--) c[e = f[g]] && (c[e] = !(d[e] = c[e]))
+        function ge(t) {
+            return function(e) {
+                return "form" in e ? e.parentNode && !1 === e.disabled ? "label" in e ? "label" in e.parentNode ? e.parentNode.disabled === t : e.disabled === t : e.isDisabled === t || e.isDisabled !== !t && ae(e) === t : e.disabled === t : "label" in e && e.disabled === t
+            }
+        }
+
+        function ye(a) {
+            return le(function(o) {
+                return o = +o, le(function(e, t) {
+                    var n, r = a([], e.length, o),
+                        i = r.length;
+                    while (i--) e[n = r[i]] && (e[n] = !(t[n] = e[n]))
                 })
             })
         }
 
-        function mb(a) {
-            return a && typeof a.getElementsByTagName !== A && a
+        function ve(e) {
+            return e && "undefined" != typeof e.getElementsByTagName && e
         }
-        c = db.support = {}, f = db.isXML = function(a) {
-            var b = a && (a.ownerDocument || a).documentElement;
-            return b ? "HTML" !== b.nodeName : !1
-        }, k = db.setDocument = function(a) {
-            var b, e = a ? a.ownerDocument || a : t,
-                g = e.defaultView;
-            return e !== l && 9 === e.nodeType && e.documentElement ? (l = e, m = e.documentElement, n = !f(e), g && g !== g.top && (g.addEventListener ? g.addEventListener("unload", function() {
-                k()
-            }, !1) : g.attachEvent && g.attachEvent("onunload", function() {
-                k()
-            })), c.attributes = gb(function(a) {
-                return a.className = "i", !a.getAttribute("className")
-            }), c.getElementsByTagName = gb(function(a) {
-                return a.appendChild(e.createComment("")), !a.getElementsByTagName("*").length
-            }), c.getElementsByClassName = Y.test(e.getElementsByClassName) && gb(function(a) {
-                return a.innerHTML = "<div class='a'></div><div class='a i'></div>", a.firstChild.className = "i", 2 === a.getElementsByClassName("i").length
-            }), c.getById = gb(function(a) {
-                return m.appendChild(a).id = s, !e.getElementsByName || !e.getElementsByName(s).length
-            }), c.getById ? (d.find.ID = function(a, b) {
-                if (typeof b.getElementById !== A && n) {
-                    var c = b.getElementById(a);
-                    return c && c.parentNode ? [c] : []
-                }
-            }, d.filter.ID = function(a) {
-                var b = a.replace(ab, bb);
-                return function(a) {
-                    return a.getAttribute("id") === b
-                }
-            }) : (delete d.find.ID, d.filter.ID = function(a) {
-                var b = a.replace(ab, bb);
-                return function(a) {
-                    var c = typeof a.getAttributeNode !== A && a.getAttributeNode("id");
-                    return c && c.value === b
-                }
-            }), d.find.TAG = c.getElementsByTagName ? function(a, b) {
-                return typeof b.getElementsByTagName !== A ? b.getElementsByTagName(a) : void 0
-            } : function(a, b) {
-                var c, d = [],
-                    e = 0,
-                    f = b.getElementsByTagName(a);
-                if ("*" === a) {
-                    while (c = f[e++]) 1 === c.nodeType && d.push(c);
-                    return d
-                }
-                return f
-            }, d.find.CLASS = c.getElementsByClassName && function(a, b) {
-                return typeof b.getElementsByClassName !== A && n ? b.getElementsByClassName(a) : void 0
-            }, p = [], o = [], (c.qsa = Y.test(e.querySelectorAll)) && (gb(function(a) {
-                a.innerHTML = "<select t=''><option selected=''></option></select>", a.querySelectorAll("[t^='']").length && o.push("[*^$]=" + K + "*(?:''|\"\")"), a.querySelectorAll("[selected]").length || o.push("\\[" + K + "*(?:value|" + J + ")"), a.querySelectorAll(":checked").length || o.push(":checked")
-            }), gb(function(a) {
-                var b = e.createElement("input");
-                b.setAttribute("type", "hidden"), a.appendChild(b).setAttribute("name", "D"), a.querySelectorAll("[name=d]").length && o.push("name" + K + "*[*^$|!~]?="), a.querySelectorAll(":enabled").length || o.push(":enabled", ":disabled"), a.querySelectorAll("*,:x"), o.push(",.*:")
-            })), (c.matchesSelector = Y.test(q = m.webkitMatchesSelector || m.mozMatchesSelector || m.oMatchesSelector || m.msMatchesSelector)) && gb(function(a) {
-                c.disconnectedMatch = q.call(a, "div"), q.call(a, "[s!='']:x"), p.push("!=", O)
-            }), o = o.length && new RegExp(o.join("|")), p = p.length && new RegExp(p.join("|")), b = Y.test(m.compareDocumentPosition), r = b || Y.test(m.contains) ? function(a, b) {
-                var c = 9 === a.nodeType ? a.documentElement : a,
-                    d = b && b.parentNode;
-                return a === d || !(!d || 1 !== d.nodeType || !(c.contains ? c.contains(d) : a.compareDocumentPosition && 16 & a.compareDocumentPosition(d)))
-            } : function(a, b) {
-                if (b)
-                    while (b = b.parentNode)
-                        if (b === a) return !0;
-                return !1
-            }, z = b ? function(a, b) {
-                if (a === b) return j = !0, 0;
-                var d = !a.compareDocumentPosition - !b.compareDocumentPosition;
-                return d ? d : (d = (a.ownerDocument || a) === (b.ownerDocument || b) ? a.compareDocumentPosition(b) : 1, 1 & d || !c.sortDetached && b.compareDocumentPosition(a) === d ? a === e || a.ownerDocument === t && r(t, a) ? -1 : b === e || b.ownerDocument === t && r(t, b) ? 1 : i ? I.call(i, a) - I.call(i, b) : 0 : 4 & d ? -1 : 1)
-            } : function(a, b) {
-                if (a === b) return j = !0, 0;
-                var c, d = 0,
-                    f = a.parentNode,
-                    g = b.parentNode,
-                    h = [a],
-                    k = [b];
-                if (!f || !g) return a === e ? -1 : b === e ? 1 : f ? -1 : g ? 1 : i ? I.call(i, a) - I.call(i, b) : 0;
-                if (f === g) return ib(a, b);
-                c = a;
-                while (c = c.parentNode) h.unshift(c);
-                c = b;
-                while (c = c.parentNode) k.unshift(c);
-                while (h[d] === k[d]) d++;
-                return d ? ib(h[d], k[d]) : h[d] === t ? -1 : k[d] === t ? 1 : 0
-            }, e) : l
-        }, db.matches = function(a, b) {
-            return db(a, null, null, b)
-        }, db.matchesSelector = function(a, b) {
-            if ((a.ownerDocument || a) !== l && k(a), b = b.replace(S, "='$1']"), !(!c.matchesSelector || !n || p && p.test(b) || o && o.test(b))) try {
-                var d = q.call(a, b);
-                if (d || c.disconnectedMatch || a.document && 11 !== a.document.nodeType) return d
-            } catch (e) {}
-            return db(b, l, null, [a]).length > 0
-        }, db.contains = function(a, b) {
-            return (a.ownerDocument || a) !== l && k(a), r(a, b)
-        }, db.attr = function(a, b) {
-            (a.ownerDocument || a) !== l && k(a);
-            var e = d.attrHandle[b.toLowerCase()],
-                f = e && C.call(d.attrHandle, b.toLowerCase()) ? e(a, b, !n) : void 0;
-            return void 0 !== f ? f : c.attributes || !n ? a.getAttribute(b) : (f = a.getAttributeNode(b)) && f.specified ? f.value : null
-        }, db.error = function(a) {
-            throw new Error("Syntax error, unrecognized expression: " + a)
-        }, db.uniqueSort = function(a) {
-            var b, d = [],
-                e = 0,
-                f = 0;
-            if (j = !c.detectDuplicates, i = !c.sortStable && a.slice(0), a.sort(z), j) {
-                while (b = a[f++]) b === a[f] && (e = d.push(f));
-                while (e--) a.splice(d[e], 1)
-            }
-            return i = null, a
-        }, e = db.getText = function(a) {
-            var b, c = "",
-                d = 0,
-                f = a.nodeType;
-            if (f) {
-                if (1 === f || 9 === f || 11 === f) {
-                    if ("string" == typeof a.textContent) return a.textContent;
-                    for (a = a.firstChild; a; a = a.nextSibling) c += e(a)
-                } else if (3 === f || 4 === f) return a.nodeValue
-            } else
-                while (b = a[d++]) c += e(b);
-            return c
-        }, d = db.selectors = {
-            cacheLength: 50,
-            createPseudo: fb,
-            match: V,
-            attrHandle: {},
-            find: {},
-            relative: {
-                ">": {
-                    dir: "parentNode",
-                    first: !0
-                },
-                " ": {
-                    dir: "parentNode"
-                },
-                "+": {
-                    dir: "previousSibling",
-                    first: !0
-                },
-                "~": {
-                    dir: "previousSibling"
-                }
-            },
-            preFilter: {
-                ATTR: function(a) {
-                    return a[1] = a[1].replace(ab, bb), a[3] = (a[4] || a[5] || "").replace(ab, bb), "~=" === a[2] && (a[3] = " " + a[3] + " "), a.slice(0, 4)
-                },
-                CHILD: function(a) {
-                    return a[1] = a[1].toLowerCase(), "nth" === a[1].slice(0, 3) ? (a[3] || db.error(a[0]), a[4] = +(a[4] ? a[5] + (a[6] || 1) : 2 * ("even" === a[3] || "odd" === a[3])), a[5] = +(a[7] + a[8] || "odd" === a[3])) : a[3] && db.error(a[0]), a
-                },
-                PSEUDO: function(a) {
-                    var b, c = !a[5] && a[2];
-                    return V.CHILD.test(a[0]) ? null : (a[3] && void 0 !== a[4] ? a[2] = a[4] : c && T.test(c) && (b = ob(c, !0)) && (b = c.indexOf(")", c.length - b) - c.length) && (a[0] = a[0].slice(0, b), a[2] = c.slice(0, b)), a.slice(0, 3))
-                }
-            },
-            filter: {
-                TAG: function(a) {
-                    var b = a.replace(ab, bb).toLowerCase();
-                    return "*" === a ? function() {
+        for (e in d = se.support = {}, i = se.isXML = function(e) {
+                var t = e && e.namespaceURI,
+                    n = e && (e.ownerDocument || e).documentElement;
+                return !Y.test(t || n && n.nodeName || "HTML")
+            }, T = se.setDocument = function(e) {
+                var t, n, r = e ? e.ownerDocument || e : p;
+                return r != C && 9 === r.nodeType && r.documentElement && (a = (C = r).documentElement, E = !i(C), p != C && (n = C.defaultView) && n.top !== n && (n.addEventListener ? n.addEventListener("unload", oe, !1) : n.attachEvent && n.attachEvent("onunload", oe)), d.scope = ce(function(e) {
+                    return a.appendChild(e).appendChild(C.createElement("div")), "undefined" != typeof e.querySelectorAll && !e.querySelectorAll(":scope fieldset div").length
+                }), d.cssHas = ce(function() {
+                    try {
+                        return C.querySelector(":has(*,:jqfake)"), !1
+                    } catch (e) {
                         return !0
-                    } : function(a) {
-                        return a.nodeName && a.nodeName.toLowerCase() === b
+                    }
+                }), d.attributes = ce(function(e) {
+                    return e.className = "i", !e.getAttribute("className")
+                }), d.getElementsByTagName = ce(function(e) {
+                    return e.appendChild(C.createComment("")), !e.getElementsByTagName("*").length
+                }), d.getElementsByClassName = K.test(C.getElementsByClassName), d.getById = ce(function(e) {
+                    return a.appendChild(e).id = S, !C.getElementsByName || !C.getElementsByName(S).length
+                }), d.getById ? (b.filter.ID = function(e) {
+                    var t = e.replace(te, ne);
+                    return function(e) {
+                        return e.getAttribute("id") === t
+                    }
+                }, b.find.ID = function(e, t) {
+                    if ("undefined" != typeof t.getElementById && E) {
+                        var n = t.getElementById(e);
+                        return n ? [n] : []
+                    }
+                }) : (b.filter.ID = function(e) {
+                    var n = e.replace(te, ne);
+                    return function(e) {
+                        var t = "undefined" != typeof e.getAttributeNode && e.getAttributeNode("id");
+                        return t && t.value === n
+                    }
+                }, b.find.ID = function(e, t) {
+                    if ("undefined" != typeof t.getElementById && E) {
+                        var n, r, i, o = t.getElementById(e);
+                        if (o) {
+                            if ((n = o.getAttributeNode("id")) && n.value === e) return [o];
+                            i = t.getElementsByName(e), r = 0;
+                            while (o = i[r++])
+                                if ((n = o.getAttributeNode("id")) && n.value === e) return [o]
+                        }
+                        return []
+                    }
+                }), b.find.TAG = d.getElementsByTagName ? function(e, t) {
+                    return "undefined" != typeof t.getElementsByTagName ? t.getElementsByTagName(e) : d.qsa ? t.querySelectorAll(e) : void 0
+                } : function(e, t) {
+                    var n, r = [],
+                        i = 0,
+                        o = t.getElementsByTagName(e);
+                    if ("*" === e) {
+                        while (n = o[i++]) 1 === n.nodeType && r.push(n);
+                        return r
+                    }
+                    return o
+                }, b.find.CLASS = d.getElementsByClassName && function(e, t) {
+                    if ("undefined" != typeof t.getElementsByClassName && E) return t.getElementsByClassName(e)
+                }, s = [], y = [], (d.qsa = K.test(C.querySelectorAll)) && (ce(function(e) {
+                    var t;
+                    a.appendChild(e).innerHTML = "<a id='" + S + "'></a><select id='" + S + "-\r\\' msallowcapture=''><option selected=''></option></select>", e.querySelectorAll("[msallowcapture^='']").length && y.push("[*^$]=" + M + "*(?:''|\"\")"), e.querySelectorAll("[selected]").length || y.push("\\[" + M + "*(?:value|" + R + ")"), e.querySelectorAll("[id~=" + S + "-]").length || y.push("~="), (t = C.createElement("input")).setAttribute("name", ""), e.appendChild(t), e.querySelectorAll("[name='']").length || y.push("\\[" + M + "*name" + M + "*=" + M + "*(?:''|\"\")"), e.querySelectorAll(":checked").length || y.push(":checked"), e.querySelectorAll("a#" + S + "+*").length || y.push(".#.+[+~]"), e.querySelectorAll("\\\f"), y.push("[\\r\\n\\f]")
+                }), ce(function(e) {
+                    e.innerHTML = "<a href='' disabled='disabled'></a><select disabled='disabled'><option/></select>";
+                    var t = C.createElement("input");
+                    t.setAttribute("type", "hidden"), e.appendChild(t).setAttribute("name", "D"), e.querySelectorAll("[name=d]").length && y.push("name" + M + "*[*^$|!~]?="), 2 !== e.querySelectorAll(":enabled").length && y.push(":enabled", ":disabled"), a.appendChild(e).disabled = !0, 2 !== e.querySelectorAll(":disabled").length && y.push(":enabled", ":disabled"), e.querySelectorAll("*,:x"), y.push(",.*:")
+                })), (d.matchesSelector = K.test(c = a.matches || a.webkitMatchesSelector || a.mozMatchesSelector || a.oMatchesSelector || a.msMatchesSelector)) && ce(function(e) {
+                    d.disconnectedMatch = c.call(e, "*"), c.call(e, "[s!='']:x"), s.push("!=", F)
+                }), d.cssHas || y.push(":has"), y = y.length && new RegExp(y.join("|")), s = s.length && new RegExp(s.join("|")), t = K.test(a.compareDocumentPosition), v = t || K.test(a.contains) ? function(e, t) {
+                    var n = 9 === e.nodeType && e.documentElement || e,
+                        r = t && t.parentNode;
+                    return e === r || !(!r || 1 !== r.nodeType || !(n.contains ? n.contains(r) : e.compareDocumentPosition && 16 & e.compareDocumentPosition(r)))
+                } : function(e, t) {
+                    if (t)
+                        while (t = t.parentNode)
+                            if (t === e) return !0;
+                    return !1
+                }, j = t ? function(e, t) {
+                    if (e === t) return l = !0, 0;
+                    var n = !e.compareDocumentPosition - !t.compareDocumentPosition;
+                    return n || (1 & (n = (e.ownerDocument || e) == (t.ownerDocument || t) ? e.compareDocumentPosition(t) : 1) || !d.sortDetached && t.compareDocumentPosition(e) === n ? e == C || e.ownerDocument == p && v(p, e) ? -1 : t == C || t.ownerDocument == p && v(p, t) ? 1 : u ? P(u, e) - P(u, t) : 0 : 4 & n ? -1 : 1)
+                } : function(e, t) {
+                    if (e === t) return l = !0, 0;
+                    var n, r = 0,
+                        i = e.parentNode,
+                        o = t.parentNode,
+                        a = [e],
+                        s = [t];
+                    if (!i || !o) return e == C ? -1 : t == C ? 1 : i ? -1 : o ? 1 : u ? P(u, e) - P(u, t) : 0;
+                    if (i === o) return pe(e, t);
+                    n = e;
+                    while (n = n.parentNode) a.unshift(n);
+                    n = t;
+                    while (n = n.parentNode) s.unshift(n);
+                    while (a[r] === s[r]) r++;
+                    return r ? pe(a[r], s[r]) : a[r] == p ? -1 : s[r] == p ? 1 : 0
+                }), C
+            }, se.matches = function(e, t) {
+                return se(e, null, null, t)
+            }, se.matchesSelector = function(e, t) {
+                if (T(e), d.matchesSelector && E && !N[t + " "] && (!s || !s.test(t)) && (!y || !y.test(t))) try {
+                    var n = c.call(e, t);
+                    if (n || d.disconnectedMatch || e.document && 11 !== e.document.nodeType) return n
+                } catch (e) {
+                    N(t, !0)
+                }
+                return 0 < se(t, C, null, [e]).length
+            }, se.contains = function(e, t) {
+                return (e.ownerDocument || e) != C && T(e), v(e, t)
+            }, se.attr = function(e, t) {
+                (e.ownerDocument || e) != C && T(e);
+                var n = b.attrHandle[t.toLowerCase()],
+                    r = n && D.call(b.attrHandle, t.toLowerCase()) ? n(e, t, !E) : void 0;
+                return void 0 !== r ? r : d.attributes || !E ? e.getAttribute(t) : (r = e.getAttributeNode(t)) && r.specified ? r.value : null
+            }, se.escape = function(e) {
+                return (e + "").replace(re, ie)
+            }, se.error = function(e) {
+                throw new Error("Syntax error, unrecognized expression: " + e)
+            }, se.uniqueSort = function(e) {
+                var t, n = [],
+                    r = 0,
+                    i = 0;
+                if (l = !d.detectDuplicates, u = !d.sortStable && e.slice(0), e.sort(j), l) {
+                    while (t = e[i++]) t === e[i] && (r = n.push(i));
+                    while (r--) e.splice(n[r], 1)
+                }
+                return u = null, e
+            }, o = se.getText = function(e) {
+                var t, n = "",
+                    r = 0,
+                    i = e.nodeType;
+                if (i) {
+                    if (1 === i || 9 === i || 11 === i) {
+                        if ("string" == typeof e.textContent) return e.textContent;
+                        for (e = e.firstChild; e; e = e.nextSibling) n += o(e)
+                    } else if (3 === i || 4 === i) return e.nodeValue
+                } else
+                    while (t = e[r++]) n += o(t);
+                return n
+            }, (b = se.selectors = {
+                cacheLength: 50,
+                createPseudo: le,
+                match: G,
+                attrHandle: {},
+                find: {},
+                relative: {
+                    ">": {
+                        dir: "parentNode",
+                        first: !0
+                    },
+                    " ": {
+                        dir: "parentNode"
+                    },
+                    "+": {
+                        dir: "previousSibling",
+                        first: !0
+                    },
+                    "~": {
+                        dir: "previousSibling"
                     }
                 },
-                CLASS: function(a) {
-                    var b = w[a + " "];
-                    return b || (b = new RegExp("(^|" + K + ")" + a + "(" + K + "|$)")) && w(a, function(a) {
-                        return b.test("string" == typeof a.className && a.className || typeof a.getAttribute !== A && a.getAttribute("class") || "")
-                    })
-                },
-                ATTR: function(a, b, c) {
-                    return function(d) {
-                        var e = db.attr(d, a);
-                        return null == e ? "!=" === b : b ? (e += "", "=" === b ? e === c : "!=" === b ? e !== c : "^=" === b ? c && 0 === e.indexOf(c) : "*=" === b ? c && e.indexOf(c) > -1 : "$=" === b ? c && e.slice(-c.length) === c : "~=" === b ? (" " + e + " ").indexOf(c) > -1 : "|=" === b ? e === c || e.slice(0, c.length + 1) === c + "-" : !1) : !0
+                preFilter: {
+                    ATTR: function(e) {
+                        return e[1] = e[1].replace(te, ne), e[3] = (e[3] || e[4] || e[5] || "").replace(te, ne), "~=" === e[2] && (e[3] = " " + e[3] + " "), e.slice(0, 4)
+                    },
+                    CHILD: function(e) {
+                        return e[1] = e[1].toLowerCase(), "nth" === e[1].slice(0, 3) ? (e[3] || se.error(e[0]), e[4] = +(e[4] ? e[5] + (e[6] || 1) : 2 * ("even" === e[3] || "odd" === e[3])), e[5] = +(e[7] + e[8] || "odd" === e[3])) : e[3] && se.error(e[0]), e
+                    },
+                    PSEUDO: function(e) {
+                        var t, n = !e[6] && e[2];
+                        return G.CHILD.test(e[0]) ? null : (e[3] ? e[2] = e[4] || e[5] || "" : n && X.test(n) && (t = h(n, !0)) && (t = n.indexOf(")", n.length - t) - n.length) && (e[0] = e[0].slice(0, t), e[2] = n.slice(0, t)), e.slice(0, 3))
                     }
                 },
-                CHILD: function(a, b, c, d, e) {
-                    var f = "nth" !== a.slice(0, 3),
-                        g = "last" !== a.slice(-4),
-                        h = "of-type" === b;
-                    return 1 === d && 0 === e ? function(a) {
-                        return !!a.parentNode
-                    } : function(b, c, i) {
-                        var j, k, l, m, n, o, p = f !== g ? "nextSibling" : "previousSibling",
-                            q = b.parentNode,
-                            r = h && b.nodeName.toLowerCase(),
-                            t = !i && !h;
-                        if (q) {
-                            if (f) {
-                                while (p) {
-                                    l = b;
-                                    while (l = l[p])
-                                        if (h ? l.nodeName.toLowerCase() === r : 1 === l.nodeType) return !1;
-                                    o = p = "only" === a && !o && "nextSibling"
+                filter: {
+                    TAG: function(e) {
+                        var t = e.replace(te, ne).toLowerCase();
+                        return "*" === e ? function() {
+                            return !0
+                        } : function(e) {
+                            return e.nodeName && e.nodeName.toLowerCase() === t
+                        }
+                    },
+                    CLASS: function(e) {
+                        var t = m[e + " "];
+                        return t || (t = new RegExp("(^|" + M + ")" + e + "(" + M + "|$)")) && m(e, function(e) {
+                            return t.test("string" == typeof e.className && e.className || "undefined" != typeof e.getAttribute && e.getAttribute("class") || "")
+                        })
+                    },
+                    ATTR: function(n, r, i) {
+                        return function(e) {
+                            var t = se.attr(e, n);
+                            return null == t ? "!=" === r : !r || (t += "", "=" === r ? t === i : "!=" === r ? t !== i : "^=" === r ? i && 0 === t.indexOf(i) : "*=" === r ? i && -1 < t.indexOf(i) : "$=" === r ? i && t.slice(-i.length) === i : "~=" === r ? -1 < (" " + t.replace($, " ") + " ").indexOf(i) : "|=" === r && (t === i || t.slice(0, i.length + 1) === i + "-"))
+                        }
+                    },
+                    CHILD: function(h, e, t, g, y) {
+                        var v = "nth" !== h.slice(0, 3),
+                            m = "last" !== h.slice(-4),
+                            x = "of-type" === e;
+                        return 1 === g && 0 === y ? function(e) {
+                            return !!e.parentNode
+                        } : function(e, t, n) {
+                            var r, i, o, a, s, u, l = v !== m ? "nextSibling" : "previousSibling",
+                                c = e.parentNode,
+                                f = x && e.nodeName.toLowerCase(),
+                                p = !n && !x,
+                                d = !1;
+                            if (c) {
+                                if (v) {
+                                    while (l) {
+                                        a = e;
+                                        while (a = a[l])
+                                            if (x ? a.nodeName.toLowerCase() === f : 1 === a.nodeType) return !1;
+                                        u = l = "only" === h && !u && "nextSibling"
+                                    }
+                                    return !0
                                 }
-                                return !0
+                                if (u = [m ? c.firstChild : c.lastChild], m && p) {
+                                    d = (s = (r = (i = (o = (a = c)[S] || (a[S] = {}))[a.uniqueID] || (o[a.uniqueID] = {}))[h] || [])[0] === k && r[1]) && r[2], a = s && c.childNodes[s];
+                                    while (a = ++s && a && a[l] || (d = s = 0) || u.pop())
+                                        if (1 === a.nodeType && ++d && a === e) {
+                                            i[h] = [k, s, d];
+                                            break
+                                        }
+                                } else if (p && (d = s = (r = (i = (o = (a = e)[S] || (a[S] = {}))[a.uniqueID] || (o[a.uniqueID] = {}))[h] || [])[0] === k && r[1]), !1 === d)
+                                    while (a = ++s && a && a[l] || (d = s = 0) || u.pop())
+                                        if ((x ? a.nodeName.toLowerCase() === f : 1 === a.nodeType) && ++d && (p && ((i = (o = a[S] || (a[S] = {}))[a.uniqueID] || (o[a.uniqueID] = {}))[h] = [k, d]), a === e)) break;
+                                return (d -= y) === g || d % g == 0 && 0 <= d / g
                             }
-                            if (o = [g ? q.firstChild : q.lastChild], g && t) {
-                                k = q[s] || (q[s] = {}), j = k[a] || [], n = j[0] === u && j[1], m = j[0] === u && j[2], l = n && q.childNodes[n];
-                                while (l = ++n && l && l[p] || (m = n = 0) || o.pop())
-                                    if (1 === l.nodeType && ++m && l === b) {
-                                        k[a] = [u, n, m];
-                                        break
-                                    }
-                            } else if (t && (j = (b[s] || (b[s] = {}))[a]) && j[0] === u) m = j[1];
-                            else
-                                while (l = ++n && l && l[p] || (m = n = 0) || o.pop())
-                                    if ((h ? l.nodeName.toLowerCase() === r : 1 === l.nodeType) && ++m && (t && ((l[s] || (l[s] = {}))[a] = [u, m]), l === b)) break;
-                            return m -= e, m === d || m % d === 0 && m / d >= 0
                         }
-                    }
-                },
-                PSEUDO: function(a, b) {
-                    var c, e = d.pseudos[a] || d.setFilters[a.toLowerCase()] || db.error("unsupported pseudo: " + a);
-                    return e[s] ? e(b) : e.length > 1 ? (c = [a, a, "", b], d.setFilters.hasOwnProperty(a.toLowerCase()) ? fb(function(a, c) {
-                        var d, f = e(a, b),
-                            g = f.length;
-                        while (g--) d = I.call(a, f[g]), a[d] = !(c[d] = f[g])
-                    }) : function(a) {
-                        return e(a, 0, c)
-                    }) : e
-                }
-            },
-            pseudos: {
-                not: fb(function(a) {
-                    var b = [],
-                        c = [],
-                        d = g(a.replace(P, "$1"));
-                    return d[s] ? fb(function(a, b, c, e) {
-                        var f, g = d(a, null, e, []),
-                            h = a.length;
-                        while (h--)(f = g[h]) && (a[h] = !(b[h] = f))
-                    }) : function(a, e, f) {
-                        return b[0] = a, d(b, null, f, c), !c.pop()
-                    }
-                }),
-                has: fb(function(a) {
-                    return function(b) {
-                        return db(a, b).length > 0
-                    }
-                }),
-                contains: fb(function(a) {
-                    return function(b) {
-                        return (b.textContent || b.innerText || e(b)).indexOf(a) > -1
-                    }
-                }),
-                lang: fb(function(a) {
-                    return U.test(a || "") || db.error("unsupported lang: " + a), a = a.replace(ab, bb).toLowerCase(),
-                        function(b) {
-                            var c;
-                            do
-                                if (c = n ? b.lang : b.getAttribute("xml:lang") || b.getAttribute("lang")) return c = c.toLowerCase(), c === a || 0 === c.indexOf(a + "-"); while ((b = b.parentNode) && 1 === b.nodeType);
-                            return !1
+                    },
+                    PSEUDO: function(e, o) {
+                        var t, a = b.pseudos[e] || b.setFilters[e.toLowerCase()] || se.error("unsupported pseudo: " + e);
+                        return a[S] ? a(o) : 1 < a.length ? (t = [e, e, "", o], b.setFilters.hasOwnProperty(e.toLowerCase()) ? le(function(e, t) {
+                            var n, r = a(e, o),
+                                i = r.length;
+                            while (i--) e[n = P(e, r[i])] = !(t[n] = r[i])
+                        }) : function(e) {
+                            return a(e, 0, t)
+                        }) : a
+                    }
+                },
+                pseudos: {
+                    not: le(function(e) {
+                        var r = [],
+                            i = [],
+                            s = f(e.replace(B, "$1"));
+                        return s[S] ? le(function(e, t, n, r) {
+                            var i, o = s(e, null, r, []),
+                                a = e.length;
+                            while (a--)(i = o[a]) && (e[a] = !(t[a] = i))
+                        }) : function(e, t, n) {
+                            return r[0] = e, s(r, null, n, i), r[0] = null, !i.pop()
                         }
-                }),
-                target: function(b) {
-                    var c = a.location && a.location.hash;
-                    return c && c.slice(1) === b.id
-                },
-                root: function(a) {
-                    return a === m
-                },
-                focus: function(a) {
-                    return a === l.activeElement && (!l.hasFocus || l.hasFocus()) && !!(a.type || a.href || ~a.tabIndex)
-                },
-                enabled: function(a) {
-                    return a.disabled === !1
-                },
-                disabled: function(a) {
-                    return a.disabled === !0
-                },
-                checked: function(a) {
-                    var b = a.nodeName.toLowerCase();
-                    return "input" === b && !!a.checked || "option" === b && !!a.selected
-                },
-                selected: function(a) {
-                    return a.parentNode && a.parentNode.selectedIndex, a.selected === !0
-                },
-                empty: function(a) {
-                    for (a = a.firstChild; a; a = a.nextSibling)
-                        if (a.nodeType < 6) return !1;
-                    return !0
-                },
-                parent: function(a) {
-                    return !d.pseudos.empty(a)
-                },
-                header: function(a) {
-                    return X.test(a.nodeName)
-                },
-                input: function(a) {
-                    return W.test(a.nodeName)
-                },
-                button: function(a) {
-                    var b = a.nodeName.toLowerCase();
-                    return "input" === b && "button" === a.type || "button" === b
-                },
-                text: function(a) {
-                    var b;
-                    return "input" === a.nodeName.toLowerCase() && "text" === a.type && (null == (b = a.getAttribute("type")) || "text" === b.toLowerCase())
-                },
-                first: lb(function() {
-                    return [0]
-                }),
-                last: lb(function(a, b) {
-                    return [b - 1]
-                }),
-                eq: lb(function(a, b, c) {
-                    return [0 > c ? c + b : c]
-                }),
-                even: lb(function(a, b) {
-                    for (var c = 0; b > c; c += 2) a.push(c);
-                    return a
-                }),
-                odd: lb(function(a, b) {
-                    for (var c = 1; b > c; c += 2) a.push(c);
-                    return a
-                }),
-                lt: lb(function(a, b, c) {
-                    for (var d = 0 > c ? c + b : c; --d >= 0;) a.push(d);
-                    return a
-                }),
-                gt: lb(function(a, b, c) {
-                    for (var d = 0 > c ? c + b : c; ++d < b;) a.push(d);
-                    return a
-                })
-            }
-        }, d.pseudos.nth = d.pseudos.eq;
-        for (b in {
+                    }),
+                    has: le(function(t) {
+                        return function(e) {
+                            return 0 < se(t, e).length
+                        }
+                    }),
+                    contains: le(function(t) {
+                        return t = t.replace(te, ne),
+                            function(e) {
+                                return -1 < (e.textContent || o(e)).indexOf(t)
+                            }
+                    }),
+                    lang: le(function(n) {
+                        return V.test(n || "") || se.error("unsupported lang: " + n), n = n.replace(te, ne).toLowerCase(),
+                            function(e) {
+                                var t;
+                                do {
+                                    if (t = E ? e.lang : e.getAttribute("xml:lang") || e.getAttribute("lang")) return (t = t.toLowerCase()) === n || 0 === t.indexOf(n + "-")
+                                } while ((e = e.parentNode) && 1 === e.nodeType);
+                                return !1
+                            }
+                    }),
+                    target: function(e) {
+                        var t = n.location && n.location.hash;
+                        return t && t.slice(1) === e.id
+                    },
+                    root: function(e) {
+                        return e === a
+                    },
+                    focus: function(e) {
+                        return e === C.activeElement && (!C.hasFocus || C.hasFocus()) && !!(e.type || e.href || ~e.tabIndex)
+                    },
+                    enabled: ge(!1),
+                    disabled: ge(!0),
+                    checked: function(e) {
+                        var t = e.nodeName.toLowerCase();
+                        return "input" === t && !!e.checked || "option" === t && !!e.selected
+                    },
+                    selected: function(e) {
+                        return e.parentNode && e.parentNode.selectedIndex, !0 === e.selected
+                    },
+                    empty: function(e) {
+                        for (e = e.firstChild; e; e = e.nextSibling)
+                            if (e.nodeType < 6) return !1;
+                        return !0
+                    },
+                    parent: function(e) {
+                        return !b.pseudos.empty(e)
+                    },
+                    header: function(e) {
+                        return J.test(e.nodeName)
+                    },
+                    input: function(e) {
+                        return Q.test(e.nodeName)
+                    },
+                    button: function(e) {
+                        var t = e.nodeName.toLowerCase();
+                        return "input" === t && "button" === e.type || "button" === t
+                    },
+                    text: function(e) {
+                        var t;
+                        return "input" === e.nodeName.toLowerCase() && "text" === e.type && (null == (t = e.getAttribute("type")) || "text" === t.toLowerCase())
+                    },
+                    first: ye(function() {
+                        return [0]
+                    }),
+                    last: ye(function(e, t) {
+                        return [t - 1]
+                    }),
+                    eq: ye(function(e, t, n) {
+                        return [n < 0 ? n + t : n]
+                    }),
+                    even: ye(function(e, t) {
+                        for (var n = 0; n < t; n += 2) e.push(n);
+                        return e
+                    }),
+                    odd: ye(function(e, t) {
+                        for (var n = 1; n < t; n += 2) e.push(n);
+                        return e
+                    }),
+                    lt: ye(function(e, t, n) {
+                        for (var r = n < 0 ? n + t : t < n ? t : n; 0 <= --r;) e.push(r);
+                        return e
+                    }),
+                    gt: ye(function(e, t, n) {
+                        for (var r = n < 0 ? n + t : n; ++r < t;) e.push(r);
+                        return e
+                    })
+                }
+            }).pseudos.nth = b.pseudos.eq, {
                 radio: !0,
                 checkbox: !0,
                 file: !0,
                 password: !0,
                 image: !0
-            }) d.pseudos[b] = jb(b);
-        for (b in {
+            }) b.pseudos[e] = de(e);
+        for (e in {
                 submit: !0,
                 reset: !0
-            }) d.pseudos[b] = kb(b);
+            }) b.pseudos[e] = he(e);
 
-        function nb() {}
-        nb.prototype = d.filters = d.pseudos, d.setFilters = new nb;
+        function me() {}
 
-        function ob(a, b) {
-            var c, e, f, g, h, i, j, k = x[a + " "];
-            if (k) return b ? 0 : k.slice(0);
-            h = a, i = [], j = d.preFilter;
-            while (h) {
-                (!c || (e = Q.exec(h))) && (e && (h = h.slice(e[0].length) || h), i.push(f = [])), c = !1, (e = R.exec(h)) && (c = e.shift(), f.push({
-                    value: c,
-                    type: e[0].replace(P, " ")
-                }), h = h.slice(c.length));
-                for (g in d.filter) !(e = V[g].exec(h)) || j[g] && !(e = j[g](e)) || (c = e.shift(), f.push({
-                    value: c,
-                    type: g,
-                    matches: e
-                }), h = h.slice(c.length));
-                if (!c) break
-            }
-            return b ? h.length : h ? db.error(a) : x(a, i).slice(0)
-        }
-
-        function pb(a) {
-            for (var b = 0, c = a.length, d = ""; c > b; b++) d += a[b].value;
-            return d
-        }
-
-        function qb(a, b, c) {
-            var d = b.dir,
-                e = c && "parentNode" === d,
-                f = v++;
-            return b.first ? function(b, c, f) {
-                while (b = b[d])
-                    if (1 === b.nodeType || e) return a(b, c, f)
-            } : function(b, c, g) {
-                var h, i, j = [u, f];
-                if (g) {
-                    while (b = b[d])
-                        if ((1 === b.nodeType || e) && a(b, c, g)) return !0
+        function xe(e) {
+            for (var t = 0, n = e.length, r = ""; t < n; t++) r += e[t].value;
+            return r
+        }
+
+        function be(s, e, t) {
+            var u = e.dir,
+                l = e.next,
+                c = l || u,
+                f = t && "parentNode" === c,
+                p = r++;
+            return e.first ? function(e, t, n) {
+                while (e = e[u])
+                    if (1 === e.nodeType || f) return s(e, t, n);
+                return !1
+            } : function(e, t, n) {
+                var r, i, o, a = [k, p];
+                if (n) {
+                    while (e = e[u])
+                        if ((1 === e.nodeType || f) && s(e, t, n)) return !0
                 } else
-                    while (b = b[d])
-                        if (1 === b.nodeType || e) {
-                            if (i = b[s] || (b[s] = {}), (h = i[d]) && h[0] === u && h[1] === f) return j[2] = h[2];
-                            if (i[d] = j, j[2] = a(b, c, g)) return !0
-                        }
+                    while (e = e[u])
+                        if (1 === e.nodeType || f)
+                            if (i = (o = e[S] || (e[S] = {}))[e.uniqueID] || (o[e.uniqueID] = {}), l && l === e.nodeName.toLowerCase()) e = e[u] || e;
+                            else {
+                                if ((r = i[c]) && r[0] === k && r[1] === p) return a[2] = r[2];
+                                if ((i[c] = a)[2] = s(e, t, n)) return !0
+                            } return !1
             }
         }
 
-        function rb(a) {
-            return a.length > 1 ? function(b, c, d) {
-                var e = a.length;
-                while (e--)
-                    if (!a[e](b, c, d)) return !1;
+        function we(i) {
+            return 1 < i.length ? function(e, t, n) {
+                var r = i.length;
+                while (r--)
+                    if (!i[r](e, t, n)) return !1;
                 return !0
-            } : a[0]
+            } : i[0]
         }
 
-        function sb(a, b, c, d, e) {
-            for (var f, g = [], h = 0, i = a.length, j = null != b; i > h; h++)(f = a[h]) && (!c || c(f, d, e)) && (g.push(f), j && b.push(h));
-            return g
-        }
-
-        function tb(a, b, c, d, e, f) {
-            return d && !d[s] && (d = tb(d)), e && !e[s] && (e = tb(e, f)), fb(function(f, g, h, i) {
-                var j, k, l, m = [],
-                    n = [],
-                    o = g.length,
-                    p = f || wb(b || "*", h.nodeType ? [h] : h, []),
-                    q = !a || !f && b ? p : sb(p, m, a, h, i),
-                    r = c ? e || (f ? a : o || d) ? [] : g : q;
-                if (c && c(q, r, h, i), d) {
-                    j = sb(r, n), d(j, [], h, i), k = j.length;
-                    while (k--)(l = j[k]) && (r[n[k]] = !(q[n[k]] = l))
-                }
-                if (f) {
-                    if (e || a) {
-                        if (e) {
-                            j = [], k = r.length;
-                            while (k--)(l = r[k]) && j.push(q[k] = l);
-                            e(null, r = [], j, i)
+        function Te(e, t, n, r, i) {
+            for (var o, a = [], s = 0, u = e.length, l = null != t; s < u; s++)(o = e[s]) && (n && !n(o, r, i) || (a.push(o), l && t.push(s)));
+            return a
+        }
+
+        function Ce(d, h, g, y, v, e) {
+            return y && !y[S] && (y = Ce(y)), v && !v[S] && (v = Ce(v, e)), le(function(e, t, n, r) {
+                var i, o, a, s = [],
+                    u = [],
+                    l = t.length,
+                    c = e || function(e, t, n) {
+                        for (var r = 0, i = t.length; r < i; r++) se(e, t[r], n);
+                        return n
+                    }(h || "*", n.nodeType ? [n] : n, []),
+                    f = !d || !e && h ? c : Te(c, s, d, n, r),
+                    p = g ? v || (e ? d : l || y) ? [] : t : f;
+                if (g && g(f, p, n, r), y) {
+                    i = Te(p, u), y(i, [], n, r), o = i.length;
+                    while (o--)(a = i[o]) && (p[u[o]] = !(f[u[o]] = a))
+                }
+                if (e) {
+                    if (v || d) {
+                        if (v) {
+                            i = [], o = p.length;
+                            while (o--)(a = p[o]) && i.push(f[o] = a);
+                            v(null, p = [], i, r)
                         }
-                        k = r.length;
-                        while (k--)(l = r[k]) && (j = e ? I.call(f, l) : m[k]) > -1 && (f[j] = !(g[j] = l))
+                        o = p.length;
+                        while (o--)(a = p[o]) && -1 < (i = v ? P(e, a) : s[o]) && (e[i] = !(t[i] = a))
                     }
-                } else r = sb(r === g ? r.splice(o, r.length) : r), e ? e(null, g, r, i) : G.apply(g, r)
+                } else p = Te(p === t ? p.splice(l, p.length) : p), v ? v(null, t, p, r) : H.apply(t, p)
             })
         }
 
-        function ub(a) {
-            for (var b, c, e, f = a.length, g = d.relative[a[0].type], i = g || d.relative[" "], j = g ? 1 : 0, k = qb(function(a) {
-                    return a === b
-                }, i, !0), l = qb(function(a) {
-                    return I.call(b, a) > -1
-                }, i, !0), m = [function(a, c, d) {
-                    return !g && (d || c !== h) || ((b = c).nodeType ? k(a, c, d) : l(a, c, d))
-                }]; f > j; j++)
-                if (c = d.relative[a[j].type]) m = [qb(rb(m), c)];
+        function Ee(e) {
+            for (var i, t, n, r = e.length, o = b.relative[e[0].type], a = o || b.relative[" "], s = o ? 1 : 0, u = be(function(e) {
+                    return e === i
+                }, a, !0), l = be(function(e) {
+                    return -1 < P(i, e)
+                }, a, !0), c = [function(e, t, n) {
+                    var r = !o && (n || t !== w) || ((i = t).nodeType ? u(e, t, n) : l(e, t, n));
+                    return i = null, r
+                }]; s < r; s++)
+                if (t = b.relative[e[s].type]) c = [be(we(c), t)];
                 else {
-                    if (c = d.filter[a[j].type].apply(null, a[j].matches), c[s]) {
-                        for (e = ++j; f > e; e++)
-                            if (d.relative[a[e].type]) break;
-                        return tb(j > 1 && rb(m), j > 1 && pb(a.slice(0, j - 1).concat({
-                            value: " " === a[j - 2].type ? "*" : ""
-                        })).replace(P, "$1"), c, e > j && ub(a.slice(j, e)), f > e && ub(a = a.slice(e)), f > e && pb(a))
-                    }
-                    m.push(c)
-                } return rb(m)
-        }
-
-        function vb(a, b) {
-            var c = b.length > 0,
-                e = a.length > 0,
-                f = function(f, g, i, j, k) {
-                    var m, n, o, p = 0,
-                        q = "0",
-                        r = f && [],
-                        s = [],
-                        t = h,
-                        v = f || e && d.find.TAG("*", k),
-                        w = u += null == t ? 1 : Math.random() || .1,
-                        x = v.length;
-                    for (k && (h = g !== l && g); q !== x && null != (m = v[q]); q++) {
-                        if (e && m) {
-                            n = 0;
-                            while (o = a[n++])
-                                if (o(m, g, i)) {
-                                    j.push(m);
+                    if ((t = b.filter[e[s].type].apply(null, e[s].matches))[S]) {
+                        for (n = ++s; n < r; n++)
+                            if (b.relative[e[n].type]) break;
+                        return Ce(1 < s && we(c), 1 < s && xe(e.slice(0, s - 1).concat({
+                            value: " " === e[s - 2].type ? "*" : ""
+                        })).replace(B, "$1"), t, s < n && Ee(e.slice(s, n)), n < r && Ee(e = e.slice(n)), n < r && xe(e))
+                    }
+                    c.push(t)
+                } return we(c)
+        }
+        return me.prototype = b.filters = b.pseudos, b.setFilters = new me, h = se.tokenize = function(e, t) {
+            var n, r, i, o, a, s, u, l = x[e + " "];
+            if (l) return t ? 0 : l.slice(0);
+            a = e, s = [], u = b.preFilter;
+            while (a) {
+                for (o in n && !(r = _.exec(a)) || (r && (a = a.slice(r[0].length) || a), s.push(i = [])), n = !1, (r = z.exec(a)) && (n = r.shift(), i.push({
+                        value: n,
+                        type: r[0].replace(B, " ")
+                    }), a = a.slice(n.length)), b.filter) !(r = G[o].exec(a)) || u[o] && !(r = u[o](r)) || (n = r.shift(), i.push({
+                    value: n,
+                    type: o,
+                    matches: r
+                }), a = a.slice(n.length));
+                if (!n) break
+            }
+            return t ? a.length : a ? se.error(e) : x(e, s).slice(0)
+        }, f = se.compile = function(e, t) {
+            var n, y, v, m, x, r, i = [],
+                o = [],
+                a = A[e + " "];
+            if (!a) {
+                t || (t = h(e)), n = t.length;
+                while (n--)(a = Ee(t[n]))[S] ? i.push(a) : o.push(a);
+                (a = A(e, (y = o, m = 0 < (v = i).length, x = 0 < y.length, r = function(e, t, n, r, i) {
+                    var o, a, s, u = 0,
+                        l = "0",
+                        c = e && [],
+                        f = [],
+                        p = w,
+                        d = e || x && b.find.TAG("*", i),
+                        h = k += null == p ? 1 : Math.random() || .1,
+                        g = d.length;
+                    for (i && (w = t == C || t || i); l !== g && null != (o = d[l]); l++) {
+                        if (x && o) {
+                            a = 0, t || o.ownerDocument == C || (T(o), n = !E);
+                            while (s = y[a++])
+                                if (s(o, t || C, n)) {
+                                    r.push(o);
                                     break
-                                } k && (u = w)
+                                } i && (k = h)
                         }
-                        c && ((m = !o && m) && p--, f && r.push(m))
+                        m && ((o = !s && o) && u--, e && c.push(o))
                     }
-                    if (p += q, c && q !== p) {
-                        n = 0;
-                        while (o = b[n++]) o(r, s, g, i);
-                        if (f) {
-                            if (p > 0)
-                                while (q--) r[q] || s[q] || (s[q] = E.call(j));
-                            s = sb(s)
+                    if (u += l, m && l !== u) {
+                        a = 0;
+                        while (s = v[a++]) s(c, f, t, n);
+                        if (e) {
+                            if (0 < u)
+                                while (l--) c[l] || f[l] || (f[l] = q.call(r));
+                            f = Te(f)
                         }
-                        G.apply(j, s), k && !f && s.length > 0 && p + b.length > 1 && db.uniqueSort(j)
+                        H.apply(r, f), i && !e && 0 < f.length && 1 < u + v.length && se.uniqueSort(r)
                     }
-                    return k && (u = w, h = t), r
-                };
-            return c ? fb(f) : f
-        }
-        g = db.compile = function(a, b) {
-            var c, d = [],
-                e = [],
-                f = y[a + " "];
-            if (!f) {
-                b || (b = ob(a)), c = b.length;
-                while (c--) f = ub(b[c]), f[s] ? d.push(f) : e.push(f);
-                f = y(a, vb(e, d))
+                    return i && (k = h, w = p), c
+                }, m ? le(r) : r))).selector = e
             }
-            return f
-        };
-
-        function wb(a, b, c) {
-            for (var d = 0, e = b.length; e > d; d++) db(a, b[d], c);
-            return c
-        }
-
-        function xb(a, b, e, f) {
-            var h, i, j, k, l, m = ob(a);
-            if (!f && 1 === m.length) {
-                if (i = m[0] = m[0].slice(0), i.length > 2 && "ID" === (j = i[0]).type && c.getById && 9 === b.nodeType && n && d.relative[i[1].type]) {
-                    if (b = (d.find.ID(j.matches[0].replace(ab, bb), b) || [])[0], !b) return e;
-                    a = a.slice(i.shift().value.length)
-                }
-                h = V.needsContext.test(a) ? 0 : i.length;
-                while (h--) {
-                    if (j = i[h], d.relative[k = j.type]) break;
-                    if ((l = d.find[k]) && (f = l(j.matches[0].replace(ab, bb), $.test(i[0].type) && mb(b.parentNode) || b))) {
-                        if (i.splice(h, 1), a = f.length && pb(i), !a) return G.apply(e, f), e;
+            return a
+        }, g = se.select = function(e, t, n, r) {
+            var i, o, a, s, u, l = "function" == typeof e && e,
+                c = !r && h(e = l.selector || e);
+            if (n = n || [], 1 === c.length) {
+                if (2 < (o = c[0] = c[0].slice(0)).length && "ID" === (a = o[0]).type && 9 === t.nodeType && E && b.relative[o[1].type]) {
+                    if (!(t = (b.find.ID(a.matches[0].replace(te, ne), t) || [])[0])) return n;
+                    l && (t = t.parentNode), e = e.slice(o.shift().value.length)
+                }
+                i = G.needsContext.test(e) ? 0 : o.length;
+                while (i--) {
+                    if (a = o[i], b.relative[s = a.type]) break;
+                    if ((u = b.find[s]) && (r = u(a.matches[0].replace(te, ne), ee.test(o[0].type) && ve(t.parentNode) || t))) {
+                        if (o.splice(i, 1), !(e = r.length && xe(o))) return H.apply(n, r), n;
                         break
                     }
                 }
             }
-            return g(a, m)(f, b, !n, e, $.test(a) && mb(b.parentNode) || b), e
-        }
-        return c.sortStable = s.split("").sort(z).join("") === s, c.detectDuplicates = !!j, k(), c.sortDetached = gb(function(a) {
-            return 1 & a.compareDocumentPosition(l.createElement("div"))
-        }), gb(function(a) {
-            return a.innerHTML = "<a href='#'></a>", "#" === a.firstChild.getAttribute("href")
-        }) || hb("type|href|height|width", function(a, b, c) {
-            return c ? void 0 : a.getAttribute(b, "type" === b.toLowerCase() ? 1 : 2)
-        }), c.attributes && gb(function(a) {
-            return a.innerHTML = "<input/>", a.firstChild.setAttribute("value", ""), "" === a.firstChild.getAttribute("value")
-        }) || hb("value", function(a, b, c) {
-            return c || "input" !== a.nodeName.toLowerCase() ? void 0 : a.defaultValue
-        }), gb(function(a) {
-            return null == a.getAttribute("disabled")
-        }) || hb(J, function(a, b, c) {
-            var d;
-            return c ? void 0 : a[b] === !0 ? b.toLowerCase() : (d = a.getAttributeNode(b)) && d.specified ? d.value : null
-        }), db
-    }(a);
-    o.find = t, o.expr = t.selectors, o.expr[":"] = o.expr.pseudos, o.unique = t.uniqueSort, o.text = t.getText, o.isXMLDoc = t.isXML, o.contains = t.contains;
-    var u = o.expr.match.needsContext,
-        v = /^<(\w+)\s*\/?>(?:<\/\1>|)$/,
-        w = /^.[^:#\[\.,]*$/;
-
-    function x(a, b, c) {
-        if (o.isFunction(b)) return o.grep(a, function(a, d) {
-            return !!b.call(a, d, a) !== c
-        });
-        if (b.nodeType) return o.grep(a, function(a) {
-            return a === b !== c
-        });
-        if ("string" == typeof b) {
-            if (w.test(b)) return o.filter(b, a, c);
-            b = o.filter(b, a)
-        }
-        return o.grep(a, function(a) {
-            return g.call(b, a) >= 0 !== c
-        })
-    }
-    o.filter = function(a, b, c) {
-        var d = b[0];
-        return c && (a = ":not(" + a + ")"), 1 === b.length && 1 === d.nodeType ? o.find.matchesSelector(d, a) ? [d] : [] : o.find.matches(a, o.grep(b, function(a) {
-            return 1 === a.nodeType
+            return (l || f(e, c))(r, t, !E, n, !t || ee.test(e) && ve(t.parentNode) || t), n
+        }, d.sortStable = S.split("").sort(j).join("") === S, d.detectDuplicates = !!l, T(), d.sortDetached = ce(function(e) {
+            return 1 & e.compareDocumentPosition(C.createElement("fieldset"))
+        }), ce(function(e) {
+            return e.innerHTML = "<a href='#'></a>", "#" === e.firstChild.getAttribute("href")
+        }) || fe("type|href|height|width", function(e, t, n) {
+            if (!n) return e.getAttribute(t, "type" === t.toLowerCase() ? 1 : 2)
+        }), d.attributes && ce(function(e) {
+            return e.innerHTML = "<input/>", e.firstChild.setAttribute("value", ""), "" === e.firstChild.getAttribute("value")
+        }) || fe("value", function(e, t, n) {
+            if (!n && "input" === e.nodeName.toLowerCase()) return e.defaultValue
+        }), ce(function(e) {
+            return null == e.getAttribute("disabled")
+        }) || fe(R, function(e, t, n) {
+            var r;
+            if (!n) return !0 === e[t] ? t.toLowerCase() : (r = e.getAttributeNode(t)) && r.specified ? r.value : null
+        }), se
+    }(C);
+    S.find = d, S.expr = d.selectors, S.expr[":"] = S.expr.pseudos, S.uniqueSort = S.unique = d.uniqueSort, S.text = d.getText, S.isXMLDoc = d.isXML, S.contains = d.contains, S.escapeSelector = d.escape;
+    var h = function(e, t, n) {
+            var r = [],
+                i = void 0 !== n;
+            while ((e = e[t]) && 9 !== e.nodeType)
+                if (1 === e.nodeType) {
+                    if (i && S(e).is(n)) break;
+                    r.push(e)
+                } return r
+        },
+        T = function(e, t) {
+            for (var n = []; e; e = e.nextSibling) 1 === e.nodeType && e !== t && n.push(e);
+            return n
+        },
+        k = S.expr.match.needsContext;
+
+    function A(e, t) {
+        return e.nodeName && e.nodeName.toLowerCase() === t.toLowerCase()
+    }
+    var N = /^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i;
+
+    function j(e, n, r) {
+        return m(n) ? S.grep(e, function(e, t) {
+            return !!n.call(e, t, e) !== r
+        }) : n.nodeType ? S.grep(e, function(e) {
+            return e === n !== r
+        }) : "string" != typeof n ? S.grep(e, function(e) {
+            return -1 < i.call(n, e) !== r
+        }) : S.filter(n, e, r)
+    }
+    S.filter = function(e, t, n) {
+        var r = t[0];
+        return n && (e = ":not(" + e + ")"), 1 === t.length && 1 === r.nodeType ? S.find.matchesSelector(r, e) ? [r] : [] : S.find.matches(e, S.grep(t, function(e) {
+            return 1 === e.nodeType
         }))
-    }, o.fn.extend({
-        find: function(a) {
-            var b, c = this.length,
-                d = [],
-                e = this;
-            if ("string" != typeof a) return this.pushStack(o(a).filter(function() {
-                for (b = 0; c > b; b++)
-                    if (o.contains(e[b], this)) return !0
+    }, S.fn.extend({
+        find: function(e) {
+            var t, n, r = this.length,
+                i = this;
+            if ("string" != typeof e) return this.pushStack(S(e).filter(function() {
+                for (t = 0; t < r; t++)
+                    if (S.contains(i[t], this)) return !0
             }));
-            for (b = 0; c > b; b++) o.find(a, e[b], d);
-            return d = this.pushStack(c > 1 ? o.unique(d) : d), d.selector = this.selector ? this.selector + " " + a : a, d
+            for (n = this.pushStack([]), t = 0; t < r; t++) S.find(e, i[t], n);
+            return 1 < r ? S.uniqueSort(n) : n
         },
-        filter: function(a) {
-            return this.pushStack(x(this, a || [], !1))
+        filter: function(e) {
+            return this.pushStack(j(this, e || [], !1))
         },
-        not: function(a) {
-            return this.pushStack(x(this, a || [], !0))
+        not: function(e) {
+            return this.pushStack(j(this, e || [], !0))
         },
-        is: function(a) {
-            return !!x(this, "string" == typeof a && u.test(a) ? o(a) : a || [], !1).length
+        is: function(e) {
+            return !!j(this, "string" == typeof e && k.test(e) ? S(e) : e || [], !1).length
         }
     });
-    var y, z = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]*))$/,
-        A = o.fn.init = function(a, b) {
-            var c, d;
-            if (!a) return this;
-            if ("string" == typeof a) {
-                if (c = "<" === a[0] && ">" === a[a.length - 1] && a.length >= 3 ? [null, a, null] : z.exec(a), !c || !c[1] && b) return !b || b.jquery ? (b || y).find(a) : this.constructor(b).find(a);
-                if (c[1]) {
-                    if (b = b instanceof o ? b[0] : b, o.merge(this, o.parseHTML(c[1], b && b.nodeType ? b.ownerDocument || b : m, !0)), v.test(c[1]) && o.isPlainObject(b))
-                        for (c in b) o.isFunction(this[c]) ? this[c](b[c]) : this.attr(c, b[c]);
-                    return this
-                }
-                return d = m.getElementById(c[2]), d && d.parentNode && (this.length = 1, this[0] = d), this.context = m, this.selector = a, this
+    var D, q = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/;
+    (S.fn.init = function(e, t, n) {
+        var r, i;
+        if (!e) return this;
+        if (n = n || D, "string" == typeof e) {
+            if (!(r = "<" === e[0] && ">" === e[e.length - 1] && 3 <= e.length ? [null, e, null] : q.exec(e)) || !r[1] && t) return !t || t.jquery ? (t || n).find(e) : this.constructor(t).find(e);
+            if (r[1]) {
+                if (t = t instanceof S ? t[0] : t, S.merge(this, S.parseHTML(r[1], t && t.nodeType ? t.ownerDocument || t : E, !0)), N.test(r[1]) && S.isPlainObject(t))
+                    for (r in t) m(this[r]) ? this[r](t[r]) : this.attr(r, t[r]);
+                return this
             }
-            return a.nodeType ? (this.context = this[0] = a, this.length = 1, this) : o.isFunction(a) ? "undefined" != typeof y.ready ? y.ready(a) : a(o) : (void 0 !== a.selector && (this.selector = a.selector, this.context = a.context), o.makeArray(a, this))
-        };
-    A.prototype = o.fn, y = o(m);
-    var B = /^(?:parents|prev(?:Until|All))/,
-        C = {
+            return (i = E.getElementById(r[2])) && (this[0] = i, this.length = 1), this
+        }
+        return e.nodeType ? (this[0] = e, this.length = 1, this) : m(e) ? void 0 !== n.ready ? n.ready(e) : e(S) : S.makeArray(e, this)
+    }).prototype = S.fn, D = S(E);
+    var L = /^(?:parents|prev(?:Until|All))/,
+        H = {
             children: !0,
             contents: !0,
             next: !0,
             prev: !0
         };
-    o.extend({
-        dir: function(a, b, c) {
-            var d = [],
-                e = void 0 !== c;
-            while ((a = a[b]) && 9 !== a.nodeType)
-                if (1 === a.nodeType) {
-                    if (e && o(a).is(c)) break;
-                    d.push(a)
-                } return d
-        },
-        sibling: function(a, b) {
-            for (var c = []; a; a = a.nextSibling) 1 === a.nodeType && a !== b && c.push(a);
-            return c
-        }
-    }), o.fn.extend({
-        has: function(a) {
-            var b = o(a, this),
-                c = b.length;
+
+    function O(e, t) {
+        while ((e = e[t]) && 1 !== e.nodeType);
+        return e
+    }
+    S.fn.extend({
+        has: function(e) {
+            var t = S(e, this),
+                n = t.length;
             return this.filter(function() {
-                for (var a = 0; c > a; a++)
-                    if (o.contains(this, b[a])) return !0
+                for (var e = 0; e < n; e++)
+                    if (S.contains(this, t[e])) return !0
             })
         },
-        closest: function(a, b) {
-            for (var c, d = 0, e = this.length, f = [], g = u.test(a) || "string" != typeof a ? o(a, b || this.context) : 0; e > d; d++)
-                for (c = this[d]; c && c !== b; c = c.parentNode)
-                    if (c.nodeType < 11 && (g ? g.index(c) > -1 : 1 === c.nodeType && o.find.matchesSelector(c, a))) {
-                        f.push(c);
-                        break
-                    } return this.pushStack(f.length > 1 ? o.unique(f) : f)
+        closest: function(e, t) {
+            var n, r = 0,
+                i = this.length,
+                o = [],
+                a = "string" != typeof e && S(e);
+            if (!k.test(e))
+                for (; r < i; r++)
+                    for (n = this[r]; n && n !== t; n = n.parentNode)
+                        if (n.nodeType < 11 && (a ? -1 < a.index(n) : 1 === n.nodeType && S.find.matchesSelector(n, e))) {
+                            o.push(n);
+                            break
+                        } return this.pushStack(1 < o.length ? S.uniqueSort(o) : o)
         },
-        index: function(a) {
-            return a ? "string" == typeof a ? g.call(o(a), this[0]) : g.call(this, a.jquery ? a[0] : a) : this[0] && this[0].parentNode ? this.first().prevAll().length : -1
+        index: function(e) {
+            return e ? "string" == typeof e ? i.call(S(e), this[0]) : i.call(this, e.jquery ? e[0] : e) : this[0] && this[0].parentNode ? this.first().prevAll().length : -1
         },
-        add: function(a, b) {
-            return this.pushStack(o.unique(o.merge(this.get(), o(a, b))))
+        add: function(e, t) {
+            return this.pushStack(S.uniqueSort(S.merge(this.get(), S(e, t))))
         },
-        addBack: function(a) {
-            return this.add(null == a ? this.prevObject : this.prevObject.filter(a))
+        addBack: function(e) {
+            return this.add(null == e ? this.prevObject : this.prevObject.filter(e))
         }
-    });
-
-    function D(a, b) {
-        while ((a = a[b]) && 1 !== a.nodeType);
-        return a
-    }
-    o.each({
-        parent: function(a) {
-            var b = a.parentNode;
-            return b && 11 !== b.nodeType ? b : null
+    }), S.each({
+        parent: function(e) {
+            var t = e.parentNode;
+            return t && 11 !== t.nodeType ? t : null
         },
-        parents: function(a) {
-            return o.dir(a, "parentNode")
+        parents: function(e) {
+            return h(e, "parentNode")
         },
-        parentsUntil: function(a, b, c) {
-            return o.dir(a, "parentNode", c)
+        parentsUntil: function(e, t, n) {
+            return h(e, "parentNode", n)
         },
-        next: function(a) {
-            return D(a, "nextSibling")
+        next: function(e) {
+            return O(e, "nextSibling")
         },
-        prev: function(a) {
-            return D(a, "previousSibling")
+        prev: function(e) {
+            return O(e, "previousSibling")
         },
-        nextAll: function(a) {
-            return o.dir(a, "nextSibling")
+        nextAll: function(e) {
+            return h(e, "nextSibling")
         },
-        prevAll: function(a) {
-            return o.dir(a, "previousSibling")
+        prevAll: function(e) {
+            return h(e, "previousSibling")
         },
-        nextUntil: function(a, b, c) {
-            return o.dir(a, "nextSibling", c)
+        nextUntil: function(e, t, n) {
+            return h(e, "nextSibling", n)
         },
-        prevUntil: function(a, b, c) {
-            return o.dir(a, "previousSibling", c)
+        prevUntil: function(e, t, n) {
+            return h(e, "previousSibling", n)
         },
-        siblings: function(a) {
-            return o.sibling((a.parentNode || {}).firstChild, a)
+        siblings: function(e) {
+            return T((e.parentNode || {}).firstChild, e)
         },
-        children: function(a) {
-            return o.sibling(a.firstChild)
+        children: function(e) {
+            return T(e.firstChild)
         },
-        contents: function(a) {
-            return a.contentDocument || o.merge([], a.childNodes)
+        contents: function(e) {
+            return null != e.contentDocument && r(e.contentDocument) ? e.contentDocument : (A(e, "template") && (e = e.content || e), S.merge([], e.childNodes))
         }
-    }, function(a, b) {
-        o.fn[a] = function(c, d) {
-            var e = o.map(this, b, c);
-            return "Until" !== a.slice(-5) && (d = c), d && "string" == typeof d && (e = o.filter(d, e)), this.length > 1 && (C[a] || o.unique(e), B.test(a) && e.reverse()), this.pushStack(e)
+    }, function(r, i) {
+        S.fn[r] = function(e, t) {
+            var n = S.map(this, i, e);
+            return "Until" !== r.slice(-5) && (t = e), t && "string" == typeof t && (n = S.filter(t, n)), 1 < this.length && (H[r] || S.uniqueSort(n), L.test(r) && n.reverse()), this.pushStack(n)
         }
     });
-    var E = /\S+/g,
-        F = {};
+    var P = /[^\x20\t\r\n\f]+/g;
 
-    function G(a) {
-        var b = F[a] = {};
-        return o.each(a.match(E) || [], function(a, c) {
-            b[c] = !0
-        }), b
-    }
-    o.Callbacks = function(a) {
-        a = "string" == typeof a ? F[a] || G(a) : o.extend({}, a);
-        var b, c, d, e, f, g, h = [],
-            i = !a.once && [],
-            j = function(l) {
-                for (b = a.memory && l, c = !0, g = e || 0, e = 0, f = h.length, d = !0; h && f > g; g++)
-                    if (h[g].apply(l[0], l[1]) === !1 && a.stopOnFalse) {
-                        b = !1;
-                        break
-                    } d = !1, h && (i ? i.length && j(i.shift()) : b ? h = [] : k.disable())
+    function R(e) {
+        return e
+    }
+
+    function M(e) {
+        throw e
+    }
+
+    function I(e, t, n, r) {
+        var i;
+        try {
+            e && m(i = e.promise) ? i.call(e).done(t).fail(n) : e && m(i = e.then) ? i.call(e, t, n) : t.apply(void 0, [e].slice(r))
+        } catch (e) {
+            n.apply(void 0, [e])
+        }
+    }
+    S.Callbacks = function(r) {
+        var e, n;
+        r = "string" == typeof r ? (e = r, n = {}, S.each(e.match(P) || [], function(e, t) {
+            n[t] = !0
+        }), n) : S.extend({}, r);
+        var i, t, o, a, s = [],
+            u = [],
+            l = -1,
+            c = function() {
+                for (a = a || r.once, o = i = !0; u.length; l = -1) {
+                    t = u.shift();
+                    while (++l < s.length) !1 === s[l].apply(t[0], t[1]) && r.stopOnFalse && (l = s.length, t = !1)
+                }
+                r.memory || (t = !1), i = !1, a && (s = t ? [] : "")
             },
-            k = {
+            f = {
                 add: function() {
-                    if (h) {
-                        var c = h.length;
-                        ! function g(b) {
-                            o.each(b, function(b, c) {
-                                var d = o.type(c);
-                                "function" === d ? a.unique && k.has(c) || h.push(c) : c && c.length && "string" !== d && g(c)
-                            })
-                        }(arguments), d ? f = h.length : b && (e = c, j(b))
-                    }
-                    return this
+                    return s && (t && !i && (l = s.length - 1, u.push(t)), function n(e) {
+                        S.each(e, function(e, t) {
+                            m(t) ? r.unique && f.has(t) || s.push(t) : t && t.length && "string" !== w(t) && n(t)
+                        })
+                    }(arguments), t && !i && c()), this
                 },
                 remove: function() {
-                    return h && o.each(arguments, function(a, b) {
-                        var c;
-                        while ((c = o.inArray(b, h, c)) > -1) h.splice(c, 1), d && (f >= c && f--, g >= c && g--)
+                    return S.each(arguments, function(e, t) {
+                        var n;
+                        while (-1 < (n = S.inArray(t, s, n))) s.splice(n, 1), n <= l && l--
                     }), this
                 },
-                has: function(a) {
-                    return a ? o.inArray(a, h) > -1 : !(!h || !h.length)
+                has: function(e) {
+                    return e ? -1 < S.inArray(e, s) : 0 < s.length
                 },
                 empty: function() {
-                    return h = [], f = 0, this
+                    return s && (s = []), this
                 },
                 disable: function() {
-                    return h = i = b = void 0, this
+                    return a = u = [], s = t = "", this
                 },
                 disabled: function() {
-                    return !h
+                    return !s
                 },
                 lock: function() {
-                    return i = void 0, b || k.disable(), this
+                    return a = u = [], t || i || (s = t = ""), this
                 },
                 locked: function() {
-                    return !i
+                    return !!a
                 },
-                fireWith: function(a, b) {
-                    return !h || c && !i || (b = b || [], b = [a, b.slice ? b.slice() : b], d ? i.push(b) : j(b)), this
+                fireWith: function(e, t) {
+                    return a || (t = [e, (t = t || []).slice ? t.slice() : t], u.push(t), i || c()), this
                 },
                 fire: function() {
-                    return k.fireWith(this, arguments), this
+                    return f.fireWith(this, arguments), this
                 },
                 fired: function() {
-                    return !!c
+                    return !!o
                 }
             };
-        return k
-    }, o.extend({
-        Deferred: function(a) {
-            var b = [
-                    ["resolve", "done", o.Callbacks("once memory"), "resolved"],
-                    ["reject", "fail", o.Callbacks("once memory"), "rejected"],
-                    ["notify", "progress", o.Callbacks("memory")]
+        return f
+    }, S.extend({
+        Deferred: function(e) {
+            var o = [
+                    ["notify", "progress", S.Callbacks("memory"), S.Callbacks("memory"), 2],
+                    ["resolve", "done", S.Callbacks("once memory"), S.Callbacks("once memory"), 0, "resolved"],
+                    ["reject", "fail", S.Callbacks("once memory"), S.Callbacks("once memory"), 1, "rejected"]
                 ],
-                c = "pending",
-                d = {
+                i = "pending",
+                a = {
                     state: function() {
-                        return c
+                        return i
                     },
                     always: function() {
-                        return e.done(arguments).fail(arguments), this
+                        return s.done(arguments).fail(arguments), this
+                    },
+                    "catch": function(e) {
+                        return a.then(null, e)
                     },
-                    then: function() {
-                        var a = arguments;
-                        return o.Deferred(function(c) {
-                            o.each(b, function(b, f) {
-                                var g = o.isFunction(a[b]) && a[b];
-                                e[f[1]](function() {
-                                    var a = g && g.apply(this, arguments);
-                                    a && o.isFunction(a.promise) ? a.promise().done(c.resolve).fail(c.reject).progress(c.notify) : c[f[0] + "With"](this === d ? c.promise() : this, g ? [a] : arguments)
+                    pipe: function() {
+                        var i = arguments;
+                        return S.Deferred(function(r) {
+                            S.each(o, function(e, t) {
+                                var n = m(i[t[4]]) && i[t[4]];
+                                s[t[1]](function() {
+                                    var e = n && n.apply(this, arguments);
+                                    e && m(e.promise) ? e.promise().progress(r.notify).done(r.resolve).fail(r.reject) : r[t[0] + "With"](this, n ? [e] : arguments)
                                 })
-                            }), a = null
+                            }), i = null
+                        }).promise()
+                    },
+                    then: function(t, n, r) {
+                        var u = 0;
+
+                        function l(i, o, a, s) {
+                            return function() {
+                                var n = this,
+                                    r = arguments,
+                                    e = function() {
+                                        var e, t;
+                                        if (!(i < u)) {
+                                            if ((e = a.apply(n, r)) === o.promise()) throw new TypeError("Thenable self-resolution");
+                                            t = e && ("object" == typeof e || "function" == typeof e) && e.then, m(t) ? s ? t.call(e, l(u, o, R, s), l(u, o, M, s)) : (u++, t.call(e, l(u, o, R, s), l(u, o, M, s), l(u, o, R, o.notifyWith))) : (a !== R && (n = void 0, r = [e]), (s || o.resolveWith)(n, r))
+                                        }
+                                    },
+                                    t = s ? e : function() {
+                                        try {
+                                            e()
+                                        } catch (e) {
+                                            S.Deferred.exceptionHook && S.Deferred.exceptionHook(e, t.stackTrace), u <= i + 1 && (a !== M && (n = void 0, r = [e]), o.rejectWith(n, r))
+                                        }
+                                    };
+                                i ? t() : (S.Deferred.getStackHook && (t.stackTrace = S.Deferred.getStackHook()), C.setTimeout(t))
+                            }
+                        }
+                        return S.Deferred(function(e) {
+                            o[0][3].add(l(0, e, m(r) ? r : R, e.notifyWith)), o[1][3].add(l(0, e, m(t) ? t : R)), o[2][3].add(l(0, e, m(n) ? n : M))
                         }).promise()
                     },
-                    promise: function(a) {
-                        return null != a ? o.extend(a, d) : d
+                    promise: function(e) {
+                        return null != e ? S.extend(e, a) : a
                     }
                 },
-                e = {};
-            return d.pipe = d.then, o.each(b, function(a, f) {
-                var g = f[2],
-                    h = f[3];
-                d[f[1]] = g.add, h && g.add(function() {
-                    c = h
-                }, b[1 ^ a][2].disable, b[2][2].lock), e[f[0]] = function() {
-                    return e[f[0] + "With"](this === e ? d : this, arguments), this
-                }, e[f[0] + "With"] = g.fireWith
-            }), d.promise(e), a && a.call(e, e), e
-        },
-        when: function(a) {
-            var b = 0,
-                c = d.call(arguments),
-                e = c.length,
-                f = 1 !== e || a && o.isFunction(a.promise) ? e : 0,
-                g = 1 === f ? a : o.Deferred(),
-                h = function(a, b, c) {
+                s = {};
+            return S.each(o, function(e, t) {
+                var n = t[2],
+                    r = t[5];
+                a[t[1]] = n.add, r && n.add(function() {
+                    i = r
+                }, o[3 - e][2].disable, o[3 - e][3].disable, o[0][2].lock, o[0][3].lock), n.add(t[3].fire), s[t[0]] = function() {
+                    return s[t[0] + "With"](this === s ? void 0 : this, arguments), this
+                }, s[t[0] + "With"] = n.fireWith
+            }), a.promise(s), e && e.call(s, s), s
+        },
+        when: function(e) {
+            var n = arguments.length,
+                t = n,
+                r = Array(t),
+                i = s.call(arguments),
+                o = S.Deferred(),
+                a = function(t) {
                     return function(e) {
-                        b[a] = this, c[a] = arguments.length > 1 ? d.call(arguments) : e, c === i ? g.notifyWith(b, c) : --f || g.resolveWith(b, c)
+                        r[t] = this, i[t] = 1 < arguments.length ? s.call(arguments) : e, --n || o.resolveWith(r, i)
                     }
-                },
-                i, j, k;
-            if (e > 1)
-                for (i = new Array(e), j = new Array(e), k = new Array(e); e > b; b++) c[b] && o.isFunction(c[b].promise) ? c[b].promise().done(h(b, k, c)).fail(g.reject).progress(h(b, j, i)) : --f;
-            return f || g.resolveWith(k, c), g.promise()
+                };
+            if (n <= 1 && (I(e, o.done(a(t)).resolve, o.reject, !n), "pending" === o.state() || m(i[t] && i[t].then))) return o.then();
+            while (t--) I(i[t], a(t), o.reject);
+            return o.promise()
         }
     });
-    var H;
-    o.fn.ready = function(a) {
-        return o.ready.promise().done(a), this
-    }, o.extend({
+    var W = /^(Eval|Internal|Range|Reference|Syntax|Type|URI)Error$/;
+    S.Deferred.exceptionHook = function(e, t) {
+        C.console && C.console.warn && e && W.test(e.name) && C.console.warn("jQuery.Deferred exception: " + e.message, e.stack, t)
+    }, S.readyException = function(e) {
+        C.setTimeout(function() {
+            throw e
+        })
+    };
+    var F = S.Deferred();
+
+    function $() {
+        E.removeEventListener("DOMContentLoaded", $), C.removeEventListener("load", $), S.ready()
+    }
+    S.fn.ready = function(e) {
+        return F.then(e)["catch"](function(e) {
+            S.readyException(e)
+        }), this
+    }, S.extend({
         isReady: !1,
         readyWait: 1,
-        holdReady: function(a) {
-            a ? o.readyWait++ : o.ready(!0)
-        },
-        ready: function(a) {
-            (a === !0 ? --o.readyWait : o.isReady) || (o.isReady = !0, a !== !0 && --o.readyWait > 0 || (H.resolveWith(m, [o]), o.fn.trigger && o(m).trigger("ready").off("ready")))
+        ready: function(e) {
+            (!0 === e ? --S.readyWait : S.isReady) || (S.isReady = !0) !== e && 0 < --S.readyWait || F.resolveWith(E, [S])
         }
-    });
+    }), S.ready.then = F.then, "complete" === E.readyState || "loading" !== E.readyState && !E.documentElement.doScroll ? C.setTimeout(S.ready) : (E.addEventListener("DOMContentLoaded", $), C.addEventListener("load", $));
+    var B = function(e, t, n, r, i, o, a) {
+            var s = 0,
+                u = e.length,
+                l = null == n;
+            if ("object" === w(n))
+                for (s in i = !0, n) B(e, t, s, n[s], !0, o, a);
+            else if (void 0 !== r && (i = !0, m(r) || (a = !0), l && (a ? (t.call(e, r), t = null) : (l = t, t = function(e, t, n) {
+                    return l.call(S(e), n)
+                })), t))
+                for (; s < u; s++) t(e[s], n, a ? r : r.call(e[s], s, t(e[s], n)));
+            return i ? e : l ? t.call(e) : u ? t(e[0], n) : o
+        },
+        _ = /^-ms-/,
+        z = /-([a-z])/g;
+
+    function U(e, t) {
+        return t.toUpperCase()
+    }
 
-    function I() {
-        m.removeEventListener("DOMContentLoaded", I, !1), a.removeEventListener("load", I, !1), o.ready()
+    function X(e) {
+        return e.replace(_, "ms-").replace(z, U)
     }
-    o.ready.promise = function(b) {
-        return H || (H = o.Deferred(), "complete" === m.readyState ? setTimeout(o.ready) : (m.addEventListener("DOMContentLoaded", I, !1), a.addEventListener("load", I, !1))), H.promise(b)
-    }, o.ready.promise();
-    var J = o.access = function(a, b, c, d, e, f, g) {
-        var h = 0,
-            i = a.length,
-            j = null == c;
-        if ("object" === o.type(c)) {
-            e = !0;
-            for (h in c) o.access(a, b, h, c[h], !0, f, g)
-        } else if (void 0 !== d && (e = !0, o.isFunction(d) || (g = !0), j && (g ? (b.call(a, d), b = null) : (j = b, b = function(a, b, c) {
-                return j.call(o(a), c)
-            })), b))
-            for (; i > h; h++) b(a[h], c, g ? d : d.call(a[h], h, b(a[h], c)));
-        return e ? a : j ? b.call(a) : i ? b(a[0], c) : f
-    };
-    o.acceptData = function(a) {
-        return 1 === a.nodeType || 9 === a.nodeType || !+a.nodeType
+    var V = function(e) {
+        return 1 === e.nodeType || 9 === e.nodeType || !+e.nodeType
     };
 
-    function K() {
-        Object.defineProperty(this.cache = {}, 0, {
-            get: function() {
-                return {}
-            }
-        }), this.expando = o.expando + Math.random()
+    function G() {
+        this.expando = S.expando + G.uid++
     }
-    K.uid = 1, K.accepts = o.acceptData, K.prototype = {
-        key: function(a) {
-            if (!K.accepts(a)) return 0;
-            var b = {},
-                c = a[this.expando];
-            if (!c) {
-                c = K.uid++;
-                try {
-                    b[this.expando] = {
-                        value: c
-                    }, Object.defineProperties(a, b)
-                } catch (d) {
-                    b[this.expando] = c, o.extend(a, b)
-                }
-            }
-            return this.cache[c] || (this.cache[c] = {}), c
-        },
-        set: function(a, b, c) {
-            var d, e = this.key(a),
-                f = this.cache[e];
-            if ("string" == typeof b) f[b] = c;
-            else if (o.isEmptyObject(f)) o.extend(this.cache[e], b);
+    G.uid = 1, G.prototype = {
+        cache: function(e) {
+            var t = e[this.expando];
+            return t || (t = {}, V(e) && (e.nodeType ? e[this.expando] = t : Object.defineProperty(e, this.expando, {
+                value: t,
+                configurable: !0
+            }))), t
+        },
+        set: function(e, t, n) {
+            var r, i = this.cache(e);
+            if ("string" == typeof t) i[X(t)] = n;
             else
-                for (d in b) f[d] = b[d];
-            return f
+                for (r in t) i[X(r)] = t[r];
+            return i
         },
-        get: function(a, b) {
-            var c = this.cache[this.key(a)];
-            return void 0 === b ? c : c[b]
-        },
-        access: function(a, b, c) {
-            var d;
-            return void 0 === b || b && "string" == typeof b && void 0 === c ? (d = this.get(a, b), void 0 !== d ? d : this.get(a, o.camelCase(b))) : (this.set(a, b, c), void 0 !== c ? c : b)
-        },
-        remove: function(a, b) {
-            var c, d, e, f = this.key(a),
-                g = this.cache[f];
-            if (void 0 === b) this.cache[f] = {};
-            else {
-                o.isArray(b) ? d = b.concat(b.map(o.camelCase)) : (e = o.camelCase(b), b in g ? d = [b, e] : (d = e, d = d in g ? [d] : d.match(E) || [])), c = d.length;
-                while (c--) delete g[d[c]]
-            }
+        get: function(e, t) {
+            return void 0 === t ? this.cache(e) : e[this.expando] && e[this.expando][X(t)]
         },
-        hasData: function(a) {
-            return !o.isEmptyObject(this.cache[a[this.expando]] || {})
+        access: function(e, t, n) {
+            return void 0 === t || t && "string" == typeof t && void 0 === n ? this.get(e, t) : (this.set(e, t, n), void 0 !== n ? n : t)
         },
-        discard: function(a) {
-            a[this.expando] && delete this.cache[a[this.expando]]
+        remove: function(e, t) {
+            var n, r = e[this.expando];
+            if (void 0 !== r) {
+                if (void 0 !== t) {
+                    n = (t = Array.isArray(t) ? t.map(X) : (t = X(t)) in r ? [t] : t.match(P) || []).length;
+                    while (n--) delete r[t[n]]
+                }(void 0 === t || S.isEmptyObject(r)) && (e.nodeType ? e[this.expando] = void 0 : delete e[this.expando])
+            }
+        },
+        hasData: function(e) {
+            var t = e[this.expando];
+            return void 0 !== t && !S.isEmptyObject(t)
         }
     };
-    var L = new K,
-        M = new K,
-        N = /^(?:\{[\w\W]*\}|\[[\w\W]*\])$/,
-        O = /([A-Z])/g;
-
-    function P(a, b, c) {
-        var d;
-        if (void 0 === c && 1 === a.nodeType)
-            if (d = "data-" + b.replace(O, "-$1").toLowerCase(), c = a.getAttribute(d), "string" == typeof c) {
+    var Y = new G,
+        Q = new G,
+        J = /^(?:\{[\w\W]*\}|\[[\w\W]*\])$/,
+        K = /[A-Z]/g;
+
+    function Z(e, t, n) {
+        var r, i;
+        if (void 0 === n && 1 === e.nodeType)
+            if (r = "data-" + t.replace(K, "-$&").toLowerCase(), "string" == typeof(n = e.getAttribute(r))) {
                 try {
-                    c = "true" === c ? !0 : "false" === c ? !1 : "null" === c ? null : +c + "" === c ? +c : N.test(c) ? o.parseJSON(c) : c
+                    n = "true" === (i = n) || "false" !== i && ("null" === i ? null : i === +i + "" ? +i : J.test(i) ? JSON.parse(i) : i)
                 } catch (e) {}
-                M.set(a, b, c)
-            } else c = void 0;
-        return c
-    }
-    o.extend({
-        hasData: function(a) {
-            return M.hasData(a) || L.hasData(a)
-        },
-        data: function(a, b, c) {
-            return M.access(a, b, c)
-        },
-        removeData: function(a, b) {
-            M.remove(a, b)
-        },
-        _data: function(a, b, c) {
-            return L.access(a, b, c)
-        },
-        _removeData: function(a, b) {
-            L.remove(a, b)
-        }
-    }), o.fn.extend({
-        data: function(a, b) {
-            var c, d, e, f = this[0],
-                g = f && f.attributes;
-            if (void 0 === a) {
-                if (this.length && (e = M.get(f), 1 === f.nodeType && !L.get(f, "hasDataAttrs"))) {
-                    c = g.length;
-                    while (c--) d = g[c].name, 0 === d.indexOf("data-") && (d = o.camelCase(d.slice(5)), P(f, d, e[d]));
-                    L.set(f, "hasDataAttrs", !0)
-                }
-                return e
-            }
-            return "object" == typeof a ? this.each(function() {
-                M.set(this, a)
-            }) : J(this, function(b) {
-                var c, d = o.camelCase(a);
-                if (f && void 0 === b) {
-                    if (c = M.get(f, a), void 0 !== c) return c;
-                    if (c = M.get(f, d), void 0 !== c) return c;
-                    if (c = P(f, d, void 0), void 0 !== c) return c
-                } else this.each(function() {
-                    var c = M.get(this, d);
-                    M.set(this, d, b), -1 !== a.indexOf("-") && void 0 !== c && M.set(this, a, b)
+                Q.set(e, t, n)
+            } else n = void 0;
+        return n
+    }
+    S.extend({
+        hasData: function(e) {
+            return Q.hasData(e) || Y.hasData(e)
+        },
+        data: function(e, t, n) {
+            return Q.access(e, t, n)
+        },
+        removeData: function(e, t) {
+            Q.remove(e, t)
+        },
+        _data: function(e, t, n) {
+            return Y.access(e, t, n)
+        },
+        _removeData: function(e, t) {
+            Y.remove(e, t)
+        }
+    }), S.fn.extend({
+        data: function(n, e) {
+            var t, r, i, o = this[0],
+                a = o && o.attributes;
+            if (void 0 === n) {
+                if (this.length && (i = Q.get(o), 1 === o.nodeType && !Y.get(o, "hasDataAttrs"))) {
+                    t = a.length;
+                    while (t--) a[t] && 0 === (r = a[t].name).indexOf("data-") && (r = X(r.slice(5)), Z(o, r, i[r]));
+                    Y.set(o, "hasDataAttrs", !0)
+                }
+                return i
+            }
+            return "object" == typeof n ? this.each(function() {
+                Q.set(this, n)
+            }) : B(this, function(e) {
+                var t;
+                if (o && void 0 === e) return void 0 !== (t = Q.get(o, n)) ? t : void 0 !== (t = Z(o, n)) ? t : void 0;
+                this.each(function() {
+                    Q.set(this, n, e)
                 })
-            }, null, b, arguments.length > 1, null, !0)
+            }, null, e, 1 < arguments.length, null, !0)
         },
-        removeData: function(a) {
+        removeData: function(e) {
             return this.each(function() {
-                M.remove(this, a)
+                Q.remove(this, e)
             })
         }
-    }), o.extend({
-        queue: function(a, b, c) {
-            var d;
-            return a ? (b = (b || "fx") + "queue", d = L.get(a, b), c && (!d || o.isArray(c) ? d = L.access(a, b, o.makeArray(c)) : d.push(c)), d || []) : void 0
-        },
-        dequeue: function(a, b) {
-            b = b || "fx";
-            var c = o.queue(a, b),
-                d = c.length,
-                e = c.shift(),
-                f = o._queueHooks(a, b),
-                g = function() {
-                    o.dequeue(a, b)
-                };
-            "inprogress" === e && (e = c.shift(), d--), e && ("fx" === b && c.unshift("inprogress"), delete f.stop, e.call(a, g, f)), !d && f && f.empty.fire()
-        },
-        _queueHooks: function(a, b) {
-            var c = b + "queueHooks";
-            return L.get(a, c) || L.access(a, c, {
-                empty: o.Callbacks("once memory").add(function() {
-                    L.remove(a, [b + "queue", c])
+    }), S.extend({
+        queue: function(e, t, n) {
+            var r;
+            if (e) return t = (t || "fx") + "queue", r = Y.get(e, t), n && (!r || Array.isArray(n) ? r = Y.access(e, t, S.makeArray(n)) : r.push(n)), r || []
+        },
+        dequeue: function(e, t) {
+            t = t || "fx";
+            var n = S.queue(e, t),
+                r = n.length,
+                i = n.shift(),
+                o = S._queueHooks(e, t);
+            "inprogress" === i && (i = n.shift(), r--), i && ("fx" === t && n.unshift("inprogress"), delete o.stop, i.call(e, function() {
+                S.dequeue(e, t)
+            }, o)), !r && o && o.empty.fire()
+        },
+        _queueHooks: function(e, t) {
+            var n = t + "queueHooks";
+            return Y.get(e, n) || Y.access(e, n, {
+                empty: S.Callbacks("once memory").add(function() {
+                    Y.remove(e, [t + "queue", n])
                 })
             })
         }
-    }), o.fn.extend({
-        queue: function(a, b) {
-            var c = 2;
-            return "string" != typeof a && (b = a, a = "fx", c--), arguments.length < c ? o.queue(this[0], a) : void 0 === b ? this : this.each(function() {
-                var c = o.queue(this, a, b);
-                o._queueHooks(this, a), "fx" === a && "inprogress" !== c[0] && o.dequeue(this, a)
+    }), S.fn.extend({
+        queue: function(t, n) {
+            var e = 2;
+            return "string" != typeof t && (n = t, t = "fx", e--), arguments.length < e ? S.queue(this[0], t) : void 0 === n ? this : this.each(function() {
+                var e = S.queue(this, t, n);
+                S._queueHooks(this, t), "fx" === t && "inprogress" !== e[0] && S.dequeue(this, t)
             })
         },
-        dequeue: function(a) {
+        dequeue: function(e) {
             return this.each(function() {
-                o.dequeue(this, a)
+                S.dequeue(this, e)
             })
         },
-        clearQueue: function(a) {
-            return this.queue(a || "fx", [])
+        clearQueue: function(e) {
+            return this.queue(e || "fx", [])
         },
-        promise: function(a, b) {
-            var c, d = 1,
-                e = o.Deferred(),
-                f = this,
-                g = this.length,
-                h = function() {
-                    --d || e.resolveWith(f, [f])
+        promise: function(e, t) {
+            var n, r = 1,
+                i = S.Deferred(),
+                o = this,
+                a = this.length,
+                s = function() {
+                    --r || i.resolveWith(o, [o])
                 };
-            "string" != typeof a && (b = a, a = void 0), a = a || "fx";
-            while (g--) c = L.get(f[g], a + "queueHooks"), c && c.empty && (d++, c.empty.add(h));
-            return h(), e.promise(b)
+            "string" != typeof e && (t = e, e = void 0), e = e || "fx";
+            while (a--)(n = Y.get(o[a], e + "queueHooks")) && n.empty && (r++, n.empty.add(s));
+            return s(), i.promise(t)
         }
     });
-    var Q = /[+-]?(?:\d*\.|)\d+(?:[eE][+-]?\d+|)/.source,
-        R = ["Top", "Right", "Bottom", "Left"],
-        S = function(a, b) {
-            return a = b || a, "none" === o.css(a, "display") || !o.contains(a.ownerDocument, a)
-        },
-        T = /^(?:checkbox|radio)$/i;
-    ! function() {
-        var a = m.createDocumentFragment(),
-            b = a.appendChild(m.createElement("div"));
-        b.innerHTML = "<input type='radio' checked='checked' name='t'/>", l.checkClone = b.cloneNode(!0).cloneNode(!0).lastChild.checked, b.innerHTML = "<textarea>x</textarea>", l.noCloneChecked = !!b.cloneNode(!0).lastChild.defaultValue
-    }();
-    var U = "undefined";
-    l.focusinBubbles = "onfocusin" in a;
-    var V = /^key/,
-        W = /^(?:mouse|contextmenu)|click/,
-        X = /^(?:focusinfocus|focusoutblur)$/,
-        Y = /^([^.]*)(?:\.(.+)|)$/;
+    var ee = /[+-]?(?:\d*\.|)\d+(?:[eE][+-]?\d+|)/.source,
+        te = new RegExp("^(?:([+-])=|)(" + ee + ")([a-z%]*)$", "i"),
+        ne = ["Top", "Right", "Bottom", "Left"],
+        re = E.documentElement,
+        ie = function(e) {
+            return S.contains(e.ownerDocument, e)
+        },
+        oe = {
+            composed: !0
+        };
+    re.getRootNode && (ie = function(e) {
+        return S.contains(e.ownerDocument, e) || e.getRootNode(oe) === e.ownerDocument
+    });
+    var ae = function(e, t) {
+        return "none" === (e = t || e).style.display || "" === e.style.display && ie(e) && "none" === S.css(e, "display")
+    };
 
-    function Z() {
+    function se(e, t, n, r) {
+        var i, o, a = 20,
+            s = r ? function() {
+                return r.cur()
+            } : function() {
+                return S.css(e, t, "")
+            },
+            u = s(),
+            l = n && n[3] || (S.cssNumber[t] ? "" : "px"),
+            c = e.nodeType && (S.cssNumber[t] || "px" !== l && +u) && te.exec(S.css(e, t));
+        if (c && c[3] !== l) {
+            u /= 2, l = l || c[3], c = +u || 1;
+            while (a--) S.style(e, t, c + l), (1 - o) * (1 - (o = s() / u || .5)) <= 0 && (a = 0), c /= o;
+            c *= 2, S.style(e, t, c + l), n = n || []
+        }
+        return n && (c = +c || +u || 0, i = n[1] ? c + (n[1] + 1) * n[2] : +n[2], r && (r.unit = l, r.start = c, r.end = i)), i
+    }
+    var ue = {};
+
+    function le(e, t) {
+        for (var n, r, i, o, a, s, u, l = [], c = 0, f = e.length; c < f; c++)(r = e[c]).style && (n = r.style.display, t ? ("none" === n && (l[c] = Y.get(r, "display") || null, l[c] || (r.style.display = "")), "" === r.style.display && ae(r) && (l[c] = (u = a = o = void 0, a = (i = r).ownerDocument, s = i.nodeName, (u = ue[s]) || (o = a.body.appendChild(a.createElement(s)), u = S.css(o, "display"), o.parentNode.removeChild(o), "none" === u && (u = "block"), ue[s] = u)))) : "none" !== n && (l[c] = "none", Y.set(r, "display", n)));
+        for (c = 0; c < f; c++) null != l[c] && (e[c].style.display = l[c]);
+        return e
+    }
+    S.fn.extend({
+        show: function() {
+            return le(this, !0)
+        },
+        hide: function() {
+            return le(this)
+        },
+        toggle: function(e) {
+            return "boolean" == typeof e ? e ? this.show() : this.hide() : this.each(function() {
+                ae(this) ? S(this).show() : S(this).hide()
+            })
+        }
+    });
+    var ce, fe, pe = /^(?:checkbox|radio)$/i,
+        de = /<([a-z][^\/\0>\x20\t\r\n\f]*)/i,
+        he = /^$|^module$|\/(?:java|ecma)script/i;
+    ce = E.createDocumentFragment().appendChild(E.createElement("div")), (fe = E.createElement("input")).setAttribute("type", "radio"), fe.setAttribute("checked", "checked"), fe.setAttribute("name", "t"), ce.appendChild(fe), v.checkClone = ce.cloneNode(!0).cloneNode(!0).lastChild.checked, ce.innerHTML = "<textarea>x</textarea>", v.noCloneChecked = !!ce.cloneNode(!0).lastChild.defaultValue, ce.innerHTML = "<option></option>", v.option = !!ce.lastChild;
+    var ge = {
+        thead: [1, "<table>", "</table>"],
+        col: [2, "<table><colgroup>", "</colgroup></table>"],
+        tr: [2, "<table><tbody>", "</tbody></table>"],
+        td: [3, "<table><tbody><tr>", "</tr></tbody></table>"],
+        _default: [0, "", ""]
+    };
+
+    function ye(e, t) {
+        var n;
+        return n = "undefined" != typeof e.getElementsByTagName ? e.getElementsByTagName(t || "*") : "undefined" != typeof e.querySelectorAll ? e.querySelectorAll(t || "*") : [], void 0 === t || t && A(e, t) ? S.merge([e], n) : n
+    }
+
+    function ve(e, t) {
+        for (var n = 0, r = e.length; n < r; n++) Y.set(e[n], "globalEval", !t || Y.get(t[n], "globalEval"))
+    }
+    ge.tbody = ge.tfoot = ge.colgroup = ge.caption = ge.thead, ge.th = ge.td, v.option || (ge.optgroup = ge.option = [1, "<select multiple='multiple'>", "</select>"]);
+    var me = /<|&#?\w+;/;
+
+    function xe(e, t, n, r, i) {
+        for (var o, a, s, u, l, c, f = t.createDocumentFragment(), p = [], d = 0, h = e.length; d < h; d++)
+            if ((o = e[d]) || 0 === o)
+                if ("object" === w(o)) S.merge(p, o.nodeType ? [o] : o);
+                else if (me.test(o)) {
+            a = a || f.appendChild(t.createElement("div")), s = (de.exec(o) || ["", ""])[1].toLowerCase(), u = ge[s] || ge._default, a.innerHTML = u[1] + S.htmlPrefilter(o) + u[2], c = u[0];
+            while (c--) a = a.lastChild;
+            S.merge(p, a.childNodes), (a = f.firstChild).textContent = ""
+        } else p.push(t.createTextNode(o));
+        f.textContent = "", d = 0;
+        while (o = p[d++])
+            if (r && -1 < S.inArray(o, r)) i && i.push(o);
+            else if (l = ie(o), a = ye(f.appendChild(o), "script"), l && ve(a), n) {
+            c = 0;
+            while (o = a[c++]) he.test(o.type || "") && n.push(o)
+        }
+        return f
+    }
+    var be = /^([^.]*)(?:\.(.+)|)/;
+
+    function we() {
         return !0
     }
 
-    function $() {
+    function Te() {
         return !1
     }
 
-    function _() {
-        try {
-            return m.activeElement
-        } catch (a) {}
+    function Ce(e, t) {
+        return e === function() {
+            try {
+                return E.activeElement
+            } catch (e) {}
+        }() == ("focus" === t)
+    }
+
+    function Ee(e, t, n, r, i, o) {
+        var a, s;
+        if ("object" == typeof t) {
+            for (s in "string" != typeof n && (r = r || n, n = void 0), t) Ee(e, s, n, r, t[s], o);
+            return e
+        }
+        if (null == r && null == i ? (i = n, r = n = void 0) : null == i && ("string" == typeof n ? (i = r, r = void 0) : (i = r, r = n, n = void 0)), !1 === i) i = Te;
+        else if (!i) return e;
+        return 1 === o && (a = i, (i = function(e) {
+            return S().off(e), a.apply(this, arguments)
+        }).guid = a.guid || (a.guid = S.guid++)), e.each(function() {
+            S.event.add(this, t, i, r, n)
+        })
+    }
+
+    function Se(e, i, o) {
+        o ? (Y.set(e, i, !1), S.event.add(e, i, {
+            namespace: !1,
+            handler: function(e) {
+                var t, n, r = Y.get(this, i);
+                if (1 & e.isTrigger && this[i]) {
+                    if (r.length)(S.event.special[i] || {}).delegateType && e.stopPropagation();
+                    else if (r = s.call(arguments), Y.set(this, i, r), t = o(this, i), this[i](), r !== (n = Y.get(this, i)) || t ? Y.set(this, i, !1) : n = {}, r !== n) return e.stopImmediatePropagation(), e.preventDefault(), n && n.value
+                } else r.length && (Y.set(this, i, {
+                    value: S.event.trigger(S.extend(r[0], S.Event.prototype), r.slice(1), this)
+                }), e.stopImmediatePropagation())
+            }
+        })) : void 0 === Y.get(e, i) && S.event.add(e, i, we)
     }
-    o.event = {
+    S.event = {
         global: {},
-        add: function(a, b, c, d, e) {
-            var f, g, h, i, j, k, l, m, n, p, q, r = L.get(a);
-            if (r) {
-                c.handler && (f = c, c = f.handler, e = f.selector), c.guid || (c.guid = o.guid++), (i = r.events) || (i = r.events = {}), (g = r.handle) || (g = r.handle = function(b) {
-                    return typeof o !== U && o.event.triggered !== b.type ? o.event.dispatch.apply(a, arguments) : void 0
-                }), b = (b || "").match(E) || [""], j = b.length;
-                while (j--) h = Y.exec(b[j]) || [], n = q = h[1], p = (h[2] || "").split(".").sort(), n && (l = o.event.special[n] || {}, n = (e ? l.delegateType : l.bindType) || n, l = o.event.special[n] || {}, k = o.extend({
-                    type: n,
-                    origType: q,
-                    data: d,
-                    handler: c,
-                    guid: c.guid,
-                    selector: e,
-                    needsContext: e && o.expr.match.needsContext.test(e),
-                    namespace: p.join(".")
-                }, f), (m = i[n]) || (m = i[n] = [], m.delegateCount = 0, l.setup && l.setup.call(a, d, p, g) !== !1 || a.addEventListener && a.addEventListener(n, g, !1)), l.add && (l.add.call(a, k), k.handler.guid || (k.handler.guid = c.guid)), e ? m.splice(m.delegateCount++, 0, k) : m.push(k), o.event.global[n] = !0)
-            }
-        },
-        remove: function(a, b, c, d, e) {
-            var f, g, h, i, j, k, l, m, n, p, q, r = L.hasData(a) && L.get(a);
-            if (r && (i = r.events)) {
-                b = (b || "").match(E) || [""], j = b.length;
-                while (j--)
-                    if (h = Y.exec(b[j]) || [], n = q = h[1], p = (h[2] || "").split(".").sort(), n) {
-                        l = o.event.special[n] || {}, n = (d ? l.delegateType : l.bindType) || n, m = i[n] || [], h = h[2] && new RegExp("(^|\\.)" + p.join("\\.(?:.*\\.|)") + "(\\.|$)"), g = f = m.length;
-                        while (f--) k = m[f], !e && q !== k.origType || c && c.guid !== k.guid || h && !h.test(k.namespace) || d && d !== k.selector && ("**" !== d || !k.selector) || (m.splice(f, 1), k.selector && m.delegateCount--, l.remove && l.remove.call(a, k));
-                        g && !m.length && (l.teardown && l.teardown.call(a, p, r.handle) !== !1 || o.removeEvent(a, n, r.handle), delete i[n])
+        add: function(t, e, n, r, i) {
+            var o, a, s, u, l, c, f, p, d, h, g, y = Y.get(t);
+            if (V(t)) {
+                n.handler && (n = (o = n).handler, i = o.selector), i && S.find.matchesSelector(re, i), n.guid || (n.guid = S.guid++), (u = y.events) || (u = y.events = Object.create(null)), (a = y.handle) || (a = y.handle = function(e) {
+                    return "undefined" != typeof S && S.event.triggered !== e.type ? S.event.dispatch.apply(t, arguments) : void 0
+                }), l = (e = (e || "").match(P) || [""]).length;
+                while (l--) d = g = (s = be.exec(e[l]) || [])[1], h = (s[2] || "").split(".").sort(), d && (f = S.event.special[d] || {}, d = (i ? f.delegateType : f.bindType) || d, f = S.event.special[d] || {}, c = S.extend({
+                    type: d,
+                    origType: g,
+                    data: r,
+                    handler: n,
+                    guid: n.guid,
+                    selector: i,
+                    needsContext: i && S.expr.match.needsContext.test(i),
+                    namespace: h.join(".")
+                }, o), (p = u[d]) || ((p = u[d] = []).delegateCount = 0, f.setup && !1 !== f.setup.call(t, r, h, a) || t.addEventListener && t.addEventListener(d, a)), f.add && (f.add.call(t, c), c.handler.guid || (c.handler.guid = n.guid)), i ? p.splice(p.delegateCount++, 0, c) : p.push(c), S.event.global[d] = !0)
+            }
+        },
+        remove: function(e, t, n, r, i) {
+            var o, a, s, u, l, c, f, p, d, h, g, y = Y.hasData(e) && Y.get(e);
+            if (y && (u = y.events)) {
+                l = (t = (t || "").match(P) || [""]).length;
+                while (l--)
+                    if (d = g = (s = be.exec(t[l]) || [])[1], h = (s[2] || "").split(".").sort(), d) {
+                        f = S.event.special[d] || {}, p = u[d = (r ? f.delegateType : f.bindType) || d] || [], s = s[2] && new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)"), a = o = p.length;
+                        while (o--) c = p[o], !i && g !== c.origType || n && n.guid !== c.guid || s && !s.test(c.namespace) || r && r !== c.selector && ("**" !== r || !c.selector) || (p.splice(o, 1), c.selector && p.delegateCount--, f.remove && f.remove.call(e, c));
+                        a && !p.length && (f.teardown && !1 !== f.teardown.call(e, h, y.handle) || S.removeEvent(e, d, y.handle), delete u[d])
                     } else
-                        for (n in i) o.event.remove(a, n + b[j], c, d, !0);
-                o.isEmptyObject(i) && (delete r.handle, L.remove(a, "events"))
+                        for (d in u) S.event.remove(e, d + t[l], n, r, !0);
+                S.isEmptyObject(u) && Y.remove(e, "handle events")
             }
         },
-        trigger: function(b, c, d, e) {
-            var f, g, h, i, k, l, n, p = [d || m],
-                q = j.call(b, "type") ? b.type : b,
-                r = j.call(b, "namespace") ? b.namespace.split(".") : [];
-            if (g = h = d = d || m, 3 !== d.nodeType && 8 !== d.nodeType && !X.test(q + o.event.triggered) && (q.indexOf(".") >= 0 && (r = q.split("."), q = r.shift(), r.sort()), k = q.indexOf(":") < 0 && "on" + q, b = b[o.expando] ? b : new o.Event(q, "object" == typeof b && b), b.isTrigger = e ? 2 : 3, b.namespace = r.join("."), b.namespace_re = b.namespace ? new RegExp("(^|\\.)" + r.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, b.result = void 0, b.target || (b.target = d), c = null == c ? [b] : o.makeArray(c, [b]), n = o.event.special[q] || {}, e || !n.trigger || n.trigger.apply(d, c) !== !1)) {
-                if (!e && !n.noBubble && !o.isWindow(d)) {
-                    for (i = n.delegateType || q, X.test(i + q) || (g = g.parentNode); g; g = g.parentNode) p.push(g), h = g;
-                    h === (d.ownerDocument || m) && p.push(h.defaultView || h.parentWindow || a)
-                }
-                f = 0;
-                while ((g = p[f++]) && !b.isPropagationStopped()) b.type = f > 1 ? i : n.bindType || q, l = (L.get(g, "events") || {})[b.type] && L.get(g, "handle"), l && l.apply(g, c), l = k && g[k], l && l.apply && o.acceptData(g) && (b.result = l.apply(g, c), b.result === !1 && b.preventDefault());
-                return b.type = q, e || b.isDefaultPrevented() || n._default && n._default.apply(p.pop(), c) !== !1 || !o.acceptData(d) || k && o.isFunction(d[q]) && !o.isWindow(d) && (h = d[k], h && (d[k] = null), o.event.triggered = q, d[q](), o.event.triggered = void 0, h && (d[k] = h)), b.result
-            }
-        },
-        dispatch: function(a) {
-            a = o.event.fix(a);
-            var b, c, e, f, g, h = [],
-                i = d.call(arguments),
-                j = (L.get(this, "events") || {})[a.type] || [],
-                k = o.event.special[a.type] || {};
-            if (i[0] = a, a.delegateTarget = this, !k.preDispatch || k.preDispatch.call(this, a) !== !1) {
-                h = o.event.handlers.call(this, a, j), b = 0;
-                while ((f = h[b++]) && !a.isPropagationStopped()) {
-                    a.currentTarget = f.elem, c = 0;
-                    while ((g = f.handlers[c++]) && !a.isImmediatePropagationStopped())(!a.namespace_re || a.namespace_re.test(g.namespace)) && (a.handleObj = g, a.data = g.data, e = ((o.event.special[g.origType] || {}).handle || g.handler).apply(f.elem, i), void 0 !== e && (a.result = e) === !1 && (a.preventDefault(), a.stopPropagation()))
-                }
-                return k.postDispatch && k.postDispatch.call(this, a), a.result
-            }
-        },
-        handlers: function(a, b) {
-            var c, d, e, f, g = [],
-                h = b.delegateCount,
-                i = a.target;
-            if (h && i.nodeType && (!a.button || "click" !== a.type))
-                for (; i !== this; i = i.parentNode || this)
-                    if (i.disabled !== !0 || "click" !== a.type) {
-                        for (d = [], c = 0; h > c; c++) f = b[c], e = f.selector + " ", void 0 === d[e] && (d[e] = f.needsContext ? o(e, this).index(i) >= 0 : o.find(e, this, null, [i]).length), d[e] && d.push(f);
-                        d.length && g.push({
-                            elem: i,
-                            handlers: d
+        dispatch: function(e) {
+            var t, n, r, i, o, a, s = new Array(arguments.length),
+                u = S.event.fix(e),
+                l = (Y.get(this, "events") || Object.create(null))[u.type] || [],
+                c = S.event.special[u.type] || {};
+            for (s[0] = u, t = 1; t < arguments.length; t++) s[t] = arguments[t];
+            if (u.delegateTarget = this, !c.preDispatch || !1 !== c.preDispatch.call(this, u)) {
+                a = S.event.handlers.call(this, u, l), t = 0;
+                while ((i = a[t++]) && !u.isPropagationStopped()) {
+                    u.currentTarget = i.elem, n = 0;
+                    while ((o = i.handlers[n++]) && !u.isImmediatePropagationStopped()) u.rnamespace && !1 !== o.namespace && !u.rnamespace.test(o.namespace) || (u.handleObj = o, u.data = o.data, void 0 !== (r = ((S.event.special[o.origType] || {}).handle || o.handler).apply(i.elem, s)) && !1 === (u.result = r) && (u.preventDefault(), u.stopPropagation()))
+                }
+                return c.postDispatch && c.postDispatch.call(this, u), u.result
+            }
+        },
+        handlers: function(e, t) {
+            var n, r, i, o, a, s = [],
+                u = t.delegateCount,
+                l = e.target;
+            if (u && l.nodeType && !("click" === e.type && 1 <= e.button))
+                for (; l !== this; l = l.parentNode || this)
+                    if (1 === l.nodeType && ("click" !== e.type || !0 !== l.disabled)) {
+                        for (o = [], a = {}, n = 0; n < u; n++) void 0 === a[i = (r = t[n]).selector + " "] && (a[i] = r.needsContext ? -1 < S(i, this).index(l) : S.find(i, this, null, [l]).length), a[i] && o.push(r);
+                        o.length && s.push({
+                            elem: l,
+                            handlers: o
                         })
-                    } return h < b.length && g.push({
-                elem: this,
-                handlers: b.slice(h)
-            }), g
-        },
-        props: "altKey bubbles cancelable ctrlKey currentTarget eventPhase metaKey relatedTarget shiftKey target timeStamp view which".split(" "),
-        fixHooks: {},
-        keyHooks: {
-            props: "char charCode key keyCode".split(" "),
-            filter: function(a, b) {
-                return null == a.which && (a.which = null != b.charCode ? b.charCode : b.keyCode), a
-            }
-        },
-        mouseHooks: {
-            props: "button buttons clientX clientY offsetX offsetY pageX pageY screenX screenY toElement".split(" "),
-            filter: function(a, b) {
-                var c, d, e, f = b.button;
-                return null == a.pageX && null != b.clientX && (c = a.target.ownerDocument || m, d = c.documentElement, e = c.body, a.pageX = b.clientX + (d && d.scrollLeft || e && e.scrollLeft || 0) - (d && d.clientLeft || e && e.clientLeft || 0), a.pageY = b.clientY + (d && d.scrollTop || e && e.scrollTop || 0) - (d && d.clientTop || e && e.clientTop || 0)), a.which || void 0 === f || (a.which = 1 & f ? 1 : 2 & f ? 3 : 4 & f ? 2 : 0), a
-            }
-        },
-        fix: function(a) {
-            if (a[o.expando]) return a;
-            var b, c, d, e = a.type,
-                f = a,
-                g = this.fixHooks[e];
-            g || (this.fixHooks[e] = g = W.test(e) ? this.mouseHooks : V.test(e) ? this.keyHooks : {}), d = g.props ? this.props.concat(g.props) : this.props, a = new o.Event(f), b = d.length;
-            while (b--) c = d[b], a[c] = f[c];
-            return a.target || (a.target = m), 3 === a.target.nodeType && (a.target = a.target.parentNode), g.filter ? g.filter(a, f) : a
+                    } return l = this, u < t.length && s.push({
+                elem: l,
+                handlers: t.slice(u)
+            }), s
+        },
+        addProp: function(t, e) {
+            Object.defineProperty(S.Event.prototype, t, {
+                enumerable: !0,
+                configurable: !0,
+                get: m(e) ? function() {
+                    if (this.originalEvent) return e(this.originalEvent)
+                } : function() {
+                    if (this.originalEvent) return this.originalEvent[t]
+                },
+                set: function(e) {
+                    Object.defineProperty(this, t, {
+                        enumerable: !0,
+                        configurable: !0,
+                        writable: !0,
+                        value: e
+                    })
+                }
+            })
+        },
+        fix: function(e) {
+            return e[S.expando] ? e : new S.Event(e)
         },
         special: {
             load: {
                 noBubble: !0
             },
-            focus: {
-                trigger: function() {
-                    return this !== _() && this.focus ? (this.focus(), !1) : void 0
-                },
-                delegateType: "focusin"
-            },
-            blur: {
-                trigger: function() {
-                    return this === _() && this.blur ? (this.blur(), !1) : void 0
-                },
-                delegateType: "focusout"
-            },
             click: {
-                trigger: function() {
-                    return "checkbox" === this.type && this.click && o.nodeName(this, "input") ? (this.click(), !1) : void 0
-                },
-                _default: function(a) {
-                    return o.nodeName(a.target, "a")
+                setup: function(e) {
+                    var t = this || e;
+                    return pe.test(t.type) && t.click && A(t, "input") && Se(t, "click", we), !1
+                },
+                trigger: function(e) {
+                    var t = this || e;
+                    return pe.test(t.type) && t.click && A(t, "input") && Se(t, "click"), !0
+                },
+                _default: function(e) {
+                    var t = e.target;
+                    return pe.test(t.type) && t.click && A(t, "input") && Y.get(t, "click") || A(t, "a")
                 }
             },
             beforeunload: {
-                postDispatch: function(a) {
-                    void 0 !== a.result && (a.originalEvent.returnValue = a.result)
+                postDispatch: function(e) {
+                    void 0 !== e.result && e.originalEvent && (e.originalEvent.returnValue = e.result)
                 }
             }
-        },
-        simulate: function(a, b, c, d) {
-            var e = o.extend(new o.Event, c, {
-                type: a,
-                isSimulated: !0,
-                originalEvent: {}
-            });
-            d ? o.event.trigger(e, null, b) : o.event.dispatch.call(b, e), e.isDefaultPrevented() && c.preventDefault()
         }
-    }, o.removeEvent = function(a, b, c) {
-        a.removeEventListener && a.removeEventListener(b, c, !1)
-    }, o.Event = function(a, b) {
-        return this instanceof o.Event ? (a && a.type ? (this.originalEvent = a, this.type = a.type, this.isDefaultPrevented = a.defaultPrevented || void 0 === a.defaultPrevented && a.getPreventDefault && a.getPreventDefault() ? Z : $) : this.type = a, b && o.extend(this, b), this.timeStamp = a && a.timeStamp || o.now(), void(this[o.expando] = !0)) : new o.Event(a, b)
-    }, o.Event.prototype = {
-        isDefaultPrevented: $,
-        isPropagationStopped: $,
-        isImmediatePropagationStopped: $,
+    }, S.removeEvent = function(e, t, n) {
+        e.removeEventListener && e.removeEventListener(t, n)
+    }, S.Event = function(e, t) {
+        if (!(this instanceof S.Event)) return new S.Event(e, t);
+        e && e.type ? (this.originalEvent = e, this.type = e.type, this.isDefaultPrevented = e.defaultPrevented || void 0 === e.defaultPrevented && !1 === e.returnValue ? we : Te, this.target = e.target && 3 === e.target.nodeType ? e.target.parentNode : e.target, this.currentTarget = e.currentTarget, this.relatedTarget = e.relatedTarget) : this.type = e, t && S.extend(this, t), this.timeStamp = e && e.timeStamp || Date.now(), this[S.expando] = !0
+    }, S.Event.prototype = {
+        constructor: S.Event,
+        isDefaultPrevented: Te,
+        isPropagationStopped: Te,
+        isImmediatePropagationStopped: Te,
+        isSimulated: !1,
         preventDefault: function() {
-            var a = this.originalEvent;
-            this.isDefaultPrevented = Z, a && a.preventDefault && a.preventDefault()
+            var e = this.originalEvent;
+            this.isDefaultPrevented = we, e && !this.isSimulated && e.preventDefault()
         },
         stopPropagation: function() {
-            var a = this.originalEvent;
-            this.isPropagationStopped = Z, a && a.stopPropagation && a.stopPropagation()
+            var e = this.originalEvent;
+            this.isPropagationStopped = we, e && !this.isSimulated && e.stopPropagation()
         },
         stopImmediatePropagation: function() {
-            this.isImmediatePropagationStopped = Z, this.stopPropagation()
-        }
-    }, o.each({
-        mouseenter: "mouseover",
-        mouseleave: "mouseout"
-    }, function(a, b) {
-        o.event.special[a] = {
-            delegateType: b,
-            bindType: b,
-            handle: function(a) {
-                var c, d = this,
-                    e = a.relatedTarget,
-                    f = a.handleObj;
-                return (!e || e !== d && !o.contains(d, e)) && (a.type = f.origType, c = f.handler.apply(this, arguments), a.type = b), c
-            }
+            var e = this.originalEvent;
+            this.isImmediatePropagationStopped = we, e && !this.isSimulated && e.stopImmediatePropagation(), this.stopPropagation()
         }
-    }), l.focusinBubbles || o.each({
+    }, S.each({
+        altKey: !0,
+        bubbles: !0,
+        cancelable: !0,
+        changedTouches: !0,
+        ctrlKey: !0,
+        detail: !0,
+        eventPhase: !0,
+        metaKey: !0,
+        pageX: !0,
+        pageY: !0,
+        shiftKey: !0,
+        view: !0,
+        "char": !0,
+        code: !0,
+        charCode: !0,
+        key: !0,
+        keyCode: !0,
+        button: !0,
+        buttons: !0,
+        clientX: !0,
+        clientY: !0,
+        offsetX: !0,
+        offsetY: !0,
+        pointerId: !0,
+        pointerType: !0,
+        screenX: !0,
+        screenY: !0,
+        targetTouches: !0,
+        toElement: !0,
+        touches: !0,
+        which: !0
+    }, S.event.addProp), S.each({
         focus: "focusin",
         blur: "focusout"
-    }, function(a, b) {
-        var c = function(a) {
-            o.event.simulate(b, a.target, o.event.fix(a), !0)
-        };
-        o.event.special[b] = {
+    }, function(t, e) {
+        S.event.special[t] = {
             setup: function() {
-                var d = this.ownerDocument || this,
-                    e = L.access(d, b);
-                e || d.addEventListener(a, c, !0), L.access(d, b, (e || 0) + 1)
+                return Se(this, t, Ce), !1
             },
-            teardown: function() {
-                var d = this.ownerDocument || this,
-                    e = L.access(d, b) - 1;
-                e ? L.access(d, b, e) : (d.removeEventListener(a, c, !0), L.remove(d, b))
-            }
+            trigger: function() {
+                return Se(this, t), !0
+            },
+            _default: function(e) {
+                return Y.get(e.target, t)
+            },
+            delegateType: e
         }
-    }), o.fn.extend({
-        on: function(a, b, c, d, e) {
-            var f, g;
-            if ("object" == typeof a) {
-                "string" != typeof b && (c = c || b, b = void 0);
-                for (g in a) this.on(g, b, c, a[g], e);
-                return this
-            }
-            if (null == c && null == d ? (d = b, c = b = void 0) : null == d && ("string" == typeof b ? (d = c, c = void 0) : (d = c, c = b, b = void 0)), d === !1) d = $;
-            else if (!d) return this;
-            return 1 === e && (f = d, d = function(a) {
-                return o().off(a), f.apply(this, arguments)
-            }, d.guid = f.guid || (f.guid = o.guid++)), this.each(function() {
-                o.event.add(this, a, d, c, b)
-            })
-        },
-        one: function(a, b, c, d) {
-            return this.on(a, b, c, d, 1)
-        },
-        off: function(a, b, c) {
-            var d, e;
-            if (a && a.preventDefault && a.handleObj) return d = a.handleObj, o(a.delegateTarget).off(d.namespace ? d.origType + "." + d.namespace : d.origType, d.selector, d.handler), this;
-            if ("object" == typeof a) {
-                for (e in a) this.off(e, b, a[e]);
+    }), S.each({
+        mouseenter: "mouseover",
+        mouseleave: "mouseout",
+        pointerenter: "pointerover",
+        pointerleave: "pointerout"
+    }, function(e, i) {
+        S.event.special[e] = {
+            delegateType: i,
+            bindType: i,
+            handle: function(e) {
+                var t, n = e.relatedTarget,
+                    r = e.handleObj;
+                return n && (n === this || S.contains(this, n)) || (e.type = r.origType, t = r.handler.apply(this, arguments), e.type = i), t
+            }
+        }
+    }), S.fn.extend({
+        on: function(e, t, n, r) {
+            return Ee(this, e, t, n, r)
+        },
+        one: function(e, t, n, r) {
+            return Ee(this, e, t, n, r, 1)
+        },
+        off: function(e, t, n) {
+            var r, i;
+            if (e && e.preventDefault && e.handleObj) return r = e.handleObj, S(e.delegateTarget).off(r.namespace ? r.origType + "." + r.namespace : r.origType, r.selector, r.handler), this;
+            if ("object" == typeof e) {
+                for (i in e) this.off(i, t, e[i]);
                 return this
             }
-            return (b === !1 || "function" == typeof b) && (c = b, b = void 0), c === !1 && (c = $), this.each(function() {
-                o.event.remove(this, a, c, b)
+            return !1 !== t && "function" != typeof t || (n = t, t = void 0), !1 === n && (n = Te), this.each(function() {
+                S.event.remove(this, e, n, t)
             })
-        },
-        trigger: function(a, b) {
-            return this.each(function() {
-                o.event.trigger(a, b, this)
-            })
-        },
-        triggerHandler: function(a, b) {
-            var c = this[0];
-            return c ? o.event.trigger(a, b, c, !0) : void 0
         }
     });
-    var ab = /<(?!area|br|col|embed|hr|img|input|link|meta|param)(([\w:]+)[^>]*)\/>/gi,
-        bb = /<([\w:]+)/,
-        cb = /<|&#?\w+;/,
-        db = /<(?:script|style|link)/i,
-        eb = /checked\s*(?:[^=]|=\s*.checked.)/i,
-        fb = /^$|\/(?:java|ecma)script/i,
-        gb = /^true\/(.*)/,
-        hb = /^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g,
-        ib = {
-            option: [1, "<select multiple='multiple'>", "</select>"],
-            thead: [1, "<table>", "</table>"],
-            col: [2, "<table><colgroup>", "</colgroup></table>"],
-            tr: [2, "<table><tbody>", "</tbody></table>"],
-            td: [3, "<table><tbody><tr>", "</tr></tbody></table>"],
-            _default: [0, "", ""]
-        };
-    ib.optgroup = ib.option, ib.tbody = ib.tfoot = ib.colgroup = ib.caption = ib.thead, ib.th = ib.td;
+    var ke = /<script|<style|<link/i,
+        Ae = /checked\s*(?:[^=]|=\s*.checked.)/i,
+        Ne = /^\s*<!\[CDATA\[|\]\]>\s*$/g;
 
-    function jb(a, b) {
-        return o.nodeName(a, "table") && o.nodeName(11 !== b.nodeType ? b : b.firstChild, "tr") ? a.getElementsByTagName("tbody")[0] || a.appendChild(a.ownerDocument.createElement("tbody")) : a
+    function je(e, t) {
+        return A(e, "table") && A(11 !== t.nodeType ? t : t.firstChild, "tr") && S(e).children("tbody")[0] || e
     }
 
-    function kb(a) {
-        return a.type = (null !== a.getAttribute("type")) + "/" + a.type, a
+    function De(e) {
+        return e.type = (null !== e.getAttribute("type")) + "/" + e.type, e
     }
 
-    function lb(a) {
-        var b = gb.exec(a.type);
-        return b ? a.type = b[1] : a.removeAttribute("type"), a
+    function qe(e) {
+        return "true/" === (e.type || "").slice(0, 5) ? e.type = e.type.slice(5) : e.removeAttribute("type"), e
     }
 
-    function mb(a, b) {
-        for (var c = 0, d = a.length; d > c; c++) L.set(a[c], "globalEval", !b || L.get(b[c], "globalEval"))
-    }
-
-    function nb(a, b) {
-        var c, d, e, f, g, h, i, j;
-        if (1 === b.nodeType) {
-            if (L.hasData(a) && (f = L.access(a), g = L.set(b, f), j = f.events)) {
-                delete g.handle, g.events = {};
-                for (e in j)
-                    for (c = 0, d = j[e].length; d > c; c++) o.event.add(b, e, j[e][c])
-            }
-            M.hasData(a) && (h = M.access(a), i = o.extend({}, h), M.set(b, i))
+    function Le(e, t) {
+        var n, r, i, o, a, s;
+        if (1 === t.nodeType) {
+            if (Y.hasData(e) && (s = Y.get(e).events))
+                for (i in Y.remove(t, "handle events"), s)
+                    for (n = 0, r = s[i].length; n < r; n++) S.event.add(t, i, s[i][n]);
+            Q.hasData(e) && (o = Q.access(e), a = S.extend({}, o), Q.set(t, a))
         }
     }
 
-    function ob(a, b) {
-        var c = a.getElementsByTagName ? a.getElementsByTagName(b || "*") : a.querySelectorAll ? a.querySelectorAll(b || "*") : [];
-        return void 0 === b || b && o.nodeName(a, b) ? o.merge([a], c) : c
+    function He(n, r, i, o) {
+        r = g(r);
+        var e, t, a, s, u, l, c = 0,
+            f = n.length,
+            p = f - 1,
+            d = r[0],
+            h = m(d);
+        if (h || 1 < f && "string" == typeof d && !v.checkClone && Ae.test(d)) return n.each(function(e) {
+            var t = n.eq(e);
+            h && (r[0] = d.call(this, e, t.html())), He(t, r, i, o)
+        });
+        if (f && (t = (e = xe(r, n[0].ownerDocument, !1, n, o)).firstChild, 1 === e.childNodes.length && (e = t), t || o)) {
+            for (s = (a = S.map(ye(e, "script"), De)).length; c < f; c++) u = e, c !== p && (u = S.clone(u, !0, !0), s && S.merge(a, ye(u, "script"))), i.call(n[c], u, c);
+            if (s)
+                for (l = a[a.length - 1].ownerDocument, S.map(a, qe), c = 0; c < s; c++) u = a[c], he.test(u.type || "") && !Y.access(u, "globalEval") && S.contains(l, u) && (u.src && "module" !== (u.type || "").toLowerCase() ? S._evalUrl && !u.noModule && S._evalUrl(u.src, {
+                    nonce: u.nonce || u.getAttribute("nonce")
+                }, l) : b(u.textContent.replace(Ne, ""), u, l))
+        }
+        return n
     }
 
-    function pb(a, b) {
-        var c = b.nodeName.toLowerCase();
-        "input" === c && T.test(a.type) ? b.checked = a.checked : ("input" === c || "textarea" === c) && (b.defaultValue = a.defaultValue)
+    function Oe(e, t, n) {
+        for (var r, i = t ? S.filter(t, e) : e, o = 0; null != (r = i[o]); o++) n || 1 !== r.nodeType || S.cleanData(ye(r)), r.parentNode && (n && ie(r) && ve(ye(r, "script")), r.parentNode.removeChild(r));
+        return e
     }
-    o.extend({
-        clone: function(a, b, c) {
-            var d, e, f, g, h = a.cloneNode(!0),
-                i = o.contains(a.ownerDocument, a);
-            if (!(l.noCloneChecked || 1 !== a.nodeType && 11 !== a.nodeType || o.isXMLDoc(a)))
-                for (g = ob(h), f = ob(a), d = 0, e = f.length; e > d; d++) pb(f[d], g[d]);
-            if (b)
-                if (c)
-                    for (f = f || ob(a), g = g || ob(h), d = 0, e = f.length; e > d; d++) nb(f[d], g[d]);
-                else nb(a, h);
-            return g = ob(h, "script"), g.length > 0 && mb(g, !i && ob(a, "script")), h
-        },
-        buildFragment: function(a, b, c, d) {
-            for (var e, f, g, h, i, j, k = b.createDocumentFragment(), l = [], m = 0, n = a.length; n > m; m++)
-                if (e = a[m], e || 0 === e)
-                    if ("object" === o.type(e)) o.merge(l, e.nodeType ? [e] : e);
-                    else if (cb.test(e)) {
-                f = f || k.appendChild(b.createElement("div")), g = (bb.exec(e) || ["", ""])[1].toLowerCase(), h = ib[g] || ib._default, f.innerHTML = h[1] + e.replace(ab, "<$1></$2>") + h[2], j = h[0];
-                while (j--) f = f.lastChild;
-                o.merge(l, f.childNodes), f = k.firstChild, f.textContent = ""
-            } else l.push(b.createTextNode(e));
-            k.textContent = "", m = 0;
-            while (e = l[m++])
-                if ((!d || -1 === o.inArray(e, d)) && (i = o.contains(e.ownerDocument, e), f = ob(k.appendChild(e), "script"), i && mb(f), c)) {
-                    j = 0;
-                    while (e = f[j++]) fb.test(e.type || "") && c.push(e)
-                } return k
+    S.extend({
+        htmlPrefilter: function(e) {
+            return e
         },
-        cleanData: function(a) {
-            for (var b, c, d, e, f, g, h = o.event.special, i = 0; void 0 !== (c = a[i]); i++) {
-                if (o.acceptData(c) && (f = c[L.expando], f && (b = L.cache[f]))) {
-                    if (d = Object.keys(b.events || {}), d.length)
-                        for (g = 0; void 0 !== (e = d[g]); g++) h[e] ? o.event.remove(c, e) : o.removeEvent(c, e, b.handle);
-                    L.cache[f] && delete L.cache[f]
-                }
-                delete M.cache[c[M.expando]]
-            }
-        }
-    }), o.fn.extend({
-        text: function(a) {
-            return J(this, function(a) {
-                return void 0 === a ? o.text(this) : this.empty().each(function() {
-                    (1 === this.nodeType || 11 === this.nodeType || 9 === this.nodeType) && (this.textContent = a)
+        clone: function(e, t, n) {
+            var r, i, o, a, s, u, l, c = e.cloneNode(!0),
+                f = ie(e);
+            if (!(v.noCloneChecked || 1 !== e.nodeType && 11 !== e.nodeType || S.isXMLDoc(e)))
+                for (a = ye(c), r = 0, i = (o = ye(e)).length; r < i; r++) s = o[r], u = a[r], void 0, "input" === (l = u.nodeName.toLowerCase()) && pe.test(s.type) ? u.checked = s.checked : "input" !== l && "textarea" !== l || (u.defaultValue = s.defaultValue);
+            if (t)
+                if (n)
+                    for (o = o || ye(e), a = a || ye(c), r = 0, i = o.length; r < i; r++) Le(o[r], a[r]);
+                else Le(e, c);
+            return 0 < (a = ye(c, "script")).length && ve(a, !f && ye(e, "script")), c
+        },
+        cleanData: function(e) {
+            for (var t, n, r, i = S.event.special, o = 0; void 0 !== (n = e[o]); o++)
+                if (V(n)) {
+                    if (t = n[Y.expando]) {
+                        if (t.events)
+                            for (r in t.events) i[r] ? S.event.remove(n, r) : S.removeEvent(n, r, t.handle);
+                        n[Y.expando] = void 0
+                    }
+                    n[Q.expando] && (n[Q.expando] = void 0)
+                }
+        }
+    }), S.fn.extend({
+        detach: function(e) {
+            return Oe(this, e, !0)
+        },
+        remove: function(e) {
+            return Oe(this, e)
+        },
+        text: function(e) {
+            return B(this, function(e) {
+                return void 0 === e ? S.text(this) : this.empty().each(function() {
+                    1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || (this.textContent = e)
                 })
-            }, null, a, arguments.length)
+            }, null, e, arguments.length)
         },
         append: function() {
-            return this.domManip(arguments, function(a) {
-                if (1 === this.nodeType || 11 === this.nodeType || 9 === this.nodeType) {
-                    var b = jb(this, a);
-                    b.appendChild(a)
-                }
+            return He(this, arguments, function(e) {
+                1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || je(this, e).appendChild(e)
             })
         },
         prepend: function() {
-            return this.domManip(arguments, function(a) {
+            return He(this, arguments, function(e) {
                 if (1 === this.nodeType || 11 === this.nodeType || 9 === this.nodeType) {
-                    var b = jb(this, a);
-                    b.insertBefore(a, b.firstChild)
+                    var t = je(this, e);
+                    t.insertBefore(e, t.firstChild)
                 }
             })
         },
         before: function() {
-            return this.domManip(arguments, function(a) {
-                this.parentNode && this.parentNode.insertBefore(a, this)
+            return He(this, arguments, function(e) {
+                this.parentNode && this.parentNode.insertBefore(e, this)
             })
         },
         after: function() {
-            return this.domManip(arguments, function(a) {
-                this.parentNode && this.parentNode.insertBefore(a, this.nextSibling)
+            return He(this, arguments, function(e) {
+                this.parentNode && this.parentNode.insertBefore(e, this.nextSibling)
             })
         },
-        remove: function(a, b) {
-            for (var c, d = a ? o.filter(a, this) : this, e = 0; null != (c = d[e]); e++) b || 1 !== c.nodeType || o.cleanData(ob(c)), c.parentNode && (b && o.contains(c.ownerDocument, c) && mb(ob(c, "script")), c.parentNode.removeChild(c));
-            return this
-        },
         empty: function() {
-            for (var a, b = 0; null != (a = this[b]); b++) 1 === a.nodeType && (o.cleanData(ob(a, !1)), a.textContent = "");
+            for (var e, t = 0; null != (e = this[t]); t++) 1 === e.nodeType && (S.cleanData(ye(e, !1)), e.textContent = "");
             return this
         },
-        clone: function(a, b) {
-            return a = null == a ? !1 : a, b = null == b ? a : b, this.map(function() {
-                return o.clone(this, a, b)
+        clone: function(e, t) {
+            return e = null != e && e, t = null == t ? e : t, this.map(function() {
+                return S.clone(this, e, t)
             })
         },
-        html: function(a) {
-            return J(this, function(a) {
-                var b = this[0] || {},
-                    c = 0,
-                    d = this.length;
-                if (void 0 === a && 1 === b.nodeType) return b.innerHTML;
-                if ("string" == typeof a && !db.test(a) && !ib[(bb.exec(a) || ["", ""])[1].toLowerCase()]) {
-                    a = a.replace(ab, "<$1></$2>");
+        html: function(e) {
+            return B(this, function(e) {
+                var t = this[0] || {},
+                    n = 0,
+                    r = this.length;
+                if (void 0 === e && 1 === t.nodeType) return t.innerHTML;
+                if ("string" == typeof e && !ke.test(e) && !ge[(de.exec(e) || ["", ""])[1].toLowerCase()]) {
+                    e = S.htmlPrefilter(e);
                     try {
-                        for (; d > c; c++) b = this[c] || {}, 1 === b.nodeType && (o.cleanData(ob(b, !1)), b.innerHTML = a);
-                        b = 0
+                        for (; n < r; n++) 1 === (t = this[n] || {}).nodeType && (S.cleanData(ye(t, !1)), t.innerHTML = e);
+                        t = 0
                     } catch (e) {}
                 }
-                b && this.empty().append(a)
-            }, null, a, arguments.length)
+                t && this.empty().append(e)
+            }, null, e, arguments.length)
         },
         replaceWith: function() {
-            var a = arguments[0];
-            return this.domManip(arguments, function(b) {
-                a = this.parentNode, o.cleanData(ob(this)), a && a.replaceChild(b, this)
-            }), a && (a.length || a.nodeType) ? this : this.remove()
-        },
-        detach: function(a) {
-            return this.remove(a, !0)
-        },
-        domManip: function(a, b) {
-            a = e.apply([], a);
-            var c, d, f, g, h, i, j = 0,
-                k = this.length,
-                m = this,
-                n = k - 1,
-                p = a[0],
-                q = o.isFunction(p);
-            if (q || k > 1 && "string" == typeof p && !l.checkClone && eb.test(p)) return this.each(function(c) {
-                var d = m.eq(c);
-                q && (a[0] = p.call(this, c, d.html())), d.domManip(a, b)
-            });
-            if (k && (c = o.buildFragment(a, this[0].ownerDocument, !1, this), d = c.firstChild, 1 === c.childNodes.length && (c = d), d)) {
-                for (f = o.map(ob(c, "script"), kb), g = f.length; k > j; j++) h = c, j !== n && (h = o.clone(h, !0, !0), g && o.merge(f, ob(h, "script"))), b.call(this[j], h, j);
-                if (g)
-                    for (i = f[f.length - 1].ownerDocument, o.map(f, lb), j = 0; g > j; j++) h = f[j], fb.test(h.type || "") && !L.access(h, "globalEval") && o.contains(i, h) && (h.src ? o._evalUrl && o._evalUrl(h.src) : o.globalEval(h.textContent.replace(hb, "")))
-            }
-            return this
+            var n = [];
+            return He(this, arguments, function(e) {
+                var t = this.parentNode;
+                S.inArray(this, n) < 0 && (S.cleanData(ye(this)), t && t.replaceChild(e, this))
+            }, n)
         }
-    }), o.each({
+    }), S.each({
         appendTo: "append",
         prependTo: "prepend",
         insertBefore: "before",
         insertAfter: "after",
         replaceAll: "replaceWith"
-    }, function(a, b) {
-        o.fn[a] = function(a) {
-            for (var c, d = [], e = o(a), g = e.length - 1, h = 0; g >= h; h++) c = h === g ? this : this.clone(!0), o(e[h])[b](c), f.apply(d, c.get());
-            return this.pushStack(d)
+    }, function(e, a) {
+        S.fn[e] = function(e) {
+            for (var t, n = [], r = S(e), i = r.length - 1, o = 0; o <= i; o++) t = o === i ? this : this.clone(!0), S(r[o])[a](t), u.apply(n, t.get());
+            return this.pushStack(n)
         }
     });
-    var qb, rb = {};
-
-    function sb(b, c) {
-        var d = o(c.createElement(b)).appendTo(c.body),
-            e = a.getDefaultComputedStyle ? a.getDefaultComputedStyle(d[0]).display : o.css(d[0], "display");
-        return d.detach(), e
-    }
-
-    function tb(a) {
-        var b = m,
-            c = rb[a];
-        return c || (c = sb(a, b), "none" !== c && c || (qb = (qb || o("<iframe frameborder='0' width='0' height='0'/>")).appendTo(b.documentElement), b = qb[0].contentDocument, b.write(), b.close(), c = sb(a, b), qb.detach()), rb[a] = c), c
-    }
-    var ub = /^margin/,
-        vb = new RegExp("^(" + Q + ")(?!px)[a-z%]+$", "i"),
-        wb = function(a) {
-            return a.ownerDocument.defaultView.getComputedStyle(a, null)
-        };
-
-    function xb(a, b, c) {
-        var d, e, f, g, h = a.style;
-        return c = c || wb(a), c && (g = c.getPropertyValue(b) || c[b]), c && ("" !== g || o.contains(a.ownerDocument, a) || (g = o.style(a, b)), vb.test(g) && ub.test(b) && (d = h.width, e = h.minWidth, f = h.maxWidth, h.minWidth = h.maxWidth = h.width = g, g = c.width, h.width = d, h.minWidth = e, h.maxWidth = f)), void 0 !== g ? g + "" : g
+    var Pe = new RegExp("^(" + ee + ")(?!px)[a-z%]+$", "i"),
+        Re = /^--/,
+        Me = function(e) {
+            var t = e.ownerDocument.defaultView;
+            return t && t.opener || (t = C), t.getComputedStyle(e)
+        },
+        Ie = function(e, t, n) {
+            var r, i, o = {};
+            for (i in t) o[i] = e.style[i], e.style[i] = t[i];
+            for (i in r = n.call(e), t) e.style[i] = o[i];
+            return r
+        },
+        We = new RegExp(ne.join("|"), "i"),
+        Fe = "[\\x20\\t\\r\\n\\f]",
+        $e = new RegExp("^" + Fe + "+|((?:^|[^\\\\])(?:\\\\.)*)" + Fe + "+$", "g");
+
+    function Be(e, t, n) {
+        var r, i, o, a, s = Re.test(t),
+            u = e.style;
+        return (n = n || Me(e)) && (a = n.getPropertyValue(t) || n[t], s && a && (a = a.replace($e, "$1") || void 0), "" !== a || ie(e) || (a = S.style(e, t)), !v.pixelBoxStyles() && Pe.test(a) && We.test(t) && (r = u.width, i = u.minWidth, o = u.maxWidth, u.minWidth = u.maxWidth = u.width = a, a = n.width, u.width = r, u.minWidth = i, u.maxWidth = o)), void 0 !== a ? a + "" : a
     }
 
-    function yb(a, b) {
+    function _e(e, t) {
         return {
             get: function() {
-                return a() ? void delete this.get : (this.get = b).apply(this, arguments)
+                if (!e()) return (this.get = t).apply(this, arguments);
+                delete this.get
             }
         }
     }! function() {
-        var b, c, d = "padding:0;margin:0;border:0;display:block;-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box",
-            e = m.documentElement,
-            f = m.createElement("div"),
-            g = m.createElement("div");
-        g.style.backgroundClip = "content-box", g.cloneNode(!0).style.backgroundClip = "", l.clearCloneStyle = "content-box" === g.style.backgroundClip, f.style.cssText = "border:0;width:0;height:0;position:absolute;top:0;left:-9999px;margin-top:1px", f.appendChild(g);
-
-        function h() {
-            g.style.cssText = "-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box;padding:1px;border:1px;display:block;width:4px;margin-top:1%;position:absolute;top:1%", e.appendChild(f);
-            var d = a.getComputedStyle(g, null);
-            b = "1%" !== d.top, c = "4px" === d.width, e.removeChild(f)
+        function e() {
+            if (l) {
+                u.style.cssText = "position:absolute;left:-11111px;width:60px;margin-top:1px;padding:0;border:0", l.style.cssText = "position:relative;display:block;box-sizing:border-box;overflow:scroll;margin:auto;border:1px;padding:1px;width:60%;top:1%", re.appendChild(u).appendChild(l);
+                var e = C.getComputedStyle(l);
+                n = "1%" !== e.top, s = 12 === t(e.marginLeft), l.style.right = "60%", o = 36 === t(e.right), r = 36 === t(e.width), l.style.position = "absolute", i = 12 === t(l.offsetWidth / 3), re.removeChild(u), l = null
+            }
+        }
+
+        function t(e) {
+            return Math.round(parseFloat(e))
         }
-        a.getComputedStyle && o.extend(l, {
+        var n, r, i, o, a, s, u = E.createElement("div"),
+            l = E.createElement("div");
+        l.style && (l.style.backgroundClip = "content-box", l.cloneNode(!0).style.backgroundClip = "", v.clearCloneStyle = "content-box" === l.style.backgroundClip, S.extend(v, {
+            boxSizingReliable: function() {
+                return e(), r
+            },
+            pixelBoxStyles: function() {
+                return e(), o
+            },
             pixelPosition: function() {
-                return h(), b
+                return e(), n
             },
-            boxSizingReliable: function() {
-                return null == c && h(), c
+            reliableMarginLeft: function() {
+                return e(), s
             },
-            reliableMarginRight: function() {
-                var b, c = g.appendChild(m.createElement("div"));
-                return c.style.cssText = g.style.cssText = d, c.style.marginRight = c.style.width = "0", g.style.width = "1px", e.appendChild(f), b = !parseFloat(a.getComputedStyle(c, null).marginRight), e.removeChild(f), g.innerHTML = "", b
+            scrollboxSize: function() {
+                return e(), i
+            },
+            reliableTrDimensions: function() {
+                var e, t, n, r;
+                return null == a && (e = E.createElement("table"), t = E.createElement("tr"), n = E.createElement("div"), e.style.cssText = "position:absolute;left:-11111px;border-collapse:separate", t.style.cssText = "border:1px solid", t.style.height = "1px", n.style.height = "9px", n.style.display = "block", re.appendChild(e).appendChild(t).appendChild(n), r = C.getComputedStyle(t), a = parseInt(r.height, 10) + parseInt(r.borderTopWidth, 10) + parseInt(r.borderBottomWidth, 10) === t.offsetHeight, re.removeChild(e)), a
             }
-        })
-    }(), o.swap = function(a, b, c, d) {
-        var e, f, g = {};
-        for (f in b) g[f] = a.style[f], a.style[f] = b[f];
-        e = c.apply(a, d || []);
-        for (f in b) a.style[f] = g[f];
-        return e
-    };
-    var zb = /^(none|table(?!-c[ea]).+)/,
-        Ab = new RegExp("^(" + Q + ")(.*)$", "i"),
-        Bb = new RegExp("^([+-])=(" + Q + ")", "i"),
-        Cb = {
+        }))
+    }();
+    var ze = ["Webkit", "Moz", "ms"],
+        Ue = E.createElement("div").style,
+        Xe = {};
+
+    function Ve(e) {
+        var t = S.cssProps[e] || Xe[e];
+        return t || (e in Ue ? e : Xe[e] = function(e) {
+            var t = e[0].toUpperCase() + e.slice(1),
+                n = ze.length;
+            while (n--)
+                if ((e = ze[n] + t) in Ue) return e
+        }(e) || e)
+    }
+    var Ge = /^(none|table(?!-c[ea]).+)/,
+        Ye = {
             position: "absolute",
             visibility: "hidden",
             display: "block"
         },
-        Db = {
-            letterSpacing: 0,
-            fontWeight: 400
-        },
-        Eb = ["Webkit", "O", "Moz", "ms"];
-
-    function Fb(a, b) {
-        if (b in a) return b;
-        var c = b[0].toUpperCase() + b.slice(1),
-            d = b,
-            e = Eb.length;
-        while (e--)
-            if (b = Eb[e] + c, b in a) return b;
-        return d
-    }
+        Qe = {
+            letterSpacing: "0",
+            fontWeight: "400"
+        };
 
-    function Gb(a, b, c) {
-        var d = Ab.exec(b);
-        return d ? Math.max(0, d[1] - (c || 0)) + (d[2] || "px") : b
+    function Je(e, t, n) {
+        var r = te.exec(t);
+        return r ? Math.max(0, r[2] - (n || 0)) + (r[3] || "px") : t
     }
 
-    function Hb(a, b, c, d, e) {
-        for (var f = c === (d ? "border" : "content") ? 4 : "width" === b ? 1 : 0, g = 0; 4 > f; f += 2) "margin" === c && (g += o.css(a, c + R[f], !0, e)), d ? ("content" === c && (g -= o.css(a, "padding" + R[f], !0, e)), "margin" !== c && (g -= o.css(a, "border" + R[f] + "Width", !0, e))) : (g += o.css(a, "padding" + R[f], !0, e), "padding" !== c && (g += o.css(a, "border" + R[f] + "Width", !0, e)));
-        return g
+    function Ke(e, t, n, r, i, o) {
+        var a = "width" === t ? 1 : 0,
+            s = 0,
+            u = 0;
+        if (n === (r ? "border" : "content")) return 0;
+        for (; a < 4; a += 2) "margin" === n && (u += S.css(e, n + ne[a], !0, i)), r ? ("content" === n && (u -= S.css(e, "padding" + ne[a], !0, i)), "margin" !== n && (u -= S.css(e, "border" + ne[a] + "Width", !0, i))) : (u += S.css(e, "padding" + ne[a], !0, i), "padding" !== n ? u += S.css(e, "border" + ne[a] + "Width", !0, i) : s += S.css(e, "border" + ne[a] + "Width", !0, i));
+        return !r && 0 <= o && (u += Math.max(0, Math.ceil(e["offset" + t[0].toUpperCase() + t.slice(1)] - o - u - s - .5)) || 0), u
     }
 
-    function Ib(a, b, c) {
-        var d = !0,
-            e = "width" === b ? a.offsetWidth : a.offsetHeight,
-            f = wb(a),
-            g = "border-box" === o.css(a, "boxSizing", !1, f);
-        if (0 >= e || null == e) {
-            if (e = xb(a, b, f), (0 > e || null == e) && (e = a.style[b]), vb.test(e)) return e;
-            d = g && (l.boxSizingReliable() || e === a.style[b]), e = parseFloat(e) || 0
+    function Ze(e, t, n) {
+        var r = Me(e),
+            i = (!v.boxSizingReliable() || n) && "border-box" === S.css(e, "boxSizing", !1, r),
+            o = i,
+            a = Be(e, t, r),
+            s = "offset" + t[0].toUpperCase() + t.slice(1);
+        if (Pe.test(a)) {
+            if (!n) return a;
+            a = "auto"
         }
-        return e + Hb(a, b, c || (g ? "border" : "content"), d, f) + "px"
+        return (!v.boxSizingReliable() && i || !v.reliableTrDimensions() && A(e, "tr") || "auto" === a || !parseFloat(a) && "inline" === S.css(e, "display", !1, r)) && e.getClientRects().length && (i = "border-box" === S.css(e, "boxSizing", !1, r), (o = s in e) && (a = e[s])), (a = parseFloat(a) || 0) + Ke(e, t, n || (i ? "border" : "content"), o, r, a) + "px"
     }
 
-    function Jb(a, b) {
-        for (var c, d, e, f = [], g = 0, h = a.length; h > g; g++) d = a[g], d.style && (f[g] = L.get(d, "olddisplay"), c = d.style.display, b ? (f[g] || "none" !== c || (d.style.display = ""), "" === d.style.display && S(d) && (f[g] = L.access(d, "olddisplay", tb(d.nodeName)))) : f[g] || (e = S(d), (c && "none" !== c || !e) && L.set(d, "olddisplay", e ? c : o.css(d, "display"))));
-        for (g = 0; h > g; g++) d = a[g], d.style && (b && "none" !== d.style.display && "" !== d.style.display || (d.style.display = b ? f[g] || "" : "none"));
-        return a
+    function et(e, t, n, r, i) {
+        return new et.prototype.init(e, t, n, r, i)
     }
-    o.extend({
+    S.extend({
         cssHooks: {
             opacity: {
-                get: function(a, b) {
-                    if (b) {
-                        var c = xb(a, "opacity");
-                        return "" === c ? "1" : c
+                get: function(e, t) {
+                    if (t) {
+                        var n = Be(e, "opacity");
+                        return "" === n ? "1" : n
                     }
                 }
             }
         },
         cssNumber: {
+            animationIterationCount: !0,
             columnCount: !0,
             fillOpacity: !0,
+            flexGrow: !0,
+            flexShrink: !0,
             fontWeight: !0,
+            gridArea: !0,
+            gridColumn: !0,
+            gridColumnEnd: !0,
+            gridColumnStart: !0,
+            gridRow: !0,
+            gridRowEnd: !0,
+            gridRowStart: !0,
             lineHeight: !0,
             opacity: !0,
             order: !0,
             orphans: !0,
             widows: !0,
             zIndex: !0,
             zoom: !0
         },
-        cssProps: {
-            "float": "cssFloat"
-        },
-        style: function(a, b, c, d) {
-            if (a && 3 !== a.nodeType && 8 !== a.nodeType && a.style) {
-                var e, f, g, h = o.camelCase(b),
-                    i = a.style;
-                return b = o.cssProps[h] || (o.cssProps[h] = Fb(i, h)), g = o.cssHooks[b] || o.cssHooks[h], void 0 === c ? g && "get" in g && void 0 !== (e = g.get(a, !1, d)) ? e : i[b] : (f = typeof c, "string" === f && (e = Bb.exec(c)) && (c = (e[1] + 1) * e[2] + parseFloat(o.css(a, b)), f = "number"), null != c && c === c && ("number" !== f || o.cssNumber[h] || (c += "px"), l.clearCloneStyle || "" !== c || 0 !== b.indexOf("background") || (i[b] = "inherit"), g && "set" in g && void 0 === (c = g.set(a, c, d)) || (i[b] = "", i[b] = c)), void 0)
-            }
-        },
-        css: function(a, b, c, d) {
-            var e, f, g, h = o.camelCase(b);
-            return b = o.cssProps[h] || (o.cssProps[h] = Fb(a.style, h)), g = o.cssHooks[b] || o.cssHooks[h], g && "get" in g && (e = g.get(a, !0, c)), void 0 === e && (e = xb(a, b, d)), "normal" === e && b in Db && (e = Db[b]), "" === c || c ? (f = parseFloat(e), c === !0 || o.isNumeric(f) ? f || 0 : e) : e
-        }
-    }), o.each(["height", "width"], function(a, b) {
-        o.cssHooks[b] = {
-            get: function(a, c, d) {
-                return c ? 0 === a.offsetWidth && zb.test(o.css(a, "display")) ? o.swap(a, Cb, function() {
-                    return Ib(a, b, d)
-                }) : Ib(a, b, d) : void 0
-            },
-            set: function(a, c, d) {
-                var e = d && wb(a);
-                return Gb(a, c, d ? Hb(a, b, d, "border-box" === o.css(a, "boxSizing", !1, e), e) : 0)
-            }
-        }
-    }), o.cssHooks.marginRight = yb(l.reliableMarginRight, function(a, b) {
-        return b ? o.swap(a, {
-            display: "inline-block"
-        }, xb, [a, "marginRight"]) : void 0
-    }), o.each({
+        cssProps: {},
+        style: function(e, t, n, r) {
+            if (e && 3 !== e.nodeType && 8 !== e.nodeType && e.style) {
+                var i, o, a, s = X(t),
+                    u = Re.test(t),
+                    l = e.style;
+                if (u || (t = Ve(s)), a = S.cssHooks[t] || S.cssHooks[s], void 0 === n) return a && "get" in a && void 0 !== (i = a.get(e, !1, r)) ? i : l[t];
+                "string" === (o = typeof n) && (i = te.exec(n)) && i[1] && (n = se(e, t, i), o = "number"), null != n && n == n && ("number" !== o || u || (n += i && i[3] || (S.cssNumber[s] ? "" : "px")), v.clearCloneStyle || "" !== n || 0 !== t.indexOf("background") || (l[t] = "inherit"), a && "set" in a && void 0 === (n = a.set(e, n, r)) || (u ? l.setProperty(t, n) : l[t] = n))
+            }
+        },
+        css: function(e, t, n, r) {
+            var i, o, a, s = X(t);
+            return Re.test(t) || (t = Ve(s)), (a = S.cssHooks[t] || S.cssHooks[s]) && "get" in a && (i = a.get(e, !0, n)), void 0 === i && (i = Be(e, t, r)), "normal" === i && t in Qe && (i = Qe[t]), "" === n || n ? (o = parseFloat(i), !0 === n || isFinite(o) ? o || 0 : i) : i
+        }
+    }), S.each(["height", "width"], function(e, u) {
+        S.cssHooks[u] = {
+            get: function(e, t, n) {
+                if (t) return !Ge.test(S.css(e, "display")) || e.getClientRects().length && e.getBoundingClientRect().width ? Ze(e, u, n) : Ie(e, Ye, function() {
+                    return Ze(e, u, n)
+                })
+            },
+            set: function(e, t, n) {
+                var r, i = Me(e),
+                    o = !v.scrollboxSize() && "absolute" === i.position,
+                    a = (o || n) && "border-box" === S.css(e, "boxSizing", !1, i),
+                    s = n ? Ke(e, u, n, a, i) : 0;
+                return a && o && (s -= Math.ceil(e["offset" + u[0].toUpperCase() + u.slice(1)] - parseFloat(i[u]) - Ke(e, u, "border", !1, i) - .5)), s && (r = te.exec(t)) && "px" !== (r[3] || "px") && (e.style[u] = t, t = S.css(e, u)), Je(0, t, s)
+            }
+        }
+    }), S.cssHooks.marginLeft = _e(v.reliableMarginLeft, function(e, t) {
+        if (t) return (parseFloat(Be(e, "marginLeft")) || e.getBoundingClientRect().left - Ie(e, {
+            marginLeft: 0
+        }, function() {
+            return e.getBoundingClientRect().left
+        })) + "px"
+    }), S.each({
         margin: "",
         padding: "",
         border: "Width"
-    }, function(a, b) {
-        o.cssHooks[a + b] = {
-            expand: function(c) {
-                for (var d = 0, e = {}, f = "string" == typeof c ? c.split(" ") : [c]; 4 > d; d++) e[a + R[d] + b] = f[d] || f[d - 2] || f[0];
-                return e
-            }
-        }, ub.test(a) || (o.cssHooks[a + b].set = Gb)
-    }), o.fn.extend({
-        css: function(a, b) {
-            return J(this, function(a, b, c) {
-                var d, e, f = {},
-                    g = 0;
-                if (o.isArray(b)) {
-                    for (d = wb(a), e = b.length; e > g; g++) f[b[g]] = o.css(a, b[g], !1, d);
-                    return f
-                }
-                return void 0 !== c ? o.style(a, b, c) : o.css(a, b)
-            }, a, b, arguments.length > 1)
-        },
-        show: function() {
-            return Jb(this, !0)
-        },
-        hide: function() {
-            return Jb(this)
-        },
-        toggle: function(a) {
-            return "boolean" == typeof a ? a ? this.show() : this.hide() : this.each(function() {
-                S(this) ? o(this).show() : o(this).hide()
-            })
-        }
-    });
-
-    function Kb(a, b, c, d, e) {
-        return new Kb.prototype.init(a, b, c, d, e)
-    }
-    o.Tween = Kb, Kb.prototype = {
-        constructor: Kb,
-        init: function(a, b, c, d, e, f) {
-            this.elem = a, this.prop = c, this.easing = e || "swing", this.options = b, this.start = this.now = this.cur(), this.end = d, this.unit = f || (o.cssNumber[c] ? "" : "px")
+    }, function(i, o) {
+        S.cssHooks[i + o] = {
+            expand: function(e) {
+                for (var t = 0, n = {}, r = "string" == typeof e ? e.split(" ") : [e]; t < 4; t++) n[i + ne[t] + o] = r[t] || r[t - 2] || r[0];
+                return n
+            }
+        }, "margin" !== i && (S.cssHooks[i + o].set = Je)
+    }), S.fn.extend({
+        css: function(e, t) {
+            return B(this, function(e, t, n) {
+                var r, i, o = {},
+                    a = 0;
+                if (Array.isArray(t)) {
+                    for (r = Me(e), i = t.length; a < i; a++) o[t[a]] = S.css(e, t[a], !1, r);
+                    return o
+                }
+                return void 0 !== n ? S.style(e, t, n) : S.css(e, t)
+            }, e, t, 1 < arguments.length)
+        }
+    }), ((S.Tween = et).prototype = {
+        constructor: et,
+        init: function(e, t, n, r, i, o) {
+            this.elem = e, this.prop = n, this.easing = i || S.easing._default, this.options = t, this.start = this.now = this.cur(), this.end = r, this.unit = o || (S.cssNumber[n] ? "" : "px")
         },
         cur: function() {
-            var a = Kb.propHooks[this.prop];
-            return a && a.get ? a.get(this) : Kb.propHooks._default.get(this)
+            var e = et.propHooks[this.prop];
+            return e && e.get ? e.get(this) : et.propHooks._default.get(this)
         },
-        run: function(a) {
-            var b, c = Kb.propHooks[this.prop];
-            return this.pos = b = this.options.duration ? o.easing[this.easing](a, this.options.duration * a, 0, 1, this.options.duration) : a, this.now = (this.end - this.start) * b + this.start, this.options.step && this.options.step.call(this.elem, this.now, this), c && c.set ? c.set(this) : Kb.propHooks._default.set(this), this
+        run: function(e) {
+            var t, n = et.propHooks[this.prop];
+            return this.options.duration ? this.pos = t = S.easing[this.easing](e, this.options.duration * e, 0, 1, this.options.duration) : this.pos = t = e, this.now = (this.end - this.start) * t + this.start, this.options.step && this.options.step.call(this.elem, this.now, this), n && n.set ? n.set(this) : et.propHooks._default.set(this), this
         }
-    }, Kb.prototype.init.prototype = Kb.prototype, Kb.propHooks = {
+    }).init.prototype = et.prototype, (et.propHooks = {
         _default: {
-            get: function(a) {
-                var b;
-                return null == a.elem[a.prop] || a.elem.style && null != a.elem.style[a.prop] ? (b = o.css(a.elem, a.prop, ""), b && "auto" !== b ? b : 0) : a.elem[a.prop]
+            get: function(e) {
+                var t;
+                return 1 !== e.elem.nodeType || null != e.elem[e.prop] && null == e.elem.style[e.prop] ? e.elem[e.prop] : (t = S.css(e.elem, e.prop, "")) && "auto" !== t ? t : 0
             },
-            set: function(a) {
-                o.fx.step[a.prop] ? o.fx.step[a.prop](a) : a.elem.style && (null != a.elem.style[o.cssProps[a.prop]] || o.cssHooks[a.prop]) ? o.style(a.elem, a.prop, a.now + a.unit) : a.elem[a.prop] = a.now
+            set: function(e) {
+                S.fx.step[e.prop] ? S.fx.step[e.prop](e) : 1 !== e.elem.nodeType || !S.cssHooks[e.prop] && null == e.elem.style[Ve(e.prop)] ? e.elem[e.prop] = e.now : S.style(e.elem, e.prop, e.now + e.unit)
             }
         }
-    }, Kb.propHooks.scrollTop = Kb.propHooks.scrollLeft = {
-        set: function(a) {
-            a.elem.nodeType && a.elem.parentNode && (a.elem[a.prop] = a.now)
+    }).scrollTop = et.propHooks.scrollLeft = {
+        set: function(e) {
+            e.elem.nodeType && e.elem.parentNode && (e.elem[e.prop] = e.now)
         }
-    }, o.easing = {
-        linear: function(a) {
-            return a
+    }, S.easing = {
+        linear: function(e) {
+            return e
         },
-        swing: function(a) {
-            return .5 - Math.cos(a * Math.PI) / 2
-        }
-    }, o.fx = Kb.prototype.init, o.fx.step = {};
-    var Lb, Mb, Nb = /^(?:toggle|show|hide)$/,
-        Ob = new RegExp("^(?:([+-])=|)(" + Q + ")([a-z%]*)$", "i"),
-        Pb = /queueHooks$/,
-        Qb = [Vb],
-        Rb = {
-            "*": [function(a, b) {
-                var c = this.createTween(a, b),
-                    d = c.cur(),
-                    e = Ob.exec(b),
-                    f = e && e[3] || (o.cssNumber[a] ? "" : "px"),
-                    g = (o.cssNumber[a] || "px" !== f && +d) && Ob.exec(o.css(c.elem, a)),
-                    h = 1,
-                    i = 20;
-                if (g && g[3] !== f) {
-                    f = f || g[3], e = e || [], g = +d || 1;
-                    do h = h || ".5", g /= h, o.style(c.elem, a, g + f); while (h !== (h = c.cur() / d) && 1 !== h && --i)
-                }
-                return e && (g = c.start = +g || +d || 0, c.unit = f, c.end = e[1] ? g + (e[1] + 1) * e[2] : +e[2]), c
-            }]
-        };
+        swing: function(e) {
+            return .5 - Math.cos(e * Math.PI) / 2
+        },
+        _default: "swing"
+    }, S.fx = et.prototype.init, S.fx.step = {};
+    var tt, nt, rt, it, ot = /^(?:toggle|show|hide)$/,
+        at = /queueHooks$/;
 
-    function Sb() {
-        return setTimeout(function() {
-            Lb = void 0
-        }), Lb = o.now()
+    function st() {
+        nt && (!1 === E.hidden && C.requestAnimationFrame ? C.requestAnimationFrame(st) : C.setTimeout(st, S.fx.interval), S.fx.tick())
     }
 
-    function Tb(a, b) {
-        var c, d = 0,
-            e = {
-                height: a
-            };
-        for (b = b ? 1 : 0; 4 > d; d += 2 - b) c = R[d], e["margin" + c] = e["padding" + c] = a;
-        return b && (e.opacity = e.width = a), e
+    function ut() {
+        return C.setTimeout(function() {
+            tt = void 0
+        }), tt = Date.now()
     }
 
-    function Ub(a, b, c) {
-        for (var d, e = (Rb[b] || []).concat(Rb["*"]), f = 0, g = e.length; g > f; f++)
-            if (d = e[f].call(c, b, a)) return d
-    }
-
-    function Vb(a, b, c) {
-        var d, e, f, g, h, i, j, k = this,
-            l = {},
-            m = a.style,
-            n = a.nodeType && S(a),
-            p = L.get(a, "fxshow");
-        c.queue || (h = o._queueHooks(a, "fx"), null == h.unqueued && (h.unqueued = 0, i = h.empty.fire, h.empty.fire = function() {
-            h.unqueued || i()
-        }), h.unqueued++, k.always(function() {
-            k.always(function() {
-                h.unqueued--, o.queue(a, "fx").length || h.empty.fire()
-            })
-        })), 1 === a.nodeType && ("height" in b || "width" in b) && (c.overflow = [m.overflow, m.overflowX, m.overflowY], j = o.css(a, "display"), "none" === j && (j = tb(a.nodeName)), "inline" === j && "none" === o.css(a, "float") && (m.display = "inline-block")), c.overflow && (m.overflow = "hidden", k.always(function() {
-            m.overflow = c.overflow[0], m.overflowX = c.overflow[1], m.overflowY = c.overflow[2]
-        }));
-        for (d in b)
-            if (e = b[d], Nb.exec(e)) {
-                if (delete b[d], f = f || "toggle" === e, e === (n ? "hide" : "show")) {
-                    if ("show" !== e || !p || void 0 === p[d]) continue;
-                    n = !0
-                }
-                l[d] = p && p[d] || o.style(a, d)
-            } if (!o.isEmptyObject(l)) {
-            p ? "hidden" in p && (n = p.hidden) : p = L.access(a, "fxshow", {}), f && (p.hidden = !n), n ? o(a).show() : k.done(function() {
-                o(a).hide()
-            }), k.done(function() {
-                var b;
-                L.remove(a, "fxshow");
-                for (b in l) o.style(a, b, l[b])
-            });
-            for (d in l) g = Ub(n ? p[d] : 0, d, k), d in p || (p[d] = g.start, n && (g.end = g.start, g.start = "width" === d || "height" === d ? 1 : 0))
-        }
+    function lt(e, t) {
+        var n, r = 0,
+            i = {
+                height: e
+            };
+        for (t = t ? 1 : 0; r < 4; r += 2 - t) i["margin" + (n = ne[r])] = i["padding" + n] = e;
+        return t && (i.opacity = i.width = e), i
     }
 
-    function Wb(a, b) {
-        var c, d, e, f, g;
-        for (c in a)
-            if (d = o.camelCase(c), e = b[d], f = a[c], o.isArray(f) && (e = f[1], f = a[c] = f[0]), c !== d && (a[d] = f, delete a[c]), g = o.cssHooks[d], g && "expand" in g) {
-                f = g.expand(f), delete a[d];
-                for (c in f) c in a || (a[c] = f[c], b[c] = e)
-            } else b[d] = e
+    function ct(e, t, n) {
+        for (var r, i = (ft.tweeners[t] || []).concat(ft.tweeners["*"]), o = 0, a = i.length; o < a; o++)
+            if (r = i[o].call(n, t, e)) return r
     }
 
-    function Xb(a, b, c) {
-        var d, e, f = 0,
-            g = Qb.length,
-            h = o.Deferred().always(function() {
-                delete i.elem
+    function ft(o, e, t) {
+        var n, a, r = 0,
+            i = ft.prefilters.length,
+            s = S.Deferred().always(function() {
+                delete u.elem
             }),
-            i = function() {
-                if (e) return !1;
-                for (var b = Lb || Sb(), c = Math.max(0, j.startTime + j.duration - b), d = c / j.duration || 0, f = 1 - d, g = 0, i = j.tweens.length; i > g; g++) j.tweens[g].run(f);
-                return h.notifyWith(a, [j, f, c]), 1 > f && i ? c : (h.resolveWith(a, [j]), !1)
-            },
-            j = h.promise({
-                elem: a,
-                props: o.extend({}, b),
-                opts: o.extend(!0, {
-                    specialEasing: {}
-                }, c),
-                originalProperties: b,
-                originalOptions: c,
-                startTime: Lb || Sb(),
-                duration: c.duration,
+            u = function() {
+                if (a) return !1;
+                for (var e = tt || ut(), t = Math.max(0, l.startTime + l.duration - e), n = 1 - (t / l.duration || 0), r = 0, i = l.tweens.length; r < i; r++) l.tweens[r].run(n);
+                return s.notifyWith(o, [l, n, t]), n < 1 && i ? t : (i || s.notifyWith(o, [l, 1, 0]), s.resolveWith(o, [l]), !1)
+            },
+            l = s.promise({
+                elem: o,
+                props: S.extend({}, e),
+                opts: S.extend(!0, {
+                    specialEasing: {},
+                    easing: S.easing._default
+                }, t),
+                originalProperties: e,
+                originalOptions: t,
+                startTime: tt || ut(),
+                duration: t.duration,
                 tweens: [],
-                createTween: function(b, c) {
-                    var d = o.Tween(a, j.opts, b, c, j.opts.specialEasing[b] || j.opts.easing);
-                    return j.tweens.push(d), d
-                },
-                stop: function(b) {
-                    var c = 0,
-                        d = b ? j.tweens.length : 0;
-                    if (e) return this;
-                    for (e = !0; d > c; c++) j.tweens[c].run(1);
-                    return b ? h.resolveWith(a, [j, b]) : h.rejectWith(a, [j, b]), this
+                createTween: function(e, t) {
+                    var n = S.Tween(o, l.opts, e, t, l.opts.specialEasing[e] || l.opts.easing);
+                    return l.tweens.push(n), n
+                },
+                stop: function(e) {
+                    var t = 0,
+                        n = e ? l.tweens.length : 0;
+                    if (a) return this;
+                    for (a = !0; t < n; t++) l.tweens[t].run(1);
+                    return e ? (s.notifyWith(o, [l, 1, 0]), s.resolveWith(o, [l, e])) : s.rejectWith(o, [l, e]), this
                 }
             }),
-            k = j.props;
-        for (Wb(k, j.opts.specialEasing); g > f; f++)
-            if (d = Qb[f].call(j, a, k, j.opts)) return d;
-        return o.map(k, Ub, j), o.isFunction(j.opts.start) && j.opts.start.call(a, j), o.fx.timer(o.extend(i, {
-            elem: a,
-            anim: j,
-            queue: j.opts.queue
-        })), j.progress(j.opts.progress).done(j.opts.done, j.opts.complete).fail(j.opts.fail).always(j.opts.always)
-    }
-    o.Animation = o.extend(Xb, {
-            tweener: function(a, b) {
-                o.isFunction(a) ? (b = a, a = ["*"]) : a = a.split(" ");
-                for (var c, d = 0, e = a.length; e > d; d++) c = a[d], Rb[c] = Rb[c] || [], Rb[c].unshift(b)
-            },
-            prefilter: function(a, b) {
-                b ? Qb.unshift(a) : Qb.push(a)
-            }
-        }), o.speed = function(a, b, c) {
-            var d = a && "object" == typeof a ? o.extend({}, a) : {
-                complete: c || !c && b || o.isFunction(a) && a,
-                duration: a,
-                easing: c && b || b && !o.isFunction(b) && b
-            };
-            return d.duration = o.fx.off ? 0 : "number" == typeof d.duration ? d.duration : d.duration in o.fx.speeds ? o.fx.speeds[d.duration] : o.fx.speeds._default, (null == d.queue || d.queue === !0) && (d.queue = "fx"), d.old = d.complete, d.complete = function() {
-                o.isFunction(d.old) && d.old.call(this), d.queue && o.dequeue(this, d.queue)
-            }, d
-        }, o.fn.extend({
-            fadeTo: function(a, b, c, d) {
-                return this.filter(S).css("opacity", 0).show().end().animate({
-                    opacity: b
-                }, a, c, d)
-            },
-            animate: function(a, b, c, d) {
-                var e = o.isEmptyObject(a),
-                    f = o.speed(b, c, d),
-                    g = function() {
-                        var b = Xb(this, o.extend({}, a), f);
-                        (e || L.get(this, "finish")) && b.stop(!0)
-                    };
-                return g.finish = g, e || f.queue === !1 ? this.each(g) : this.queue(f.queue, g)
-            },
-            stop: function(a, b, c) {
-                var d = function(a) {
-                    var b = a.stop;
-                    delete a.stop, b(c)
+            c = l.props;
+        for (! function(e, t) {
+                var n, r, i, o, a;
+                for (n in e)
+                    if (i = t[r = X(n)], o = e[n], Array.isArray(o) && (i = o[1], o = e[n] = o[0]), n !== r && (e[r] = o, delete e[n]), (a = S.cssHooks[r]) && "expand" in a)
+                        for (n in o = a.expand(o), delete e[r], o) n in e || (e[n] = o[n], t[n] = i);
+                    else t[r] = i
+            }(c, l.opts.specialEasing); r < i; r++)
+            if (n = ft.prefilters[r].call(l, o, c, l.opts)) return m(n.stop) && (S._queueHooks(l.elem, l.opts.queue).stop = n.stop.bind(n)), n;
+        return S.map(c, ct, l), m(l.opts.start) && l.opts.start.call(o, l), l.progress(l.opts.progress).done(l.opts.done, l.opts.complete).fail(l.opts.fail).always(l.opts.always), S.fx.timer(S.extend(u, {
+            elem: o,
+            anim: l,
+            queue: l.opts.queue
+        })), l
+    }
+    S.Animation = S.extend(ft, {
+        tweeners: {
+            "*": [function(e, t) {
+                var n = this.createTween(e, t);
+                return se(n.elem, e, te.exec(t), n), n
+            }]
+        },
+        tweener: function(e, t) {
+            m(e) ? (t = e, e = ["*"]) : e = e.match(P);
+            for (var n, r = 0, i = e.length; r < i; r++) n = e[r], ft.tweeners[n] = ft.tweeners[n] || [], ft.tweeners[n].unshift(t)
+        },
+        prefilters: [function(e, t, n) {
+            var r, i, o, a, s, u, l, c, f = "width" in t || "height" in t,
+                p = this,
+                d = {},
+                h = e.style,
+                g = e.nodeType && ae(e),
+                y = Y.get(e, "fxshow");
+            for (r in n.queue || (null == (a = S._queueHooks(e, "fx")).unqueued && (a.unqueued = 0, s = a.empty.fire, a.empty.fire = function() {
+                    a.unqueued || s()
+                }), a.unqueued++, p.always(function() {
+                    p.always(function() {
+                        a.unqueued--, S.queue(e, "fx").length || a.empty.fire()
+                    })
+                })), t)
+                if (i = t[r], ot.test(i)) {
+                    if (delete t[r], o = o || "toggle" === i, i === (g ? "hide" : "show")) {
+                        if ("show" !== i || !y || void 0 === y[r]) continue;
+                        g = !0
+                    }
+                    d[r] = y && y[r] || S.style(e, r)
+                } if ((u = !S.isEmptyObject(t)) || !S.isEmptyObject(d))
+                for (r in f && 1 === e.nodeType && (n.overflow = [h.overflow, h.overflowX, h.overflowY], null == (l = y && y.display) && (l = Y.get(e, "display")), "none" === (c = S.css(e, "display")) && (l ? c = l : (le([e], !0), l = e.style.display || l, c = S.css(e, "display"), le([e]))), ("inline" === c || "inline-block" === c && null != l) && "none" === S.css(e, "float") && (u || (p.done(function() {
+                        h.display = l
+                    }), null == l && (c = h.display, l = "none" === c ? "" : c)), h.display = "inline-block")), n.overflow && (h.overflow = "hidden", p.always(function() {
+                        h.overflow = n.overflow[0], h.overflowX = n.overflow[1], h.overflowY = n.overflow[2]
+                    })), u = !1, d) u || (y ? "hidden" in y && (g = y.hidden) : y = Y.access(e, "fxshow", {
+                    display: l
+                }), o && (y.hidden = !g), g && le([e], !0), p.done(function() {
+                    for (r in g || le([e]), Y.remove(e, "fxshow"), d) S.style(e, r, d[r])
+                })), u = ct(g ? y[r] : 0, r, p), r in y || (y[r] = u.start, g && (u.end = u.start, u.start = 0))
+        }],
+        prefilter: function(e, t) {
+            t ? ft.prefilters.unshift(e) : ft.prefilters.push(e)
+        }
+    }), S.speed = function(e, t, n) {
+        var r = e && "object" == typeof e ? S.extend({}, e) : {
+            complete: n || !n && t || m(e) && e,
+            duration: e,
+            easing: n && t || t && !m(t) && t
+        };
+        return S.fx.off ? r.duration = 0 : "number" != typeof r.duration && (r.duration in S.fx.speeds ? r.duration = S.fx.speeds[r.duration] : r.duration = S.fx.speeds._default), null != r.queue && !0 !== r.queue || (r.queue = "fx"), r.old = r.complete, r.complete = function() {
+            m(r.old) && r.old.call(this), r.queue && S.dequeue(this, r.queue)
+        }, r
+    }, S.fn.extend({
+        fadeTo: function(e, t, n, r) {
+            return this.filter(ae).css("opacity", 0).show().end().animate({
+                opacity: t
+            }, e, n, r)
+        },
+        animate: function(t, e, n, r) {
+            var i = S.isEmptyObject(t),
+                o = S.speed(e, n, r),
+                a = function() {
+                    var e = ft(this, S.extend({}, t), o);
+                    (i || Y.get(this, "finish")) && e.stop(!0)
                 };
-                return "string" != typeof a && (c = b, b = a, a = void 0), b && a !== !1 && this.queue(a || "fx", []), this.each(function() {
-                    var b = !0,
-                        e = null != a && a + "queueHooks",
-                        f = o.timers,
-                        g = L.get(this);
-                    if (e) g[e] && g[e].stop && d(g[e]);
-                    else
-                        for (e in g) g[e] && g[e].stop && Pb.test(e) && d(g[e]);
-                    for (e = f.length; e--;) f[e].elem !== this || null != a && f[e].queue !== a || (f[e].anim.stop(c), b = !1, f.splice(e, 1));
-                    (b || !c) && o.dequeue(this, a)
-                })
-            },
-            finish: function(a) {
-                return a !== !1 && (a = a || "fx"), this.each(function() {
-                    var b, c = L.get(this),
-                        d = c[a + "queue"],
-                        e = c[a + "queueHooks"],
-                        f = o.timers,
-                        g = d ? d.length : 0;
-                    for (c.finish = !0, o.queue(this, a, []), e && e.stop && e.stop.call(this, !0), b = f.length; b--;) f[b].elem === this && f[b].queue === a && (f[b].anim.stop(!0), f.splice(b, 1));
-                    for (b = 0; g > b; b++) d[b] && d[b].finish && d[b].finish.call(this);
-                    delete c.finish
-                })
-            }
-        }), o.each(["toggle", "show", "hide"], function(a, b) {
-            var c = o.fn[b];
-            o.fn[b] = function(a, d, e) {
-                return null == a || "boolean" == typeof a ? c.apply(this, arguments) : this.animate(Tb(b, !0), a, d, e)
-            }
-        }), o.each({
-            slideDown: Tb("show"),
-            slideUp: Tb("hide"),
-            slideToggle: Tb("toggle"),
-            fadeIn: {
-                opacity: "show"
-            },
-            fadeOut: {
-                opacity: "hide"
-            },
-            fadeToggle: {
-                opacity: "toggle"
-            }
-        }, function(a, b) {
-            o.fn[a] = function(a, c, d) {
-                return this.animate(b, a, c, d)
-            }
-        }), o.timers = [], o.fx.tick = function() {
-            var a, b = 0,
-                c = o.timers;
-            for (Lb = o.now(); b < c.length; b++) a = c[b], a() || c[b] !== a || c.splice(b--, 1);
-            c.length || o.fx.stop(), Lb = void 0
-        }, o.fx.timer = function(a) {
-            o.timers.push(a), a() ? o.fx.start() : o.timers.pop()
-        }, o.fx.interval = 13, o.fx.start = function() {
-            Mb || (Mb = setInterval(o.fx.tick, o.fx.interval))
-        }, o.fx.stop = function() {
-            clearInterval(Mb), Mb = null
-        }, o.fx.speeds = {
-            slow: 600,
-            fast: 200,
-            _default: 400
-        }, o.fn.delay = function(a, b) {
-            return a = o.fx ? o.fx.speeds[a] || a : a, b = b || "fx", this.queue(b, function(b, c) {
-                var d = setTimeout(b, a);
-                c.stop = function() {
-                    clearTimeout(d)
-                }
-            })
+            return a.finish = a, i || !1 === o.queue ? this.each(a) : this.queue(o.queue, a)
         },
-        function() {
-            var a = m.createElement("input"),
-                b = m.createElement("select"),
-                c = b.appendChild(m.createElement("option"));
-            a.type = "checkbox", l.checkOn = "" !== a.value, l.optSelected = c.selected, b.disabled = !0, l.optDisabled = !c.disabled, a = m.createElement("input"), a.value = "t", a.type = "radio", l.radioValue = "t" === a.value
-        }();
-    var Yb, Zb, $b = o.expr.attrHandle;
-    o.fn.extend({
-        attr: function(a, b) {
-            return J(this, o.attr, a, b, arguments.length > 1)
+        stop: function(i, e, o) {
+            var a = function(e) {
+                var t = e.stop;
+                delete e.stop, t(o)
+            };
+            return "string" != typeof i && (o = e, e = i, i = void 0), e && this.queue(i || "fx", []), this.each(function() {
+                var e = !0,
+                    t = null != i && i + "queueHooks",
+                    n = S.timers,
+                    r = Y.get(this);
+                if (t) r[t] && r[t].stop && a(r[t]);
+                else
+                    for (t in r) r[t] && r[t].stop && at.test(t) && a(r[t]);
+                for (t = n.length; t--;) n[t].elem !== this || null != i && n[t].queue !== i || (n[t].anim.stop(o), e = !1, n.splice(t, 1));
+                !e && o || S.dequeue(this, i)
+            })
+        },
+        finish: function(a) {
+            return !1 !== a && (a = a || "fx"), this.each(function() {
+                var e, t = Y.get(this),
+                    n = t[a + "queue"],
+                    r = t[a + "queueHooks"],
+                    i = S.timers,
+                    o = n ? n.length : 0;
+                for (t.finish = !0, S.queue(this, a, []), r && r.stop && r.stop.call(this, !0), e = i.length; e--;) i[e].elem === this && i[e].queue === a && (i[e].anim.stop(!0), i.splice(e, 1));
+                for (e = 0; e < o; e++) n[e] && n[e].finish && n[e].finish.call(this);
+                delete t.finish
+            })
+        }
+    }), S.each(["toggle", "show", "hide"], function(e, r) {
+        var i = S.fn[r];
+        S.fn[r] = function(e, t, n) {
+            return null == e || "boolean" == typeof e ? i.apply(this, arguments) : this.animate(lt(r, !0), e, t, n)
+        }
+    }), S.each({
+        slideDown: lt("show"),
+        slideUp: lt("hide"),
+        slideToggle: lt("toggle"),
+        fadeIn: {
+            opacity: "show"
+        },
+        fadeOut: {
+            opacity: "hide"
+        },
+        fadeToggle: {
+            opacity: "toggle"
+        }
+    }, function(e, r) {
+        S.fn[e] = function(e, t, n) {
+            return this.animate(r, e, t, n)
+        }
+    }), S.timers = [], S.fx.tick = function() {
+        var e, t = 0,
+            n = S.timers;
+        for (tt = Date.now(); t < n.length; t++)(e = n[t])() || n[t] !== e || n.splice(t--, 1);
+        n.length || S.fx.stop(), tt = void 0
+    }, S.fx.timer = function(e) {
+        S.timers.push(e), S.fx.start()
+    }, S.fx.interval = 13, S.fx.start = function() {
+        nt || (nt = !0, st())
+    }, S.fx.stop = function() {
+        nt = null
+    }, S.fx.speeds = {
+        slow: 600,
+        fast: 200,
+        _default: 400
+    }, S.fn.delay = function(r, e) {
+        return r = S.fx && S.fx.speeds[r] || r, e = e || "fx", this.queue(e, function(e, t) {
+            var n = C.setTimeout(e, r);
+            t.stop = function() {
+                C.clearTimeout(n)
+            }
+        })
+    }, rt = E.createElement("input"), it = E.createElement("select").appendChild(E.createElement("option")), rt.type = "checkbox", v.checkOn = "" !== rt.value, v.optSelected = it.selected, (rt = E.createElement("input")).value = "t", rt.type = "radio", v.radioValue = "t" === rt.value;
+    var pt, dt = S.expr.attrHandle;
+    S.fn.extend({
+        attr: function(e, t) {
+            return B(this, S.attr, e, t, 1 < arguments.length)
         },
-        removeAttr: function(a) {
+        removeAttr: function(e) {
             return this.each(function() {
-                o.removeAttr(this, a)
+                S.removeAttr(this, e)
             })
         }
-    }), o.extend({
-        attr: function(a, b, c) {
-            var d, e, f = a.nodeType;
-            if (a && 3 !== f && 8 !== f && 2 !== f) return typeof a.getAttribute === U ? o.prop(a, b, c) : (1 === f && o.isXMLDoc(a) || (b = b.toLowerCase(), d = o.attrHooks[b] || (o.expr.match.bool.test(b) ? Zb : Yb)), void 0 === c ? d && "get" in d && null !== (e = d.get(a, b)) ? e : (e = o.find.attr(a, b), null == e ? void 0 : e) : null !== c ? d && "set" in d && void 0 !== (e = d.set(a, c, b)) ? e : (a.setAttribute(b, c + ""), c) : void o.removeAttr(a, b))
-        },
-        removeAttr: function(a, b) {
-            var c, d, e = 0,
-                f = b && b.match(E);
-            if (f && 1 === a.nodeType)
-                while (c = f[e++]) d = o.propFix[c] || c, o.expr.match.bool.test(c) && (a[d] = !1), a.removeAttribute(c)
+    }), S.extend({
+        attr: function(e, t, n) {
+            var r, i, o = e.nodeType;
+            if (3 !== o && 8 !== o && 2 !== o) return "undefined" == typeof e.getAttribute ? S.prop(e, t, n) : (1 === o && S.isXMLDoc(e) || (i = S.attrHooks[t.toLowerCase()] || (S.expr.match.bool.test(t) ? pt : void 0)), void 0 !== n ? null === n ? void S.removeAttr(e, t) : i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : (e.setAttribute(t, n + ""), n) : i && "get" in i && null !== (r = i.get(e, t)) ? r : null == (r = S.find.attr(e, t)) ? void 0 : r)
         },
         attrHooks: {
             type: {
-                set: function(a, b) {
-                    if (!l.radioValue && "radio" === b && o.nodeName(a, "input")) {
-                        var c = a.value;
-                        return a.setAttribute("type", b), c && (a.value = c), b
+                set: function(e, t) {
+                    if (!v.radioValue && "radio" === t && A(e, "input")) {
+                        var n = e.value;
+                        return e.setAttribute("type", t), n && (e.value = n), t
                     }
                 }
             }
+        },
+        removeAttr: function(e, t) {
+            var n, r = 0,
+                i = t && t.match(P);
+            if (i && 1 === e.nodeType)
+                while (n = i[r++]) e.removeAttribute(n)
         }
-    }), Zb = {
-        set: function(a, b, c) {
-            return b === !1 ? o.removeAttr(a, c) : a.setAttribute(c, c), c
+    }), pt = {
+        set: function(e, t, n) {
+            return !1 === t ? S.removeAttr(e, n) : e.setAttribute(n, n), n
         }
-    }, o.each(o.expr.match.bool.source.match(/\w+/g), function(a, b) {
-        var c = $b[b] || o.find.attr;
-        $b[b] = function(a, b, d) {
-            var e, f;
-            return d || (f = $b[b], $b[b] = e, e = null != c(a, b, d) ? b.toLowerCase() : null, $b[b] = f), e
+    }, S.each(S.expr.match.bool.source.match(/\w+/g), function(e, t) {
+        var a = dt[t] || S.find.attr;
+        dt[t] = function(e, t, n) {
+            var r, i, o = t.toLowerCase();
+            return n || (i = dt[o], dt[o] = r, r = null != a(e, t, n) ? o : null, dt[o] = i), r
         }
     });
-    var _b = /^(?:input|select|textarea|button)$/i;
-    o.fn.extend({
-        prop: function(a, b) {
-            return J(this, o.prop, a, b, arguments.length > 1)
+    var ht = /^(?:input|select|textarea|button)$/i,
+        gt = /^(?:a|area)$/i;
+
+    function yt(e) {
+        return (e.match(P) || []).join(" ")
+    }
+
+    function vt(e) {
+        return e.getAttribute && e.getAttribute("class") || ""
+    }
+
+    function mt(e) {
+        return Array.isArray(e) ? e : "string" == typeof e && e.match(P) || []
+    }
+    S.fn.extend({
+        prop: function(e, t) {
+            return B(this, S.prop, e, t, 1 < arguments.length)
         },
-        removeProp: function(a) {
+        removeProp: function(e) {
             return this.each(function() {
-                delete this[o.propFix[a] || a]
+                delete this[S.propFix[e] || e]
             })
         }
-    }), o.extend({
-        propFix: {
-            "for": "htmlFor",
-            "class": "className"
-        },
-        prop: function(a, b, c) {
-            var d, e, f, g = a.nodeType;
-            if (a && 3 !== g && 8 !== g && 2 !== g) return f = 1 !== g || !o.isXMLDoc(a), f && (b = o.propFix[b] || b, e = o.propHooks[b]), void 0 !== c ? e && "set" in e && void 0 !== (d = e.set(a, c, b)) ? d : a[b] = c : e && "get" in e && null !== (d = e.get(a, b)) ? d : a[b]
+    }), S.extend({
+        prop: function(e, t, n) {
+            var r, i, o = e.nodeType;
+            if (3 !== o && 8 !== o && 2 !== o) return 1 === o && S.isXMLDoc(e) || (t = S.propFix[t] || t, i = S.propHooks[t]), void 0 !== n ? i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : e[t] = n : i && "get" in i && null !== (r = i.get(e, t)) ? r : e[t]
         },
         propHooks: {
             tabIndex: {
-                get: function(a) {
-                    return a.hasAttribute("tabindex") || _b.test(a.nodeName) || a.href ? a.tabIndex : -1
+                get: function(e) {
+                    var t = S.find.attr(e, "tabindex");
+                    return t ? parseInt(t, 10) : ht.test(e.nodeName) || gt.test(e.nodeName) && e.href ? 0 : -1
                 }
             }
+        },
+        propFix: {
+            "for": "htmlFor",
+            "class": "className"
         }
-    }), l.optSelected || (o.propHooks.selected = {
-        get: function(a) {
-            var b = a.parentNode;
-            return b && b.parentNode && b.parentNode.selectedIndex, null
-        }
-    }), o.each(["tabIndex", "readOnly", "maxLength", "cellSpacing", "cellPadding", "rowSpan", "colSpan", "useMap", "frameBorder", "contentEditable"], function() {
-        o.propFix[this.toLowerCase()] = this
-    });
-    var ac = /[\t\r\n\f]/g;
-    o.fn.extend({
-        addClass: function(a) {
-            var b, c, d, e, f, g, h = "string" == typeof a && a,
-                i = 0,
-                j = this.length;
-            if (o.isFunction(a)) return this.each(function(b) {
-                o(this).addClass(a.call(this, b, this.className))
-            });
-            if (h)
-                for (b = (a || "").match(E) || []; j > i; i++)
-                    if (c = this[i], d = 1 === c.nodeType && (c.className ? (" " + c.className + " ").replace(ac, " ") : " ")) {
-                        f = 0;
-                        while (e = b[f++]) d.indexOf(" " + e + " ") < 0 && (d += e + " ");
-                        g = o.trim(d), c.className !== g && (c.className = g)
-                    } return this
-        },
-        removeClass: function(a) {
-            var b, c, d, e, f, g, h = 0 === arguments.length || "string" == typeof a && a,
-                i = 0,
-                j = this.length;
-            if (o.isFunction(a)) return this.each(function(b) {
-                o(this).removeClass(a.call(this, b, this.className))
-            });
-            if (h)
-                for (b = (a || "").match(E) || []; j > i; i++)
-                    if (c = this[i], d = 1 === c.nodeType && (c.className ? (" " + c.className + " ").replace(ac, " ") : "")) {
-                        f = 0;
-                        while (e = b[f++])
-                            while (d.indexOf(" " + e + " ") >= 0) d = d.replace(" " + e + " ", " ");
-                        g = a ? o.trim(d) : "", c.className !== g && (c.className = g)
-                    } return this
-        },
-        toggleClass: function(a, b) {
-            var c = typeof a;
-            return "boolean" == typeof b && "string" === c ? b ? this.addClass(a) : this.removeClass(a) : this.each(o.isFunction(a) ? function(c) {
-                o(this).toggleClass(a.call(this, c, this.className, b), b)
-            } : function() {
-                if ("string" === c) {
-                    var b, d = 0,
-                        e = o(this),
-                        f = a.match(E) || [];
-                    while (b = f[d++]) e.hasClass(b) ? e.removeClass(b) : e.addClass(b)
-                } else(c === U || "boolean" === c) && (this.className && L.set(this, "__className__", this.className), this.className = this.className || a === !1 ? "" : L.get(this, "__className__") || "")
-            })
+    }), v.optSelected || (S.propHooks.selected = {
+        get: function(e) {
+            var t = e.parentNode;
+            return t && t.parentNode && t.parentNode.selectedIndex, null
+        },
+        set: function(e) {
+            var t = e.parentNode;
+            t && (t.selectedIndex, t.parentNode && t.parentNode.selectedIndex)
+        }
+    }), S.each(["tabIndex", "readOnly", "maxLength", "cellSpacing", "cellPadding", "rowSpan", "colSpan", "useMap", "frameBorder", "contentEditable"], function() {
+        S.propFix[this.toLowerCase()] = this
+    }), S.fn.extend({
+        addClass: function(t) {
+            var e, n, r, i, o, a;
+            return m(t) ? this.each(function(e) {
+                S(this).addClass(t.call(this, e, vt(this)))
+            }) : (e = mt(t)).length ? this.each(function() {
+                if (r = vt(this), n = 1 === this.nodeType && " " + yt(r) + " ") {
+                    for (o = 0; o < e.length; o++) i = e[o], n.indexOf(" " + i + " ") < 0 && (n += i + " ");
+                    a = yt(n), r !== a && this.setAttribute("class", a)
+                }
+            }) : this
+        },
+        removeClass: function(t) {
+            var e, n, r, i, o, a;
+            return m(t) ? this.each(function(e) {
+                S(this).removeClass(t.call(this, e, vt(this)))
+            }) : arguments.length ? (e = mt(t)).length ? this.each(function() {
+                if (r = vt(this), n = 1 === this.nodeType && " " + yt(r) + " ") {
+                    for (o = 0; o < e.length; o++) {
+                        i = e[o];
+                        while (-1 < n.indexOf(" " + i + " ")) n = n.replace(" " + i + " ", " ")
+                    }
+                    a = yt(n), r !== a && this.setAttribute("class", a)
+                }
+            }) : this : this.attr("class", "")
+        },
+        toggleClass: function(t, n) {
+            var e, r, i, o, a = typeof t,
+                s = "string" === a || Array.isArray(t);
+            return m(t) ? this.each(function(e) {
+                S(this).toggleClass(t.call(this, e, vt(this), n), n)
+            }) : "boolean" == typeof n && s ? n ? this.addClass(t) : this.removeClass(t) : (e = mt(t), this.each(function() {
+                if (s)
+                    for (o = S(this), i = 0; i < e.length; i++) r = e[i], o.hasClass(r) ? o.removeClass(r) : o.addClass(r);
+                else void 0 !== t && "boolean" !== a || ((r = vt(this)) && Y.set(this, "__className__", r), this.setAttribute && this.setAttribute("class", r || !1 === t ? "" : Y.get(this, "__className__") || ""))
+            }))
         },
-        hasClass: function(a) {
-            for (var b = " " + a + " ", c = 0, d = this.length; d > c; c++)
-                if (1 === this[c].nodeType && (" " + this[c].className + " ").replace(ac, " ").indexOf(b) >= 0) return !0;
+        hasClass: function(e) {
+            var t, n, r = 0;
+            t = " " + e + " ";
+            while (n = this[r++])
+                if (1 === n.nodeType && -1 < (" " + yt(vt(n)) + " ").indexOf(t)) return !0;
             return !1
         }
     });
-    var bc = /\r/g;
-    o.fn.extend({
-        val: function(a) {
-            var b, c, d, e = this[0]; {
-                if (arguments.length) return d = o.isFunction(a), this.each(function(c) {
-                    var e;
-                    1 === this.nodeType && (e = d ? a.call(this, c, o(this).val()) : a, null == e ? e = "" : "number" == typeof e ? e += "" : o.isArray(e) && (e = o.map(e, function(a) {
-                        return null == a ? "" : a + ""
-                    })), b = o.valHooks[this.type] || o.valHooks[this.nodeName.toLowerCase()], b && "set" in b && void 0 !== b.set(this, e, "value") || (this.value = e))
-                });
-                if (e) return b = o.valHooks[e.type] || o.valHooks[e.nodeName.toLowerCase()], b && "get" in b && void 0 !== (c = b.get(e, "value")) ? c : (c = e.value, "string" == typeof c ? c.replace(bc, "") : null == c ? "" : c)
-            }
+    var xt = /\r/g;
+    S.fn.extend({
+        val: function(n) {
+            var r, e, i, t = this[0];
+            return arguments.length ? (i = m(n), this.each(function(e) {
+                var t;
+                1 === this.nodeType && (null == (t = i ? n.call(this, e, S(this).val()) : n) ? t = "" : "number" == typeof t ? t += "" : Array.isArray(t) && (t = S.map(t, function(e) {
+                    return null == e ? "" : e + ""
+                })), (r = S.valHooks[this.type] || S.valHooks[this.nodeName.toLowerCase()]) && "set" in r && void 0 !== r.set(this, t, "value") || (this.value = t))
+            })) : t ? (r = S.valHooks[t.type] || S.valHooks[t.nodeName.toLowerCase()]) && "get" in r && void 0 !== (e = r.get(t, "value")) ? e : "string" == typeof(e = t.value) ? e.replace(xt, "") : null == e ? "" : e : void 0
         }
-    }), o.extend({
+    }), S.extend({
         valHooks: {
+            option: {
+                get: function(e) {
+                    var t = S.find.attr(e, "value");
+                    return null != t ? t : yt(S.text(e))
+                }
+            },
             select: {
-                get: function(a) {
-                    for (var b, c, d = a.options, e = a.selectedIndex, f = "select-one" === a.type || 0 > e, g = f ? null : [], h = f ? e + 1 : d.length, i = 0 > e ? h : f ? e : 0; h > i; i++)
-                        if (c = d[i], !(!c.selected && i !== e || (l.optDisabled ? c.disabled : null !== c.getAttribute("disabled")) || c.parentNode.disabled && o.nodeName(c.parentNode, "optgroup"))) {
-                            if (b = o(c).val(), f) return b;
-                            g.push(b)
-                        } return g
-                },
-                set: function(a, b) {
-                    var c, d, e = a.options,
-                        f = o.makeArray(b),
-                        g = e.length;
-                    while (g--) d = e[g], (d.selected = o.inArray(o(d).val(), f) >= 0) && (c = !0);
-                    return c || (a.selectedIndex = -1), f
+                get: function(e) {
+                    var t, n, r, i = e.options,
+                        o = e.selectedIndex,
+                        a = "select-one" === e.type,
+                        s = a ? null : [],
+                        u = a ? o + 1 : i.length;
+                    for (r = o < 0 ? u : a ? o : 0; r < u; r++)
+                        if (((n = i[r]).selected || r === o) && !n.disabled && (!n.parentNode.disabled || !A(n.parentNode, "optgroup"))) {
+                            if (t = S(n).val(), a) return t;
+                            s.push(t)
+                        } return s
+                },
+                set: function(e, t) {
+                    var n, r, i = e.options,
+                        o = S.makeArray(t),
+                        a = i.length;
+                    while (a--)((r = i[a]).selected = -1 < S.inArray(S.valHooks.option.get(r), o)) && (n = !0);
+                    return n || (e.selectedIndex = -1), o
                 }
             }
         }
-    }), o.each(["radio", "checkbox"], function() {
-        o.valHooks[this] = {
-            set: function(a, b) {
-                return o.isArray(b) ? a.checked = o.inArray(o(a).val(), b) >= 0 : void 0
+    }), S.each(["radio", "checkbox"], function() {
+        S.valHooks[this] = {
+            set: function(e, t) {
+                if (Array.isArray(t)) return e.checked = -1 < S.inArray(S(e).val(), t)
             }
-        }, l.checkOn || (o.valHooks[this].get = function(a) {
-            return null === a.getAttribute("value") ? "on" : a.value
+        }, v.checkOn || (S.valHooks[this].get = function(e) {
+            return null === e.getAttribute("value") ? "on" : e.value
         })
-    }), o.each("blur focus focusin focusout load resize scroll unload click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup error contextmenu".split(" "), function(a, b) {
-        o.fn[b] = function(a, c) {
-            return arguments.length > 0 ? this.on(b, null, a, c) : this.trigger(b)
+    }), v.focusin = "onfocusin" in C;
+    var bt = /^(?:focusinfocus|focusoutblur)$/,
+        wt = function(e) {
+            e.stopPropagation()
+        };
+    S.extend(S.event, {
+        trigger: function(e, t, n, r) {
+            var i, o, a, s, u, l, c, f, p = [n || E],
+                d = y.call(e, "type") ? e.type : e,
+                h = y.call(e, "namespace") ? e.namespace.split(".") : [];
+            if (o = f = a = n = n || E, 3 !== n.nodeType && 8 !== n.nodeType && !bt.test(d + S.event.triggered) && (-1 < d.indexOf(".") && (d = (h = d.split(".")).shift(), h.sort()), u = d.indexOf(":") < 0 && "on" + d, (e = e[S.expando] ? e : new S.Event(d, "object" == typeof e && e)).isTrigger = r ? 2 : 3, e.namespace = h.join("."), e.rnamespace = e.namespace ? new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, e.result = void 0, e.target || (e.target = n), t = null == t ? [e] : S.makeArray(t, [e]), c = S.event.special[d] || {}, r || !c.trigger || !1 !== c.trigger.apply(n, t))) {
+                if (!r && !c.noBubble && !x(n)) {
+                    for (s = c.delegateType || d, bt.test(s + d) || (o = o.parentNode); o; o = o.parentNode) p.push(o), a = o;
+                    a === (n.ownerDocument || E) && p.push(a.defaultView || a.parentWindow || C)
+                }
+                i = 0;
+                while ((o = p[i++]) && !e.isPropagationStopped()) f = o, e.type = 1 < i ? s : c.bindType || d, (l = (Y.get(o, "events") || Object.create(null))[e.type] && Y.get(o, "handle")) && l.apply(o, t), (l = u && o[u]) && l.apply && V(o) && (e.result = l.apply(o, t), !1 === e.result && e.preventDefault());
+                return e.type = d, r || e.isDefaultPrevented() || c._default && !1 !== c._default.apply(p.pop(), t) || !V(n) || u && m(n[d]) && !x(n) && ((a = n[u]) && (n[u] = null), S.event.triggered = d, e.isPropagationStopped() && f.addEventListener(d, wt), n[d](), e.isPropagationStopped() && f.removeEventListener(d, wt), S.event.triggered = void 0, a && (n[u] = a)), e.result
+            }
+        },
+        simulate: function(e, t, n) {
+            var r = S.extend(new S.Event, n, {
+                type: e,
+                isSimulated: !0
+            });
+            S.event.trigger(r, null, t)
         }
-    }), o.fn.extend({
-        hover: function(a, b) {
-            return this.mouseenter(a).mouseleave(b || a)
-        },
-        bind: function(a, b, c) {
-            return this.on(a, null, b, c)
-        },
-        unbind: function(a, b) {
-            return this.off(a, null, b)
-        },
-        delegate: function(a, b, c, d) {
-            return this.on(b, a, c, d)
+    }), S.fn.extend({
+        trigger: function(e, t) {
+            return this.each(function() {
+                S.event.trigger(e, t, this)
+            })
         },
-        undelegate: function(a, b, c) {
-            return 1 === arguments.length ? this.off(a, "**") : this.off(b, a || "**", c)
+        triggerHandler: function(e, t) {
+            var n = this[0];
+            if (n) return S.event.trigger(e, t, n, !0)
+        }
+    }), v.focusin || S.each({
+        focus: "focusin",
+        blur: "focusout"
+    }, function(n, r) {
+        var i = function(e) {
+            S.event.simulate(r, e.target, S.event.fix(e))
+        };
+        S.event.special[r] = {
+            setup: function() {
+                var e = this.ownerDocument || this.document || this,
+                    t = Y.access(e, r);
+                t || e.addEventListener(n, i, !0), Y.access(e, r, (t || 0) + 1)
+            },
+            teardown: function() {
+                var e = this.ownerDocument || this.document || this,
+                    t = Y.access(e, r) - 1;
+                t ? Y.access(e, r, t) : (e.removeEventListener(n, i, !0), Y.remove(e, r))
+            }
         }
     });
-    var cc = o.now(),
-        dc = /\?/;
-    o.parseJSON = function(a) {
-        return JSON.parse(a + "")
-    }, o.parseXML = function(a) {
-        var b, c;
-        if (!a || "string" != typeof a) return null;
+    var Tt = C.location,
+        Ct = {
+            guid: Date.now()
+        },
+        Et = /\?/;
+    S.parseXML = function(e) {
+        var t, n;
+        if (!e || "string" != typeof e) return null;
         try {
-            c = new DOMParser, b = c.parseFromString(a, "text/xml")
-        } catch (d) {
-            b = void 0
-        }
-        return (!b || b.getElementsByTagName("parsererror").length) && o.error("Invalid XML: " + a), b
+            t = (new C.DOMParser).parseFromString(e, "text/xml")
+        } catch (e) {}
+        return n = t && t.getElementsByTagName("parsererror")[0], t && !n || S.error("Invalid XML: " + (n ? S.map(n.childNodes, function(e) {
+            return e.textContent
+        }).join("\n") : e)), t
     };
-    var ec, fc, gc = /#.*$/,
-        hc = /([?&])_=[^&]*/,
-        ic = /^(.*?):[ \t]*([^\r\n]*)$/gm,
-        jc = /^(?:about|app|app-storage|.+-extension|file|res|widget):$/,
-        kc = /^(?:GET|HEAD)$/,
-        lc = /^\/\//,
-        mc = /^([\w.+-]+:)(?:\/\/(?:[^\/?#]*@|)([^\/?#:]*)(?::(\d+)|)|)/,
-        nc = {},
-        oc = {},
-        pc = "*/".concat("*");
-    try {
-        fc = location.href
-    } catch (qc) {
-        fc = m.createElement("a"), fc.href = "", fc = fc.href
-    }
-    ec = mc.exec(fc.toLowerCase()) || [];
-
-    function rc(a) {
-        return function(b, c) {
-            "string" != typeof b && (c = b, b = "*");
-            var d, e = 0,
-                f = b.toLowerCase().match(E) || [];
-            if (o.isFunction(c))
-                while (d = f[e++]) "+" === d[0] ? (d = d.slice(1) || "*", (a[d] = a[d] || []).unshift(c)) : (a[d] = a[d] || []).push(c)
-        }
-    }
-
-    function sc(a, b, c, d) {
-        var e = {},
-            f = a === oc;
-
-        function g(h) {
-            var i;
-            return e[h] = !0, o.each(a[h] || [], function(a, h) {
-                var j = h(b, c, d);
-                return "string" != typeof j || f || e[j] ? f ? !(i = j) : void 0 : (b.dataTypes.unshift(j), g(j), !1)
-            }), i
-        }
-        return g(b.dataTypes[0]) || !e["*"] && g("*")
-    }
-
-    function tc(a, b) {
-        var c, d, e = o.ajaxSettings.flatOptions || {};
-        for (c in b) void 0 !== b[c] && ((e[c] ? a : d || (d = {}))[c] = b[c]);
-        return d && o.extend(!0, a, d), a
-    }
-
-    function uc(a, b, c) {
-        var d, e, f, g, h = a.contents,
-            i = a.dataTypes;
-        while ("*" === i[0]) i.shift(), void 0 === d && (d = a.mimeType || b.getResponseHeader("Content-Type"));
-        if (d)
-            for (e in h)
-                if (h[e] && h[e].test(d)) {
-                    i.unshift(e);
-                    break
-                } if (i[0] in c) f = i[0];
-        else {
-            for (e in c) {
-                if (!i[0] || a.converters[e + " " + i[0]]) {
-                    f = e;
-                    break
-                }
-                g || (g = e)
-            }
-            f = f || g
-        }
-        return f ? (f !== i[0] && i.unshift(f), c[f]) : void 0
-    }
-
-    function vc(a, b, c, d) {
-        var e, f, g, h, i, j = {},
-            k = a.dataTypes.slice();
-        if (k[1])
-            for (g in a.converters) j[g.toLowerCase()] = a.converters[g];
-        f = k.shift();
-        while (f)
-            if (a.responseFields[f] && (c[a.responseFields[f]] = b), !i && d && a.dataFilter && (b = a.dataFilter(b, a.dataType)), i = f, f = k.shift())
-                if ("*" === f) f = i;
-                else if ("*" !== i && i !== f) {
-            if (g = j[i + " " + f] || j["* " + f], !g)
-                for (e in j)
-                    if (h = e.split(" "), h[1] === f && (g = j[i + " " + h[0]] || j["* " + h[0]])) {
-                        g === !0 ? g = j[e] : j[e] !== !0 && (f = h[0], k.unshift(h[1]));
-                        break
-                    } if (g !== !0)
-                if (g && a["throws"]) b = g(b);
-                else try {
-                    b = g(b)
-                } catch (l) {
+    var St = /\[\]$/,
+        kt = /\r?\n/g,
+        At = /^(?:submit|button|image|reset|file)$/i,
+        Nt = /^(?:input|select|textarea|keygen)/i;
+
+    function jt(n, e, r, i) {
+        var t;
+        if (Array.isArray(e)) S.each(e, function(e, t) {
+            r || St.test(n) ? i(n, t) : jt(n + "[" + ("object" == typeof t && null != t ? e : "") + "]", t, r, i)
+        });
+        else if (r || "object" !== w(e)) i(n, e);
+        else
+            for (t in e) jt(n + "[" + t + "]", e[t], r, i)
+    }
+    S.param = function(e, t) {
+        var n, r = [],
+            i = function(e, t) {
+                var n = m(t) ? t() : t;
+                r[r.length] = encodeURIComponent(e) + "=" + encodeURIComponent(null == n ? "" : n)
+            };
+        if (null == e) return "";
+        if (Array.isArray(e) || e.jquery && !S.isPlainObject(e)) S.each(e, function() {
+            i(this.name, this.value)
+        });
+        else
+            for (n in e) jt(n, e[n], t, i);
+        return r.join("&")
+    }, S.fn.extend({
+        serialize: function() {
+            return S.param(this.serializeArray())
+        },
+        serializeArray: function() {
+            return this.map(function() {
+                var e = S.prop(this, "elements");
+                return e ? S.makeArray(e) : this
+            }).filter(function() {
+                var e = this.type;
+                return this.name && !S(this).is(":disabled") && Nt.test(this.nodeName) && !At.test(e) && (this.checked || !pe.test(e))
+            }).map(function(e, t) {
+                var n = S(this).val();
+                return null == n ? null : Array.isArray(n) ? S.map(n, function(e) {
                     return {
-                        state: "parsererror",
-                        error: g ? l : "No conversion from " + i + " to " + f
+                        name: t.name,
+                        value: e.replace(kt, "\r\n")
                     }
+                }) : {
+                    name: t.name,
+                    value: n.replace(kt, "\r\n")
                 }
+            }).get()
         }
-        return {
-            state: "success",
-            data: b
+    });
+    var Dt = /%20/g,
+        qt = /#.*$/,
+        Lt = /([?&])_=[^&]*/,
+        Ht = /^(.*?):[ \t]*([^\r\n]*)$/gm,
+        Ot = /^(?:GET|HEAD)$/,
+        Pt = /^\/\//,
+        Rt = {},
+        Mt = {},
+        It = "*/".concat("*"),
+        Wt = E.createElement("a");
+
+    function Ft(o) {
+        return function(e, t) {
+            "string" != typeof e && (t = e, e = "*");
+            var n, r = 0,
+                i = e.toLowerCase().match(P) || [];
+            if (m(t))
+                while (n = i[r++]) "+" === n[0] ? (n = n.slice(1) || "*", (o[n] = o[n] || []).unshift(t)) : (o[n] = o[n] || []).push(t)
         }
     }
-    o.extend({
+
+    function $t(t, i, o, a) {
+        var s = {},
+            u = t === Mt;
+
+        function l(e) {
+            var r;
+            return s[e] = !0, S.each(t[e] || [], function(e, t) {
+                var n = t(i, o, a);
+                return "string" != typeof n || u || s[n] ? u ? !(r = n) : void 0 : (i.dataTypes.unshift(n), l(n), !1)
+            }), r
+        }
+        return l(i.dataTypes[0]) || !s["*"] && l("*")
+    }
+
+    function Bt(e, t) {
+        var n, r, i = S.ajaxSettings.flatOptions || {};
+        for (n in t) void 0 !== t[n] && ((i[n] ? e : r || (r = {}))[n] = t[n]);
+        return r && S.extend(!0, e, r), e
+    }
+    Wt.href = Tt.href, S.extend({
         active: 0,
         lastModified: {},
         etag: {},
         ajaxSettings: {
-            url: fc,
+            url: Tt.href,
             type: "GET",
-            isLocal: jc.test(ec[1]),
+            isLocal: /^(?:about|app|app-storage|.+-extension|file|res|widget):$/.test(Tt.protocol),
             global: !0,
             processData: !0,
             async: !0,
             contentType: "application/x-www-form-urlencoded; charset=UTF-8",
             accepts: {
-                "*": pc,
+                "*": It,
                 text: "text/plain",
                 html: "text/html",
                 xml: "application/xml, text/xml",
                 json: "application/json, text/javascript"
             },
             contents: {
-                xml: /xml/,
-                html: /html/,
-                json: /json/
+                xml: /\bxml\b/,
+                html: /\bhtml/,
+                json: /\bjson\b/
             },
             responseFields: {
                 xml: "responseXML",
                 text: "responseText",
                 json: "responseJSON"
             },
             converters: {
                 "* text": String,
                 "text html": !0,
-                "text json": o.parseJSON,
-                "text xml": o.parseXML
+                "text json": JSON.parse,
+                "text xml": S.parseXML
             },
             flatOptions: {
                 url: !0,
                 context: !0
             }
         },
-        ajaxSetup: function(a, b) {
-            return b ? tc(tc(a, o.ajaxSettings), b) : tc(o.ajaxSettings, a)
+        ajaxSetup: function(e, t) {
+            return t ? Bt(Bt(e, S.ajaxSettings), t) : Bt(S.ajaxSettings, e)
         },
-        ajaxPrefilter: rc(nc),
-        ajaxTransport: rc(oc),
-        ajax: function(a, b) {
-            "object" == typeof a && (b = a, a = void 0), b = b || {};
-            var c, d, e, f, g, h, i, j, k = o.ajaxSetup({}, b),
-                l = k.context || k,
-                m = k.context && (l.nodeType || l.jquery) ? o(l) : o.event,
-                n = o.Deferred(),
-                p = o.Callbacks("once memory"),
-                q = k.statusCode || {},
-                r = {},
+        ajaxPrefilter: Ft(Rt),
+        ajaxTransport: Ft(Mt),
+        ajax: function(e, t) {
+            "object" == typeof e && (t = e, e = void 0), t = t || {};
+            var c, f, p, n, d, r, h, g, i, o, y = S.ajaxSetup({}, t),
+                v = y.context || y,
+                m = y.context && (v.nodeType || v.jquery) ? S(v) : S.event,
+                x = S.Deferred(),
+                b = S.Callbacks("once memory"),
+                w = y.statusCode || {},
+                a = {},
                 s = {},
-                t = 0,
                 u = "canceled",
-                v = {
+                T = {
                     readyState: 0,
-                    getResponseHeader: function(a) {
-                        var b;
-                        if (2 === t) {
-                            if (!f) {
-                                f = {};
-                                while (b = ic.exec(e)) f[b[1].toLowerCase()] = b[2]
+                    getResponseHeader: function(e) {
+                        var t;
+                        if (h) {
+                            if (!n) {
+                                n = {};
+                                while (t = Ht.exec(p)) n[t[1].toLowerCase() + " "] = (n[t[1].toLowerCase() + " "] || []).concat(t[2])
                             }
-                            b = f[a.toLowerCase()]
+                            t = n[e.toLowerCase() + " "]
                         }
-                        return null == b ? null : b
+                        return null == t ? null : t.join(", ")
                     },
                     getAllResponseHeaders: function() {
-                        return 2 === t ? e : null
+                        return h ? p : null
+                    },
+                    setRequestHeader: function(e, t) {
+                        return null == h && (e = s[e.toLowerCase()] = s[e.toLowerCase()] || e, a[e] = t), this
                     },
-                    setRequestHeader: function(a, b) {
-                        var c = a.toLowerCase();
-                        return t || (a = s[c] = s[c] || a, r[a] = b), this
-                    },
-                    overrideMimeType: function(a) {
-                        return t || (k.mimeType = a), this
-                    },
-                    statusCode: function(a) {
-                        var b;
-                        if (a)
-                            if (2 > t)
-                                for (b in a) q[b] = [q[b], a[b]];
-                            else v.always(a[v.status]);
+                    overrideMimeType: function(e) {
+                        return null == h && (y.mimeType = e), this
+                    },
+                    statusCode: function(e) {
+                        var t;
+                        if (e)
+                            if (h) T.always(e[T.status]);
+                            else
+                                for (t in e) w[t] = [w[t], e[t]];
                         return this
                     },
-                    abort: function(a) {
-                        var b = a || u;
-                        return c && c.abort(b), x(0, b), this
+                    abort: function(e) {
+                        var t = e || u;
+                        return c && c.abort(t), l(0, t), this
                     }
                 };
-            if (n.promise(v).complete = p.add, v.success = v.done, v.error = v.fail, k.url = ((a || k.url || fc) + "").replace(gc, "").replace(lc, ec[1] + "//"), k.type = b.method || b.type || k.method || k.type, k.dataTypes = o.trim(k.dataType || "*").toLowerCase().match(E) || [""], null == k.crossDomain && (h = mc.exec(k.url.toLowerCase()), k.crossDomain = !(!h || h[1] === ec[1] && h[2] === ec[2] && (h[3] || ("http:" === h[1] ? "80" : "443")) === (ec[3] || ("http:" === ec[1] ? "80" : "443")))), k.data && k.processData && "string" != typeof k.data && (k.data = o.param(k.data, k.traditional)), sc(nc, k, b, v), 2 === t) return v;
-            i = k.global, i && 0 === o.active++ && o.event.trigger("ajaxStart"), k.type = k.type.toUpperCase(), k.hasContent = !kc.test(k.type), d = k.url, k.hasContent || (k.data && (d = k.url += (dc.test(d) ? "&" : "?") + k.data, delete k.data), k.cache === !1 && (k.url = hc.test(d) ? d.replace(hc, "$1_=" + cc++) : d + (dc.test(d) ? "&" : "?") + "_=" + cc++)), k.ifModified && (o.lastModified[d] && v.setRequestHeader("If-Modified-Since", o.lastModified[d]), o.etag[d] && v.setRequestHeader("If-None-Match", o.etag[d])), (k.data && k.hasContent && k.contentType !== !1 || b.contentType) && v.setRequestHeader("Content-Type", k.contentType), v.setRequestHeader("Accept", k.dataTypes[0] && k.accepts[k.dataTypes[0]] ? k.accepts[k.dataTypes[0]] + ("*" !== k.dataTypes[0] ? ", " + pc + "; q=0.01" : "") : k.accepts["*"]);
-            for (j in k.headers) v.setRequestHeader(j, k.headers[j]);
-            if (k.beforeSend && (k.beforeSend.call(l, v, k) === !1 || 2 === t)) return v.abort();
-            u = "abort";
-            for (j in {
-                    success: 1,
-                    error: 1,
-                    complete: 1
-                }) v[j](k[j]);
-            if (c = sc(oc, k, b, v)) {
-                v.readyState = 1, i && m.trigger("ajaxSend", [v, k]), k.async && k.timeout > 0 && (g = setTimeout(function() {
-                    v.abort("timeout")
-                }, k.timeout));
+            if (x.promise(T), y.url = ((e || y.url || Tt.href) + "").replace(Pt, Tt.protocol + "//"), y.type = t.method || t.type || y.method || y.type, y.dataTypes = (y.dataType || "*").toLowerCase().match(P) || [""], null == y.crossDomain) {
+                r = E.createElement("a");
                 try {
-                    t = 1, c.send(r, x)
-                } catch (w) {
-                    if (!(2 > t)) throw w;
-                    x(-1, w)
-                }
-            } else x(-1, "No Transport");
-
-            function x(a, b, f, h) {
-                var j, r, s, u, w, x = b;
-                2 !== t && (t = 2, g && clearTimeout(g), c = void 0, e = h || "", v.readyState = a > 0 ? 4 : 0, j = a >= 200 && 300 > a || 304 === a, f && (u = uc(k, v, f)), u = vc(k, u, v, j), j ? (k.ifModified && (w = v.getResponseHeader("Last-Modified"), w && (o.lastModified[d] = w), w = v.getResponseHeader("etag"), w && (o.etag[d] = w)), 204 === a || "HEAD" === k.type ? x = "nocontent" : 304 === a ? x = "notmodified" : (x = u.state, r = u.data, s = u.error, j = !s)) : (s = x, (a || !x) && (x = "error", 0 > a && (a = 0))), v.status = a, v.statusText = (b || x) + "", j ? n.resolveWith(l, [r, x, v]) : n.rejectWith(l, [v, x, s]), v.statusCode(q), q = void 0, i && m.trigger(j ? "ajaxSuccess" : "ajaxError", [v, k, j ? r : s]), p.fireWith(l, [v, x]), i && (m.trigger("ajaxComplete", [v, k]), --o.active || o.event.trigger("ajaxStop")))
-            }
-            return v
-        },
-        getJSON: function(a, b, c) {
-            return o.get(a, b, c, "json")
-        },
-        getScript: function(a, b) {
-            return o.get(a, void 0, b, "script")
-        }
-    }), o.each(["get", "post"], function(a, b) {
-        o[b] = function(a, c, d, e) {
-            return o.isFunction(c) && (e = e || d, d = c, c = void 0), o.ajax({
-                url: a,
-                type: b,
-                dataType: e,
-                data: c,
-                success: d
-            })
-        }
-    }), o.each(["ajaxStart", "ajaxStop", "ajaxComplete", "ajaxError", "ajaxSuccess", "ajaxSend"], function(a, b) {
-        o.fn[b] = function(a) {
-            return this.on(b, a)
-        }
-    }), o._evalUrl = function(a) {
-        return o.ajax({
-            url: a,
+                    r.href = y.url, r.href = r.href, y.crossDomain = Wt.protocol + "//" + Wt.host != r.protocol + "//" + r.host
+                } catch (e) {
+                    y.crossDomain = !0
+                }
+            }
+            if (y.data && y.processData && "string" != typeof y.data && (y.data = S.param(y.data, y.traditional)), $t(Rt, y, t, T), h) return T;
+            for (i in (g = S.event && y.global) && 0 == S.active++ && S.event.trigger("ajaxStart"), y.type = y.type.toUpperCase(), y.hasContent = !Ot.test(y.type), f = y.url.replace(qt, ""), y.hasContent ? y.data && y.processData && 0 === (y.contentType || "").indexOf("application/x-www-form-urlencoded") && (y.data = y.data.replace(Dt, "+")) : (o = y.url.slice(f.length), y.data && (y.processData || "string" == typeof y.data) && (f += (Et.test(f) ? "&" : "?") + y.data, delete y.data), !1 === y.cache && (f = f.replace(Lt, "$1"), o = (Et.test(f) ? "&" : "?") + "_=" + Ct.guid++ + o), y.url = f + o), y.ifModified && (S.lastModified[f] && T.setRequestHeader("If-Modified-Since", S.lastModified[f]), S.etag[f] && T.setRequestHeader("If-None-Match", S.etag[f])), (y.data && y.hasContent && !1 !== y.contentType || t.contentType) && T.setRequestHeader("Content-Type", y.contentType), T.setRequestHeader("Accept", y.dataTypes[0] && y.accepts[y.dataTypes[0]] ? y.accepts[y.dataTypes[0]] + ("*" !== y.dataTypes[0] ? ", " + It + "; q=0.01" : "") : y.accepts["*"]), y.headers) T.setRequestHeader(i, y.headers[i]);
+            if (y.beforeSend && (!1 === y.beforeSend.call(v, T, y) || h)) return T.abort();
+            if (u = "abort", b.add(y.complete), T.done(y.success), T.fail(y.error), c = $t(Mt, y, t, T)) {
+                if (T.readyState = 1, g && m.trigger("ajaxSend", [T, y]), h) return T;
+                y.async && 0 < y.timeout && (d = C.setTimeout(function() {
+                    T.abort("timeout")
+                }, y.timeout));
+                try {
+                    h = !1, c.send(a, l)
+                } catch (e) {
+                    if (h) throw e;
+                    l(-1, e)
+                }
+            } else l(-1, "No Transport");
+
+            function l(e, t, n, r) {
+                var i, o, a, s, u, l = t;
+                h || (h = !0, d && C.clearTimeout(d), c = void 0, p = r || "", T.readyState = 0 < e ? 4 : 0, i = 200 <= e && e < 300 || 304 === e, n && (s = function(e, t, n) {
+                    var r, i, o, a, s = e.contents,
+                        u = e.dataTypes;
+                    while ("*" === u[0]) u.shift(), void 0 === r && (r = e.mimeType || t.getResponseHeader("Content-Type"));
+                    if (r)
+                        for (i in s)
+                            if (s[i] && s[i].test(r)) {
+                                u.unshift(i);
+                                break
+                            } if (u[0] in n) o = u[0];
+                    else {
+                        for (i in n) {
+                            if (!u[0] || e.converters[i + " " + u[0]]) {
+                                o = i;
+                                break
+                            }
+                            a || (a = i)
+                        }
+                        o = o || a
+                    }
+                    if (o) return o !== u[0] && u.unshift(o), n[o]
+                }(y, T, n)), !i && -1 < S.inArray("script", y.dataTypes) && S.inArray("json", y.dataTypes) < 0 && (y.converters["text script"] = function() {}), s = function(e, t, n, r) {
+                    var i, o, a, s, u, l = {},
+                        c = e.dataTypes.slice();
+                    if (c[1])
+                        for (a in e.converters) l[a.toLowerCase()] = e.converters[a];
+                    o = c.shift();
+                    while (o)
+                        if (e.responseFields[o] && (n[e.responseFields[o]] = t), !u && r && e.dataFilter && (t = e.dataFilter(t, e.dataType)), u = o, o = c.shift())
+                            if ("*" === o) o = u;
+                            else if ("*" !== u && u !== o) {
+                        if (!(a = l[u + " " + o] || l["* " + o]))
+                            for (i in l)
+                                if ((s = i.split(" "))[1] === o && (a = l[u + " " + s[0]] || l["* " + s[0]])) {
+                                    !0 === a ? a = l[i] : !0 !== l[i] && (o = s[0], c.unshift(s[1]));
+                                    break
+                                } if (!0 !== a)
+                            if (a && e["throws"]) t = a(t);
+                            else try {
+                                t = a(t)
+                            } catch (e) {
+                                return {
+                                    state: "parsererror",
+                                    error: a ? e : "No conversion from " + u + " to " + o
+                                }
+                            }
+                    }
+                    return {
+                        state: "success",
+                        data: t
+                    }
+                }(y, s, T, i), i ? (y.ifModified && ((u = T.getResponseHeader("Last-Modified")) && (S.lastModified[f] = u), (u = T.getResponseHeader("etag")) && (S.etag[f] = u)), 204 === e || "HEAD" === y.type ? l = "nocontent" : 304 === e ? l = "notmodified" : (l = s.state, o = s.data, i = !(a = s.error))) : (a = l, !e && l || (l = "error", e < 0 && (e = 0))), T.status = e, T.statusText = (t || l) + "", i ? x.resolveWith(v, [o, l, T]) : x.rejectWith(v, [T, l, a]), T.statusCode(w), w = void 0, g && m.trigger(i ? "ajaxSuccess" : "ajaxError", [T, y, i ? o : a]), b.fireWith(v, [T, l]), g && (m.trigger("ajaxComplete", [T, y]), --S.active || S.event.trigger("ajaxStop")))
+            }
+            return T
+        },
+        getJSON: function(e, t, n) {
+            return S.get(e, t, n, "json")
+        },
+        getScript: function(e, t) {
+            return S.get(e, void 0, t, "script")
+        }
+    }), S.each(["get", "post"], function(e, i) {
+        S[i] = function(e, t, n, r) {
+            return m(t) && (r = r || n, n = t, t = void 0), S.ajax(S.extend({
+                url: e,
+                type: i,
+                dataType: r,
+                data: t,
+                success: n
+            }, S.isPlainObject(e) && e))
+        }
+    }), S.ajaxPrefilter(function(e) {
+        var t;
+        for (t in e.headers) "content-type" === t.toLowerCase() && (e.contentType = e.headers[t] || "")
+    }), S._evalUrl = function(e, t, n) {
+        return S.ajax({
+            url: e,
             type: "GET",
             dataType: "script",
+            cache: !0,
             async: !1,
             global: !1,
-            "throws": !0
+            converters: {
+                "text script": function() {}
+            },
+            dataFilter: function(e) {
+                S.globalEval(e, t, n)
+            }
         })
-    }, o.fn.extend({
-        wrapAll: function(a) {
-            var b;
-            return o.isFunction(a) ? this.each(function(b) {
-                o(this).wrapAll(a.call(this, b))
-            }) : (this[0] && (b = o(a, this[0].ownerDocument).eq(0).clone(!0), this[0].parentNode && b.insertBefore(this[0]), b.map(function() {
-                var a = this;
-                while (a.firstElementChild) a = a.firstElementChild;
-                return a
-            }).append(this)), this)
-        },
-        wrapInner: function(a) {
-            return this.each(o.isFunction(a) ? function(b) {
-                o(this).wrapInner(a.call(this, b))
-            } : function() {
-                var b = o(this),
-                    c = b.contents();
-                c.length ? c.wrapAll(a) : b.append(a)
-            })
-        },
-        wrap: function(a) {
-            var b = o.isFunction(a);
-            return this.each(function(c) {
-                o(this).wrapAll(b ? a.call(this, c) : a)
-            })
-        },
-        unwrap: function() {
-            return this.parent().each(function() {
-                o.nodeName(this, "body") || o(this).replaceWith(this.childNodes)
-            }).end()
-        }
-    }), o.expr.filters.hidden = function(a) {
-        return a.offsetWidth <= 0 && a.offsetHeight <= 0
-    }, o.expr.filters.visible = function(a) {
-        return !o.expr.filters.hidden(a)
-    };
-    var wc = /%20/g,
-        xc = /\[\]$/,
-        yc = /\r?\n/g,
-        zc = /^(?:submit|button|image|reset|file)$/i,
-        Ac = /^(?:input|select|textarea|keygen)/i;
-
-    function Bc(a, b, c, d) {
-        var e;
-        if (o.isArray(b)) o.each(b, function(b, e) {
-            c || xc.test(a) ? d(a, e) : Bc(a + "[" + ("object" == typeof e ? b : "") + "]", e, c, d)
-        });
-        else if (c || "object" !== o.type(b)) d(a, b);
-        else
-            for (e in b) Bc(a + "[" + e + "]", b[e], c, d)
-    }
-    o.param = function(a, b) {
-        var c, d = [],
-            e = function(a, b) {
-                b = o.isFunction(b) ? b() : null == b ? "" : b, d[d.length] = encodeURIComponent(a) + "=" + encodeURIComponent(b)
-            };
-        if (void 0 === b && (b = o.ajaxSettings && o.ajaxSettings.traditional), o.isArray(a) || a.jquery && !o.isPlainObject(a)) o.each(a, function() {
-            e(this.name, this.value)
-        });
-        else
-            for (c in a) Bc(c, a[c], b, e);
-        return d.join("&").replace(wc, "+")
-    }, o.fn.extend({
-        serialize: function() {
-            return o.param(this.serializeArray())
+    }, S.fn.extend({
+        wrapAll: function(e) {
+            var t;
+            return this[0] && (m(e) && (e = e.call(this[0])), t = S(e, this[0].ownerDocument).eq(0).clone(!0), this[0].parentNode && t.insertBefore(this[0]), t.map(function() {
+                var e = this;
+                while (e.firstElementChild) e = e.firstElementChild;
+                return e
+            }).append(this)), this
         },
-        serializeArray: function() {
-            return this.map(function() {
-                var a = o.prop(this, "elements");
-                return a ? o.makeArray(a) : this
-            }).filter(function() {
-                var a = this.type;
-                return this.name && !o(this).is(":disabled") && Ac.test(this.nodeName) && !zc.test(a) && (this.checked || !T.test(a))
-            }).map(function(a, b) {
-                var c = o(this).val();
-                return null == c ? null : o.isArray(c) ? o.map(c, function(a) {
-                    return {
-                        name: b.name,
-                        value: a.replace(yc, "\r\n")
-                    }
-                }) : {
-                    name: b.name,
-                    value: c.replace(yc, "\r\n")
-                }
-            }).get()
-        }
-    }), o.ajaxSettings.xhr = function() {
+        wrapInner: function(n) {
+            return m(n) ? this.each(function(e) {
+                S(this).wrapInner(n.call(this, e))
+            }) : this.each(function() {
+                var e = S(this),
+                    t = e.contents();
+                t.length ? t.wrapAll(n) : e.append(n)
+            })
+        },
+        wrap: function(t) {
+            var n = m(t);
+            return this.each(function(e) {
+                S(this).wrapAll(n ? t.call(this, e) : t)
+            })
+        },
+        unwrap: function(e) {
+            return this.parent(e).not("body").each(function() {
+                S(this).replaceWith(this.childNodes)
+            }), this
+        }
+    }), S.expr.pseudos.hidden = function(e) {
+        return !S.expr.pseudos.visible(e)
+    }, S.expr.pseudos.visible = function(e) {
+        return !!(e.offsetWidth || e.offsetHeight || e.getClientRects().length)
+    }, S.ajaxSettings.xhr = function() {
         try {
-            return new XMLHttpRequest
-        } catch (a) {}
+            return new C.XMLHttpRequest
+        } catch (e) {}
     };
-    var Cc = 0,
-        Dc = {},
-        Ec = {
+    var _t = {
             0: 200,
             1223: 204
         },
-        Fc = o.ajaxSettings.xhr();
-    a.ActiveXObject && o(a).on("unload", function() {
-        for (var a in Dc) Dc[a]()
-    }), l.cors = !!Fc && "withCredentials" in Fc, l.ajax = Fc = !!Fc, o.ajaxTransport(function(a) {
-        var b;
-        return l.cors || Fc && !a.crossDomain ? {
-            send: function(c, d) {
-                var e, f = a.xhr(),
-                    g = ++Cc;
-                if (f.open(a.type, a.url, a.async, a.username, a.password), a.xhrFields)
-                    for (e in a.xhrFields) f[e] = a.xhrFields[e];
-                a.mimeType && f.overrideMimeType && f.overrideMimeType(a.mimeType), a.crossDomain || c["X-Requested-With"] || (c["X-Requested-With"] = "XMLHttpRequest");
-                for (e in c) f.setRequestHeader(e, c[e]);
-                b = function(a) {
+        zt = S.ajaxSettings.xhr();
+    v.cors = !!zt && "withCredentials" in zt, v.ajax = zt = !!zt, S.ajaxTransport(function(i) {
+        var o, a;
+        if (v.cors || zt && !i.crossDomain) return {
+            send: function(e, t) {
+                var n, r = i.xhr();
+                if (r.open(i.type, i.url, i.async, i.username, i.password), i.xhrFields)
+                    for (n in i.xhrFields) r[n] = i.xhrFields[n];
+                for (n in i.mimeType && r.overrideMimeType && r.overrideMimeType(i.mimeType), i.crossDomain || e["X-Requested-With"] || (e["X-Requested-With"] = "XMLHttpRequest"), e) r.setRequestHeader(n, e[n]);
+                o = function(e) {
                     return function() {
-                        b && (delete Dc[g], b = f.onload = f.onerror = null, "abort" === a ? f.abort() : "error" === a ? d(f.status, f.statusText) : d(Ec[f.status] || f.status, f.statusText, "string" == typeof f.responseText ? {
-                            text: f.responseText
-                        } : void 0, f.getAllResponseHeaders()))
-                    }
-                }, f.onload = b(), f.onerror = b("error"), b = Dc[g] = b("abort"), f.send(a.hasContent && a.data || null)
+                        o && (o = a = r.onload = r.onerror = r.onabort = r.ontimeout = r.onreadystatechange = null, "abort" === e ? r.abort() : "error" === e ? "number" != typeof r.status ? t(0, "error") : t(r.status, r.statusText) : t(_t[r.status] || r.status, r.statusText, "text" !== (r.responseType || "text") || "string" != typeof r.responseText ? {
+                            binary: r.response
+                        } : {
+                            text: r.responseText
+                        }, r.getAllResponseHeaders()))
+                    }
+                }, r.onload = o(), a = r.onerror = r.ontimeout = o("error"), void 0 !== r.onabort ? r.onabort = a : r.onreadystatechange = function() {
+                    4 === r.readyState && C.setTimeout(function() {
+                        o && a()
+                    })
+                }, o = o("abort");
+                try {
+                    r.send(i.hasContent && i.data || null)
+                } catch (e) {
+                    if (o) throw e
+                }
             },
             abort: function() {
-                b && b()
+                o && o()
             }
-        } : void 0
-    }), o.ajaxSetup({
+        }
+    }), S.ajaxPrefilter(function(e) {
+        e.crossDomain && (e.contents.script = !1)
+    }), S.ajaxSetup({
         accepts: {
             script: "text/javascript, application/javascript, application/ecmascript, application/x-ecmascript"
         },
         contents: {
-            script: /(?:java|ecma)script/
+            script: /\b(?:java|ecma)script\b/
         },
         converters: {
-            "text script": function(a) {
-                return o.globalEval(a), a
+            "text script": function(e) {
+                return S.globalEval(e), e
             }
         }
-    }), o.ajaxPrefilter("script", function(a) {
-        void 0 === a.cache && (a.cache = !1), a.crossDomain && (a.type = "GET")
-    }), o.ajaxTransport("script", function(a) {
-        if (a.crossDomain) {
-            var b, c;
-            return {
-                send: function(d, e) {
-                    b = o("<script>").prop({
-                        async: !0,
-                        charset: a.scriptCharset,
-                        src: a.url
-                    }).on("load error", c = function(a) {
-                        b.remove(), c = null, a && e("error" === a.type ? 404 : 200, a.type)
-                    }), m.head.appendChild(b[0])
-                },
-                abort: function() {
-                    c && c()
-                }
+    }), S.ajaxPrefilter("script", function(e) {
+        void 0 === e.cache && (e.cache = !1), e.crossDomain && (e.type = "GET")
+    }), S.ajaxTransport("script", function(n) {
+        var r, i;
+        if (n.crossDomain || n.scriptAttrs) return {
+            send: function(e, t) {
+                r = S("<script>").attr(n.scriptAttrs || {}).prop({
+                    charset: n.scriptCharset,
+                    src: n.url
+                }).on("load error", i = function(e) {
+                    r.remove(), i = null, e && t("error" === e.type ? 404 : 200, e.type)
+                }), E.head.appendChild(r[0])
+            },
+            abort: function() {
+                i && i()
             }
         }
     });
-    var Gc = [],
-        Hc = /(=)\?(?=&|$)|\?\?/;
-    o.ajaxSetup({
+    var Ut, Xt = [],
+        Vt = /(=)\?(?=&|$)|\?\?/;
+    S.ajaxSetup({
         jsonp: "callback",
         jsonpCallback: function() {
-            var a = Gc.pop() || o.expando + "_" + cc++;
-            return this[a] = !0, a
+            var e = Xt.pop() || S.expando + "_" + Ct.guid++;
+            return this[e] = !0, e
         }
-    }), o.ajaxPrefilter("json jsonp", function(b, c, d) {
-        var e, f, g, h = b.jsonp !== !1 && (Hc.test(b.url) ? "url" : "string" == typeof b.data && !(b.contentType || "").indexOf("application/x-www-form-urlencoded") && Hc.test(b.data) && "data");
-        return h || "jsonp" === b.dataTypes[0] ? (e = b.jsonpCallback = o.isFunction(b.jsonpCallback) ? b.jsonpCallback() : b.jsonpCallback, h ? b[h] = b[h].replace(Hc, "$1" + e) : b.jsonp !== !1 && (b.url += (dc.test(b.url) ? "&" : "?") + b.jsonp + "=" + e), b.converters["script json"] = function() {
-            return g || o.error(e + " was not called"), g[0]
-        }, b.dataTypes[0] = "json", f = a[e], a[e] = function() {
-            g = arguments
-        }, d.always(function() {
-            a[e] = f, b[e] && (b.jsonpCallback = c.jsonpCallback, Gc.push(e)), g && o.isFunction(f) && f(g[0]), g = f = void 0
-        }), "script") : void 0
-    }), o.parseHTML = function(a, b, c) {
-        if (!a || "string" != typeof a) return null;
-        "boolean" == typeof b && (c = b, b = !1), b = b || m;
-        var d = v.exec(a),
-            e = !c && [];
-        return d ? [b.createElement(d[1])] : (d = o.buildFragment([a], b, e), e && e.length && o(e).remove(), o.merge([], d.childNodes))
-    };
-    var Ic = o.fn.load;
-    o.fn.load = function(a, b, c) {
-        if ("string" != typeof a && Ic) return Ic.apply(this, arguments);
-        var d, e, f, g = this,
-            h = a.indexOf(" ");
-        return h >= 0 && (d = a.slice(h), a = a.slice(0, h)), o.isFunction(b) ? (c = b, b = void 0) : b && "object" == typeof b && (e = "POST"), g.length > 0 && o.ajax({
-            url: a,
-            type: e,
+    }), S.ajaxPrefilter("json jsonp", function(e, t, n) {
+        var r, i, o, a = !1 !== e.jsonp && (Vt.test(e.url) ? "url" : "string" == typeof e.data && 0 === (e.contentType || "").indexOf("application/x-www-form-urlencoded") && Vt.test(e.data) && "data");
+        if (a || "jsonp" === e.dataTypes[0]) return r = e.jsonpCallback = m(e.jsonpCallback) ? e.jsonpCallback() : e.jsonpCallback, a ? e[a] = e[a].replace(Vt, "$1" + r) : !1 !== e.jsonp && (e.url += (Et.test(e.url) ? "&" : "?") + e.jsonp + "=" + r), e.converters["script json"] = function() {
+            return o || S.error(r + " was not called"), o[0]
+        }, e.dataTypes[0] = "json", i = C[r], C[r] = function() {
+            o = arguments
+        }, n.always(function() {
+            void 0 === i ? S(C).removeProp(r) : C[r] = i, e[r] && (e.jsonpCallback = t.jsonpCallback, Xt.push(r)), o && m(i) && i(o[0]), o = i = void 0
+        }), "script"
+    }), v.createHTMLDocument = ((Ut = E.implementation.createHTMLDocument("").body).innerHTML = "<form></form><form></form>", 2 === Ut.childNodes.length), S.parseHTML = function(e, t, n) {
+        return "string" != typeof e ? [] : ("boolean" == typeof t && (n = t, t = !1), t || (v.createHTMLDocument ? ((r = (t = E.implementation.createHTMLDocument("")).createElement("base")).href = E.location.href, t.head.appendChild(r)) : t = E), o = !n && [], (i = N.exec(e)) ? [t.createElement(i[1])] : (i = xe([e], t, o), o && o.length && S(o).remove(), S.merge([], i.childNodes)));
+        var r, i, o
+    }, S.fn.load = function(e, t, n) {
+        var r, i, o, a = this,
+            s = e.indexOf(" ");
+        return -1 < s && (r = yt(e.slice(s)), e = e.slice(0, s)), m(t) ? (n = t, t = void 0) : t && "object" == typeof t && (i = "POST"), 0 < a.length && S.ajax({
+            url: e,
+            type: i || "GET",
             dataType: "html",
-            data: b
-        }).done(function(a) {
-            f = arguments, g.html(d ? o("<div>").append(o.parseHTML(a)).find(d) : a)
-        }).complete(c && function(a, b) {
-            g.each(c, f || [a.responseText, b, a])
+            data: t
+        }).done(function(e) {
+            o = arguments, a.html(r ? S("<div>").append(S.parseHTML(e)).find(r) : e)
+        }).always(n && function(e, t) {
+            a.each(function() {
+                n.apply(this, o || [e.responseText, t, e])
+            })
         }), this
-    }, o.expr.filters.animated = function(a) {
-        return o.grep(o.timers, function(b) {
-            return a === b.elem
+    }, S.expr.pseudos.animated = function(t) {
+        return S.grep(S.timers, function(e) {
+            return t === e.elem
         }).length
-    };
-    var Jc = a.document.documentElement;
-
-    function Kc(a) {
-        return o.isWindow(a) ? a : 9 === a.nodeType && a.defaultView
-    }
-    o.offset = {
-        setOffset: function(a, b, c) {
-            var d, e, f, g, h, i, j, k = o.css(a, "position"),
-                l = o(a),
-                m = {};
-            "static" === k && (a.style.position = "relative"), h = l.offset(), f = o.css(a, "top"), i = o.css(a, "left"), j = ("absolute" === k || "fixed" === k) && (f + i).indexOf("auto") > -1, j ? (d = l.position(), g = d.top, e = d.left) : (g = parseFloat(f) || 0, e = parseFloat(i) || 0), o.isFunction(b) && (b = b.call(a, c, h)), null != b.top && (m.top = b.top - h.top + g), null != b.left && (m.left = b.left - h.left + e), "using" in b ? b.using.call(a, m) : l.css(m)
-        }
-    }, o.fn.extend({
-        offset: function(a) {
-            if (arguments.length) return void 0 === a ? this : this.each(function(b) {
-                o.offset.setOffset(this, a, b)
+    }, S.offset = {
+        setOffset: function(e, t, n) {
+            var r, i, o, a, s, u, l = S.css(e, "position"),
+                c = S(e),
+                f = {};
+            "static" === l && (e.style.position = "relative"), s = c.offset(), o = S.css(e, "top"), u = S.css(e, "left"), ("absolute" === l || "fixed" === l) && -1 < (o + u).indexOf("auto") ? (a = (r = c.position()).top, i = r.left) : (a = parseFloat(o) || 0, i = parseFloat(u) || 0), m(t) && (t = t.call(e, n, S.extend({}, s))), null != t.top && (f.top = t.top - s.top + a), null != t.left && (f.left = t.left - s.left + i), "using" in t ? t.using.call(e, f) : c.css(f)
+        }
+    }, S.fn.extend({
+        offset: function(t) {
+            if (arguments.length) return void 0 === t ? this : this.each(function(e) {
+                S.offset.setOffset(this, t, e)
             });
-            var b, c, d = this[0],
-                e = {
-                    top: 0,
-                    left: 0
-                },
-                f = d && d.ownerDocument;
-            if (f) return b = f.documentElement, o.contains(b, d) ? (typeof d.getBoundingClientRect !== U && (e = d.getBoundingClientRect()), c = Kc(f), {
-                top: e.top + c.pageYOffset - b.clientTop,
-                left: e.left + c.pageXOffset - b.clientLeft
-            }) : e
+            var e, n, r = this[0];
+            return r ? r.getClientRects().length ? (e = r.getBoundingClientRect(), n = r.ownerDocument.defaultView, {
+                top: e.top + n.pageYOffset,
+                left: e.left + n.pageXOffset
+            }) : {
+                top: 0,
+                left: 0
+            } : void 0
         },
         position: function() {
             if (this[0]) {
-                var a, b, c = this[0],
-                    d = {
+                var e, t, n, r = this[0],
+                    i = {
                         top: 0,
                         left: 0
                     };
-                return "fixed" === o.css(c, "position") ? b = c.getBoundingClientRect() : (a = this.offsetParent(), b = this.offset(), o.nodeName(a[0], "html") || (d = a.offset()), d.top += o.css(a[0], "borderTopWidth", !0), d.left += o.css(a[0], "borderLeftWidth", !0)), {
-                    top: b.top - d.top - o.css(c, "marginTop", !0),
-                    left: b.left - d.left - o.css(c, "marginLeft", !0)
+                if ("fixed" === S.css(r, "position")) t = r.getBoundingClientRect();
+                else {
+                    t = this.offset(), n = r.ownerDocument, e = r.offsetParent || n.documentElement;
+                    while (e && (e === n.body || e === n.documentElement) && "static" === S.css(e, "position")) e = e.parentNode;
+                    e && e !== r && 1 === e.nodeType && ((i = S(e).offset()).top += S.css(e, "borderTopWidth", !0), i.left += S.css(e, "borderLeftWidth", !0))
+                }
+                return {
+                    top: t.top - i.top - S.css(r, "marginTop", !0),
+                    left: t.left - i.left - S.css(r, "marginLeft", !0)
                 }
             }
         },
         offsetParent: function() {
             return this.map(function() {
-                var a = this.offsetParent || Jc;
-                while (a && !o.nodeName(a, "html") && "static" === o.css(a, "position")) a = a.offsetParent;
-                return a || Jc
+                var e = this.offsetParent;
+                while (e && "static" === S.css(e, "position")) e = e.offsetParent;
+                return e || re
             })
         }
-    }), o.each({
+    }), S.each({
         scrollLeft: "pageXOffset",
         scrollTop: "pageYOffset"
-    }, function(b, c) {
-        var d = "pageYOffset" === c;
-        o.fn[b] = function(e) {
-            return J(this, function(b, e, f) {
-                var g = Kc(b);
-                return void 0 === f ? g ? g[c] : b[e] : void(g ? g.scrollTo(d ? a.pageXOffset : f, d ? f : a.pageYOffset) : b[e] = f)
-            }, b, e, arguments.length, null)
-        }
-    }), o.each(["top", "left"], function(a, b) {
-        o.cssHooks[b] = yb(l.pixelPosition, function(a, c) {
-            return c ? (c = xb(a, b), vb.test(c) ? o(a).position()[b] + "px" : c) : void 0
+    }, function(t, i) {
+        var o = "pageYOffset" === i;
+        S.fn[t] = function(e) {
+            return B(this, function(e, t, n) {
+                var r;
+                if (x(e) ? r = e : 9 === e.nodeType && (r = e.defaultView), void 0 === n) return r ? r[i] : e[t];
+                r ? r.scrollTo(o ? r.pageXOffset : n, o ? n : r.pageYOffset) : e[t] = n
+            }, t, e, arguments.length)
+        }
+    }), S.each(["top", "left"], function(e, n) {
+        S.cssHooks[n] = _e(v.pixelPosition, function(e, t) {
+            if (t) return t = Be(e, n), Pe.test(t) ? S(e).position()[n] + "px" : t
         })
-    }), o.each({
+    }), S.each({
         Height: "height",
         Width: "width"
-    }, function(a, b) {
-        o.each({
+    }, function(a, s) {
+        S.each({
             padding: "inner" + a,
-            content: b,
+            content: s,
             "": "outer" + a
-        }, function(c, d) {
-            o.fn[d] = function(d, e) {
-                var f = arguments.length && (c || "boolean" != typeof d),
-                    g = c || (d === !0 || e === !0 ? "margin" : "border");
-                return J(this, function(b, c, d) {
-                    var e;
-                    return o.isWindow(b) ? b.document.documentElement["client" + a] : 9 === b.nodeType ? (e = b.documentElement, Math.max(b.body["scroll" + a], e["scroll" + a], b.body["offset" + a], e["offset" + a], e["client" + a])) : void 0 === d ? o.css(b, c, g) : o.style(b, c, d, g)
-                }, b, f ? d : void 0, f, null)
+        }, function(r, o) {
+            S.fn[o] = function(e, t) {
+                var n = arguments.length && (r || "boolean" != typeof e),
+                    i = r || (!0 === e || !0 === t ? "margin" : "border");
+                return B(this, function(e, t, n) {
+                    var r;
+                    return x(e) ? 0 === o.indexOf("outer") ? e["inner" + a] : e.document.documentElement["client" + a] : 9 === e.nodeType ? (r = e.documentElement, Math.max(e.body["scroll" + a], r["scroll" + a], e.body["offset" + a], r["offset" + a], r["client" + a])) : void 0 === n ? S.css(e, t, i) : S.style(e, t, n, i)
+                }, s, n ? e : void 0, n)
             }
         })
-    }), o.fn.size = function() {
-        return this.length
-    }, o.fn.andSelf = o.fn.addBack, "function" == typeof define && define.amd && define("jquery", [], function() {
-        return o
+    }), S.each(["ajaxStart", "ajaxStop", "ajaxComplete", "ajaxError", "ajaxSuccess", "ajaxSend"], function(e, t) {
+        S.fn[t] = function(e) {
+            return this.on(t, e)
+        }
+    }), S.fn.extend({
+        bind: function(e, t, n) {
+            return this.on(e, null, t, n)
+        },
+        unbind: function(e, t) {
+            return this.off(e, null, t)
+        },
+        delegate: function(e, t, n, r) {
+            return this.on(t, e, n, r)
+        },
+        undelegate: function(e, t, n) {
+            return 1 === arguments.length ? this.off(e, "**") : this.off(t, e || "**", n)
+        },
+        hover: function(e, t) {
+            return this.mouseenter(e).mouseleave(t || e)
+        }
+    }), S.each("blur focus focusin focusout resize scroll click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup contextmenu".split(" "), function(e, n) {
+        S.fn[n] = function(e, t) {
+            return 0 < arguments.length ? this.on(n, null, e, t) : this.trigger(n)
+        }
+    });
+    var Gt = /^[\s\uFEFF\xA0]+|([^\s\uFEFF\xA0])[\s\uFEFF\xA0]+$/g;
+    S.proxy = function(e, t) {
+        var n, r, i;
+        if ("string" == typeof t && (n = e[t], t = e, e = n), m(e)) return r = s.call(arguments, 2), (i = function() {
+            return e.apply(t || this, r.concat(s.call(arguments)))
+        }).guid = e.guid = e.guid || S.guid++, i
+    }, S.holdReady = function(e) {
+        e ? S.readyWait++ : S.ready(!0)
+    }, S.isArray = Array.isArray, S.parseJSON = JSON.parse, S.nodeName = A, S.isFunction = m, S.isWindow = x, S.camelCase = X, S.type = w, S.now = Date.now, S.isNumeric = function(e) {
+        var t = S.type(e);
+        return ("number" === t || "string" === t) && !isNaN(e - parseFloat(e))
+    }, S.trim = function(e) {
+        return null == e ? "" : (e + "").replace(Gt, "$1")
+    }, "function" == typeof define && define.amd && define("jquery", [], function() {
+        return S
     });
-    var Lc = a.jQuery,
-        Mc = a.$;
-    return o.noConflict = function(b) {
-        return a.$ === o && (a.$ = Mc), b && a.jQuery === o && (a.jQuery = Lc), o
-    }, typeof b === U && (a.jQuery = a.$ = o), o
+    var Yt = C.jQuery,
+        Qt = C.$;
+    return S.noConflict = function(e) {
+        return C.$ === S && (C.$ = Qt), e && C.jQuery === S && (C.jQuery = Yt), S
+    }, "undefined" == typeof e && (C.jQuery = C.$ = S), S
 });
```

### Comparing `django-gas-0.8.6/gas/static/vendor/jquery.formset.js` & `django-gas-0.8.7/gas/static/vendor/jquery.formset.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/.github/CONTRIBUTING.md` & `django-gas-0.8.7/gas/static/vendor/select2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/.github/ISSUE_TEMPLATE.md` & `django-gas-0.8.7/gas/static/vendor/select2/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/.github/stale.yml` & `django-gas-0.8.7/gas/static/vendor/select2/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/.github/workflows/docs-deploy.yml` & `django-gas-0.8.7/gas/static/vendor/select2/.github/workflows/docs-deploy.yml`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/.github/workflows/main.yml` & `django-gas-0.8.7/gas/static/vendor/select2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/.github/workflows/package-deploy.yml` & `django-gas-0.8.7/gas/static/vendor/select2/.github/workflows/package-deploy.yml`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/LICENSE.md` & `django-gas-0.8.7/gas/static/vendor/select2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/css/select2.css` & `django-gas-0.8.7/gas/static/vendor/select2/css/select2.css`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/css/select2.min.css` & `django-gas-0.8.7/gas/static/vendor/select2/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/af.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/af.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/ar.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/ar.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/az.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/az.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/bg.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/bg.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/bn.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/bn.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/bs.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/bs.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/ca.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/ca.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/cs.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/cs.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/da.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/da.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/de.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/de.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/dsb.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/dsb.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/el.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/el.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/en.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/en.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/es.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/es.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/et.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/et.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/eu.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/eu.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/fa.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/fa.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/fi.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/fi.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/fr.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/fr.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/gl.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/gl.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/he.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/he.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/hi.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/hi.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/hr.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/hr.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/hsb.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/hsb.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/hu.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/hu.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/hy.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/hy.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/id.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/id.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/is.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/is.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/it.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/it.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/ja.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/ja.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/ka.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/ka.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/km.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/km.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/ko.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/ko.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/lt.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/lt.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/lv.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/lv.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/mk.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/mk.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/ms.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/ms.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/nb.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/nb.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/ne.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/ne.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/nl.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/nl.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/pl.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/pl.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/ps.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/ps.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/pt-BR.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/pt.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/pt.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/ro.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/ro.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/ru.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/ru.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/sk.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/sk.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/sl.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/sl.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/sq.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/sq.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/sr-Cyrl.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/sr.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/sr.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/sv.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/sv.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/th.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/th.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/tk.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/tk.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/tr.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/tr.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/uk.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/uk.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/vi.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/vi.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/zh-CN.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/zh-CN.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/i18n/zh-TW.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/i18n/zh-TW.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/select2.full.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/select2.full.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/select2.full.min.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/select2.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/select2.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/static/vendor/select2/js/select2.min.js` & `django-gas-0.8.7/gas/static/vendor/select2/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/templates/gas/base.html` & `django-gas-0.8.7/gas/templates/gas/base.html`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/templates/gas/base_form.html` & `django-gas-0.8.7/gas/templates/gas/base_form.html`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/templates/gas/base_list.html` & `django-gas-0.8.7/gas/templates/gas/base_list.html`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/templates/gas/delete_confirmation.html` & `django-gas-0.8.7/gas/templates/gas/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/templates/gas/login.html` & `django-gas-0.8.7/gas/templates/gas/login.html`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/templates/gas/tags/forms/field.html` & `django-gas-0.8.7/gas/templates/gas/tags/forms/field.html`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/templates/gas/tags/navigation.html` & `django-gas-0.8.7/gas/templates/gas/tags/navigation.html`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/templates/gas/tags/pagination.html` & `django-gas-0.8.7/gas/templates/gas/tags/pagination.html`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/templates/gas/users/user_list.html` & `django-gas-0.8.7/gas/templates/gas/users/user_list.html`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/templatetags/form_tags.py` & `django-gas-0.8.7/gas/templatetags/form_tags.py`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/templatetags/gas_tags.py` & `django-gas-0.8.7/gas/templatetags/gas_tags.py`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/tests/test_core_views.py` & `django-gas-0.8.7/gas/tests/test_core_views.py`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/tests/test_site.py` & `django-gas-0.8.7/gas/tests/test_site.py`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/tests/test_user_forms.py` & `django-gas-0.8.7/gas/tests/test_user_forms.py`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/tests/test_utils.py` & `django-gas-0.8.7/gas/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/tests/test_views.py` & `django-gas-0.8.7/gas/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/utils.py` & `django-gas-0.8.7/gas/utils.py`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/gas/views.py` & `django-gas-0.8.7/gas/views.py`

 * *Files identical despite different names*

### Comparing `django-gas-0.8.6/setup.cfg` & `django-gas-0.8.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-gas
-version = 0.8.6
+version = 0.8.7
 description = An alternative to django admin
 long_description = file: readme.md, changelog.md, collaborators.md
 long_description_content_type = text/markdown
 url = https://git.negromate.rocks/shagi/gas
 author = Ales (Shagi) Zabala Alava
 author_email = shagi@gisa-elkartea.org
 license = GPLv3
```

