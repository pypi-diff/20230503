# Comparing `tmp/irails-1.1.1.tar.gz` & `tmp/irails-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.1.1.tar", last modified: Mon May  1 07:13:47 2023, max compression
+gzip compressed data, was "irails-1.1.2.tar", last modified: Wed May  3 14:54:30 2023, max compression
```

## Comparing `irails-1.1.1.tar` & `irails-1.1.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.186154 irails-1.1.1/
--rw-rw-rw-   0        0        0       39 2023-04-30 09:03:04.000000 irails-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6901 2023-05-01 07:13:47.185159 irails-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     6120 2023-05-01 07:13:46.000000 irails-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.131298 irails-1.1.1/irails/
--rw-rw-rw-   0        0        0      295 2023-04-24 10:22:01.000000 irails-1.1.1/irails/__init__.py
--rw-rw-rw-   0        0        0     1507 2023-04-30 11:36:07.000000 irails-1.1.1/irails/_loader.py
--rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.1.1/irails/_utils.py
--rw-rw-rw-   0        0        0    11003 2023-04-30 14:40:36.000000 irails-1.1.1/irails/auth.py
--rw-rw-rw-   0        0        0    10558 2023-05-01 06:23:44.000000 irails-1.1.1/irails/base_controller.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.1.1/irails/cbv.py
--rw-rw-rw-   0        0        0     6367 2023-05-01 04:02:40.000000 irails-1.1.1/irails/config.py
--rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.1.1/irails/controller.py
--rw-rw-rw-   0        0        0    12619 2023-04-27 14:24:00.000000 irails-1.1.1/irails/controller_utils.py
--rw-rw-rw-   0        0        0    14294 2023-05-01 04:41:56.000000 irails-1.1.1/irails/core.py
--rw-rw-rw-   0        0        0     6110 2023-04-30 14:34:13.000000 irails-1.1.1/irails/database.py
--rw-rw-rw-   0        0        0     7943 2023-05-01 07:11:01.000000 irails-1.1.1/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.1.1/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.1.1/irails/midware_session.py
-drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.145260 irails-1.1.1/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.1.1/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     8345 2023-04-30 09:03:04.000000 irails-1.1.1/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     6545 2023-04-30 09:03:04.000000 irails-1.1.1/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     2283 2023-04-30 09:03:04.000000 irails-1.1.1/irails/scripts/_project.py
--rw-rw-rw-   0        0        0      591 2023-04-30 09:03:04.000000 irails-1.1.1/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     1535 2023-04-30 09:03:04.000000 irails-1.1.1/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.105585 irails-1.1.1/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.155233 irails-1.1.1/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0     1517 2023-04-30 09:03:04.000000 irails-1.1.1/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.1.1/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.1.1/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1263 2023-04-25 10:41:46.000000 irails-1.1.1/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.1.1/irails/scripts/tpls/app/model.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.1.1/irails/scripts/tpls/app/service.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.1.1/irails/scripts/tpls/app/test.tpl
--rw-rw-rw-   0        0        0       19 2023-04-28 05:57:01.000000 irails-1.1.1/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.157229 irails-1.1.1/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.1.1/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.158225 irails-1.1.1/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.1.1/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.167203 irails-1.1.1/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-04-18 14:10:48.000000 irails-1.1.1/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.1.1/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      342 2023-04-22 11:06:16.000000 irails-1.1.1/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      300 2023-04-03 07:47:20.000000 irails-1.1.1/irails/scripts/tpls/project/configs/casbin-model.conf
--rw-rw-rw-   0        0        0      839 2023-04-19 05:59:11.000000 irails-1.1.1/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      831 2023-04-26 09:58:29.000000 irails-1.1.1/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.1.1/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      144 2023-04-30 09:03:04.000000 irails-1.1.1/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.172187 irails-1.1.1/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1234 2023-04-07 11:12:30.000000 irails-1.1.1/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1056 2023-04-07 11:24:23.000000 irails-1.1.1/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.174184 irails-1.1.1/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.110572 irails-1.1.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.177182 irails-1.1.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.1.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.180168 irails-1.1.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.1.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.1.1/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.1.1/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.110572 irails-1.1.1/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.182162 irails-1.1.1/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.1.1/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     2073 2023-05-01 07:10:19.000000 irails-1.1.1/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-01 07:13:47.139277 irails-1.1.1/irails.egg-info/
--rw-rw-rw-   0        0        0     6901 2023-05-01 07:13:46.000000 irails-1.1.1/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1878 2023-05-01 07:13:47.000000 irails-1.1.1/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 07:13:46.000000 irails-1.1.1/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-01 07:13:46.000000 irails-1.1.1/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      767 2023-05-01 07:13:46.000000 irails-1.1.1/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-01 07:13:46.000000 irails-1.1.1/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 07:13:47.187148 irails-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2921 2023-05-01 07:13:37.000000 irails-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.545630 irails-1.1.2/
+-rw-rw-rw-   0        0        0       39 2023-04-30 09:03:04.000000 irails-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6937 2023-05-03 14:54:30.543624 irails-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6156 2023-05-03 14:54:30.000000 irails-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.461842 irails-1.1.2/irails/
+-rw-rw-rw-   0        0        0      318 2023-05-03 14:19:47.000000 irails-1.1.2/irails/__init__.py
+-rw-rw-rw-   0        0        0     1682 2023-05-02 08:43:36.000000 irails-1.1.2/irails/_loader.py
+-rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.1.2/irails/_utils.py
+-rw-rw-rw-   0        0        0    11616 2023-05-02 08:29:17.000000 irails-1.1.2/irails/auth.py
+-rw-rw-rw-   0        0        0    10573 2023-05-02 06:49:08.000000 irails-1.1.2/irails/base_controller.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.1.2/irails/cbv.py
+-rw-rw-rw-   0        0        0     6464 2023-05-03 14:45:48.000000 irails-1.1.2/irails/config.py
+-rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.1.2/irails/controller.py
+-rw-rw-rw-   0        0        0    12261 2023-05-03 14:53:53.000000 irails-1.1.2/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    14411 2023-05-03 14:49:52.000000 irails-1.1.2/irails/core.py
+-rw-rw-rw-   0        0        0     6110 2023-04-30 14:34:13.000000 irails-1.1.2/irails/database.py
+-rw-rw-rw-   0        0        0     7943 2023-05-01 07:11:01.000000 irails-1.1.2/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.1.2/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.1.2/irails/midware_session.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.483783 irails-1.1.2/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.1.2/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7692 2023-05-03 14:35:44.000000 irails-1.1.2/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     7133 2023-05-03 07:16:46.000000 irails-1.1.2/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.1.2/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0      591 2023-04-30 09:03:04.000000 irails-1.1.2/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     1702 2023-05-03 14:31:14.000000 irails-1.1.2/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.418322 irails-1.1.2/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.497745 irails-1.1.2/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0     1517 2023-04-30 09:03:04.000000 irails-1.1.2/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.1.2/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.1.2/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1258 2023-05-02 08:55:43.000000 irails-1.1.2/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.1.2/irails/scripts/tpls/app/model.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.1.2/irails/scripts/tpls/app/service.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.1.2/irails/scripts/tpls/app/test.tpl
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.1.2/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.500739 irails-1.1.2/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.1.2/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.503730 irails-1.1.2/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.1.2/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.517693 irails-1.1.2/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-04-18 14:10:48.000000 irails-1.1.2/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.1.2/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      342 2023-04-22 11:06:16.000000 irails-1.1.2/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      300 2023-04-03 07:47:20.000000 irails-1.1.2/irails/scripts/tpls/project/configs/casbin-model.conf
+-rw-rw-rw-   0        0        0      839 2023-04-19 05:59:11.000000 irails-1.1.2/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0     1074 2023-05-02 08:48:52.000000 irails-1.1.2/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.1.2/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      144 2023-04-30 09:03:04.000000 irails-1.1.2/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.522679 irails-1.1.2/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.1.2/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.1.2/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.525671 irails-1.1.2/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.425304 irails-1.1.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.531655 irails-1.1.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.1.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.537639 irails-1.1.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.1.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.1.2/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.1.2/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.427299 irails-1.1.2/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.540631 irails-1.1.2/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.1.2/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     2094 2023-05-01 09:15:49.000000 irails-1.1.2/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:54:30.473811 irails-1.1.2/irails.egg-info/
+-rw-rw-rw-   0        0        0     6937 2023-05-03 14:54:30.000000 irails-1.1.2/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1878 2023-05-03 14:54:30.000000 irails-1.1.2/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 14:54:30.000000 irails-1.1.2/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-03 14:54:30.000000 irails-1.1.2/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      767 2023-05-03 14:54:30.000000 irails-1.1.2/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-03 14:54:30.000000 irails-1.1.2/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 14:54:30.546615 irails-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2955 2023-05-03 14:33:36.000000 irails-1.1.2/setup.py
```

### Comparing `irails-1.1.1/PKG-INFO` & `irails-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.1.1
+Version: 1.1.2
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
@@ -69,15 +69,15 @@
 controller:
 ```python
 
 from irails import api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect,UploadFile,File
 
 from typing import Any, Dict ,List
 from pydantic import conlist
-
+from app.services import UserService
 application._public_auth_url = '/user/login'
 application._user_auth_url = '/user/login'
  
 @api_router(auth='public')
 class TestController(BaseController): 
     @api.get("/user/login" )
     def login(self):
```

