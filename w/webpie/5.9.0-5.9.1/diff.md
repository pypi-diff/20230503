# Comparing `tmp/webpie-5.9.0.tar.gz` & `tmp/webpie-5.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/webpie-5.9.0.tar", last modified: Tue Oct 11 12:16:44 2022, max compression
+gzip compressed data, was "dist/webpie-5.9.1.tar", last modified: Wed Oct 12 14:14:12 2022, max compression
```

## Comparing `webpie-5.9.0.tar` & `webpie-5.9.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-10-11 12:16:44.000000 webpie-5.9.0/
--rw-r--r--   0 ivm        (503) staff       (20)    25245 2022-10-11 12:16:44.000000 webpie-5.9.0/PKG-INFO
--rwxr-xr-x   0 ivm        (503) staff       (20)    19894 2022-06-04 12:29:34.000000 webpie-5.9.0/README.rst
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-10-11 12:16:44.000000 webpie-5.9.0/multiserver/
--rwxr-xr-x   0 ivm        (503) staff       (20)    20762 2022-10-09 12:57:22.000000 webpie-5.9.0/multiserver/multiserver.py
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-10-11 12:16:44.000000 webpie-5.9.0/router/
--rwxr-xr-x   0 ivm        (503) staff       (20)     7278 2021-11-11 19:43:18.000000 webpie-5.9.0/router/router.py
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-10-11 12:16:44.000000 webpie-5.9.0/samples/
--rwxr-xr-x   0 ivm        (503) staff       (20)      793 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/callable_handler.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      344 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/clock.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     1037 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/date_time_simple.py
--rw-r--r--   0 ivm        (503) staff       (20)     3668 2022-06-04 14:27:36.000000 webpie-5.9.0/samples/digest_authentication.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      195 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/exception.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      164 2021-11-12 15:57:29.000000 webpie-5.9.0/samples/function_app.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      304 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/function_app2.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      534 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/getset.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      473 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/hello_time.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      135 2021-11-12 18:38:47.000000 webpie-5.9.0/samples/hello_world.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      302 2021-11-12 16:03:35.000000 webpie-5.9.0/samples/hello_world_relpath.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      246 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/hello_world_wsgi.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      913 2022-06-04 12:29:56.000000 webpie-5.9.0/samples/http_server.py
--rwxr-xr-x   0 ivm        (503) staff       (20)        0 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/https.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      277 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/https_server.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      146 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/lambda_app.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      589 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/make_response.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      773 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/nested_handlers.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     1553 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/permissions.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      275 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/post.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      231 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/post_client.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      207 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/post_print.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      446 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/post_receiver.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      358 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/redirect.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      270 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/relpath.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      987 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/robots.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      527 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/slow_server.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      744 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/standalone_server.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     1331 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/standalone_session_app.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      597 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/standalone_threaded_app.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      146 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/static_server.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      661 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/strict_handler.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      507 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/templates.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      923 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/test.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      544 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/threads_1.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      967 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/threads_2.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      568 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/threads_context.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      893 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/time_args.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      527 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/time_count.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      555 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/time_count_thread_safe.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     1196 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/time_handlers.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      858 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/time_hello_split.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      385 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/time_index.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     1276 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/time_returns.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     1316 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/time_server.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      555 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/uwsgi_app.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      639 2021-11-11 19:43:18.000000 webpie-5.9.0/samples/wp_test.py
--rw-r--r--   0 ivm        (503) staff       (20)       38 2022-10-11 12:16:44.000000 webpie-5.9.0/setup.cfg
--rwxr-xr-x   0 ivm        (503) staff       (20)     1874 2022-10-09 12:57:22.000000 webpie-5.9.0/setup.py
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-10-11 12:16:44.000000 webpie-5.9.0/webpie/
--rwxr-xr-x   0 ivm        (503) staff       (20)    22391 2022-10-11 00:22:59.000000 webpie-5.9.0/webpie/HTTPServer.py
--rwxr-xr-x   0 ivm        (503) staff       (20)       67 2022-10-11 12:16:12.000000 webpie-5.9.0/webpie/Version.py
--rwxr-xr-x   0 ivm        (503) staff       (20)    26173 2022-10-11 00:28:23.000000 webpie-5.9.0/webpie/WPApp.py
--rwxr-xr-x   0 ivm        (503) staff       (20)    17123 2021-11-11 19:43:18.000000 webpie-5.9.0/webpie/WPSessionApp.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      537 2022-06-04 12:29:56.000000 webpie-5.9.0/webpie/__init__.py
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-10-11 12:16:44.000000 webpie-5.9.0/webpie/logs/
--rw-r--r--   0 ivm        (503) staff       (20)      148 2022-06-23 16:48:39.000000 webpie-5.9.0/webpie/logs/__init__.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     5182 2022-06-23 16:48:39.000000 webpie-5.9.0/webpie/logs/log_file.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     4815 2022-10-09 12:57:22.000000 webpie-5.9.0/webpie/logs/logs.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      372 2021-11-11 19:43:18.000000 webpie-5.9.0/webpie/py3.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      978 2022-10-09 12:57:22.000000 webpie-5.9.0/webpie/uid.py
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-10-11 12:16:44.000000 webpie-5.9.0/webpie/webob/
--rwxr-xr-x   0 ivm        (503) staff       (20)      538 2021-11-11 19:43:18.000000 webpie-5.9.0/webpie/webob/__init__.py
--rwxr-xr-x   0 ivm        (503) staff       (20)   210210 2021-11-11 19:43:18.000000 webpie-5.9.0/webpie/webob/acceptparse.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     4744 2021-11-11 19:43:18.000000 webpie-5.9.0/webpie/webob/byterange.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     6772 2021-11-11 19:43:18.000000 webpie-5.9.0/webpie/webob/cachecontrol.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     6835 2021-11-11 19:43:18.000000 webpie-5.9.0/webpie/webob/client.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     7261 2021-11-11 19:43:18.000000 webpie-5.9.0/webpie/webob/compat.py
--rwxr-xr-x   0 ivm        (503) staff       (20)    31373 2021-11-11 19:43:18.000000 webpie-5.9.0/webpie/webob/cookies.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     2547 2021-11-11 19:43:18.000000 webpie-5.9.0/webpie/webob/datetime_utils.py
--rwxr-xr-x   0 ivm        (503) staff       (20)    10470 2021-11-11 19:43:18.000000 webpie-5.9.0/webpie/webob/dec.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     9192 2021-11-11 19:43:18.000000 webpie-5.9.0/webpie/webob/descriptors.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     3738 2021-11-11 19:43:18.000000 webpie-5.9.0/webpie/webob/etag.py
--rwxr-xr-x   0 ivm        (503) staff       (20)    38214 2021-11-11 19:43:18.000000 webpie-5.9.0/webpie/webob/exc.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     4076 2021-11-11 19:43:18.000000 webpie-5.9.0/webpie/webob/headers.py
--rwxr-xr-x   0 ivm        (503) staff       (20)    13940 2021-11-11 19:43:18.000000 webpie-5.9.0/webpie/webob/multidict.py
--rwxr-xr-x   0 ivm        (503) staff       (20)    58927 2021-11-11 19:43:18.000000 webpie-5.9.0/webpie/webob/request.py
--rwxr-xr-x   0 ivm        (503) staff       (20)    55415 2021-11-11 19:43:18.000000 webpie-5.9.0/webpie/webob/response.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     5628 2021-11-11 19:43:18.000000 webpie-5.9.0/webpie/webob/static.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     4833 2021-11-11 19:43:18.000000 webpie-5.9.0/webpie/webob/util.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     1115 2021-11-11 19:43:18.000000 webpie-5.9.0/webpie/yaml_expand.py
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-10-11 12:16:44.000000 webpie-5.9.0/webpie.egg-info/
--rw-r--r--   0 ivm        (503) staff       (20)    25245 2022-10-11 12:16:43.000000 webpie-5.9.0/webpie.egg-info/PKG-INFO
--rw-r--r--   0 ivm        (503) staff       (20)     2049 2022-10-11 12:16:43.000000 webpie-5.9.0/webpie.egg-info/SOURCES.txt
--rw-r--r--   0 ivm        (503) staff       (20)        1 2022-10-11 12:16:43.000000 webpie-5.9.0/webpie.egg-info/dependency_links.txt
--rw-r--r--   0 ivm        (503) staff       (20)      104 2022-10-11 12:16:43.000000 webpie-5.9.0/webpie.egg-info/entry_points.txt
--rw-r--r--   0 ivm        (503) staff       (20)        1 2022-06-16 13:16:58.000000 webpie-5.9.0/webpie.egg-info/not-zip-safe
--rw-r--r--   0 ivm        (503) staff       (20)       18 2022-10-11 12:16:43.000000 webpie-5.9.0/webpie.egg-info/requires.txt
--rw-r--r--   0 ivm        (503) staff       (20)       59 2022-10-11 12:16:43.000000 webpie-5.9.0/webpie.egg-info/top_level.txt
+drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-10-12 14:14:12.000000 webpie-5.9.1/
+-rw-r--r--   0 ivm        (503) staff       (20)    25245 2022-10-12 14:14:12.000000 webpie-5.9.1/PKG-INFO
+-rwxr-xr-x   0 ivm        (503) staff       (20)    19894 2022-06-04 12:29:34.000000 webpie-5.9.1/README.rst
+drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-10-12 14:14:12.000000 webpie-5.9.1/multiserver/
+-rwxr-xr-x   0 ivm        (503) staff       (20)    20762 2022-10-09 12:57:22.000000 webpie-5.9.1/multiserver/multiserver.py
+drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-10-12 14:14:12.000000 webpie-5.9.1/router/
+-rwxr-xr-x   0 ivm        (503) staff       (20)     7278 2021-11-11 19:43:18.000000 webpie-5.9.1/router/router.py
+drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-10-12 14:14:12.000000 webpie-5.9.1/samples/
+-rwxr-xr-x   0 ivm        (503) staff       (20)      793 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/callable_handler.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      344 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/clock.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     1037 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/date_time_simple.py
+-rw-r--r--   0 ivm        (503) staff       (20)     3668 2022-06-04 14:27:36.000000 webpie-5.9.1/samples/digest_authentication.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      195 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/exception.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      164 2021-11-12 15:57:29.000000 webpie-5.9.1/samples/function_app.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      304 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/function_app2.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      534 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/getset.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      473 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/hello_time.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      135 2021-11-12 18:38:47.000000 webpie-5.9.1/samples/hello_world.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      302 2021-11-12 16:03:35.000000 webpie-5.9.1/samples/hello_world_relpath.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      246 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/hello_world_wsgi.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      913 2022-06-04 12:29:56.000000 webpie-5.9.1/samples/http_server.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)        0 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/https.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      277 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/https_server.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      146 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/lambda_app.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      589 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/make_response.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      773 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/nested_handlers.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     1553 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/permissions.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      275 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/post.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      231 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/post_client.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      207 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/post_print.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      446 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/post_receiver.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      358 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/redirect.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      270 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/relpath.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      987 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/robots.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      527 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/slow_server.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      744 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/standalone_server.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     1331 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/standalone_session_app.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      597 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/standalone_threaded_app.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      146 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/static_server.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      661 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/strict_handler.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      507 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/templates.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      923 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/test.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      544 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/threads_1.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      967 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/threads_2.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      568 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/threads_context.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      893 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/time_args.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      527 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/time_count.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      555 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/time_count_thread_safe.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     1196 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/time_handlers.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      858 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/time_hello_split.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      385 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/time_index.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     1276 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/time_returns.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     1316 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/time_server.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      555 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/uwsgi_app.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      639 2021-11-11 19:43:18.000000 webpie-5.9.1/samples/wp_test.py
+-rw-r--r--   0 ivm        (503) staff       (20)       38 2022-10-12 14:14:12.000000 webpie-5.9.1/setup.cfg
+-rwxr-xr-x   0 ivm        (503) staff       (20)     1874 2022-10-09 12:57:22.000000 webpie-5.9.1/setup.py
+drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-10-12 14:14:12.000000 webpie-5.9.1/webpie/
+-rwxr-xr-x   0 ivm        (503) staff       (20)    22391 2022-10-11 00:22:59.000000 webpie-5.9.1/webpie/HTTPServer.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)       67 2022-10-12 14:13:55.000000 webpie-5.9.1/webpie/Version.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)    26275 2022-10-12 13:51:34.000000 webpie-5.9.1/webpie/WPApp.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)    17123 2021-11-11 19:43:18.000000 webpie-5.9.1/webpie/WPSessionApp.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      537 2022-06-04 12:29:56.000000 webpie-5.9.1/webpie/__init__.py
+drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-10-12 14:14:12.000000 webpie-5.9.1/webpie/logs/
+-rw-r--r--   0 ivm        (503) staff       (20)      148 2022-06-23 16:48:39.000000 webpie-5.9.1/webpie/logs/__init__.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     5182 2022-06-23 16:48:39.000000 webpie-5.9.1/webpie/logs/log_file.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     4815 2022-10-09 12:57:22.000000 webpie-5.9.1/webpie/logs/logs.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      372 2021-11-11 19:43:18.000000 webpie-5.9.1/webpie/py3.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)      978 2022-10-09 12:57:22.000000 webpie-5.9.1/webpie/uid.py
+drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-10-12 14:14:12.000000 webpie-5.9.1/webpie/webob/
+-rwxr-xr-x   0 ivm        (503) staff       (20)      538 2021-11-11 19:43:18.000000 webpie-5.9.1/webpie/webob/__init__.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)   210210 2021-11-11 19:43:18.000000 webpie-5.9.1/webpie/webob/acceptparse.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     4744 2021-11-11 19:43:18.000000 webpie-5.9.1/webpie/webob/byterange.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     6772 2021-11-11 19:43:18.000000 webpie-5.9.1/webpie/webob/cachecontrol.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     6835 2021-11-11 19:43:18.000000 webpie-5.9.1/webpie/webob/client.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     7261 2021-11-11 19:43:18.000000 webpie-5.9.1/webpie/webob/compat.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)    31373 2021-11-11 19:43:18.000000 webpie-5.9.1/webpie/webob/cookies.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     2547 2021-11-11 19:43:18.000000 webpie-5.9.1/webpie/webob/datetime_utils.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)    10470 2021-11-11 19:43:18.000000 webpie-5.9.1/webpie/webob/dec.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     9192 2021-11-11 19:43:18.000000 webpie-5.9.1/webpie/webob/descriptors.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     3738 2021-11-11 19:43:18.000000 webpie-5.9.1/webpie/webob/etag.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)    38214 2021-11-11 19:43:18.000000 webpie-5.9.1/webpie/webob/exc.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     4076 2021-11-11 19:43:18.000000 webpie-5.9.1/webpie/webob/headers.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)    13940 2021-11-11 19:43:18.000000 webpie-5.9.1/webpie/webob/multidict.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)    58927 2021-11-11 19:43:18.000000 webpie-5.9.1/webpie/webob/request.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)    55415 2021-11-11 19:43:18.000000 webpie-5.9.1/webpie/webob/response.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     5628 2021-11-11 19:43:18.000000 webpie-5.9.1/webpie/webob/static.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     4833 2021-11-11 19:43:18.000000 webpie-5.9.1/webpie/webob/util.py
+-rwxr-xr-x   0 ivm        (503) staff       (20)     1115 2021-11-11 19:43:18.000000 webpie-5.9.1/webpie/yaml_expand.py
+drwxr-xr-x   0 ivm        (503) staff       (20)        0 2022-10-12 14:14:12.000000 webpie-5.9.1/webpie.egg-info/
+-rw-r--r--   0 ivm        (503) staff       (20)    25245 2022-10-12 14:14:11.000000 webpie-5.9.1/webpie.egg-info/PKG-INFO
+-rw-r--r--   0 ivm        (503) staff       (20)     2049 2022-10-12 14:14:11.000000 webpie-5.9.1/webpie.egg-info/SOURCES.txt
+-rw-r--r--   0 ivm        (503) staff       (20)        1 2022-10-12 14:14:11.000000 webpie-5.9.1/webpie.egg-info/dependency_links.txt
+-rw-r--r--   0 ivm        (503) staff       (20)      104 2022-10-12 14:14:11.000000 webpie-5.9.1/webpie.egg-info/entry_points.txt
+-rw-r--r--   0 ivm        (503) staff       (20)        1 2022-06-16 13:16:58.000000 webpie-5.9.1/webpie.egg-info/not-zip-safe
+-rw-r--r--   0 ivm        (503) staff       (20)       18 2022-10-12 14:14:11.000000 webpie-5.9.1/webpie.egg-info/requires.txt
+-rw-r--r--   0 ivm        (503) staff       (20)       59 2022-10-12 14:14:11.000000 webpie-5.9.1/webpie.egg-info/top_level.txt
```

### Comparing `webpie-5.9.0/PKG-INFO` & `webpie-5.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: webpie
-Version: 5.9.0
+Version: 5.9.1
 Summary: A set of useful tools built on top of standard Python threading module
 Home-page: https://webpie.github.io/
 Author: Igor Mandrichenko
 Author-email: igorvm@gmail.com
 License: BSD 3-clause
 Description: 
         WebPie