### Comparing `irails-1.1.1/README.md` & `irails-1.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 controller:
 ```python
 
 from irails import api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect,UploadFile,File
 
 from typing import Any, Dict ,List
 from pydantic import conlist
-
+from app.services import UserService
 application._public_auth_url = '/user/login'
 application._user_auth_url = '/user/login'
  
 @api_router(auth='public')
 class TestController(BaseController): 
     @api.get("/user/login" )
     def login(self):
```

### Comparing `irails-1.1.1/irails/_loader.py` & `irails-1.1.2/irails/_loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .config import config,ROOT_PATH,_log
 app_cfg=config.get('app')
 app_dirs = app_cfg.get("appdir")
 app_enabled = app_cfg.get("enabled")
 
 def __list_directories(dir):
     """
-    遍历目录，返回所有子目录的路径
+    return all subdirectory under :dir
     """
     dirs_list = [] 
     for name in os.listdir(dir):
        
         path = os.path.join(dir,name)
         if os.path.isdir(path) and name!='__pycache__': 
             dirs_list.append(name)
@@ -27,23 +27,27 @@
         spec = importlib.util.spec_from_file_location(module_name, module_path)
         module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(module)
         return module
     return None
 
 def _load_apps(debug=False):
-    sys.path.insert(-1,ROOT_PATH)
+    if ROOT_PATH not in sys.path:
+        sys.path.insert(-1,ROOT_PATH)
     unloaded = 0
     loaded = 0
     for app_dir in app_dirs:
         app_list =  __list_directories(app_dir)
         for app in app_list:
             if __check_if_enabled(app): 
                 if debug:
                     _log.info(f'Loading {app_dir}.{app}')