```

### Comparing `webpie-5.9.0/README.rst` & `webpie-5.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/multiserver/multiserver.py` & `webpie-5.9.1/multiserver/multiserver.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/router/router.py` & `webpie-5.9.1/router/router.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/callable_handler.py` & `webpie-5.9.1/samples/callable_handler.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/date_time_simple.py` & `webpie-5.9.1/samples/date_time_simple.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/digest_authentication.py` & `webpie-5.9.1/samples/digest_authentication.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/getset.py` & `webpie-5.9.1/samples/getset.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/http_server.py` & `webpie-5.9.1/samples/http_server.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/make_response.py` & `webpie-5.9.1/samples/make_response.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/nested_handlers.py` & `webpie-5.9.1/samples/nested_handlers.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/permissions.py` & `webpie-5.9.1/samples/permissions.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/robots.py` & `webpie-5.9.1/samples/robots.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/slow_server.py` & `webpie-5.9.1/samples/slow_server.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/standalone_server.py` & `webpie-5.9.1/samples/standalone_server.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/standalone_session_app.py` & `webpie-5.9.1/samples/standalone_session_app.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/standalone_threaded_app.py` & `webpie-5.9.1/samples/standalone_threaded_app.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/strict_handler.py` & `webpie-5.9.1/samples/strict_handler.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/test.py` & `webpie-5.9.1/samples/test.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/threads_1.py` & `webpie-5.9.1/samples/threads_1.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/threads_2.py` & `webpie-5.9.1/samples/threads_2.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/threads_context.py` & `webpie-5.9.1/samples/threads_context.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/time_args.py` & `webpie-5.9.1/samples/time_args.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/time_count.py` & `webpie-5.9.1/samples/time_count.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/time_count_thread_safe.py` & `webpie-5.9.1/samples/time_count_thread_safe.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/time_handlers.py` & `webpie-5.9.1/samples/time_handlers.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/time_hello_split.py` & `webpie-5.9.1/samples/time_hello_split.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/time_returns.py` & `webpie-5.9.1/samples/time_returns.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/time_server.py` & `webpie-5.9.1/samples/time_server.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/uwsgi_app.py` & `webpie-5.9.1/samples/uwsgi_app.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/samples/wp_test.py` & `webpie-5.9.1/samples/wp_test.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/setup.py` & `webpie-5.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/HTTPServer.py` & `webpie-5.9.1/webpie/HTTPServer.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/WPApp.py` & `webpie-5.9.1/webpie/WPApp.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,14 +460,15 @@
         self.ScriptHome = None
         self.Initialized = False
         self.Prefix = prefix            # this prefix will be removed from the URL path before the mapping to the method
         self.ReplacePrefix = replace_prefix     # this prefix will be added after self.Prefix was removed
         self.HandlerParams = []
         self.HandlerArgs = {}
         self.Environ = environ