+                _path = os.path.join(ROOT_PATH,app_dir)
+                if _path not in sys.path:
+                    sys.path.insert(-1,_path)
                 __import__(f'{app_dir}.{app}')
                 loaded = loaded + 1
             else:
                 unloaded = unloaded + 1
         
     
     return loaded,unloaded
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `irails-1.1.1/irails/_utils.py` & `irails-1.1.2/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.1/irails/auth.py` & `irails-1.1.2/irails/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,30 @@
     pass
 class CasbinAuth:
     def __init__(self,enforcer:Enforcer,session_name="user") -> None:
         global _session_name
         self.enforcer = enforcer
         self.__session_name = _session_name = session_name
         pass
+    def modify_authorization(self,sub,obj,act,authorize:bool):
+        """
+        :sub(user_name or mainbody),:obj(resource or url),:act(action like 'GET','POST','DELETE')
+        add or remove authorization info by :authorzie
+        """
+        if self.enforcer:
+            if authorize:
+                return self.enforcer.add_policy(sub,obj,act)
+            else:
+                return self.enforcer.remove_policy(sub,obj,act)
+        raise RuntimeError("Casbin Enforcer is None")
+    
     def _auth(self,request:Request,username:str):
+        '''
+        do verity,return True means `Success` and others `Failed`
+        '''
         path = request.url.path
         method = request.method   
         if username:
             user = username
         else:
             user = request.user.display_name if request.user.is_authenticated else 'anonymous'
 
@@ -64,15 +79,15 @@
                 scheme, credentials = auth.split() 
                 token = self.__get_token_from_header(authorization=auth, prefix=prefix)
                 
                 del kwargs['username_field']
                 try:
                     payload = jwt.decode(token,**kwargs)
                 except jwt.InvalidTokenError as e:
-                    _log.debug('token:'+token + ' has been expired.')
+                    _log.debug('token:'+token + f' has been expired.{e.args}')
                     request.session[self.__session_name] = None
                     return "","",None
                 if is_datetime_format(payload['exp']):
                     payload['exp'] = datetime.fromisoformat(payload['exp'])
 
 
                 return  payload[username_field],token,payload
@@ -229,14 +244,15 @@
     global _casbin_auth
     cfg = config.get("auth")
     adapter_uri = kwagrs.get('adapter_uri',None)
     del kwagrs['adapter_uri']
     model_file = cfg.get("auth_model",'./configs/casbin-model.conf')    
     adapter = adapter_class(adapter_uri)
     enforcer = casbin.Enforcer(model_file, adapter)
+   
     _casbin_auth = CasbinAuth(enforcer=enforcer,session_name=__session_name)
     
     return backend(**kwagrs) 
 def reload_adapter(app:FastAPI,adapter:Adapter=None):
     cfg = config.get("auth")
     model_file = cfg.get("auth_model",'./configs/casbin-model.conf')    
     if not adapter:
```

### Comparing `irails-1.1.1/irails/base_controller.py` & `irails-1.1.2/irails/base_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 from logging import Logger
 import inspect
 import datetime
 
  
 __session_config = config.get('session') 
 _session_key = "session_id"
+alow_extensions = []
+MAX_UPLOAD_LEN = -1
+MAX_FILES = 1
 if __session_config:
     _session_key = __session_config.get("key","session_id")
 __upload_cfg=config.get("upload")
 if __upload_cfg:
     __max_upload = __upload_cfg.get('max')
     __max_files = __upload_cfg.get('count')
     updir = __upload_cfg['dir'] or "uploads"
@@ -78,22 +81,22 @@
     @classmethod
     def redirect(self,url ,statu_code=StateCodes.HTTP_303_SEE_OTHER):
         """
         return RedirectResponse to the special URL   
         """
         return RedirectResponse(url,status_code=statu_code)
     
-    def _verity_successed(self,user,redirect,msg="User authentication successed!"):
+    def _verity_successed(self,user,msg="User authentication successed!",redirect='/'):
         """
         return Response for Verity successed information
         if redirect is provide,then redirect to the redirect URL
         """
         pass
         
-    def _user_logout(self,msg="You are successed logout!"):
+    def _user_logout(self,msg="You are successed logout!",redirect='/'):
         """return Response for logout to root('/')"""
         pass
 
     def _verity_error(self,msg="User authentication failed!"):
         """return Response for show Verity failed infomation"""
         pass
      
@@ -114,23 +117,22 @@
                     pairs.append(kws['app'].strip())
                 if 'controller' in kws  and kws['controller'].strip():
                     pairs.append(kws['controller'].strip())
                 if 'version' in kws  and kws['version'].strip():
                     pairs.append(kws['version'].strip())
                 if 'action' in kws  and kws['action'].strip():
                     pairs.append(kws['action'].strip())
-                elif url :
-                    pairs.append(url)
+                 
                 url_path = "/"+"/".join(pairs)
                  
             else: 
                 url_path = self.__template_path__.replace('{controller}',self.__controller_name__).replace("{version}",self.__version__)
-                url_path = url_path + "/" + url.strip()
+                 
         
-            return url_path  
+            return url_path.lower() + "/" + url.strip()
             
         if content:
             if format=='html':
                 return HTMLResponse(content,**kwargs)
             elif format=='text':
                 return PlainTextResponse(content,**kwargs)
             else:
```

### Comparing `irails-1.1.1/irails/cbv.py` & `irails-1.1.2/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.1/irails/config.py` & `irails-1.1.2/irails/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 import os,sys
 import yaml
 import logging
 from hashlib import md5
 from typing import Dict
 import os.path
-
-# from fastapi.logger import logger
-
 import re
- 
 
 def is_in_irails(directory):
     """
     check exists configs dir,   main.py and configs/general.yaml 
     """
     
     configs_dir = os.path.join(directory, 'configs')
@@ -28,15 +24,15 @@
     return True
 ROOT_PATH = os.path.realpath(os.curdir)
  
 IS_IN_irails = is_in_irails(ROOT_PATH)
 def is_cli_mode():
     executeble = sys.argv[0]
     executeble = os.path.basename(executeble)
-    print(f"current executeble:" + executeble)
+    # print(f"current executeble:" + executeble)
     return (executeble.lower().startswith('irails'))
 
 def _extract_name(string):
     match = re.search(r'{([^}]*)}', string)
     if match:
         return match.group(1)
     else:
@@ -46,14 +42,18 @@
     _raw_config = {}
     def __init__(self, filename:str="",config:Dict={}):
         self.filename = filename
         self.config = config
         self.load()
     def __getitem__(self,key):
         return self.get(key)
+    def __setitem__(self,key,value):
+        self.set(key,value)
+    def reload(self):
+        return self.load()
     def load(self):
         if os.path.isfile(self.filename):
             with open(self.filename, "r") as f:
                 self.config = yaml.safe_load(f)
                 YamlConfig._raw_config = self.config
 
         elif os.path.isdir(self.filename):
@@ -63,14 +63,15 @@
             return True
         else:
             if is_cli_mode():
                 pass
             else:
                 raise Exception(f"{self.filename} is not a file or directory")
             return False
+        return True
     def dump(self):
         return yaml.safe_dump(self.config) if self.config else ""
     def save(self):
         if not self.filename:
             return False
         with open(self.filename, "w") as f:
             yaml.safe_dump(self.config, f)
```

### Comparing `irails-1.1.1/irails/controller.py` & `irails-1.1.2/irails/controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.1/irails/controller_utils.py` & `irails-1.1.2/irails/controller_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,29 +278,21 @@
                 route_method = getattr(router, value[METHOD_KEY]) 
                 # 添加到 fastapi apiroute
                 new_route_method = route_method(path, **kwargs)(new_member)
         setattr(controller, name, new_route_method)
     
     cbv(router)(controller)
 
-def auth_error():
-    # 构建自定义的响应对象
-    # response_content =  "未经授权的访问" 
-    # response_headers = {"Content-Type": "application/json"}
-    # response_status_code = 403
-    # response = Response(content=response_content, headers=response_headers, status_code=response_status_code)
-    
-    # 抛出 403 错误，使用自定义的响应对象
-    raise HTTPException(status_code=403, detail="未经授权的访问" )
+ 
 
  
 
 def _route_method(path: str, method, *args, **mwargs): 
     if not path.startswith("/"):
-        raise "path must start with '/'"
+        raise RuntimeError("path must start with '/'")
     def wrapper(func ): 
         @wraps(func)
         async def decorator(  *args, **kwargs):
             auth_type:str = getattr(func,AUTH_KEY) 
             has_request = kwargs.get("__has_request__")
             has_response = kwargs.get("__has_response__")
             module = inspect.getmodule(func)
@@ -310,20 +302,21 @@
             response:Response = None
             result:Response = None
             
             if 'request' in kwargs and 'response' in kwargs:
                 response  = kwargs["response"]
                 rqst = kwargs['request']  
                 #auth first then call constructor
-                if auth_type and auth_type !="none"  :
+                if auth_type:
                     auth_result,user = await cls._auth__(request=rqst,response=kwargs['response'],auth_type=auth_type)
                     if isinstance(auth_result,Response): 
                         return auth_result
                     if not auth_result:
-                        auth_error()
+                        raise HTTPException(status_code=403, detail="未经授权的访问" )
+                        return Response(None,403)
                 _constructor = getattr(cls,'_constructor_')
                 await _constructor(cls,request = kwargs['request'],response=kwargs['response'])
 
             if 'request' in kwargs and not has_request:  
                 del kwargs['request']  
             if 'response' in kwargs and not has_response:  
                 del kwargs['response']
```

### Comparing `irails-1.1.1/irails/core.py` & `irails-1.1.2/irails/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,25 +132,25 @@
     def _wapper(targetController):  
         
         class puppetController( targetController ,_controllerBase ): 
             '''puppet class inherited by the User defined controller class '''
             def __init__(self,**kwags) -> None: 
                 
                 super().__init__()
-            def _user_logout(self,msg='your are successed logout!'):
+            def _user_logout(self,msg='your are successed logout!',redirect:str="/"):
                 """see .core.py"""
                 self.flash  = msg
                 if  hasattr(application,'authObj'):
                     application.authObj.clear_userinfo(request=self.request)
                 accept_header = self.request.headers.get("Accept")    
                 if accept_header == "application/json":
                     return {'status':'success','msg':msg}
                 else:
-                    return self.redirect('/')
-            def _verity_successed(self,user,redirect_url='/', msg="User authentication successed!"):
+                    return self.redirect(redirect)
+            def _verity_successed(self,user, msg="User authentication successed!",redirect_url='/'):
                 '''call by targetController''' 
                  
                 self.flash  = msg
                 accept_header = self._request.headers.get("Accept")
                 if  hasattr(application,'authObj'):
                     access_token = application.authObj.create_access_token(user,request=self.request)
                 
@@ -162,18 +162,19 @@
                         return {'status':'success','msg':msg }
                  
                 return RedirectResponse(redirect_url,status_code=StateCodes.HTTP_303_SEE_OTHER)
             def _verity_error(self,msg="User authentication failed!"):
                 '''call by targetController'''
                  
                 self.flash  = msg 
-                url =  self.request.headers.get("Referer") or '/'
+                
                 accept_header = self.request.headers.get("Accept")
                 if accept_header == "application/json":
                     return JSONResponse(content={'status':StateCodes.HTTP_200_OK,'msg':msg})
+                url =  self.request.headers.get("Referer") or '/'
                 return RedirectResponse(url,status_code=StateCodes.HTTP_303_SEE_OTHER),None
             
             @classmethod
             async def _auth__(cls,request:Request,response:Response,**kwargs):
                 '''called by .controller_util.py->route_method'''
                 auth_type = kwargs['auth_type'] 
                 
@@ -181,14 +182,16 @@
                     return True,None
                 
                 kwargs['session'] = request.session  
                 ret,user = await application.authObj.authenticate(request,**kwargs)
                 if user==auth.AUTH_EXPIRED:
                     request.session['flash']  = "your authencation has been expired!"  
                     user = False
+                if auth_type=='none':
+                    return True,user
                 def add_redirect_param(url: str, redirect_url: str) -> str:
                     if "?" in url:
                         return url + "&redirect=" + redirect_url
                     else:
                         return url + "?redirect=" + redirect_url
                 accept_header = request.headers.get("Accept")
                 if user: #continue singture
```

### Comparing `irails-1.1.1/irails/database.py` & `irails-1.1.2/irails/database.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.1/irails/midware.py` & `irails-1.1.2/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.1/irails/midware_casbin.py` & `irails-1.1.2/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.1/irails/midware_session.py` & `irails-1.1.2/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.1/irails/scripts/_app.py` & `irails-1.1.2/irails/scripts/_app.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,61 +11,68 @@
         pass
     def gen_common(self):
         '''#todo: check configs dir
                   check data dir
 
         '''
         pass
-    def gen_tpl(self,tpl_file,dest,context={}, use_micro=True,dir_only=True):
-        tpl_dir = os.path.dirname(__file__)+"/tpls/app"
-        tpl_file = os.path.join(tpl_dir,tpl_file)
-        dest = os.path.normpath(dest)
-        if not os.path.exists(tpl_file):
-            raise Exception(f"{tpl_file} does not exists!")
-        dir = os.path.normpath(os.path.dirname(dest))
-        if not os.path.exists(dir):
-            os.makedirs(dir,exist_ok=True)
-            print(f"create {dir}")
-        if not dir_only:
-            with open(tpl_file,'r') as f:
-                content = f.read()
-            dest_content = content
-            if use_micro:
-                template = Template(content)
-                dest_content = template.render(context)
-            
-            
-                with open(dest,'w') as f:
-                    f.write(dest_content)
-            print(f"create {dest}")
-        return True
+     
     def add_enabled_to_app(self,app_name):
         import yaml
         try:
             file = './configs/general.yaml'
  
             with open(file, "r") as f:
                 data = yaml.load(f, Loader=yaml.FullLoader)
  
             enabled = data['app']['enabled']
             if not enabled:
+                return True
                 enabled = [app_name]
             else:
-                enabled.append(app_name) 
+                if isinstance(enabled,list):
+                    enabled.append(app_name) 
             new_enabled = list(set(enabled))
 
             data['app']['enabled'] = new_enabled
             with open(file, "w") as f:
                 yaml.dump(data, f)
+            print(f"configs/general.yaml app.enabled has been added {app_name}!")
+            return True
         except Exception as e:
             print(f'an error raised {e.args}')
             print(f"now please open configs/general.yaml to modify app.enabled to add {app_name}!")
             return
-        print(f"configs/general.yaml app.enabled has been added {app_name}!")
-    
+        
+    def set_root_controller_to_config(self,app_dir,app_name):
+        import yaml
+        try:
+            file = './configs/general.yaml' 
+            with open(file, "r") as f:
+                data = yaml.load(f, Loader=yaml.FullLoader) 
+            app_cfg = data['app'] 
+            changed = False
+            if not 'root' in app_cfg:
+                data['app']['root']=f"{app_dir}.{app_name}" 
+                changed = True
+            else: 
+                if not app_cfg['root']:
+                    data['app']['root']=f"{app_dir}.{app_name}" 
+                    changed = True
+            if changed:
+                with open(file, "w") as f:
+                    yaml.dump(data, f)
+                print(f'set {app_dir}.{app_name} to root on configs/general.yaml.')
+
+            return changed
+        except Exception as e:
+            print(f'an error raised {e.args}')
+            print(f"now please open configs/general.yaml to modify app.root to add {app_dir}.{app_name}!")
+            return
+         
     def do_copy(self,tpl_file,dest_file,over_write=False):
         dest_file  = os.path.normpath(dest_file)
         if os.path.exists(dest_file) and not over_write:
             print(f'{dest_file} is exists,skip...')
             return True
         os.makedirs(os.path.dirname(dest_file),exist_ok=True)
         with open(tpl_file,'r') as f:
@@ -93,15 +100,15 @@
         dest_file = os.path.normpath(dest_file)
         if os.path.exists(dest_file):
             print(f'{dest_file} is exists,skip...')
             return True
         with open(dest_file,'w') as f:
             f.write("""
 # -*- coding: utf-8 -*- 
-from irails import api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect,UploadFile,File
+from irails import api_router,api,Request,Response,BaseController,application
 @api_router(auth='none')
 class HomeController(BaseController): 
     @api.get("/")
     def home(self): 
         '''
         :title Home
         '''
@@ -139,60 +146,48 @@
             if os.path.exists(store_dir):
                 if os.path.isdir(store_dir):
                     if bool(os.listdir(store_dir)):
                         print(f"directory {store_dir} is exists and is not empty!")
                         exit()
             
             
-            dirs_items =  {
-                'controllers':{'tpl':'controller.tpl','dest':f'{app_name}_controller.py','micro':True} , 
-                'models': {'tpl':'model.tpl','dest' : f'{app_name}_model.py','micro':True},
-                'services':{'tpl':'service.tpl','dest': f'{app_name}_service.py','micro':True },
-                'views': [
-                    {'tpl' : 'view.tpl','dest': f'{app_name}/home.html','micro':False},
-                    {'tpl' : 'home.css.tpl','dest': f'{app_name}/home.css','micro':False}
-                    ] ,
-                
-                'tests': {'tpl':'test.tpl','dest': f'test_{app_name}.py','micro':True}
-            }
+            dirs_items =  [
+                'controllers',
+                'models',
+                'services',
+                'views',
+                'tests'
+            ]
             context = {'app':app_name}
             for dir in dirs_items:
                 _current_dir = os.path.join(store_dir,dir)
                 os.makedirs(_current_dir,exist_ok=True)
-                items = dirs_items[dir]
-                if isinstance(items,list):
-                    _item = items
-                else:
-                    _item = [items]
-                for item in _item:
-                    tpl = item['tpl']
-                    dest = os.path.join(_current_dir , item['dest'])
-                    micro = item['micro']
-                    self.gen_tpl(tpl_file=tpl,dest=dest,context=context,use_micro=micro) 
+                 
             _init_file = os.path.normpath(os.path.join(store_dir,'__init__.py'))
             with open(_init_file,'w') as f: #root path of app's dir
                 f.write(f"from .controllers import *")
             
             print(f"create {_init_file}")
 
             self.add_enabled_to_app(app_name)
-            self.add_home_controller(self.args.dir,app_name)
-            self.add_home_view(self.args.dir,app_name)
+            if self.set_root_controller_to_config(self.args.dir,app_name):
+                self.add_home_controller(self.args.dir,app_name)
+                self.add_home_view(self.args.dir,app_name)
             cnt += 1
         if cnt:
-            print(f"now ,you can cd to {self.args.dir}/{app_name} and run `irails controller controller's name` to create controllers")
+            print(f"now ,you can cd to {self.args.dir}/{app_name} and run `irails controller \"controller's name`\" to create controllers")
             print(f"now ,you can also run `burcelee run` to run project")
         print(f"Done! created {cnt} app[s]")
     pass
 
 def main():
     if not IS_IN_irails:
         print(f"Please exec in irails project dir")
         exit()
-    self_file = __file__.lstrip("_").replace(".py",'')
+    self_file = os.path.basename(__file__).lstrip("_").replace(".py",'')
     parser = argparse.ArgumentParser(usage=f"{sys.argv[0]} {self_file} [-h]  [-d DIR] [--name NAME] `app` ...", description='new app')
     parser.add_argument('--name',help="name to create app")
     parser.add_argument('-d','--dir',help="dir to store app files")
     parser.add_argument('args', nargs=argparse.REMAINDER)
 
     args = parser.parse_args()
     if not any(args.__dict__.values()):
```

### Comparing `irails-1.1.1/irails/scripts/_controller.py` & `irails-1.1.2/irails/scripts/_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,18 @@
                 lines = file.readlines()
 
                 # Check if the line is already in the file
                 for line in lines:
                     if line.strip() == line_to_add.strip():
                         found = True
                         break
-
+        else:
+            with open(filepath,'w') as file:
+                file.write(line_to_add)
+            return True              
         # If the line is not in the file, add it
         if not found:
             lines.append('\n' + line_to_add.strip() + '\n')
             with open(filepath, 'w') as file:
                 file.writelines(lines)
 
     def __call__(self) -> Any:
@@ -115,33 +118,42 @@
                 else:
                     _item = [items]
                 for item in _item:
                     tpl = item['tpl']
                     dest = os.path.join(_current_dir , item['dest'])
                     micro = item['micro']
                     self.gen_tpl(tpl_file=tpl,dest=dest,context=context,use_micro=micro,dir_only=False) 
+
             __init_file = os.path.join(_current_dir,'controllers','__init__.py')
             self.ensure_line(__init_file,f"from . import {controler_path_name}_controller")
+            __init_file = os.path.join(_current_dir,'models','__init__.py')
+            self.ensure_line(__init_file,f"from . import {controler_path_name}_model")
+            __init_file = os.path.join(_current_dir,'services','__init__.py')
+            self.ensure_line(__init_file,f"from . import {controler_path_name}_service")
              
         
         print("Done!")
     pass
 
 def is_in_app(directory):
     """
-    check exists configs dir, apps dir, main.py and configs/general.yaml 
+    check exists controllers , views dir in :directory
     """
     
     controller_dir = os.path.join(directory, 'controllers')
     views_dir = os.path.join(directory, 'views')  
-    if not os.path.exists(controller_dir) or not os.path.exists(views_dir) :
+    if not os.path.exists(controller_dir):
+        print(f"can't location `controller` dir")
         return False  
-    initfile = os.path.join(controller_dir, '__init__.py') 
-    if not os.path.exists(initfile):
+    if  not os.path.exists(views_dir) :
+        print(f"can't location `views` dir")
         return False
+    # initfile = os.path.join(controller_dir, '__init__.py') 
+    # if not os.path.exists(initfile):
+    #     return False
     
     return True
 def main():
      
     cur_dir = os.path.abspath(os.curdir)
     root_path = os.path.abspath(os.path.join(cur_dir,"../.."))
     if os.path.exists(root_path) and  os.path.isdir(root_path):
```

### Comparing `irails-1.1.1/irails/scripts/_project.py` & `irails-1.1.2/irails/scripts/_project.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,15 +43,15 @@
                 print("Done!")
         except Exception as e:
             print("Error!")
             print(e.args)
             exit()
 
 def main():
-    self_file = __file__.lstrip("_").replace(".py",'')
+    self_file = os.path.basename(__file__).lstrip("_").replace(".py",'')
     parser = argparse.ArgumentParser(usage=f"{sys.argv[0]} {self_file} [-h] [-d DIR]", description='new app') 
     parser.add_argument('-d','--dir',help="dir to store project files")
     parser.add_argument('args', nargs=argparse.REMAINDER)
     args = parser.parse_args()
     if not any(args.__dict__.values()):
         parser.print_help()
         exit()
```

### Comparing `irails-1.1.1/irails/scripts/_run.py` & `irails-1.1.2/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.1/irails/scripts/main.py` & `irails-1.1.2/irails/scripts/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import sys
 import importlib.util
 import os.path
  
 import os
 import re
- 
+from irails import __version__
 def collect_features():
     """
     return files in current dir start with '_' no sub dir
     """
     
     dir_path = os.path.dirname(os.path.abspath(__file__))  
     py_files = []
@@ -18,25 +18,27 @@
             py_files.append(os.path.splitext(file)[0].lstrip('_')) 
     return py_files 
 
 module_dir = os.path.dirname(__file__)
 avalible_features = collect_features()
 
 def main():
-
+    
     parser = argparse.ArgumentParser(description='generator for irails')
-    parser.add_argument('feature',choices=avalible_features, help='feature to run') 
+    parser.add_argument('feature', choices=avalible_features, nargs='?', help='feature to run')
+    parser.add_argument('--version', action='version', version=__version__, help='show the version of the program')
     parser.add_argument('args', nargs=argparse.REMAINDER)
 
     if not avalible_features:
         print(f"no feature on current dir")
         exit()
      
     args = parser.parse_args()
     
+    
     args.feature = '_' +args.feature
     
     module_path = os.path.join(module_dir, args.feature + '.py')
     if sys.argv[0]!='irails':
         sys.argv[0] = 'irails'
     if os.path.exists(module_path):
         spec = importlib.util.spec_from_file_location(args.feature, module_path)
```

### Comparing `irails-1.1.1/irails/scripts/tpls/app/controller.tpl` & `irails-1.1.2/irails/scripts/tpls/app/controller.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.1.1/irails/scripts/tpls/app/home.css.tpl` & `irails-1.1.2/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.1.1/irails/scripts/tpls/app/home.tpl` & `irails-1.1.2/irails/scripts/tpls/app/home.tpl`

 * *Files 9% similar despite different names*

```diff
@@ -12,27 +12,27 @@
     <header style="text-align:left;display: flex;">
         <h1>Python</h1>
         <h4>on FastApi</h4>
 
     </header>
     <nav>
         {% for item in routers_map %} {% if 'GET' in routers_map[item]['methods'] %} {% if routers_map[item]['auth']=='none' or request.session['user'] %}
-        <a href="{{routers_map[item]['path']}}">{{routers_map[item]['doc']
-                and routers_map[item]['doc']['title'] or item}}</a> {% endif %} {% endif %} {% endfor %}
+        <a href="${routers_map[item]['path']}">${routers_map[item]['doc']
+                and routers_map[item]['doc']['title'] or item}</a> {% endif %} {% endif %} {% endfor %}
 
         <a href="#">About</a>
         <a href="#">Contact</a> {% if request.session['user'] %}
-        <a href="/user/logout"><b>{{request.session['user']['username']}}</b>
+        <a href="/user/logout"><b>${request.session['user']['username']}</b>
                 Logout</a> {% endif %}
     </nav>
     <section>
         <h2>Welcome to my website</h2>
         <p>This is an example of a responsive design that works well on both desktop and mobile devices.</p>
-        <p>here is the `text` variable in class method:{{text}}</p>
-        <p style="color:red"><b>{{flash}}</b></p>
+        <p>here is the `text` variable in class method:${text}</p>
+        <p style="color:red"><b>${flash}</b></p>
     </section>
     <footer>
         <p>&copy; 2023 My Website</p>
     </footer>
 </body>
 
 </html>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 ****** Python ******
 *** on FastApi ***
   {% for item in routers_map %} {% if 'GET' in routers_map[item]['methods'] %}
-{% if routers_map[item]['auth']=='none' or request.session['user'] %} {
-{routers_map[item]['doc']_and_routers_map[item]['doc']['title']_or_item}} {%
+{% if routers_map[item]['auth']=='none' or request.session['user'] %} $
+{routers_map[item]['doc']_and_routers_map[item]['doc']['title']_or_item} {%
 endif %} {% endif %} {% endfor %} About Contact {% if request.session['user']
-%} {{request.session['user']['username']}}_Logout {% endif %}
+%} ${request.session['user']['username']}_Logout {% endif %}
 ***** Welcome to my website *****
 This is an example of a responsive design that works well on both desktop and
 mobile devices.
-here is the `text` variable in class method:{{text}}
-{{flash}}
+here is the `text` variable in class method:${text}
+${flash}
 
 © 2023 My Website
```

### Comparing `irails-1.1.1/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.1.2/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.1.1/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.1.2/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.1.1/irails/scripts/tpls/project/public/error_404.html` & `irails-1.1.2/irails/scripts/tpls/project/public/error_404.html`

 * *Files 8% similar despite different names*

```diff
@@ -44,12 +44,12 @@
 </head>
 
 <body>
     <div class="container">
         <h1>Page Not Found</h1>
         <p>We're sorry, but the page you requested could not be found.</p>
         <p>Please check the URL and try again, or return to the <a href="/">homepage</a>.</p>
-        <p>{{error.detail}}.</p>
+        <p>${error.detail}.</p>
     </div>
 </body>
 
 </html>
```

#### html2text {}

```diff
@@ -1,4 +1,4 @@
 ****** Page Not Found ******
 We're sorry, but the page you requested could not be found.
 Please check the URL and try again, or return to the homepage.
-{{error.detail}}.
+${error.detail}.
```

### Comparing `irails-1.1.1/irails/scripts/tpls/project/public/error_500.html` & `irails-1.1.2/irails/scripts/tpls/project/public/error_500.html`

 * *Files 11% similar despite different names*

```diff
@@ -32,11 +32,11 @@
     </style>
 </head>
 
 <body>
     <h1>500 Internal Server Error</h1>
     <p>Oops! Something went wrong. Our server is currently unable to handle your request. Please try again later.</p>
     <p>If you need further assistance, please contact our support team at <a href="mailto:support@yourwebsite.com">support@yourwebsite.com</a>.</p>
-
+    <p>${error.detail}.</p>
 </body>
 
 </html>
```

#### html2text {}

```diff
@@ -1,5 +1,6 @@
 ****** 500 Internal Server Error ******
 Oops! Something went wrong. Our server is currently unable to handle your
 request. Please try again later.
 If you need further assistance, please contact our support team at
 support@yourwebsite.com.
+${error.detail}.
```

### Comparing `irails-1.1.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.1.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.1/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.1.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.1.1/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.1.2/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.1/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.1.2/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.1/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.1.2/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.1/irails/view.py` & `irails-1.1.2/irails/view.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from typing import Any, Mapping
 from fastapi import BackgroundTasks, Request,Response
 from fastapi.templating import Jinja2Templates
 from fastapi.exceptions import HTTPException
-import jinja2 
  
-from .config import ROOT_PATH,config
+ 
+from .config import ROOT_PATH,config,_log
 
 env_configs = {} 
 static_format = []
 def __get_view_configure():
     global static_format,env_configs
     env_options = config.get("view")# {'variable_start_string':'${','variable_end_string':'}'}
     if env_options:
@@ -51,12 +51,13 @@
         if not view_path.endswith(".html"):
             view_path = f"{view_path}.html"
 
         context["request"] = request
         try:
             res = self._templates.TemplateResponse(view_path, context,**kwargs)
             return res
-        except jinja2.exceptions.TemplateNotFound:
+        except Exception as e:
+            _log.error("template not found"+e.args)
             view_path = os.path.join(self.views_directory,view_path).replace(ROOT_PATH,"").replace("\\","/")
-            raise HTTPException(500,f"template not found ![{view_path}]")
+            raise HTTPException(500,f"template not found ![{e.args}]")
```

### Comparing `irails-1.1.1/irails.egg-info/PKG-INFO` & `irails-1.1.2/irails.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.1.1
+Version: 1.1.2
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
@@ -69,15 +69,15 @@
 controller:
 ```python
 
 from irails import api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect,UploadFile,File
 
 from typing import Any, Dict ,List
 from pydantic import conlist
-
+from app.services import UserService
 application._public_auth_url = '/user/login'
 application._user_auth_url = '/user/login'
  
 @api_router(auth='public')
 class TestController(BaseController): 
     @api.get("/user/login" )
     def login(self):
```

### Comparing `irails-1.1.1/irails.egg-info/SOURCES.txt` & `irails-1.1.2/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.1.1/irails.egg-info/requires.txt` & `irails-1.1.2/irails.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `irails-1.1.1/setup.py` & `irails-1.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup,find_packages
 import chardet
-
-version = "1.1.1"
+from irails import __version__
+version = __version__
 def update_readme(source,spec,content=""):
     assert source or content
 
     if not content:
         with open(source, 'r') as file:
             content = file.read()
     with open('README.md', 'r') as file:
```