+        print("App initialized at prefix:", prefix, "   replace prefix:", replace_prefix)
         
     def _app_lock(self):
         return self._AppLock
         
     def __enter__(self):
         return self._AppLock.__enter__()
         
@@ -535,21 +536,23 @@
             if path == self.Prefix:
                 matched = path
             elif path.startswith(self.Prefix + '/'):
                 matched = self.Prefix
                 
             if matched is None:
                 return None
-                
+
+            path = path[len(matched):]
+
             if self.ReplacePrefix:
-                path = self.ReplacePrefix + path[len(matched):]
+                path = self.ReplacePrefix + path
                 
-            path = path or "/"
+            path = self.canonicPath(path or "/")
             #print(f"converted to: [{path}]")
-                
+
         return path
         
     def handler_options(self, *params, **args):
         self.HandlerParams = params
         self.HandlerArgs = args
         return self
 
@@ -776,8 +779,8 @@
     
     class MyApp(WPApp):
         pass
         
     class MyHandler(WPHandler):
         pass
             
-    MyApp(MyHandler).run_server(8080)
+    MyApp(MyHandler).run_server(8080)
```

### Comparing `webpie-5.9.0/webpie/WPSessionApp.py` & `webpie-5.9.1/webpie/WPSessionApp.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/__init__.py` & `webpie-5.9.1/webpie/__init__.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/logs/log_file.py` & `webpie-5.9.1/webpie/logs/log_file.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/logs/logs.py` & `webpie-5.9.1/webpie/logs/logs.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/uid.py` & `webpie-5.9.1/webpie/uid.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/webob/__init__.py` & `webpie-5.9.1/webpie/webob/__init__.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/webob/acceptparse.py` & `webpie-5.9.1/webpie/webob/acceptparse.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/webob/byterange.py` & `webpie-5.9.1/webpie/webob/byterange.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/webob/cachecontrol.py` & `webpie-5.9.1/webpie/webob/cachecontrol.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/webob/client.py` & `webpie-5.9.1/webpie/webob/client.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/webob/compat.py` & `webpie-5.9.1/webpie/webob/compat.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/webob/cookies.py` & `webpie-5.9.1/webpie/webob/cookies.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/webob/datetime_utils.py` & `webpie-5.9.1/webpie/webob/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/webob/dec.py` & `webpie-5.9.1/webpie/webob/dec.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/webob/descriptors.py` & `webpie-5.9.1/webpie/webob/descriptors.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/webob/etag.py` & `webpie-5.9.1/webpie/webob/etag.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/webob/exc.py` & `webpie-5.9.1/webpie/webob/exc.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/webob/headers.py` & `webpie-5.9.1/webpie/webob/headers.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/webob/multidict.py` & `webpie-5.9.1/webpie/webob/multidict.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/webob/request.py` & `webpie-5.9.1/webpie/webob/request.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/webob/response.py` & `webpie-5.9.1/webpie/webob/response.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/webob/static.py` & `webpie-5.9.1/webpie/webob/static.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/webob/util.py` & `webpie-5.9.1/webpie/webob/util.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie/yaml_expand.py` & `webpie-5.9.1/webpie/yaml_expand.py`

 * *Files identical despite different names*

### Comparing `webpie-5.9.0/webpie.egg-info/PKG-INFO` & `webpie-5.9.1/webpie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: webpie
-Version: 5.9.0
+Version: 5.9.1
 Summary: A set of useful tools built on top of standard Python threading module
 Home-page: https://webpie.github.io/
 Author: Igor Mandrichenko
 Author-email: igorvm@gmail.com
 License: BSD 3-clause
 Description: 
         WebPie
```

### Comparing `webpie-5.9.0/webpie.egg-info/SOURCES.txt` & `webpie-5.9.1/webpie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

